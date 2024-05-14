# Comparing `tmp/example990420-1.1.0.tar.gz` & `tmp/example990420-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-1.1.0.tar", last modified: Sun Apr 28 02:17:08 2024, max compression
+gzip compressed data, was "example990420-1.1.1.tar", last modified: Wed May  1 20:28:08 2024, max compression
```

## Comparing `example990420-1.1.0.tar` & `example990420-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 02:17:08.012819 example990420-1.1.0/
--rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    13004 2024-04-28 02:17:08.011634 example990420-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    12204 2024-04-28 01:15:26.000000 example990420-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 02:17:08.006224 example990420-1.1.0/example990420.egg-info/
--rw-rw-rw-   0        0        0    13004 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 02:17:07.000000 example990420-1.1.0/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       50 2024-04-28 02:07:06.000000 example990420-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      882 2024-04-28 02:17:08.018963 example990420-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 02:17:07.982112 example990420-1.1.0/taibun/
--rw-rw-rw-   0        0        0       85 2024-04-27 02:04:57.000000 example990420-1.1.0/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 02:17:07.992912 example990420-1.1.0/taibun/data/
--rw-rw-rw-   0        0        0    17160 2024-04-27 02:06:10.000000 example990420-1.1.0/taibun/data/simplified.json
--rw-rw-rw-   0        0        0  1893344 2024-04-28 00:12:08.000000 example990420-1.1.0/taibun/data/words.json
--rw-rw-rw-   0        0        0    25042 2024-04-28 00:18:10.000000 example990420-1.1.0/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:08.628515 example990420-1.1.1/
+-rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 example990420-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    14713 2024-05-01 20:28:08.627508 example990420-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13913 2024-05-01 20:27:29.000000 example990420-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:08.624141 example990420-1.1.1/example990420.egg-info/
+-rw-rw-rw-   0        0        0    14713 2024-05-01 20:28:08.000000 example990420-1.1.1/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2024-05-01 20:28:08.000000 example990420-1.1.1/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:28:08.000000 example990420-1.1.1/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 20:28:08.000000 example990420-1.1.1/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       50 2024-04-28 02:07:06.000000 example990420-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2024-05-01 20:28:08.641743 example990420-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:08.564271 example990420-1.1.1/taibun/
+-rw-rw-rw-   0        0        0       85 2024-04-27 02:04:57.000000 example990420-1.1.1/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:08.570060 example990420-1.1.1/taibun/data/
+-rw-rw-rw-   0        0        0    17179 2024-04-29 21:05:07.000000 example990420-1.1.1/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0  1893345 2024-04-29 20:09:25.000000 example990420-1.1.1/taibun/data/words.json
+-rw-rw-rw-   0        0        0    25617 2024-05-01 09:33:10.000000 example990420-1.1.1/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:08.621094 example990420-1.1.1/tests/
+-rw-rw-rw-   0        0        0      871 2024-04-30 01:24:16.000000 example990420-1.1.1/tests/test_additional.py
+-rw-rw-rw-   0        0        0    17991 2024-05-01 08:36:51.000000 example990420-1.1.1/tests/test_convert_non_cjk.py
+-rw-rw-rw-   0        0        0     9435 2024-04-29 20:28:54.000000 example990420-1.1.1/tests/test_delimiter.py
+-rw-rw-rw-   0        0        0     7052 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_format.py
+-rw-rw-rw-   0        0        0    21528 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_ipa_conversion.py
+-rw-rw-rw-   0        0        0     9356 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_pingyim_conversion.py
+-rw-rw-rw-   0        0        0     9815 2023-12-27 21:54:31.000000 example990420-1.1.1/tests/test_poj_conversion.py
+-rw-rw-rw-   0        0        0    12568 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_punctuation.py
+-rw-rw-rw-   0        0        0    34119 2024-05-01 06:33:17.000000 example990420-1.1.1/tests/test_sandhi.py
+-rw-rw-rw-   0        0        0     9724 2023-12-27 21:54:31.000000 example990420-1.1.1/tests/test_tailo_conversion.py
+-rw-rw-rw-   0        0        0     9818 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_tlpa_conversion.py
+-rw-rw-rw-   0        0        0     1097 2024-04-29 21:08:07.000000 example990420-1.1.1/tests/test_tokenisation.py
+-rw-rw-rw-   0        0        0     9702 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_tongiong_conversion.py
+-rw-rw-rw-   0        0        0    14164 2024-04-27 00:02:02.000000 example990420-1.1.1/tests/test_zhuyin_conversion.py
```

### Comparing `example990420-1.1.0/LICENSE` & `example990420-1.1.1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Andrei Harbachov
+Copyright (c) 2023-2024 Andrei Harbachov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `example990420-1.1.0/PKG-INFO` & `example990420-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,813 +1,870 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7861  : 2.1..Name: exa
-00000020: 6d70 6c65 3939 3034 3230 0d0a 5665 7273  mple990420..Vers
-00000030: 696f 6e3a 2031 2e31 2e30 0d0a 5375 6d6d  ion: 1.1.0..Summ
-00000040: 6172 793a 2054 6169 7761 6e65 7365 2048  ary: Taiwanese H
-00000050: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
-00000060: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
-00000070: 7365 720d 0a48 6f6d 652d 7061 6765 3a20  ser..Home-page: 
-00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000090: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
-000000a0: 6275 6e0d 0a41 7574 686f 723a 2041 6e64  bun..Author: And
-000000b0: 7265 6920 4861 7262 6163 686f 760d 0a41  rei Harbachov..A
-000000c0: 7574 686f 722d 656d 6169 6c3a 2061 6e64  uthor-email: and
-000000d0: 7265 692e 6861 7262 6163 686f 7640 676d  rei.harbachov@gm
-000000e0: 6169 6c2e 636f 6d0d 0a4c 6963 656e 7365  ail.com..License
-000000f0: 3a20 4d49 540d 0a4b 6579 776f 7264 733a  : MIT..Keywords:
-00000100: 2070 7974 686f 6e2c 7461 6977 616e 2c74   python,taiwan,t
-00000110: 6169 7761 6e65 7365 2c74 6169 6769 2c68  aiwanese,taigi,h
-00000120: 6f6b 6b69 656e 2c72 6f6d 616e 697a 6174  okkien,romanizat
-00000130: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
-00000140: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
-00000150: 6f72 2c74 6f6b 656e 697a 6174 696f 6e2c  or,tokenization,
-00000160: 746f 6b65 6e69 7a65 720d 0a43 6c61 7373  tokenizer..Class
-00000170: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-00000180: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
-00000190: 3a3a 204c 696e 6775 6973 7469 630d 0a43  :: Linguistic..C
-000001a0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-000001b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-000001c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
-000001d0: 5374 6162 6c65 0d0a 436c 6173 7369 6669  Stable..Classifi
-000001e0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
-000001f0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000200: 6572 730d 0a43 6c61 7373 6966 6965 723a  ers..Classifier:
-00000210: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000230: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
-00000240: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-00000250: 656d 203a 3a20 556e 6978 0d0a 436c 6173  em :: Unix..Clas
-00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000270: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
-00000280: 5320 3a3a 204d 6163 4f53 2058 0d0a 436c  S :: MacOS X..Cl
-00000290: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-000002a0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-000002b0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-000002c0: 7773 0d0a 5265 7175 6972 6573 2d50 7974  ws..Requires-Pyt
-000002d0: 686f 6e3a 203e 3d33 2e38 0d0a 4465 7363  hon: >=3.8..Desc
-000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000300: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
-00000310: 653a 204c 4943 454e 5345 0d0a 0d0a 3c21  e: LICENSE....<!
-00000320: 2d2d 2050 524f 4a45 4354 204c 4f47 4f20  -- PROJECT LOGO 
-00000330: 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c 6469  -->..<br />..<di
-00000340: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000350: 3e0d 0a20 200d 0a23 2054 6169 6275 6e0d  >..  ..# Taibun.
-00000360: 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052 4f4a  .......<!-- PROJ
-00000370: 4543 5420 5348 4945 4c44 5320 2d2d 3e0d  ECT SHIELDS -->.
-00000380: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
-00000390: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
-000003a0: 0a5b 215b 436f 6e74 7269 6275 746f 7273  .[![Contributors
-000003b0: 5d5b 636f 6e74 7269 6275 746f 7273 2d62  ][contributors-b
-000003c0: 6164 6765 5d5d 5b63 6f6e 7472 6962 7574  adge]][contribut
-000003d0: 6f72 735d 0d0a 5b21 5b52 656c 6561 7365  ors]..[![Release
-000003e0: 5d5b 7265 6c65 6173 652d 6261 6467 655d  ][release-badge]
-000003f0: 5d5b 7265 6c65 6173 655d 0d0a 5b21 5b4c  ][release]..[![L
-00000400: 6963 656e 6365 5d5b 6c69 6365 6e63 652d  icence][licence-
-00000410: 6261 6467 655d 5d5b 6c69 6365 6e63 655d  badge]][licence]
-00000420: 0d0a 5b21 5b4c 696e 6b65 6449 6e5d 5b6c  ..[![LinkedIn][l
-00000430: 696e 6b65 6469 6e2d 6261 6467 655d 5d5b  inkedin-badge]][
-00000440: 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a 2a54  linkedin]....**T
-00000450: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000460: 2054 7261 6e73 6c69 7465 7261 746f 7220   Transliterator 
-00000470: 616e 6420 546f 6b65 6e69 7365 722a 2a0d  and Tokeniser**.
-00000480: 0a0d 0a49 7420 6861 7320 6d65 7468 6f64  ...It has method
-00000490: 7320 7468 6174 2061 6c6c 6f77 2074 6f20  s that allow to 
-000004a0: 6375 7374 6f6d 6973 6520 7472 616e 736c  customise transl
-000004b0: 6974 6572 6174 696f 6e20 616e 6420 7265  iteration and re
-000004c0: 7472 6965 7665 2061 6e79 206e 6563 6573  trieve any neces
-000004d0: 7361 7279 2069 6e66 6f72 6d61 7469 6f6e  sary information
-000004e0: 2061 626f 7574 2054 6169 7761 6e65 7365   about Taiwanese
-000004f0: 2048 6f6b 6b69 656e 2070 726f 6e75 6e63   Hokkien pronunc
-00000500: 6961 7469 6f6e 2e3c 6272 202f 3e0d 0a49  iation.<br />..I
-00000510: 6e63 6c75 6465 7320 776f 7264 2074 6f6b  ncludes word tok
-00000520: 656e 6973 6572 2066 6f72 2054 6169 7761  eniser for Taiwa
-00000530: 6e65 7365 2048 6f6b 6b69 656e 2e0d 0a0d  nese Hokkien....
-00000540: 0a5b 5265 706f 7274 2042 7567 5d5b 6275  .[Report Bug][bu
-00000550: 675d 20e2 80a2 0d0a 5b50 7950 495d 5b70  g] .....[PyPI][p
-00000560: 7970 695d 0d0a 0d0a 3c2f 6469 763e 0d0a  ypi]....</div>..
-00000570: 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d 0a0d  ......---.......
-00000580: 0a3c 212d 2d20 494e 5354 414c 4c20 2d2d  .<!-- INSTALL --
-00000590: 3e0d 0a23 2320 496e 7374 616c 6c0d 0a0d  >..## Install...
-000005a0: 0a54 6169 6275 6e20 6361 6e20 6265 2069  .Taibun can be i
-000005b0: 6e73 7461 6c6c 6564 2066 726f 6d20 5b70  nstalled from [p
-000005c0: 7970 695d 5b70 7970 695d 0d0a 0d0a 6060  ypi][pypi]....``
-000005d0: 6062 6173 680d 0a24 2070 6970 2069 6e73  `bash..$ pip ins
-000005e0: 7461 6c6c 2074 6169 6275 6e0d 0a60 6060  tall taibun..```
-000005f0: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055 5341  ........<!-- USA
-00000600: 4745 202d 2d3e 0d0a 2323 2055 7361 6765  GE -->..## Usage
-00000610: 0d0a 0d0a 2323 2320 436f 6e76 6572 7465  ....### Converte
-00000620: 720d 0a0d 0a60 436f 6e76 6572 7465 7260  r....`Converter`
-00000630: 2063 6c61 7373 2074 7261 6e73 6c69 7465   class translite
-00000640: 7261 7465 7320 7468 6520 4368 696e 6573  rates the Chines
-00000650: 6520 6368 6172 6163 7465 7273 2074 6f20  e characters to 
-00000660: 7468 6520 6368 6f73 656e 2074 7261 6e73  the chosen trans
-00000670: 6c69 7465 7261 7469 6f6e 2073 7973 7465  literation syste
-00000680: 6d20 7769 7468 2070 6172 616d 6574 6572  m with parameter
-00000690: 7320 7370 6563 6966 6965 6420 6279 2074  s specified by t
-000006a0: 6865 2064 6576 656c 6f70 6572 2e20 576f  he developer. Wo
-000006b0: 726b 7320 666f 7220 626f 7468 2054 7261  rks for both Tra
-000006c0: 6469 7469 6f6e 616c 2061 6e64 2053 696d  ditional and Sim
-000006d0: 706c 6966 6965 6420 6368 6172 6163 7465  plified characte
-000006e0: 7273 2e0d 0a0d 0a60 6060 7079 7468 6f6e  rs.....```python
-000006f0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
-00000700: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
-00000710: 7973 7465 6d2c 2064 6961 6c65 6374 2c20  ystem, dialect, 
-00000720: 666f 726d 6174 2c20 6465 6c69 6d69 7465  format, delimite
-00000730: 722c 2073 616e 6468 692c 2070 756e 6374  r, sandhi, punct
-00000740: 7561 7469 6f6e 2c20 636f 6e76 6572 745f  uation, convert_
-00000750: 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320 7472  non_cjk)....# tr
-00000760: 616e 736c 6974 6572 6174 6520 4368 696e  ansliterate Chin
-00000770: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
-00000780: 632e 6765 7428 696e 7075 7429 0d0a 6060  c.get(input)..``
-00000790: 600d 0a0d 0a23 2323 2320 5379 7374 656d  `....#### System
-000007a0: 0d0a 0d0a 6073 7973 7465 6d60 2053 7472  ....`system` Str
-000007b0: 696e 6720 2d20 7379 7374 656d 206f 6620  ing - system of 
-000007c0: 7472 616e 736c 6974 6572 6174 696f 6e2e  transliteration.
-000007d0: 0d0a 0d0a 2a20 6054 6169 6c6f 6020 2864  ....* `Tailo` (d
-000007e0: 6566 6175 6c74 2920 2d20 5b54 c3a2 692d  efault) - [T..i-
-000007f0: 75c3 a26e 204c c3b4 2d6d c3a1 2d6a c4ab  u..n L..-m..-j..
-00000800: 2050 6869 6e67 2d69 6d20 486f 6e67 2dc3   Phing-im Hong-.
-00000810: a06e 5d5b 7461 696c 6f2d 7769 6b69 5d0d  .n][tailo-wiki].
-00000820: 0a2a 2060 504f 4a60 202d 205b 5065 cc8d  .* `POJ` - [Pe..
-00000830: 682d c58d 652d 6ac4 ab5d 5b70 6f6a 2d77  h-..e-j..][poj-w
-00000840: 696b 695d 0d0a 2a20 605a 6875 7969 6e60  iki]..* `Zhuyin`
-00000850: 202d 205b 5461 6977 616e 6573 6520 5068   - [Taiwanese Ph
-00000860: 6f6e 6574 6963 2053 796d 626f 6c73 5d5b  onetic Symbols][
-00000870: 7a68 7579 696e 2d77 696b 695d 0d0a 2a20  zhuyin-wiki]..* 
-00000880: 6054 4c50 4160 202d 205b 5461 6977 616e  `TLPA` - [Taiwan
-00000890: 6573 6520 4c61 6e67 7561 6765 2050 686f  ese Language Pho
-000008a0: 6e65 7469 6320 416c 7068 6162 6574 5d5b  netic Alphabet][
-000008b0: 746c 7061 2d77 696b 695d 0d0a 2a20 6050  tlpa-wiki]..* `P
-000008c0: 696e 6779 696d 6020 2d20 5b42 62c3 a16e  ingyim` - [Bb..n
-000008d0: 6cc3 a16d 2055 c493 2050 c3ac 6e67 79c4  l..m U.. P..ngy.
-000008e0: ab6d 2048 c58d 6e67 27c3 a06e 5d5b 7069  .m H..ng'..n][pi
-000008f0: 6e67 7969 6d2d 7769 6b69 5d0d 0a2a 2060  ngyim-wiki]..* `
-00000900: 546f 6e67 696f 6e67 6020 2d20 5b44 61c4  Tongiong` - [Da.
-00000910: ab2d 6768 c3ae 2054 c58d 6e67 2d69 c58d  .-gh.. T..ng-i..
-00000920: 6e67 2050 c4ab 6e67 2d69 6d5d 5b74 6f6e  ng P..ng-im][ton
-00000930: 6769 6f6e 672d 7769 6b69 5d0d 0a2a 2060  giong-wiki]..* `
-00000940: 4950 4160 202d 205b 496e 7465 726e 6174  IPA` - [Internat
-00000950: 696f 6e61 6c20 5068 6f6e 6574 6963 2041  ional Phonetic A
-00000960: 6c70 6861 6265 745d 5b69 7061 2d77 696b  lphabet][ipa-wik
-00000970: 695d 0d0a 0d0a 7c20 7465 7874 207c 2054  i]....| text | T
-00000980: 6169 6c6f 2020 207c 2050 4f4a 2020 2020  ailo   | POJ    
-00000990: 207c 205a 6875 7969 6e20 2020 2020 207c   | Zhuyin      |
-000009a0: 2054 4c50 4120 2020 2020 207c 2050 696e   TLPA      | Pin
-000009b0: 6779 696d 207c 2054 6f6e 6769 6f6e 6720  gyim | Tongiong 
-000009c0: 7c20 4950 4120 2020 2020 2020 2020 7c0d  | IPA         |.
-000009d0: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
-000009e0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
-000009f0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00000a00: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20  ----- | ------- 
-00000a10: 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  | -------- | ---
-00000a20: 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20 e58f  -------- |..| ..
-00000a30: b0e7 81a3 207c 2054 c3a2 692d 75c3 a26e  .... | T..i-u..n
-00000a40: 207c 2054 c3a2 692d 6fc3 a26e 207c 20e3   | T..i-o..n | .
-00000a50: 8489 e384 9ecb 8a20 e384 a8e3 84a2 cb8a  ....... ........
-00000a60: 207c 2054 6169 3520 7561 6e35 207c 2044   | Tai5 uan5 | D
-00000a70: c3a1 6977 c3a1 6e20 207c 2054 c481 692d  ..iw..n  | T..i-
-00000a80: 75c7 8e6e 2020 7c20 5461 69c2 b2e2 81b5  u..n  | Tai.....
-00000a90: 2075 616e c2b2 e281 b520 7c0d 0a0d 0a23   uan..... |....#
-00000aa0: 2323 2320 4469 616c 6563 740d 0a0d 0a60  ### Dialect....`
-00000ab0: 6469 616c 6563 7460 2053 7472 696e 6720  dialect` String 
-00000ac0: 2d20 7072 6566 6572 7265 6420 7072 6f6e  - preferred pron
-00000ad0: 756e 6369 6174 696f 6e2e 0d0a 0d0a 2a20  unciation.....* 
-00000ae0: 6073 6f75 7468 6020 2864 6566 6175 6c74  `south` (default
-00000af0: 2920 2d20 5b5a 6861 6e67 7a68 6f75 5d5b  ) - [Zhangzhou][
-00000b00: 7a68 616e 677a 686f 752d 7769 6b69 5d2d  zhangzhou-wiki]-
-00000b10: 6c65 616e 696e 6720 7072 6f6e 756e 6369  leaning pronunci
-00000b20: 6174 696f 6e0d 0a2a 2060 6e6f 7274 6860  ation..* `north`
-00000b30: 202d 205b 5175 616e 7a68 6f75 5d5b 7175   - [Quanzhou][qu
-00000b40: 616e 7a68 6f75 2d77 696b 695d 2d6c 6561  anzhou-wiki]-lea
-00000b50: 6e69 6e67 2070 726f 6e75 6e63 6961 7469  ning pronunciati
-00000b60: 6f6e 0d0a 0d0a 7c20 7465 7874 2020 207c  on....| text   |
-00000b70: 2073 6f75 7468 2020 2020 2020 2020 207c   south         |
-00000b80: 206e 6f72 7468 2020 2020 2020 2020 207c   north         |
-00000b90: 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d 2d2d  ..| ------ | ---
-00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
-00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
-00000bc0: e4ba 94e6 9c88 e7af 8020 7c20 47c5 8d6f  ......... | G..o
-00000bd0: 2d67 7565 cc8d 682d 7473 6568 207c 2047  -gue..h-tseh | G
-00000be0: c58d 6f2d 6765 cc8d 682d 7473 7565 6820  ..o-ge..h-tsueh 
-00000bf0: 7c0d 0a0d 0a23 2323 2320 466f 726d 6174  |....#### Format
-00000c00: 0d0a 0d0a 6066 6f72 6d61 7460 2053 7472  ....`format` Str
-00000c10: 696e 6720 2d20 666f 726d 6174 2069 6e20  ing - format in 
-00000c20: 7768 6963 6820 746f 6e65 7320 7769 6c6c  which tones will
-00000c30: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
-00000c40: 696e 2074 6865 2063 6f6e 7665 7274 6564  in the converted
-00000c50: 2073 656e 7465 6e63 652e 0d0a 0d0a 2a20   sentence.....* 
-00000c60: 606d 6172 6b60 2028 6465 6661 756c 7429  `mark` (default)
-00000c70: 202d 2075 7365 7320 6469 6163 7269 7469   - uses diacriti
-00000c80: 6373 2066 6f72 2065 6163 6820 7379 6c6c  cs for each syll
-00000c90: 6162 6c65 2e20 4e6f 7420 6176 6169 6c61  able. Not availa
-00000ca0: 626c 6520 666f 7220 544c 5041 2e0d 0a2a  ble for TLPA...*
-00000cb0: 2060 6e75 6d62 6572 6020 2d20 6164 6420   `number` - add 
-00000cc0: 6120 6e75 6d62 6572 2077 6869 6368 2072  a number which r
-00000cd0: 6570 7265 7365 6e74 7320 7468 6520 746f  epresents the to
-00000ce0: 6e65 2061 7420 7468 6520 656e 6420 6f66  ne at the end of
-00000cf0: 2074 6865 2073 796c 6c61 626c 650d 0a2a   the syllable..*
-00000d00: 2060 7374 7269 7060 202d 2072 656d 6f76   `strip` - remov
-00000d10: 6573 2061 6e79 2074 6f6e 6520 6d61 726b  es any tone mark
-00000d20: 696e 670d 0a0d 0a7c 2074 6578 7420 7c20  ing....| text | 
-00000d30: 6d61 726b 2020 2020 7c20 6e75 6d62 6572  mark    | number
-00000d40: 2020 2020 7c20 7374 7269 7020 2020 7c0d      | strip   |.
-00000d50: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
-00000d60: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20 7c20  - | --------- | 
-00000d70: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0  ------- |..| ...
-00000d80: e781 a320 7c20 54c3 a269 2d75 c3a2 6e20  ... | T..i-u..n 
-00000d90: 7c20 5461 6935 2d75 616e 3520 7c20 5461  | Tai5-uan5 | Ta
-00000da0: 692d 7561 6e20 7c0d 0a0d 0a23 2323 2320  i-uan |....#### 
-00000db0: 4465 6c69 6d69 7465 720d 0a0d 0a60 6465  Delimiter....`de
-00000dc0: 6c69 6d69 7465 7260 2053 7472 696e 6720  limiter` String 
-00000dd0: 2d20 7365 7473 2074 6865 2064 656c 696d  - sets the delim
-00000de0: 6974 6572 2063 6861 7261 6374 6572 2074  iter character t
-00000df0: 6861 7420 7769 6c6c 2062 6520 706c 6163  hat will be plac
-00000e00: 6564 2069 6e20 6265 7477 6565 6e20 7379  ed in between sy
-00000e10: 6c6c 6162 6c65 7320 6f66 2061 2077 6f72  llables of a wor
-00000e20: 642e 0d0a 0d0a 4465 6661 756c 7420 7661  d.....Default va
-00000e30: 6c75 6520 6465 7065 6e64 7320 6f6e 2074  lue depends on t
-00000e40: 6865 2063 686f 7365 6e20 6073 7973 7465  he chosen `syste
-00000e50: 6d60 3a0d 0a0d 0a2a 2060 272d 2760 202d  m`:....* `'-'` -
-00000e60: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
-00000e70: 4f4a 602c 2060 546f 6e67 696f 6e67 600d  OJ`, `Tongiong`.
-00000e80: 0a2a 2060 2727 6020 2d20 666f 7220 6050  .* `''` - for `P
-00000e90: 696e 6779 696d 600d 0a2a 2060 2720 2760  ingyim`..* `' '`
-00000ea0: 202d 2066 6f72 2060 5a68 7579 696e 602c   - for `Zhuyin`,
-00000eb0: 2060 544c 5041 602c 2060 4950 4160 0d0a   `TLPA`, `IPA`..
-00000ec0: 0d0a 7c20 7465 7874 207c 2027 2d27 2020  ..| text | '-'  
-00000ed0: 2020 207c 2027 2720 2020 2020 7c20 2720     | ''     | ' 
-00000ee0: 2720 2020 2020 7c0d 0a7c 202d 2d2d 2d20  '     |..| ---- 
-00000ef0: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
-00000f00: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
-00000f10: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
-00000f20: 75c3 a26e 207c 2054 c3a2 6975 c3a2 6e20  u..n | T..iu..n 
-00000f30: 7c20 54c3 a269 2075 c3a2 6e20 7c0d 0a0d  | T..i u..n |...
-00000f40: 0a23 2323 2320 5361 6e64 6869 0d0a 0d0a  .#### Sandhi....
-00000f50: 6073 616e 6468 6960 2053 7472 696e 6720  `sandhi` String 
-00000f60: 2d20 6170 706c 6965 7320 7468 6520 5b73  - applies the [s
-00000f70: 616e 6468 6920 7275 6c65 7320 6f66 2054  andhi rules of T
-00000f80: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000f90: 5d5b 7361 6e64 6869 2d77 696b 695d 2074  ][sandhi-wiki] t
-00000fa0: 6f20 7379 6c6c 6162 6c65 7320 6f66 2061  o syllables of a
-00000fb0: 2073 696e 676c 6520 776f 7264 2e0d 0a0d   single word....
-00000fc0: 0a53 696e 6365 2069 7427 7320 6469 6666  .Since it's diff
-00000fd0: 6963 756c 7420 746f 2065 6e63 6f64 6520  icult to encode 
-00000fe0: 616c 6c20 7361 6e64 6869 2072 756c 6573  all sandhi rules
-00000ff0: 2c20 5461 6962 756e 2070 726f 7669 6465  , Taibun provide
-00001000: 7320 6d75 6c74 6970 6c65 206d 6f64 6573  s multiple modes
-00001010: 2066 6f72 2073 616e 6468 6920 636f 6e76   for sandhi conv
-00001020: 6572 7369 6f6e 2074 6f20 616c 6c6f 7720  ersion to allow 
-00001030: 666f 7220 6375 7374 6f6d 6973 6564 2073  for customised s
-00001040: 616e 6468 6920 6861 6e64 6c69 6e67 2e0d  andhi handling..
-00001050: 0a0d 0a2a 2060 6e6f 6e65 6020 2d20 646f  ...* `none` - do
-00001060: 6573 6e27 7420 7065 7266 6f72 6d20 616e  esn't perform an
-00001070: 7920 746f 6e65 2073 616e 6468 690d 0a2a  y tone sandhi..*
-00001080: 2060 6175 746f 6020 2d20 636c 6f73 6573   `auto` - closes
-00001090: 7420 6170 7072 6f78 696d 6174 696f 6e20  t approximation 
-000010a0: 746f 2066 756c 6c20 636f 7272 6563 7420  to full correct 
-000010b0: 746f 6e65 2073 616e 6468 6920 6f66 2054  tone sandhi of T
-000010c0: 6169 7761 6e65 7365 2c20 7769 7468 2070  aiwanese, with p
-000010d0: 726f 7065 7220 7361 6e64 6869 206f 6620  roper sandhi of 
-000010e0: 7072 6f6e 6f75 6e73 2c20 7375 6666 6978  pronouns, suffix
-000010f0: 6573 2c20 616e 6420 776f 7264 7320 7769  es, and words wi
-00001100: 7468 20e4 bb94 0d0a 2a20 6065 7863 5f6c  th .....* `exc_l
-00001110: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
-00001120: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
-00001130: 6c6c 6162 6c65 2065 7863 6570 7420 666f  llable except fo
-00001140: 7220 7468 6520 6c61 7374 206f 6e65 0d0a  r the last one..
-00001150: 2a20 6069 6e63 6c5f 6c61 7374 6020 2d20  * `incl_last` - 
-00001160: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
-00001170: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
-00001180: 696e 636c 7564 696e 6720 7468 6520 6c61  including the la
-00001190: 7374 206f 6e65 0d0a 0d0a 4465 6661 756c  st one....Defaul
-000011a0: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
-000011b0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
-000011c0: 7973 7465 6d60 3a0d 0a0d 0a2a 2060 6175  ystem`:....* `au
-000011d0: 746f 6020 2d20 666f 7220 6054 6f6e 6769  to` - for `Tongi
-000011e0: 6f6e 6760 0d0a 2a20 606e 6f6e 6560 202d  ong`..* `none` -
-000011f0: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
-00001200: 4f4a 602c 2060 5a68 7579 696e 602c 2060  OJ`, `Zhuyin`, `
-00001210: 544c 5041 602c 2060 5069 6e67 7969 6d60  TLPA`, `Pingyim`
-00001220: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
-00001230: 7420 2020 2020 2020 2020 7c20 6e6f 6e65  t         | none
-00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
-00001260: 2020 2020 2020 2020 7c20 6578 635f 6c61          | exc_la
-00001270: 7374 2020 2020 2020 2020 2020 2020 207c  st             |
-00001280: 2069 6e63 6c5f 6c61 7374 2020 2020 2020   incl_last      
-00001290: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
-000012a0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
-000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000012c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000012d0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-000012e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
-000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001300: 2d2d 2d20 7c0d 0a7c 20e9 8099 e698 afe5  --- |..| .......
-00001310: 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20 5473  ........... | Ts
-00001320: 6520 73c4 ab20 54c3 a269 2d75 c3a2 6e20  e s.. T..i-u..n 
-00001330: 67c3 ad6e 2dc3 a120 7c20 5473 6520 73c3  g..n-.. | Tse s.
-00001340: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
-00001350: c3a1 207c 2054 73c4 9320 73c3 ac20 54c4  .. | Ts.. s.. T.
-00001360: 8169 2d75 c481 6e20 6769 6e2d c3a1 207c  .i-u..n gin-.. |
-00001370: 2054 73c4 9320 73c3 ac20 54c4 8169 2d75   Ts.. s.. T..i-u
-00001380: c481 6e20 6769 6e2d 6120 7c0d 0a0d 0a53  ..n gin-a |....S
-00001390: 616e 6468 6920 7275 6c65 7320 616c 736f  andhi rules also
-000013a0: 2063 6861 6e67 6520 6465 7065 6e64 696e   change dependin
-000013b0: 6720 6f6e 2074 6865 2064 6961 6c65 6374  g on the dialect
-000013c0: 2063 686f 7365 6e2e 0d0a 0d0a 7c20 7465   chosen.....| te
-000013d0: 7874 207c 206e 6f20 7361 6e64 6869 207c  xt | no sandhi |
-000013e0: 2073 6f75 7468 2020 207c 206e 6f72 7468   south   | north
-000013f0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
-00001400: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
-00001410: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
-00001420: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
-00001430: 75c3 a26e 2020 207c 2054 c481 692d 75c3  u..n   | T..i-u.
-00001440: a26e 207c 2054 c3a0 692d 75c3 a26e 207c  .n | T..i-u..n |
-00001450: 0d0a 0d0a 2323 2323 2050 756e 6374 7561  ....#### Punctua
-00001460: 7469 6f6e 0d0a 0d0a 6070 756e 6374 7561  tion....`punctua
-00001470: 7469 6f6e 6020 5374 7269 6e67 0d0a 0d0a  tion` String....
-00001480: 2a20 6066 6f72 6d61 7460 2028 6465 6661  * `format` (defa
-00001490: 756c 7429 202d 2063 6f6e 7665 7274 7320  ult) - converts 
-000014a0: 4368 696e 6573 652d 7374 796c 6520 7075  Chinese-style pu
-000014b0: 6e63 7475 6174 696f 6e20 746f 204c 6174  nctuation to Lat
-000014c0: 696e 2d73 7479 6c65 2070 756e 6374 7561  in-style punctua
-000014d0: 7469 6f6e 2061 6e64 2063 6170 6974 616c  tion and capital
-000014e0: 6973 6573 2077 6f72 6473 2061 7420 7468  ises words at th
-000014f0: 6520 6265 6769 6e6e 696e 6720 6f66 2065  e beginning of e
-00001500: 6163 6820 7365 6e74 656e 6365 2e0d 0a2a  ach sentence...*
-00001510: 2060 6e6f 6e65 6020 2d20 7072 6573 6572   `none` - preser
-00001520: 7665 7320 4368 696e 6573 652d 7374 796c  ves Chinese-styl
-00001530: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
-00001540: 6420 646f 6573 6e27 7420 6361 7069 7461  d doesn't capita
-00001550: 6c69 7365 2077 6f72 6473 2061 7420 7468  lise words at th
-00001560: 6520 6265 6769 6e6e 696e 6720 6f66 206e  e beginning of n
-00001570: 6577 2073 656e 7465 6e63 6573 2e0d 0a0d  ew sentences....
-00001580: 0a7c 2074 6578 7420 2020 2020 2020 2020  .| text         
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 7c20 666f 726d 6174 2020 2020 2020    | format      
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 7c20 6e6f 6e65 2020 2020        | none    
-00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-000016a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
-000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016f0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001750: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
-00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000017b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c  ----------- |..|
-000017c0: 20e9 8099 e698 afe8 87ba e58d 97ef bc8c   ...............
-000017d0: e7b0 a1e7 a8b1 e380 8ce5 8d97 e380 8def  ................
-000017e0: bc88 e799 bde8 a9b1 e5ad 97ef bc9a 54c3  ..............T.
-000017f0: a269 2d6c c3a2 6def bc9b e6b3 a8e9 9fb3  .i-l..m.........
-00001800: e7ac a6e8 999f efbc 9ae3 848a e384 9ecb  ................
-00001810: 8a20 e384 8be3 84a2 cb8a efbc 8ce5 9c8b  . ..............
-00001820: e8aa 9eef bc9a 54c3 a169 6ec3 a16e efbc  ......T..in..n..
-00001830: 89e3 8082 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
-00001840: c3a2 692d 6cc3 a26d 2c20 6bc3 a16e 2d74  ..i-l..m, k..n-t
-00001850: 7368 696e 6720 226c c3a2 6d22 2028 5065  shing "l..m" (Pe
-00001860: cc8d 682d 75c4 932d 6ac4 ab3a 2054 c3a2  ..h-u..-j..: T..
-00001870: 692d 6cc3 a26d 3b20 7473 c3b9 2d69 6d20  i-l..m; ts..-im 
-00001880: 68c3 bb2d 68c5 8d3a 20e3 848a e384 9ecb  h..-h..: .......
-00001890: 8a20 e384 8be3 84a2 cb8a 2c20 6b6f 6b2d  . ........, kok-
-000018a0: 67c3 ad3a 2054 c3a1 696e c3a1 6e29 2e20  g..: T..in..n). 
-000018b0: 7c20 7473 6520 73c4 ab20 54c3 a269 2d6c  | tse s.. T..i-l
-000018c0: c3a2 6def bc8c 6bc3 a16e 2d74 7368 696e  ..m...k..n-tshin
-000018d0: 67e3 808c 6cc3 a26d e380 8def bc88 5065  g...l..m......Pe
-000018e0: cc8d 682d 75c4 932d 6ac4 abef bc9a 54c3  ..h-u..-j.....T.
-000018f0: a269 2d6c c3a2 6def bc9b 7473 c3b9 2d69  .i-l..m...ts..-i
-00001900: 6d20 68c3 bb2d 68c5 8def bc9a e384 8ae3  m h..-h.........
-00001910: 849e cb8a 20e3 848b e384 a2cb 8aef bc8c  .... ...........
-00001920: 6b6f 6b2d 67c3 adef bc9a 54c3 a169 6ec3  kok-g.....T..in.
-00001930: a16e efbc 89e3 8082 207c 0d0a 0d0a 2323  .n...... |....##
-00001940: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
-00001950: 4a4b 0d0a 0d0a 6063 6f6e 7665 7274 5f6e  JK....`convert_n
-00001960: 6f6e 5f63 6a6b 6020 426f 6f6c 6561 6e20  on_cjk` Boolean 
-00001970: 2d20 6465 6669 6e65 7320 7768 6574 6865  - defines whethe
-00001980: 7220 6f72 206e 6f74 2074 6f20 636f 6e76  r or not to conv
-00001990: 6572 7420 6e6f 6e2d 4368 696e 6573 6520  ert non-Chinese 
-000019a0: 776f 7264 732e 2043 616e 2062 6520 7573  words. Can be us
-000019b0: 6564 2074 6f20 636f 6e76 6572 7420 5461  ed to convert Ta
-000019c0: 696c 6f20 746f 2061 6e6f 7468 6572 2072  ilo to another r
-000019d0: 6f6d 616e 6973 6174 696f 6e20 7379 7374  omanisation syst
-000019e0: 656d 2e0d 0a0d 0a2a 2060 5472 7565 6020  em.....* `True` 
-000019f0: 2d20 636f 6e76 6572 7420 6e6f 6e2d 4368  - convert non-Ch
-00001a00: 696e 6573 6520 6368 6172 6163 7465 7220  inese character 
-00001a10: 776f 7264 730d 0a2a 2060 4661 6c73 6560  words..* `False`
-00001a20: 2028 6465 6661 756c 7429 202d 2063 6f6e   (default) - con
-00001a30: 7665 7274 206f 6e6c 7920 4368 696e 6573  vert only Chines
-00001a40: 6520 6368 6172 6163 7465 7220 776f 7264  e character word
-00001a50: 730d 0a0d 0a7c 2074 6578 7420 2020 2020  s....| text     
-00001a60: 207c 2046 616c 7365 2020 2020 2020 2020   | False        
-00001a70: 2020 2020 2020 2020 2020 207c 2054 7275             | Tru
-00001a80: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00001a90: 2020 2020 207c 0d0a 7c20 2d2d 2d2d 2d2d       |..| ------
-00001aa0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
-00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ad0: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6 8891  ------- |..| ...
-00001ae0: e9a3 9f70 68c3 a16e 6720 7c20 e386 a3e3  ...ph..ng | ....
-00001af0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
-00001b00: 9ae3 86b7 cb99 2070 68c3 a16e 6720 7c20  ...... ph..ng | 
-00001b10: e386 a3e3 84a8 e384 9acb 8b20 e384 90e3  ........... ....
-00001b20: 84a7 e384 9ae3 86b7 cb99 20e3 8486 e384  .......... .....
-00001b30: a4cb 8b20 7c0d 0a0d 0a23 2323 2054 6f6b  ... |....### Tok
-00001b40: 656e 6973 6572 0d0a 0d0a 6054 6f6b 656e  eniser....`Token
-00001b50: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
-00001b60: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
-00001b70: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
-00001b80: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
-00001b90: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
-00001ba0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
-00001bb0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
-00001bc0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
-00001bd0: 2063 6f6e 7374 7275 6374 6f72 0d0a 7420   constructor..t 
-00001be0: 3d20 546f 6b65 6e69 7365 7228 290d 0a0d  = Tokeniser()...
-00001bf0: 0a23 2074 6f6b 656e 6973 6520 5461 6977  .# tokenise Taiw
-00001c00: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
-00001c10: 6e74 656e 6365 0d0a 742e 746f 6b65 6e69  ntence..t.tokeni
-00001c20: 7365 2869 6e70 7574 290d 0a60 6060 0d0a  se(input)..```..
-00001c30: 0d0a 2323 2320 4f74 6865 7220 4675 6e63  ..### Other Func
-00001c40: 7469 6f6e 730d 0a0d 0a60 6060 7079 7468  tions....```pyth
-00001c50: 6f6e 0d0a 2320 436f 6e76 6572 7420 746f  on..# Convert to
-00001c60: 2054 7261 6469 7469 6f6e 616c 0d0a 746f   Traditional..to
-00001c70: 5f74 7261 6469 7469 6f6e 616c 2869 6e70  _traditional(inp
-00001c80: 7574 290d 0a0d 0a23 2043 6f6e 7665 7274  ut)....# Convert
-00001c90: 2074 6f20 5369 6d70 6c69 6669 6564 0d0a   to Simplified..
-00001ca0: 746f 5f73 696d 706c 6966 6965 6428 696e  to_simplified(in
-00001cb0: 7075 7429 0d0a 0d0a 2320 4368 6563 6b20  put)....# Check 
-00001cc0: 6966 2074 6865 2073 7472 696e 6720 6973  if the string is
-00001cd0: 2066 756c 6c79 2063 6f6d 706f 7365 6420   fully composed 
-00001ce0: 6f66 2043 6869 6e65 7365 2063 6861 7261  of Chinese chara
-00001cf0: 6374 6572 730d 0a69 735f 636a 6b28 696e  cters..is_cjk(in
-00001d00: 7075 7429 0d0a 6060 600d 0a0d 0a0d 0a0d  put)..```.......
-00001d10: 0a3c 212d 2d20 4558 414d 504c 4520 2d2d  .<!-- EXAMPLE --
-00001d20: 3e0d 0a23 2320 4578 616d 706c 650d 0a0d  >..## Example...
-00001d30: 0a60 6060 7079 7468 6f6e 0d0a 2320 436f  .```python..# Co
-00001d40: 6e76 6572 7465 720d 0a66 726f 6d20 7461  nverter..from ta
-00001d50: 6962 756e 2069 6d70 6f72 7420 436f 6e76  ibun import Conv
-00001d60: 6572 7465 720d 0a0d 0a23 2320 5379 7374  erter....## Syst
-00001d70: 656d 0d0a 6320 3d20 436f 6e76 6572 7465  em..c = Converte
-00001d80: 7228 2920 2320 5461 696c 6f20 7379 7374  r() # Tailo syst
-00001d90: 656d 2064 6566 6175 6c74 0d0a 632e 6765  em default..c.ge
-00001da0: 7428 27e5 8588 e794 9fe8 ac9b efbc 8ce5  t('.............
-00001db0: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
-00001dc0: 8227 290d 0a3e 3e20 5369 616e 2d73 696e  .')..>> Sian-sin
-00001dd0: 6e20 6bc3 b36e 672c 2068 61cc 8d6b 2d73  n k..ng, ha..k-s
-00001de0: 696e 6720 7469 c481 6d2d 7469 c481 6d20  ing ti..m-ti..m 
-00001df0: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
-00001e00: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
-00001e10: 275a 6875 7969 6e27 290d 0a63 2e67 6574  'Zhuyin')..c.get
-00001e20: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
-00001e30: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
-00001e40: 2729 0d0a 3e3e 20e3 8492 e384 a7e3 84a2  ')..>> .........
-00001e50: 20e3 8492 e386 aa20 e384 8de3 86b2 cb8b   ...... ........
-00001e60: 2c20 e384 8fe3 849a e386 b6cb 9920 e384  , ........... ..
-00001e70: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
-00001e80: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
-00001e90: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2323  ..............##
-00001ea0: 2044 6961 6c65 6374 0d0a 6320 3d20 436f   Dialect..c = Co
-00001eb0: 6e76 6572 7465 7228 2920 2320 736f 7574  nverter() # sout
-00001ec0: 6820 6469 616c 6563 7420 6465 6661 756c  h dialect defaul
-00001ed0: 740d 0a63 2e67 6574 2822 e688 91e6 acb2  t..c.get("......
-00001ee0: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
-00001ef0: 3e3e 2047 75c3 a120 6265 6820 c4ab 6e67  >> Gu.. beh ..ng
-00001f00: 2074 c4ab 2074 7369 61cc 8d68 2068 c3ae   t.. tsia..h h..
-00001f10: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001f20: 7228 6469 616c 6563 743d 276e 6f72 7468  r(dialect='north
-00001f30: 2729 0d0a 632e 6765 7428 22e6 8891 e6ac  ')..c.get(".....
-00001f40: b2e7 94a8 e7ae b8e9 a39f e9ad 9a22 290d  .............").
-00001f50: 0a3e 3e20 4775 c3a1 2062 7565 6820 c4ab  .>> Gu.. bueh ..
-00001f60: 6e67 2074 c5ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
-00001f70: c3bb 0d0a 0d0a 2323 2046 6f72 6d61 740d  ......## Format.
-00001f80: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
-00001f90: 2023 2066 6f72 2054 6169 6c6f 2c20 6d61   # for Tailo, ma
-00001fa0: 726b 2062 7920 6465 6661 756c 740d 0a63  rk by default..c
-00001fb0: 2e67 6574 2822 e794 9fe6 97a5 e5bf abe6  .get("..........
-00001fc0: a882 2229 0d0a 3e3e 2053 656e 6e2d 6a69  ..")..>> Senn-ji
-00001fd0: cc8d 7420 6b68 75c3 a069 2d6c 6fcc 8d6b  ..t khu..i-lo..k
-00001fe0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001ff0: 7228 666f 726d 6174 3d27 6e75 6d62 6572  r(format='number
-00002000: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
-00002010: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
-00002020: 6e6e 312d 6a69 7438 206b 6875 6169 332d  nn1-jit8 khuai3-
-00002030: 6c6f 6b38 0d0a 0d0a 6320 3d20 436f 6e76  lok8....c = Conv
-00002040: 6572 7465 7228 666f 726d 6174 3d27 7374  erter(format='st
-00002050: 7269 7027 290d 0a63 2e67 6574 2822 e794  rip')..c.get("..
-00002060: 9fe6 97a5 e5bf abe6 a882 2229 0d0a 3e3e  ..........")..>>
-00002070: 2053 656e 6e2d 6a69 7420 6b68 7561 692d   Senn-jit khuai-
-00002080: 6c6f 6b0d 0a0d 0a23 2320 4465 6c69 6d69  lok....## Delimi
-00002090: 7465 720d 0a63 203d 2043 6f6e 7665 7274  ter..c = Convert
-000020a0: 6572 2864 656c 696d 6974 6572 3d27 2729  er(delimiter='')
-000020b0: 0d0a 632e 6765 7428 22e5 8588 e794 9fe8  ..c.get(".......
-000020c0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
-000020d0: ace8 81bd e380 8222 290d 0a3e 3e20 5369  .......")..>> Si
-000020e0: 616e 7369 6e6e 206b c3b3 6e67 2c20 6861  ansinn k..ng, ha
-000020f0: cc8d 6b73 696e 6720 7469 c481 6d74 69c4  ..ksing ti..mti.
-00002100: 816d 2074 6869 616e 6e2e 0d0a 0d0a 6320  .m thiann.....c 
-00002110: 3d20 436f 6e76 6572 7465 7228 7379 7374  = Converter(syst
-00002120: 656d 3d27 5069 6e67 7969 6d27 2c20 6465  em='Pingyim', de
-00002130: 6c69 6d69 7465 723d 272d 2729 0d0a 632e  limiter='-')..c.
-00002140: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
-00002150: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
-00002160: e380 8222 290d 0a3e 3e20 5369 c481 6e2d  ...")..>> Si..n-
-00002170: 736e c4ab 2067 c792 6e67 2c20 68c3 a167  sn.. g..ng, h..g
-00002180: 2d73 c4ab 6e67 2064 69c3 a26d 2d64 69c3  -s..ng di..m-di.
-00002190: a26d 2074 696e c481 2e0d 0a0d 0a23 2320  .m tin.......## 
-000021a0: 5361 6e64 6869 0d0a 6320 3d20 436f 6e76  Sandhi..c = Conv
-000021b0: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
-000021c0: 696c 6f2c 2073 616e 6468 6920 6e6f 6e65  ilo, sandhi none
-000021d0: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
-000021e0: 6574 2822 e980 99e6 98af e58f b0e7 81a3  et("............
-000021f0: e59b a1e4 bb94 2229 0d0a 3e3e 2054 7365  ......")..>> Tse
-00002200: 2073 c4ab 2054 c3a2 692d 75c3 a26e 2067   s.. T..i-u..n g
-00002210: c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20 436f  ..n-......c = Co
-00002220: 6e76 6572 7465 7228 7361 6e64 6869 3d27  nverter(sandhi='
-00002230: 6175 746f 2729 0d0a 632e 6765 7428 22e9  auto')..c.get(".
-00002240: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
-00002250: 9422 290d 0a3e 3e20 5473 6520 73c3 ac20  .")..>> Tse s.. 
-00002260: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
-00002270: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00002280: 7228 7361 6e64 6869 3d27 6578 635f 6c61  r(sandhi='exc_la
-00002290: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
-000022a0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
-000022b0: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
-000022c0: c481 692d 75c4 816e 2067 696e 2dc3 a10d  ..i-u..n gin-...
-000022d0: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-000022e0: 2873 616e 6468 693d 2769 6e63 6c5f 6c61  (sandhi='incl_la
-000022f0: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
-00002300: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
-00002310: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
-00002320: c481 692d 75c4 816e 2067 696e 2d61 0d0a  ..i-u..n gin-a..
-00002330: 0d0a 2323 2050 756e 6374 7561 7469 6f6e  ..## Punctuation
-00002340: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00002350: 2920 2320 666f 726d 6174 2070 756e 6374  ) # format punct
-00002360: 7561 7469 6f6e 2064 6566 6175 6c74 0d0a  uation default..
-00002370: 632e 6765 7428 22e5 a4aa e7a9 bae6 9c8b  c.get(".........
-00002380: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
-00002390: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
-000023a0: 0d0a 3e3e 2054 68c3 a069 2d6b 686f 6e67  ..>> Th..i-khong
-000023b0: 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
-000023c0: 2d68 c3b3 2120 4cc3 ad6e 2074 7369 61cc  -h..! L..n tsia.
-000023d0: 8d68 2d70 c3a1 2062 75c4 933f 0d0a 0d0a  .h-p.. bu..?....
-000023e0: 6320 3d20 436f 6e76 6572 7465 7228 7075  c = Converter(pu
-000023f0: 6e63 7475 6174 696f 6e3d 276e 6f6e 6527  nctuation='none'
-00002400: 290d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  )..c.get("......
-00002410: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
-00002420: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
-00002430: 9f22 290d 0a3e 3e20 7468 c3a0 692d 6b68  .")..>> th..i-kh
-00002440: 6f6e 6720 70c3 ae6e 672d 69c3 baef bc8c  ong p..ng-i.....
-00002450: 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad 6e20  l..n-h.....l..n 
-00002460: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
-00002470: efbc 9f0d 0a0d 0a23 2320 436f 6e76 6572  .......## Conver
-00002480: 7420 6e6f 6e2d 434a 4b0d 0a63 203d 2043  t non-CJK..c = C
-00002490: 6f6e 7665 7274 2873 7973 7465 6d3d 275a  onvert(system='Z
-000024a0: 6875 7969 6e27 2920 2320 4661 6c73 6520  huyin') # False 
-000024b0: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b20  convert_non_cjk 
-000024c0: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
-000024d0: e688 91e9 a39f 7068 c3a1 6e67 2229 0d0a  ......ph..ng")..
-000024e0: 3e3e 20e3 86a3 e384 a8e3 849a cb8b 20e3  >> ........... .
-000024f0: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
-00002500: c3a1 6e67 0d0a 0d0a 6320 3d20 436f 6e76  ..ng....c = Conv
-00002510: 6572 7428 7379 7374 656d 3d27 5a68 7579  ert(system='Zhuy
-00002520: 696e 272c 2063 6f6e 7665 7274 5f6e 6f6e  in', convert_non
-00002530: 5f63 6a6b 3d54 7275 6529 0d0a 632e 6765  _cjk=True)..c.ge
-00002540: 7428 22e6 8891 e9a3 9f70 68c3 a16e 6722  t("......ph..ng"
-00002550: 290d 0a3e 3e20 e386 a3e3 84a8 e384 9acb  )..>> ..........
-00002560: 8b20 e384 90e3 84a7 e384 9ae3 86b7 cb99  . ..............
-00002570: 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23   ..............#
-00002580: 2054 6f6b 656e 6973 6572 0d0a 6672 6f6d   Tokeniser..from
-00002590: 2074 6169 6275 6e20 696d 706f 7274 2054   taibun import T
-000025a0: 6f6b 656e 6973 6572 0d0a 0d0a 7420 3d20  okeniser....t = 
-000025b0: 546f 6b65 6e69 7365 7228 290d 0a74 2e74  Tokeniser()..t.t
-000025c0: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
-000025d0: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
-000025e0: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
-000025f0: 2229 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27  ")..>> ['......'
-00002600: 2c20 27e6 9c8b e58f 8b27 2c20 27ef bc8c  , '......', '...
-00002610: 272c 2027 e681 81e5 a5bd 272c 2027 efbc  ', '......', '..
-00002620: 8127 2c20 27e6 8181 272c 2027 e9a3 9fe9  .', '...', '....
-00002630: a3bd 272c 2027 e69c aa27 2c20 27ef bc9f  ..', '...', '...
-00002640: 275d 0d0a 0d0a 0d0a 2320 4f74 6865 7220  ']......# Other 
-00002650: 4675 6e63 7469 6f6e 730d 0a66 726f 6d20  Functions..from 
-00002660: 7461 6962 756e 2069 6d70 6f72 7420 746f  taibun import to
-00002670: 5f74 7261 6469 7469 6f6e 616c 2c20 746f  _traditional, to
-00002680: 5f73 696d 706c 6966 6965 642c 2069 735f  _simplified, is_
-00002690: 636a 6b0d 0a0d 0a74 6f5f 7472 6164 6974  cjk....to_tradit
-000026a0: 696f 6e61 6c28 22e6 8891 e590 ace6 97a0  ional(".........
-000026b0: e58f b0e6 b9be e8af 9d22 290d 0a3e 3e20  .........")..>> 
-000026c0: e688 91e8 81bd e784 a1e5 8fb0 e781 a3e8  ................
-000026d0: a9b1 0d0a 0d0a 746f 5f73 696d 706c 6966  ......to_simplif
-000026e0: 6965 6428 22e6 8891 e881 bde7 84a1 e887  ied("...........
-000026f0: bae7 81a3 e8a9 b122 290d 0a3e 3e20 e688  .......")..>> ..
-00002700: 91e5 90ac e697 a0e5 8fb0 e6b9 bee8 af9d  ................
-00002710: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
-00002720: a39f e9ba ad27 290d 0a3e 3e20 5472 7565  .....')..>> True
-00002730: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
-00002740: a39f 7068 c3a1 6e67 2729 0d0a 3e3e 2046  ..ph..ng')..>> F
-00002750: 616c 7365 0d0a 6060 600d 0a0d 0a0d 0a0d  alse..```.......
-00002760: 0a3c 212d 2d20 4441 5441 202d 2d3e 0d0a  .<!-- DATA -->..
-00002770: 2323 2044 6174 610d 0a0d 0a2d 205b 5461  ## Data....- [Ta
-00002780: 6977 616e 6573 652d 4368 696e 6573 6520  iwanese-Chinese 
-00002790: 4f6e 6c69 6e65 2044 6963 7469 6f6e 6172  Online Dictionar
-000027a0: 795d 5b6f 6e6c 696e 652d 6469 6374 696f  y][online-dictio
-000027b0: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
-000027c0: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
-000027d0: 5d29 0d0a 2d20 5b69 5461 6967 6920 4368  ])..- [iTaigi Ch
-000027e0: 696e 6573 652d 5461 6977 616e 6573 6520  inese-Taiwanese 
-000027f0: 436f 6d70 6172 6973 6f6e 2044 6963 7469  Comparison Dicti
-00002800: 6f6e 6172 795d 5b69 7461 6967 692d 6469  onary][itaigi-di
-00002810: 6374 696f 6e61 7279 5d20 2876 6961 205b  ctionary] (via [
-00002820: 4368 686f 6554 6169 6769 5d5b 6461 7461  ChhoeTaigi][data
-00002830: 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21  -via])........<!
-00002840: 2d2d 2041 434b 4e4f 574c 4544 4745 4d45  -- ACKNOWLEDGEME
-00002850: 4e54 5320 2d2d 3e0d 0a23 2320 4163 6b6e  NTS -->..## Ackn
-00002860: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
-00002870: 2d20 5361 6d75 656c 204a 656e 2028 5b47  - Samuel Jen ([G
-00002880: 6974 6875 625d 5b73 616d 7565 6c2d 6769  ithub][samuel-gi
-00002890: 7468 7562 5d20 c2b7 205b 4c69 6e6b 6564  thub] .. [Linked
-000028a0: 496e 5d5b 7361 6d75 656c 2d6c 696e 6b65  In][samuel-linke
-000028b0: 6469 6e5d 2920 2d20 5461 6977 616e 6573  din]) - Taiwanes
-000028c0: 6520 616e 6420 4d61 6e64 6172 696e 2074  e and Mandarin t
-000028d0: 7261 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a  ranslation......
-000028e0: 0d0a 3c21 2d2d 204c 4943 454e 4345 202d  ..<!-- LICENCE -
-000028f0: 2d3e 0d0a 2323 204c 6963 656e 6365 0d0a  ->..## Licence..
-00002900: 0d0a 4265 6361 7573 6520 5461 6962 756e  ..Because Taibun
-00002910: 2069 7320 4d49 542d 6c69 6365 6e73 6564   is MIT-licensed
-00002920: 2c20 616e 7920 6465 7665 6c6f 7065 7220  , any developer 
-00002930: 6361 6e20 6573 7365 6e74 6961 6c6c 7920  can essentially 
-00002940: 646f 2077 6861 7465 7665 7220 7468 6579  do whatever they
-00002950: 2077 616e 7420 7769 7468 2069 7420 6173   want with it as
-00002960: 206c 6f6e 6720 6173 2074 6865 7920 696e   long as they in
-00002970: 636c 7564 6520 7468 6520 6f72 6967 696e  clude the origin
-00002980: 616c 2063 6f70 7972 6967 6874 2061 6e64  al copyright and
-00002990: 206c 6963 656e 6365 206e 6f74 6963 6520   licence notice 
-000029a0: 696e 2061 6e79 2063 6f70 6965 7320 6f66  in any copies of
-000029b0: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
-000029c0: 2e20 4e6f 7465 2c20 7468 6174 2074 6865  . Note, that the
-000029d0: 2064 6174 6120 7573 6564 2062 7920 7468   data used by th
-000029e0: 6520 7061 636b 6167 6520 6973 206c 6963  e package is lic
-000029f0: 656e 7365 6420 756e 6465 7220 6120 6469  ensed under a di
-00002a00: 6666 6572 656e 7420 636f 7079 7269 6768  fferent copyrigh
-00002a10: 742e 0d0a 0d0a 5468 6520 6461 7461 2069  t.....The data i
-00002a20: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-00002a30: 205b 4343 2042 592d 5341 2034 2e30 5d5b   [CC BY-SA 4.0][
-00002a40: 6461 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a  data-cc]........
-00002a50: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
-00002a60: 4e4b 5320 2d2d 3e0d 0a5b 7465 7374 735d  NKS -->..[tests]
-00002a70: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00002a80: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
-00002a90: 6169 6275 6e2f 6163 7469 6f6e 730d 0a5b  aibun/actions..[
-00002aa0: 7465 7374 732d 6261 6467 655d 3a20 6874  tests-badge]: ht
-00002ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00002ac0: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
-00002ad0: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
-00002ae0: 7475 732f 616e 6472 6569 6861 722f 7461  tus/andreihar/ta
-00002af0: 6962 756e 2f63 692e 7961 6d6c 3f73 7479  ibun/ci.yaml?sty
-00002b00: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
-00002b10: 266c 6f67 6f3d 6769 7468 7562 0d0a 5b63  &logo=github..[c
-00002b20: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
-00002b30: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
-00002b40: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00002b50: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
-00002b60: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
-00002b70: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00002b80: 6467 650d 0a5b 636f 6e74 7269 6275 746f  dge..[contributo
-00002b90: 7273 5d3a 2023 7573 6167 650d 0a5b 7265  rs]: #usage..[re
-00002ba0: 6c65 6173 652d 6261 6467 655d 3a20 6874  lease-badge]: ht
-00002bb0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00002bc0: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
-00002bd0: 6c65 6173 652f 616e 6472 6569 6861 722f  lease/andreihar/
-00002be0: 7461 6962 756e 3f63 6f6c 6f72 3d33 3836  taibun?color=386
-00002bf0: 3138 6326 7374 796c 653d 666f 722d 7468  18c&style=for-th
-00002c00: 652d 6261 6467 650d 0a5b 7265 6c65 6173  e-badge..[releas
-00002c10: 655d 3a20 6874 7470 733a 2f2f 6769 7468  e]: https://gith
-00002c20: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
-00002c30: 2f74 6169 6275 6e2f 7265 6c65 6173 6573  /taibun/releases
-00002c40: 0d0a 5b6c 6963 656e 6365 2d62 6164 6765  ..[licence-badge
-00002c50: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00002c60: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00002c70: 2f6c 6963 656e 7365 2f61 6e64 7265 6968  /license/andreih
-00002c80: 6172 2f74 6169 6275 6e3f 636f 6c6f 723d  ar/taibun?color=
-00002c90: 3030 3030 3030 2673 7479 6c65 3d66 6f72  000000&style=for
-00002ca0: 2d74 6865 2d62 6164 6765 0d0a 5b6c 6963  -the-badge..[lic
-00002cb0: 656e 6365 5d3a 204c 4943 454e 5345 0d0a  ence]: LICENSE..
-00002cc0: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
-00002cd0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00002ce0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00002cf0: 696e 6b65 6449 6e2d 3030 3737 4235 3f73  inkedIn-0077B5?s
-00002d00: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00002d10: 6765 266c 6f67 6f3d 6c69 6e6b 6564 696e  ge&logo=linkedin
-00002d20: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00002d30: 0d0a 5b6c 696e 6b65 6469 6e5d 3a20 6874  ..[linkedin]: ht
-00002d40: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00002d50: 696e 2e63 6f6d 2f69 6e2f 616e 6472 6569  in.com/in/andrei
-00002d60: 2d68 6172 6261 6368 6f76 2f0d 0a0d 0a5b  -harbachov/....[
-00002d70: 7079 7069 5d3a 2068 7474 7073 3a2f 2f70  pypi]: https://p
-00002d80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00002d90: 7461 6962 756e 0d0a 5b62 7567 5d3a 2068  taibun..[bug]: h
-00002da0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002db0: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
-00002dc0: 756e 2f69 7373 7565 730d 0a5b 6f6e 6c69  un/issues..[onli
-00002dd0: 6e65 2d64 6963 7469 6f6e 6172 795d 3a20  ne-dictionary]: 
-00002de0: 6874 7470 3a2f 2f69 7031 3934 3039 372e  http://ip194097.
-00002df0: 6e74 6375 2e65 6475 2e74 772f 756e 6769  ntcu.edu.tw/ungi
-00002e00: 616e 2f73 6f61 6e6e 7465 6e67 2f63 6869  an/soannteng/chi
-00002e10: 6c2f 5461 6968 6f61 2e61 7370 0d0a 5b69  l/Taihoa.asp..[i
-00002e20: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
-00002e30: 5d3a 2068 7474 7073 3a2f 2f69 7461 6967  ]: https://itaig
-00002e40: 692e 7477 2f0d 0a5b 6461 7461 2d76 6961  i.tw/..[data-via
-00002e50: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-00002e60: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
-00002e70: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
-00002e80: 6173 650d 0a5b 6461 7461 2d63 635d 3a20  ase..[data-cc]: 
-00002e90: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
-00002ea0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
-00002eb0: 6e73 6573 2f62 792d 7361 2f34 2e30 2f64  nses/by-sa/4.0/d
-00002ec0: 6565 642e 656e 0d0a 5b73 616d 7565 6c2d  eed.en..[samuel-
-00002ed0: 6769 7468 7562 5d3a 2068 7474 7073 3a2f  github]: https:/
-00002ee0: 2f67 6974 6875 622e 636f 6d2f 5353 5361  /github.com/SSSa
-00002ef0: 6d0d 0a5b 7361 6d75 656c 2d6c 696e 6b65  m..[samuel-linke
-00002f00: 6469 6e5d 3a20 6874 7470 733a 2f2f 7777  din]: https://ww
-00002f10: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
-00002f20: 6e2f 7361 6d75 656c 2d6a 656e 2f0d 0a0d  n/samuel-jen/...
-00002f30: 0a5b 7461 696c 6f2d 7769 6b69 5d3a 2068  .[tailo-wiki]: h
-00002f40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00002f50: 6469 612e 6f72 672f 7769 6b69 2f54 2543  dia.org/wiki/T%C
-00002f60: 3325 4132 692d 7525 4333 2541 326e 5f4c  3%A2i-u%C3%A2n_L
-00002f70: 2543 3325 4234 2d6d 2543 3325 4131 2d6a  %C3%B4-m%C3%A1-j
-00002f80: 2543 3425 4142 5f50 6869 6e67 2d69 6d5f  %C4%AB_Phing-im_
-00002f90: 486f 6e67 2d25 4333 2541 306e 0d0a 5b70  Hong-%C3%A0n..[p
-00002fa0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
-00002fb0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002fc0: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
-00002fd0: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
-00002fe0: 420d 0a5b 7a68 7579 696e 2d77 696b 695d  B..[zhuyin-wiki]
-00002ff0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00003000: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00003010: 5461 6977 616e 6573 655f 5068 6f6e 6574  Taiwanese_Phonet
-00003020: 6963 5f53 796d 626f 6c73 0d0a 5b74 6c70  ic_Symbols..[tlp
-00003030: 612d 7769 6b69 5d3a 2068 7474 7073 3a2f  a-wiki]: https:/
-00003040: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00003050: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
-00003060: 5f4c 616e 6775 6167 655f 5068 6f6e 6574  _Language_Phonet
-00003070: 6963 5f41 6c70 6861 6265 740d 0a5b 7069  ic_Alphabet..[pi
-00003080: 6e67 7969 6d2d 7769 6b69 5d3a 2068 7474  ngyim-wiki]: htt
-00003090: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000030a0: 612e 6f72 672f 7769 6b69 2f42 6225 4333  a.org/wiki/Bb%C3
-000030b0: 2541 316e 6c25 4333 2541 316d 5f70 2543  %A1nl%C3%A1m_p%C
-000030c0: 3325 4143 6e67 7925 4334 2541 426d 0d0a  3%ACngy%C4%ABm..
-000030d0: 5b74 6f6e 6769 6f6e 672d 7769 6b69 5d3a  [tongiong-wiki]:
-000030e0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-000030f0: 7065 6469 612e 6f72 672f 7769 6b69 2f44  pedia.org/wiki/D
-00003100: 6125 4334 2541 422d 6768 2543 3325 4145  a%C4%AB-gh%C3%AE
-00003110: 5f74 2543 3525 3844 6e67 2d69 2543 3525  _t%C5%8Dng-i%C5%
-00003120: 3844 6e67 5f70 2543 3425 4142 6e67 2d69  8Dng_p%C4%ABng-i
-00003130: 6d0d 0a5b 6970 612d 7769 6b69 5d3a 2068  m..[ipa-wiki]: h
-00003140: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00003150: 6469 612e 6f72 672f 7769 6b69 2f49 6e74  dia.org/wiki/Int
-00003160: 6572 6e61 7469 6f6e 616c 5f50 686f 6e65  ernational_Phone
-00003170: 7469 635f 416c 7068 6162 6574 0d0a 5b7a  tic_Alphabet..[z
-00003180: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
-00003190: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000031a0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
-000031b0: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
-000031c0: 0d0a 5b71 7561 6e7a 686f 752d 7769 6b69  ..[quanzhou-wiki
-000031d0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
-000031e0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-000031f0: 2f51 7561 6e7a 686f 755f 6469 616c 6563  /Quanzhou_dialec
-00003200: 7473 0d0a 5b6e 6c74 6b2d 746f 6b65 6e69  ts..[nltk-tokeni
-00003210: 7a65 5d3a 2068 7474 7073 3a2f 2f6e 6c74  ze]: https://nlt
-00003220: 6b2e 6f72 672f 6170 692f 6e6c 746b 2e74  k.org/api/nltk.t
-00003230: 6f6b 656e 697a 652e 6874 6d6c 0d0a 5b73  okenize.html..[s
-00003240: 616e 6468 692d 7769 6b69 5d3a 2068 7474  andhi-wiki]: htt
-00003250: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-00003260: 612e 6f72 672f 7769 6b69 2f54 6169 7761  a.org/wiki/Taiwa
-00003270: 6e65 7365 5f48 6f6b 6b69 656e 2354 6f6e  nese_Hokkien#Ton
-00003280: 6525 3230 7361 6e64 6869 3a7e 3a74 6578  e%20sandhi:~:tex
-00003290: 743d 7468 6e67 2545 3225 3946 2541 3925  t=thng%E2%9F%A9%
-000032a0: 3230 2825 3232 736f 7570 2532 3229 2e2d  20(%22soup%22).-
-000032b0: 2c54 6f6e 6525 3230 7361 6e64 6869 2c2d  ,Tone%20sandhi,-
-000032c0: 2535 4265 6469 7425 3544 0d0a            %5Bedit%5D..
+00000000: 3c21 2d2d 2050 524f 4a45 4354 204c 4f47  <!-- PROJECT LOG
+00000010: 4f20 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c  O -->..<br />..<
+00000020: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000030: 7222 3e0d 0a20 203c 6120 6872 6566 3d22  r">..  <a href="
+00000040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000050: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+00000060: 6275 6e22 3e0d 0a20 2020 203c 696d 6720  bun">..    <img 
+00000070: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000080: 6875 622e 636f 6d2f 616e 6472 6569 6861  hub.com/andreiha
+00000090: 722f 7461 6962 756e 2f72 6177 2f6d 6169  r/taibun/raw/mai
+000000a0: 6e2f 7265 6164 6d65 2f6c 6f67 6f2e 706e  n/readme/logo.pn
+000000b0: 6722 2061 6c74 3d22 4c6f 676f 2220 7769  g" alt="Logo" wi
+000000c0: 6474 683d 2239 3022 2068 6569 6768 743d  dth="90" height=
+000000d0: 2238 3022 3e0d 0a20 203c 2f61 3e0d 0a20  "80">..  </a>.. 
+000000e0: 200d 0a23 2054 6169 6275 6e0d 0a0d 0a0d   ..# Taibun.....
+000000f0: 0a0d 0a3c 212d 2d20 5052 4f4a 4543 5420  ...<!-- PROJECT 
+00000100: 5348 4945 4c44 5320 2d2d 3e0d 0a5b 215b  SHIELDS -->..[![
+00000110: 436f 6e74 7269 6275 7469 6f6e 735d 5b63  Contributions][c
+00000120: 6f6e 7472 6962 7574 696f 6e73 2d62 6164  ontributions-bad
+00000130: 6765 5d5d 5b63 6f6e 7472 6962 7574 696f  ge]][contributio
+00000140: 6e73 5d0d 0a5b 215b 5465 7374 735d 5b74  ns]..[![Tests][t
+00000150: 6573 7473 2d62 6164 6765 5d5d 5b74 6573  ests-badge]][tes
+00000160: 7473 5d0d 0a5b 215b 5265 6c65 6173 655d  ts]..[![Release]
+00000170: 5b72 656c 6561 7365 2d62 6164 6765 5d5d  [release-badge]]
+00000180: 5b72 656c 6561 7365 5d0d 0a5b 215b 4c69  [release]..[![Li
+00000190: 6365 6e63 655d 5b6c 6963 656e 6365 2d62  cence][licence-b
+000001a0: 6164 6765 5d5d 5b6c 6963 656e 6365 5d0d  adge]][licence].
+000001b0: 0a5b 215b 4c69 6e6b 6564 496e 5d5b 6c69  .[![LinkedIn][li
+000001c0: 6e6b 6564 696e 2d62 6164 6765 5d5d 5b6c  nkedin-badge]][l
+000001d0: 696e 6b65 6469 6e5d 0d0a 0d0a 2a2a 5461  inkedin]....**Ta
+000001e0: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+000001f0: 5472 616e 736c 6974 6572 6174 6f72 2061  Transliterator a
+00000200: 6e64 2054 6f6b 656e 6973 6572 2a2a 0d0a  nd Tokeniser**..
+00000210: 0d0a 4974 2068 6173 206d 6574 686f 6473  ..It has methods
+00000220: 2074 6861 7420 616c 6c6f 7720 746f 2063   that allow to c
+00000230: 7573 746f 6d69 7365 2074 7261 6e73 6c69  ustomise transli
+00000240: 7465 7261 7469 6f6e 2061 6e64 2072 6574  teration and ret
+00000250: 7269 6576 6520 616e 7920 6e65 6365 7373  rieve any necess
+00000260: 6172 7920 696e 666f 726d 6174 696f 6e20  ary information 
+00000270: 6162 6f75 7420 5461 6977 616e 6573 6520  about Taiwanese 
+00000280: 486f 6b6b 6965 6e20 7072 6f6e 756e 6369  Hokkien pronunci
+00000290: 6174 696f 6e2e 3c62 7220 2f3e 0d0a 496e  ation.<br />..In
+000002a0: 636c 7564 6573 2077 6f72 6420 746f 6b65  cludes word toke
+000002b0: 6e69 7365 7220 666f 7220 5461 6977 616e  niser for Taiwan
+000002c0: 6573 6520 486f 6b6b 6965 6e2e 0d0a 0d0a  ese Hokkien.....
+000002d0: 5b52 6570 6f72 7420 4275 675d 5b62 7567  [Report Bug][bug
+000002e0: 5d20 e280 a20d 0a5b 5079 5049 5d5b 7079  ] .....[PyPI][py
+000002f0: 7069 5d0d 0a0d 0a3c 2f64 6976 3e0d 0a0d  pi]....</div>...
+00000300: 0a0d 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a 0d0a  .....---........
+00000310: 3c21 2d2d 2054 4142 4c45 204f 4620 434f  <!-- TABLE OF CO
+00000320: 4e54 454e 5453 202d 2d3e 0d0a 3c64 6574  NTENTS -->..<det
+00000330: 6169 6c73 206f 7065 6e3e 0d0a 2020 3c73  ails open>..  <s
+00000340: 756d 6d61 7279 3e54 6162 6c65 206f 6620  ummary>Table of 
+00000350: 436f 6e74 656e 7473 3c2f 7375 6d6d 6172  Contents</summar
+00000360: 793e 0d0a 2020 3c6f 6c3e 0d0a 2020 2020  y>..  <ol>..    
+00000370: 3c6c 693e 3c61 2068 7265 663d 2223 7665  <li><a href="#ve
+00000380: 7273 696f 6e73 223e 5665 7273 696f 6e73  rsions">Versions
+00000390: 3c2f 613e 3c2f 6c69 3e0d 0a20 2020 203c  </a></li>..    <
+000003a0: 6c69 3e3c 6120 6872 6566 3d22 2369 6e73  li><a href="#ins
+000003b0: 7461 6c6c 223e 496e 7374 616c 6c3c 2f61  tall">Install</a
+000003c0: 3e3c 2f6c 693e 0d0a 2020 2020 3c6c 693e  ></li>..    <li>
+000003d0: 0d0a 2020 2020 2020 3c61 2068 7265 663d  ..      <a href=
+000003e0: 2223 7573 6167 6522 3e55 7361 6765 3c2f  "#usage">Usage</
+000003f0: 613e 0d0a 2020 2020 2020 3c75 6c3e 0d0a  a>..      <ul>..
+00000400: 2020 2020 2020 2020 3c6c 693e 0d0a 2020          <li>..  
+00000410: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
+00000420: 2223 636f 6e76 6572 7465 7222 3e43 6f6e  "#converter">Con
+00000430: 7665 7274 6572 3c2f 613e 0d0a 2020 2020  verter</a>..    
+00000440: 2020 2020 2020 3c75 6c3e 0d0a 2020 2020        <ul>..    
+00000450: 2020 2020 2020 2020 3c6c 693e 3c61 2068          <li><a h
+00000460: 7265 663d 2223 7379 7374 656d 223e 5379  ref="#system">Sy
+00000470: 7374 656d 3c2f 613e 3c2f 6c69 3e0d 0a20  stem</a></li>.. 
+00000480: 2020 2020 2020 2020 2020 203c 6c69 3e3c             <li><
+00000490: 6120 6872 6566 3d22 2364 6961 6c65 6374  a href="#dialect
+000004a0: 223e 4469 616c 6563 743c 2f61 3e3c 2f6c  ">Dialect</a></l
+000004b0: 693e 0d0a 2020 2020 2020 2020 2020 2020  i>..            
+000004c0: 3c6c 693e 3c61 2068 7265 663d 2223 666f  <li><a href="#fo
+000004d0: 726d 6174 223e 466f 726d 6174 3c2f 613e  rmat">Format</a>
+000004e0: 3c2f 6c69 3e0d 0a20 2020 2020 2020 2020  </li>..         
+000004f0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
+00000500: 2364 656c 696d 6974 6572 223e 4465 6c69  #delimiter">Deli
+00000510: 6d69 7465 723c 2f61 3e3c 2f6c 693e 0d0a  miter</a></li>..
+00000520: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+00000530: 3c61 2068 7265 663d 2223 7361 6e64 6869  <a href="#sandhi
+00000540: 223e 5361 6e64 6869 3c2f 613e 3c2f 6c69  ">Sandhi</a></li
+00000550: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000560: 6c69 3e3c 6120 6872 6566 3d22 2370 756e  li><a href="#pun
+00000570: 6374 7561 7469 6f6e 223e 5075 6e63 7475  ctuation">Punctu
+00000580: 6174 696f 6e3c 2f61 3e3c 2f6c 693e 0d0a  ation</a></li>..
+00000590: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+000005a0: 3c61 2068 7265 663d 2223 636f 6e76 6572  <a href="#conver
+000005b0: 742d 6e6f 6e2d 636a 6b22 3e43 6f6e 7665  t-non-cjk">Conve
+000005c0: 7274 206e 6f6e 2d43 4a4b 3c2f 613e 3c2f  rt non-CJK</a></
+000005d0: 6c69 3e0d 0a20 2020 2020 2020 2020 203c  li>..          <
+000005e0: 2f75 6c3e 0d0a 2020 2020 2020 2020 3c2f  /ul>..        </
+000005f0: 6c69 3e0d 0a20 2020 2020 2020 203c 6c69  li>..        <li
+00000600: 3e3c 6120 6872 6566 3d22 2374 6f6b 656e  ><a href="#token
+00000610: 6973 6572 223e 546f 6b65 6e69 7365 723c  iser">Tokeniser<
+00000620: 2f61 3e3c 2f6c 693e 0d0a 2020 2020 2020  /a></li>..      
+00000630: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
+00000640: 6f74 6865 722d 6675 6e63 7469 6f6e 7322  other-functions"
+00000650: 3e4f 7468 6572 2046 756e 6374 696f 6e73  >Other Functions
+00000660: 3c2f 613e 3c2f 6c69 3e0d 0a20 2020 2020  </a></li>..     
+00000670: 203c 2f75 6c3e 0d0a 2020 2020 3c2f 6c69   </ul>..    </li
+00000680: 3e0d 0a20 2020 203c 6c69 3e3c 6120 6872  >..    <li><a hr
+00000690: 6566 3d22 2365 7861 6d70 6c65 223e 4578  ef="#example">Ex
+000006a0: 616d 706c 653c 2f61 3e3c 2f6c 693e 0d0a  ample</a></li>..
+000006b0: 2020 2020 3c6c 693e 3c61 2068 7265 663d      <li><a href=
+000006c0: 2223 6461 7461 223e 4461 7461 3c2f 613e  "#data">Data</a>
+000006d0: 3c2f 6c69 3e0d 0a20 2020 203c 6c69 3e3c  </li>..    <li><
+000006e0: 6120 6872 6566 3d22 2361 636b 6e6f 776c  a href="#acknowl
+000006f0: 6564 6765 6d65 6e74 7322 3e41 636b 6e6f  edgements">Ackno
+00000700: 776c 6564 6765 6d65 6e74 733c 2f61 3e3c  wledgements</a><
+00000710: 2f6c 693e 0d0a 2020 2020 3c6c 693e 3c61  /li>..    <li><a
+00000720: 2068 7265 663d 2223 6c69 6365 6e63 6522   href="#licence"
+00000730: 3e4c 6963 656e 6365 3c2f 613e 3c2f 6c69  >Licence</a></li
+00000740: 3e0d 0a20 203c 2f6f 6c3e 0d0a 3c2f 6465  >..  </ol>..</de
+00000750: 7461 696c 733e 0d0a 0d0a 0d0a 0d0a 3c21  tails>........<!
+00000760: 2d2d 204f 5448 4552 2056 4552 5349 4f4e  -- OTHER VERSION
+00000770: 5320 2d2d 3e0d 0a23 2320 5665 7273 696f  S -->..## Versio
+00000780: 6e73 0d0a 0d0a 5b21 5b4a 6176 6153 6372  ns....[![JavaScr
+00000790: 6970 7420 5665 7273 696f 6e5d 5b6a 732d  ipt Version][js-
+000007a0: 6261 6467 655d 5d5b 6a73 2d6c 696e 6b5d  badge]][js-link]
+000007b0: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2049 4e53  ........<!-- INS
+000007c0: 5441 4c4c 202d 2d3e 0d0a 2323 2049 6e73  TALL -->..## Ins
+000007d0: 7461 6c6c 0d0a 0d0a 5461 6962 756e 2063  tall....Taibun c
+000007e0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+000007f0: 6672 6f6d 205b 7079 7069 5d5b 7079 7069  from [pypi][pypi
+00000800: 5d0d 0a0d 0a60 6060 6261 7368 0d0a 2420  ]....```bash..$ 
+00000810: 7069 7020 696e 7374 616c 6c20 7461 6962  pip install taib
+00000820: 756e 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c  un..```........<
+00000830: 212d 2d20 5553 4147 4520 2d2d 3e0d 0a23  !-- USAGE -->..#
+00000840: 2320 5573 6167 650d 0a0d 0a23 2323 2043  # Usage....### C
+00000850: 6f6e 7665 7274 6572 0d0a 0d0a 6043 6f6e  onverter....`Con
+00000860: 7665 7274 6572 6020 636c 6173 7320 7472  verter` class tr
+00000870: 616e 736c 6974 6572 6174 6573 2074 6865  ansliterates the
+00000880: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+00000890: 6572 7320 746f 2074 6865 2063 686f 7365  ers to the chose
+000008a0: 6e20 7472 616e 736c 6974 6572 6174 696f  n transliteratio
+000008b0: 6e20 7379 7374 656d 2077 6974 6820 7061  n system with pa
+000008c0: 7261 6d65 7465 7273 2073 7065 6369 6669  rameters specifi
+000008d0: 6564 2062 7920 7468 6520 6465 7665 6c6f  ed by the develo
+000008e0: 7065 722e 2057 6f72 6b73 2066 6f72 2062  per. Works for b
+000008f0: 6f74 6820 5472 6164 6974 696f 6e61 6c20  oth Traditional 
+00000900: 616e 6420 5369 6d70 6c69 6669 6564 2063  and Simplified c
+00000910: 6861 7261 6374 6572 732e 0d0a 0d0a 6060  haracters.....``
+00000920: 6070 7974 686f 6e0d 0a23 2043 6f6e 7374  `python..# Const
+00000930: 7275 6374 6f72 0d0a 6320 3d20 436f 6e76  ructor..c = Conv
+00000940: 6572 7465 7228 7379 7374 656d 2c20 6469  erter(system, di
+00000950: 616c 6563 742c 2066 6f72 6d61 742c 2064  alect, format, d
+00000960: 656c 696d 6974 6572 2c20 7361 6e64 6869  elimiter, sandhi
+00000970: 2c20 7075 6e63 7475 6174 696f 6e2c 2063  , punctuation, c
+00000980: 6f6e 7665 7274 5f6e 6f6e 5f63 6a6b 290d  onvert_non_cjk).
+00000990: 0a0d 0a23 2054 7261 6e73 6c69 7465 7261  ...# Translitera
+000009a0: 7465 2043 6869 6e65 7365 2063 6861 7261  te Chinese chara
+000009b0: 6374 6572 730d 0a63 2e67 6574 2869 6e70  cters..c.get(inp
+000009c0: 7574 290d 0a60 6060 0d0a 0d0a 2323 2323  ut)..```....####
+000009d0: 2053 7973 7465 6d0d 0a0d 0a60 7379 7374   System....`syst
+000009e0: 656d 6020 5374 7269 6e67 202d 2073 7973  em` String - sys
+000009f0: 7465 6d20 6f66 2074 7261 6e73 6c69 7465  tem of translite
+00000a00: 7261 7469 6f6e 2e0d 0a0d 0a2a 2060 5461  ration.....* `Ta
+00000a10: 696c 6f60 2028 6465 6661 756c 7429 202d  ilo` (default) -
+00000a20: 205b 54c3 a269 2d75 c3a2 6e20 4cc3 b42d   [T..i-u..n L..-
+00000a30: 6dc3 a12d 6ac4 ab20 5068 696e 672d 696d  m..-j.. Phing-im
+00000a40: 2048 6f6e 672d c3a0 6e5d 5b74 6169 6c6f   Hong-..n][tailo
+00000a50: 2d77 696b 695d 0d0a 2a20 6050 4f4a 6020  -wiki]..* `POJ` 
+00000a60: 2d20 5b50 65cc 8d68 2dc5 8d65 2d6a c4ab  - [Pe..h-..e-j..
+00000a70: 5d5b 706f 6a2d 7769 6b69 5d0d 0a2a 2060  ][poj-wiki]..* `
+00000a80: 5a68 7579 696e 6020 2d20 5b54 6169 7761  Zhuyin` - [Taiwa
+00000a90: 6e65 7365 2050 686f 6e65 7469 6320 5379  nese Phonetic Sy
+00000aa0: 6d62 6f6c 735d 5b7a 6875 7969 6e2d 7769  mbols][zhuyin-wi
+00000ab0: 6b69 5d0d 0a2a 2060 544c 5041 6020 2d20  ki]..* `TLPA` - 
+00000ac0: 5b54 6169 7761 6e65 7365 204c 616e 6775  [Taiwanese Langu
+00000ad0: 6167 6520 5068 6f6e 6574 6963 2041 6c70  age Phonetic Alp
+00000ae0: 6861 6265 745d 5b74 6c70 612d 7769 6b69  habet][tlpa-wiki
+00000af0: 5d0d 0a2a 2060 5069 6e67 7969 6d60 202d  ]..* `Pingyim` -
+00000b00: 205b 4262 c3a1 6e6c c3a1 6d20 55c4 9320   [Bb..nl..m U.. 
+00000b10: 50c3 ac6e 6779 c4ab 6d20 48c5 8d6e 6727  P..ngy..m H..ng'
+00000b20: c3a0 6e5d 5b70 696e 6779 696d 2d77 696b  ..n][pingyim-wik
+00000b30: 695d 0d0a 2a20 6054 6f6e 6769 6f6e 6760  i]..* `Tongiong`
+00000b40: 202d 205b 4461 c4ab 2d67 68c3 ae20 54c5   - [Da..-gh.. T.
+00000b50: 8d6e 672d 69c5 8d6e 6720 50c4 ab6e 672d  .ng-i..ng P..ng-
+00000b60: 696d 5d5b 746f 6e67 696f 6e67 2d77 696b  im][tongiong-wik
+00000b70: 695d 0d0a 2a20 6049 5041 6020 2d20 5b49  i]..* `IPA` - [I
+00000b80: 6e74 6572 6e61 7469 6f6e 616c 2050 686f  nternational Pho
+00000b90: 6e65 7469 6320 416c 7068 6162 6574 5d5b  netic Alphabet][
+00000ba0: 6970 612d 7769 6b69 5d0d 0a0d 0a7c 2074  ipa-wiki]....| t
+00000bb0: 6578 7420 7c20 5461 696c 6f20 2020 7c20  ext | Tailo   | 
+00000bc0: 504f 4a20 2020 2020 7c20 5a68 7579 696e  POJ     | Zhuyin
+00000bd0: 2020 2020 2020 7c20 544c 5041 2020 2020        | TLPA    
+00000be0: 2020 7c20 5069 6e67 7969 6d20 7c20 546f    | Pingyim | To
+00000bf0: 6e67 696f 6e67 207c 2049 5041 2020 2020  ngiong | IPA    
+00000c00: 2020 2020 207c 0d0a 7c20 2d2d 2d2d 207c       |..| ---- |
+00000c10: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
+00000c20: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
+00000c30: 207c 202d 2d2d 2d2d 2d2d 2d2d 207c 202d   | --------- | -
+00000c40: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00000c50: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  - | ----------- 
+00000c60: 7c0d 0a7c 20e5 8fb0 e781 a320 7c20 54c3  |..| ...... | T.
+00000c70: a269 2d75 c3a2 6e20 7c20 54c3 a269 2d6f  .i-u..n | T..i-o
+00000c80: c3a2 6e20 7c20 e384 89e3 849e cb8a 20e3  ..n | ........ .
+00000c90: 84a8 e384 a2cb 8a20 7c20 5461 6935 2075  ....... | Tai5 u
+00000ca0: 616e 3520 7c20 44c3 a169 77c3 a16e 2020  an5 | D..iw..n  
+00000cb0: 7c20 54c4 8169 2d75 c78e 6e20 207c 2054  | T..i-u..n  | T
+00000cc0: 6169 c2b2 e281 b520 7561 6ec2 b2e2 81b5  ai..... uan.....
+00000cd0: 207c 0d0a 0d0a 2323 2323 2044 6961 6c65   |....#### Diale
+00000ce0: 6374 0d0a 0d0a 6064 6961 6c65 6374 6020  ct....`dialect` 
+00000cf0: 5374 7269 6e67 202d 2070 7265 6665 7272  String - preferr
+00000d00: 6564 2070 726f 6e75 6e63 6961 7469 6f6e  ed pronunciation
+00000d10: 2e0d 0a0d 0a2a 2060 736f 7574 6860 2028  .....* `south` (
+00000d20: 6465 6661 756c 7429 202d 205b 5a68 616e  default) - [Zhan
+00000d30: 677a 686f 755d 5b7a 6861 6e67 7a68 6f75  gzhou][zhangzhou
+00000d40: 2d77 696b 695d 2d6c 6561 6e69 6e67 2070  -wiki]-leaning p
+00000d50: 726f 6e75 6e63 6961 7469 6f6e 0d0a 2a20  ronunciation..* 
+00000d60: 606e 6f72 7468 6020 2d20 5b51 7561 6e7a  `north` - [Quanz
+00000d70: 686f 755d 5b71 7561 6e7a 686f 752d 7769  hou][quanzhou-wi
+00000d80: 6b69 5d2d 6c65 616e 696e 6720 7072 6f6e  ki]-leaning pron
+00000d90: 756e 6369 6174 696f 6e0d 0a0d 0a7c 2074  unciation....| t
+00000da0: 6578 7420 2020 7c20 736f 7574 6820 2020  ext   | south   
+00000db0: 2020 2020 2020 7c20 6e6f 7274 6820 2020        | north   
+00000dc0: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+00000dd0: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
+00000de0: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
+00000df0: 2d20 7c0d 0a7c 20e4 ba94 e69c 88e7 af80  - |..| .........
+00000e00: 207c 2047 c58d 6f2d 6775 65cc 8d68 2d74   | G..o-gue..h-t
+00000e10: 7365 6820 7c20 47c5 8d6f 2d67 65cc 8d68  seh | G..o-ge..h
+00000e20: 2d74 7375 6568 207c 0d0a 0d0a 2323 2323  -tsueh |....####
+00000e30: 2046 6f72 6d61 740d 0a0d 0a60 666f 726d   Format....`form
+00000e40: 6174 6020 5374 7269 6e67 202d 2066 6f72  at` String - for
+00000e50: 6d61 7420 696e 2077 6869 6368 2074 6f6e  mat in which ton
+00000e60: 6573 2077 696c 6c20 6265 2072 6570 7265  es will be repre
+00000e70: 7365 6e74 6564 2069 6e20 7468 6520 636f  sented in the co
+00000e80: 6e76 6572 7465 6420 7365 6e74 656e 6365  nverted sentence
+00000e90: 2e0d 0a0d 0a2a 2060 6d61 726b 6020 2864  .....* `mark` (d
+00000ea0: 6566 6175 6c74 2920 2d20 7573 6573 2064  efault) - uses d
+00000eb0: 6961 6372 6974 6963 7320 666f 7220 6561  iacritics for ea
+00000ec0: 6368 2073 796c 6c61 626c 652e 204e 6f74  ch syllable. Not
+00000ed0: 2061 7661 696c 6162 6c65 2066 6f72 2054   available for T
+00000ee0: 4c50 412e 0d0a 2a20 606e 756d 6265 7260  LPA...* `number`
+00000ef0: 202d 2061 6464 2061 206e 756d 6265 7220   - add a number 
+00000f00: 7768 6963 6820 7265 7072 6573 656e 7473  which represents
+00000f10: 2074 6865 2074 6f6e 6520 6174 2074 6865   the tone at the
+00000f20: 2065 6e64 206f 6620 7468 6520 7379 6c6c   end of the syll
+00000f30: 6162 6c65 0d0a 2a20 6073 7472 6970 6020  able..* `strip` 
+00000f40: 2d20 7265 6d6f 7665 7320 616e 7920 746f  - removes any to
+00000f50: 6e65 206d 6172 6b69 6e67 0d0a 0d0a 7c20  ne marking....| 
+00000f60: 7465 7874 207c 206d 6172 6b20 2020 207c  text | mark    |
+00000f70: 206e 756d 6265 7220 2020 207c 2073 7472   number    | str
+00000f80: 6970 2020 207c 0d0a 7c20 2d2d 2d2d 207c  ip   |..| ---- |
+00000f90: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
+00000fa0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
+00000fb0: 0d0a 7c20 e58f b0e7 81a3 207c 2054 c3a2  ..| ...... | T..
+00000fc0: 692d 75c3 a26e 207c 2054 6169 352d 7561  i-u..n | Tai5-ua
+00000fd0: 6e35 207c 2054 6169 2d75 616e 207c 0d0a  n5 | Tai-uan |..
+00000fe0: 0d0a 2323 2323 2044 656c 696d 6974 6572  ..#### Delimiter
+00000ff0: 0d0a 0d0a 6064 656c 696d 6974 6572 6020  ....`delimiter` 
+00001000: 5374 7269 6e67 202d 2073 6574 7320 7468  String - sets th
+00001010: 6520 6465 6c69 6d69 7465 7220 6368 6172  e delimiter char
+00001020: 6163 7465 7220 7468 6174 2077 696c 6c20  acter that will 
+00001030: 6265 2070 6c61 6365 6420 696e 2062 6574  be placed in bet
+00001040: 7765 656e 2073 796c 6c61 626c 6573 206f  ween syllables o
+00001050: 6620 6120 776f 7264 2e0d 0a0d 0a44 6566  f a word.....Def
+00001060: 6175 6c74 2076 616c 7565 2064 6570 656e  ault value depen
+00001070: 6473 206f 6e20 7468 6520 6368 6f73 656e  ds on the chosen
+00001080: 2060 7379 7374 656d 603a 0d0a 0d0a 2a20   `system`:....* 
+00001090: 6027 2d27 6020 2d20 666f 7220 6054 6169  `'-'` - for `Tai
+000010a0: 6c6f 602c 2060 504f 4a60 2c20 6054 6f6e  lo`, `POJ`, `Ton
+000010b0: 6769 6f6e 6760 0d0a 2a20 6027 2760 202d  giong`..* `''` -
+000010c0: 2066 6f72 2060 5069 6e67 7969 6d60 0d0a   for `Pingyim`..
+000010d0: 2a20 6027 2027 6020 2d20 666f 7220 605a  * `' '` - for `Z
+000010e0: 6875 7969 6e60 2c20 6054 4c50 4160 2c20  huyin`, `TLPA`, 
+000010f0: 6049 5041 600d 0a0d 0a7c 2074 6578 7420  `IPA`....| text 
+00001100: 7c20 272d 2720 2020 2020 7c20 2727 2020  | '-'     | ''  
+00001110: 2020 207c 2027 2027 2020 2020 207c 0d0a     | ' '     |..
+00001120: 7c20 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  | ---- | -------
+00001130: 207c 202d 2d2d 2d2d 2d20 7c20 2d2d 2d2d   | ------ | ----
+00001140: 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781 a320  --- |..| ...... 
+00001150: 7c20 54c3 a269 2d75 c3a2 6e20 7c20 54c3  | T..i-u..n | T.
+00001160: a269 75c3 a26e 207c 2054 c3a2 6920 75c3  .iu..n | T..i u.
+00001170: a26e 207c 0d0a 0d0a 2323 2323 2053 616e  .n |....#### San
+00001180: 6468 690d 0a0d 0a60 7361 6e64 6869 6020  dhi....`sandhi` 
+00001190: 5374 7269 6e67 202d 2061 7070 6c69 6573  String - applies
+000011a0: 2074 6865 205b 7361 6e64 6869 2072 756c   the [sandhi rul
+000011b0: 6573 206f 6620 5461 6977 616e 6573 6520  es of Taiwanese 
+000011c0: 486f 6b6b 6965 6e5d 5b73 616e 6468 692d  Hokkien][sandhi-
+000011d0: 7769 6b69 5d2e 0d0a 0d0a 5369 6e63 6520  wiki].....Since 
+000011e0: 6974 2773 2064 6966 6669 6375 6c74 2074  it's difficult t
+000011f0: 6f20 656e 636f 6465 2061 6c6c 2073 616e  o encode all san
+00001200: 6468 6920 7275 6c65 732c 2054 6169 6275  dhi rules, Taibu
+00001210: 6e20 7072 6f76 6964 6573 206d 756c 7469  n provides multi
+00001220: 706c 6520 6d6f 6465 7320 666f 7220 7361  ple modes for sa
+00001230: 6e64 6869 2063 6f6e 7665 7273 696f 6e20  ndhi conversion 
+00001240: 746f 2061 6c6c 6f77 2066 6f72 2063 7573  to allow for cus
+00001250: 746f 6d69 7365 6420 7361 6e64 6869 2068  tomised sandhi h
+00001260: 616e 646c 696e 672e 0d0a 0d0a 2a20 606e  andling.....* `n
+00001270: 6f6e 6560 202d 2064 6f65 736e 2774 2070  one` - doesn't p
+00001280: 6572 666f 726d 2061 6e79 2074 6f6e 6520  erform any tone 
+00001290: 7361 6e64 6869 0d0a 2a20 6061 7574 6f60  sandhi..* `auto`
+000012a0: 202d 2063 6c6f 7365 7374 2061 7070 726f   - closest appro
+000012b0: 7869 6d61 7469 6f6e 2074 6f20 6675 6c6c  ximation to full
+000012c0: 2063 6f72 7265 6374 2074 6f6e 6520 7361   correct tone sa
+000012d0: 6e64 6869 206f 6620 5461 6977 616e 6573  ndhi of Taiwanes
+000012e0: 652c 2077 6974 6820 7072 6f70 6572 2073  e, with proper s
+000012f0: 616e 6468 6920 6f66 2070 726f 6e6f 756e  andhi of pronoun
+00001300: 732c 2073 7566 6669 7865 732c 2061 6e64  s, suffixes, and
+00001310: 2077 6f72 6473 2077 6974 6820 e4bb 940d   words with ....
+00001320: 0a2a 2060 6578 635f 6c61 7374 6020 2d20  .* `exc_last` - 
+00001330: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
+00001340: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
+00001350: 6578 6365 7074 2066 6f72 2074 6865 206c  except for the l
+00001360: 6173 7420 6f6e 650d 0a2a 2060 696e 636c  ast one..* `incl
+00001370: 5f6c 6173 7460 202d 2063 6861 6e67 6573  _last` - changes
+00001380: 2074 6f6e 6520 666f 7220 6576 6572 7920   tone for every 
+00001390: 7379 6c6c 6162 6c65 2069 6e63 6c75 6469  syllable includi
+000013a0: 6e67 2074 6865 206c 6173 7420 6f6e 650d  ng the last one.
+000013b0: 0a0d 0a44 6566 6175 6c74 2076 616c 7565  ...Default value
+000013c0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
+000013d0: 6368 6f73 656e 2060 7379 7374 656d 603a  chosen `system`:
+000013e0: 0d0a 0d0a 2a20 6061 7574 6f60 202d 2066  ....* `auto` - f
+000013f0: 6f72 2060 546f 6e67 696f 6e67 600d 0a2a  or `Tongiong`..*
+00001400: 2060 6e6f 6e65 6020 2d20 666f 7220 6054   `none` - for `T
+00001410: 6169 6c6f 602c 2060 504f 4a60 2c20 605a  ailo`, `POJ`, `Z
+00001420: 6875 7969 6e60 2c20 6054 4c50 4160 2c20  huyin`, `TLPA`, 
+00001430: 6050 696e 6779 696d 602c 2060 4950 4160  `Pingyim`, `IPA`
+00001440: 0d0a 0d0a 7c20 7465 7874 2020 2020 2020  ....| text      
+00001450: 2020 2020 2020 207c 206e 6f6e 6520 2020         | none   
+00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001470: 2020 207c 2061 7574 6f20 2020 2020 2020     | auto       
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 7c20 6578 635f 6c61 7374 2020 2020 2020  | exc_last      
+000014a0: 2020 2020 2020 2020 2020 2020 7c20 696e              | in
+000014b0: 636c 5f6c 6173 7420 2020 2020 2020 2020  cl_last         
+000014c0: 2020 2020 2020 2020 7c0d 0a7c 202d 2d2d          |..| ---
+000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+000014e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014f0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001510: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001530: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
+00001540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00001550: 0d0a 7c20 e980 99e6 98af e4bd a0e7 9a84  ..| ............
+00001560: e689 8be6 a99f e4bb 94e7 84a1 207c 2054  ............ | T
+00001570: 7365 2073 c4ab 206c c3ad 20c3 aa20 7473  se s.. l.. .. ts
+00001580: 6869 c3ba 2d6b 692d c3a1 2062 c3b4 207c  hi..-ki-.. b.. |
+00001590: 2054 7365 2073 c3ac 206c 6920 c493 2074   Tse s.. li .. t
+000015a0: 7368 6975 2d6b c4ab 2dc3 a120 62c3 b43f  shiu-k..-.. b..?
+000015b0: 207c 2054 73c4 9320 73c3 ac20 6c69 20c4   | Ts.. s.. li .
+000015c0: 9320 7473 6869 752d 6bc4 ab2d 6120 62c3  . tshiu-k..-a b.
+000015d0: b420 7c20 5473 c493 2073 c3ac 206c 6920  . | Ts.. s.. li 
+000015e0: c493 2074 7368 6975 2d6b c4ab 2d61 2062  .. tshiu-k..-a b
+000015f0: c58d 207c 0d0a 0d0a 5361 6e64 6869 2072  .. |....Sandhi r
+00001600: 756c 6573 2061 6c73 6f20 6368 616e 6765  ules also change
+00001610: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+00001620: 6520 6469 616c 6563 7420 6368 6f73 656e  e dialect chosen
+00001630: 2e0d 0a0d 0a7c 2074 6578 7420 7c20 6e6f  .....| text | no
+00001640: 2073 616e 6468 6920 7c20 736f 7574 6820   sandhi | south 
+00001650: 2020 7c20 6e6f 7274 6820 2020 7c0d 0a7c    | north   |..|
+00001660: 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d   ---- | --------
+00001670: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
+00001680: 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781  ----- |..| .....
+00001690: a320 7c20 54c3 a269 2d75 c3a2 6e20 2020  . | T..i-u..n   
+000016a0: 7c20 54c4 8169 2d75 c3a2 6e20 7c20 54c3  | T..i-u..n | T.
+000016b0: a069 2d75 c3a2 6e20 7c0d 0a0d 0a23 2323  .i-u..n |....###
+000016c0: 2320 5075 6e63 7475 6174 696f 6e0d 0a0d  # Punctuation...
+000016d0: 0a60 7075 6e63 7475 6174 696f 6e60 2053  .`punctuation` S
+000016e0: 7472 696e 670d 0a0d 0a2a 2060 666f 726d  tring....* `form
+000016f0: 6174 6020 2864 6566 6175 6c74 2920 2d20  at` (default) - 
+00001700: 636f 6e76 6572 7473 2043 6869 6e65 7365  converts Chinese
+00001710: 2d73 7479 6c65 2070 756e 6374 7561 7469  -style punctuati
+00001720: 6f6e 2074 6f20 4c61 7469 6e2d 7374 796c  on to Latin-styl
+00001730: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
+00001740: 6420 6361 7069 7461 6c69 7365 7320 776f  d capitalises wo
+00001750: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+00001760: 6e69 6e67 206f 6620 6561 6368 2073 656e  ning of each sen
+00001770: 7465 6e63 652e 0d0a 2a20 606e 6f6e 6560  tence...* `none`
+00001780: 202d 2070 7265 7365 7276 6573 2043 6869   - preserves Chi
+00001790: 6e65 7365 2d73 7479 6c65 2070 756e 6374  nese-style punct
+000017a0: 7561 7469 6f6e 2061 6e64 2064 6f65 736e  uation and doesn
+000017b0: 2774 2063 6170 6974 616c 6973 6520 776f  't capitalise wo
+000017c0: 7264 7320 6174 2074 6865 2062 6567 696e  rds at the begin
+000017d0: 6e69 6e67 206f 6620 6e65 7720 7365 6e74  ning of new sent
+000017e0: 656e 6365 732e 0d0a 0d0a 7c20 7465 7874  ences.....| text
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 2020 2020 2020 2020 207c 2066 6f72             | for
+00001840: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001890: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000018a0: 206e 6f6e 6520 2020 2020 2020 2020 2020   none           
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+00001910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001950: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
+00001960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+000019c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a20: 2d2d 2d2d 207c 0d0a 7c20 e980 99e6 98af  ---- |..| ......
+00001a30: e887 bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3  ................
+00001a40: 808c e58d 97e3 808d efbc 88e7 99bd e8a9  ................
+00001a50: b1e5 ad97 efbc 9a54 c3a2 692d 6cc3 a26d  .......T..i-l..m
+00001a60: efbc 9be6 b3a8 e99f b3e7 aca6 e899 9fef  ................
+00001a70: bc9a e384 8ae3 849e cb8a 20e3 848b e384  .......... .....
+00001a80: a2cb 8aef bc8c e59c 8be8 aa9e efbc 9a54  ...............T
+00001a90: c3a1 696e c3a1 6eef bc89 e380 8220 7c20  ..in..n...... | 
+00001aa0: 5473 6520 73c4 ab20 54c3 a269 2d6c c3a2  Tse s.. T..i-l..
+00001ab0: 6d2c 206b c3a1 6e2d 7473 6869 6e67 2022  m, k..n-tshing "
+00001ac0: 6cc3 a26d 2220 2850 65cc 8d68 2d75 c493  l..m" (Pe..h-u..
+00001ad0: 2d6a c4ab 3a20 54c3 a269 2d6c c3a2 6d3b  -j..: T..i-l..m;
+00001ae0: 2074 73c3 b92d 696d 2068 c3bb 2d68 c58d   ts..-im h..-h..
+00001af0: 3a20 e384 8ae3 849e cb8a 20e3 848b e384  : ........ .....
+00001b00: a2cb 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3  ..., kok-g..: T.
+00001b10: a169 6ec3 a16e 292e 207c 2074 7365 2073  .in..n). | tse s
+00001b20: c4ab 2054 c3a2 692d 6cc3 a26d efbc 8c6b  .. T..i-l..m...k
+00001b30: c3a1 6e2d 7473 6869 6e67 e380 8c6c c3a2  ..n-tshing...l..
+00001b40: 6de3 808d efbc 8850 65cc 8d68 2d75 c493  m......Pe..h-u..
+00001b50: 2d6a c4ab efbc 9a54 c3a2 692d 6cc3 a26d  -j.....T..i-l..m
+00001b60: efbc 9b74 73c3 b92d 696d 2068 c3bb 2d68  ...ts..-im h..-h
+00001b70: c58d efbc 9ae3 848a e384 9ecb 8a20 e384  ............. ..
+00001b80: 8be3 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad  .........kok-g..
+00001b90: efbc 9a54 c3a1 696e c3a1 6eef bc89 e380  ...T..in..n.....
+00001ba0: 8220 7c0d 0a0d 0a23 2323 2320 436f 6e76  . |....#### Conv
+00001bb0: 6572 7420 6e6f 6e2d 434a 4b0d 0a0d 0a60  ert non-CJK....`
+00001bc0: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b60  convert_non_cjk`
+00001bd0: 2042 6f6f 6c65 616e 202d 2064 6566 696e   Boolean - defin
+00001be0: 6573 2077 6865 7468 6572 206f 7220 6e6f  es whether or no
+00001bf0: 7420 746f 2063 6f6e 7665 7274 206e 6f6e  t to convert non
+00001c00: 2d43 6869 6e65 7365 2077 6f72 6473 2e20  -Chinese words. 
+00001c10: 4361 6e20 6265 2075 7365 6420 746f 2063  Can be used to c
+00001c20: 6f6e 7665 7274 2054 6169 6c6f 2074 6f20  onvert Tailo to 
+00001c30: 616e 6f74 6865 7220 726f 6d61 6e69 7361  another romanisa
+00001c40: 7469 6f6e 2073 7973 7465 6d2e 0d0a 0d0a  tion system.....
+00001c50: 2a20 6054 7275 6560 202d 2063 6f6e 7665  * `True` - conve
+00001c60: 7274 206e 6f6e 2d43 6869 6e65 7365 2063  rt non-Chinese c
+00001c70: 6861 7261 6374 6572 2077 6f72 6473 0d0a  haracter words..
+00001c80: 2a20 6046 616c 7365 6020 2864 6566 6175  * `False` (defau
+00001c90: 6c74 2920 2d20 636f 6e76 6572 7420 6f6e  lt) - convert on
+00001ca0: 6c79 2043 6869 6e65 7365 2063 6861 7261  ly Chinese chara
+00001cb0: 6374 6572 2077 6f72 6473 0d0a 0d0a 7c20  cter words....| 
+00001cc0: 7465 7874 2020 2020 2020 7c20 4661 6c73  text      | Fals
+00001cd0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001ce0: 2020 2020 7c20 5472 7565 2020 2020 2020      | True      
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+00001d00: 0a7c 202d 2d2d 2d2d 2d2d 2d2d 207c 202d  .| --------- | -
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 207c 0d0a 7c20 e688 91e9 a39f 7068 c3a1   |..| ......ph..
+00001d50: 6e67 207c 20e3 86a3 e384 a8e3 849a cb8b  ng | ...........
+00001d60: 20e3 8490 e384 a7e3 849a e386 b7cb 9920   .............. 
+00001d70: 7068 c3a1 6e67 207c 20e3 86a3 e384 a8e3  ph..ng | .......
+00001d80: 849a cb8b 20e3 8490 e384 a7e3 849a e386  .... ...........
+00001d90: b7cb 9920 e384 86e3 84a4 cb8b 207c 0d0a  ... ........ |..
+00001da0: 0d0a 2323 2320 546f 6b65 6e69 7365 720d  ..### Tokeniser.
+00001db0: 0a0d 0a60 546f 6b65 6e69 7365 7260 2063  ...`Tokeniser` c
+00001dc0: 6c61 7373 2070 6572 666f 726d 7320 5b4e  lass performs [N
+00001dd0: 4c54 4b20 776f 7264 7075 6e63 745f 746f  LTK wordpunct_to
+00001de0: 6b65 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b  kenize][nltk-tok
+00001df0: 656e 697a 655d 2d6c 696b 6520 746f 6b65  enize]-like toke
+00001e00: 6e69 7361 7469 6f6e 206f 6620 6120 5461  nisation of a Ta
+00001e10: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
+00001e20: 7365 6e74 656e 6365 2e0d 0a0d 0a60 6060  sentence.....```
+00001e30: 7079 7468 6f6e 0d0a 2320 436f 6e73 7472  python..# Constr
+00001e40: 7563 746f 720d 0a74 203d 2054 6f6b 656e  uctor..t = Token
+00001e50: 6973 6572 2829 0d0a 0d0a 2320 546f 6b65  iser()....# Toke
+00001e60: 6e69 7365 2054 6169 7761 6e65 7365 2048  nise Taiwanese H
+00001e70: 6f6b 6b69 656e 2073 656e 7465 6e63 650d  okkien sentence.
+00001e80: 0a74 2e74 6f6b 656e 6973 6528 696e 7075  .t.tokenise(inpu
+00001e90: 7429 0d0a 6060 600d 0a0d 0a23 2323 204f  t)..```....### O
+00001ea0: 7468 6572 2046 756e 6374 696f 6e73 0d0a  ther Functions..
+00001eb0: 0d0a 4861 6e64 7920 6675 6e63 7469 6f6e  ..Handy function
+00001ec0: 7320 666f 7220 4e4c 5020 7461 736b 7320  s for NLP tasks 
+00001ed0: 696e 2054 6169 7761 6e65 7365 2048 6f6b  in Taiwanese Hok
+00001ee0: 6b69 656e 2e0d 0a0d 0a60 6060 7079 7468  kien.....```pyth
+00001ef0: 6f6e 0d0a 2320 436f 6e76 6572 7420 746f  on..# Convert to
+00001f00: 2054 7261 6469 7469 6f6e 616c 0d0a 746f   Traditional..to
+00001f10: 5f74 7261 6469 7469 6f6e 616c 2869 6e70  _traditional(inp
+00001f20: 7574 290d 0a0d 0a23 2043 6f6e 7665 7274  ut)....# Convert
+00001f30: 2074 6f20 5369 6d70 6c69 6669 6564 0d0a   to Simplified..
+00001f40: 746f 5f73 696d 706c 6966 6965 6428 696e  to_simplified(in
+00001f50: 7075 7429 0d0a 0d0a 2320 4368 6563 6b20  put)....# Check 
+00001f60: 6966 2074 6865 2073 7472 696e 6720 6973  if the string is
+00001f70: 2066 756c 6c79 2063 6f6d 706f 7365 6420   fully composed 
+00001f80: 6f66 2043 6869 6e65 7365 2063 6861 7261  of Chinese chara
+00001f90: 6374 6572 730d 0a69 735f 636a 6b28 696e  cters..is_cjk(in
+00001fa0: 7075 7429 0d0a 6060 600d 0a0d 0a0d 0a0d  put)..```.......
+00001fb0: 0a3c 212d 2d20 4558 414d 504c 4520 2d2d  .<!-- EXAMPLE --
+00001fc0: 3e0d 0a23 2320 4578 616d 706c 650d 0a0d  >..## Example...
+00001fd0: 0a60 6060 7079 7468 6f6e 0d0a 2320 436f  .```python..# Co
+00001fe0: 6e76 6572 7465 720d 0a66 726f 6d20 7461  nverter..from ta
+00001ff0: 6962 756e 2069 6d70 6f72 7420 436f 6e76  ibun import Conv
+00002000: 6572 7465 720d 0a0d 0a23 2320 5379 7374  erter....## Syst
+00002010: 656d 0d0a 6320 3d20 436f 6e76 6572 7465  em..c = Converte
+00002020: 7228 2920 2320 5461 696c 6f20 7379 7374  r() # Tailo syst
+00002030: 656d 2064 6566 6175 6c74 0d0a 632e 6765  em default..c.ge
+00002040: 7428 27e5 8588 e794 9fe8 ac9b efbc 8ce5  t('.............
+00002050: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
+00002060: 8227 290d 0a3e 3e20 5369 616e 2d73 696e  .')..>> Sian-sin
+00002070: 6e20 6bc3 b36e 672c 2068 61cc 8d6b 2d73  n k..ng, ha..k-s
+00002080: 696e 6720 7469 c481 6d2d 7469 c481 6d20  ing ti..m-ti..m 
+00002090: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
+000020a0: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
+000020b0: 275a 6875 7969 6e27 290d 0a63 2e67 6574  'Zhuyin')..c.get
+000020c0: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
+000020d0: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
+000020e0: 2729 0d0a 3e3e 20e3 8492 e384 a7e3 84a2  ')..>> .........
+000020f0: 20e3 8492 e386 aa20 e384 8de3 86b2 cb8b   ...... ........
+00002100: 2c20 e384 8fe3 849a e386 b6cb 9920 e384  , ........... ..
+00002110: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
+00002120: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
+00002130: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2323  ..............##
+00002140: 2044 6961 6c65 6374 0d0a 6320 3d20 436f   Dialect..c = Co
+00002150: 6e76 6572 7465 7228 2920 2320 736f 7574  nverter() # sout
+00002160: 6820 6469 616c 6563 7420 6465 6661 756c  h dialect defaul
+00002170: 740d 0a63 2e67 6574 2822 e688 91e6 acb2  t..c.get("......
+00002180: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
+00002190: 3e3e 2047 75c3 a120 6265 6820 c4ab 6e67  >> Gu.. beh ..ng
+000021a0: 2074 c4ab 2074 7369 61cc 8d68 2068 c3ae   t.. tsia..h h..
+000021b0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+000021c0: 7228 6469 616c 6563 743d 276e 6f72 7468  r(dialect='north
+000021d0: 2729 0d0a 632e 6765 7428 22e6 8891 e6ac  ')..c.get(".....
+000021e0: b2e7 94a8 e7ae b8e9 a39f e9ad 9a22 290d  .............").
+000021f0: 0a3e 3e20 4775 c3a1 2062 7565 6820 c4ab  .>> Gu.. bueh ..
+00002200: 6e67 2074 c5ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
+00002210: c3bb 0d0a 0d0a 2323 2046 6f72 6d61 740d  ......## Format.
+00002220: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
+00002230: 2023 2066 6f72 2054 6169 6c6f 2c20 6d61   # for Tailo, ma
+00002240: 726b 2062 7920 6465 6661 756c 740d 0a63  rk by default..c
+00002250: 2e67 6574 2822 e794 9fe6 97a5 e5bf abe6  .get("..........
+00002260: a882 2229 0d0a 3e3e 2053 656e 6e2d 6a69  ..")..>> Senn-ji
+00002270: cc8d 7420 6b68 75c3 a069 2d6c 6fcc 8d6b  ..t khu..i-lo..k
+00002280: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00002290: 7228 666f 726d 6174 3d27 6e75 6d62 6572  r(format='number
+000022a0: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
+000022b0: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
+000022c0: 6e6e 312d 6a69 7438 206b 6875 6169 332d  nn1-jit8 khuai3-
+000022d0: 6c6f 6b38 0d0a 0d0a 6320 3d20 436f 6e76  lok8....c = Conv
+000022e0: 6572 7465 7228 666f 726d 6174 3d27 7374  erter(format='st
+000022f0: 7269 7027 290d 0a63 2e67 6574 2822 e794  rip')..c.get("..
+00002300: 9fe6 97a5 e5bf abe6 a882 2229 0d0a 3e3e  ..........")..>>
+00002310: 2053 656e 6e2d 6a69 7420 6b68 7561 692d   Senn-jit khuai-
+00002320: 6c6f 6b0d 0a0d 0a23 2320 4465 6c69 6d69  lok....## Delimi
+00002330: 7465 720d 0a63 203d 2043 6f6e 7665 7274  ter..c = Convert
+00002340: 6572 2864 656c 696d 6974 6572 3d27 2729  er(delimiter='')
+00002350: 0d0a 632e 6765 7428 22e5 8588 e794 9fe8  ..c.get(".......
+00002360: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
+00002370: ace8 81bd e380 8222 290d 0a3e 3e20 5369  .......")..>> Si
+00002380: 616e 7369 6e6e 206b c3b3 6e67 2c20 6861  ansinn k..ng, ha
+00002390: cc8d 6b73 696e 6720 7469 c481 6d74 69c4  ..ksing ti..mti.
+000023a0: 816d 2074 6869 616e 6e2e 0d0a 0d0a 6320  .m thiann.....c 
+000023b0: 3d20 436f 6e76 6572 7465 7228 7379 7374  = Converter(syst
+000023c0: 656d 3d27 5069 6e67 7969 6d27 2c20 6465  em='Pingyim', de
+000023d0: 6c69 6d69 7465 723d 272d 2729 0d0a 632e  limiter='-')..c.
+000023e0: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
+000023f0: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
+00002400: e380 8222 290d 0a3e 3e20 5369 c481 6e2d  ...")..>> Si..n-
+00002410: 736e c4ab 2067 c792 6e67 2c20 68c3 a167  sn.. g..ng, h..g
+00002420: 2d73 c4ab 6e67 2064 69c3 a26d 2d64 69c3  -s..ng di..m-di.
+00002430: a26d 2074 696e c481 2e0d 0a0d 0a23 2320  .m tin.......## 
+00002440: 5361 6e64 6869 0d0a 6320 3d20 436f 6e76  Sandhi..c = Conv
+00002450: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
+00002460: 696c 6f2c 2073 616e 6468 6920 6e6f 6e65  ilo, sandhi none
+00002470: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
+00002480: 6574 2822 e980 99e6 98af e58f b0e7 81a3  et("............
+00002490: e59b a1e4 bb94 2229 0d0a 3e3e 2054 7365  ......")..>> Tse
+000024a0: 2073 c4ab 2054 c3a2 692d 75c3 a26e 2067   s.. T..i-u..n g
+000024b0: c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20 436f  ..n-......c = Co
+000024c0: 6e76 6572 7465 7228 7361 6e64 6869 3d27  nverter(sandhi='
+000024d0: 6175 746f 2729 0d0a 632e 6765 7428 22e9  auto')..c.get(".
+000024e0: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
+000024f0: 9422 290d 0a3e 3e20 5473 6520 73c3 ac20  .")..>> Tse s.. 
+00002500: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
+00002510: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
+00002520: 7228 7361 6e64 6869 3d27 6578 635f 6c61  r(sandhi='exc_la
+00002530: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+00002540: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+00002550: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+00002560: c481 692d 75c4 816e 2067 696e 2dc3 a10d  ..i-u..n gin-...
+00002570: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
+00002580: 2873 616e 6468 693d 2769 6e63 6c5f 6c61  (sandhi='incl_la
+00002590: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
+000025a0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+000025b0: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
+000025c0: c481 692d 75c4 816e 2067 696e 2d61 0d0a  ..i-u..n gin-a..
+000025d0: 0d0a 2323 2050 756e 6374 7561 7469 6f6e  ..## Punctuation
+000025e0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000025f0: 2920 2320 666f 726d 6174 2070 756e 6374  ) # format punct
+00002600: 7561 7469 6f6e 2064 6566 6175 6c74 0d0a  uation default..
+00002610: 632e 6765 7428 22e5 a4aa e7a9 bae6 9c8b  c.get(".........
+00002620: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
+00002630: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
+00002640: 0d0a 3e3e 2054 68c3 a069 2d6b 686f 6e67  ..>> Th..i-khong
+00002650: 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
+00002660: 2d68 c3b3 2120 4cc3 ad6e 2074 7369 61cc  -h..! L..n tsia.
+00002670: 8d68 2d70 c3a1 2062 75c4 933f 0d0a 0d0a  .h-p.. bu..?....
+00002680: 6320 3d20 436f 6e76 6572 7465 7228 7075  c = Converter(pu
+00002690: 6e63 7475 6174 696f 6e3d 276e 6f6e 6527  nctuation='none'
+000026a0: 290d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  )..c.get("......
+000026b0: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
+000026c0: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
+000026d0: 9f22 290d 0a3e 3e20 7468 c3a0 692d 6b68  .")..>> th..i-kh
+000026e0: 6f6e 6720 70c3 ae6e 672d 69c3 baef bc8c  ong p..ng-i.....
+000026f0: 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad 6e20  l..n-h.....l..n 
+00002700: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
+00002710: efbc 9f0d 0a0d 0a23 2320 436f 6e76 6572  .......## Conver
+00002720: 7420 6e6f 6e2d 434a 4b0d 0a63 203d 2043  t non-CJK..c = C
+00002730: 6f6e 7665 7274 2873 7973 7465 6d3d 275a  onvert(system='Z
+00002740: 6875 7969 6e27 2920 2320 4661 6c73 6520  huyin') # False 
+00002750: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b20  convert_non_cjk 
+00002760: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
+00002770: e688 91e9 a39f 7068 c3a1 6e67 2229 0d0a  ......ph..ng")..
+00002780: 3e3e 20e3 86a3 e384 a8e3 849a cb8b 20e3  >> ........... .
+00002790: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
+000027a0: c3a1 6e67 0d0a 0d0a 6320 3d20 436f 6e76  ..ng....c = Conv
+000027b0: 6572 7428 7379 7374 656d 3d27 5a68 7579  ert(system='Zhuy
+000027c0: 696e 272c 2063 6f6e 7665 7274 5f6e 6f6e  in', convert_non
+000027d0: 5f63 6a6b 3d54 7275 6529 0d0a 632e 6765  _cjk=True)..c.ge
+000027e0: 7428 22e6 8891 e9a3 9f70 68c3 a16e 6722  t("......ph..ng"
+000027f0: 290d 0a3e 3e20 e386 a3e3 84a8 e384 9acb  )..>> ..........
+00002800: 8b20 e384 90e3 84a7 e384 9ae3 86b7 cb99  . ..............
+00002810: 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23   ..............#
+00002820: 2054 6f6b 656e 6973 6572 0d0a 6672 6f6d   Tokeniser..from
+00002830: 2074 6169 6275 6e20 696d 706f 7274 2054   taibun import T
+00002840: 6f6b 656e 6973 6572 0d0a 0d0a 7420 3d20  okeniser....t = 
+00002850: 546f 6b65 6e69 7365 7228 290d 0a74 2e74  Tokeniser()..t.t
+00002860: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
+00002870: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
+00002880: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
+00002890: 2229 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27  ")..>> ['......'
+000028a0: 2c20 27e6 9c8b e58f 8b27 2c20 27ef bc8c  , '......', '...
+000028b0: 272c 2027 e681 81e5 a5bd 272c 2027 efbc  ', '......', '..
+000028c0: 8127 2c20 27e6 8181 272c 2027 e9a3 9fe9  .', '...', '....
+000028d0: a3bd 272c 2027 e69c aa27 2c20 27ef bc9f  ..', '...', '...
+000028e0: 275d 0d0a 0d0a 0d0a 2320 4f74 6865 7220  ']......# Other 
+000028f0: 4675 6e63 7469 6f6e 730d 0a66 726f 6d20  Functions..from 
+00002900: 7461 6962 756e 2069 6d70 6f72 7420 746f  taibun import to
+00002910: 5f74 7261 6469 7469 6f6e 616c 2c20 746f  _traditional, to
+00002920: 5f73 696d 706c 6966 6965 642c 2069 735f  _simplified, is_
+00002930: 636a 6b0d 0a0d 0a74 6f5f 7472 6164 6974  cjk....to_tradit
+00002940: 696f 6e61 6c28 22e6 8891 e590 ace6 97a0  ional(".........
+00002950: e58f b0e6 b9be e8af 9d22 290d 0a3e 3e20  .........")..>> 
+00002960: e688 91e8 81bd e784 a1e5 8fb0 e781 a3e8  ................
+00002970: a9b1 0d0a 0d0a 746f 5f73 696d 706c 6966  ......to_simplif
+00002980: 6965 6428 22e6 8891 e881 bde7 84a1 e887  ied("...........
+00002990: bae7 81a3 e8a9 b122 290d 0a3e 3e20 e688  .......")..>> ..
+000029a0: 91e5 90ac e697 a0e5 8fb0 e6b9 bee8 af9d  ................
+000029b0: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+000029c0: a39f e9ba ad27 290d 0a3e 3e20 5472 7565  .....')..>> True
+000029d0: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
+000029e0: a39f 7068 c3a1 6e67 2729 0d0a 3e3e 2046  ..ph..ng')..>> F
+000029f0: 616c 7365 0d0a 6060 600d 0a0d 0a0d 0a0d  alse..```.......
+00002a00: 0a3c 212d 2d20 4441 5441 202d 2d3e 0d0a  .<!-- DATA -->..
+00002a10: 2323 2044 6174 610d 0a0d 0a2d 205b 5461  ## Data....- [Ta
+00002a20: 6977 616e 6573 652d 4368 696e 6573 6520  iwanese-Chinese 
+00002a30: 4f6e 6c69 6e65 2044 6963 7469 6f6e 6172  Online Dictionar
+00002a40: 795d 5b6f 6e6c 696e 652d 6469 6374 696f  y][online-dictio
+00002a50: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
+00002a60: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
+00002a70: 5d29 0d0a 2d20 5b69 5461 6967 6920 4368  ])..- [iTaigi Ch
+00002a80: 696e 6573 652d 5461 6977 616e 6573 6520  inese-Taiwanese 
+00002a90: 436f 6d70 6172 6973 6f6e 2044 6963 7469  Comparison Dicti
+00002aa0: 6f6e 6172 795d 5b69 7461 6967 692d 6469  onary][itaigi-di
+00002ab0: 6374 696f 6e61 7279 5d20 2876 6961 205b  ctionary] (via [
+00002ac0: 4368 686f 6554 6169 6769 5d5b 6461 7461  ChhoeTaigi][data
+00002ad0: 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21  -via])........<!
+00002ae0: 2d2d 2041 434b 4e4f 574c 4544 4745 4d45  -- ACKNOWLEDGEME
+00002af0: 4e54 5320 2d2d 3e0d 0a23 2320 4163 6b6e  NTS -->..## Ackn
+00002b00: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
+00002b10: 2d20 5361 6d75 656c 204a 656e 2028 5b47  - Samuel Jen ([G
+00002b20: 6974 6875 625d 5b73 616d 7565 6c2d 6769  ithub][samuel-gi
+00002b30: 7468 7562 5d20 c2b7 205b 4c69 6e6b 6564  thub] .. [Linked
+00002b40: 496e 5d5b 7361 6d75 656c 2d6c 696e 6b65  In][samuel-linke
+00002b50: 6469 6e5d 2920 2d20 5461 6977 616e 6573  din]) - Taiwanes
+00002b60: 6520 616e 6420 4d61 6e64 6172 696e 2074  e and Mandarin t
+00002b70: 7261 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a  ranslation......
+00002b80: 0d0a 3c21 2d2d 204c 4943 454e 4345 202d  ..<!-- LICENCE -
+00002b90: 2d3e 0d0a 2323 204c 6963 656e 6365 0d0a  ->..## Licence..
+00002ba0: 0d0a 4265 6361 7573 6520 5461 6962 756e  ..Because Taibun
+00002bb0: 2069 7320 4d49 542d 6c69 6365 6e73 6564   is MIT-licensed
+00002bc0: 2c20 616e 7920 6465 7665 6c6f 7065 7220  , any developer 
+00002bd0: 6361 6e20 6573 7365 6e74 6961 6c6c 7920  can essentially 
+00002be0: 646f 2077 6861 7465 7665 7220 7468 6579  do whatever they
+00002bf0: 2077 616e 7420 7769 7468 2069 7420 6173   want with it as
+00002c00: 206c 6f6e 6720 6173 2074 6865 7920 696e   long as they in
+00002c10: 636c 7564 6520 7468 6520 6f72 6967 696e  clude the origin
+00002c20: 616c 2063 6f70 7972 6967 6874 2061 6e64  al copyright and
+00002c30: 206c 6963 656e 6365 206e 6f74 6963 6520   licence notice 
+00002c40: 696e 2061 6e79 2063 6f70 6965 7320 6f66  in any copies of
+00002c50: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
+00002c60: 2e20 4e6f 7465 2c20 7468 6174 2074 6865  . Note, that the
+00002c70: 2064 6174 6120 7573 6564 2062 7920 7468   data used by th
+00002c80: 6520 7061 636b 6167 6520 6973 206c 6963  e package is lic
+00002c90: 656e 7365 6420 756e 6465 7220 6120 6469  ensed under a di
+00002ca0: 6666 6572 656e 7420 636f 7079 7269 6768  fferent copyrigh
+00002cb0: 742e 0d0a 0d0a 5468 6520 6461 7461 2069  t.....The data i
+00002cc0: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00002cd0: 205b 4343 2042 592d 5341 2034 2e30 5d5b   [CC BY-SA 4.0][
+00002ce0: 6461 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a  data-cc]........
+00002cf0: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
+00002d00: 4e4b 5320 2d2d 3e0d 0a5b 636f 6e74 7269  NKS -->..[contri
+00002d10: 6275 7469 6f6e 735d 3a20 6874 7470 733a  butions]: https:
+00002d20: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e64  //github.com/and
+00002d30: 7265 6968 6172 2f74 6169 6275 6e2f 6973  reihar/taibun/is
+00002d40: 7375 6573 0d0a 5b63 6f6e 7472 6962 7574  sues..[contribut
+00002d50: 696f 6e73 2d62 6164 6765 5d3a 2068 7474  ions-badge]: htt
+00002d60: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00002d70: 2e69 6f2f 6261 6467 652f 436f 6e74 7269  .io/badge/Contri
+00002d80: 6275 7469 6f6e 732d 5765 6c63 6f6d 6564  butions-Welcomed
+00002d90: 2d62 6531 3332 643f 7374 796c 653d 666f  -be132d?style=fo
+00002da0: 722d 7468 652d 6261 6467 6526 6c6f 676f  r-the-badge&logo
+00002db0: 3d67 6974 6875 620d 0a5b 7465 7374 735d  =github..[tests]
+00002dc0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002dd0: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
+00002de0: 6169 6275 6e2f 6163 7469 6f6e 730d 0a5b  aibun/actions..[
+00002df0: 7465 7374 732d 6261 6467 655d 3a20 6874  tests-badge]: ht
+00002e00: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00002e10: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
+00002e20: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
+00002e30: 7475 732f 616e 6472 6569 6861 722f 7461  tus/andreihar/ta
+00002e40: 6962 756e 2f63 692e 7961 6d6c 3f73 7479  ibun/ci.yaml?sty
+00002e50: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00002e60: 266c 6f67 6f3d 6769 7468 7562 2d61 6374  &logo=github-act
+00002e70: 696f 6e73 266c 6f67 6f43 6f6c 6f72 3d66  ions&logoColor=f
+00002e80: 6666 6666 660d 0a5b 7265 6c65 6173 652d  fffff..[release-
+00002e90: 6261 6467 655d 3a20 6874 7470 733a 2f2f  badge]: https://
+00002ea0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00002eb0: 6974 6875 622f 762f 7265 6c65 6173 652f  ithub/v/release/
+00002ec0: 616e 6472 6569 6861 722f 7461 6962 756e  andreihar/taibun
+00002ed0: 3f63 6f6c 6f72 3d33 3836 3138 6326 7374  ?color=38618c&st
+00002ee0: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00002ef0: 650d 0a5b 7265 6c65 6173 655d 3a20 6874  e..[release]: ht
+00002f00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002f10: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00002f20: 6e2f 7265 6c65 6173 6573 0d0a 5b6c 6963  n/releases..[lic
+00002f30: 656e 6365 2d62 6164 6765 5d3a 2068 7474  ence-badge]: htt
+00002f40: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00002f50: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
+00002f60: 7365 2f61 6e64 7265 6968 6172 2f74 6169  se/andreihar/tai
+00002f70: 6275 6e3f 636f 6c6f 723d 3030 3030 3030  bun?color=000000
+00002f80: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
+00002f90: 6164 6765 0d0a 5b6c 6963 656e 6365 5d3a  adge..[licence]:
+00002fa0: 204c 4943 454e 5345 0d0a 5b6c 696e 6b65   LICENSE..[linke
+00002fb0: 6469 6e2d 6261 6467 655d 3a20 6874 7470  din-badge]: http
+00002fc0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00002fd0: 696f 2f62 6164 6765 2f4c 696e 6b65 6449  io/badge/LinkedI
+00002fe0: 6e2d 3030 3737 6235 3f73 7479 6c65 3d66  n-0077b5?style=f
+00002ff0: 6f72 2d74 6865 2d62 6164 6765 266c 6f67  or-the-badge&log
+00003000: 6f3d 6c69 6e6b 6564 696e 266c 6f67 6f43  o=linkedin&logoC
+00003010: 6f6c 6f72 3d66 6666 6666 660d 0a5b 6c69  olor=ffffff..[li
+00003020: 6e6b 6564 696e 5d3a 2068 7474 7073 3a2f  nkedin]: https:/
+00003030: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+00003040: 6d2f 696e 2f61 6e64 7265 692d 6861 7262  m/in/andrei-harb
+00003050: 6163 686f 762f 0d0a 5b6a 732d 6261 6467  achov/..[js-badg
+00003060: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+00003070: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00003080: 2f4a 535f 5665 7273 696f 6e2d 6637 6466  /JS_Version-f7df
+00003090: 3165 3f73 7479 6c65 3d66 6f72 2d74 6865  1e?style=for-the
+000030a0: 2d62 6164 6765 266c 6f67 6f3d 6a61 7661  -badge&logo=java
+000030b0: 7363 7269 7074 266c 6f67 6f43 6f6c 6f72  script&logoColor
+000030c0: 3d30 3030 3030 300d 0a5b 6a73 2d6c 696e  =000000..[js-lin
+000030d0: 6b5d 3a20 6874 7470 733a 2f2f 6769 7468  k]: https://gith
+000030e0: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
+000030f0: 2f74 6169 6275 6e2e 6a73 0d0a 0d0a 5b70  /taibun.js....[p
+00003100: 7970 695d 3a20 6874 7470 733a 2f2f 7079  ypi]: https://py
+00003110: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
+00003120: 6169 6275 6e0d 0a5b 6275 675d 3a20 6874  aibun..[bug]: ht
+00003130: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003140: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00003150: 6e2f 6973 7375 6573 0d0a 5b6f 6e6c 696e  n/issues..[onlin
+00003160: 652d 6469 6374 696f 6e61 7279 5d3a 2068  e-dictionary]: h
+00003170: 7474 703a 2f2f 6970 3139 3430 3937 2e6e  ttp://ip194097.n
+00003180: 7463 752e 6564 752e 7477 2f75 6e67 6961  tcu.edu.tw/ungia
+00003190: 6e2f 736f 616e 6e74 656e 672f 6368 696c  n/soannteng/chil
+000031a0: 2f54 6169 686f 612e 6173 700d 0a5b 6974  /Taihoa.asp..[it
+000031b0: 6169 6769 2d64 6963 7469 6f6e 6172 795d  aigi-dictionary]
+000031c0: 3a20 6874 7470 733a 2f2f 6974 6169 6769  : https://itaigi
+000031d0: 2e74 772f 0d0a 5b64 6174 612d 7669 615d  .tw/..[data-via]
+000031e0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000031f0: 2e63 6f6d 2f43 6868 6f65 5461 6967 692f  .com/ChhoeTaigi/
+00003200: 4368 686f 6554 6169 6769 4461 7461 6261  ChhoeTaigiDataba
+00003210: 7365 0d0a 5b64 6174 612d 6363 5d3a 2068  se..[data-cc]: h
+00003220: 7474 7073 3a2f 2f63 7265 6174 6976 6563  ttps://creativec
+00003230: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
+00003240: 7365 732f 6279 2d73 612f 342e 302f 6465  ses/by-sa/4.0/de
+00003250: 6564 2e65 6e0d 0a5b 7361 6d75 656c 2d67  ed.en..[samuel-g
+00003260: 6974 6875 625d 3a20 6874 7470 733a 2f2f  ithub]: https://
+00003270: 6769 7468 7562 2e63 6f6d 2f53 5353 616d  github.com/SSSam
+00003280: 0d0a 5b73 616d 7565 6c2d 6c69 6e6b 6564  ..[samuel-linked
+00003290: 696e 5d3a 2068 7474 7073 3a2f 2f77 7777  in]: https://www
+000032a0: 2e6c 696e 6b65 6469 6e2e 636f 6d2f 696e  .linkedin.com/in
+000032b0: 2f73 616d 7565 6c2d 6a65 6e2f 0d0a 0d0a  /samuel-jen/....
+000032c0: 5b74 6169 6c6f 2d77 696b 695d 3a20 6874  [tailo-wiki]: ht
+000032d0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000032e0: 6961 2e6f 7267 2f77 696b 692f 5425 4333  ia.org/wiki/T%C3
+000032f0: 2541 3269 2d75 2543 3325 4132 6e5f 4c25  %A2i-u%C3%A2n_L%
+00003300: 4333 2542 342d 6d25 4333 2541 312d 6a25  C3%B4-m%C3%A1-j%
+00003310: 4334 2541 425f 5068 696e 672d 696d 5f48  C4%AB_Phing-im_H
+00003320: 6f6e 672d 2543 3325 4130 6e0d 0a5b 706f  ong-%C3%A0n..[po
+00003330: 6a2d 7769 6b69 5d3a 2068 7474 7073 3a2f  j-wiki]: https:/
+00003340: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00003350: 672f 7769 6b69 2f50 6525 4343 2538 4468  g/wiki/Pe%CC%8Dh
+00003360: 2d25 4335 2538 4465 2d6a 2543 3425 4142  -%C5%8De-j%C4%AB
+00003370: 0d0a 5b7a 6875 7969 6e2d 7769 6b69 5d3a  ..[zhuyin-wiki]:
+00003380: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00003390: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
+000033a0: 6169 7761 6e65 7365 5f50 686f 6e65 7469  aiwanese_Phoneti
+000033b0: 635f 5379 6d62 6f6c 730d 0a5b 746c 7061  c_Symbols..[tlpa
+000033c0: 2d77 696b 695d 3a20 6874 7470 733a 2f2f  -wiki]: https://
+000033d0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+000033e0: 2f77 696b 692f 5461 6977 616e 6573 655f  /wiki/Taiwanese_
+000033f0: 4c61 6e67 7561 6765 5f50 686f 6e65 7469  Language_Phoneti
+00003400: 635f 416c 7068 6162 6574 0d0a 5b70 696e  c_Alphabet..[pin
+00003410: 6779 696d 2d77 696b 695d 3a20 6874 7470  gyim-wiki]: http
+00003420: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00003430: 2e6f 7267 2f77 696b 692f 4262 2543 3325  .org/wiki/Bb%C3%
+00003440: 4131 6e6c 2543 3325 4131 6d5f 7025 4333  A1nl%C3%A1m_p%C3
+00003450: 2541 436e 6779 2543 3425 4142 6d0d 0a5b  %ACngy%C4%ABm..[
+00003460: 746f 6e67 696f 6e67 2d77 696b 695d 3a20  tongiong-wiki]: 
+00003470: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00003480: 6564 6961 2e6f 7267 2f77 696b 692f 4461  edia.org/wiki/Da
+00003490: 2543 3425 4142 2d67 6825 4333 2541 455f  %C4%AB-gh%C3%AE_
+000034a0: 7425 4335 2538 446e 672d 6925 4335 2538  t%C5%8Dng-i%C5%8
+000034b0: 446e 675f 7025 4334 2541 426e 672d 696d  Dng_p%C4%ABng-im
+000034c0: 0d0a 5b69 7061 2d77 696b 695d 3a20 6874  ..[ipa-wiki]: ht
+000034d0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000034e0: 6961 2e6f 7267 2f77 696b 692f 496e 7465  ia.org/wiki/Inte
+000034f0: 726e 6174 696f 6e61 6c5f 5068 6f6e 6574  rnational_Phonet
+00003500: 6963 5f41 6c70 6861 6265 740d 0a5b 7a68  ic_Alphabet..[zh
+00003510: 616e 677a 686f 752d 7769 6b69 5d3a 2068  angzhou-wiki]: h
+00003520: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00003530: 6469 612e 6f72 672f 7769 6b69 2f5a 6861  dia.org/wiki/Zha
+00003540: 6e67 7a68 6f75 5f64 6961 6c65 6374 730d  ngzhou_dialects.
+00003550: 0a5b 7175 616e 7a68 6f75 2d77 696b 695d  .[quanzhou-wiki]
+00003560: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003570: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003580: 5175 616e 7a68 6f75 5f64 6961 6c65 6374  Quanzhou_dialect
+00003590: 730d 0a5b 6e6c 746b 2d74 6f6b 656e 697a  s..[nltk-tokeniz
+000035a0: 655d 3a20 6874 7470 733a 2f2f 6e6c 746b  e]: https://nltk
+000035b0: 2e6f 7267 2f61 7069 2f6e 6c74 6b2e 746f  .org/api/nltk.to
+000035c0: 6b65 6e69 7a65 2e68 746d 6c0d 0a5b 7361  kenize.html..[sa
+000035d0: 6e64 6869 2d77 696b 695d 3a20 6874 7470  ndhi-wiki]: http
+000035e0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+000035f0: 2e6f 7267 2f77 696b 692f 5461 6977 616e  .org/wiki/Taiwan
+00003600: 6573 655f 486f 6b6b 6965 6e23 546f 6e65  ese_Hokkien#Tone
+00003610: 2532 3073 616e 6468 693a 7e3a 7465 7874  %20sandhi:~:text
+00003620: 3d74 686e 6725 4532 2539 4625 4139 2532  =thng%E2%9F%A9%2
+00003630: 3028 2532 3273 6f75 7025 3232 292e 2d2c  0(%22soup%22).-,
+00003640: 546f 6e65 2532 3073 616e 6468 692c 2d25  Tone%20sandhi,-%
+00003650: 3542 6564 6974 2535 44                   5Bedit%5D
```

### Comparing `example990420-1.1.0/README.md` & `example990420-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,763 +1,920 @@
-00000000: 3c21 2d2d 2050 524f 4a45 4354 204c 4f47  <!-- PROJECT LOG
-00000010: 4f20 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c  O -->..<br />..<
-00000020: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000030: 7222 3e0d 0a20 200d 0a23 2054 6169 6275  r">..  ..# Taibu
-00000040: 6e0d 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052  n........<!-- PR
-00000050: 4f4a 4543 5420 5348 4945 4c44 5320 2d2d  OJECT SHIELDS --
-00000060: 3e0d 0a5b 215b 5465 7374 735d 5b74 6573  >..[![Tests][tes
-00000070: 7473 2d62 6164 6765 5d5d 5b74 6573 7473  ts-badge]][tests
-00000080: 5d0d 0a5b 215b 436f 6e74 7269 6275 746f  ]..[![Contributo
-00000090: 7273 5d5b 636f 6e74 7269 6275 746f 7273  rs][contributors
-000000a0: 2d62 6164 6765 5d5d 5b63 6f6e 7472 6962  -badge]][contrib
-000000b0: 7574 6f72 735d 0d0a 5b21 5b52 656c 6561  utors]..[![Relea
-000000c0: 7365 5d5b 7265 6c65 6173 652d 6261 6467  se][release-badg
-000000d0: 655d 5d5b 7265 6c65 6173 655d 0d0a 5b21  e]][release]..[!
-000000e0: 5b4c 6963 656e 6365 5d5b 6c69 6365 6e63  [Licence][licenc
-000000f0: 652d 6261 6467 655d 5d5b 6c69 6365 6e63  e-badge]][licenc
-00000100: 655d 0d0a 5b21 5b4c 696e 6b65 6449 6e5d  e]..[![LinkedIn]
-00000110: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
-00000120: 5d5b 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a  ][linkedin]....*
-00000130: 2a54 6169 7761 6e65 7365 2048 6f6b 6b69  *Taiwanese Hokki
-00000140: 656e 2054 7261 6e73 6c69 7465 7261 746f  en Transliterato
-00000150: 7220 616e 6420 546f 6b65 6e69 7365 722a  r and Tokeniser*
-00000160: 2a0d 0a0d 0a49 7420 6861 7320 6d65 7468  *....It has meth
-00000170: 6f64 7320 7468 6174 2061 6c6c 6f77 2074  ods that allow t
-00000180: 6f20 6375 7374 6f6d 6973 6520 7472 616e  o customise tran
-00000190: 736c 6974 6572 6174 696f 6e20 616e 6420  sliteration and 
-000001a0: 7265 7472 6965 7665 2061 6e79 206e 6563  retrieve any nec
-000001b0: 6573 7361 7279 2069 6e66 6f72 6d61 7469  essary informati
-000001c0: 6f6e 2061 626f 7574 2054 6169 7761 6e65  on about Taiwane
-000001d0: 7365 2048 6f6b 6b69 656e 2070 726f 6e75  se Hokkien pronu
-000001e0: 6e63 6961 7469 6f6e 2e3c 6272 202f 3e0d  nciation.<br />.
-000001f0: 0a49 6e63 6c75 6465 7320 776f 7264 2074  .Includes word t
-00000200: 6f6b 656e 6973 6572 2066 6f72 2054 6169  okeniser for Tai
-00000210: 7761 6e65 7365 2048 6f6b 6b69 656e 2e0d  wanese Hokkien..
-00000220: 0a0d 0a5b 5265 706f 7274 2042 7567 5d5b  ...[Report Bug][
-00000230: 6275 675d 20e2 80a2 0d0a 5b50 7950 495d  bug] .....[PyPI]
-00000240: 5b70 7970 695d 0d0a 0d0a 3c2f 6469 763e  [pypi]....</div>
-00000250: 0d0a 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d  ........---.....
-00000260: 0a0d 0a3c 212d 2d20 494e 5354 414c 4c20  ...<!-- INSTALL 
-00000270: 2d2d 3e0d 0a23 2320 496e 7374 616c 6c0d  -->..## Install.
-00000280: 0a0d 0a54 6169 6275 6e20 6361 6e20 6265  ...Taibun can be
-00000290: 2069 6e73 7461 6c6c 6564 2066 726f 6d20   installed from 
-000002a0: 5b70 7970 695d 5b70 7970 695d 0d0a 0d0a  [pypi][pypi]....
-000002b0: 6060 6062 6173 680d 0a24 2070 6970 2069  ```bash..$ pip i
-000002c0: 6e73 7461 6c6c 2074 6169 6275 6e0d 0a60  nstall taibun..`
-000002d0: 6060 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055  ``........<!-- U
-000002e0: 5341 4745 202d 2d3e 0d0a 2323 2055 7361  SAGE -->..## Usa
-000002f0: 6765 0d0a 0d0a 2323 2320 436f 6e76 6572  ge....### Conver
-00000300: 7465 720d 0a0d 0a60 436f 6e76 6572 7465  ter....`Converte
-00000310: 7260 2063 6c61 7373 2074 7261 6e73 6c69  r` class transli
-00000320: 7465 7261 7465 7320 7468 6520 4368 696e  terates the Chin
-00000330: 6573 6520 6368 6172 6163 7465 7273 2074  ese characters t
-00000340: 6f20 7468 6520 6368 6f73 656e 2074 7261  o the chosen tra
-00000350: 6e73 6c69 7465 7261 7469 6f6e 2073 7973  nsliteration sys
-00000360: 7465 6d20 7769 7468 2070 6172 616d 6574  tem with paramet
-00000370: 6572 7320 7370 6563 6966 6965 6420 6279  ers specified by
-00000380: 2074 6865 2064 6576 656c 6f70 6572 2e20   the developer. 
-00000390: 576f 726b 7320 666f 7220 626f 7468 2054  Works for both T
-000003a0: 7261 6469 7469 6f6e 616c 2061 6e64 2053  raditional and S
-000003b0: 696d 706c 6966 6965 6420 6368 6172 6163  implified charac
-000003c0: 7465 7273 2e0d 0a0d 0a60 6060 7079 7468  ters.....```pyth
-000003d0: 6f6e 0d0a 2320 636f 6e73 7472 7563 746f  on..# constructo
-000003e0: 720d 0a63 203d 2043 6f6e 7665 7274 6572  r..c = Converter
-000003f0: 2873 7973 7465 6d2c 2064 6961 6c65 6374  (system, dialect
-00000400: 2c20 666f 726d 6174 2c20 6465 6c69 6d69  , format, delimi
-00000410: 7465 722c 2073 616e 6468 692c 2070 756e  ter, sandhi, pun
-00000420: 6374 7561 7469 6f6e 2c20 636f 6e76 6572  ctuation, conver
-00000430: 745f 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320  t_non_cjk)....# 
-00000440: 7472 616e 736c 6974 6572 6174 6520 4368  transliterate Ch
-00000450: 696e 6573 6520 6368 6172 6163 7465 7273  inese characters
-00000460: 0d0a 632e 6765 7428 696e 7075 7429 0d0a  ..c.get(input)..
-00000470: 6060 600d 0a0d 0a23 2323 2320 5379 7374  ```....#### Syst
-00000480: 656d 0d0a 0d0a 6073 7973 7465 6d60 2053  em....`system` S
-00000490: 7472 696e 6720 2d20 7379 7374 656d 206f  tring - system o
-000004a0: 6620 7472 616e 736c 6974 6572 6174 696f  f transliteratio
-000004b0: 6e2e 0d0a 0d0a 2a20 6054 6169 6c6f 6020  n.....* `Tailo` 
-000004c0: 2864 6566 6175 6c74 2920 2d20 5b54 c3a2  (default) - [T..
-000004d0: 692d 75c3 a26e 204c c3b4 2d6d c3a1 2d6a  i-u..n L..-m..-j
-000004e0: c4ab 2050 6869 6e67 2d69 6d20 486f 6e67  .. Phing-im Hong
-000004f0: 2dc3 a06e 5d5b 7461 696c 6f2d 7769 6b69  -..n][tailo-wiki
-00000500: 5d0d 0a2a 2060 504f 4a60 202d 205b 5065  ]..* `POJ` - [Pe
-00000510: cc8d 682d c58d 652d 6ac4 ab5d 5b70 6f6a  ..h-..e-j..][poj
-00000520: 2d77 696b 695d 0d0a 2a20 605a 6875 7969  -wiki]..* `Zhuyi
-00000530: 6e60 202d 205b 5461 6977 616e 6573 6520  n` - [Taiwanese 
-00000540: 5068 6f6e 6574 6963 2053 796d 626f 6c73  Phonetic Symbols
-00000550: 5d5b 7a68 7579 696e 2d77 696b 695d 0d0a  ][zhuyin-wiki]..
-00000560: 2a20 6054 4c50 4160 202d 205b 5461 6977  * `TLPA` - [Taiw
-00000570: 616e 6573 6520 4c61 6e67 7561 6765 2050  anese Language P
-00000580: 686f 6e65 7469 6320 416c 7068 6162 6574  honetic Alphabet
-00000590: 5d5b 746c 7061 2d77 696b 695d 0d0a 2a20  ][tlpa-wiki]..* 
-000005a0: 6050 696e 6779 696d 6020 2d20 5b42 62c3  `Pingyim` - [Bb.
-000005b0: a16e 6cc3 a16d 2055 c493 2050 c3ac 6e67  .nl..m U.. P..ng
-000005c0: 79c4 ab6d 2048 c58d 6e67 27c3 a06e 5d5b  y..m H..ng'..n][
-000005d0: 7069 6e67 7969 6d2d 7769 6b69 5d0d 0a2a  pingyim-wiki]..*
-000005e0: 2060 546f 6e67 696f 6e67 6020 2d20 5b44   `Tongiong` - [D
-000005f0: 61c4 ab2d 6768 c3ae 2054 c58d 6e67 2d69  a..-gh.. T..ng-i
-00000600: c58d 6e67 2050 c4ab 6e67 2d69 6d5d 5b74  ..ng P..ng-im][t
-00000610: 6f6e 6769 6f6e 672d 7769 6b69 5d0d 0a2a  ongiong-wiki]..*
-00000620: 2060 4950 4160 202d 205b 496e 7465 726e   `IPA` - [Intern
-00000630: 6174 696f 6e61 6c20 5068 6f6e 6574 6963  ational Phonetic
-00000640: 2041 6c70 6861 6265 745d 5b69 7061 2d77   Alphabet][ipa-w
-00000650: 696b 695d 0d0a 0d0a 7c20 7465 7874 207c  iki]....| text |
-00000660: 2054 6169 6c6f 2020 207c 2050 4f4a 2020   Tailo   | POJ  
-00000670: 2020 207c 205a 6875 7969 6e20 2020 2020     | Zhuyin     
-00000680: 207c 2054 4c50 4120 2020 2020 207c 2050   | TLPA      | P
-00000690: 696e 6779 696d 207c 2054 6f6e 6769 6f6e  ingyim | Tongion
-000006a0: 6720 7c20 4950 4120 2020 2020 2020 2020  g | IPA         
-000006b0: 7c0d 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d  |..| ---- | ----
-000006c0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20  --- | ------- | 
-000006d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
-000006e0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
-000006f0: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d  - | -------- | -
-00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
-00000710: e58f b0e7 81a3 207c 2054 c3a2 692d 75c3  ...... | T..i-u.
-00000720: a26e 207c 2054 c3a2 692d 6fc3 a26e 207c  .n | T..i-o..n |
-00000730: 20e3 8489 e384 9ecb 8a20 e384 a8e3 84a2   ........ ......
-00000740: cb8a 207c 2054 6169 3520 7561 6e35 207c  .. | Tai5 uan5 |
-00000750: 2044 c3a1 6977 c3a1 6e20 207c 2054 c481   D..iw..n  | T..
-00000760: 692d 75c7 8e6e 2020 7c20 5461 69c2 b2e2  i-u..n  | Tai...
-00000770: 81b5 2075 616e c2b2 e281 b520 7c0d 0a0d  .. uan..... |...
-00000780: 0a23 2323 2320 4469 616c 6563 740d 0a0d  .#### Dialect...
-00000790: 0a60 6469 616c 6563 7460 2053 7472 696e  .`dialect` Strin
-000007a0: 6720 2d20 7072 6566 6572 7265 6420 7072  g - preferred pr
-000007b0: 6f6e 756e 6369 6174 696f 6e2e 0d0a 0d0a  onunciation.....
-000007c0: 2a20 6073 6f75 7468 6020 2864 6566 6175  * `south` (defau
-000007d0: 6c74 2920 2d20 5b5a 6861 6e67 7a68 6f75  lt) - [Zhangzhou
-000007e0: 5d5b 7a68 616e 677a 686f 752d 7769 6b69  ][zhangzhou-wiki
-000007f0: 5d2d 6c65 616e 696e 6720 7072 6f6e 756e  ]-leaning pronun
-00000800: 6369 6174 696f 6e0d 0a2a 2060 6e6f 7274  ciation..* `nort
-00000810: 6860 202d 205b 5175 616e 7a68 6f75 5d5b  h` - [Quanzhou][
-00000820: 7175 616e 7a68 6f75 2d77 696b 695d 2d6c  quanzhou-wiki]-l
-00000830: 6561 6e69 6e67 2070 726f 6e75 6e63 6961  eaning pronuncia
-00000840: 7469 6f6e 0d0a 0d0a 7c20 7465 7874 2020  tion....| text  
-00000850: 207c 2073 6f75 7468 2020 2020 2020 2020   | south        
-00000860: 207c 206e 6f72 7468 2020 2020 2020 2020   | north        
-00000870: 207c 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d   |..| ------ | -
-00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
-00000890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
-000008a0: 7c20 e4ba 94e6 9c88 e7af 8020 7c20 47c5  | ......... | G.
-000008b0: 8d6f 2d67 7565 cc8d 682d 7473 6568 207c  .o-gue..h-tseh |
-000008c0: 2047 c58d 6f2d 6765 cc8d 682d 7473 7565   G..o-ge..h-tsue
-000008d0: 6820 7c0d 0a0d 0a23 2323 2320 466f 726d  h |....#### Form
-000008e0: 6174 0d0a 0d0a 6066 6f72 6d61 7460 2053  at....`format` S
-000008f0: 7472 696e 6720 2d20 666f 726d 6174 2069  tring - format i
-00000900: 6e20 7768 6963 6820 746f 6e65 7320 7769  n which tones wi
-00000910: 6c6c 2062 6520 7265 7072 6573 656e 7465  ll be represente
-00000920: 6420 696e 2074 6865 2063 6f6e 7665 7274  d in the convert
-00000930: 6564 2073 656e 7465 6e63 652e 0d0a 0d0a  ed sentence.....
-00000940: 2a20 606d 6172 6b60 2028 6465 6661 756c  * `mark` (defaul
-00000950: 7429 202d 2075 7365 7320 6469 6163 7269  t) - uses diacri
-00000960: 7469 6373 2066 6f72 2065 6163 6820 7379  tics for each sy
-00000970: 6c6c 6162 6c65 2e20 4e6f 7420 6176 6169  llable. Not avai
-00000980: 6c61 626c 6520 666f 7220 544c 5041 2e0d  lable for TLPA..
-00000990: 0a2a 2060 6e75 6d62 6572 6020 2d20 6164  .* `number` - ad
-000009a0: 6420 6120 6e75 6d62 6572 2077 6869 6368  d a number which
-000009b0: 2072 6570 7265 7365 6e74 7320 7468 6520   represents the 
-000009c0: 746f 6e65 2061 7420 7468 6520 656e 6420  tone at the end 
-000009d0: 6f66 2074 6865 2073 796c 6c61 626c 650d  of the syllable.
-000009e0: 0a2a 2060 7374 7269 7060 202d 2072 656d  .* `strip` - rem
-000009f0: 6f76 6573 2061 6e79 2074 6f6e 6520 6d61  oves any tone ma
-00000a00: 726b 696e 670d 0a0d 0a7c 2074 6578 7420  rking....| text 
-00000a10: 7c20 6d61 726b 2020 2020 7c20 6e75 6d62  | mark    | numb
-00000a20: 6572 2020 2020 7c20 7374 7269 7020 2020  er    | strip   
-00000a30: 7c0d 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d  |..| ---- | ----
-00000a40: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20  --- | --------- 
-00000a50: 7c20 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5  | ------- |..| .
-00000a60: 8fb0 e781 a320 7c20 54c3 a269 2d75 c3a2  ..... | T..i-u..
-00000a70: 6e20 7c20 5461 6935 2d75 616e 3520 7c20  n | Tai5-uan5 | 
-00000a80: 5461 692d 7561 6e20 7c0d 0a0d 0a23 2323  Tai-uan |....###
-00000a90: 2320 4465 6c69 6d69 7465 720d 0a0d 0a60  # Delimiter....`
-00000aa0: 6465 6c69 6d69 7465 7260 2053 7472 696e  delimiter` Strin
-00000ab0: 6720 2d20 7365 7473 2074 6865 2064 656c  g - sets the del
-00000ac0: 696d 6974 6572 2063 6861 7261 6374 6572  imiter character
-00000ad0: 2074 6861 7420 7769 6c6c 2062 6520 706c   that will be pl
-00000ae0: 6163 6564 2069 6e20 6265 7477 6565 6e20  aced in between 
-00000af0: 7379 6c6c 6162 6c65 7320 6f66 2061 2077  syllables of a w
-00000b00: 6f72 642e 0d0a 0d0a 4465 6661 756c 7420  ord.....Default 
-00000b10: 7661 6c75 6520 6465 7065 6e64 7320 6f6e  value depends on
-00000b20: 2074 6865 2063 686f 7365 6e20 6073 7973   the chosen `sys
-00000b30: 7465 6d60 3a0d 0a0d 0a2a 2060 272d 2760  tem`:....* `'-'`
-00000b40: 202d 2066 6f72 2060 5461 696c 6f60 2c20   - for `Tailo`, 
-00000b50: 6050 4f4a 602c 2060 546f 6e67 696f 6e67  `POJ`, `Tongiong
-00000b60: 600d 0a2a 2060 2727 6020 2d20 666f 7220  `..* `''` - for 
-00000b70: 6050 696e 6779 696d 600d 0a2a 2060 2720  `Pingyim`..* `' 
-00000b80: 2760 202d 2066 6f72 2060 5a68 7579 696e  '` - for `Zhuyin
-00000b90: 602c 2060 544c 5041 602c 2060 4950 4160  `, `TLPA`, `IPA`
-00000ba0: 0d0a 0d0a 7c20 7465 7874 207c 2027 2d27  ....| text | '-'
-00000bb0: 2020 2020 207c 2027 2720 2020 2020 7c20       | ''     | 
-00000bc0: 2720 2720 2020 2020 7c0d 0a7c 202d 2d2d  ' '     |..| ---
-00000bd0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
-00000be0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
-00000bf0: 0d0a 7c20 e58f b0e7 81a3 207c 2054 c3a2  ..| ...... | T..
-00000c00: 692d 75c3 a26e 207c 2054 c3a2 6975 c3a2  i-u..n | T..iu..
-00000c10: 6e20 7c20 54c3 a269 2075 c3a2 6e20 7c0d  n | T..i u..n |.
-00000c20: 0a0d 0a23 2323 2320 5361 6e64 6869 0d0a  ...#### Sandhi..
-00000c30: 0d0a 6073 616e 6468 6960 2053 7472 696e  ..`sandhi` Strin
-00000c40: 6720 2d20 6170 706c 6965 7320 7468 6520  g - applies the 
-00000c50: 5b73 616e 6468 6920 7275 6c65 7320 6f66  [sandhi rules of
-00000c60: 2054 6169 7761 6e65 7365 2048 6f6b 6b69   Taiwanese Hokki
-00000c70: 656e 5d5b 7361 6e64 6869 2d77 696b 695d  en][sandhi-wiki]
-00000c80: 2074 6f20 7379 6c6c 6162 6c65 7320 6f66   to syllables of
-00000c90: 2061 2073 696e 676c 6520 776f 7264 2e0d   a single word..
-00000ca0: 0a0d 0a53 696e 6365 2069 7427 7320 6469  ...Since it's di
-00000cb0: 6666 6963 756c 7420 746f 2065 6e63 6f64  fficult to encod
-00000cc0: 6520 616c 6c20 7361 6e64 6869 2072 756c  e all sandhi rul
-00000cd0: 6573 2c20 5461 6962 756e 2070 726f 7669  es, Taibun provi
-00000ce0: 6465 7320 6d75 6c74 6970 6c65 206d 6f64  des multiple mod
-00000cf0: 6573 2066 6f72 2073 616e 6468 6920 636f  es for sandhi co
-00000d00: 6e76 6572 7369 6f6e 2074 6f20 616c 6c6f  nversion to allo
-00000d10: 7720 666f 7220 6375 7374 6f6d 6973 6564  w for customised
-00000d20: 2073 616e 6468 6920 6861 6e64 6c69 6e67   sandhi handling
-00000d30: 2e0d 0a0d 0a2a 2060 6e6f 6e65 6020 2d20  .....* `none` - 
-00000d40: 646f 6573 6e27 7420 7065 7266 6f72 6d20  doesn't perform 
-00000d50: 616e 7920 746f 6e65 2073 616e 6468 690d  any tone sandhi.
-00000d60: 0a2a 2060 6175 746f 6020 2d20 636c 6f73  .* `auto` - clos
-00000d70: 6573 7420 6170 7072 6f78 696d 6174 696f  est approximatio
-00000d80: 6e20 746f 2066 756c 6c20 636f 7272 6563  n to full correc
-00000d90: 7420 746f 6e65 2073 616e 6468 6920 6f66  t tone sandhi of
-00000da0: 2054 6169 7761 6e65 7365 2c20 7769 7468   Taiwanese, with
-00000db0: 2070 726f 7065 7220 7361 6e64 6869 206f   proper sandhi o
-00000dc0: 6620 7072 6f6e 6f75 6e73 2c20 7375 6666  f pronouns, suff
-00000dd0: 6978 6573 2c20 616e 6420 776f 7264 7320  ixes, and words 
-00000de0: 7769 7468 20e4 bb94 0d0a 2a20 6065 7863  with .....* `exc
-00000df0: 5f6c 6173 7460 202d 2063 6861 6e67 6573  _last` - changes
-00000e00: 2074 6f6e 6520 666f 7220 6576 6572 7920   tone for every 
-00000e10: 7379 6c6c 6162 6c65 2065 7863 6570 7420  syllable except 
-00000e20: 666f 7220 7468 6520 6c61 7374 206f 6e65  for the last one
-00000e30: 0d0a 2a20 6069 6e63 6c5f 6c61 7374 6020  ..* `incl_last` 
-00000e40: 2d20 6368 616e 6765 7320 746f 6e65 2066  - changes tone f
-00000e50: 6f72 2065 7665 7279 2073 796c 6c61 626c  or every syllabl
-00000e60: 6520 696e 636c 7564 696e 6720 7468 6520  e including the 
-00000e70: 6c61 7374 206f 6e65 0d0a 0d0a 4465 6661  last one....Defa
-00000e80: 756c 7420 7661 6c75 6520 6465 7065 6e64  ult value depend
-00000e90: 7320 6f6e 2074 6865 2063 686f 7365 6e20  s on the chosen 
-00000ea0: 6073 7973 7465 6d60 3a0d 0a0d 0a2a 2060  `system`:....* `
-00000eb0: 6175 746f 6020 2d20 666f 7220 6054 6f6e  auto` - for `Ton
-00000ec0: 6769 6f6e 6760 0d0a 2a20 606e 6f6e 6560  giong`..* `none`
-00000ed0: 202d 2066 6f72 2060 5461 696c 6f60 2c20   - for `Tailo`, 
-00000ee0: 6050 4f4a 602c 2060 5a68 7579 696e 602c  `POJ`, `Zhuyin`,
-00000ef0: 2060 544c 5041 602c 2060 5069 6e67 7969   `TLPA`, `Pingyi
-00000f00: 6d60 2c20 6049 5041 600d 0a0d 0a7c 2074  m`, `IPA`....| t
-00000f10: 6578 7420 2020 2020 2020 2020 7c20 6e6f  ext         | no
-00000f20: 6e65 2020 2020 2020 2020 2020 2020 2020  ne              
-00000f30: 2020 207c 2061 7574 6f20 2020 2020 2020     | auto       
-00000f40: 2020 2020 2020 2020 2020 7c20 6578 635f            | exc_
-00000f50: 6c61 7374 2020 2020 2020 2020 2020 2020  last            
-00000f60: 207c 2069 6e63 6c5f 6c61 7374 2020 2020   | incl_last    
-00000f70: 2020 2020 2020 2020 7c0d 0a7c 202d 2d2d          |..| ---
-00000f80: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fa0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00000fb0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
-00000fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-00000fd0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00000fe0: 2d2d 2d2d 2d20 7c0d 0a7c 20e9 8099 e698  ----- |..| .....
-00000ff0: afe5 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20  ............. | 
-00001000: 5473 6520 73c4 ab20 54c3 a269 2d75 c3a2  Tse s.. T..i-u..
-00001010: 6e20 67c3 ad6e 2dc3 a120 7c20 5473 6520  n g..n-.. | Tse 
-00001020: 73c3 ac20 54c4 8169 2d75 c481 6e20 6769  s.. T..i-u..n gi
-00001030: 6e2d c3a1 207c 2054 73c4 9320 73c3 ac20  n-.. | Ts.. s.. 
-00001040: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
-00001050: 207c 2054 73c4 9320 73c3 ac20 54c4 8169   | Ts.. s.. T..i
-00001060: 2d75 c481 6e20 6769 6e2d 6120 7c0d 0a0d  -u..n gin-a |...
-00001070: 0a53 616e 6468 6920 7275 6c65 7320 616c  .Sandhi rules al
-00001080: 736f 2063 6861 6e67 6520 6465 7065 6e64  so change depend
-00001090: 696e 6720 6f6e 2074 6865 2064 6961 6c65  ing on the diale
-000010a0: 6374 2063 686f 7365 6e2e 0d0a 0d0a 7c20  ct chosen.....| 
-000010b0: 7465 7874 207c 206e 6f20 7361 6e64 6869  text | no sandhi
-000010c0: 207c 2073 6f75 7468 2020 207c 206e 6f72   | south   | nor
-000010d0: 7468 2020 207c 0d0a 7c20 2d2d 2d2d 207c  th   |..| ---- |
-000010e0: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
-000010f0: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
-00001100: 0d0a 7c20 e58f b0e7 81a3 207c 2054 c3a2  ..| ...... | T..
-00001110: 692d 75c3 a26e 2020 207c 2054 c481 692d  i-u..n   | T..i-
-00001120: 75c3 a26e 207c 2054 c3a0 692d 75c3 a26e  u..n | T..i-u..n
-00001130: 207c 0d0a 0d0a 2323 2323 2050 756e 6374   |....#### Punct
-00001140: 7561 7469 6f6e 0d0a 0d0a 6070 756e 6374  uation....`punct
-00001150: 7561 7469 6f6e 6020 5374 7269 6e67 0d0a  uation` String..
-00001160: 0d0a 2a20 6066 6f72 6d61 7460 2028 6465  ..* `format` (de
-00001170: 6661 756c 7429 202d 2063 6f6e 7665 7274  fault) - convert
-00001180: 7320 4368 696e 6573 652d 7374 796c 6520  s Chinese-style 
-00001190: 7075 6e63 7475 6174 696f 6e20 746f 204c  punctuation to L
-000011a0: 6174 696e 2d73 7479 6c65 2070 756e 6374  atin-style punct
-000011b0: 7561 7469 6f6e 2061 6e64 2063 6170 6974  uation and capit
-000011c0: 616c 6973 6573 2077 6f72 6473 2061 7420  alises words at 
-000011d0: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
-000011e0: 2065 6163 6820 7365 6e74 656e 6365 2e0d   each sentence..
-000011f0: 0a2a 2060 6e6f 6e65 6020 2d20 7072 6573  .* `none` - pres
-00001200: 6572 7665 7320 4368 696e 6573 652d 7374  erves Chinese-st
-00001210: 796c 6520 7075 6e63 7475 6174 696f 6e20  yle punctuation 
-00001220: 616e 6420 646f 6573 6e27 7420 6361 7069  and doesn't capi
-00001230: 7461 6c69 7365 2077 6f72 6473 2061 7420  talise words at 
-00001240: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
-00001250: 206e 6577 2073 656e 7465 6e63 6573 2e0d   new sentences..
-00001260: 0a0d 0a7c 2074 6578 7420 2020 2020 2020  ...| text       
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 7c20 666f 726d 6174 2020 2020      | format    
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 7c20 6e6f 6e65 2020          | none  
-00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001380: 0d0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..| ------------
-00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013d0: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
-000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001430: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-00001440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  ------------- |.
-000014a0: 0a7c 20e9 8099 e698 afe8 87ba e58d 97ef  .| .............
-000014b0: bc8c e7b0 a1e7 a8b1 e380 8ce5 8d97 e380  ................
-000014c0: 8def bc88 e799 bde8 a9b1 e5ad 97ef bc9a  ................
-000014d0: 54c3 a269 2d6c c3a2 6def bc9b e6b3 a8e9  T..i-l..m.......
-000014e0: 9fb3 e7ac a6e8 999f efbc 9ae3 848a e384  ................
-000014f0: 9ecb 8a20 e384 8be3 84a2 cb8a efbc 8ce5  ... ............
-00001500: 9c8b e8aa 9eef bc9a 54c3 a169 6ec3 a16e  ........T..in..n
-00001510: efbc 89e3 8082 207c 2054 7365 2073 c4ab  ...... | Tse s..
-00001520: 2054 c3a2 692d 6cc3 a26d 2c20 6bc3 a16e   T..i-l..m, k..n
-00001530: 2d74 7368 696e 6720 226c c3a2 6d22 2028  -tshing "l..m" (
-00001540: 5065 cc8d 682d 75c4 932d 6ac4 ab3a 2054  Pe..h-u..-j..: T
-00001550: c3a2 692d 6cc3 a26d 3b20 7473 c3b9 2d69  ..i-l..m; ts..-i
-00001560: 6d20 68c3 bb2d 68c5 8d3a 20e3 848a e384  m h..-h..: .....
-00001570: 9ecb 8a20 e384 8be3 84a2 cb8a 2c20 6b6f  ... ........, ko
-00001580: 6b2d 67c3 ad3a 2054 c3a1 696e c3a1 6e29  k-g..: T..in..n)
-00001590: 2e20 7c20 7473 6520 73c4 ab20 54c3 a269  . | tse s.. T..i
-000015a0: 2d6c c3a2 6def bc8c 6bc3 a16e 2d74 7368  -l..m...k..n-tsh
-000015b0: 696e 67e3 808c 6cc3 a26d e380 8def bc88  ing...l..m......
-000015c0: 5065 cc8d 682d 75c4 932d 6ac4 abef bc9a  Pe..h-u..-j.....
-000015d0: 54c3 a269 2d6c c3a2 6def bc9b 7473 c3b9  T..i-l..m...ts..
-000015e0: 2d69 6d20 68c3 bb2d 68c5 8def bc9a e384  -im h..-h.......
-000015f0: 8ae3 849e cb8a 20e3 848b e384 a2cb 8aef  ...... .........
-00001600: bc8c 6b6f 6b2d 67c3 adef bc9a 54c3 a169  ..kok-g.....T..i
-00001610: 6ec3 a16e efbc 89e3 8082 207c 0d0a 0d0a  n..n...... |....
-00001620: 2323 2323 2043 6f6e 7665 7274 206e 6f6e  #### Convert non
-00001630: 2d43 4a4b 0d0a 0d0a 6063 6f6e 7665 7274  -CJK....`convert
-00001640: 5f6e 6f6e 5f63 6a6b 6020 426f 6f6c 6561  _non_cjk` Boolea
-00001650: 6e20 2d20 6465 6669 6e65 7320 7768 6574  n - defines whet
-00001660: 6865 7220 6f72 206e 6f74 2074 6f20 636f  her or not to co
-00001670: 6e76 6572 7420 6e6f 6e2d 4368 696e 6573  nvert non-Chines
-00001680: 6520 776f 7264 732e 2043 616e 2062 6520  e words. Can be 
-00001690: 7573 6564 2074 6f20 636f 6e76 6572 7420  used to convert 
-000016a0: 5461 696c 6f20 746f 2061 6e6f 7468 6572  Tailo to another
-000016b0: 2072 6f6d 616e 6973 6174 696f 6e20 7379   romanisation sy
-000016c0: 7374 656d 2e0d 0a0d 0a2a 2060 5472 7565  stem.....* `True
-000016d0: 6020 2d20 636f 6e76 6572 7420 6e6f 6e2d  ` - convert non-
-000016e0: 4368 696e 6573 6520 6368 6172 6163 7465  Chinese characte
-000016f0: 7220 776f 7264 730d 0a2a 2060 4661 6c73  r words..* `Fals
-00001700: 6560 2028 6465 6661 756c 7429 202d 2063  e` (default) - c
-00001710: 6f6e 7665 7274 206f 6e6c 7920 4368 696e  onvert only Chin
-00001720: 6573 6520 6368 6172 6163 7465 7220 776f  ese character wo
-00001730: 7264 730d 0a0d 0a7c 2074 6578 7420 2020  rds....| text   
-00001740: 2020 207c 2046 616c 7365 2020 2020 2020     | False      
-00001750: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-00001760: 7275 6520 2020 2020 2020 2020 2020 2020  rue             
-00001770: 2020 2020 2020 207c 0d0a 7c20 2d2d 2d2d         |..| ----
-00001780: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
-000017a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
-000017b0: 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6  --------- |..| .
-000017c0: 8891 e9a3 9f70 68c3 a16e 6720 7c20 e386  .....ph..ng | ..
-000017d0: a3e3 84a8 e384 9acb 8b20 e384 90e3 84a7  ......... ......
-000017e0: e384 9ae3 86b7 cb99 2070 68c3 a16e 6720  ........ ph..ng 
-000017f0: 7c20 e386 a3e3 84a8 e384 9acb 8b20 e384  | ........... ..
-00001800: 90e3 84a7 e384 9ae3 86b7 cb99 20e3 8486  ............ ...
-00001810: e384 a4cb 8b20 7c0d 0a0d 0a23 2323 2054  ..... |....### T
-00001820: 6f6b 656e 6973 6572 0d0a 0d0a 6054 6f6b  okeniser....`Tok
-00001830: 656e 6973 6572 6020 636c 6173 7320 7065  eniser` class pe
-00001840: 7266 6f72 6d73 205b 4e4c 544b 2077 6f72  rforms [NLTK wor
-00001850: 6470 756e 6374 5f74 6f6b 656e 697a 655d  dpunct_tokenize]
-00001860: 5b6e 6c74 6b2d 746f 6b65 6e69 7a65 5d2d  [nltk-tokenize]-
-00001870: 6c69 6b65 2074 6f6b 656e 6973 6174 696f  like tokenisatio
-00001880: 6e20 6f66 2061 2054 6169 7761 6e65 7365  n of a Taiwanese
-00001890: 2048 6f6b 6b69 656e 2073 656e 7465 6e63   Hokkien sentenc
-000018a0: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
-000018b0: 0a23 2063 6f6e 7374 7275 6374 6f72 0d0a  .# constructor..
-000018c0: 7420 3d20 546f 6b65 6e69 7365 7228 290d  t = Tokeniser().
-000018d0: 0a0d 0a23 2074 6f6b 656e 6973 6520 5461  ...# tokenise Ta
-000018e0: 6977 616e 6573 6520 486f 6b6b 6965 6e20  iwanese Hokkien 
-000018f0: 7365 6e74 656e 6365 0d0a 742e 746f 6b65  sentence..t.toke
-00001900: 6e69 7365 2869 6e70 7574 290d 0a60 6060  nise(input)..```
-00001910: 0d0a 0d0a 2323 2320 4f74 6865 7220 4675  ....### Other Fu
-00001920: 6e63 7469 6f6e 730d 0a0d 0a60 6060 7079  nctions....```py
-00001930: 7468 6f6e 0d0a 2320 436f 6e76 6572 7420  thon..# Convert 
-00001940: 746f 2054 7261 6469 7469 6f6e 616c 0d0a  to Traditional..
-00001950: 746f 5f74 7261 6469 7469 6f6e 616c 2869  to_traditional(i
-00001960: 6e70 7574 290d 0a0d 0a23 2043 6f6e 7665  nput)....# Conve
-00001970: 7274 2074 6f20 5369 6d70 6c69 6669 6564  rt to Simplified
-00001980: 0d0a 746f 5f73 696d 706c 6966 6965 6428  ..to_simplified(
-00001990: 696e 7075 7429 0d0a 0d0a 2320 4368 6563  input)....# Chec
-000019a0: 6b20 6966 2074 6865 2073 7472 696e 6720  k if the string 
-000019b0: 6973 2066 756c 6c79 2063 6f6d 706f 7365  is fully compose
-000019c0: 6420 6f66 2043 6869 6e65 7365 2063 6861  d of Chinese cha
-000019d0: 7261 6374 6572 730d 0a69 735f 636a 6b28  racters..is_cjk(
-000019e0: 696e 7075 7429 0d0a 6060 600d 0a0d 0a0d  input)..```.....
-000019f0: 0a0d 0a3c 212d 2d20 4558 414d 504c 4520  ...<!-- EXAMPLE 
-00001a00: 2d2d 3e0d 0a23 2320 4578 616d 706c 650d  -->..## Example.
-00001a10: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 2320  ...```python..# 
-00001a20: 436f 6e76 6572 7465 720d 0a66 726f 6d20  Converter..from 
-00001a30: 7461 6962 756e 2069 6d70 6f72 7420 436f  taibun import Co
-00001a40: 6e76 6572 7465 720d 0a0d 0a23 2320 5379  nverter....## Sy
-00001a50: 7374 656d 0d0a 6320 3d20 436f 6e76 6572  stem..c = Conver
-00001a60: 7465 7228 2920 2320 5461 696c 6f20 7379  ter() # Tailo sy
-00001a70: 7374 656d 2064 6566 6175 6c74 0d0a 632e  stem default..c.
-00001a80: 6765 7428 27e5 8588 e794 9fe8 ac9b efbc  get('...........
-00001a90: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
-00001aa0: e380 8227 290d 0a3e 3e20 5369 616e 2d73  ...')..>> Sian-s
-00001ab0: 696e 6e20 6bc3 b36e 672c 2068 61cc 8d6b  inn k..ng, ha..k
-00001ac0: 2d73 696e 6720 7469 c481 6d2d 7469 c481  -sing ti..m-ti..
-00001ad0: 6d20 7468 6961 6e6e 2e0d 0a0d 0a63 203d  m thiann.....c =
-00001ae0: 2043 6f6e 7665 7274 6572 2873 7973 7465   Converter(syste
-00001af0: 6d3d 275a 6875 7969 6e27 290d 0a63 2e67  m='Zhuyin')..c.g
-00001b00: 6574 2827 e585 88e7 949f e8ac 9bef bc8c  et('............
-00001b10: e5ad b8e7 949f e681 ace6 81ac e881 bde3  ................
-00001b20: 8082 2729 0d0a 3e3e 20e3 8492 e384 a7e3  ..')..>> .......
-00001b30: 84a2 20e3 8492 e386 aa20 e384 8de3 86b2  .. ...... ......
-00001b40: cb8b 2c20 e384 8fe3 849a e386 b6cb 9920  .., ........... 
-00001b50: e384 92e3 84a7 e384 a520 e384 89e3 84a7  ......... ......
-00001b60: e386 b0cb ab20 e384 89e3 84a7 e386 b0cb  ..... ..........
-00001b70: ab20 e384 8ae3 84a7 e386 a92e 0d0a 0d0a  . ..............
-00001b80: 2323 2044 6961 6c65 6374 0d0a 6320 3d20  ## Dialect..c = 
-00001b90: 436f 6e76 6572 7465 7228 2920 2320 736f  Converter() # so
-00001ba0: 7574 6820 6469 616c 6563 7420 6465 6661  uth dialect defa
-00001bb0: 756c 740d 0a63 2e67 6574 2822 e688 91e6  ult..c.get("....
-00001bc0: acb2 e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229  ..............")
-00001bd0: 0d0a 3e3e 2047 75c3 a120 6265 6820 c4ab  ..>> Gu.. beh ..
-00001be0: 6e67 2074 c4ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
-00001bf0: c3ae 0d0a 0d0a 6320 3d20 436f 6e76 6572  ......c = Conver
-00001c00: 7465 7228 6469 616c 6563 743d 276e 6f72  ter(dialect='nor
-00001c10: 7468 2729 0d0a 632e 6765 7428 22e6 8891  th')..c.get("...
-00001c20: e6ac b2e7 94a8 e7ae b8e9 a39f e9ad 9a22  ..............."
-00001c30: 290d 0a3e 3e20 4775 c3a1 2062 7565 6820  )..>> Gu.. bueh 
-00001c40: c4ab 6e67 2074 c5ab 2074 7369 61cc 8d68  ..ng t.. tsia..h
-00001c50: 2068 c3bb 0d0a 0d0a 2323 2046 6f72 6d61   h......## Forma
-00001c60: 740d 0a63 203d 2043 6f6e 7665 7274 6572  t..c = Converter
-00001c70: 2829 2023 2066 6f72 2054 6169 6c6f 2c20  () # for Tailo, 
-00001c80: 6d61 726b 2062 7920 6465 6661 756c 740d  mark by default.
-00001c90: 0a63 2e67 6574 2822 e794 9fe6 97a5 e5bf  .c.get("........
-00001ca0: abe6 a882 2229 0d0a 3e3e 2053 656e 6e2d  ....")..>> Senn-
-00001cb0: 6a69 cc8d 7420 6b68 75c3 a069 2d6c 6fcc  ji..t khu..i-lo.
-00001cc0: 8d6b 0d0a 0d0a 6320 3d20 436f 6e76 6572  .k....c = Conver
-00001cd0: 7465 7228 666f 726d 6174 3d27 6e75 6d62  ter(format='numb
-00001ce0: 6572 2729 0d0a 632e 6765 7428 22e7 949f  er')..c.get("...
-00001cf0: e697 a5e5 bfab e6a8 8222 290d 0a3e 3e20  .........")..>> 
-00001d00: 5365 6e6e 312d 6a69 7438 206b 6875 6169  Senn1-jit8 khuai
-00001d10: 332d 6c6f 6b38 0d0a 0d0a 6320 3d20 436f  3-lok8....c = Co
-00001d20: 6e76 6572 7465 7228 666f 726d 6174 3d27  nverter(format='
-00001d30: 7374 7269 7027 290d 0a63 2e67 6574 2822  strip')..c.get("
-00001d40: e794 9fe6 97a5 e5bf abe6 a882 2229 0d0a  ............")..
-00001d50: 3e3e 2053 656e 6e2d 6a69 7420 6b68 7561  >> Senn-jit khua
-00001d60: 692d 6c6f 6b0d 0a0d 0a23 2320 4465 6c69  i-lok....## Deli
-00001d70: 6d69 7465 720d 0a63 203d 2043 6f6e 7665  miter..c = Conve
-00001d80: 7274 6572 2864 656c 696d 6974 6572 3d27  rter(delimiter='
-00001d90: 2729 0d0a 632e 6765 7428 22e5 8588 e794  ')..c.get(".....
-00001da0: 9fe8 ac9b efbc 8ce5 adb8 e794 9fe6 81ac  ................
-00001db0: e681 ace8 81bd e380 8222 290d 0a3e 3e20  .........")..>> 
-00001dc0: 5369 616e 7369 6e6e 206b c3b3 6e67 2c20  Siansinn k..ng, 
-00001dd0: 6861 cc8d 6b73 696e 6720 7469 c481 6d74  ha..ksing ti..mt
-00001de0: 69c4 816d 2074 6869 616e 6e2e 0d0a 0d0a  i..m thiann.....
-00001df0: 6320 3d20 436f 6e76 6572 7465 7228 7379  c = Converter(sy
-00001e00: 7374 656d 3d27 5069 6e67 7969 6d27 2c20  stem='Pingyim', 
-00001e10: 6465 6c69 6d69 7465 723d 272d 2729 0d0a  delimiter='-')..
-00001e20: 632e 6765 7428 22e5 8588 e794 9fe8 ac9b  c.get(".........
-00001e30: efbc 8ce5 adb8 e794 9fe6 81ac e681 ace8  ................
-00001e40: 81bd e380 8222 290d 0a3e 3e20 5369 c481  .....")..>> Si..
-00001e50: 6e2d 736e c4ab 2067 c792 6e67 2c20 68c3  n-sn.. g..ng, h.
-00001e60: a167 2d73 c4ab 6e67 2064 69c3 a26d 2d64  .g-s..ng di..m-d
-00001e70: 69c3 a26d 2074 696e c481 2e0d 0a0d 0a23  i..m tin.......#
-00001e80: 2320 5361 6e64 6869 0d0a 6320 3d20 436f  # Sandhi..c = Co
-00001e90: 6e76 6572 7465 7228 2920 2320 666f 7220  nverter() # for 
-00001ea0: 5461 696c 6f2c 2073 616e 6468 6920 6e6f  Tailo, sandhi no
-00001eb0: 6e65 2062 7920 6465 6661 756c 740d 0a63  ne by default..c
-00001ec0: 2e67 6574 2822 e980 99e6 98af e58f b0e7  .get("..........
-00001ed0: 81a3 e59b a1e4 bb94 2229 0d0a 3e3e 2054  ........")..>> T
-00001ee0: 7365 2073 c4ab 2054 c3a2 692d 75c3 a26e  se s.. T..i-u..n
-00001ef0: 2067 c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20   g..n-......c = 
-00001f00: 436f 6e76 6572 7465 7228 7361 6e64 6869  Converter(sandhi
-00001f10: 3d27 6175 746f 2729 0d0a 632e 6765 7428  ='auto')..c.get(
-00001f20: 22e9 8099 e698 afe5 8fb0 e781 a3e5 9ba1  "...............
-00001f30: e4bb 9422 290d 0a3e 3e20 5473 6520 73c3  ...")..>> Tse s.
-00001f40: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
-00001f50: c3a1 0d0a 0d0a 6320 3d20 436f 6e76 6572  ......c = Conver
-00001f60: 7465 7228 7361 6e64 6869 3d27 6578 635f  ter(sandhi='exc_
-00001f70: 6c61 7374 2729 0d0a 632e 6765 7428 22e9  last')..c.get(".
-00001f80: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
-00001f90: 9422 290d 0a3e 3e20 5473 c493 2073 c3ac  .")..>> Ts.. s..
-00001fa0: 2054 c481 692d 75c4 816e 2067 696e 2dc3   T..i-u..n gin-.
-00001fb0: a10d 0a0d 0a63 203d 2043 6f6e 7665 7274  .....c = Convert
-00001fc0: 6572 2873 616e 6468 693d 2769 6e63 6c5f  er(sandhi='incl_
-00001fd0: 6c61 7374 2729 0d0a 632e 6765 7428 22e9  last')..c.get(".
-00001fe0: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
-00001ff0: 9422 290d 0a3e 3e20 5473 c493 2073 c3ac  .")..>> Ts.. s..
-00002000: 2054 c481 692d 75c4 816e 2067 696e 2d61   T..i-u..n gin-a
-00002010: 0d0a 0d0a 2323 2050 756e 6374 7561 7469  ....## Punctuati
-00002020: 6f6e 0d0a 6320 3d20 436f 6e76 6572 7465  on..c = Converte
-00002030: 7228 2920 2320 666f 726d 6174 2070 756e  r() # format pun
-00002040: 6374 7561 7469 6f6e 2064 6566 6175 6c74  ctuation default
-00002050: 0d0a 632e 6765 7428 22e5 a4aa e7a9 bae6  ..c.get(".......
-00002060: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
-00002070: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
-00002080: 2229 0d0a 3e3e 2054 68c3 a069 2d6b 686f  ")..>> Th..i-kho
-00002090: 6e67 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3  ng p..ng-i.., l.
-000020a0: ad6e 2d68 c3b3 2120 4cc3 ad6e 2074 7369  .n-h..! L..n tsi
-000020b0: 61cc 8d68 2d70 c3a1 2062 75c4 933f 0d0a  a..h-p.. bu..?..
-000020c0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-000020d0: 7075 6e63 7475 6174 696f 6e3d 276e 6f6e  punctuation='non
-000020e0: 6527 290d 0a63 2e67 6574 2822 e5a4 aae7  e')..c.get("....
-000020f0: a9ba e69c 8be5 8f8b efbc 8ce6 8181 e5a5  ................
-00002100: bdef bc81 e681 81e9 a39f e9a3 bde6 9caa  ................
-00002110: efbc 9f22 290d 0a3e 3e20 7468 c3a0 692d  ...")..>> th..i-
-00002120: 6b68 6f6e 6720 70c3 ae6e 672d 69c3 baef  khong p..ng-i...
-00002130: bc8c 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad  ..l..n-h.....l..
-00002140: 6e20 7473 6961 cc8d 682d 70c3 a120 6275  n tsia..h-p.. bu
-00002150: c493 efbc 9f0d 0a0d 0a23 2320 436f 6e76  .........## Conv
-00002160: 6572 7420 6e6f 6e2d 434a 4b0d 0a63 203d  ert non-CJK..c =
-00002170: 2043 6f6e 7665 7274 2873 7973 7465 6d3d   Convert(system=
-00002180: 275a 6875 7969 6e27 2920 2320 4661 6c73  'Zhuyin') # Fals
-00002190: 6520 636f 6e76 6572 745f 6e6f 6e5f 636a  e convert_non_cj
-000021a0: 6b20 6465 6661 756c 740d 0a63 2e67 6574  k default..c.get
-000021b0: 2822 e688 91e9 a39f 7068 c3a1 6e67 2229  ("......ph..ng")
-000021c0: 0d0a 3e3e 20e3 86a3 e384 a8e3 849a cb8b  ..>> ...........
-000021d0: 20e3 8490 e384 a7e3 849a e386 b7cb 9920   .............. 
-000021e0: 7068 c3a1 6e67 0d0a 0d0a 6320 3d20 436f  ph..ng....c = Co
-000021f0: 6e76 6572 7428 7379 7374 656d 3d27 5a68  nvert(system='Zh
-00002200: 7579 696e 272c 2063 6f6e 7665 7274 5f6e  uyin', convert_n
-00002210: 6f6e 5f63 6a6b 3d54 7275 6529 0d0a 632e  on_cjk=True)..c.
-00002220: 6765 7428 22e6 8891 e9a3 9f70 68c3 a16e  get("......ph..n
-00002230: 6722 290d 0a3e 3e20 e386 a3e3 84a8 e384  g")..>> ........
-00002240: 9acb 8b20 e384 90e3 84a7 e384 9ae3 86b7  ... ............
-00002250: cb99 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d  .. .............
-00002260: 0a23 2054 6f6b 656e 6973 6572 0d0a 6672  .# Tokeniser..fr
-00002270: 6f6d 2074 6169 6275 6e20 696d 706f 7274  om taibun import
-00002280: 2054 6f6b 656e 6973 6572 0d0a 0d0a 7420   Tokeniser....t 
-00002290: 3d20 546f 6b65 6e69 7365 7228 290d 0a74  = Tokeniser()..t
-000022a0: 2e74 6f6b 656e 6973 6528 22e5 a4aa e7a9  .tokenise(".....
-000022b0: bae6 9c8b e58f 8bef bc8c e681 81e5 a5bd  ................
-000022c0: efbc 81e6 8181 e9a3 9fe9 a3bd e69c aaef  ................
-000022d0: bc9f 2229 0d0a 3e3e 205b 27e5 a4aa e7a9  ..")..>> ['.....
-000022e0: ba27 2c20 27e6 9c8b e58f 8b27 2c20 27ef  .', '......', '.
-000022f0: bc8c 272c 2027 e681 81e5 a5bd 272c 2027  ..', '......', '
-00002300: efbc 8127 2c20 27e6 8181 272c 2027 e9a3  ...', '...', '..
-00002310: 9fe9 a3bd 272c 2027 e69c aa27 2c20 27ef  ....', '...', '.
-00002320: bc9f 275d 0d0a 0d0a 0d0a 2320 4f74 6865  ..']......# Othe
-00002330: 7220 4675 6e63 7469 6f6e 730d 0a66 726f  r Functions..fro
-00002340: 6d20 7461 6962 756e 2069 6d70 6f72 7420  m taibun import 
-00002350: 746f 5f74 7261 6469 7469 6f6e 616c 2c20  to_traditional, 
-00002360: 746f 5f73 696d 706c 6966 6965 642c 2069  to_simplified, i
-00002370: 735f 636a 6b0d 0a0d 0a74 6f5f 7472 6164  s_cjk....to_trad
-00002380: 6974 696f 6e61 6c28 22e6 8891 e590 ace6  itional(".......
-00002390: 97a0 e58f b0e6 b9be e8af 9d22 290d 0a3e  ...........")..>
-000023a0: 3e20 e688 91e8 81bd e784 a1e5 8fb0 e781  > ..............
-000023b0: a3e8 a9b1 0d0a 0d0a 746f 5f73 696d 706c  ........to_simpl
-000023c0: 6966 6965 6428 22e6 8891 e881 bde7 84a1  ified(".........
-000023d0: e887 bae7 81a3 e8a9 b122 290d 0a3e 3e20  .........")..>> 
-000023e0: e688 91e5 90ac e697 a0e5 8fb0 e6b9 bee8  ................
-000023f0: af9d 0d0a 0d0a 6973 5f63 6a6b 2827 e688  ......is_cjk('..
-00002400: 91e9 a39f e9ba ad27 290d 0a3e 3e20 5472  .......')..>> Tr
-00002410: 7565 0d0a 0d0a 6973 5f63 6a6b 2827 e688  ue....is_cjk('..
-00002420: 91e9 a39f 7068 c3a1 6e67 2729 0d0a 3e3e  ....ph..ng')..>>
-00002430: 2046 616c 7365 0d0a 6060 600d 0a0d 0a0d   False..```.....
-00002440: 0a0d 0a3c 212d 2d20 4441 5441 202d 2d3e  ...<!-- DATA -->
-00002450: 0d0a 2323 2044 6174 610d 0a0d 0a2d 205b  ..## Data....- [
-00002460: 5461 6977 616e 6573 652d 4368 696e 6573  Taiwanese-Chines
-00002470: 6520 4f6e 6c69 6e65 2044 6963 7469 6f6e  e Online Diction
-00002480: 6172 795d 5b6f 6e6c 696e 652d 6469 6374  ary][online-dict
-00002490: 696f 6e61 7279 5d20 2876 6961 205b 4368  ionary] (via [Ch
-000024a0: 686f 6554 6169 6769 5d5b 6461 7461 2d76  hoeTaigi][data-v
-000024b0: 6961 5d29 0d0a 2d20 5b69 5461 6967 6920  ia])..- [iTaigi 
-000024c0: 4368 696e 6573 652d 5461 6977 616e 6573  Chinese-Taiwanes
-000024d0: 6520 436f 6d70 6172 6973 6f6e 2044 6963  e Comparison Dic
-000024e0: 7469 6f6e 6172 795d 5b69 7461 6967 692d  tionary][itaigi-
-000024f0: 6469 6374 696f 6e61 7279 5d20 2876 6961  dictionary] (via
-00002500: 205b 4368 686f 6554 6169 6769 5d5b 6461   [ChhoeTaigi][da
-00002510: 7461 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a  ta-via])........
-00002520: 3c21 2d2d 2041 434b 4e4f 574c 4544 4745  <!-- ACKNOWLEDGE
-00002530: 4d45 4e54 5320 2d2d 3e0d 0a23 2320 4163  MENTS -->..## Ac
-00002540: 6b6e 6f77 6c65 6467 656d 656e 7473 0d0a  knowledgements..
-00002550: 0d0a 2d20 5361 6d75 656c 204a 656e 2028  ..- Samuel Jen (
-00002560: 5b47 6974 6875 625d 5b73 616d 7565 6c2d  [Github][samuel-
-00002570: 6769 7468 7562 5d20 c2b7 205b 4c69 6e6b  github] .. [Link
-00002580: 6564 496e 5d5b 7361 6d75 656c 2d6c 696e  edIn][samuel-lin
-00002590: 6b65 6469 6e5d 2920 2d20 5461 6977 616e  kedin]) - Taiwan
-000025a0: 6573 6520 616e 6420 4d61 6e64 6172 696e  ese and Mandarin
-000025b0: 2074 7261 6e73 6c61 7469 6f6e 0d0a 0d0a   translation....
-000025c0: 0d0a 0d0a 3c21 2d2d 204c 4943 454e 4345  ....<!-- LICENCE
-000025d0: 202d 2d3e 0d0a 2323 204c 6963 656e 6365   -->..## Licence
-000025e0: 0d0a 0d0a 4265 6361 7573 6520 5461 6962  ....Because Taib
-000025f0: 756e 2069 7320 4d49 542d 6c69 6365 6e73  un is MIT-licens
-00002600: 6564 2c20 616e 7920 6465 7665 6c6f 7065  ed, any develope
-00002610: 7220 6361 6e20 6573 7365 6e74 6961 6c6c  r can essentiall
-00002620: 7920 646f 2077 6861 7465 7665 7220 7468  y do whatever th
-00002630: 6579 2077 616e 7420 7769 7468 2069 7420  ey want with it 
-00002640: 6173 206c 6f6e 6720 6173 2074 6865 7920  as long as they 
-00002650: 696e 636c 7564 6520 7468 6520 6f72 6967  include the orig
-00002660: 696e 616c 2063 6f70 7972 6967 6874 2061  inal copyright a
-00002670: 6e64 206c 6963 656e 6365 206e 6f74 6963  nd licence notic
-00002680: 6520 696e 2061 6e79 2063 6f70 6965 7320  e in any copies 
-00002690: 6f66 2074 6865 2073 6f75 7263 6520 636f  of the source co
-000026a0: 6465 2e20 4e6f 7465 2c20 7468 6174 2074  de. Note, that t
-000026b0: 6865 2064 6174 6120 7573 6564 2062 7920  he data used by 
-000026c0: 7468 6520 7061 636b 6167 6520 6973 206c  the package is l
-000026d0: 6963 656e 7365 6420 756e 6465 7220 6120  icensed under a 
-000026e0: 6469 6666 6572 656e 7420 636f 7079 7269  different copyri
-000026f0: 6768 742e 0d0a 0d0a 5468 6520 6461 7461  ght.....The data
-00002700: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00002710: 6572 205b 4343 2042 592d 5341 2034 2e30  er [CC BY-SA 4.0
-00002720: 5d5b 6461 7461 2d63 635d 0d0a 0d0a 0d0a  ][data-cc]......
-00002730: 0d0a 3c21 2d2d 204d 4152 4b44 4f57 4e20  ..<!-- MARKDOWN 
-00002740: 4c49 4e4b 5320 2d2d 3e0d 0a5b 7465 7374  LINKS -->..[test
-00002750: 735d 3a20 6874 7470 733a 2f2f 6769 7468  s]: https://gith
-00002760: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
-00002770: 2f74 6169 6275 6e2f 6163 7469 6f6e 730d  /taibun/actions.
-00002780: 0a5b 7465 7374 732d 6261 6467 655d 3a20  .[tests-badge]: 
-00002790: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000027a0: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
-000027b0: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
-000027c0: 7461 7475 732f 616e 6472 6569 6861 722f  tatus/andreihar/
-000027d0: 7461 6962 756e 2f63 692e 7961 6d6c 3f73  taibun/ci.yaml?s
-000027e0: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-000027f0: 6765 266c 6f67 6f3d 6769 7468 7562 0d0a  ge&logo=github..
-00002800: 5b63 6f6e 7472 6962 7574 6f72 732d 6261  [contributors-ba
-00002810: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
-00002820: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00002830: 6875 622f 636f 6e74 7269 6275 746f 7273  hub/contributors
-00002840: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
-00002850: 6e3f 7374 796c 653d 666f 722d 7468 652d  n?style=for-the-
-00002860: 6261 6467 650d 0a5b 636f 6e74 7269 6275  badge..[contribu
-00002870: 746f 7273 5d3a 2023 7573 6167 650d 0a5b  tors]: #usage..[
-00002880: 7265 6c65 6173 652d 6261 6467 655d 3a20  release-badge]: 
-00002890: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000028a0: 6c64 732e 696f 2f67 6974 6875 622f 762f  lds.io/github/v/
-000028b0: 7265 6c65 6173 652f 616e 6472 6569 6861  release/andreiha
-000028c0: 722f 7461 6962 756e 3f63 6f6c 6f72 3d33  r/taibun?color=3
-000028d0: 3836 3138 6326 7374 796c 653d 666f 722d  8618c&style=for-
-000028e0: 7468 652d 6261 6467 650d 0a5b 7265 6c65  the-badge..[rele
-000028f0: 6173 655d 3a20 6874 7470 733a 2f2f 6769  ase]: https://gi
-00002900: 7468 7562 2e63 6f6d 2f61 6e64 7265 6968  thub.com/andreih
-00002910: 6172 2f74 6169 6275 6e2f 7265 6c65 6173  ar/taibun/releas
-00002920: 6573 0d0a 5b6c 6963 656e 6365 2d62 6164  es..[licence-bad
-00002930: 6765 5d3a 2068 7474 7073 3a2f 2f69 6d67  ge]: https://img
-00002940: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00002950: 7562 2f6c 6963 656e 7365 2f61 6e64 7265  ub/license/andre
-00002960: 6968 6172 2f74 6169 6275 6e3f 636f 6c6f  ihar/taibun?colo
-00002970: 723d 3030 3030 3030 2673 7479 6c65 3d66  r=000000&style=f
-00002980: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b6c  or-the-badge..[l
-00002990: 6963 656e 6365 5d3a 204c 4943 454e 5345  icence]: LICENSE
-000029a0: 0d0a 5b6c 696e 6b65 6469 6e2d 6261 6467  ..[linkedin-badg
-000029b0: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
-000029c0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-000029d0: 2f4c 696e 6b65 6449 6e2d 3030 3737 4235  /LinkedIn-0077B5
-000029e0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
-000029f0: 6164 6765 266c 6f67 6f3d 6c69 6e6b 6564  adge&logo=linked
-00002a00: 696e 266c 6f67 6f43 6f6c 6f72 3d77 6869  in&logoColor=whi
-00002a10: 7465 0d0a 5b6c 696e 6b65 6469 6e5d 3a20  te..[linkedin]: 
-00002a20: 6874 7470 733a 2f2f 7777 772e 6c69 6e6b  https://www.link
-00002a30: 6564 696e 2e63 6f6d 2f69 6e2f 616e 6472  edin.com/in/andr
-00002a40: 6569 2d68 6172 6261 6368 6f76 2f0d 0a0d  ei-harbachov/...
-00002a50: 0a5b 7079 7069 5d3a 2068 7474 7073 3a2f  .[pypi]: https:/
-00002a60: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00002a70: 742f 7461 6962 756e 0d0a 5b62 7567 5d3a  t/taibun..[bug]:
-00002a80: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00002a90: 636f 6d2f 616e 6472 6569 6861 722f 7461  com/andreihar/ta
-00002aa0: 6962 756e 2f69 7373 7565 730d 0a5b 6f6e  ibun/issues..[on
-00002ab0: 6c69 6e65 2d64 6963 7469 6f6e 6172 795d  line-dictionary]
-00002ac0: 3a20 6874 7470 3a2f 2f69 7031 3934 3039  : http://ip19409
-00002ad0: 372e 6e74 6375 2e65 6475 2e74 772f 756e  7.ntcu.edu.tw/un
-00002ae0: 6769 616e 2f73 6f61 6e6e 7465 6e67 2f63  gian/soannteng/c
-00002af0: 6869 6c2f 5461 6968 6f61 2e61 7370 0d0a  hil/Taihoa.asp..
-00002b00: 5b69 7461 6967 692d 6469 6374 696f 6e61  [itaigi-dictiona
-00002b10: 7279 5d3a 2068 7474 7073 3a2f 2f69 7461  ry]: https://ita
-00002b20: 6967 692e 7477 2f0d 0a5b 6461 7461 2d76  igi.tw/..[data-v
-00002b30: 6961 5d3a 2068 7474 7073 3a2f 2f67 6974  ia]: https://git
-00002b40: 6875 622e 636f 6d2f 4368 686f 6554 6169  hub.com/ChhoeTai
-00002b50: 6769 2f43 6868 6f65 5461 6967 6944 6174  gi/ChhoeTaigiDat
-00002b60: 6162 6173 650d 0a5b 6461 7461 2d63 635d  abase..[data-cc]
-00002b70: 3a20 6874 7470 733a 2f2f 6372 6561 7469  : https://creati
-00002b80: 7665 636f 6d6d 6f6e 732e 6f72 672f 6c69  vecommons.org/li
-00002b90: 6365 6e73 6573 2f62 792d 7361 2f34 2e30  censes/by-sa/4.0
-00002ba0: 2f64 6565 642e 656e 0d0a 5b73 616d 7565  /deed.en..[samue
-00002bb0: 6c2d 6769 7468 7562 5d3a 2068 7474 7073  l-github]: https
-00002bc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5353  ://github.com/SS
-00002bd0: 5361 6d0d 0a5b 7361 6d75 656c 2d6c 696e  Sam..[samuel-lin
-00002be0: 6b65 6469 6e5d 3a20 6874 7470 733a 2f2f  kedin]: https://
-00002bf0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
-00002c00: 2f69 6e2f 7361 6d75 656c 2d6a 656e 2f0d  /in/samuel-jen/.
-00002c10: 0a0d 0a5b 7461 696c 6f2d 7769 6b69 5d3a  ...[tailo-wiki]:
-00002c20: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002c30: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
-00002c40: 2543 3325 4132 692d 7525 4333 2541 326e  %C3%A2i-u%C3%A2n
-00002c50: 5f4c 2543 3325 4234 2d6d 2543 3325 4131  _L%C3%B4-m%C3%A1
-00002c60: 2d6a 2543 3425 4142 5f50 6869 6e67 2d69  -j%C4%AB_Phing-i
-00002c70: 6d5f 486f 6e67 2d25 4333 2541 306e 0d0a  m_Hong-%C3%A0n..
-00002c80: 5b70 6f6a 2d77 696b 695d 3a20 6874 7470  [poj-wiki]: http
-00002c90: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00002ca0: 2e6f 7267 2f77 696b 692f 5065 2543 4325  .org/wiki/Pe%CC%
-00002cb0: 3844 682d 2543 3525 3844 652d 6a25 4334  8Dh-%C5%8De-j%C4
-00002cc0: 2541 420d 0a5b 7a68 7579 696e 2d77 696b  %AB..[zhuyin-wik
-00002cd0: 695d 3a20 6874 7470 733a 2f2f 656e 2e77  i]: https://en.w
-00002ce0: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002cf0: 692f 5461 6977 616e 6573 655f 5068 6f6e  i/Taiwanese_Phon
-00002d00: 6574 6963 5f53 796d 626f 6c73 0d0a 5b74  etic_Symbols..[t
-00002d10: 6c70 612d 7769 6b69 5d3a 2068 7474 7073  lpa-wiki]: https
-00002d20: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00002d30: 6f72 672f 7769 6b69 2f54 6169 7761 6e65  org/wiki/Taiwane
-00002d40: 7365 5f4c 616e 6775 6167 655f 5068 6f6e  se_Language_Phon
-00002d50: 6574 6963 5f41 6c70 6861 6265 740d 0a5b  etic_Alphabet..[
-00002d60: 7069 6e67 7969 6d2d 7769 6b69 5d3a 2068  pingyim-wiki]: h
-00002d70: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00002d80: 6469 612e 6f72 672f 7769 6b69 2f42 6225  dia.org/wiki/Bb%
-00002d90: 4333 2541 316e 6c25 4333 2541 316d 5f70  C3%A1nl%C3%A1m_p
-00002da0: 2543 3325 4143 6e67 7925 4334 2541 426d  %C3%ACngy%C4%ABm
-00002db0: 0d0a 5b74 6f6e 6769 6f6e 672d 7769 6b69  ..[tongiong-wiki
-00002dc0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
-00002dd0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00002de0: 2f44 6125 4334 2541 422d 6768 2543 3325  /Da%C4%AB-gh%C3%
-00002df0: 4145 5f74 2543 3525 3844 6e67 2d69 2543  AE_t%C5%8Dng-i%C
-00002e00: 3525 3844 6e67 5f70 2543 3425 4142 6e67  5%8Dng_p%C4%ABng
-00002e10: 2d69 6d0d 0a5b 6970 612d 7769 6b69 5d3a  -im..[ipa-wiki]:
-00002e20: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-00002e30: 7065 6469 612e 6f72 672f 7769 6b69 2f49  pedia.org/wiki/I
-00002e40: 6e74 6572 6e61 7469 6f6e 616c 5f50 686f  nternational_Pho
-00002e50: 6e65 7469 635f 416c 7068 6162 6574 0d0a  netic_Alphabet..
-00002e60: 5b7a 6861 6e67 7a68 6f75 2d77 696b 695d  [zhangzhou-wiki]
-00002e70: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00002e80: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002e90: 5a68 616e 677a 686f 755f 6469 616c 6563  Zhangzhou_dialec
-00002ea0: 7473 0d0a 5b71 7561 6e7a 686f 752d 7769  ts..[quanzhou-wi
-00002eb0: 6b69 5d3a 2068 7474 7073 3a2f 2f65 6e2e  ki]: https://en.
-00002ec0: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00002ed0: 6b69 2f51 7561 6e7a 686f 755f 6469 616c  ki/Quanzhou_dial
-00002ee0: 6563 7473 0d0a 5b6e 6c74 6b2d 746f 6b65  ects..[nltk-toke
-00002ef0: 6e69 7a65 5d3a 2068 7474 7073 3a2f 2f6e  nize]: https://n
-00002f00: 6c74 6b2e 6f72 672f 6170 692f 6e6c 746b  ltk.org/api/nltk
-00002f10: 2e74 6f6b 656e 697a 652e 6874 6d6c 0d0a  .tokenize.html..
-00002f20: 5b73 616e 6468 692d 7769 6b69 5d3a 2068  [sandhi-wiki]: h
-00002f30: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00002f40: 6469 612e 6f72 672f 7769 6b69 2f54 6169  dia.org/wiki/Tai
-00002f50: 7761 6e65 7365 5f48 6f6b 6b69 656e 2354  wanese_Hokkien#T
-00002f60: 6f6e 6525 3230 7361 6e64 6869 3a7e 3a74  one%20sandhi:~:t
-00002f70: 6578 743d 7468 6e67 2545 3225 3946 2541  ext=thng%E2%9F%A
-00002f80: 3925 3230 2825 3232 736f 7570 2532 3229  9%20(%22soup%22)
-00002f90: 2e2d 2c54 6f6e 6525 3230 7361 6e64 6869  .-,Tone%20sandhi
-00002fa0: 2c2d 2535 4265 6469 7425 3544            ,-%5Bedit%5D
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7861  : 2.1..Name: exa
+00000020: 6d70 6c65 3939 3034 3230 0d0a 5665 7273  mple990420..Vers
+00000030: 696f 6e3a 2031 2e31 2e31 0d0a 5375 6d6d  ion: 1.1.1..Summ
+00000040: 6172 793a 2054 6169 7761 6e65 7365 2048  ary: Taiwanese H
+00000050: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
+00000060: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
+00000070: 7365 720d 0a48 6f6d 652d 7061 6765 3a20  ser..Home-page: 
+00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000090: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+000000a0: 6275 6e0d 0a41 7574 686f 723a 2041 6e64  bun..Author: And
+000000b0: 7265 6920 4861 7262 6163 686f 760d 0a41  rei Harbachov..A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2061 6e64  uthor-email: and
+000000d0: 7265 692e 6861 7262 6163 686f 7640 676d  rei.harbachov@gm
+000000e0: 6169 6c2e 636f 6d0d 0a4c 6963 656e 7365  ail.com..License
+000000f0: 3a20 4d49 540d 0a4b 6579 776f 7264 733a  : MIT..Keywords:
+00000100: 2070 7974 686f 6e2c 7461 6977 616e 2c74   python,taiwan,t
+00000110: 6169 7761 6e65 7365 2c74 6169 6769 2c68  aiwanese,taigi,h
+00000120: 6f6b 6b69 656e 2c72 6f6d 616e 697a 6174  okkien,romanizat
+00000130: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000140: 696f 6e2c 7472 616e 736c 6974 6572 6174  ion,transliterat
+00000150: 6f72 2c74 6f6b 656e 697a 6174 696f 6e2c  or,tokenization,
+00000160: 746f 6b65 6e69 7a65 720d 0a43 6c61 7373  tokenizer..Class
+00000170: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000180: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
+00000190: 3a3a 204c 696e 6775 6973 7469 630d 0a43  :: Linguistic..C
+000001a0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+000001b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000001c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000001d0: 5374 6162 6c65 0d0a 436c 6173 7369 6669  Stable..Classifi
+000001e0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001f0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000200: 6572 730d 0a43 6c61 7373 6966 6965 723a  ers..Classifier:
+00000210: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
+00000240: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000250: 656d 203a 3a20 556e 6978 0d0a 436c 6173  em :: Unix..Clas
+00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000280: 5320 3a3a 204d 6163 4f53 2058 0d0a 436c  S :: MacOS X..Cl
+00000290: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000002a0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+000002b0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+000002c0: 7773 0d0a 5265 7175 6972 6573 2d50 7974  ws..Requires-Pyt
+000002d0: 686f 6e3a 203e 3d33 2e38 0d0a 4465 7363  hon: >=3.8..Desc
+000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000300: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
+00000310: 653a 204c 4943 454e 5345 0d0a 0d0a 3c21  e: LICENSE....<!
+00000320: 2d2d 2050 524f 4a45 4354 204c 4f47 4f20  -- PROJECT LOGO 
+00000330: 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c 6469  -->..<br />..<di
+00000340: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000350: 3e0d 0a20 203c 6120 6872 6566 3d22 6874  >..  <a href="ht
+00000360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000370: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00000380: 6e22 3e0d 0a20 2020 203c 696d 6720 7372  n">..    <img sr
+00000390: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000003a0: 622e 636f 6d2f 616e 6472 6569 6861 722f  b.com/andreihar/
+000003b0: 7461 6962 756e 2f72 6177 2f6d 6169 6e2f  taibun/raw/main/
+000003c0: 7265 6164 6d65 2f6c 6f67 6f2e 706e 6722  readme/logo.png"
+000003d0: 2061 6c74 3d22 4c6f 676f 2220 7769 6474   alt="Logo" widt
+000003e0: 683d 2239 3022 2068 6569 6768 743d 2238  h="90" height="8
+000003f0: 3022 3e0d 0a20 203c 2f61 3e0d 0a20 200d  0">..  </a>..  .
+00000400: 0a23 2054 6169 6275 6e0d 0a0d 0a0d 0a0d  .# Taibun.......
+00000410: 0a3c 212d 2d20 5052 4f4a 4543 5420 5348  .<!-- PROJECT SH
+00000420: 4945 4c44 5320 2d2d 3e0d 0a5b 215b 436f  IELDS -->..[![Co
+00000430: 6e74 7269 6275 7469 6f6e 735d 5b63 6f6e  ntributions][con
+00000440: 7472 6962 7574 696f 6e73 2d62 6164 6765  tributions-badge
+00000450: 5d5d 5b63 6f6e 7472 6962 7574 696f 6e73  ]][contributions
+00000460: 5d0d 0a5b 215b 5465 7374 735d 5b74 6573  ]..[![Tests][tes
+00000470: 7473 2d62 6164 6765 5d5d 5b74 6573 7473  ts-badge]][tests
+00000480: 5d0d 0a5b 215b 5265 6c65 6173 655d 5b72  ]..[![Release][r
+00000490: 656c 6561 7365 2d62 6164 6765 5d5d 5b72  elease-badge]][r
+000004a0: 656c 6561 7365 5d0d 0a5b 215b 4c69 6365  elease]..[![Lice
+000004b0: 6e63 655d 5b6c 6963 656e 6365 2d62 6164  nce][licence-bad
+000004c0: 6765 5d5d 5b6c 6963 656e 6365 5d0d 0a5b  ge]][licence]..[
+000004d0: 215b 4c69 6e6b 6564 496e 5d5b 6c69 6e6b  ![LinkedIn][link
+000004e0: 6564 696e 2d62 6164 6765 5d5d 5b6c 696e  edin-badge]][lin
+000004f0: 6b65 6469 6e5d 0d0a 0d0a 2a2a 5461 6977  kedin]....**Taiw
+00000500: 616e 6573 6520 486f 6b6b 6965 6e20 5472  anese Hokkien Tr
+00000510: 616e 736c 6974 6572 6174 6f72 2061 6e64  ansliterator and
+00000520: 2054 6f6b 656e 6973 6572 2a2a 0d0a 0d0a   Tokeniser**....
+00000530: 4974 2068 6173 206d 6574 686f 6473 2074  It has methods t
+00000540: 6861 7420 616c 6c6f 7720 746f 2063 7573  hat allow to cus
+00000550: 746f 6d69 7365 2074 7261 6e73 6c69 7465  tomise translite
+00000560: 7261 7469 6f6e 2061 6e64 2072 6574 7269  ration and retri
+00000570: 6576 6520 616e 7920 6e65 6365 7373 6172  eve any necessar
+00000580: 7920 696e 666f 726d 6174 696f 6e20 6162  y information ab
+00000590: 6f75 7420 5461 6977 616e 6573 6520 486f  out Taiwanese Ho
+000005a0: 6b6b 6965 6e20 7072 6f6e 756e 6369 6174  kkien pronunciat
+000005b0: 696f 6e2e 3c62 7220 2f3e 0d0a 496e 636c  ion.<br />..Incl
+000005c0: 7564 6573 2077 6f72 6420 746f 6b65 6e69  udes word tokeni
+000005d0: 7365 7220 666f 7220 5461 6977 616e 6573  ser for Taiwanes
+000005e0: 6520 486f 6b6b 6965 6e2e 0d0a 0d0a 5b52  e Hokkien.....[R
+000005f0: 6570 6f72 7420 4275 675d 5b62 7567 5d20  eport Bug][bug] 
+00000600: e280 a20d 0a5b 5079 5049 5d5b 7079 7069  .....[PyPI][pypi
+00000610: 5d0d 0a0d 0a3c 2f64 6976 3e0d 0a0d 0a0d  ]....</div>.....
+00000620: 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a 0d0a 3c21  ...---........<!
+00000630: 2d2d 2054 4142 4c45 204f 4620 434f 4e54  -- TABLE OF CONT
+00000640: 454e 5453 202d 2d3e 0d0a 3c64 6574 6169  ENTS -->..<detai
+00000650: 6c73 206f 7065 6e3e 0d0a 2020 3c73 756d  ls open>..  <sum
+00000660: 6d61 7279 3e54 6162 6c65 206f 6620 436f  mary>Table of Co
+00000670: 6e74 656e 7473 3c2f 7375 6d6d 6172 793e  ntents</summary>
+00000680: 0d0a 2020 3c6f 6c3e 0d0a 2020 2020 3c6c  ..  <ol>..    <l
+00000690: 693e 3c61 2068 7265 663d 2223 7665 7273  i><a href="#vers
+000006a0: 696f 6e73 223e 5665 7273 696f 6e73 3c2f  ions">Versions</
+000006b0: 613e 3c2f 6c69 3e0d 0a20 2020 203c 6c69  a></li>..    <li
+000006c0: 3e3c 6120 6872 6566 3d22 2369 6e73 7461  ><a href="#insta
+000006d0: 6c6c 223e 496e 7374 616c 6c3c 2f61 3e3c  ll">Install</a><
+000006e0: 2f6c 693e 0d0a 2020 2020 3c6c 693e 0d0a  /li>..    <li>..
+000006f0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+00000700: 7573 6167 6522 3e55 7361 6765 3c2f 613e  usage">Usage</a>
+00000710: 0d0a 2020 2020 2020 3c75 6c3e 0d0a 2020  ..      <ul>..  
+00000720: 2020 2020 2020 3c6c 693e 0d0a 2020 2020        <li>..    
+00000730: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+00000740: 636f 6e76 6572 7465 7222 3e43 6f6e 7665  converter">Conve
+00000750: 7274 6572 3c2f 613e 0d0a 2020 2020 2020  rter</a>..      
+00000760: 2020 2020 3c75 6c3e 0d0a 2020 2020 2020      <ul>..      
+00000770: 2020 2020 2020 3c6c 693e 3c61 2068 7265        <li><a hre
+00000780: 663d 2223 7379 7374 656d 223e 5379 7374  f="#system">Syst
+00000790: 656d 3c2f 613e 3c2f 6c69 3e0d 0a20 2020  em</a></li>..   
+000007a0: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
+000007b0: 6872 6566 3d22 2364 6961 6c65 6374 223e  href="#dialect">
+000007c0: 4469 616c 6563 743c 2f61 3e3c 2f6c 693e  Dialect</a></li>
+000007d0: 0d0a 2020 2020 2020 2020 2020 2020 3c6c  ..            <l
+000007e0: 693e 3c61 2068 7265 663d 2223 666f 726d  i><a href="#form
+000007f0: 6174 223e 466f 726d 6174 3c2f 613e 3c2f  at">Format</a></
+00000800: 6c69 3e0d 0a20 2020 2020 2020 2020 2020  li>..           
+00000810: 203c 6c69 3e3c 6120 6872 6566 3d22 2364   <li><a href="#d
+00000820: 656c 696d 6974 6572 223e 4465 6c69 6d69  elimiter">Delimi
+00000830: 7465 723c 2f61 3e3c 2f6c 693e 0d0a 2020  ter</a></li>..  
+00000840: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
+00000850: 2068 7265 663d 2223 7361 6e64 6869 223e   href="#sandhi">
+00000860: 5361 6e64 6869 3c2f 613e 3c2f 6c69 3e0d  Sandhi</a></li>.
+00000870: 0a20 2020 2020 2020 2020 2020 203c 6c69  .            <li
+00000880: 3e3c 6120 6872 6566 3d22 2370 756e 6374  ><a href="#punct
+00000890: 7561 7469 6f6e 223e 5075 6e63 7475 6174  uation">Punctuat
+000008a0: 696f 6e3c 2f61 3e3c 2f6c 693e 0d0a 2020  ion</a></li>..  
+000008b0: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
+000008c0: 2068 7265 663d 2223 636f 6e76 6572 742d   href="#convert-
+000008d0: 6e6f 6e2d 636a 6b22 3e43 6f6e 7665 7274  non-cjk">Convert
+000008e0: 206e 6f6e 2d43 4a4b 3c2f 613e 3c2f 6c69   non-CJK</a></li
+000008f0: 3e0d 0a20 2020 2020 2020 2020 203c 2f75  >..          </u
+00000900: 6c3e 0d0a 2020 2020 2020 2020 3c2f 6c69  l>..        </li
+00000910: 3e0d 0a20 2020 2020 2020 203c 6c69 3e3c  >..        <li><
+00000920: 6120 6872 6566 3d22 2374 6f6b 656e 6973  a href="#tokenis
+00000930: 6572 223e 546f 6b65 6e69 7365 723c 2f61  er">Tokeniser</a
+00000940: 3e3c 2f6c 693e 0d0a 2020 2020 2020 2020  ></li>..        
+00000950: 3c6c 693e 3c61 2068 7265 663d 2223 6f74  <li><a href="#ot
+00000960: 6865 722d 6675 6e63 7469 6f6e 7322 3e4f  her-functions">O
+00000970: 7468 6572 2046 756e 6374 696f 6e73 3c2f  ther Functions</
+00000980: 613e 3c2f 6c69 3e0d 0a20 2020 2020 203c  a></li>..      <
+00000990: 2f75 6c3e 0d0a 2020 2020 3c2f 6c69 3e0d  /ul>..    </li>.
+000009a0: 0a20 2020 203c 6c69 3e3c 6120 6872 6566  .    <li><a href
+000009b0: 3d22 2365 7861 6d70 6c65 223e 4578 616d  ="#example">Exam
+000009c0: 706c 653c 2f61 3e3c 2f6c 693e 0d0a 2020  ple</a></li>..  
+000009d0: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
+000009e0: 6461 7461 223e 4461 7461 3c2f 613e 3c2f  data">Data</a></
+000009f0: 6c69 3e0d 0a20 2020 203c 6c69 3e3c 6120  li>..    <li><a 
+00000a00: 6872 6566 3d22 2361 636b 6e6f 776c 6564  href="#acknowled
+00000a10: 6765 6d65 6e74 7322 3e41 636b 6e6f 776c  gements">Acknowl
+00000a20: 6564 6765 6d65 6e74 733c 2f61 3e3c 2f6c  edgements</a></l
+00000a30: 693e 0d0a 2020 2020 3c6c 693e 3c61 2068  i>..    <li><a h
+00000a40: 7265 663d 2223 6c69 6365 6e63 6522 3e4c  ref="#licence">L
+00000a50: 6963 656e 6365 3c2f 613e 3c2f 6c69 3e0d  icence</a></li>.
+00000a60: 0a20 203c 2f6f 6c3e 0d0a 3c2f 6465 7461  .  </ol>..</deta
+00000a70: 696c 733e 0d0a 0d0a 0d0a 0d0a 3c21 2d2d  ils>........<!--
+00000a80: 204f 5448 4552 2056 4552 5349 4f4e 5320   OTHER VERSIONS 
+00000a90: 2d2d 3e0d 0a23 2320 5665 7273 696f 6e73  -->..## Versions
+00000aa0: 0d0a 0d0a 5b21 5b4a 6176 6153 6372 6970  ....[![JavaScrip
+00000ab0: 7420 5665 7273 696f 6e5d 5b6a 732d 6261  t Version][js-ba
+00000ac0: 6467 655d 5d5b 6a73 2d6c 696e 6b5d 0d0a  dge]][js-link]..
+00000ad0: 0d0a 0d0a 0d0a 3c21 2d2d 2049 4e53 5441  ......<!-- INSTA
+00000ae0: 4c4c 202d 2d3e 0d0a 2323 2049 6e73 7461  LL -->..## Insta
+00000af0: 6c6c 0d0a 0d0a 5461 6962 756e 2063 616e  ll....Taibun can
+00000b00: 2062 6520 696e 7374 616c 6c65 6420 6672   be installed fr
+00000b10: 6f6d 205b 7079 7069 5d5b 7079 7069 5d0d  om [pypi][pypi].
+00000b20: 0a0d 0a60 6060 6261 7368 0d0a 2420 7069  ...```bash..$ pi
+00000b30: 7020 696e 7374 616c 6c20 7461 6962 756e  p install taibun
+00000b40: 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c 212d  ..```........<!-
+00000b50: 2d20 5553 4147 4520 2d2d 3e0d 0a23 2320  - USAGE -->..## 
+00000b60: 5573 6167 650d 0a0d 0a23 2323 2043 6f6e  Usage....### Con
+00000b70: 7665 7274 6572 0d0a 0d0a 6043 6f6e 7665  verter....`Conve
+00000b80: 7274 6572 6020 636c 6173 7320 7472 616e  rter` class tran
+00000b90: 736c 6974 6572 6174 6573 2074 6865 2043  sliterates the C
+00000ba0: 6869 6e65 7365 2063 6861 7261 6374 6572  hinese character
+00000bb0: 7320 746f 2074 6865 2063 686f 7365 6e20  s to the chosen 
+00000bc0: 7472 616e 736c 6974 6572 6174 696f 6e20  transliteration 
+00000bd0: 7379 7374 656d 2077 6974 6820 7061 7261  system with para
+00000be0: 6d65 7465 7273 2073 7065 6369 6669 6564  meters specified
+00000bf0: 2062 7920 7468 6520 6465 7665 6c6f 7065   by the develope
+00000c00: 722e 2057 6f72 6b73 2066 6f72 2062 6f74  r. Works for bot
+00000c10: 6820 5472 6164 6974 696f 6e61 6c20 616e  h Traditional an
+00000c20: 6420 5369 6d70 6c69 6669 6564 2063 6861  d Simplified cha
+00000c30: 7261 6374 6572 732e 0d0a 0d0a 6060 6070  racters.....```p
+00000c40: 7974 686f 6e0d 0a23 2043 6f6e 7374 7275  ython..# Constru
+00000c50: 6374 6f72 0d0a 6320 3d20 436f 6e76 6572  ctor..c = Conver
+00000c60: 7465 7228 7379 7374 656d 2c20 6469 616c  ter(system, dial
+00000c70: 6563 742c 2066 6f72 6d61 742c 2064 656c  ect, format, del
+00000c80: 696d 6974 6572 2c20 7361 6e64 6869 2c20  imiter, sandhi, 
+00000c90: 7075 6e63 7475 6174 696f 6e2c 2063 6f6e  punctuation, con
+00000ca0: 7665 7274 5f6e 6f6e 5f63 6a6b 290d 0a0d  vert_non_cjk)...
+00000cb0: 0a23 2054 7261 6e73 6c69 7465 7261 7465  .# Transliterate
+00000cc0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+00000cd0: 6572 730d 0a63 2e67 6574 2869 6e70 7574  ers..c.get(input
+00000ce0: 290d 0a60 6060 0d0a 0d0a 2323 2323 2053  )..```....#### S
+00000cf0: 7973 7465 6d0d 0a0d 0a60 7379 7374 656d  ystem....`system
+00000d00: 6020 5374 7269 6e67 202d 2073 7973 7465  ` String - syste
+00000d10: 6d20 6f66 2074 7261 6e73 6c69 7465 7261  m of translitera
+00000d20: 7469 6f6e 2e0d 0a0d 0a2a 2060 5461 696c  tion.....* `Tail
+00000d30: 6f60 2028 6465 6661 756c 7429 202d 205b  o` (default) - [
+00000d40: 54c3 a269 2d75 c3a2 6e20 4cc3 b42d 6dc3  T..i-u..n L..-m.
+00000d50: a12d 6ac4 ab20 5068 696e 672d 696d 2048  .-j.. Phing-im H
+00000d60: 6f6e 672d c3a0 6e5d 5b74 6169 6c6f 2d77  ong-..n][tailo-w
+00000d70: 696b 695d 0d0a 2a20 6050 4f4a 6020 2d20  iki]..* `POJ` - 
+00000d80: 5b50 65cc 8d68 2dc5 8d65 2d6a c4ab 5d5b  [Pe..h-..e-j..][
+00000d90: 706f 6a2d 7769 6b69 5d0d 0a2a 2060 5a68  poj-wiki]..* `Zh
+00000da0: 7579 696e 6020 2d20 5b54 6169 7761 6e65  uyin` - [Taiwane
+00000db0: 7365 2050 686f 6e65 7469 6320 5379 6d62  se Phonetic Symb
+00000dc0: 6f6c 735d 5b7a 6875 7969 6e2d 7769 6b69  ols][zhuyin-wiki
+00000dd0: 5d0d 0a2a 2060 544c 5041 6020 2d20 5b54  ]..* `TLPA` - [T
+00000de0: 6169 7761 6e65 7365 204c 616e 6775 6167  aiwanese Languag
+00000df0: 6520 5068 6f6e 6574 6963 2041 6c70 6861  e Phonetic Alpha
+00000e00: 6265 745d 5b74 6c70 612d 7769 6b69 5d0d  bet][tlpa-wiki].
+00000e10: 0a2a 2060 5069 6e67 7969 6d60 202d 205b  .* `Pingyim` - [
+00000e20: 4262 c3a1 6e6c c3a1 6d20 55c4 9320 50c3  Bb..nl..m U.. P.
+00000e30: ac6e 6779 c4ab 6d20 48c5 8d6e 6727 c3a0  .ngy..m H..ng'..
+00000e40: 6e5d 5b70 696e 6779 696d 2d77 696b 695d  n][pingyim-wiki]
+00000e50: 0d0a 2a20 6054 6f6e 6769 6f6e 6760 202d  ..* `Tongiong` -
+00000e60: 205b 4461 c4ab 2d67 68c3 ae20 54c5 8d6e   [Da..-gh.. T..n
+00000e70: 672d 69c5 8d6e 6720 50c4 ab6e 672d 696d  g-i..ng P..ng-im
+00000e80: 5d5b 746f 6e67 696f 6e67 2d77 696b 695d  ][tongiong-wiki]
+00000e90: 0d0a 2a20 6049 5041 6020 2d20 5b49 6e74  ..* `IPA` - [Int
+00000ea0: 6572 6e61 7469 6f6e 616c 2050 686f 6e65  ernational Phone
+00000eb0: 7469 6320 416c 7068 6162 6574 5d5b 6970  tic Alphabet][ip
+00000ec0: 612d 7769 6b69 5d0d 0a0d 0a7c 2074 6578  a-wiki]....| tex
+00000ed0: 7420 7c20 5461 696c 6f20 2020 7c20 504f  t | Tailo   | PO
+00000ee0: 4a20 2020 2020 7c20 5a68 7579 696e 2020  J     | Zhuyin  
+00000ef0: 2020 2020 7c20 544c 5041 2020 2020 2020      | TLPA      
+00000f00: 7c20 5069 6e67 7969 6d20 7c20 546f 6e67  | Pingyim | Tong
+00000f10: 696f 6e67 207c 2049 5041 2020 2020 2020  iong | IPA      
+00000f20: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+00000f30: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00000f40: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 207c   | ----------- |
+00000f50: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00000f60: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d20  ---- | -------- 
+00000f70: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  | ----------- |.
+00000f80: 0a7c 20e5 8fb0 e781 a320 7c20 54c3 a269  .| ...... | T..i
+00000f90: 2d75 c3a2 6e20 7c20 54c3 a269 2d6f c3a2  -u..n | T..i-o..
+00000fa0: 6e20 7c20 e384 89e3 849e cb8a 20e3 84a8  n | ........ ...
+00000fb0: e384 a2cb 8a20 7c20 5461 6935 2075 616e  ..... | Tai5 uan
+00000fc0: 3520 7c20 44c3 a169 77c3 a16e 2020 7c20  5 | D..iw..n  | 
+00000fd0: 54c4 8169 2d75 c78e 6e20 207c 2054 6169  T..i-u..n  | Tai
+00000fe0: c2b2 e281 b520 7561 6ec2 b2e2 81b5 207c  ..... uan..... |
+00000ff0: 0d0a 0d0a 2323 2323 2044 6961 6c65 6374  ....#### Dialect
+00001000: 0d0a 0d0a 6064 6961 6c65 6374 6020 5374  ....`dialect` St
+00001010: 7269 6e67 202d 2070 7265 6665 7272 6564  ring - preferred
+00001020: 2070 726f 6e75 6e63 6961 7469 6f6e 2e0d   pronunciation..
+00001030: 0a0d 0a2a 2060 736f 7574 6860 2028 6465  ...* `south` (de
+00001040: 6661 756c 7429 202d 205b 5a68 616e 677a  fault) - [Zhangz
+00001050: 686f 755d 5b7a 6861 6e67 7a68 6f75 2d77  hou][zhangzhou-w
+00001060: 696b 695d 2d6c 6561 6e69 6e67 2070 726f  iki]-leaning pro
+00001070: 6e75 6e63 6961 7469 6f6e 0d0a 2a20 606e  nunciation..* `n
+00001080: 6f72 7468 6020 2d20 5b51 7561 6e7a 686f  orth` - [Quanzho
+00001090: 755d 5b71 7561 6e7a 686f 752d 7769 6b69  u][quanzhou-wiki
+000010a0: 5d2d 6c65 616e 696e 6720 7072 6f6e 756e  ]-leaning pronun
+000010b0: 6369 6174 696f 6e0d 0a0d 0a7c 2074 6578  ciation....| tex
+000010c0: 7420 2020 7c20 736f 7574 6820 2020 2020  t   | south     
+000010d0: 2020 2020 7c20 6e6f 7274 6820 2020 2020      | north     
+000010e0: 2020 2020 7c0d 0a7c 202d 2d2d 2d2d 2d20      |..| ------ 
+000010f0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  | ------------- 
+00001100: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  | ------------- 
+00001110: 7c0d 0a7c 20e4 ba94 e69c 88e7 af80 207c  |..| ......... |
+00001120: 2047 c58d 6f2d 6775 65cc 8d68 2d74 7365   G..o-gue..h-tse
+00001130: 6820 7c20 47c5 8d6f 2d67 65cc 8d68 2d74  h | G..o-ge..h-t
+00001140: 7375 6568 207c 0d0a 0d0a 2323 2323 2046  sueh |....#### F
+00001150: 6f72 6d61 740d 0a0d 0a60 666f 726d 6174  ormat....`format
+00001160: 6020 5374 7269 6e67 202d 2066 6f72 6d61  ` String - forma
+00001170: 7420 696e 2077 6869 6368 2074 6f6e 6573  t in which tones
+00001180: 2077 696c 6c20 6265 2072 6570 7265 7365   will be represe
+00001190: 6e74 6564 2069 6e20 7468 6520 636f 6e76  nted in the conv
+000011a0: 6572 7465 6420 7365 6e74 656e 6365 2e0d  erted sentence..
+000011b0: 0a0d 0a2a 2060 6d61 726b 6020 2864 6566  ...* `mark` (def
+000011c0: 6175 6c74 2920 2d20 7573 6573 2064 6961  ault) - uses dia
+000011d0: 6372 6974 6963 7320 666f 7220 6561 6368  critics for each
+000011e0: 2073 796c 6c61 626c 652e 204e 6f74 2061   syllable. Not a
+000011f0: 7661 696c 6162 6c65 2066 6f72 2054 4c50  vailable for TLP
+00001200: 412e 0d0a 2a20 606e 756d 6265 7260 202d  A...* `number` -
+00001210: 2061 6464 2061 206e 756d 6265 7220 7768   add a number wh
+00001220: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
+00001230: 6865 2074 6f6e 6520 6174 2074 6865 2065  he tone at the e
+00001240: 6e64 206f 6620 7468 6520 7379 6c6c 6162  nd of the syllab
+00001250: 6c65 0d0a 2a20 6073 7472 6970 6020 2d20  le..* `strip` - 
+00001260: 7265 6d6f 7665 7320 616e 7920 746f 6e65  removes any tone
+00001270: 206d 6172 6b69 6e67 0d0a 0d0a 7c20 7465   marking....| te
+00001280: 7874 207c 206d 6172 6b20 2020 207c 206e  xt | mark    | n
+00001290: 756d 6265 7220 2020 207c 2073 7472 6970  umber    | strip
+000012a0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+000012b0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+000012c0: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+000012d0: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+000012e0: 75c3 a26e 207c 2054 6169 352d 7561 6e35  u..n | Tai5-uan5
+000012f0: 207c 2054 6169 2d75 616e 207c 0d0a 0d0a   | Tai-uan |....
+00001300: 2323 2323 2044 656c 696d 6974 6572 0d0a  #### Delimiter..
+00001310: 0d0a 6064 656c 696d 6974 6572 6020 5374  ..`delimiter` St
+00001320: 7269 6e67 202d 2073 6574 7320 7468 6520  ring - sets the 
+00001330: 6465 6c69 6d69 7465 7220 6368 6172 6163  delimiter charac
+00001340: 7465 7220 7468 6174 2077 696c 6c20 6265  ter that will be
+00001350: 2070 6c61 6365 6420 696e 2062 6574 7765   placed in betwe
+00001360: 656e 2073 796c 6c61 626c 6573 206f 6620  en syllables of 
+00001370: 6120 776f 7264 2e0d 0a0d 0a44 6566 6175  a word.....Defau
+00001380: 6c74 2076 616c 7565 2064 6570 656e 6473  lt value depends
+00001390: 206f 6e20 7468 6520 6368 6f73 656e 2060   on the chosen `
+000013a0: 7379 7374 656d 603a 0d0a 0d0a 2a20 6027  system`:....* `'
+000013b0: 2d27 6020 2d20 666f 7220 6054 6169 6c6f  -'` - for `Tailo
+000013c0: 602c 2060 504f 4a60 2c20 6054 6f6e 6769  `, `POJ`, `Tongi
+000013d0: 6f6e 6760 0d0a 2a20 6027 2760 202d 2066  ong`..* `''` - f
+000013e0: 6f72 2060 5069 6e67 7969 6d60 0d0a 2a20  or `Pingyim`..* 
+000013f0: 6027 2027 6020 2d20 666f 7220 605a 6875  `' '` - for `Zhu
+00001400: 7969 6e60 2c20 6054 4c50 4160 2c20 6049  yin`, `TLPA`, `I
+00001410: 5041 600d 0a0d 0a7c 2074 6578 7420 7c20  PA`....| text | 
+00001420: 272d 2720 2020 2020 7c20 2727 2020 2020  '-'     | ''    
+00001430: 207c 2027 2027 2020 2020 207c 0d0a 7c20   | ' '     |..| 
+00001440: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
+00001450: 202d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d   ------ | ------
+00001460: 2d20 7c0d 0a7c 20e5 8fb0 e781 a320 7c20  - |..| ...... | 
+00001470: 54c3 a269 2d75 c3a2 6e20 7c20 54c3 a269  T..i-u..n | T..i
+00001480: 75c3 a26e 207c 2054 c3a2 6920 75c3 a26e  u..n | T..i u..n
+00001490: 207c 0d0a 0d0a 2323 2323 2053 616e 6468   |....#### Sandh
+000014a0: 690d 0a0d 0a60 7361 6e64 6869 6020 5374  i....`sandhi` St
+000014b0: 7269 6e67 202d 2061 7070 6c69 6573 2074  ring - applies t
+000014c0: 6865 205b 7361 6e64 6869 2072 756c 6573  he [sandhi rules
+000014d0: 206f 6620 5461 6977 616e 6573 6520 486f   of Taiwanese Ho
+000014e0: 6b6b 6965 6e5d 5b73 616e 6468 692d 7769  kkien][sandhi-wi
+000014f0: 6b69 5d2e 0d0a 0d0a 5369 6e63 6520 6974  ki].....Since it
+00001500: 2773 2064 6966 6669 6375 6c74 2074 6f20  's difficult to 
+00001510: 656e 636f 6465 2061 6c6c 2073 616e 6468  encode all sandh
+00001520: 6920 7275 6c65 732c 2054 6169 6275 6e20  i rules, Taibun 
+00001530: 7072 6f76 6964 6573 206d 756c 7469 706c  provides multipl
+00001540: 6520 6d6f 6465 7320 666f 7220 7361 6e64  e modes for sand
+00001550: 6869 2063 6f6e 7665 7273 696f 6e20 746f  hi conversion to
+00001560: 2061 6c6c 6f77 2066 6f72 2063 7573 746f   allow for custo
+00001570: 6d69 7365 6420 7361 6e64 6869 2068 616e  mised sandhi han
+00001580: 646c 696e 672e 0d0a 0d0a 2a20 606e 6f6e  dling.....* `non
+00001590: 6560 202d 2064 6f65 736e 2774 2070 6572  e` - doesn't per
+000015a0: 666f 726d 2061 6e79 2074 6f6e 6520 7361  form any tone sa
+000015b0: 6e64 6869 0d0a 2a20 6061 7574 6f60 202d  ndhi..* `auto` -
+000015c0: 2063 6c6f 7365 7374 2061 7070 726f 7869   closest approxi
+000015d0: 6d61 7469 6f6e 2074 6f20 6675 6c6c 2063  mation to full c
+000015e0: 6f72 7265 6374 2074 6f6e 6520 7361 6e64  orrect tone sand
+000015f0: 6869 206f 6620 5461 6977 616e 6573 652c  hi of Taiwanese,
+00001600: 2077 6974 6820 7072 6f70 6572 2073 616e   with proper san
+00001610: 6468 6920 6f66 2070 726f 6e6f 756e 732c  dhi of pronouns,
+00001620: 2073 7566 6669 7865 732c 2061 6e64 2077   suffixes, and w
+00001630: 6f72 6473 2077 6974 6820 e4bb 940d 0a2a  ords with .....*
+00001640: 2060 6578 635f 6c61 7374 6020 2d20 6368   `exc_last` - ch
+00001650: 616e 6765 7320 746f 6e65 2066 6f72 2065  anges tone for e
+00001660: 7665 7279 2073 796c 6c61 626c 6520 6578  very syllable ex
+00001670: 6365 7074 2066 6f72 2074 6865 206c 6173  cept for the las
+00001680: 7420 6f6e 650d 0a2a 2060 696e 636c 5f6c  t one..* `incl_l
+00001690: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
+000016a0: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
+000016b0: 6c6c 6162 6c65 2069 6e63 6c75 6469 6e67  llable including
+000016c0: 2074 6865 206c 6173 7420 6f6e 650d 0a0d   the last one...
+000016d0: 0a44 6566 6175 6c74 2076 616c 7565 2064  .Default value d
+000016e0: 6570 656e 6473 206f 6e20 7468 6520 6368  epends on the ch
+000016f0: 6f73 656e 2060 7379 7374 656d 603a 0d0a  osen `system`:..
+00001700: 0d0a 2a20 6061 7574 6f60 202d 2066 6f72  ..* `auto` - for
+00001710: 2060 546f 6e67 696f 6e67 600d 0a2a 2060   `Tongiong`..* `
+00001720: 6e6f 6e65 6020 2d20 666f 7220 6054 6169  none` - for `Tai
+00001730: 6c6f 602c 2060 504f 4a60 2c20 605a 6875  lo`, `POJ`, `Zhu
+00001740: 7969 6e60 2c20 6054 4c50 4160 2c20 6050  yin`, `TLPA`, `P
+00001750: 696e 6779 696d 602c 2060 4950 4160 0d0a  ingyim`, `IPA`..
+00001760: 0d0a 7c20 7465 7874 2020 2020 2020 2020  ..| text        
+00001770: 2020 2020 207c 206e 6f6e 6520 2020 2020       | none     
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
+000017a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000017b0: 6578 635f 6c61 7374 2020 2020 2020 2020  exc_last        
+000017c0: 2020 2020 2020 2020 2020 7c20 696e 636c            | incl
+000017d0: 5f6c 6173 7420 2020 2020 2020 2020 2020  _last           
+000017e0: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001810: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001830: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
+00001870: 7c20 e980 99e6 98af e4bd a0e7 9a84 e689  | ..............
+00001880: 8be6 a99f e4bb 94e7 84a1 207c 2054 7365  .......... | Tse
+00001890: 2073 c4ab 206c c3ad 20c3 aa20 7473 6869   s.. l.. .. tshi
+000018a0: c3ba 2d6b 692d c3a1 2062 c3b4 207c 2054  ..-ki-.. b.. | T
+000018b0: 7365 2073 c3ac 206c 6920 c493 2074 7368  se s.. li .. tsh
+000018c0: 6975 2d6b c4ab 2dc3 a120 62c3 b43f 207c  iu-k..-.. b..? |
+000018d0: 2054 73c4 9320 73c3 ac20 6c69 20c4 9320   Ts.. s.. li .. 
+000018e0: 7473 6869 752d 6bc4 ab2d 6120 62c3 b420  tshiu-k..-a b.. 
+000018f0: 7c20 5473 c493 2073 c3ac 206c 6920 c493  | Ts.. s.. li ..
+00001900: 2074 7368 6975 2d6b c4ab 2d61 2062 c58d   tshiu-k..-a b..
+00001910: 207c 0d0a 0d0a 5361 6e64 6869 2072 756c   |....Sandhi rul
+00001920: 6573 2061 6c73 6f20 6368 616e 6765 2064  es also change d
+00001930: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+00001940: 6469 616c 6563 7420 6368 6f73 656e 2e0d  dialect chosen..
+00001950: 0a0d 0a7c 2074 6578 7420 7c20 6e6f 2073  ...| text | no s
+00001960: 616e 6468 6920 7c20 736f 7574 6820 2020  andhi | south   
+00001970: 7c20 6e6f 7274 6820 2020 7c0d 0a7c 202d  | north   |..| -
+00001980: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20  --- | --------- 
+00001990: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
+000019a0: 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781 a320  --- |..| ...... 
+000019b0: 7c20 54c3 a269 2d75 c3a2 6e20 2020 7c20  | T..i-u..n   | 
+000019c0: 54c4 8169 2d75 c3a2 6e20 7c20 54c3 a069  T..i-u..n | T..i
+000019d0: 2d75 c3a2 6e20 7c0d 0a0d 0a23 2323 2320  -u..n |....#### 
+000019e0: 5075 6e63 7475 6174 696f 6e0d 0a0d 0a60  Punctuation....`
+000019f0: 7075 6e63 7475 6174 696f 6e60 2053 7472  punctuation` Str
+00001a00: 696e 670d 0a0d 0a2a 2060 666f 726d 6174  ing....* `format
+00001a10: 6020 2864 6566 6175 6c74 2920 2d20 636f  ` (default) - co
+00001a20: 6e76 6572 7473 2043 6869 6e65 7365 2d73  nverts Chinese-s
+00001a30: 7479 6c65 2070 756e 6374 7561 7469 6f6e  tyle punctuation
+00001a40: 2074 6f20 4c61 7469 6e2d 7374 796c 6520   to Latin-style 
+00001a50: 7075 6e63 7475 6174 696f 6e20 616e 6420  punctuation and 
+00001a60: 6361 7069 7461 6c69 7365 7320 776f 7264  capitalises word
+00001a70: 7320 6174 2074 6865 2062 6567 696e 6e69  s at the beginni
+00001a80: 6e67 206f 6620 6561 6368 2073 656e 7465  ng of each sente
+00001a90: 6e63 652e 0d0a 2a20 606e 6f6e 6560 202d  nce...* `none` -
+00001aa0: 2070 7265 7365 7276 6573 2043 6869 6e65   preserves Chine
+00001ab0: 7365 2d73 7479 6c65 2070 756e 6374 7561  se-style punctua
+00001ac0: 7469 6f6e 2061 6e64 2064 6f65 736e 2774  tion and doesn't
+00001ad0: 2063 6170 6974 616c 6973 6520 776f 7264   capitalise word
+00001ae0: 7320 6174 2074 6865 2062 6567 696e 6e69  s at the beginni
+00001af0: 6e67 206f 6620 6e65 7720 7365 6e74 656e  ng of new senten
+00001b00: 6365 732e 0d0a 0d0a 7c20 7465 7874 2020  ces.....| text  
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b50: 2020 2020 2020 2020 207c 2066 6f72 6d61           | forma
+00001b60: 7420 2020 2020 2020 2020 2020 2020 2020  t               
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 2020 2020 207c 206e               | n
+00001bc0: 6f6e 6520 2020 2020 2020 2020 2020 2020  one             
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 7c0d 0a7c 202d 2d2d 2d2d 2d2d      |..| -------
+00001c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c70: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+00001c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 2d2d 207c 0d0a 7c20 e980 99e6 98af e887  -- |..| ........
+00001d50: bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3 808c  ................
+00001d60: e58d 97e3 808d efbc 88e7 99bd e8a9 b1e5  ................
+00001d70: ad97 efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
+00001d80: 9be6 b3a8 e99f b3e7 aca6 e899 9fef bc9a  ................
+00001d90: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
+00001da0: 8aef bc8c e59c 8be8 aa9e efbc 9a54 c3a1  .............T..
+00001db0: 696e c3a1 6eef bc89 e380 8220 7c20 5473  in..n...... | Ts
+00001dc0: 6520 73c4 ab20 54c3 a269 2d6c c3a2 6d2c  e s.. T..i-l..m,
+00001dd0: 206b c3a1 6e2d 7473 6869 6e67 2022 6cc3   k..n-tshing "l.
+00001de0: a26d 2220 2850 65cc 8d68 2d75 c493 2d6a  .m" (Pe..h-u..-j
+00001df0: c4ab 3a20 54c3 a269 2d6c c3a2 6d3b 2074  ..: T..i-l..m; t
+00001e00: 73c3 b92d 696d 2068 c3bb 2d68 c58d 3a20  s..-im h..-h..: 
+00001e10: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
+00001e20: 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3 a169  ., kok-g..: T..i
+00001e30: 6ec3 a16e 292e 207c 2074 7365 2073 c4ab  n..n). | tse s..
+00001e40: 2054 c3a2 692d 6cc3 a26d efbc 8c6b c3a1   T..i-l..m...k..
+00001e50: 6e2d 7473 6869 6e67 e380 8c6c c3a2 6de3  n-tshing...l..m.
+00001e60: 808d efbc 8850 65cc 8d68 2d75 c493 2d6a  .....Pe..h-u..-j
+00001e70: c4ab efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
+00001e80: 9b74 73c3 b92d 696d 2068 c3bb 2d68 c58d  .ts..-im h..-h..
+00001e90: efbc 9ae3 848a e384 9ecb 8a20 e384 8be3  ........... ....
+00001ea0: 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad efbc  .......kok-g....
+00001eb0: 9a54 c3a1 696e c3a1 6eef bc89 e380 8220  .T..in..n...... 
+00001ec0: 7c0d 0a0d 0a23 2323 2320 436f 6e76 6572  |....#### Conver
+00001ed0: 7420 6e6f 6e2d 434a 4b0d 0a0d 0a60 636f  t non-CJK....`co
+00001ee0: 6e76 6572 745f 6e6f 6e5f 636a 6b60 2042  nvert_non_cjk` B
+00001ef0: 6f6f 6c65 616e 202d 2064 6566 696e 6573  oolean - defines
+00001f00: 2077 6865 7468 6572 206f 7220 6e6f 7420   whether or not 
+00001f10: 746f 2063 6f6e 7665 7274 206e 6f6e 2d43  to convert non-C
+00001f20: 6869 6e65 7365 2077 6f72 6473 2e20 4361  hinese words. Ca
+00001f30: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+00001f40: 7665 7274 2054 6169 6c6f 2074 6f20 616e  vert Tailo to an
+00001f50: 6f74 6865 7220 726f 6d61 6e69 7361 7469  other romanisati
+00001f60: 6f6e 2073 7973 7465 6d2e 0d0a 0d0a 2a20  on system.....* 
+00001f70: 6054 7275 6560 202d 2063 6f6e 7665 7274  `True` - convert
+00001f80: 206e 6f6e 2d43 6869 6e65 7365 2063 6861   non-Chinese cha
+00001f90: 7261 6374 6572 2077 6f72 6473 0d0a 2a20  racter words..* 
+00001fa0: 6046 616c 7365 6020 2864 6566 6175 6c74  `False` (default
+00001fb0: 2920 2d20 636f 6e76 6572 7420 6f6e 6c79  ) - convert only
+00001fc0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+00001fd0: 6572 2077 6f72 6473 0d0a 0d0a 7c20 7465  er words....| te
+00001fe0: 7874 2020 2020 2020 7c20 4661 6c73 6520  xt      | False 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 2020 7c20 5472 7565 2020 2020 2020 2020    | True        
+00002010: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
+00002020: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002040: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00002060: 0d0a 7c20 e688 91e9 a39f 7068 c3a1 6e67  ..| ......ph..ng
+00002070: 207c 20e3 86a3 e384 a8e3 849a cb8b 20e3   | ........... .
+00002080: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
+00002090: c3a1 6e67 207c 20e3 86a3 e384 a8e3 849a  ..ng | .........
+000020a0: cb8b 20e3 8490 e384 a7e3 849a e386 b7cb  .. .............
+000020b0: 9920 e384 86e3 84a4 cb8b 207c 0d0a 0d0a  . ........ |....
+000020c0: 2323 2320 546f 6b65 6e69 7365 720d 0a0d  ### Tokeniser...
+000020d0: 0a60 546f 6b65 6e69 7365 7260 2063 6c61  .`Tokeniser` cla
+000020e0: 7373 2070 6572 666f 726d 7320 5b4e 4c54  ss performs [NLT
+000020f0: 4b20 776f 7264 7075 6e63 745f 746f 6b65  K wordpunct_toke
+00002100: 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b 656e  nize][nltk-token
+00002110: 697a 655d 2d6c 696b 6520 746f 6b65 6e69  ize]-like tokeni
+00002120: 7361 7469 6f6e 206f 6620 6120 5461 6977  sation of a Taiw
+00002130: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
+00002140: 6e74 656e 6365 2e0d 0a0d 0a60 6060 7079  ntence.....```py
+00002150: 7468 6f6e 0d0a 2320 436f 6e73 7472 7563  thon..# Construc
+00002160: 746f 720d 0a74 203d 2054 6f6b 656e 6973  tor..t = Tokenis
+00002170: 6572 2829 0d0a 0d0a 2320 546f 6b65 6e69  er()....# Tokeni
+00002180: 7365 2054 6169 7761 6e65 7365 2048 6f6b  se Taiwanese Hok
+00002190: 6b69 656e 2073 656e 7465 6e63 650d 0a74  kien sentence..t
+000021a0: 2e74 6f6b 656e 6973 6528 696e 7075 7429  .tokenise(input)
+000021b0: 0d0a 6060 600d 0a0d 0a23 2323 204f 7468  ..```....### Oth
+000021c0: 6572 2046 756e 6374 696f 6e73 0d0a 0d0a  er Functions....
+000021d0: 4861 6e64 7920 6675 6e63 7469 6f6e 7320  Handy functions 
+000021e0: 666f 7220 4e4c 5020 7461 736b 7320 696e  for NLP tasks in
+000021f0: 2054 6169 7761 6e65 7365 2048 6f6b 6b69   Taiwanese Hokki
+00002200: 656e 2e0d 0a0d 0a60 6060 7079 7468 6f6e  en.....```python
+00002210: 0d0a 2320 436f 6e76 6572 7420 746f 2054  ..# Convert to T
+00002220: 7261 6469 7469 6f6e 616c 0d0a 746f 5f74  raditional..to_t
+00002230: 7261 6469 7469 6f6e 616c 2869 6e70 7574  raditional(input
+00002240: 290d 0a0d 0a23 2043 6f6e 7665 7274 2074  )....# Convert t
+00002250: 6f20 5369 6d70 6c69 6669 6564 0d0a 746f  o Simplified..to
+00002260: 5f73 696d 706c 6966 6965 6428 696e 7075  _simplified(inpu
+00002270: 7429 0d0a 0d0a 2320 4368 6563 6b20 6966  t)....# Check if
+00002280: 2074 6865 2073 7472 696e 6720 6973 2066   the string is f
+00002290: 756c 6c79 2063 6f6d 706f 7365 6420 6f66  ully composed of
+000022a0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+000022b0: 6572 730d 0a69 735f 636a 6b28 696e 7075  ers..is_cjk(inpu
+000022c0: 7429 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c  t)..```........<
+000022d0: 212d 2d20 4558 414d 504c 4520 2d2d 3e0d  !-- EXAMPLE -->.
+000022e0: 0a23 2320 4578 616d 706c 650d 0a0d 0a60  .## Example....`
+000022f0: 6060 7079 7468 6f6e 0d0a 2320 436f 6e76  ``python..# Conv
+00002300: 6572 7465 720d 0a66 726f 6d20 7461 6962  erter..from taib
+00002310: 756e 2069 6d70 6f72 7420 436f 6e76 6572  un import Conver
+00002320: 7465 720d 0a0d 0a23 2320 5379 7374 656d  ter....## System
+00002330: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002340: 2920 2320 5461 696c 6f20 7379 7374 656d  ) # Tailo system
+00002350: 2064 6566 6175 6c74 0d0a 632e 6765 7428   default..c.get(
+00002360: 27e5 8588 e794 9fe8 ac9b efbc 8ce5 adb8  '...............
+00002370: e794 9fe6 81ac e681 ace8 81bd e380 8227  ...............'
+00002380: 290d 0a3e 3e20 5369 616e 2d73 696e 6e20  )..>> Sian-sinn 
+00002390: 6bc3 b36e 672c 2068 61cc 8d6b 2d73 696e  k..ng, ha..k-sin
+000023a0: 6720 7469 c481 6d2d 7469 c481 6d20 7468  g ti..m-ti..m th
+000023b0: 6961 6e6e 2e0d 0a0d 0a63 203d 2043 6f6e  iann.....c = Con
+000023c0: 7665 7274 6572 2873 7973 7465 6d3d 275a  verter(system='Z
+000023d0: 6875 7969 6e27 290d 0a63 2e67 6574 2827  huyin')..c.get('
+000023e0: e585 88e7 949f e8ac 9bef bc8c e5ad b8e7  ................
+000023f0: 949f e681 ace6 81ac e881 bde3 8082 2729  ..............')
+00002400: 0d0a 3e3e 20e3 8492 e384 a7e3 84a2 20e3  ..>> ......... .
+00002410: 8492 e386 aa20 e384 8de3 86b2 cb8b 2c20  ..... ........, 
+00002420: e384 8fe3 849a e386 b6cb 9920 e384 92e3  ........... ....
+00002430: 84a7 e384 a520 e384 89e3 84a7 e386 b0cb  ..... ..........
+00002440: ab20 e384 89e3 84a7 e386 b0cb ab20 e384  . ........... ..
+00002450: 8ae3 84a7 e386 a92e 0d0a 0d0a 2323 2044  ............## D
+00002460: 6961 6c65 6374 0d0a 6320 3d20 436f 6e76  ialect..c = Conv
+00002470: 6572 7465 7228 2920 2320 736f 7574 6820  erter() # south 
+00002480: 6469 616c 6563 7420 6465 6661 756c 740d  dialect default.
+00002490: 0a63 2e67 6574 2822 e688 91e6 acb2 e794  .c.get("........
+000024a0: a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a 3e3e  ..........")..>>
+000024b0: 2047 75c3 a120 6265 6820 c4ab 6e67 2074   Gu.. beh ..ng t
+000024c0: c4ab 2074 7369 61cc 8d68 2068 c3ae 0d0a  .. tsia..h h....
+000024d0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000024e0: 6469 616c 6563 743d 276e 6f72 7468 2729  dialect='north')
+000024f0: 0d0a 632e 6765 7428 22e6 8891 e6ac b2e7  ..c.get(".......
+00002500: 94a8 e7ae b8e9 a39f e9ad 9a22 290d 0a3e  ...........")..>
+00002510: 3e20 4775 c3a1 2062 7565 6820 c4ab 6e67  > Gu.. bueh ..ng
+00002520: 2074 c5ab 2074 7369 61cc 8d68 2068 c3bb   t.. tsia..h h..
+00002530: 0d0a 0d0a 2323 2046 6f72 6d61 740d 0a63  ....## Format..c
+00002540: 203d 2043 6f6e 7665 7274 6572 2829 2023   = Converter() #
+00002550: 2066 6f72 2054 6169 6c6f 2c20 6d61 726b   for Tailo, mark
+00002560: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
+00002570: 6574 2822 e794 9fe6 97a5 e5bf abe6 a882  et("............
+00002580: 2229 0d0a 3e3e 2053 656e 6e2d 6a69 cc8d  ")..>> Senn-ji..
+00002590: 7420 6b68 75c3 a069 2d6c 6fcc 8d6b 0d0a  t khu..i-lo..k..
+000025a0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000025b0: 666f 726d 6174 3d27 6e75 6d62 6572 2729  format='number')
+000025c0: 0d0a 632e 6765 7428 22e7 949f e697 a5e5  ..c.get(".......
+000025d0: bfab e6a8 8222 290d 0a3e 3e20 5365 6e6e  .....")..>> Senn
+000025e0: 312d 6a69 7438 206b 6875 6169 332d 6c6f  1-jit8 khuai3-lo
+000025f0: 6b38 0d0a 0d0a 6320 3d20 436f 6e76 6572  k8....c = Conver
+00002600: 7465 7228 666f 726d 6174 3d27 7374 7269  ter(format='stri
+00002610: 7027 290d 0a63 2e67 6574 2822 e794 9fe6  p')..c.get("....
+00002620: 97a5 e5bf abe6 a882 2229 0d0a 3e3e 2053  ........")..>> S
+00002630: 656e 6e2d 6a69 7420 6b68 7561 692d 6c6f  enn-jit khuai-lo
+00002640: 6b0d 0a0d 0a23 2320 4465 6c69 6d69 7465  k....## Delimite
+00002650: 720d 0a63 203d 2043 6f6e 7665 7274 6572  r..c = Converter
+00002660: 2864 656c 696d 6974 6572 3d27 2729 0d0a  (delimiter='')..
+00002670: 632e 6765 7428 22e5 8588 e794 9fe8 ac9b  c.get(".........
+00002680: efbc 8ce5 adb8 e794 9fe6 81ac e681 ace8  ................
+00002690: 81bd e380 8222 290d 0a3e 3e20 5369 616e  .....")..>> Sian
+000026a0: 7369 6e6e 206b c3b3 6e67 2c20 6861 cc8d  sinn k..ng, ha..
+000026b0: 6b73 696e 6720 7469 c481 6d74 69c4 816d  ksing ti..mti..m
+000026c0: 2074 6869 616e 6e2e 0d0a 0d0a 6320 3d20   thiann.....c = 
+000026d0: 436f 6e76 6572 7465 7228 7379 7374 656d  Converter(system
+000026e0: 3d27 5069 6e67 7969 6d27 2c20 6465 6c69  ='Pingyim', deli
+000026f0: 6d69 7465 723d 272d 2729 0d0a 632e 6765  miter='-')..c.ge
+00002700: 7428 22e5 8588 e794 9fe8 ac9b efbc 8ce5  t(".............
+00002710: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
+00002720: 8222 290d 0a3e 3e20 5369 c481 6e2d 736e  .")..>> Si..n-sn
+00002730: c4ab 2067 c792 6e67 2c20 68c3 a167 2d73  .. g..ng, h..g-s
+00002740: c4ab 6e67 2064 69c3 a26d 2d64 69c3 a26d  ..ng di..m-di..m
+00002750: 2074 696e c481 2e0d 0a0d 0a23 2320 5361   tin.......## Sa
+00002760: 6e64 6869 0d0a 6320 3d20 436f 6e76 6572  ndhi..c = Conver
+00002770: 7465 7228 2920 2320 666f 7220 5461 696c  ter() # for Tail
+00002780: 6f2c 2073 616e 6468 6920 6e6f 6e65 2062  o, sandhi none b
+00002790: 7920 6465 6661 756c 740d 0a63 2e67 6574  y default..c.get
+000027a0: 2822 e980 99e6 98af e58f b0e7 81a3 e59b  ("..............
+000027b0: a1e4 bb94 2229 0d0a 3e3e 2054 7365 2073  ....")..>> Tse s
+000027c0: c4ab 2054 c3a2 692d 75c3 a26e 2067 c3ad  .. T..i-u..n g..
+000027d0: 6e2d c3a1 0d0a 0d0a 6320 3d20 436f 6e76  n-......c = Conv
+000027e0: 6572 7465 7228 7361 6e64 6869 3d27 6175  erter(sandhi='au
+000027f0: 746f 2729 0d0a 632e 6765 7428 22e9 8099  to')..c.get("...
+00002800: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+00002810: 290d 0a3e 3e20 5473 6520 73c3 ac20 54c4  )..>> Tse s.. T.
+00002820: 8169 2d75 c481 6e20 6769 6e2d c3a1 0d0a  .i-u..n gin-....
+00002830: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002840: 7361 6e64 6869 3d27 6578 635f 6c61 7374  sandhi='exc_last
+00002850: 2729 0d0a 632e 6765 7428 22e9 8099 e698  ')..c.get(".....
+00002860: afe5 8fb0 e781 a3e5 9ba1 e4bb 9422 290d  .............").
+00002870: 0a3e 3e20 5473 c493 2073 c3ac 2054 c481  .>> Ts.. s.. T..
+00002880: 692d 75c4 816e 2067 696e 2dc3 a10d 0a0d  i-u..n gin-.....
+00002890: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
+000028a0: 616e 6468 693d 2769 6e63 6c5f 6c61 7374  andhi='incl_last
+000028b0: 2729 0d0a 632e 6765 7428 22e9 8099 e698  ')..c.get(".....
+000028c0: afe5 8fb0 e781 a3e5 9ba1 e4bb 9422 290d  .............").
+000028d0: 0a3e 3e20 5473 c493 2073 c3ac 2054 c481  .>> Ts.. s.. T..
+000028e0: 692d 75c4 816e 2067 696e 2d61 0d0a 0d0a  i-u..n gin-a....
+000028f0: 2323 2050 756e 6374 7561 7469 6f6e 0d0a  ## Punctuation..
+00002900: 6320 3d20 436f 6e76 6572 7465 7228 2920  c = Converter() 
+00002910: 2320 666f 726d 6174 2070 756e 6374 7561  # format punctua
+00002920: 7469 6f6e 2064 6566 6175 6c74 0d0a 632e  tion default..c.
+00002930: 6765 7428 22e5 a4aa e7a9 bae6 9c8b e58f  get("...........
+00002940: 8bef bc8c e681 81e5 a5bd efbc 81e6 8181  ................
+00002950: e9a3 9fe9 a3bd e69c aaef bc9f 2229 0d0a  ............")..
+00002960: 3e3e 2054 68c3 a069 2d6b 686f 6e67 2070  >> Th..i-khong p
+00002970: c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e 2d68  ..ng-i.., l..n-h
+00002980: c3b3 2120 4cc3 ad6e 2074 7369 61cc 8d68  ..! L..n tsia..h
+00002990: 2d70 c3a1 2062 75c4 933f 0d0a 0d0a 6320  -p.. bu..?....c 
+000029a0: 3d20 436f 6e76 6572 7465 7228 7075 6e63  = Converter(punc
+000029b0: 7475 6174 696f 6e3d 276e 6f6e 6527 290d  tuation='none').
+000029c0: 0a63 2e67 6574 2822 e5a4 aae7 a9ba e69c  .c.get("........
+000029d0: 8be5 8f8b efbc 8ce6 8181 e5a5 bdef bc81  ................
+000029e0: e681 81e9 a39f e9a3 bde6 9caa efbc 9f22  ..............."
+000029f0: 290d 0a3e 3e20 7468 c3a0 692d 6b68 6f6e  )..>> th..i-khon
+00002a00: 6720 70c3 ae6e 672d 69c3 baef bc8c 6cc3  g p..ng-i.....l.
+00002a10: ad6e 2d68 c3b3 efbc 816c c3ad 6e20 7473  .n-h.....l..n ts
+00002a20: 6961 cc8d 682d 70c3 a120 6275 c493 efbc  ia..h-p.. bu....
+00002a30: 9f0d 0a0d 0a23 2320 436f 6e76 6572 7420  .....## Convert 
+00002a40: 6e6f 6e2d 434a 4b0d 0a63 203d 2043 6f6e  non-CJK..c = Con
+00002a50: 7665 7274 2873 7973 7465 6d3d 275a 6875  vert(system='Zhu
+00002a60: 7969 6e27 2920 2320 4661 6c73 6520 636f  yin') # False co
+00002a70: 6e76 6572 745f 6e6f 6e5f 636a 6b20 6465  nvert_non_cjk de
+00002a80: 6661 756c 740d 0a63 2e67 6574 2822 e688  fault..c.get("..
+00002a90: 91e9 a39f 7068 c3a1 6e67 2229 0d0a 3e3e  ....ph..ng")..>>
+00002aa0: 20e3 86a3 e384 a8e3 849a cb8b 20e3 8490   ........... ...
+00002ab0: e384 a7e3 849a e386 b7cb 9920 7068 c3a1  ........... ph..
+00002ac0: 6e67 0d0a 0d0a 6320 3d20 436f 6e76 6572  ng....c = Conver
+00002ad0: 7428 7379 7374 656d 3d27 5a68 7579 696e  t(system='Zhuyin
+00002ae0: 272c 2063 6f6e 7665 7274 5f6e 6f6e 5f63  ', convert_non_c
+00002af0: 6a6b 3d54 7275 6529 0d0a 632e 6765 7428  jk=True)..c.get(
+00002b00: 22e6 8891 e9a3 9f70 68c3 a16e 6722 290d  "......ph..ng").
+00002b10: 0a3e 3e20 e386 a3e3 84a8 e384 9acb 8b20  .>> ........... 
+00002b20: e384 90e3 84a7 e384 9ae3 86b7 cb99 20e3  .............. .
+00002b30: 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23 2054  .............# T
+00002b40: 6f6b 656e 6973 6572 0d0a 6672 6f6d 2074  okeniser..from t
+00002b50: 6169 6275 6e20 696d 706f 7274 2054 6f6b  aibun import Tok
+00002b60: 656e 6973 6572 0d0a 0d0a 7420 3d20 546f  eniser....t = To
+00002b70: 6b65 6e69 7365 7228 290d 0a74 2e74 6f6b  keniser()..t.tok
+00002b80: 656e 6973 6528 22e5 a4aa e7a9 bae6 9c8b  enise(".........
+00002b90: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
+00002ba0: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
+00002bb0: 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27 2c20  ..>> ['......', 
+00002bc0: 27e6 9c8b e58f 8b27 2c20 27ef bc8c 272c  '......', '...',
+00002bd0: 2027 e681 81e5 a5bd 272c 2027 efbc 8127   '......', '...'
+00002be0: 2c20 27e6 8181 272c 2027 e9a3 9fe9 a3bd  , '...', '......
+00002bf0: 272c 2027 e69c aa27 2c20 27ef bc9f 275d  ', '...', '...']
+00002c00: 0d0a 0d0a 0d0a 2320 4f74 6865 7220 4675  ......# Other Fu
+00002c10: 6e63 7469 6f6e 730d 0a66 726f 6d20 7461  nctions..from ta
+00002c20: 6962 756e 2069 6d70 6f72 7420 746f 5f74  ibun import to_t
+00002c30: 7261 6469 7469 6f6e 616c 2c20 746f 5f73  raditional, to_s
+00002c40: 696d 706c 6966 6965 642c 2069 735f 636a  implified, is_cj
+00002c50: 6b0d 0a0d 0a74 6f5f 7472 6164 6974 696f  k....to_traditio
+00002c60: 6e61 6c28 22e6 8891 e590 ace6 97a0 e58f  nal("...........
+00002c70: b0e6 b9be e8af 9d22 290d 0a3e 3e20 e688  .......")..>> ..
+00002c80: 91e8 81bd e784 a1e5 8fb0 e781 a3e8 a9b1  ................
+00002c90: 0d0a 0d0a 746f 5f73 696d 706c 6966 6965  ....to_simplifie
+00002ca0: 6428 22e6 8891 e881 bde7 84a1 e887 bae7  d(".............
+00002cb0: 81a3 e8a9 b122 290d 0a3e 3e20 e688 91e5  .....")..>> ....
+00002cc0: 90ac e697 a0e5 8fb0 e6b9 bee8 af9d 0d0a  ................
+00002cd0: 0d0a 6973 5f63 6a6b 2827 e688 91e9 a39f  ..is_cjk('......
+00002ce0: e9ba ad27 290d 0a3e 3e20 5472 7565 0d0a  ...')..>> True..
+00002cf0: 0d0a 6973 5f63 6a6b 2827 e688 91e9 a39f  ..is_cjk('......
+00002d00: 7068 c3a1 6e67 2729 0d0a 3e3e 2046 616c  ph..ng')..>> Fal
+00002d10: 7365 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c  se..```........<
+00002d20: 212d 2d20 4441 5441 202d 2d3e 0d0a 2323  !-- DATA -->..##
+00002d30: 2044 6174 610d 0a0d 0a2d 205b 5461 6977   Data....- [Taiw
+00002d40: 616e 6573 652d 4368 696e 6573 6520 4f6e  anese-Chinese On
+00002d50: 6c69 6e65 2044 6963 7469 6f6e 6172 795d  line Dictionary]
+00002d60: 5b6f 6e6c 696e 652d 6469 6374 696f 6e61  [online-dictiona
+00002d70: 7279 5d20 2876 6961 205b 4368 686f 6554  ry] (via [ChhoeT
+00002d80: 6169 6769 5d5b 6461 7461 2d76 6961 5d29  aigi][data-via])
+00002d90: 0d0a 2d20 5b69 5461 6967 6920 4368 696e  ..- [iTaigi Chin
+00002da0: 6573 652d 5461 6977 616e 6573 6520 436f  ese-Taiwanese Co
+00002db0: 6d70 6172 6973 6f6e 2044 6963 7469 6f6e  mparison Diction
+00002dc0: 6172 795d 5b69 7461 6967 692d 6469 6374  ary][itaigi-dict
+00002dd0: 696f 6e61 7279 5d20 2876 6961 205b 4368  ionary] (via [Ch
+00002de0: 686f 6554 6169 6769 5d5b 6461 7461 2d76  hoeTaigi][data-v
+00002df0: 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21 2d2d  ia])........<!--
+00002e00: 2041 434b 4e4f 574c 4544 4745 4d45 4e54   ACKNOWLEDGEMENT
+00002e10: 5320 2d2d 3e0d 0a23 2320 4163 6b6e 6f77  S -->..## Acknow
+00002e20: 6c65 6467 656d 656e 7473 0d0a 0d0a 2d20  ledgements....- 
+00002e30: 5361 6d75 656c 204a 656e 2028 5b47 6974  Samuel Jen ([Git
+00002e40: 6875 625d 5b73 616d 7565 6c2d 6769 7468  hub][samuel-gith
+00002e50: 7562 5d20 c2b7 205b 4c69 6e6b 6564 496e  ub] .. [LinkedIn
+00002e60: 5d5b 7361 6d75 656c 2d6c 696e 6b65 6469  ][samuel-linkedi
+00002e70: 6e5d 2920 2d20 5461 6977 616e 6573 6520  n]) - Taiwanese 
+00002e80: 616e 6420 4d61 6e64 6172 696e 2074 7261  and Mandarin tra
+00002e90: 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a 0d0a  nslation........
+00002ea0: 3c21 2d2d 204c 4943 454e 4345 202d 2d3e  <!-- LICENCE -->
+00002eb0: 0d0a 2323 204c 6963 656e 6365 0d0a 0d0a  ..## Licence....
+00002ec0: 4265 6361 7573 6520 5461 6962 756e 2069  Because Taibun i
+00002ed0: 7320 4d49 542d 6c69 6365 6e73 6564 2c20  s MIT-licensed, 
+00002ee0: 616e 7920 6465 7665 6c6f 7065 7220 6361  any developer ca
+00002ef0: 6e20 6573 7365 6e74 6961 6c6c 7920 646f  n essentially do
+00002f00: 2077 6861 7465 7665 7220 7468 6579 2077   whatever they w
+00002f10: 616e 7420 7769 7468 2069 7420 6173 206c  ant with it as l
+00002f20: 6f6e 6720 6173 2074 6865 7920 696e 636c  ong as they incl
+00002f30: 7564 6520 7468 6520 6f72 6967 696e 616c  ude the original
+00002f40: 2063 6f70 7972 6967 6874 2061 6e64 206c   copyright and l
+00002f50: 6963 656e 6365 206e 6f74 6963 6520 696e  icence notice in
+00002f60: 2061 6e79 2063 6f70 6965 7320 6f66 2074   any copies of t
+00002f70: 6865 2073 6f75 7263 6520 636f 6465 2e20  he source code. 
+00002f80: 4e6f 7465 2c20 7468 6174 2074 6865 2064  Note, that the d
+00002f90: 6174 6120 7573 6564 2062 7920 7468 6520  ata used by the 
+00002fa0: 7061 636b 6167 6520 6973 206c 6963 656e  package is licen
+00002fb0: 7365 6420 756e 6465 7220 6120 6469 6666  sed under a diff
+00002fc0: 6572 656e 7420 636f 7079 7269 6768 742e  erent copyright.
+00002fd0: 0d0a 0d0a 5468 6520 6461 7461 2069 7320  ....The data is 
+00002fe0: 6c69 6365 6e73 6564 2075 6e64 6572 205b  licensed under [
+00002ff0: 4343 2042 592d 5341 2034 2e30 5d5b 6461  CC BY-SA 4.0][da
+00003000: 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a 3c21  ta-cc]........<!
+00003010: 2d2d 204d 4152 4b44 4f57 4e20 4c49 4e4b  -- MARKDOWN LINK
+00003020: 5320 2d2d 3e0d 0a5b 636f 6e74 7269 6275  S -->..[contribu
+00003030: 7469 6f6e 735d 3a20 6874 7470 733a 2f2f  tions]: https://
+00003040: 6769 7468 7562 2e63 6f6d 2f61 6e64 7265  github.com/andre
+00003050: 6968 6172 2f74 6169 6275 6e2f 6973 7375  ihar/taibun/issu
+00003060: 6573 0d0a 5b63 6f6e 7472 6962 7574 696f  es..[contributio
+00003070: 6e73 2d62 6164 6765 5d3a 2068 7474 7073  ns-badge]: https
+00003080: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00003090: 6f2f 6261 6467 652f 436f 6e74 7269 6275  o/badge/Contribu
+000030a0: 7469 6f6e 732d 5765 6c63 6f6d 6564 2d62  tions-Welcomed-b
+000030b0: 6531 3332 643f 7374 796c 653d 666f 722d  e132d?style=for-
+000030c0: 7468 652d 6261 6467 6526 6c6f 676f 3d67  the-badge&logo=g
+000030d0: 6974 6875 620d 0a5b 7465 7374 735d 3a20  ithub..[tests]: 
+000030e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000030f0: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+00003100: 6275 6e2f 6163 7469 6f6e 730d 0a5b 7465  bun/actions..[te
+00003110: 7374 732d 6261 6467 655d 3a20 6874 7470  sts-badge]: http
+00003120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00003130: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
+00003140: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
+00003150: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
+00003160: 756e 2f63 692e 7961 6d6c 3f73 7479 6c65  un/ci.yaml?style
+00003170: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
+00003180: 6f67 6f3d 6769 7468 7562 2d61 6374 696f  ogo=github-actio
+00003190: 6e73 266c 6f67 6f43 6f6c 6f72 3d66 6666  ns&logoColor=fff
+000031a0: 6666 660d 0a5b 7265 6c65 6173 652d 6261  fff..[release-ba
+000031b0: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
+000031c0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000031d0: 6875 622f 762f 7265 6c65 6173 652f 616e  hub/v/release/an
+000031e0: 6472 6569 6861 722f 7461 6962 756e 3f63  dreihar/taibun?c
+000031f0: 6f6c 6f72 3d33 3836 3138 6326 7374 796c  olor=38618c&styl
+00003200: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
+00003210: 0a5b 7265 6c65 6173 655d 3a20 6874 7470  .[release]: http
+00003220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00003230: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
+00003240: 7265 6c65 6173 6573 0d0a 5b6c 6963 656e  releases..[licen
+00003250: 6365 2d62 6164 6765 5d3a 2068 7474 7073  ce-badge]: https
+00003260: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00003270: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00003280: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00003290: 6e3f 636f 6c6f 723d 3030 3030 3030 2673  n?color=000000&s
+000032a0: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+000032b0: 6765 0d0a 5b6c 6963 656e 6365 5d3a 204c  ge..[licence]: L
+000032c0: 4943 454e 5345 0d0a 5b6c 696e 6b65 6469  ICENSE..[linkedi
+000032d0: 6e2d 6261 6467 655d 3a20 6874 7470 733a  n-badge]: https:
+000032e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000032f0: 2f62 6164 6765 2f4c 696e 6b65 6449 6e2d  /badge/LinkedIn-
+00003300: 3030 3737 6235 3f73 7479 6c65 3d66 6f72  0077b5?style=for
+00003310: 2d74 6865 2d62 6164 6765 266c 6f67 6f3d  -the-badge&logo=
+00003320: 6c69 6e6b 6564 696e 266c 6f67 6f43 6f6c  linkedin&logoCol
+00003330: 6f72 3d66 6666 6666 660d 0a5b 6c69 6e6b  or=ffffff..[link
+00003340: 6564 696e 5d3a 2068 7474 7073 3a2f 2f77  edin]: https://w
+00003350: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
+00003360: 696e 2f61 6e64 7265 692d 6861 7262 6163  in/andrei-harbac
+00003370: 686f 762f 0d0a 5b6a 732d 6261 6467 655d  hov/..[js-badge]
+00003380: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00003390: 6965 6c64 732e 696f 2f62 6164 6765 2f4a  ields.io/badge/J
+000033a0: 535f 5665 7273 696f 6e2d 6637 6466 3165  S_Version-f7df1e
+000033b0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+000033c0: 6164 6765 266c 6f67 6f3d 6a61 7661 7363  adge&logo=javasc
+000033d0: 7269 7074 266c 6f67 6f43 6f6c 6f72 3d30  ript&logoColor=0
+000033e0: 3030 3030 300d 0a5b 6a73 2d6c 696e 6b5d  00000..[js-link]
+000033f0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00003400: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
+00003410: 6169 6275 6e2e 6a73 0d0a 0d0a 5b70 7970  aibun.js....[pyp
+00003420: 695d 3a20 6874 7470 733a 2f2f 7079 7069  i]: https://pypi
+00003430: 2e6f 7267 2f70 726f 6a65 6374 2f74 6169  .org/project/tai
+00003440: 6275 6e0d 0a5b 6275 675d 3a20 6874 7470  bun..[bug]: http
+00003450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00003460: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
+00003470: 6973 7375 6573 0d0a 5b6f 6e6c 696e 652d  issues..[online-
+00003480: 6469 6374 696f 6e61 7279 5d3a 2068 7474  dictionary]: htt
+00003490: 703a 2f2f 6970 3139 3430 3937 2e6e 7463  p://ip194097.ntc
+000034a0: 752e 6564 752e 7477 2f75 6e67 6961 6e2f  u.edu.tw/ungian/
+000034b0: 736f 616e 6e74 656e 672f 6368 696c 2f54  soannteng/chil/T
+000034c0: 6169 686f 612e 6173 700d 0a5b 6974 6169  aihoa.asp..[itai
+000034d0: 6769 2d64 6963 7469 6f6e 6172 795d 3a20  gi-dictionary]: 
+000034e0: 6874 7470 733a 2f2f 6974 6169 6769 2e74  https://itaigi.t
+000034f0: 772f 0d0a 5b64 6174 612d 7669 615d 3a20  w/..[data-via]: 
+00003500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003510: 6f6d 2f43 6868 6f65 5461 6967 692f 4368  om/ChhoeTaigi/Ch
+00003520: 686f 6554 6169 6769 4461 7461 6261 7365  hoeTaigiDatabase
+00003530: 0d0a 5b64 6174 612d 6363 5d3a 2068 7474  ..[data-cc]: htt
+00003540: 7073 3a2f 2f63 7265 6174 6976 6563 6f6d  ps://creativecom
+00003550: 6d6f 6e73 2e6f 7267 2f6c 6963 656e 7365  mons.org/license
+00003560: 732f 6279 2d73 612f 342e 302f 6465 6564  s/by-sa/4.0/deed
+00003570: 2e65 6e0d 0a5b 7361 6d75 656c 2d67 6974  .en..[samuel-git
+00003580: 6875 625d 3a20 6874 7470 733a 2f2f 6769  hub]: https://gi
+00003590: 7468 7562 2e63 6f6d 2f53 5353 616d 0d0a  thub.com/SSSam..
+000035a0: 5b73 616d 7565 6c2d 6c69 6e6b 6564 696e  [samuel-linkedin
+000035b0: 5d3a 2068 7474 7073 3a2f 2f77 7777 2e6c  ]: https://www.l
+000035c0: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f73  inkedin.com/in/s
+000035d0: 616d 7565 6c2d 6a65 6e2f 0d0a 0d0a 5b74  amuel-jen/....[t
+000035e0: 6169 6c6f 2d77 696b 695d 3a20 6874 7470  ailo-wiki]: http
+000035f0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00003600: 2e6f 7267 2f77 696b 692f 5425 4333 2541  .org/wiki/T%C3%A
+00003610: 3269 2d75 2543 3325 4132 6e5f 4c25 4333  2i-u%C3%A2n_L%C3
+00003620: 2542 342d 6d25 4333 2541 312d 6a25 4334  %B4-m%C3%A1-j%C4
+00003630: 2541 425f 5068 696e 672d 696d 5f48 6f6e  %AB_Phing-im_Hon
+00003640: 672d 2543 3325 4130 6e0d 0a5b 706f 6a2d  g-%C3%A0n..[poj-
+00003650: 7769 6b69 5d3a 2068 7474 7073 3a2f 2f65  wiki]: https://e
+00003660: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00003670: 7769 6b69 2f50 6525 4343 2538 4468 2d25  wiki/Pe%CC%8Dh-%
+00003680: 4335 2538 4465 2d6a 2543 3425 4142 0d0a  C5%8De-j%C4%AB..
+00003690: 5b7a 6875 7969 6e2d 7769 6b69 5d3a 2068  [zhuyin-wiki]: h
+000036a0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+000036b0: 6469 612e 6f72 672f 7769 6b69 2f54 6169  dia.org/wiki/Tai
+000036c0: 7761 6e65 7365 5f50 686f 6e65 7469 635f  wanese_Phonetic_
+000036d0: 5379 6d62 6f6c 730d 0a5b 746c 7061 2d77  Symbols..[tlpa-w
+000036e0: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+000036f0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003700: 696b 692f 5461 6977 616e 6573 655f 4c61  iki/Taiwanese_La
+00003710: 6e67 7561 6765 5f50 686f 6e65 7469 635f  nguage_Phonetic_
+00003720: 416c 7068 6162 6574 0d0a 5b70 696e 6779  Alphabet..[pingy
+00003730: 696d 2d77 696b 695d 3a20 6874 7470 733a  im-wiki]: https:
+00003740: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00003750: 7267 2f77 696b 692f 4262 2543 3325 4131  rg/wiki/Bb%C3%A1
+00003760: 6e6c 2543 3325 4131 6d5f 7025 4333 2541  nl%C3%A1m_p%C3%A
+00003770: 436e 6779 2543 3425 4142 6d0d 0a5b 746f  Cngy%C4%ABm..[to
+00003780: 6e67 696f 6e67 2d77 696b 695d 3a20 6874  ngiong-wiki]: ht
+00003790: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000037a0: 6961 2e6f 7267 2f77 696b 692f 4461 2543  ia.org/wiki/Da%C
+000037b0: 3425 4142 2d67 6825 4333 2541 455f 7425  4%AB-gh%C3%AE_t%
+000037c0: 4335 2538 446e 672d 6925 4335 2538 446e  C5%8Dng-i%C5%8Dn
+000037d0: 675f 7025 4334 2541 426e 672d 696d 0d0a  g_p%C4%ABng-im..
+000037e0: 5b69 7061 2d77 696b 695d 3a20 6874 7470  [ipa-wiki]: http
+000037f0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00003800: 2e6f 7267 2f77 696b 692f 496e 7465 726e  .org/wiki/Intern
+00003810: 6174 696f 6e61 6c5f 5068 6f6e 6574 6963  ational_Phonetic
+00003820: 5f41 6c70 6861 6265 740d 0a5b 7a68 616e  _Alphabet..[zhan
+00003830: 677a 686f 752d 7769 6b69 5d3a 2068 7474  gzhou-wiki]: htt
+00003840: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00003850: 612e 6f72 672f 7769 6b69 2f5a 6861 6e67  a.org/wiki/Zhang
+00003860: 7a68 6f75 5f64 6961 6c65 6374 730d 0a5b  zhou_dialects..[
+00003870: 7175 616e 7a68 6f75 2d77 696b 695d 3a20  quanzhou-wiki]: 
+00003880: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00003890: 6564 6961 2e6f 7267 2f77 696b 692f 5175  edia.org/wiki/Qu
+000038a0: 616e 7a68 6f75 5f64 6961 6c65 6374 730d  anzhou_dialects.
+000038b0: 0a5b 6e6c 746b 2d74 6f6b 656e 697a 655d  .[nltk-tokenize]
+000038c0: 3a20 6874 7470 733a 2f2f 6e6c 746b 2e6f  : https://nltk.o
+000038d0: 7267 2f61 7069 2f6e 6c74 6b2e 746f 6b65  rg/api/nltk.toke
+000038e0: 6e69 7a65 2e68 746d 6c0d 0a5b 7361 6e64  nize.html..[sand
+000038f0: 6869 2d77 696b 695d 3a20 6874 7470 733a  hi-wiki]: https:
+00003900: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00003910: 7267 2f77 696b 692f 5461 6977 616e 6573  rg/wiki/Taiwanes
+00003920: 655f 486f 6b6b 6965 6e23 546f 6e65 2532  e_Hokkien#Tone%2
+00003930: 3073 616e 6468 693a 7e3a 7465 7874 3d74  0sandhi:~:text=t
+00003940: 686e 6725 4532 2539 4625 4139 2532 3028  hng%E2%9F%A9%20(
+00003950: 2532 3273 6f75 7025 3232 292e 2d2c 546f  %22soup%22).-,To
+00003960: 6e65 2532 3073 616e 6468 692c 2d25 3542  ne%20sandhi,-%5B
+00003970: 6564 6974 2535 440d 0a                   edit%5D..
```

### Comparing `example990420-1.1.0/example990420.egg-info/PKG-INFO` & `example990420-1.1.1/example990420.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2065 7861  : 2.1..Name: exa
 00000020: 6d70 6c65 3939 3034 3230 0d0a 5665 7273  mple990420..Vers
-00000030: 696f 6e3a 2031 2e31 2e30 0d0a 5375 6d6d  ion: 1.1.0..Summ
+00000030: 696f 6e3a 2031 2e31 2e31 0d0a 5375 6d6d  ion: 1.1.1..Summ
 00000040: 6172 793a 2054 6169 7761 6e65 7365 2048  ary: Taiwanese H
 00000050: 6f6b 6b69 656e 2054 7261 6e73 6c69 7465  okkien Translite
 00000060: 7261 746f 7220 616e 6420 546f 6b65 6e69  rator and Tokeni
 00000070: 7365 720d 0a48 6f6d 652d 7061 6765 3a20  ser..Home-page: 
 00000080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000090: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
 000000a0: 6275 6e0d 0a41 7574 686f 723a 2041 6e64  bun..Author: And
@@ -47,767 +47,874 @@
 000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
 000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
 00000300: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
 00000310: 653a 204c 4943 454e 5345 0d0a 0d0a 3c21  e: LICENSE....<!
 00000320: 2d2d 2050 524f 4a45 4354 204c 4f47 4f20  -- PROJECT LOGO 
 00000330: 2d2d 3e0d 0a3c 6272 202f 3e0d 0a3c 6469  -->..<br />..<di
 00000340: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000350: 3e0d 0a20 200d 0a23 2054 6169 6275 6e0d  >..  ..# Taibun.
-00000360: 0a0d 0a0d 0a0d 0a3c 212d 2d20 5052 4f4a  .......<!-- PROJ
-00000370: 4543 5420 5348 4945 4c44 5320 2d2d 3e0d  ECT SHIELDS -->.
-00000380: 0a5b 215b 5465 7374 735d 5b74 6573 7473  .[![Tests][tests
-00000390: 2d62 6164 6765 5d5d 5b74 6573 7473 5d0d  -badge]][tests].
-000003a0: 0a5b 215b 436f 6e74 7269 6275 746f 7273  .[![Contributors
-000003b0: 5d5b 636f 6e74 7269 6275 746f 7273 2d62  ][contributors-b
-000003c0: 6164 6765 5d5d 5b63 6f6e 7472 6962 7574  adge]][contribut
-000003d0: 6f72 735d 0d0a 5b21 5b52 656c 6561 7365  ors]..[![Release
-000003e0: 5d5b 7265 6c65 6173 652d 6261 6467 655d  ][release-badge]
-000003f0: 5d5b 7265 6c65 6173 655d 0d0a 5b21 5b4c  ][release]..[![L
-00000400: 6963 656e 6365 5d5b 6c69 6365 6e63 652d  icence][licence-
-00000410: 6261 6467 655d 5d5b 6c69 6365 6e63 655d  badge]][licence]
-00000420: 0d0a 5b21 5b4c 696e 6b65 6449 6e5d 5b6c  ..[![LinkedIn][l
-00000430: 696e 6b65 6469 6e2d 6261 6467 655d 5d5b  inkedin-badge]][
-00000440: 6c69 6e6b 6564 696e 5d0d 0a0d 0a2a 2a54  linkedin]....**T
-00000450: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000460: 2054 7261 6e73 6c69 7465 7261 746f 7220   Transliterator 
-00000470: 616e 6420 546f 6b65 6e69 7365 722a 2a0d  and Tokeniser**.
-00000480: 0a0d 0a49 7420 6861 7320 6d65 7468 6f64  ...It has method
-00000490: 7320 7468 6174 2061 6c6c 6f77 2074 6f20  s that allow to 
-000004a0: 6375 7374 6f6d 6973 6520 7472 616e 736c  customise transl
-000004b0: 6974 6572 6174 696f 6e20 616e 6420 7265  iteration and re
-000004c0: 7472 6965 7665 2061 6e79 206e 6563 6573  trieve any neces
-000004d0: 7361 7279 2069 6e66 6f72 6d61 7469 6f6e  sary information
-000004e0: 2061 626f 7574 2054 6169 7761 6e65 7365   about Taiwanese
-000004f0: 2048 6f6b 6b69 656e 2070 726f 6e75 6e63   Hokkien pronunc
-00000500: 6961 7469 6f6e 2e3c 6272 202f 3e0d 0a49  iation.<br />..I
-00000510: 6e63 6c75 6465 7320 776f 7264 2074 6f6b  ncludes word tok
-00000520: 656e 6973 6572 2066 6f72 2054 6169 7761  eniser for Taiwa
-00000530: 6e65 7365 2048 6f6b 6b69 656e 2e0d 0a0d  nese Hokkien....
-00000540: 0a5b 5265 706f 7274 2042 7567 5d5b 6275  .[Report Bug][bu
-00000550: 675d 20e2 80a2 0d0a 5b50 7950 495d 5b70  g] .....[PyPI][p
-00000560: 7970 695d 0d0a 0d0a 3c2f 6469 763e 0d0a  ypi]....</div>..
-00000570: 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d 0a0d  ......---.......
-00000580: 0a3c 212d 2d20 494e 5354 414c 4c20 2d2d  .<!-- INSTALL --
-00000590: 3e0d 0a23 2320 496e 7374 616c 6c0d 0a0d  >..## Install...
-000005a0: 0a54 6169 6275 6e20 6361 6e20 6265 2069  .Taibun can be i
-000005b0: 6e73 7461 6c6c 6564 2066 726f 6d20 5b70  nstalled from [p
-000005c0: 7970 695d 5b70 7970 695d 0d0a 0d0a 6060  ypi][pypi]....``
-000005d0: 6062 6173 680d 0a24 2070 6970 2069 6e73  `bash..$ pip ins
-000005e0: 7461 6c6c 2074 6169 6275 6e0d 0a60 6060  tall taibun..```
-000005f0: 0d0a 0d0a 0d0a 0d0a 3c21 2d2d 2055 5341  ........<!-- USA
-00000600: 4745 202d 2d3e 0d0a 2323 2055 7361 6765  GE -->..## Usage
-00000610: 0d0a 0d0a 2323 2320 436f 6e76 6572 7465  ....### Converte
-00000620: 720d 0a0d 0a60 436f 6e76 6572 7465 7260  r....`Converter`
-00000630: 2063 6c61 7373 2074 7261 6e73 6c69 7465   class translite
-00000640: 7261 7465 7320 7468 6520 4368 696e 6573  rates the Chines
-00000650: 6520 6368 6172 6163 7465 7273 2074 6f20  e characters to 
-00000660: 7468 6520 6368 6f73 656e 2074 7261 6e73  the chosen trans
-00000670: 6c69 7465 7261 7469 6f6e 2073 7973 7465  literation syste
-00000680: 6d20 7769 7468 2070 6172 616d 6574 6572  m with parameter
-00000690: 7320 7370 6563 6966 6965 6420 6279 2074  s specified by t
-000006a0: 6865 2064 6576 656c 6f70 6572 2e20 576f  he developer. Wo
-000006b0: 726b 7320 666f 7220 626f 7468 2054 7261  rks for both Tra
-000006c0: 6469 7469 6f6e 616c 2061 6e64 2053 696d  ditional and Sim
-000006d0: 706c 6966 6965 6420 6368 6172 6163 7465  plified characte
-000006e0: 7273 2e0d 0a0d 0a60 6060 7079 7468 6f6e  rs.....```python
-000006f0: 0d0a 2320 636f 6e73 7472 7563 746f 720d  ..# constructor.
-00000700: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
-00000710: 7973 7465 6d2c 2064 6961 6c65 6374 2c20  ystem, dialect, 
-00000720: 666f 726d 6174 2c20 6465 6c69 6d69 7465  format, delimite
-00000730: 722c 2073 616e 6468 692c 2070 756e 6374  r, sandhi, punct
-00000740: 7561 7469 6f6e 2c20 636f 6e76 6572 745f  uation, convert_
-00000750: 6e6f 6e5f 636a 6b29 0d0a 0d0a 2320 7472  non_cjk)....# tr
-00000760: 616e 736c 6974 6572 6174 6520 4368 696e  ansliterate Chin
-00000770: 6573 6520 6368 6172 6163 7465 7273 0d0a  ese characters..
-00000780: 632e 6765 7428 696e 7075 7429 0d0a 6060  c.get(input)..``
-00000790: 600d 0a0d 0a23 2323 2320 5379 7374 656d  `....#### System
-000007a0: 0d0a 0d0a 6073 7973 7465 6d60 2053 7472  ....`system` Str
-000007b0: 696e 6720 2d20 7379 7374 656d 206f 6620  ing - system of 
-000007c0: 7472 616e 736c 6974 6572 6174 696f 6e2e  transliteration.
-000007d0: 0d0a 0d0a 2a20 6054 6169 6c6f 6020 2864  ....* `Tailo` (d
-000007e0: 6566 6175 6c74 2920 2d20 5b54 c3a2 692d  efault) - [T..i-
-000007f0: 75c3 a26e 204c c3b4 2d6d c3a1 2d6a c4ab  u..n L..-m..-j..
-00000800: 2050 6869 6e67 2d69 6d20 486f 6e67 2dc3   Phing-im Hong-.
-00000810: a06e 5d5b 7461 696c 6f2d 7769 6b69 5d0d  .n][tailo-wiki].
-00000820: 0a2a 2060 504f 4a60 202d 205b 5065 cc8d  .* `POJ` - [Pe..
-00000830: 682d c58d 652d 6ac4 ab5d 5b70 6f6a 2d77  h-..e-j..][poj-w
-00000840: 696b 695d 0d0a 2a20 605a 6875 7969 6e60  iki]..* `Zhuyin`
-00000850: 202d 205b 5461 6977 616e 6573 6520 5068   - [Taiwanese Ph
-00000860: 6f6e 6574 6963 2053 796d 626f 6c73 5d5b  onetic Symbols][
-00000870: 7a68 7579 696e 2d77 696b 695d 0d0a 2a20  zhuyin-wiki]..* 
-00000880: 6054 4c50 4160 202d 205b 5461 6977 616e  `TLPA` - [Taiwan
-00000890: 6573 6520 4c61 6e67 7561 6765 2050 686f  ese Language Pho
-000008a0: 6e65 7469 6320 416c 7068 6162 6574 5d5b  netic Alphabet][
-000008b0: 746c 7061 2d77 696b 695d 0d0a 2a20 6050  tlpa-wiki]..* `P
-000008c0: 696e 6779 696d 6020 2d20 5b42 62c3 a16e  ingyim` - [Bb..n
-000008d0: 6cc3 a16d 2055 c493 2050 c3ac 6e67 79c4  l..m U.. P..ngy.
-000008e0: ab6d 2048 c58d 6e67 27c3 a06e 5d5b 7069  .m H..ng'..n][pi
-000008f0: 6e67 7969 6d2d 7769 6b69 5d0d 0a2a 2060  ngyim-wiki]..* `
-00000900: 546f 6e67 696f 6e67 6020 2d20 5b44 61c4  Tongiong` - [Da.
-00000910: ab2d 6768 c3ae 2054 c58d 6e67 2d69 c58d  .-gh.. T..ng-i..
-00000920: 6e67 2050 c4ab 6e67 2d69 6d5d 5b74 6f6e  ng P..ng-im][ton
-00000930: 6769 6f6e 672d 7769 6b69 5d0d 0a2a 2060  giong-wiki]..* `
-00000940: 4950 4160 202d 205b 496e 7465 726e 6174  IPA` - [Internat
-00000950: 696f 6e61 6c20 5068 6f6e 6574 6963 2041  ional Phonetic A
-00000960: 6c70 6861 6265 745d 5b69 7061 2d77 696b  lphabet][ipa-wik
-00000970: 695d 0d0a 0d0a 7c20 7465 7874 207c 2054  i]....| text | T
-00000980: 6169 6c6f 2020 207c 2050 4f4a 2020 2020  ailo   | POJ    
-00000990: 207c 205a 6875 7969 6e20 2020 2020 207c   | Zhuyin      |
-000009a0: 2054 4c50 4120 2020 2020 207c 2050 696e   TLPA      | Pin
-000009b0: 6779 696d 207c 2054 6f6e 6769 6f6e 6720  gyim | Tongiong 
-000009c0: 7c20 4950 4120 2020 2020 2020 2020 7c0d  | IPA         |.
-000009d0: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
-000009e0: 2d20 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  - | ------- | --
-000009f0: 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  --------- | ----
-00000a00: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d20  ----- | ------- 
-00000a10: 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  | -------- | ---
-00000a20: 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20 e58f  -------- |..| ..
-00000a30: b0e7 81a3 207c 2054 c3a2 692d 75c3 a26e  .... | T..i-u..n
-00000a40: 207c 2054 c3a2 692d 6fc3 a26e 207c 20e3   | T..i-o..n | .
-00000a50: 8489 e384 9ecb 8a20 e384 a8e3 84a2 cb8a  ....... ........
-00000a60: 207c 2054 6169 3520 7561 6e35 207c 2044   | Tai5 uan5 | D
-00000a70: c3a1 6977 c3a1 6e20 207c 2054 c481 692d  ..iw..n  | T..i-
-00000a80: 75c7 8e6e 2020 7c20 5461 69c2 b2e2 81b5  u..n  | Tai.....
-00000a90: 2075 616e c2b2 e281 b520 7c0d 0a0d 0a23   uan..... |....#
-00000aa0: 2323 2320 4469 616c 6563 740d 0a0d 0a60  ### Dialect....`
-00000ab0: 6469 616c 6563 7460 2053 7472 696e 6720  dialect` String 
-00000ac0: 2d20 7072 6566 6572 7265 6420 7072 6f6e  - preferred pron
-00000ad0: 756e 6369 6174 696f 6e2e 0d0a 0d0a 2a20  unciation.....* 
-00000ae0: 6073 6f75 7468 6020 2864 6566 6175 6c74  `south` (default
-00000af0: 2920 2d20 5b5a 6861 6e67 7a68 6f75 5d5b  ) - [Zhangzhou][
-00000b00: 7a68 616e 677a 686f 752d 7769 6b69 5d2d  zhangzhou-wiki]-
-00000b10: 6c65 616e 696e 6720 7072 6f6e 756e 6369  leaning pronunci
-00000b20: 6174 696f 6e0d 0a2a 2060 6e6f 7274 6860  ation..* `north`
-00000b30: 202d 205b 5175 616e 7a68 6f75 5d5b 7175   - [Quanzhou][qu
-00000b40: 616e 7a68 6f75 2d77 696b 695d 2d6c 6561  anzhou-wiki]-lea
-00000b50: 6e69 6e67 2070 726f 6e75 6e63 6961 7469  ning pronunciati
-00000b60: 6f6e 0d0a 0d0a 7c20 7465 7874 2020 207c  on....| text   |
-00000b70: 2073 6f75 7468 2020 2020 2020 2020 207c   south         |
-00000b80: 206e 6f72 7468 2020 2020 2020 2020 207c   north         |
-00000b90: 0d0a 7c20 2d2d 2d2d 2d2d 207c 202d 2d2d  ..| ------ | ---
-00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
-00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a 7c20  ---------- |..| 
-00000bc0: e4ba 94e6 9c88 e7af 8020 7c20 47c5 8d6f  ......... | G..o
-00000bd0: 2d67 7565 cc8d 682d 7473 6568 207c 2047  -gue..h-tseh | G
-00000be0: c58d 6f2d 6765 cc8d 682d 7473 7565 6820  ..o-ge..h-tsueh 
-00000bf0: 7c0d 0a0d 0a23 2323 2320 466f 726d 6174  |....#### Format
-00000c00: 0d0a 0d0a 6066 6f72 6d61 7460 2053 7472  ....`format` Str
-00000c10: 696e 6720 2d20 666f 726d 6174 2069 6e20  ing - format in 
-00000c20: 7768 6963 6820 746f 6e65 7320 7769 6c6c  which tones will
-00000c30: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
-00000c40: 696e 2074 6865 2063 6f6e 7665 7274 6564  in the converted
-00000c50: 2073 656e 7465 6e63 652e 0d0a 0d0a 2a20   sentence.....* 
-00000c60: 606d 6172 6b60 2028 6465 6661 756c 7429  `mark` (default)
-00000c70: 202d 2075 7365 7320 6469 6163 7269 7469   - uses diacriti
-00000c80: 6373 2066 6f72 2065 6163 6820 7379 6c6c  cs for each syll
-00000c90: 6162 6c65 2e20 4e6f 7420 6176 6169 6c61  able. Not availa
-00000ca0: 626c 6520 666f 7220 544c 5041 2e0d 0a2a  ble for TLPA...*
-00000cb0: 2060 6e75 6d62 6572 6020 2d20 6164 6420   `number` - add 
-00000cc0: 6120 6e75 6d62 6572 2077 6869 6368 2072  a number which r
-00000cd0: 6570 7265 7365 6e74 7320 7468 6520 746f  epresents the to
-00000ce0: 6e65 2061 7420 7468 6520 656e 6420 6f66  ne at the end of
-00000cf0: 2074 6865 2073 796c 6c61 626c 650d 0a2a   the syllable..*
-00000d00: 2060 7374 7269 7060 202d 2072 656d 6f76   `strip` - remov
-00000d10: 6573 2061 6e79 2074 6f6e 6520 6d61 726b  es any tone mark
-00000d20: 696e 670d 0a0d 0a7c 2074 6578 7420 7c20  ing....| text | 
-00000d30: 6d61 726b 2020 2020 7c20 6e75 6d62 6572  mark    | number
-00000d40: 2020 2020 7c20 7374 7269 7020 2020 7c0d      | strip   |.
-00000d50: 0a7c 202d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  .| ---- | ------
-00000d60: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20 7c20  - | --------- | 
-00000d70: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e5 8fb0  ------- |..| ...
-00000d80: e781 a320 7c20 54c3 a269 2d75 c3a2 6e20  ... | T..i-u..n 
-00000d90: 7c20 5461 6935 2d75 616e 3520 7c20 5461  | Tai5-uan5 | Ta
-00000da0: 692d 7561 6e20 7c0d 0a0d 0a23 2323 2320  i-uan |....#### 
-00000db0: 4465 6c69 6d69 7465 720d 0a0d 0a60 6465  Delimiter....`de
-00000dc0: 6c69 6d69 7465 7260 2053 7472 696e 6720  limiter` String 
-00000dd0: 2d20 7365 7473 2074 6865 2064 656c 696d  - sets the delim
-00000de0: 6974 6572 2063 6861 7261 6374 6572 2074  iter character t
-00000df0: 6861 7420 7769 6c6c 2062 6520 706c 6163  hat will be plac
-00000e00: 6564 2069 6e20 6265 7477 6565 6e20 7379  ed in between sy
-00000e10: 6c6c 6162 6c65 7320 6f66 2061 2077 6f72  llables of a wor
-00000e20: 642e 0d0a 0d0a 4465 6661 756c 7420 7661  d.....Default va
-00000e30: 6c75 6520 6465 7065 6e64 7320 6f6e 2074  lue depends on t
-00000e40: 6865 2063 686f 7365 6e20 6073 7973 7465  he chosen `syste
-00000e50: 6d60 3a0d 0a0d 0a2a 2060 272d 2760 202d  m`:....* `'-'` -
-00000e60: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
-00000e70: 4f4a 602c 2060 546f 6e67 696f 6e67 600d  OJ`, `Tongiong`.
-00000e80: 0a2a 2060 2727 6020 2d20 666f 7220 6050  .* `''` - for `P
-00000e90: 696e 6779 696d 600d 0a2a 2060 2720 2760  ingyim`..* `' '`
-00000ea0: 202d 2066 6f72 2060 5a68 7579 696e 602c   - for `Zhuyin`,
-00000eb0: 2060 544c 5041 602c 2060 4950 4160 0d0a   `TLPA`, `IPA`..
-00000ec0: 0d0a 7c20 7465 7874 207c 2027 2d27 2020  ..| text | '-'  
-00000ed0: 2020 207c 2027 2720 2020 2020 7c20 2720     | ''     | ' 
-00000ee0: 2720 2020 2020 7c0d 0a7c 202d 2d2d 2d20  '     |..| ---- 
-00000ef0: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
-00000f00: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
-00000f10: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
-00000f20: 75c3 a26e 207c 2054 c3a2 6975 c3a2 6e20  u..n | T..iu..n 
-00000f30: 7c20 54c3 a269 2075 c3a2 6e20 7c0d 0a0d  | T..i u..n |...
-00000f40: 0a23 2323 2320 5361 6e64 6869 0d0a 0d0a  .#### Sandhi....
-00000f50: 6073 616e 6468 6960 2053 7472 696e 6720  `sandhi` String 
-00000f60: 2d20 6170 706c 6965 7320 7468 6520 5b73  - applies the [s
-00000f70: 616e 6468 6920 7275 6c65 7320 6f66 2054  andhi rules of T
-00000f80: 6169 7761 6e65 7365 2048 6f6b 6b69 656e  aiwanese Hokkien
-00000f90: 5d5b 7361 6e64 6869 2d77 696b 695d 2074  ][sandhi-wiki] t
-00000fa0: 6f20 7379 6c6c 6162 6c65 7320 6f66 2061  o syllables of a
-00000fb0: 2073 696e 676c 6520 776f 7264 2e0d 0a0d   single word....
-00000fc0: 0a53 696e 6365 2069 7427 7320 6469 6666  .Since it's diff
-00000fd0: 6963 756c 7420 746f 2065 6e63 6f64 6520  icult to encode 
-00000fe0: 616c 6c20 7361 6e64 6869 2072 756c 6573  all sandhi rules
-00000ff0: 2c20 5461 6962 756e 2070 726f 7669 6465  , Taibun provide
-00001000: 7320 6d75 6c74 6970 6c65 206d 6f64 6573  s multiple modes
-00001010: 2066 6f72 2073 616e 6468 6920 636f 6e76   for sandhi conv
-00001020: 6572 7369 6f6e 2074 6f20 616c 6c6f 7720  ersion to allow 
-00001030: 666f 7220 6375 7374 6f6d 6973 6564 2073  for customised s
-00001040: 616e 6468 6920 6861 6e64 6c69 6e67 2e0d  andhi handling..
-00001050: 0a0d 0a2a 2060 6e6f 6e65 6020 2d20 646f  ...* `none` - do
-00001060: 6573 6e27 7420 7065 7266 6f72 6d20 616e  esn't perform an
-00001070: 7920 746f 6e65 2073 616e 6468 690d 0a2a  y tone sandhi..*
-00001080: 2060 6175 746f 6020 2d20 636c 6f73 6573   `auto` - closes
-00001090: 7420 6170 7072 6f78 696d 6174 696f 6e20  t approximation 
-000010a0: 746f 2066 756c 6c20 636f 7272 6563 7420  to full correct 
-000010b0: 746f 6e65 2073 616e 6468 6920 6f66 2054  tone sandhi of T
-000010c0: 6169 7761 6e65 7365 2c20 7769 7468 2070  aiwanese, with p
-000010d0: 726f 7065 7220 7361 6e64 6869 206f 6620  roper sandhi of 
-000010e0: 7072 6f6e 6f75 6e73 2c20 7375 6666 6978  pronouns, suffix
-000010f0: 6573 2c20 616e 6420 776f 7264 7320 7769  es, and words wi
-00001100: 7468 20e4 bb94 0d0a 2a20 6065 7863 5f6c  th .....* `exc_l
-00001110: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
-00001120: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
-00001130: 6c6c 6162 6c65 2065 7863 6570 7420 666f  llable except fo
-00001140: 7220 7468 6520 6c61 7374 206f 6e65 0d0a  r the last one..
-00001150: 2a20 6069 6e63 6c5f 6c61 7374 6020 2d20  * `incl_last` - 
-00001160: 6368 616e 6765 7320 746f 6e65 2066 6f72  changes tone for
-00001170: 2065 7665 7279 2073 796c 6c61 626c 6520   every syllable 
-00001180: 696e 636c 7564 696e 6720 7468 6520 6c61  including the la
-00001190: 7374 206f 6e65 0d0a 0d0a 4465 6661 756c  st one....Defaul
-000011a0: 7420 7661 6c75 6520 6465 7065 6e64 7320  t value depends 
-000011b0: 6f6e 2074 6865 2063 686f 7365 6e20 6073  on the chosen `s
-000011c0: 7973 7465 6d60 3a0d 0a0d 0a2a 2060 6175  ystem`:....* `au
-000011d0: 746f 6020 2d20 666f 7220 6054 6f6e 6769  to` - for `Tongi
-000011e0: 6f6e 6760 0d0a 2a20 606e 6f6e 6560 202d  ong`..* `none` -
-000011f0: 2066 6f72 2060 5461 696c 6f60 2c20 6050   for `Tailo`, `P
-00001200: 4f4a 602c 2060 5a68 7579 696e 602c 2060  OJ`, `Zhuyin`, `
-00001210: 544c 5041 602c 2060 5069 6e67 7969 6d60  TLPA`, `Pingyim`
-00001220: 2c20 6049 5041 600d 0a0d 0a7c 2074 6578  , `IPA`....| tex
-00001230: 7420 2020 2020 2020 2020 7c20 6e6f 6e65  t         | none
-00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
-00001260: 2020 2020 2020 2020 7c20 6578 635f 6c61          | exc_la
-00001270: 7374 2020 2020 2020 2020 2020 2020 207c  st             |
-00001280: 2069 6e63 6c5f 6c61 7374 2020 2020 2020   incl_last      
-00001290: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
-000012a0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
-000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-000012c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000012d0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-000012e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d  ------------ | -
-000012f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001300: 2d2d 2d20 7c0d 0a7c 20e9 8099 e698 afe5  --- |..| .......
-00001310: 8fb0 e781 a3e5 9ba1 e4bb 9420 7c20 5473  ........... | Ts
-00001320: 6520 73c4 ab20 54c3 a269 2d75 c3a2 6e20  e s.. T..i-u..n 
-00001330: 67c3 ad6e 2dc3 a120 7c20 5473 6520 73c3  g..n-.. | Tse s.
-00001340: ac20 54c4 8169 2d75 c481 6e20 6769 6e2d  . T..i-u..n gin-
-00001350: c3a1 207c 2054 73c4 9320 73c3 ac20 54c4  .. | Ts.. s.. T.
-00001360: 8169 2d75 c481 6e20 6769 6e2d c3a1 207c  .i-u..n gin-.. |
-00001370: 2054 73c4 9320 73c3 ac20 54c4 8169 2d75   Ts.. s.. T..i-u
-00001380: c481 6e20 6769 6e2d 6120 7c0d 0a0d 0a53  ..n gin-a |....S
-00001390: 616e 6468 6920 7275 6c65 7320 616c 736f  andhi rules also
-000013a0: 2063 6861 6e67 6520 6465 7065 6e64 696e   change dependin
-000013b0: 6720 6f6e 2074 6865 2064 6961 6c65 6374  g on the dialect
-000013c0: 2063 686f 7365 6e2e 0d0a 0d0a 7c20 7465   chosen.....| te
-000013d0: 7874 207c 206e 6f20 7361 6e64 6869 207c  xt | no sandhi |
-000013e0: 2073 6f75 7468 2020 207c 206e 6f72 7468   south   | north
-000013f0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
-00001400: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
-00001410: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
-00001420: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
-00001430: 75c3 a26e 2020 207c 2054 c481 692d 75c3  u..n   | T..i-u.
-00001440: a26e 207c 2054 c3a0 692d 75c3 a26e 207c  .n | T..i-u..n |
-00001450: 0d0a 0d0a 2323 2323 2050 756e 6374 7561  ....#### Punctua
-00001460: 7469 6f6e 0d0a 0d0a 6070 756e 6374 7561  tion....`punctua
-00001470: 7469 6f6e 6020 5374 7269 6e67 0d0a 0d0a  tion` String....
-00001480: 2a20 6066 6f72 6d61 7460 2028 6465 6661  * `format` (defa
-00001490: 756c 7429 202d 2063 6f6e 7665 7274 7320  ult) - converts 
-000014a0: 4368 696e 6573 652d 7374 796c 6520 7075  Chinese-style pu
-000014b0: 6e63 7475 6174 696f 6e20 746f 204c 6174  nctuation to Lat
-000014c0: 696e 2d73 7479 6c65 2070 756e 6374 7561  in-style punctua
-000014d0: 7469 6f6e 2061 6e64 2063 6170 6974 616c  tion and capital
-000014e0: 6973 6573 2077 6f72 6473 2061 7420 7468  ises words at th
-000014f0: 6520 6265 6769 6e6e 696e 6720 6f66 2065  e beginning of e
-00001500: 6163 6820 7365 6e74 656e 6365 2e0d 0a2a  ach sentence...*
-00001510: 2060 6e6f 6e65 6020 2d20 7072 6573 6572   `none` - preser
-00001520: 7665 7320 4368 696e 6573 652d 7374 796c  ves Chinese-styl
-00001530: 6520 7075 6e63 7475 6174 696f 6e20 616e  e punctuation an
-00001540: 6420 646f 6573 6e27 7420 6361 7069 7461  d doesn't capita
-00001550: 6c69 7365 2077 6f72 6473 2061 7420 7468  lise words at th
-00001560: 6520 6265 6769 6e6e 696e 6720 6f66 206e  e beginning of n
-00001570: 6577 2073 656e 7465 6e63 6573 2e0d 0a0d  ew sentences....
-00001580: 0a7c 2074 6578 7420 2020 2020 2020 2020  .| text         
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 7c20 666f 726d 6174 2020 2020 2020    | format      
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 7c20 6e6f 6e65 2020 2020        | none    
-00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-000016a0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
-000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016f0: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
-00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001750: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
-00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000017a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000017b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c  ----------- |..|
-000017c0: 20e9 8099 e698 afe8 87ba e58d 97ef bc8c   ...............
-000017d0: e7b0 a1e7 a8b1 e380 8ce5 8d97 e380 8def  ................
-000017e0: bc88 e799 bde8 a9b1 e5ad 97ef bc9a 54c3  ..............T.
-000017f0: a269 2d6c c3a2 6def bc9b e6b3 a8e9 9fb3  .i-l..m.........
-00001800: e7ac a6e8 999f efbc 9ae3 848a e384 9ecb  ................
-00001810: 8a20 e384 8be3 84a2 cb8a efbc 8ce5 9c8b  . ..............
-00001820: e8aa 9eef bc9a 54c3 a169 6ec3 a16e efbc  ......T..in..n..
-00001830: 89e3 8082 207c 2054 7365 2073 c4ab 2054  .... | Tse s.. T
-00001840: c3a2 692d 6cc3 a26d 2c20 6bc3 a16e 2d74  ..i-l..m, k..n-t
-00001850: 7368 696e 6720 226c c3a2 6d22 2028 5065  shing "l..m" (Pe
-00001860: cc8d 682d 75c4 932d 6ac4 ab3a 2054 c3a2  ..h-u..-j..: T..
-00001870: 692d 6cc3 a26d 3b20 7473 c3b9 2d69 6d20  i-l..m; ts..-im 
-00001880: 68c3 bb2d 68c5 8d3a 20e3 848a e384 9ecb  h..-h..: .......
-00001890: 8a20 e384 8be3 84a2 cb8a 2c20 6b6f 6b2d  . ........, kok-
-000018a0: 67c3 ad3a 2054 c3a1 696e c3a1 6e29 2e20  g..: T..in..n). 
-000018b0: 7c20 7473 6520 73c4 ab20 54c3 a269 2d6c  | tse s.. T..i-l
-000018c0: c3a2 6def bc8c 6bc3 a16e 2d74 7368 696e  ..m...k..n-tshin
-000018d0: 67e3 808c 6cc3 a26d e380 8def bc88 5065  g...l..m......Pe
-000018e0: cc8d 682d 75c4 932d 6ac4 abef bc9a 54c3  ..h-u..-j.....T.
-000018f0: a269 2d6c c3a2 6def bc9b 7473 c3b9 2d69  .i-l..m...ts..-i
-00001900: 6d20 68c3 bb2d 68c5 8def bc9a e384 8ae3  m h..-h.........
-00001910: 849e cb8a 20e3 848b e384 a2cb 8aef bc8c  .... ...........
-00001920: 6b6f 6b2d 67c3 adef bc9a 54c3 a169 6ec3  kok-g.....T..in.
-00001930: a16e efbc 89e3 8082 207c 0d0a 0d0a 2323  .n...... |....##
-00001940: 2323 2043 6f6e 7665 7274 206e 6f6e 2d43  ## Convert non-C
-00001950: 4a4b 0d0a 0d0a 6063 6f6e 7665 7274 5f6e  JK....`convert_n
-00001960: 6f6e 5f63 6a6b 6020 426f 6f6c 6561 6e20  on_cjk` Boolean 
-00001970: 2d20 6465 6669 6e65 7320 7768 6574 6865  - defines whethe
-00001980: 7220 6f72 206e 6f74 2074 6f20 636f 6e76  r or not to conv
-00001990: 6572 7420 6e6f 6e2d 4368 696e 6573 6520  ert non-Chinese 
-000019a0: 776f 7264 732e 2043 616e 2062 6520 7573  words. Can be us
-000019b0: 6564 2074 6f20 636f 6e76 6572 7420 5461  ed to convert Ta
-000019c0: 696c 6f20 746f 2061 6e6f 7468 6572 2072  ilo to another r
-000019d0: 6f6d 616e 6973 6174 696f 6e20 7379 7374  omanisation syst
-000019e0: 656d 2e0d 0a0d 0a2a 2060 5472 7565 6020  em.....* `True` 
-000019f0: 2d20 636f 6e76 6572 7420 6e6f 6e2d 4368  - convert non-Ch
-00001a00: 696e 6573 6520 6368 6172 6163 7465 7220  inese character 
-00001a10: 776f 7264 730d 0a2a 2060 4661 6c73 6560  words..* `False`
-00001a20: 2028 6465 6661 756c 7429 202d 2063 6f6e   (default) - con
-00001a30: 7665 7274 206f 6e6c 7920 4368 696e 6573  vert only Chines
-00001a40: 6520 6368 6172 6163 7465 7220 776f 7264  e character word
-00001a50: 730d 0a0d 0a7c 2074 6578 7420 2020 2020  s....| text     
-00001a60: 207c 2046 616c 7365 2020 2020 2020 2020   | False        
-00001a70: 2020 2020 2020 2020 2020 207c 2054 7275             | Tru
-00001a80: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00001a90: 2020 2020 207c 0d0a 7c20 2d2d 2d2d 2d2d       |..| ------
-00001aa0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
-00001ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
-00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ad0: 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 20e6 8891  ------- |..| ...
-00001ae0: e9a3 9f70 68c3 a16e 6720 7c20 e386 a3e3  ...ph..ng | ....
-00001af0: 84a8 e384 9acb 8b20 e384 90e3 84a7 e384  ....... ........
-00001b00: 9ae3 86b7 cb99 2070 68c3 a16e 6720 7c20  ...... ph..ng | 
-00001b10: e386 a3e3 84a8 e384 9acb 8b20 e384 90e3  ........... ....
-00001b20: 84a7 e384 9ae3 86b7 cb99 20e3 8486 e384  .......... .....
-00001b30: a4cb 8b20 7c0d 0a0d 0a23 2323 2054 6f6b  ... |....### Tok
-00001b40: 656e 6973 6572 0d0a 0d0a 6054 6f6b 656e  eniser....`Token
-00001b50: 6973 6572 6020 636c 6173 7320 7065 7266  iser` class perf
-00001b60: 6f72 6d73 205b 4e4c 544b 2077 6f72 6470  orms [NLTK wordp
-00001b70: 756e 6374 5f74 6f6b 656e 697a 655d 5b6e  unct_tokenize][n
-00001b80: 6c74 6b2d 746f 6b65 6e69 7a65 5d2d 6c69  ltk-tokenize]-li
-00001b90: 6b65 2074 6f6b 656e 6973 6174 696f 6e20  ke tokenisation 
-00001ba0: 6f66 2061 2054 6169 7761 6e65 7365 2048  of a Taiwanese H
-00001bb0: 6f6b 6b69 656e 2073 656e 7465 6e63 652e  okkien sentence.
-00001bc0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
-00001bd0: 2063 6f6e 7374 7275 6374 6f72 0d0a 7420   constructor..t 
-00001be0: 3d20 546f 6b65 6e69 7365 7228 290d 0a0d  = Tokeniser()...
-00001bf0: 0a23 2074 6f6b 656e 6973 6520 5461 6977  .# tokenise Taiw
-00001c00: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
-00001c10: 6e74 656e 6365 0d0a 742e 746f 6b65 6e69  ntence..t.tokeni
-00001c20: 7365 2869 6e70 7574 290d 0a60 6060 0d0a  se(input)..```..
-00001c30: 0d0a 2323 2320 4f74 6865 7220 4675 6e63  ..### Other Func
-00001c40: 7469 6f6e 730d 0a0d 0a60 6060 7079 7468  tions....```pyth
-00001c50: 6f6e 0d0a 2320 436f 6e76 6572 7420 746f  on..# Convert to
-00001c60: 2054 7261 6469 7469 6f6e 616c 0d0a 746f   Traditional..to
-00001c70: 5f74 7261 6469 7469 6f6e 616c 2869 6e70  _traditional(inp
-00001c80: 7574 290d 0a0d 0a23 2043 6f6e 7665 7274  ut)....# Convert
-00001c90: 2074 6f20 5369 6d70 6c69 6669 6564 0d0a   to Simplified..
-00001ca0: 746f 5f73 696d 706c 6966 6965 6428 696e  to_simplified(in
-00001cb0: 7075 7429 0d0a 0d0a 2320 4368 6563 6b20  put)....# Check 
-00001cc0: 6966 2074 6865 2073 7472 696e 6720 6973  if the string is
-00001cd0: 2066 756c 6c79 2063 6f6d 706f 7365 6420   fully composed 
-00001ce0: 6f66 2043 6869 6e65 7365 2063 6861 7261  of Chinese chara
-00001cf0: 6374 6572 730d 0a69 735f 636a 6b28 696e  cters..is_cjk(in
-00001d00: 7075 7429 0d0a 6060 600d 0a0d 0a0d 0a0d  put)..```.......
-00001d10: 0a3c 212d 2d20 4558 414d 504c 4520 2d2d  .<!-- EXAMPLE --
-00001d20: 3e0d 0a23 2320 4578 616d 706c 650d 0a0d  >..## Example...
-00001d30: 0a60 6060 7079 7468 6f6e 0d0a 2320 436f  .```python..# Co
-00001d40: 6e76 6572 7465 720d 0a66 726f 6d20 7461  nverter..from ta
-00001d50: 6962 756e 2069 6d70 6f72 7420 436f 6e76  ibun import Conv
-00001d60: 6572 7465 720d 0a0d 0a23 2320 5379 7374  erter....## Syst
-00001d70: 656d 0d0a 6320 3d20 436f 6e76 6572 7465  em..c = Converte
-00001d80: 7228 2920 2320 5461 696c 6f20 7379 7374  r() # Tailo syst
-00001d90: 656d 2064 6566 6175 6c74 0d0a 632e 6765  em default..c.ge
-00001da0: 7428 27e5 8588 e794 9fe8 ac9b efbc 8ce5  t('.............
-00001db0: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
-00001dc0: 8227 290d 0a3e 3e20 5369 616e 2d73 696e  .')..>> Sian-sin
-00001dd0: 6e20 6bc3 b36e 672c 2068 61cc 8d6b 2d73  n k..ng, ha..k-s
-00001de0: 696e 6720 7469 c481 6d2d 7469 c481 6d20  ing ti..m-ti..m 
-00001df0: 7468 6961 6e6e 2e0d 0a0d 0a63 203d 2043  thiann.....c = C
-00001e00: 6f6e 7665 7274 6572 2873 7973 7465 6d3d  onverter(system=
-00001e10: 275a 6875 7969 6e27 290d 0a63 2e67 6574  'Zhuyin')..c.get
-00001e20: 2827 e585 88e7 949f e8ac 9bef bc8c e5ad  ('..............
-00001e30: b8e7 949f e681 ace6 81ac e881 bde3 8082  ................
-00001e40: 2729 0d0a 3e3e 20e3 8492 e384 a7e3 84a2  ')..>> .........
-00001e50: 20e3 8492 e386 aa20 e384 8de3 86b2 cb8b   ...... ........
-00001e60: 2c20 e384 8fe3 849a e386 b6cb 9920 e384  , ........... ..
-00001e70: 92e3 84a7 e384 a520 e384 89e3 84a7 e386  ....... ........
-00001e80: b0cb ab20 e384 89e3 84a7 e386 b0cb ab20  ... ........... 
-00001e90: e384 8ae3 84a7 e386 a92e 0d0a 0d0a 2323  ..............##
-00001ea0: 2044 6961 6c65 6374 0d0a 6320 3d20 436f   Dialect..c = Co
-00001eb0: 6e76 6572 7465 7228 2920 2320 736f 7574  nverter() # sout
-00001ec0: 6820 6469 616c 6563 7420 6465 6661 756c  h dialect defaul
-00001ed0: 740d 0a63 2e67 6574 2822 e688 91e6 acb2  t..c.get("......
-00001ee0: e794 a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a  ............")..
-00001ef0: 3e3e 2047 75c3 a120 6265 6820 c4ab 6e67  >> Gu.. beh ..ng
-00001f00: 2074 c4ab 2074 7369 61cc 8d68 2068 c3ae   t.. tsia..h h..
-00001f10: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001f20: 7228 6469 616c 6563 743d 276e 6f72 7468  r(dialect='north
-00001f30: 2729 0d0a 632e 6765 7428 22e6 8891 e6ac  ')..c.get(".....
-00001f40: b2e7 94a8 e7ae b8e9 a39f e9ad 9a22 290d  .............").
-00001f50: 0a3e 3e20 4775 c3a1 2062 7565 6820 c4ab  .>> Gu.. bueh ..
-00001f60: 6e67 2074 c5ab 2074 7369 61cc 8d68 2068  ng t.. tsia..h h
-00001f70: c3bb 0d0a 0d0a 2323 2046 6f72 6d61 740d  ......## Format.
-00001f80: 0a63 203d 2043 6f6e 7665 7274 6572 2829  .c = Converter()
-00001f90: 2023 2066 6f72 2054 6169 6c6f 2c20 6d61   # for Tailo, ma
-00001fa0: 726b 2062 7920 6465 6661 756c 740d 0a63  rk by default..c
-00001fb0: 2e67 6574 2822 e794 9fe6 97a5 e5bf abe6  .get("..........
-00001fc0: a882 2229 0d0a 3e3e 2053 656e 6e2d 6a69  ..")..>> Senn-ji
-00001fd0: cc8d 7420 6b68 75c3 a069 2d6c 6fcc 8d6b  ..t khu..i-lo..k
-00001fe0: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00001ff0: 7228 666f 726d 6174 3d27 6e75 6d62 6572  r(format='number
-00002000: 2729 0d0a 632e 6765 7428 22e7 949f e697  ')..c.get(".....
-00002010: a5e5 bfab e6a8 8222 290d 0a3e 3e20 5365  .......")..>> Se
-00002020: 6e6e 312d 6a69 7438 206b 6875 6169 332d  nn1-jit8 khuai3-
-00002030: 6c6f 6b38 0d0a 0d0a 6320 3d20 436f 6e76  lok8....c = Conv
-00002040: 6572 7465 7228 666f 726d 6174 3d27 7374  erter(format='st
-00002050: 7269 7027 290d 0a63 2e67 6574 2822 e794  rip')..c.get("..
-00002060: 9fe6 97a5 e5bf abe6 a882 2229 0d0a 3e3e  ..........")..>>
-00002070: 2053 656e 6e2d 6a69 7420 6b68 7561 692d   Senn-jit khuai-
-00002080: 6c6f 6b0d 0a0d 0a23 2320 4465 6c69 6d69  lok....## Delimi
-00002090: 7465 720d 0a63 203d 2043 6f6e 7665 7274  ter..c = Convert
-000020a0: 6572 2864 656c 696d 6974 6572 3d27 2729  er(delimiter='')
-000020b0: 0d0a 632e 6765 7428 22e5 8588 e794 9fe8  ..c.get(".......
-000020c0: ac9b efbc 8ce5 adb8 e794 9fe6 81ac e681  ................
-000020d0: ace8 81bd e380 8222 290d 0a3e 3e20 5369  .......")..>> Si
-000020e0: 616e 7369 6e6e 206b c3b3 6e67 2c20 6861  ansinn k..ng, ha
-000020f0: cc8d 6b73 696e 6720 7469 c481 6d74 69c4  ..ksing ti..mti.
-00002100: 816d 2074 6869 616e 6e2e 0d0a 0d0a 6320  .m thiann.....c 
-00002110: 3d20 436f 6e76 6572 7465 7228 7379 7374  = Converter(syst
-00002120: 656d 3d27 5069 6e67 7969 6d27 2c20 6465  em='Pingyim', de
-00002130: 6c69 6d69 7465 723d 272d 2729 0d0a 632e  limiter='-')..c.
-00002140: 6765 7428 22e5 8588 e794 9fe8 ac9b efbc  get("...........
-00002150: 8ce5 adb8 e794 9fe6 81ac e681 ace8 81bd  ................
-00002160: e380 8222 290d 0a3e 3e20 5369 c481 6e2d  ...")..>> Si..n-
-00002170: 736e c4ab 2067 c792 6e67 2c20 68c3 a167  sn.. g..ng, h..g
-00002180: 2d73 c4ab 6e67 2064 69c3 a26d 2d64 69c3  -s..ng di..m-di.
-00002190: a26d 2074 696e c481 2e0d 0a0d 0a23 2320  .m tin.......## 
-000021a0: 5361 6e64 6869 0d0a 6320 3d20 436f 6e76  Sandhi..c = Conv
-000021b0: 6572 7465 7228 2920 2320 666f 7220 5461  erter() # for Ta
-000021c0: 696c 6f2c 2073 616e 6468 6920 6e6f 6e65  ilo, sandhi none
-000021d0: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
-000021e0: 6574 2822 e980 99e6 98af e58f b0e7 81a3  et("............
-000021f0: e59b a1e4 bb94 2229 0d0a 3e3e 2054 7365  ......")..>> Tse
-00002200: 2073 c4ab 2054 c3a2 692d 75c3 a26e 2067   s.. T..i-u..n g
-00002210: c3ad 6e2d c3a1 0d0a 0d0a 6320 3d20 436f  ..n-......c = Co
-00002220: 6e76 6572 7465 7228 7361 6e64 6869 3d27  nverter(sandhi='
-00002230: 6175 746f 2729 0d0a 632e 6765 7428 22e9  auto')..c.get(".
-00002240: 8099 e698 afe5 8fb0 e781 a3e5 9ba1 e4bb  ................
-00002250: 9422 290d 0a3e 3e20 5473 6520 73c3 ac20  .")..>> Tse s.. 
-00002260: 54c4 8169 2d75 c481 6e20 6769 6e2d c3a1  T..i-u..n gin-..
-00002270: 0d0a 0d0a 6320 3d20 436f 6e76 6572 7465  ....c = Converte
-00002280: 7228 7361 6e64 6869 3d27 6578 635f 6c61  r(sandhi='exc_la
-00002290: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
-000022a0: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
-000022b0: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
-000022c0: c481 692d 75c4 816e 2067 696e 2dc3 a10d  ..i-u..n gin-...
-000022d0: 0a0d 0a63 203d 2043 6f6e 7665 7274 6572  ...c = Converter
-000022e0: 2873 616e 6468 693d 2769 6e63 6c5f 6c61  (sandhi='incl_la
-000022f0: 7374 2729 0d0a 632e 6765 7428 22e9 8099  st')..c.get("...
-00002300: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
-00002310: 290d 0a3e 3e20 5473 c493 2073 c3ac 2054  )..>> Ts.. s.. T
-00002320: c481 692d 75c4 816e 2067 696e 2d61 0d0a  ..i-u..n gin-a..
-00002330: 0d0a 2323 2050 756e 6374 7561 7469 6f6e  ..## Punctuation
-00002340: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
-00002350: 2920 2320 666f 726d 6174 2070 756e 6374  ) # format punct
-00002360: 7561 7469 6f6e 2064 6566 6175 6c74 0d0a  uation default..
-00002370: 632e 6765 7428 22e5 a4aa e7a9 bae6 9c8b  c.get(".........
-00002380: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
-00002390: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
-000023a0: 0d0a 3e3e 2054 68c3 a069 2d6b 686f 6e67  ..>> Th..i-khong
-000023b0: 2070 c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e   p..ng-i.., l..n
-000023c0: 2d68 c3b3 2120 4cc3 ad6e 2074 7369 61cc  -h..! L..n tsia.
-000023d0: 8d68 2d70 c3a1 2062 75c4 933f 0d0a 0d0a  .h-p.. bu..?....
-000023e0: 6320 3d20 436f 6e76 6572 7465 7228 7075  c = Converter(pu
-000023f0: 6e63 7475 6174 696f 6e3d 276e 6f6e 6527  nctuation='none'
-00002400: 290d 0a63 2e67 6574 2822 e5a4 aae7 a9ba  )..c.get("......
-00002410: e69c 8be5 8f8b efbc 8ce6 8181 e5a5 bdef  ................
-00002420: bc81 e681 81e9 a39f e9a3 bde6 9caa efbc  ................
-00002430: 9f22 290d 0a3e 3e20 7468 c3a0 692d 6b68  .")..>> th..i-kh
-00002440: 6f6e 6720 70c3 ae6e 672d 69c3 baef bc8c  ong p..ng-i.....
-00002450: 6cc3 ad6e 2d68 c3b3 efbc 816c c3ad 6e20  l..n-h.....l..n 
-00002460: 7473 6961 cc8d 682d 70c3 a120 6275 c493  tsia..h-p.. bu..
-00002470: efbc 9f0d 0a0d 0a23 2320 436f 6e76 6572  .......## Conver
-00002480: 7420 6e6f 6e2d 434a 4b0d 0a63 203d 2043  t non-CJK..c = C
-00002490: 6f6e 7665 7274 2873 7973 7465 6d3d 275a  onvert(system='Z
-000024a0: 6875 7969 6e27 2920 2320 4661 6c73 6520  huyin') # False 
-000024b0: 636f 6e76 6572 745f 6e6f 6e5f 636a 6b20  convert_non_cjk 
-000024c0: 6465 6661 756c 740d 0a63 2e67 6574 2822  default..c.get("
-000024d0: e688 91e9 a39f 7068 c3a1 6e67 2229 0d0a  ......ph..ng")..
-000024e0: 3e3e 20e3 86a3 e384 a8e3 849a cb8b 20e3  >> ........... .
-000024f0: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
-00002500: c3a1 6e67 0d0a 0d0a 6320 3d20 436f 6e76  ..ng....c = Conv
-00002510: 6572 7428 7379 7374 656d 3d27 5a68 7579  ert(system='Zhuy
-00002520: 696e 272c 2063 6f6e 7665 7274 5f6e 6f6e  in', convert_non
-00002530: 5f63 6a6b 3d54 7275 6529 0d0a 632e 6765  _cjk=True)..c.ge
-00002540: 7428 22e6 8891 e9a3 9f70 68c3 a16e 6722  t("......ph..ng"
-00002550: 290d 0a3e 3e20 e386 a3e3 84a8 e384 9acb  )..>> ..........
-00002560: 8b20 e384 90e3 84a7 e384 9ae3 86b7 cb99  . ..............
-00002570: 20e3 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23   ..............#
-00002580: 2054 6f6b 656e 6973 6572 0d0a 6672 6f6d   Tokeniser..from
-00002590: 2074 6169 6275 6e20 696d 706f 7274 2054   taibun import T
-000025a0: 6f6b 656e 6973 6572 0d0a 0d0a 7420 3d20  okeniser....t = 
-000025b0: 546f 6b65 6e69 7365 7228 290d 0a74 2e74  Tokeniser()..t.t
-000025c0: 6f6b 656e 6973 6528 22e5 a4aa e7a9 bae6  okenise(".......
-000025d0: 9c8b e58f 8bef bc8c e681 81e5 a5bd efbc  ................
-000025e0: 81e6 8181 e9a3 9fe9 a3bd e69c aaef bc9f  ................
-000025f0: 2229 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27  ")..>> ['......'
-00002600: 2c20 27e6 9c8b e58f 8b27 2c20 27ef bc8c  , '......', '...
-00002610: 272c 2027 e681 81e5 a5bd 272c 2027 efbc  ', '......', '..
-00002620: 8127 2c20 27e6 8181 272c 2027 e9a3 9fe9  .', '...', '....
-00002630: a3bd 272c 2027 e69c aa27 2c20 27ef bc9f  ..', '...', '...
-00002640: 275d 0d0a 0d0a 0d0a 2320 4f74 6865 7220  ']......# Other 
-00002650: 4675 6e63 7469 6f6e 730d 0a66 726f 6d20  Functions..from 
-00002660: 7461 6962 756e 2069 6d70 6f72 7420 746f  taibun import to
-00002670: 5f74 7261 6469 7469 6f6e 616c 2c20 746f  _traditional, to
-00002680: 5f73 696d 706c 6966 6965 642c 2069 735f  _simplified, is_
-00002690: 636a 6b0d 0a0d 0a74 6f5f 7472 6164 6974  cjk....to_tradit
-000026a0: 696f 6e61 6c28 22e6 8891 e590 ace6 97a0  ional(".........
-000026b0: e58f b0e6 b9be e8af 9d22 290d 0a3e 3e20  .........")..>> 
-000026c0: e688 91e8 81bd e784 a1e5 8fb0 e781 a3e8  ................
-000026d0: a9b1 0d0a 0d0a 746f 5f73 696d 706c 6966  ......to_simplif
-000026e0: 6965 6428 22e6 8891 e881 bde7 84a1 e887  ied("...........
-000026f0: bae7 81a3 e8a9 b122 290d 0a3e 3e20 e688  .......")..>> ..
-00002700: 91e5 90ac e697 a0e5 8fb0 e6b9 bee8 af9d  ................
-00002710: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
-00002720: a39f e9ba ad27 290d 0a3e 3e20 5472 7565  .....')..>> True
-00002730: 0d0a 0d0a 6973 5f63 6a6b 2827 e688 91e9  ....is_cjk('....
-00002740: a39f 7068 c3a1 6e67 2729 0d0a 3e3e 2046  ..ph..ng')..>> F
-00002750: 616c 7365 0d0a 6060 600d 0a0d 0a0d 0a0d  alse..```.......
-00002760: 0a3c 212d 2d20 4441 5441 202d 2d3e 0d0a  .<!-- DATA -->..
-00002770: 2323 2044 6174 610d 0a0d 0a2d 205b 5461  ## Data....- [Ta
-00002780: 6977 616e 6573 652d 4368 696e 6573 6520  iwanese-Chinese 
-00002790: 4f6e 6c69 6e65 2044 6963 7469 6f6e 6172  Online Dictionar
-000027a0: 795d 5b6f 6e6c 696e 652d 6469 6374 696f  y][online-dictio
-000027b0: 6e61 7279 5d20 2876 6961 205b 4368 686f  nary] (via [Chho
-000027c0: 6554 6169 6769 5d5b 6461 7461 2d76 6961  eTaigi][data-via
-000027d0: 5d29 0d0a 2d20 5b69 5461 6967 6920 4368  ])..- [iTaigi Ch
-000027e0: 696e 6573 652d 5461 6977 616e 6573 6520  inese-Taiwanese 
-000027f0: 436f 6d70 6172 6973 6f6e 2044 6963 7469  Comparison Dicti
-00002800: 6f6e 6172 795d 5b69 7461 6967 692d 6469  onary][itaigi-di
-00002810: 6374 696f 6e61 7279 5d20 2876 6961 205b  ctionary] (via [
-00002820: 4368 686f 6554 6169 6769 5d5b 6461 7461  ChhoeTaigi][data
-00002830: 2d76 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21  -via])........<!
-00002840: 2d2d 2041 434b 4e4f 574c 4544 4745 4d45  -- ACKNOWLEDGEME
-00002850: 4e54 5320 2d2d 3e0d 0a23 2320 4163 6b6e  NTS -->..## Ackn
-00002860: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
-00002870: 2d20 5361 6d75 656c 204a 656e 2028 5b47  - Samuel Jen ([G
-00002880: 6974 6875 625d 5b73 616d 7565 6c2d 6769  ithub][samuel-gi
-00002890: 7468 7562 5d20 c2b7 205b 4c69 6e6b 6564  thub] .. [Linked
-000028a0: 496e 5d5b 7361 6d75 656c 2d6c 696e 6b65  In][samuel-linke
-000028b0: 6469 6e5d 2920 2d20 5461 6977 616e 6573  din]) - Taiwanes
-000028c0: 6520 616e 6420 4d61 6e64 6172 696e 2074  e and Mandarin t
-000028d0: 7261 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a  ranslation......
-000028e0: 0d0a 3c21 2d2d 204c 4943 454e 4345 202d  ..<!-- LICENCE -
-000028f0: 2d3e 0d0a 2323 204c 6963 656e 6365 0d0a  ->..## Licence..
-00002900: 0d0a 4265 6361 7573 6520 5461 6962 756e  ..Because Taibun
-00002910: 2069 7320 4d49 542d 6c69 6365 6e73 6564   is MIT-licensed
-00002920: 2c20 616e 7920 6465 7665 6c6f 7065 7220  , any developer 
-00002930: 6361 6e20 6573 7365 6e74 6961 6c6c 7920  can essentially 
-00002940: 646f 2077 6861 7465 7665 7220 7468 6579  do whatever they
-00002950: 2077 616e 7420 7769 7468 2069 7420 6173   want with it as
-00002960: 206c 6f6e 6720 6173 2074 6865 7920 696e   long as they in
-00002970: 636c 7564 6520 7468 6520 6f72 6967 696e  clude the origin
-00002980: 616c 2063 6f70 7972 6967 6874 2061 6e64  al copyright and
-00002990: 206c 6963 656e 6365 206e 6f74 6963 6520   licence notice 
-000029a0: 696e 2061 6e79 2063 6f70 6965 7320 6f66  in any copies of
-000029b0: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
-000029c0: 2e20 4e6f 7465 2c20 7468 6174 2074 6865  . Note, that the
-000029d0: 2064 6174 6120 7573 6564 2062 7920 7468   data used by th
-000029e0: 6520 7061 636b 6167 6520 6973 206c 6963  e package is lic
-000029f0: 656e 7365 6420 756e 6465 7220 6120 6469  ensed under a di
-00002a00: 6666 6572 656e 7420 636f 7079 7269 6768  fferent copyrigh
-00002a10: 742e 0d0a 0d0a 5468 6520 6461 7461 2069  t.....The data i
-00002a20: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-00002a30: 205b 4343 2042 592d 5341 2034 2e30 5d5b   [CC BY-SA 4.0][
-00002a40: 6461 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a  data-cc]........
-00002a50: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
-00002a60: 4e4b 5320 2d2d 3e0d 0a5b 7465 7374 735d  NKS -->..[tests]
-00002a70: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00002a80: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
-00002a90: 6169 6275 6e2f 6163 7469 6f6e 730d 0a5b  aibun/actions..[
-00002aa0: 7465 7374 732d 6261 6467 655d 3a20 6874  tests-badge]: ht
-00002ab0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00002ac0: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
-00002ad0: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
-00002ae0: 7475 732f 616e 6472 6569 6861 722f 7461  tus/andreihar/ta
-00002af0: 6962 756e 2f63 692e 7961 6d6c 3f73 7479  ibun/ci.yaml?sty
-00002b00: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
-00002b10: 266c 6f67 6f3d 6769 7468 7562 0d0a 5b63  &logo=github..[c
-00002b20: 6f6e 7472 6962 7574 6f72 732d 6261 6467  ontributors-badg
-00002b30: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
-00002b40: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00002b50: 622f 636f 6e74 7269 6275 746f 7273 2f61  b/contributors/a
-00002b60: 6e64 7265 6968 6172 2f74 6169 6275 6e3f  ndreihar/taibun?
-00002b70: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00002b80: 6467 650d 0a5b 636f 6e74 7269 6275 746f  dge..[contributo
-00002b90: 7273 5d3a 2023 7573 6167 650d 0a5b 7265  rs]: #usage..[re
-00002ba0: 6c65 6173 652d 6261 6467 655d 3a20 6874  lease-badge]: ht
-00002bb0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00002bc0: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
-00002bd0: 6c65 6173 652f 616e 6472 6569 6861 722f  lease/andreihar/
-00002be0: 7461 6962 756e 3f63 6f6c 6f72 3d33 3836  taibun?color=386
-00002bf0: 3138 6326 7374 796c 653d 666f 722d 7468  18c&style=for-th
-00002c00: 652d 6261 6467 650d 0a5b 7265 6c65 6173  e-badge..[releas
-00002c10: 655d 3a20 6874 7470 733a 2f2f 6769 7468  e]: https://gith
-00002c20: 7562 2e63 6f6d 2f61 6e64 7265 6968 6172  ub.com/andreihar
-00002c30: 2f74 6169 6275 6e2f 7265 6c65 6173 6573  /taibun/releases
-00002c40: 0d0a 5b6c 6963 656e 6365 2d62 6164 6765  ..[licence-badge
-00002c50: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00002c60: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00002c70: 2f6c 6963 656e 7365 2f61 6e64 7265 6968  /license/andreih
-00002c80: 6172 2f74 6169 6275 6e3f 636f 6c6f 723d  ar/taibun?color=
-00002c90: 3030 3030 3030 2673 7479 6c65 3d66 6f72  000000&style=for
-00002ca0: 2d74 6865 2d62 6164 6765 0d0a 5b6c 6963  -the-badge..[lic
-00002cb0: 656e 6365 5d3a 204c 4943 454e 5345 0d0a  ence]: LICENSE..
-00002cc0: 5b6c 696e 6b65 6469 6e2d 6261 6467 655d  [linkedin-badge]
-00002cd0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00002ce0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00002cf0: 696e 6b65 6449 6e2d 3030 3737 4235 3f73  inkedIn-0077B5?s
-00002d00: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00002d10: 6765 266c 6f67 6f3d 6c69 6e6b 6564 696e  ge&logo=linkedin
-00002d20: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00002d30: 0d0a 5b6c 696e 6b65 6469 6e5d 3a20 6874  ..[linkedin]: ht
-00002d40: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00002d50: 696e 2e63 6f6d 2f69 6e2f 616e 6472 6569  in.com/in/andrei
-00002d60: 2d68 6172 6261 6368 6f76 2f0d 0a0d 0a5b  -harbachov/....[
-00002d70: 7079 7069 5d3a 2068 7474 7073 3a2f 2f70  pypi]: https://p
-00002d80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00002d90: 7461 6962 756e 0d0a 5b62 7567 5d3a 2068  taibun..[bug]: h
-00002da0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002db0: 6d2f 616e 6472 6569 6861 722f 7461 6962  m/andreihar/taib
-00002dc0: 756e 2f69 7373 7565 730d 0a5b 6f6e 6c69  un/issues..[onli
-00002dd0: 6e65 2d64 6963 7469 6f6e 6172 795d 3a20  ne-dictionary]: 
-00002de0: 6874 7470 3a2f 2f69 7031 3934 3039 372e  http://ip194097.
-00002df0: 6e74 6375 2e65 6475 2e74 772f 756e 6769  ntcu.edu.tw/ungi
-00002e00: 616e 2f73 6f61 6e6e 7465 6e67 2f63 6869  an/soannteng/chi
-00002e10: 6c2f 5461 6968 6f61 2e61 7370 0d0a 5b69  l/Taihoa.asp..[i
-00002e20: 7461 6967 692d 6469 6374 696f 6e61 7279  taigi-dictionary
-00002e30: 5d3a 2068 7474 7073 3a2f 2f69 7461 6967  ]: https://itaig
-00002e40: 692e 7477 2f0d 0a5b 6461 7461 2d76 6961  i.tw/..[data-via
-00002e50: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-00002e60: 622e 636f 6d2f 4368 686f 6554 6169 6769  b.com/ChhoeTaigi
-00002e70: 2f43 6868 6f65 5461 6967 6944 6174 6162  /ChhoeTaigiDatab
-00002e80: 6173 650d 0a5b 6461 7461 2d63 635d 3a20  ase..[data-cc]: 
-00002e90: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
-00002ea0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
-00002eb0: 6e73 6573 2f62 792d 7361 2f34 2e30 2f64  nses/by-sa/4.0/d
-00002ec0: 6565 642e 656e 0d0a 5b73 616d 7565 6c2d  eed.en..[samuel-
-00002ed0: 6769 7468 7562 5d3a 2068 7474 7073 3a2f  github]: https:/
-00002ee0: 2f67 6974 6875 622e 636f 6d2f 5353 5361  /github.com/SSSa
-00002ef0: 6d0d 0a5b 7361 6d75 656c 2d6c 696e 6b65  m..[samuel-linke
-00002f00: 6469 6e5d 3a20 6874 7470 733a 2f2f 7777  din]: https://ww
-00002f10: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
-00002f20: 6e2f 7361 6d75 656c 2d6a 656e 2f0d 0a0d  n/samuel-jen/...
-00002f30: 0a5b 7461 696c 6f2d 7769 6b69 5d3a 2068  .[tailo-wiki]: h
-00002f40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00002f50: 6469 612e 6f72 672f 7769 6b69 2f54 2543  dia.org/wiki/T%C
-00002f60: 3325 4132 692d 7525 4333 2541 326e 5f4c  3%A2i-u%C3%A2n_L
-00002f70: 2543 3325 4234 2d6d 2543 3325 4131 2d6a  %C3%B4-m%C3%A1-j
-00002f80: 2543 3425 4142 5f50 6869 6e67 2d69 6d5f  %C4%AB_Phing-im_
-00002f90: 486f 6e67 2d25 4333 2541 306e 0d0a 5b70  Hong-%C3%A0n..[p
-00002fa0: 6f6a 2d77 696b 695d 3a20 6874 7470 733a  oj-wiki]: https:
-00002fb0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002fc0: 7267 2f77 696b 692f 5065 2543 4325 3844  rg/wiki/Pe%CC%8D
-00002fd0: 682d 2543 3525 3844 652d 6a25 4334 2541  h-%C5%8De-j%C4%A
-00002fe0: 420d 0a5b 7a68 7579 696e 2d77 696b 695d  B..[zhuyin-wiki]
-00002ff0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
-00003000: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00003010: 5461 6977 616e 6573 655f 5068 6f6e 6574  Taiwanese_Phonet
-00003020: 6963 5f53 796d 626f 6c73 0d0a 5b74 6c70  ic_Symbols..[tlp
-00003030: 612d 7769 6b69 5d3a 2068 7474 7073 3a2f  a-wiki]: https:/
-00003040: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00003050: 672f 7769 6b69 2f54 6169 7761 6e65 7365  g/wiki/Taiwanese
-00003060: 5f4c 616e 6775 6167 655f 5068 6f6e 6574  _Language_Phonet
-00003070: 6963 5f41 6c70 6861 6265 740d 0a5b 7069  ic_Alphabet..[pi
-00003080: 6e67 7969 6d2d 7769 6b69 5d3a 2068 7474  ngyim-wiki]: htt
-00003090: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000030a0: 612e 6f72 672f 7769 6b69 2f42 6225 4333  a.org/wiki/Bb%C3
-000030b0: 2541 316e 6c25 4333 2541 316d 5f70 2543  %A1nl%C3%A1m_p%C
-000030c0: 3325 4143 6e67 7925 4334 2541 426d 0d0a  3%ACngy%C4%ABm..
-000030d0: 5b74 6f6e 6769 6f6e 672d 7769 6b69 5d3a  [tongiong-wiki]:
-000030e0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
-000030f0: 7065 6469 612e 6f72 672f 7769 6b69 2f44  pedia.org/wiki/D
-00003100: 6125 4334 2541 422d 6768 2543 3325 4145  a%C4%AB-gh%C3%AE
-00003110: 5f74 2543 3525 3844 6e67 2d69 2543 3525  _t%C5%8Dng-i%C5%
-00003120: 3844 6e67 5f70 2543 3425 4142 6e67 2d69  8Dng_p%C4%ABng-i
-00003130: 6d0d 0a5b 6970 612d 7769 6b69 5d3a 2068  m..[ipa-wiki]: h
-00003140: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00003150: 6469 612e 6f72 672f 7769 6b69 2f49 6e74  dia.org/wiki/Int
-00003160: 6572 6e61 7469 6f6e 616c 5f50 686f 6e65  ernational_Phone
-00003170: 7469 635f 416c 7068 6162 6574 0d0a 5b7a  tic_Alphabet..[z
-00003180: 6861 6e67 7a68 6f75 2d77 696b 695d 3a20  hangzhou-wiki]: 
-00003190: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000031a0: 6564 6961 2e6f 7267 2f77 696b 692f 5a68  edia.org/wiki/Zh
-000031b0: 616e 677a 686f 755f 6469 616c 6563 7473  angzhou_dialects
-000031c0: 0d0a 5b71 7561 6e7a 686f 752d 7769 6b69  ..[quanzhou-wiki
-000031d0: 5d3a 2068 7474 7073 3a2f 2f65 6e2e 7769  ]: https://en.wi
-000031e0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-000031f0: 2f51 7561 6e7a 686f 755f 6469 616c 6563  /Quanzhou_dialec
-00003200: 7473 0d0a 5b6e 6c74 6b2d 746f 6b65 6e69  ts..[nltk-tokeni
-00003210: 7a65 5d3a 2068 7474 7073 3a2f 2f6e 6c74  ze]: https://nlt
-00003220: 6b2e 6f72 672f 6170 692f 6e6c 746b 2e74  k.org/api/nltk.t
-00003230: 6f6b 656e 697a 652e 6874 6d6c 0d0a 5b73  okenize.html..[s
-00003240: 616e 6468 692d 7769 6b69 5d3a 2068 7474  andhi-wiki]: htt
-00003250: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-00003260: 612e 6f72 672f 7769 6b69 2f54 6169 7761  a.org/wiki/Taiwa
-00003270: 6e65 7365 5f48 6f6b 6b69 656e 2354 6f6e  nese_Hokkien#Ton
-00003280: 6525 3230 7361 6e64 6869 3a7e 3a74 6578  e%20sandhi:~:tex
-00003290: 743d 7468 6e67 2545 3225 3946 2541 3925  t=thng%E2%9F%A9%
-000032a0: 3230 2825 3232 736f 7570 2532 3229 2e2d  20(%22soup%22).-
-000032b0: 2c54 6f6e 6525 3230 7361 6e64 6869 2c2d  ,Tone%20sandhi,-
-000032c0: 2535 4265 6469 7425 3544 0d0a            %5Bedit%5D..
+00000350: 3e0d 0a20 203c 6120 6872 6566 3d22 6874  >..  <a href="ht
+00000360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000370: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00000380: 6e22 3e0d 0a20 2020 203c 696d 6720 7372  n">..    <img sr
+00000390: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000003a0: 622e 636f 6d2f 616e 6472 6569 6861 722f  b.com/andreihar/
+000003b0: 7461 6962 756e 2f72 6177 2f6d 6169 6e2f  taibun/raw/main/
+000003c0: 7265 6164 6d65 2f6c 6f67 6f2e 706e 6722  readme/logo.png"
+000003d0: 2061 6c74 3d22 4c6f 676f 2220 7769 6474   alt="Logo" widt
+000003e0: 683d 2239 3022 2068 6569 6768 743d 2238  h="90" height="8
+000003f0: 3022 3e0d 0a20 203c 2f61 3e0d 0a20 200d  0">..  </a>..  .
+00000400: 0a23 2054 6169 6275 6e0d 0a0d 0a0d 0a0d  .# Taibun.......
+00000410: 0a3c 212d 2d20 5052 4f4a 4543 5420 5348  .<!-- PROJECT SH
+00000420: 4945 4c44 5320 2d2d 3e0d 0a5b 215b 436f  IELDS -->..[![Co
+00000430: 6e74 7269 6275 7469 6f6e 735d 5b63 6f6e  ntributions][con
+00000440: 7472 6962 7574 696f 6e73 2d62 6164 6765  tributions-badge
+00000450: 5d5d 5b63 6f6e 7472 6962 7574 696f 6e73  ]][contributions
+00000460: 5d0d 0a5b 215b 5465 7374 735d 5b74 6573  ]..[![Tests][tes
+00000470: 7473 2d62 6164 6765 5d5d 5b74 6573 7473  ts-badge]][tests
+00000480: 5d0d 0a5b 215b 5265 6c65 6173 655d 5b72  ]..[![Release][r
+00000490: 656c 6561 7365 2d62 6164 6765 5d5d 5b72  elease-badge]][r
+000004a0: 656c 6561 7365 5d0d 0a5b 215b 4c69 6365  elease]..[![Lice
+000004b0: 6e63 655d 5b6c 6963 656e 6365 2d62 6164  nce][licence-bad
+000004c0: 6765 5d5d 5b6c 6963 656e 6365 5d0d 0a5b  ge]][licence]..[
+000004d0: 215b 4c69 6e6b 6564 496e 5d5b 6c69 6e6b  ![LinkedIn][link
+000004e0: 6564 696e 2d62 6164 6765 5d5d 5b6c 696e  edin-badge]][lin
+000004f0: 6b65 6469 6e5d 0d0a 0d0a 2a2a 5461 6977  kedin]....**Taiw
+00000500: 616e 6573 6520 486f 6b6b 6965 6e20 5472  anese Hokkien Tr
+00000510: 616e 736c 6974 6572 6174 6f72 2061 6e64  ansliterator and
+00000520: 2054 6f6b 656e 6973 6572 2a2a 0d0a 0d0a   Tokeniser**....
+00000530: 4974 2068 6173 206d 6574 686f 6473 2074  It has methods t
+00000540: 6861 7420 616c 6c6f 7720 746f 2063 7573  hat allow to cus
+00000550: 746f 6d69 7365 2074 7261 6e73 6c69 7465  tomise translite
+00000560: 7261 7469 6f6e 2061 6e64 2072 6574 7269  ration and retri
+00000570: 6576 6520 616e 7920 6e65 6365 7373 6172  eve any necessar
+00000580: 7920 696e 666f 726d 6174 696f 6e20 6162  y information ab
+00000590: 6f75 7420 5461 6977 616e 6573 6520 486f  out Taiwanese Ho
+000005a0: 6b6b 6965 6e20 7072 6f6e 756e 6369 6174  kkien pronunciat
+000005b0: 696f 6e2e 3c62 7220 2f3e 0d0a 496e 636c  ion.<br />..Incl
+000005c0: 7564 6573 2077 6f72 6420 746f 6b65 6e69  udes word tokeni
+000005d0: 7365 7220 666f 7220 5461 6977 616e 6573  ser for Taiwanes
+000005e0: 6520 486f 6b6b 6965 6e2e 0d0a 0d0a 5b52  e Hokkien.....[R
+000005f0: 6570 6f72 7420 4275 675d 5b62 7567 5d20  eport Bug][bug] 
+00000600: e280 a20d 0a5b 5079 5049 5d5b 7079 7069  .....[PyPI][pypi
+00000610: 5d0d 0a0d 0a3c 2f64 6976 3e0d 0a0d 0a0d  ]....</div>.....
+00000620: 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a 0d0a 3c21  ...---........<!
+00000630: 2d2d 2054 4142 4c45 204f 4620 434f 4e54  -- TABLE OF CONT
+00000640: 454e 5453 202d 2d3e 0d0a 3c64 6574 6169  ENTS -->..<detai
+00000650: 6c73 206f 7065 6e3e 0d0a 2020 3c73 756d  ls open>..  <sum
+00000660: 6d61 7279 3e54 6162 6c65 206f 6620 436f  mary>Table of Co
+00000670: 6e74 656e 7473 3c2f 7375 6d6d 6172 793e  ntents</summary>
+00000680: 0d0a 2020 3c6f 6c3e 0d0a 2020 2020 3c6c  ..  <ol>..    <l
+00000690: 693e 3c61 2068 7265 663d 2223 7665 7273  i><a href="#vers
+000006a0: 696f 6e73 223e 5665 7273 696f 6e73 3c2f  ions">Versions</
+000006b0: 613e 3c2f 6c69 3e0d 0a20 2020 203c 6c69  a></li>..    <li
+000006c0: 3e3c 6120 6872 6566 3d22 2369 6e73 7461  ><a href="#insta
+000006d0: 6c6c 223e 496e 7374 616c 6c3c 2f61 3e3c  ll">Install</a><
+000006e0: 2f6c 693e 0d0a 2020 2020 3c6c 693e 0d0a  /li>..    <li>..
+000006f0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+00000700: 7573 6167 6522 3e55 7361 6765 3c2f 613e  usage">Usage</a>
+00000710: 0d0a 2020 2020 2020 3c75 6c3e 0d0a 2020  ..      <ul>..  
+00000720: 2020 2020 2020 3c6c 693e 0d0a 2020 2020        <li>..    
+00000730: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+00000740: 636f 6e76 6572 7465 7222 3e43 6f6e 7665  converter">Conve
+00000750: 7274 6572 3c2f 613e 0d0a 2020 2020 2020  rter</a>..      
+00000760: 2020 2020 3c75 6c3e 0d0a 2020 2020 2020      <ul>..      
+00000770: 2020 2020 2020 3c6c 693e 3c61 2068 7265        <li><a hre
+00000780: 663d 2223 7379 7374 656d 223e 5379 7374  f="#system">Syst
+00000790: 656d 3c2f 613e 3c2f 6c69 3e0d 0a20 2020  em</a></li>..   
+000007a0: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
+000007b0: 6872 6566 3d22 2364 6961 6c65 6374 223e  href="#dialect">
+000007c0: 4469 616c 6563 743c 2f61 3e3c 2f6c 693e  Dialect</a></li>
+000007d0: 0d0a 2020 2020 2020 2020 2020 2020 3c6c  ..            <l
+000007e0: 693e 3c61 2068 7265 663d 2223 666f 726d  i><a href="#form
+000007f0: 6174 223e 466f 726d 6174 3c2f 613e 3c2f  at">Format</a></
+00000800: 6c69 3e0d 0a20 2020 2020 2020 2020 2020  li>..           
+00000810: 203c 6c69 3e3c 6120 6872 6566 3d22 2364   <li><a href="#d
+00000820: 656c 696d 6974 6572 223e 4465 6c69 6d69  elimiter">Delimi
+00000830: 7465 723c 2f61 3e3c 2f6c 693e 0d0a 2020  ter</a></li>..  
+00000840: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
+00000850: 2068 7265 663d 2223 7361 6e64 6869 223e   href="#sandhi">
+00000860: 5361 6e64 6869 3c2f 613e 3c2f 6c69 3e0d  Sandhi</a></li>.
+00000870: 0a20 2020 2020 2020 2020 2020 203c 6c69  .            <li
+00000880: 3e3c 6120 6872 6566 3d22 2370 756e 6374  ><a href="#punct
+00000890: 7561 7469 6f6e 223e 5075 6e63 7475 6174  uation">Punctuat
+000008a0: 696f 6e3c 2f61 3e3c 2f6c 693e 0d0a 2020  ion</a></li>..  
+000008b0: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
+000008c0: 2068 7265 663d 2223 636f 6e76 6572 742d   href="#convert-
+000008d0: 6e6f 6e2d 636a 6b22 3e43 6f6e 7665 7274  non-cjk">Convert
+000008e0: 206e 6f6e 2d43 4a4b 3c2f 613e 3c2f 6c69   non-CJK</a></li
+000008f0: 3e0d 0a20 2020 2020 2020 2020 203c 2f75  >..          </u
+00000900: 6c3e 0d0a 2020 2020 2020 2020 3c2f 6c69  l>..        </li
+00000910: 3e0d 0a20 2020 2020 2020 203c 6c69 3e3c  >..        <li><
+00000920: 6120 6872 6566 3d22 2374 6f6b 656e 6973  a href="#tokenis
+00000930: 6572 223e 546f 6b65 6e69 7365 723c 2f61  er">Tokeniser</a
+00000940: 3e3c 2f6c 693e 0d0a 2020 2020 2020 2020  ></li>..        
+00000950: 3c6c 693e 3c61 2068 7265 663d 2223 6f74  <li><a href="#ot
+00000960: 6865 722d 6675 6e63 7469 6f6e 7322 3e4f  her-functions">O
+00000970: 7468 6572 2046 756e 6374 696f 6e73 3c2f  ther Functions</
+00000980: 613e 3c2f 6c69 3e0d 0a20 2020 2020 203c  a></li>..      <
+00000990: 2f75 6c3e 0d0a 2020 2020 3c2f 6c69 3e0d  /ul>..    </li>.
+000009a0: 0a20 2020 203c 6c69 3e3c 6120 6872 6566  .    <li><a href
+000009b0: 3d22 2365 7861 6d70 6c65 223e 4578 616d  ="#example">Exam
+000009c0: 706c 653c 2f61 3e3c 2f6c 693e 0d0a 2020  ple</a></li>..  
+000009d0: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
+000009e0: 6461 7461 223e 4461 7461 3c2f 613e 3c2f  data">Data</a></
+000009f0: 6c69 3e0d 0a20 2020 203c 6c69 3e3c 6120  li>..    <li><a 
+00000a00: 6872 6566 3d22 2361 636b 6e6f 776c 6564  href="#acknowled
+00000a10: 6765 6d65 6e74 7322 3e41 636b 6e6f 776c  gements">Acknowl
+00000a20: 6564 6765 6d65 6e74 733c 2f61 3e3c 2f6c  edgements</a></l
+00000a30: 693e 0d0a 2020 2020 3c6c 693e 3c61 2068  i>..    <li><a h
+00000a40: 7265 663d 2223 6c69 6365 6e63 6522 3e4c  ref="#licence">L
+00000a50: 6963 656e 6365 3c2f 613e 3c2f 6c69 3e0d  icence</a></li>.
+00000a60: 0a20 203c 2f6f 6c3e 0d0a 3c2f 6465 7461  .  </ol>..</deta
+00000a70: 696c 733e 0d0a 0d0a 0d0a 0d0a 3c21 2d2d  ils>........<!--
+00000a80: 204f 5448 4552 2056 4552 5349 4f4e 5320   OTHER VERSIONS 
+00000a90: 2d2d 3e0d 0a23 2320 5665 7273 696f 6e73  -->..## Versions
+00000aa0: 0d0a 0d0a 5b21 5b4a 6176 6153 6372 6970  ....[![JavaScrip
+00000ab0: 7420 5665 7273 696f 6e5d 5b6a 732d 6261  t Version][js-ba
+00000ac0: 6467 655d 5d5b 6a73 2d6c 696e 6b5d 0d0a  dge]][js-link]..
+00000ad0: 0d0a 0d0a 0d0a 3c21 2d2d 2049 4e53 5441  ......<!-- INSTA
+00000ae0: 4c4c 202d 2d3e 0d0a 2323 2049 6e73 7461  LL -->..## Insta
+00000af0: 6c6c 0d0a 0d0a 5461 6962 756e 2063 616e  ll....Taibun can
+00000b00: 2062 6520 696e 7374 616c 6c65 6420 6672   be installed fr
+00000b10: 6f6d 205b 7079 7069 5d5b 7079 7069 5d0d  om [pypi][pypi].
+00000b20: 0a0d 0a60 6060 6261 7368 0d0a 2420 7069  ...```bash..$ pi
+00000b30: 7020 696e 7374 616c 6c20 7461 6962 756e  p install taibun
+00000b40: 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c 212d  ..```........<!-
+00000b50: 2d20 5553 4147 4520 2d2d 3e0d 0a23 2320  - USAGE -->..## 
+00000b60: 5573 6167 650d 0a0d 0a23 2323 2043 6f6e  Usage....### Con
+00000b70: 7665 7274 6572 0d0a 0d0a 6043 6f6e 7665  verter....`Conve
+00000b80: 7274 6572 6020 636c 6173 7320 7472 616e  rter` class tran
+00000b90: 736c 6974 6572 6174 6573 2074 6865 2043  sliterates the C
+00000ba0: 6869 6e65 7365 2063 6861 7261 6374 6572  hinese character
+00000bb0: 7320 746f 2074 6865 2063 686f 7365 6e20  s to the chosen 
+00000bc0: 7472 616e 736c 6974 6572 6174 696f 6e20  transliteration 
+00000bd0: 7379 7374 656d 2077 6974 6820 7061 7261  system with para
+00000be0: 6d65 7465 7273 2073 7065 6369 6669 6564  meters specified
+00000bf0: 2062 7920 7468 6520 6465 7665 6c6f 7065   by the develope
+00000c00: 722e 2057 6f72 6b73 2066 6f72 2062 6f74  r. Works for bot
+00000c10: 6820 5472 6164 6974 696f 6e61 6c20 616e  h Traditional an
+00000c20: 6420 5369 6d70 6c69 6669 6564 2063 6861  d Simplified cha
+00000c30: 7261 6374 6572 732e 0d0a 0d0a 6060 6070  racters.....```p
+00000c40: 7974 686f 6e0d 0a23 2043 6f6e 7374 7275  ython..# Constru
+00000c50: 6374 6f72 0d0a 6320 3d20 436f 6e76 6572  ctor..c = Conver
+00000c60: 7465 7228 7379 7374 656d 2c20 6469 616c  ter(system, dial
+00000c70: 6563 742c 2066 6f72 6d61 742c 2064 656c  ect, format, del
+00000c80: 696d 6974 6572 2c20 7361 6e64 6869 2c20  imiter, sandhi, 
+00000c90: 7075 6e63 7475 6174 696f 6e2c 2063 6f6e  punctuation, con
+00000ca0: 7665 7274 5f6e 6f6e 5f63 6a6b 290d 0a0d  vert_non_cjk)...
+00000cb0: 0a23 2054 7261 6e73 6c69 7465 7261 7465  .# Transliterate
+00000cc0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+00000cd0: 6572 730d 0a63 2e67 6574 2869 6e70 7574  ers..c.get(input
+00000ce0: 290d 0a60 6060 0d0a 0d0a 2323 2323 2053  )..```....#### S
+00000cf0: 7973 7465 6d0d 0a0d 0a60 7379 7374 656d  ystem....`system
+00000d00: 6020 5374 7269 6e67 202d 2073 7973 7465  ` String - syste
+00000d10: 6d20 6f66 2074 7261 6e73 6c69 7465 7261  m of translitera
+00000d20: 7469 6f6e 2e0d 0a0d 0a2a 2060 5461 696c  tion.....* `Tail
+00000d30: 6f60 2028 6465 6661 756c 7429 202d 205b  o` (default) - [
+00000d40: 54c3 a269 2d75 c3a2 6e20 4cc3 b42d 6dc3  T..i-u..n L..-m.
+00000d50: a12d 6ac4 ab20 5068 696e 672d 696d 2048  .-j.. Phing-im H
+00000d60: 6f6e 672d c3a0 6e5d 5b74 6169 6c6f 2d77  ong-..n][tailo-w
+00000d70: 696b 695d 0d0a 2a20 6050 4f4a 6020 2d20  iki]..* `POJ` - 
+00000d80: 5b50 65cc 8d68 2dc5 8d65 2d6a c4ab 5d5b  [Pe..h-..e-j..][
+00000d90: 706f 6a2d 7769 6b69 5d0d 0a2a 2060 5a68  poj-wiki]..* `Zh
+00000da0: 7579 696e 6020 2d20 5b54 6169 7761 6e65  uyin` - [Taiwane
+00000db0: 7365 2050 686f 6e65 7469 6320 5379 6d62  se Phonetic Symb
+00000dc0: 6f6c 735d 5b7a 6875 7969 6e2d 7769 6b69  ols][zhuyin-wiki
+00000dd0: 5d0d 0a2a 2060 544c 5041 6020 2d20 5b54  ]..* `TLPA` - [T
+00000de0: 6169 7761 6e65 7365 204c 616e 6775 6167  aiwanese Languag
+00000df0: 6520 5068 6f6e 6574 6963 2041 6c70 6861  e Phonetic Alpha
+00000e00: 6265 745d 5b74 6c70 612d 7769 6b69 5d0d  bet][tlpa-wiki].
+00000e10: 0a2a 2060 5069 6e67 7969 6d60 202d 205b  .* `Pingyim` - [
+00000e20: 4262 c3a1 6e6c c3a1 6d20 55c4 9320 50c3  Bb..nl..m U.. P.
+00000e30: ac6e 6779 c4ab 6d20 48c5 8d6e 6727 c3a0  .ngy..m H..ng'..
+00000e40: 6e5d 5b70 696e 6779 696d 2d77 696b 695d  n][pingyim-wiki]
+00000e50: 0d0a 2a20 6054 6f6e 6769 6f6e 6760 202d  ..* `Tongiong` -
+00000e60: 205b 4461 c4ab 2d67 68c3 ae20 54c5 8d6e   [Da..-gh.. T..n
+00000e70: 672d 69c5 8d6e 6720 50c4 ab6e 672d 696d  g-i..ng P..ng-im
+00000e80: 5d5b 746f 6e67 696f 6e67 2d77 696b 695d  ][tongiong-wiki]
+00000e90: 0d0a 2a20 6049 5041 6020 2d20 5b49 6e74  ..* `IPA` - [Int
+00000ea0: 6572 6e61 7469 6f6e 616c 2050 686f 6e65  ernational Phone
+00000eb0: 7469 6320 416c 7068 6162 6574 5d5b 6970  tic Alphabet][ip
+00000ec0: 612d 7769 6b69 5d0d 0a0d 0a7c 2074 6578  a-wiki]....| tex
+00000ed0: 7420 7c20 5461 696c 6f20 2020 7c20 504f  t | Tailo   | PO
+00000ee0: 4a20 2020 2020 7c20 5a68 7579 696e 2020  J     | Zhuyin  
+00000ef0: 2020 2020 7c20 544c 5041 2020 2020 2020      | TLPA      
+00000f00: 7c20 5069 6e67 7969 6d20 7c20 546f 6e67  | Pingyim | Tong
+00000f10: 696f 6e67 207c 2049 5041 2020 2020 2020  iong | IPA      
+00000f20: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+00000f30: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00000f40: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 207c   | ----------- |
+00000f50: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00000f60: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d20  ---- | -------- 
+00000f70: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  | ----------- |.
+00000f80: 0a7c 20e5 8fb0 e781 a320 7c20 54c3 a269  .| ...... | T..i
+00000f90: 2d75 c3a2 6e20 7c20 54c3 a269 2d6f c3a2  -u..n | T..i-o..
+00000fa0: 6e20 7c20 e384 89e3 849e cb8a 20e3 84a8  n | ........ ...
+00000fb0: e384 a2cb 8a20 7c20 5461 6935 2075 616e  ..... | Tai5 uan
+00000fc0: 3520 7c20 44c3 a169 77c3 a16e 2020 7c20  5 | D..iw..n  | 
+00000fd0: 54c4 8169 2d75 c78e 6e20 207c 2054 6169  T..i-u..n  | Tai
+00000fe0: c2b2 e281 b520 7561 6ec2 b2e2 81b5 207c  ..... uan..... |
+00000ff0: 0d0a 0d0a 2323 2323 2044 6961 6c65 6374  ....#### Dialect
+00001000: 0d0a 0d0a 6064 6961 6c65 6374 6020 5374  ....`dialect` St
+00001010: 7269 6e67 202d 2070 7265 6665 7272 6564  ring - preferred
+00001020: 2070 726f 6e75 6e63 6961 7469 6f6e 2e0d   pronunciation..
+00001030: 0a0d 0a2a 2060 736f 7574 6860 2028 6465  ...* `south` (de
+00001040: 6661 756c 7429 202d 205b 5a68 616e 677a  fault) - [Zhangz
+00001050: 686f 755d 5b7a 6861 6e67 7a68 6f75 2d77  hou][zhangzhou-w
+00001060: 696b 695d 2d6c 6561 6e69 6e67 2070 726f  iki]-leaning pro
+00001070: 6e75 6e63 6961 7469 6f6e 0d0a 2a20 606e  nunciation..* `n
+00001080: 6f72 7468 6020 2d20 5b51 7561 6e7a 686f  orth` - [Quanzho
+00001090: 755d 5b71 7561 6e7a 686f 752d 7769 6b69  u][quanzhou-wiki
+000010a0: 5d2d 6c65 616e 696e 6720 7072 6f6e 756e  ]-leaning pronun
+000010b0: 6369 6174 696f 6e0d 0a0d 0a7c 2074 6578  ciation....| tex
+000010c0: 7420 2020 7c20 736f 7574 6820 2020 2020  t   | south     
+000010d0: 2020 2020 7c20 6e6f 7274 6820 2020 2020      | north     
+000010e0: 2020 2020 7c0d 0a7c 202d 2d2d 2d2d 2d20      |..| ------ 
+000010f0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  | ------------- 
+00001100: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  | ------------- 
+00001110: 7c0d 0a7c 20e4 ba94 e69c 88e7 af80 207c  |..| ......... |
+00001120: 2047 c58d 6f2d 6775 65cc 8d68 2d74 7365   G..o-gue..h-tse
+00001130: 6820 7c20 47c5 8d6f 2d67 65cc 8d68 2d74  h | G..o-ge..h-t
+00001140: 7375 6568 207c 0d0a 0d0a 2323 2323 2046  sueh |....#### F
+00001150: 6f72 6d61 740d 0a0d 0a60 666f 726d 6174  ormat....`format
+00001160: 6020 5374 7269 6e67 202d 2066 6f72 6d61  ` String - forma
+00001170: 7420 696e 2077 6869 6368 2074 6f6e 6573  t in which tones
+00001180: 2077 696c 6c20 6265 2072 6570 7265 7365   will be represe
+00001190: 6e74 6564 2069 6e20 7468 6520 636f 6e76  nted in the conv
+000011a0: 6572 7465 6420 7365 6e74 656e 6365 2e0d  erted sentence..
+000011b0: 0a0d 0a2a 2060 6d61 726b 6020 2864 6566  ...* `mark` (def
+000011c0: 6175 6c74 2920 2d20 7573 6573 2064 6961  ault) - uses dia
+000011d0: 6372 6974 6963 7320 666f 7220 6561 6368  critics for each
+000011e0: 2073 796c 6c61 626c 652e 204e 6f74 2061   syllable. Not a
+000011f0: 7661 696c 6162 6c65 2066 6f72 2054 4c50  vailable for TLP
+00001200: 412e 0d0a 2a20 606e 756d 6265 7260 202d  A...* `number` -
+00001210: 2061 6464 2061 206e 756d 6265 7220 7768   add a number wh
+00001220: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
+00001230: 6865 2074 6f6e 6520 6174 2074 6865 2065  he tone at the e
+00001240: 6e64 206f 6620 7468 6520 7379 6c6c 6162  nd of the syllab
+00001250: 6c65 0d0a 2a20 6073 7472 6970 6020 2d20  le..* `strip` - 
+00001260: 7265 6d6f 7665 7320 616e 7920 746f 6e65  removes any tone
+00001270: 206d 6172 6b69 6e67 0d0a 0d0a 7c20 7465   marking....| te
+00001280: 7874 207c 206d 6172 6b20 2020 207c 206e  xt | mark    | n
+00001290: 756d 6265 7220 2020 207c 2073 7472 6970  umber    | strip
+000012a0: 2020 207c 0d0a 7c20 2d2d 2d2d 207c 202d     |..| ---- | -
+000012b0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+000012c0: 2d2d 207c 202d 2d2d 2d2d 2d2d 207c 0d0a  -- | ------- |..
+000012d0: 7c20 e58f b0e7 81a3 207c 2054 c3a2 692d  | ...... | T..i-
+000012e0: 75c3 a26e 207c 2054 6169 352d 7561 6e35  u..n | Tai5-uan5
+000012f0: 207c 2054 6169 2d75 616e 207c 0d0a 0d0a   | Tai-uan |....
+00001300: 2323 2323 2044 656c 696d 6974 6572 0d0a  #### Delimiter..
+00001310: 0d0a 6064 656c 696d 6974 6572 6020 5374  ..`delimiter` St
+00001320: 7269 6e67 202d 2073 6574 7320 7468 6520  ring - sets the 
+00001330: 6465 6c69 6d69 7465 7220 6368 6172 6163  delimiter charac
+00001340: 7465 7220 7468 6174 2077 696c 6c20 6265  ter that will be
+00001350: 2070 6c61 6365 6420 696e 2062 6574 7765   placed in betwe
+00001360: 656e 2073 796c 6c61 626c 6573 206f 6620  en syllables of 
+00001370: 6120 776f 7264 2e0d 0a0d 0a44 6566 6175  a word.....Defau
+00001380: 6c74 2076 616c 7565 2064 6570 656e 6473  lt value depends
+00001390: 206f 6e20 7468 6520 6368 6f73 656e 2060   on the chosen `
+000013a0: 7379 7374 656d 603a 0d0a 0d0a 2a20 6027  system`:....* `'
+000013b0: 2d27 6020 2d20 666f 7220 6054 6169 6c6f  -'` - for `Tailo
+000013c0: 602c 2060 504f 4a60 2c20 6054 6f6e 6769  `, `POJ`, `Tongi
+000013d0: 6f6e 6760 0d0a 2a20 6027 2760 202d 2066  ong`..* `''` - f
+000013e0: 6f72 2060 5069 6e67 7969 6d60 0d0a 2a20  or `Pingyim`..* 
+000013f0: 6027 2027 6020 2d20 666f 7220 605a 6875  `' '` - for `Zhu
+00001400: 7969 6e60 2c20 6054 4c50 4160 2c20 6049  yin`, `TLPA`, `I
+00001410: 5041 600d 0a0d 0a7c 2074 6578 7420 7c20  PA`....| text | 
+00001420: 272d 2720 2020 2020 7c20 2727 2020 2020  '-'     | ''    
+00001430: 207c 2027 2027 2020 2020 207c 0d0a 7c20   | ' '     |..| 
+00001440: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 207c  ---- | ------- |
+00001450: 202d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d   ------ | ------
+00001460: 2d20 7c0d 0a7c 20e5 8fb0 e781 a320 7c20  - |..| ...... | 
+00001470: 54c3 a269 2d75 c3a2 6e20 7c20 54c3 a269  T..i-u..n | T..i
+00001480: 75c3 a26e 207c 2054 c3a2 6920 75c3 a26e  u..n | T..i u..n
+00001490: 207c 0d0a 0d0a 2323 2323 2053 616e 6468   |....#### Sandh
+000014a0: 690d 0a0d 0a60 7361 6e64 6869 6020 5374  i....`sandhi` St
+000014b0: 7269 6e67 202d 2061 7070 6c69 6573 2074  ring - applies t
+000014c0: 6865 205b 7361 6e64 6869 2072 756c 6573  he [sandhi rules
+000014d0: 206f 6620 5461 6977 616e 6573 6520 486f   of Taiwanese Ho
+000014e0: 6b6b 6965 6e5d 5b73 616e 6468 692d 7769  kkien][sandhi-wi
+000014f0: 6b69 5d2e 0d0a 0d0a 5369 6e63 6520 6974  ki].....Since it
+00001500: 2773 2064 6966 6669 6375 6c74 2074 6f20  's difficult to 
+00001510: 656e 636f 6465 2061 6c6c 2073 616e 6468  encode all sandh
+00001520: 6920 7275 6c65 732c 2054 6169 6275 6e20  i rules, Taibun 
+00001530: 7072 6f76 6964 6573 206d 756c 7469 706c  provides multipl
+00001540: 6520 6d6f 6465 7320 666f 7220 7361 6e64  e modes for sand
+00001550: 6869 2063 6f6e 7665 7273 696f 6e20 746f  hi conversion to
+00001560: 2061 6c6c 6f77 2066 6f72 2063 7573 746f   allow for custo
+00001570: 6d69 7365 6420 7361 6e64 6869 2068 616e  mised sandhi han
+00001580: 646c 696e 672e 0d0a 0d0a 2a20 606e 6f6e  dling.....* `non
+00001590: 6560 202d 2064 6f65 736e 2774 2070 6572  e` - doesn't per
+000015a0: 666f 726d 2061 6e79 2074 6f6e 6520 7361  form any tone sa
+000015b0: 6e64 6869 0d0a 2a20 6061 7574 6f60 202d  ndhi..* `auto` -
+000015c0: 2063 6c6f 7365 7374 2061 7070 726f 7869   closest approxi
+000015d0: 6d61 7469 6f6e 2074 6f20 6675 6c6c 2063  mation to full c
+000015e0: 6f72 7265 6374 2074 6f6e 6520 7361 6e64  orrect tone sand
+000015f0: 6869 206f 6620 5461 6977 616e 6573 652c  hi of Taiwanese,
+00001600: 2077 6974 6820 7072 6f70 6572 2073 616e   with proper san
+00001610: 6468 6920 6f66 2070 726f 6e6f 756e 732c  dhi of pronouns,
+00001620: 2073 7566 6669 7865 732c 2061 6e64 2077   suffixes, and w
+00001630: 6f72 6473 2077 6974 6820 e4bb 940d 0a2a  ords with .....*
+00001640: 2060 6578 635f 6c61 7374 6020 2d20 6368   `exc_last` - ch
+00001650: 616e 6765 7320 746f 6e65 2066 6f72 2065  anges tone for e
+00001660: 7665 7279 2073 796c 6c61 626c 6520 6578  very syllable ex
+00001670: 6365 7074 2066 6f72 2074 6865 206c 6173  cept for the las
+00001680: 7420 6f6e 650d 0a2a 2060 696e 636c 5f6c  t one..* `incl_l
+00001690: 6173 7460 202d 2063 6861 6e67 6573 2074  ast` - changes t
+000016a0: 6f6e 6520 666f 7220 6576 6572 7920 7379  one for every sy
+000016b0: 6c6c 6162 6c65 2069 6e63 6c75 6469 6e67  llable including
+000016c0: 2074 6865 206c 6173 7420 6f6e 650d 0a0d   the last one...
+000016d0: 0a44 6566 6175 6c74 2076 616c 7565 2064  .Default value d
+000016e0: 6570 656e 6473 206f 6e20 7468 6520 6368  epends on the ch
+000016f0: 6f73 656e 2060 7379 7374 656d 603a 0d0a  osen `system`:..
+00001700: 0d0a 2a20 6061 7574 6f60 202d 2066 6f72  ..* `auto` - for
+00001710: 2060 546f 6e67 696f 6e67 600d 0a2a 2060   `Tongiong`..* `
+00001720: 6e6f 6e65 6020 2d20 666f 7220 6054 6169  none` - for `Tai
+00001730: 6c6f 602c 2060 504f 4a60 2c20 605a 6875  lo`, `POJ`, `Zhu
+00001740: 7969 6e60 2c20 6054 4c50 4160 2c20 6050  yin`, `TLPA`, `P
+00001750: 696e 6779 696d 602c 2060 4950 4160 0d0a  ingyim`, `IPA`..
+00001760: 0d0a 7c20 7465 7874 2020 2020 2020 2020  ..| text        
+00001770: 2020 2020 207c 206e 6f6e 6520 2020 2020       | none     
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 207c 2061 7574 6f20 2020 2020 2020 2020   | auto         
+000017a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000017b0: 6578 635f 6c61 7374 2020 2020 2020 2020  exc_last        
+000017c0: 2020 2020 2020 2020 2020 7c20 696e 636c            | incl
+000017d0: 5f6c 6173 7420 2020 2020 2020 2020 2020  _last           
+000017e0: 2020 2020 2020 7c0d 0a7c 202d 2d2d 2d2d        |..| -----
+000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001810: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001830: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   | -------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0d0a  ------------ |..
+00001870: 7c20 e980 99e6 98af e4bd a0e7 9a84 e689  | ..............
+00001880: 8be6 a99f e4bb 94e7 84a1 207c 2054 7365  .......... | Tse
+00001890: 2073 c4ab 206c c3ad 20c3 aa20 7473 6869   s.. l.. .. tshi
+000018a0: c3ba 2d6b 692d c3a1 2062 c3b4 207c 2054  ..-ki-.. b.. | T
+000018b0: 7365 2073 c3ac 206c 6920 c493 2074 7368  se s.. li .. tsh
+000018c0: 6975 2d6b c4ab 2dc3 a120 62c3 b43f 207c  iu-k..-.. b..? |
+000018d0: 2054 73c4 9320 73c3 ac20 6c69 20c4 9320   Ts.. s.. li .. 
+000018e0: 7473 6869 752d 6bc4 ab2d 6120 62c3 b420  tshiu-k..-a b.. 
+000018f0: 7c20 5473 c493 2073 c3ac 206c 6920 c493  | Ts.. s.. li ..
+00001900: 2074 7368 6975 2d6b c4ab 2d61 2062 c58d   tshiu-k..-a b..
+00001910: 207c 0d0a 0d0a 5361 6e64 6869 2072 756c   |....Sandhi rul
+00001920: 6573 2061 6c73 6f20 6368 616e 6765 2064  es also change d
+00001930: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+00001940: 6469 616c 6563 7420 6368 6f73 656e 2e0d  dialect chosen..
+00001950: 0a0d 0a7c 2074 6578 7420 7c20 6e6f 2073  ...| text | no s
+00001960: 616e 6468 6920 7c20 736f 7574 6820 2020  andhi | south   
+00001970: 7c20 6e6f 7274 6820 2020 7c0d 0a7c 202d  | north   |..| -
+00001980: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d20  --- | --------- 
+00001990: 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d  | ------- | ----
+000019a0: 2d2d 2d20 7c0d 0a7c 20e5 8fb0 e781 a320  --- |..| ...... 
+000019b0: 7c20 54c3 a269 2d75 c3a2 6e20 2020 7c20  | T..i-u..n   | 
+000019c0: 54c4 8169 2d75 c3a2 6e20 7c20 54c3 a069  T..i-u..n | T..i
+000019d0: 2d75 c3a2 6e20 7c0d 0a0d 0a23 2323 2320  -u..n |....#### 
+000019e0: 5075 6e63 7475 6174 696f 6e0d 0a0d 0a60  Punctuation....`
+000019f0: 7075 6e63 7475 6174 696f 6e60 2053 7472  punctuation` Str
+00001a00: 696e 670d 0a0d 0a2a 2060 666f 726d 6174  ing....* `format
+00001a10: 6020 2864 6566 6175 6c74 2920 2d20 636f  ` (default) - co
+00001a20: 6e76 6572 7473 2043 6869 6e65 7365 2d73  nverts Chinese-s
+00001a30: 7479 6c65 2070 756e 6374 7561 7469 6f6e  tyle punctuation
+00001a40: 2074 6f20 4c61 7469 6e2d 7374 796c 6520   to Latin-style 
+00001a50: 7075 6e63 7475 6174 696f 6e20 616e 6420  punctuation and 
+00001a60: 6361 7069 7461 6c69 7365 7320 776f 7264  capitalises word
+00001a70: 7320 6174 2074 6865 2062 6567 696e 6e69  s at the beginni
+00001a80: 6e67 206f 6620 6561 6368 2073 656e 7465  ng of each sente
+00001a90: 6e63 652e 0d0a 2a20 606e 6f6e 6560 202d  nce...* `none` -
+00001aa0: 2070 7265 7365 7276 6573 2043 6869 6e65   preserves Chine
+00001ab0: 7365 2d73 7479 6c65 2070 756e 6374 7561  se-style punctua
+00001ac0: 7469 6f6e 2061 6e64 2064 6f65 736e 2774  tion and doesn't
+00001ad0: 2063 6170 6974 616c 6973 6520 776f 7264   capitalise word
+00001ae0: 7320 6174 2074 6865 2062 6567 696e 6e69  s at the beginni
+00001af0: 6e67 206f 6620 6e65 7720 7365 6e74 656e  ng of new senten
+00001b00: 6365 732e 0d0a 0d0a 7c20 7465 7874 2020  ces.....| text  
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b50: 2020 2020 2020 2020 207c 2066 6f72 6d61           | forma
+00001b60: 7420 2020 2020 2020 2020 2020 2020 2020  t               
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 2020 2020 207c 206e               | n
+00001bc0: 6f6e 6520 2020 2020 2020 2020 2020 2020  one             
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 7c0d 0a7c 202d 2d2d 2d2d 2d2d      |..| -------
+00001c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c70: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+00001c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ----------- | --
+00001ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 2d2d 207c 0d0a 7c20 e980 99e6 98af e887  -- |..| ........
+00001d50: bae5 8d97 efbc 8ce7 b0a1 e7a8 b1e3 808c  ................
+00001d60: e58d 97e3 808d efbc 88e7 99bd e8a9 b1e5  ................
+00001d70: ad97 efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
+00001d80: 9be6 b3a8 e99f b3e7 aca6 e899 9fef bc9a  ................
+00001d90: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
+00001da0: 8aef bc8c e59c 8be8 aa9e efbc 9a54 c3a1  .............T..
+00001db0: 696e c3a1 6eef bc89 e380 8220 7c20 5473  in..n...... | Ts
+00001dc0: 6520 73c4 ab20 54c3 a269 2d6c c3a2 6d2c  e s.. T..i-l..m,
+00001dd0: 206b c3a1 6e2d 7473 6869 6e67 2022 6cc3   k..n-tshing "l.
+00001de0: a26d 2220 2850 65cc 8d68 2d75 c493 2d6a  .m" (Pe..h-u..-j
+00001df0: c4ab 3a20 54c3 a269 2d6c c3a2 6d3b 2074  ..: T..i-l..m; t
+00001e00: 73c3 b92d 696d 2068 c3bb 2d68 c58d 3a20  s..-im h..-h..: 
+00001e10: e384 8ae3 849e cb8a 20e3 848b e384 a2cb  ........ .......
+00001e20: 8a2c 206b 6f6b 2d67 c3ad 3a20 54c3 a169  ., kok-g..: T..i
+00001e30: 6ec3 a16e 292e 207c 2074 7365 2073 c4ab  n..n). | tse s..
+00001e40: 2054 c3a2 692d 6cc3 a26d efbc 8c6b c3a1   T..i-l..m...k..
+00001e50: 6e2d 7473 6869 6e67 e380 8c6c c3a2 6de3  n-tshing...l..m.
+00001e60: 808d efbc 8850 65cc 8d68 2d75 c493 2d6a  .....Pe..h-u..-j
+00001e70: c4ab efbc 9a54 c3a2 692d 6cc3 a26d efbc  .....T..i-l..m..
+00001e80: 9b74 73c3 b92d 696d 2068 c3bb 2d68 c58d  .ts..-im h..-h..
+00001e90: efbc 9ae3 848a e384 9ecb 8a20 e384 8be3  ........... ....
+00001ea0: 84a2 cb8a efbc 8c6b 6f6b 2d67 c3ad efbc  .......kok-g....
+00001eb0: 9a54 c3a1 696e c3a1 6eef bc89 e380 8220  .T..in..n...... 
+00001ec0: 7c0d 0a0d 0a23 2323 2320 436f 6e76 6572  |....#### Conver
+00001ed0: 7420 6e6f 6e2d 434a 4b0d 0a0d 0a60 636f  t non-CJK....`co
+00001ee0: 6e76 6572 745f 6e6f 6e5f 636a 6b60 2042  nvert_non_cjk` B
+00001ef0: 6f6f 6c65 616e 202d 2064 6566 696e 6573  oolean - defines
+00001f00: 2077 6865 7468 6572 206f 7220 6e6f 7420   whether or not 
+00001f10: 746f 2063 6f6e 7665 7274 206e 6f6e 2d43  to convert non-C
+00001f20: 6869 6e65 7365 2077 6f72 6473 2e20 4361  hinese words. Ca
+00001f30: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+00001f40: 7665 7274 2054 6169 6c6f 2074 6f20 616e  vert Tailo to an
+00001f50: 6f74 6865 7220 726f 6d61 6e69 7361 7469  other romanisati
+00001f60: 6f6e 2073 7973 7465 6d2e 0d0a 0d0a 2a20  on system.....* 
+00001f70: 6054 7275 6560 202d 2063 6f6e 7665 7274  `True` - convert
+00001f80: 206e 6f6e 2d43 6869 6e65 7365 2063 6861   non-Chinese cha
+00001f90: 7261 6374 6572 2077 6f72 6473 0d0a 2a20  racter words..* 
+00001fa0: 6046 616c 7365 6020 2864 6566 6175 6c74  `False` (default
+00001fb0: 2920 2d20 636f 6e76 6572 7420 6f6e 6c79  ) - convert only
+00001fc0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+00001fd0: 6572 2077 6f72 6473 0d0a 0d0a 7c20 7465  er words....| te
+00001fe0: 7874 2020 2020 2020 7c20 4661 6c73 6520  xt      | False 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 2020 7c20 5472 7565 2020 2020 2020 2020    | True        
+00002010: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
+00002020: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002040: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+00002060: 0d0a 7c20 e688 91e9 a39f 7068 c3a1 6e67  ..| ......ph..ng
+00002070: 207c 20e3 86a3 e384 a8e3 849a cb8b 20e3   | ........... .
+00002080: 8490 e384 a7e3 849a e386 b7cb 9920 7068  ............. ph
+00002090: c3a1 6e67 207c 20e3 86a3 e384 a8e3 849a  ..ng | .........
+000020a0: cb8b 20e3 8490 e384 a7e3 849a e386 b7cb  .. .............
+000020b0: 9920 e384 86e3 84a4 cb8b 207c 0d0a 0d0a  . ........ |....
+000020c0: 2323 2320 546f 6b65 6e69 7365 720d 0a0d  ### Tokeniser...
+000020d0: 0a60 546f 6b65 6e69 7365 7260 2063 6c61  .`Tokeniser` cla
+000020e0: 7373 2070 6572 666f 726d 7320 5b4e 4c54  ss performs [NLT
+000020f0: 4b20 776f 7264 7075 6e63 745f 746f 6b65  K wordpunct_toke
+00002100: 6e69 7a65 5d5b 6e6c 746b 2d74 6f6b 656e  nize][nltk-token
+00002110: 697a 655d 2d6c 696b 6520 746f 6b65 6e69  ize]-like tokeni
+00002120: 7361 7469 6f6e 206f 6620 6120 5461 6977  sation of a Taiw
+00002130: 616e 6573 6520 486f 6b6b 6965 6e20 7365  anese Hokkien se
+00002140: 6e74 656e 6365 2e0d 0a0d 0a60 6060 7079  ntence.....```py
+00002150: 7468 6f6e 0d0a 2320 436f 6e73 7472 7563  thon..# Construc
+00002160: 746f 720d 0a74 203d 2054 6f6b 656e 6973  tor..t = Tokenis
+00002170: 6572 2829 0d0a 0d0a 2320 546f 6b65 6e69  er()....# Tokeni
+00002180: 7365 2054 6169 7761 6e65 7365 2048 6f6b  se Taiwanese Hok
+00002190: 6b69 656e 2073 656e 7465 6e63 650d 0a74  kien sentence..t
+000021a0: 2e74 6f6b 656e 6973 6528 696e 7075 7429  .tokenise(input)
+000021b0: 0d0a 6060 600d 0a0d 0a23 2323 204f 7468  ..```....### Oth
+000021c0: 6572 2046 756e 6374 696f 6e73 0d0a 0d0a  er Functions....
+000021d0: 4861 6e64 7920 6675 6e63 7469 6f6e 7320  Handy functions 
+000021e0: 666f 7220 4e4c 5020 7461 736b 7320 696e  for NLP tasks in
+000021f0: 2054 6169 7761 6e65 7365 2048 6f6b 6b69   Taiwanese Hokki
+00002200: 656e 2e0d 0a0d 0a60 6060 7079 7468 6f6e  en.....```python
+00002210: 0d0a 2320 436f 6e76 6572 7420 746f 2054  ..# Convert to T
+00002220: 7261 6469 7469 6f6e 616c 0d0a 746f 5f74  raditional..to_t
+00002230: 7261 6469 7469 6f6e 616c 2869 6e70 7574  raditional(input
+00002240: 290d 0a0d 0a23 2043 6f6e 7665 7274 2074  )....# Convert t
+00002250: 6f20 5369 6d70 6c69 6669 6564 0d0a 746f  o Simplified..to
+00002260: 5f73 696d 706c 6966 6965 6428 696e 7075  _simplified(inpu
+00002270: 7429 0d0a 0d0a 2320 4368 6563 6b20 6966  t)....# Check if
+00002280: 2074 6865 2073 7472 696e 6720 6973 2066   the string is f
+00002290: 756c 6c79 2063 6f6d 706f 7365 6420 6f66  ully composed of
+000022a0: 2043 6869 6e65 7365 2063 6861 7261 6374   Chinese charact
+000022b0: 6572 730d 0a69 735f 636a 6b28 696e 7075  ers..is_cjk(inpu
+000022c0: 7429 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c  t)..```........<
+000022d0: 212d 2d20 4558 414d 504c 4520 2d2d 3e0d  !-- EXAMPLE -->.
+000022e0: 0a23 2320 4578 616d 706c 650d 0a0d 0a60  .## Example....`
+000022f0: 6060 7079 7468 6f6e 0d0a 2320 436f 6e76  ``python..# Conv
+00002300: 6572 7465 720d 0a66 726f 6d20 7461 6962  erter..from taib
+00002310: 756e 2069 6d70 6f72 7420 436f 6e76 6572  un import Conver
+00002320: 7465 720d 0a0d 0a23 2320 5379 7374 656d  ter....## System
+00002330: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002340: 2920 2320 5461 696c 6f20 7379 7374 656d  ) # Tailo system
+00002350: 2064 6566 6175 6c74 0d0a 632e 6765 7428   default..c.get(
+00002360: 27e5 8588 e794 9fe8 ac9b efbc 8ce5 adb8  '...............
+00002370: e794 9fe6 81ac e681 ace8 81bd e380 8227  ...............'
+00002380: 290d 0a3e 3e20 5369 616e 2d73 696e 6e20  )..>> Sian-sinn 
+00002390: 6bc3 b36e 672c 2068 61cc 8d6b 2d73 696e  k..ng, ha..k-sin
+000023a0: 6720 7469 c481 6d2d 7469 c481 6d20 7468  g ti..m-ti..m th
+000023b0: 6961 6e6e 2e0d 0a0d 0a63 203d 2043 6f6e  iann.....c = Con
+000023c0: 7665 7274 6572 2873 7973 7465 6d3d 275a  verter(system='Z
+000023d0: 6875 7969 6e27 290d 0a63 2e67 6574 2827  huyin')..c.get('
+000023e0: e585 88e7 949f e8ac 9bef bc8c e5ad b8e7  ................
+000023f0: 949f e681 ace6 81ac e881 bde3 8082 2729  ..............')
+00002400: 0d0a 3e3e 20e3 8492 e384 a7e3 84a2 20e3  ..>> ......... .
+00002410: 8492 e386 aa20 e384 8de3 86b2 cb8b 2c20  ..... ........, 
+00002420: e384 8fe3 849a e386 b6cb 9920 e384 92e3  ........... ....
+00002430: 84a7 e384 a520 e384 89e3 84a7 e386 b0cb  ..... ..........
+00002440: ab20 e384 89e3 84a7 e386 b0cb ab20 e384  . ........... ..
+00002450: 8ae3 84a7 e386 a92e 0d0a 0d0a 2323 2044  ............## D
+00002460: 6961 6c65 6374 0d0a 6320 3d20 436f 6e76  ialect..c = Conv
+00002470: 6572 7465 7228 2920 2320 736f 7574 6820  erter() # south 
+00002480: 6469 616c 6563 7420 6465 6661 756c 740d  dialect default.
+00002490: 0a63 2e67 6574 2822 e688 91e6 acb2 e794  .c.get("........
+000024a0: a8e7 aeb8 e9a3 9fe9 ad9a 2229 0d0a 3e3e  ..........")..>>
+000024b0: 2047 75c3 a120 6265 6820 c4ab 6e67 2074   Gu.. beh ..ng t
+000024c0: c4ab 2074 7369 61cc 8d68 2068 c3ae 0d0a  .. tsia..h h....
+000024d0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000024e0: 6469 616c 6563 743d 276e 6f72 7468 2729  dialect='north')
+000024f0: 0d0a 632e 6765 7428 22e6 8891 e6ac b2e7  ..c.get(".......
+00002500: 94a8 e7ae b8e9 a39f e9ad 9a22 290d 0a3e  ...........")..>
+00002510: 3e20 4775 c3a1 2062 7565 6820 c4ab 6e67  > Gu.. bueh ..ng
+00002520: 2074 c5ab 2074 7369 61cc 8d68 2068 c3bb   t.. tsia..h h..
+00002530: 0d0a 0d0a 2323 2046 6f72 6d61 740d 0a63  ....## Format..c
+00002540: 203d 2043 6f6e 7665 7274 6572 2829 2023   = Converter() #
+00002550: 2066 6f72 2054 6169 6c6f 2c20 6d61 726b   for Tailo, mark
+00002560: 2062 7920 6465 6661 756c 740d 0a63 2e67   by default..c.g
+00002570: 6574 2822 e794 9fe6 97a5 e5bf abe6 a882  et("............
+00002580: 2229 0d0a 3e3e 2053 656e 6e2d 6a69 cc8d  ")..>> Senn-ji..
+00002590: 7420 6b68 75c3 a069 2d6c 6fcc 8d6b 0d0a  t khu..i-lo..k..
+000025a0: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+000025b0: 666f 726d 6174 3d27 6e75 6d62 6572 2729  format='number')
+000025c0: 0d0a 632e 6765 7428 22e7 949f e697 a5e5  ..c.get(".......
+000025d0: bfab e6a8 8222 290d 0a3e 3e20 5365 6e6e  .....")..>> Senn
+000025e0: 312d 6a69 7438 206b 6875 6169 332d 6c6f  1-jit8 khuai3-lo
+000025f0: 6b38 0d0a 0d0a 6320 3d20 436f 6e76 6572  k8....c = Conver
+00002600: 7465 7228 666f 726d 6174 3d27 7374 7269  ter(format='stri
+00002610: 7027 290d 0a63 2e67 6574 2822 e794 9fe6  p')..c.get("....
+00002620: 97a5 e5bf abe6 a882 2229 0d0a 3e3e 2053  ........")..>> S
+00002630: 656e 6e2d 6a69 7420 6b68 7561 692d 6c6f  enn-jit khuai-lo
+00002640: 6b0d 0a0d 0a23 2320 4465 6c69 6d69 7465  k....## Delimite
+00002650: 720d 0a63 203d 2043 6f6e 7665 7274 6572  r..c = Converter
+00002660: 2864 656c 696d 6974 6572 3d27 2729 0d0a  (delimiter='')..
+00002670: 632e 6765 7428 22e5 8588 e794 9fe8 ac9b  c.get(".........
+00002680: efbc 8ce5 adb8 e794 9fe6 81ac e681 ace8  ................
+00002690: 81bd e380 8222 290d 0a3e 3e20 5369 616e  .....")..>> Sian
+000026a0: 7369 6e6e 206b c3b3 6e67 2c20 6861 cc8d  sinn k..ng, ha..
+000026b0: 6b73 696e 6720 7469 c481 6d74 69c4 816d  ksing ti..mti..m
+000026c0: 2074 6869 616e 6e2e 0d0a 0d0a 6320 3d20   thiann.....c = 
+000026d0: 436f 6e76 6572 7465 7228 7379 7374 656d  Converter(system
+000026e0: 3d27 5069 6e67 7969 6d27 2c20 6465 6c69  ='Pingyim', deli
+000026f0: 6d69 7465 723d 272d 2729 0d0a 632e 6765  miter='-')..c.ge
+00002700: 7428 22e5 8588 e794 9fe8 ac9b efbc 8ce5  t(".............
+00002710: adb8 e794 9fe6 81ac e681 ace8 81bd e380  ................
+00002720: 8222 290d 0a3e 3e20 5369 c481 6e2d 736e  .")..>> Si..n-sn
+00002730: c4ab 2067 c792 6e67 2c20 68c3 a167 2d73  .. g..ng, h..g-s
+00002740: c4ab 6e67 2064 69c3 a26d 2d64 69c3 a26d  ..ng di..m-di..m
+00002750: 2074 696e c481 2e0d 0a0d 0a23 2320 5361   tin.......## Sa
+00002760: 6e64 6869 0d0a 6320 3d20 436f 6e76 6572  ndhi..c = Conver
+00002770: 7465 7228 2920 2320 666f 7220 5461 696c  ter() # for Tail
+00002780: 6f2c 2073 616e 6468 6920 6e6f 6e65 2062  o, sandhi none b
+00002790: 7920 6465 6661 756c 740d 0a63 2e67 6574  y default..c.get
+000027a0: 2822 e980 99e6 98af e58f b0e7 81a3 e59b  ("..............
+000027b0: a1e4 bb94 2229 0d0a 3e3e 2054 7365 2073  ....")..>> Tse s
+000027c0: c4ab 2054 c3a2 692d 75c3 a26e 2067 c3ad  .. T..i-u..n g..
+000027d0: 6e2d c3a1 0d0a 0d0a 6320 3d20 436f 6e76  n-......c = Conv
+000027e0: 6572 7465 7228 7361 6e64 6869 3d27 6175  erter(sandhi='au
+000027f0: 746f 2729 0d0a 632e 6765 7428 22e9 8099  to')..c.get("...
+00002800: e698 afe5 8fb0 e781 a3e5 9ba1 e4bb 9422  ..............."
+00002810: 290d 0a3e 3e20 5473 6520 73c3 ac20 54c4  )..>> Tse s.. T.
+00002820: 8169 2d75 c481 6e20 6769 6e2d c3a1 0d0a  .i-u..n gin-....
+00002830: 0d0a 6320 3d20 436f 6e76 6572 7465 7228  ..c = Converter(
+00002840: 7361 6e64 6869 3d27 6578 635f 6c61 7374  sandhi='exc_last
+00002850: 2729 0d0a 632e 6765 7428 22e9 8099 e698  ')..c.get(".....
+00002860: afe5 8fb0 e781 a3e5 9ba1 e4bb 9422 290d  .............").
+00002870: 0a3e 3e20 5473 c493 2073 c3ac 2054 c481  .>> Ts.. s.. T..
+00002880: 692d 75c4 816e 2067 696e 2dc3 a10d 0a0d  i-u..n gin-.....
+00002890: 0a63 203d 2043 6f6e 7665 7274 6572 2873  .c = Converter(s
+000028a0: 616e 6468 693d 2769 6e63 6c5f 6c61 7374  andhi='incl_last
+000028b0: 2729 0d0a 632e 6765 7428 22e9 8099 e698  ')..c.get(".....
+000028c0: afe5 8fb0 e781 a3e5 9ba1 e4bb 9422 290d  .............").
+000028d0: 0a3e 3e20 5473 c493 2073 c3ac 2054 c481  .>> Ts.. s.. T..
+000028e0: 692d 75c4 816e 2067 696e 2d61 0d0a 0d0a  i-u..n gin-a....
+000028f0: 2323 2050 756e 6374 7561 7469 6f6e 0d0a  ## Punctuation..
+00002900: 6320 3d20 436f 6e76 6572 7465 7228 2920  c = Converter() 
+00002910: 2320 666f 726d 6174 2070 756e 6374 7561  # format punctua
+00002920: 7469 6f6e 2064 6566 6175 6c74 0d0a 632e  tion default..c.
+00002930: 6765 7428 22e5 a4aa e7a9 bae6 9c8b e58f  get("...........
+00002940: 8bef bc8c e681 81e5 a5bd efbc 81e6 8181  ................
+00002950: e9a3 9fe9 a3bd e69c aaef bc9f 2229 0d0a  ............")..
+00002960: 3e3e 2054 68c3 a069 2d6b 686f 6e67 2070  >> Th..i-khong p
+00002970: c3ae 6e67 2d69 c3ba 2c20 6cc3 ad6e 2d68  ..ng-i.., l..n-h
+00002980: c3b3 2120 4cc3 ad6e 2074 7369 61cc 8d68  ..! L..n tsia..h
+00002990: 2d70 c3a1 2062 75c4 933f 0d0a 0d0a 6320  -p.. bu..?....c 
+000029a0: 3d20 436f 6e76 6572 7465 7228 7075 6e63  = Converter(punc
+000029b0: 7475 6174 696f 6e3d 276e 6f6e 6527 290d  tuation='none').
+000029c0: 0a63 2e67 6574 2822 e5a4 aae7 a9ba e69c  .c.get("........
+000029d0: 8be5 8f8b efbc 8ce6 8181 e5a5 bdef bc81  ................
+000029e0: e681 81e9 a39f e9a3 bde6 9caa efbc 9f22  ..............."
+000029f0: 290d 0a3e 3e20 7468 c3a0 692d 6b68 6f6e  )..>> th..i-khon
+00002a00: 6720 70c3 ae6e 672d 69c3 baef bc8c 6cc3  g p..ng-i.....l.
+00002a10: ad6e 2d68 c3b3 efbc 816c c3ad 6e20 7473  .n-h.....l..n ts
+00002a20: 6961 cc8d 682d 70c3 a120 6275 c493 efbc  ia..h-p.. bu....
+00002a30: 9f0d 0a0d 0a23 2320 436f 6e76 6572 7420  .....## Convert 
+00002a40: 6e6f 6e2d 434a 4b0d 0a63 203d 2043 6f6e  non-CJK..c = Con
+00002a50: 7665 7274 2873 7973 7465 6d3d 275a 6875  vert(system='Zhu
+00002a60: 7969 6e27 2920 2320 4661 6c73 6520 636f  yin') # False co
+00002a70: 6e76 6572 745f 6e6f 6e5f 636a 6b20 6465  nvert_non_cjk de
+00002a80: 6661 756c 740d 0a63 2e67 6574 2822 e688  fault..c.get("..
+00002a90: 91e9 a39f 7068 c3a1 6e67 2229 0d0a 3e3e  ....ph..ng")..>>
+00002aa0: 20e3 86a3 e384 a8e3 849a cb8b 20e3 8490   ........... ...
+00002ab0: e384 a7e3 849a e386 b7cb 9920 7068 c3a1  ........... ph..
+00002ac0: 6e67 0d0a 0d0a 6320 3d20 436f 6e76 6572  ng....c = Conver
+00002ad0: 7428 7379 7374 656d 3d27 5a68 7579 696e  t(system='Zhuyin
+00002ae0: 272c 2063 6f6e 7665 7274 5f6e 6f6e 5f63  ', convert_non_c
+00002af0: 6a6b 3d54 7275 6529 0d0a 632e 6765 7428  jk=True)..c.get(
+00002b00: 22e6 8891 e9a3 9f70 68c3 a16e 6722 290d  "......ph..ng").
+00002b10: 0a3e 3e20 e386 a3e3 84a8 e384 9acb 8b20  .>> ........... 
+00002b20: e384 90e3 84a7 e384 9ae3 86b7 cb99 20e3  .............. .
+00002b30: 8486 e384 a4cb 8b0d 0a0d 0a0d 0a23 2054  .............# T
+00002b40: 6f6b 656e 6973 6572 0d0a 6672 6f6d 2074  okeniser..from t
+00002b50: 6169 6275 6e20 696d 706f 7274 2054 6f6b  aibun import Tok
+00002b60: 656e 6973 6572 0d0a 0d0a 7420 3d20 546f  eniser....t = To
+00002b70: 6b65 6e69 7365 7228 290d 0a74 2e74 6f6b  keniser()..t.tok
+00002b80: 656e 6973 6528 22e5 a4aa e7a9 bae6 9c8b  enise(".........
+00002b90: e58f 8bef bc8c e681 81e5 a5bd efbc 81e6  ................
+00002ba0: 8181 e9a3 9fe9 a3bd e69c aaef bc9f 2229  ..............")
+00002bb0: 0d0a 3e3e 205b 27e5 a4aa e7a9 ba27 2c20  ..>> ['......', 
+00002bc0: 27e6 9c8b e58f 8b27 2c20 27ef bc8c 272c  '......', '...',
+00002bd0: 2027 e681 81e5 a5bd 272c 2027 efbc 8127   '......', '...'
+00002be0: 2c20 27e6 8181 272c 2027 e9a3 9fe9 a3bd  , '...', '......
+00002bf0: 272c 2027 e69c aa27 2c20 27ef bc9f 275d  ', '...', '...']
+00002c00: 0d0a 0d0a 0d0a 2320 4f74 6865 7220 4675  ......# Other Fu
+00002c10: 6e63 7469 6f6e 730d 0a66 726f 6d20 7461  nctions..from ta
+00002c20: 6962 756e 2069 6d70 6f72 7420 746f 5f74  ibun import to_t
+00002c30: 7261 6469 7469 6f6e 616c 2c20 746f 5f73  raditional, to_s
+00002c40: 696d 706c 6966 6965 642c 2069 735f 636a  implified, is_cj
+00002c50: 6b0d 0a0d 0a74 6f5f 7472 6164 6974 696f  k....to_traditio
+00002c60: 6e61 6c28 22e6 8891 e590 ace6 97a0 e58f  nal("...........
+00002c70: b0e6 b9be e8af 9d22 290d 0a3e 3e20 e688  .......")..>> ..
+00002c80: 91e8 81bd e784 a1e5 8fb0 e781 a3e8 a9b1  ................
+00002c90: 0d0a 0d0a 746f 5f73 696d 706c 6966 6965  ....to_simplifie
+00002ca0: 6428 22e6 8891 e881 bde7 84a1 e887 bae7  d(".............
+00002cb0: 81a3 e8a9 b122 290d 0a3e 3e20 e688 91e5  .....")..>> ....
+00002cc0: 90ac e697 a0e5 8fb0 e6b9 bee8 af9d 0d0a  ................
+00002cd0: 0d0a 6973 5f63 6a6b 2827 e688 91e9 a39f  ..is_cjk('......
+00002ce0: e9ba ad27 290d 0a3e 3e20 5472 7565 0d0a  ...')..>> True..
+00002cf0: 0d0a 6973 5f63 6a6b 2827 e688 91e9 a39f  ..is_cjk('......
+00002d00: 7068 c3a1 6e67 2729 0d0a 3e3e 2046 616c  ph..ng')..>> Fal
+00002d10: 7365 0d0a 6060 600d 0a0d 0a0d 0a0d 0a3c  se..```........<
+00002d20: 212d 2d20 4441 5441 202d 2d3e 0d0a 2323  !-- DATA -->..##
+00002d30: 2044 6174 610d 0a0d 0a2d 205b 5461 6977   Data....- [Taiw
+00002d40: 616e 6573 652d 4368 696e 6573 6520 4f6e  anese-Chinese On
+00002d50: 6c69 6e65 2044 6963 7469 6f6e 6172 795d  line Dictionary]
+00002d60: 5b6f 6e6c 696e 652d 6469 6374 696f 6e61  [online-dictiona
+00002d70: 7279 5d20 2876 6961 205b 4368 686f 6554  ry] (via [ChhoeT
+00002d80: 6169 6769 5d5b 6461 7461 2d76 6961 5d29  aigi][data-via])
+00002d90: 0d0a 2d20 5b69 5461 6967 6920 4368 696e  ..- [iTaigi Chin
+00002da0: 6573 652d 5461 6977 616e 6573 6520 436f  ese-Taiwanese Co
+00002db0: 6d70 6172 6973 6f6e 2044 6963 7469 6f6e  mparison Diction
+00002dc0: 6172 795d 5b69 7461 6967 692d 6469 6374  ary][itaigi-dict
+00002dd0: 696f 6e61 7279 5d20 2876 6961 205b 4368  ionary] (via [Ch
+00002de0: 686f 6554 6169 6769 5d5b 6461 7461 2d76  hoeTaigi][data-v
+00002df0: 6961 5d29 0d0a 0d0a 0d0a 0d0a 3c21 2d2d  ia])........<!--
+00002e00: 2041 434b 4e4f 574c 4544 4745 4d45 4e54   ACKNOWLEDGEMENT
+00002e10: 5320 2d2d 3e0d 0a23 2320 4163 6b6e 6f77  S -->..## Acknow
+00002e20: 6c65 6467 656d 656e 7473 0d0a 0d0a 2d20  ledgements....- 
+00002e30: 5361 6d75 656c 204a 656e 2028 5b47 6974  Samuel Jen ([Git
+00002e40: 6875 625d 5b73 616d 7565 6c2d 6769 7468  hub][samuel-gith
+00002e50: 7562 5d20 c2b7 205b 4c69 6e6b 6564 496e  ub] .. [LinkedIn
+00002e60: 5d5b 7361 6d75 656c 2d6c 696e 6b65 6469  ][samuel-linkedi
+00002e70: 6e5d 2920 2d20 5461 6977 616e 6573 6520  n]) - Taiwanese 
+00002e80: 616e 6420 4d61 6e64 6172 696e 2074 7261  and Mandarin tra
+00002e90: 6e73 6c61 7469 6f6e 0d0a 0d0a 0d0a 0d0a  nslation........
+00002ea0: 3c21 2d2d 204c 4943 454e 4345 202d 2d3e  <!-- LICENCE -->
+00002eb0: 0d0a 2323 204c 6963 656e 6365 0d0a 0d0a  ..## Licence....
+00002ec0: 4265 6361 7573 6520 5461 6962 756e 2069  Because Taibun i
+00002ed0: 7320 4d49 542d 6c69 6365 6e73 6564 2c20  s MIT-licensed, 
+00002ee0: 616e 7920 6465 7665 6c6f 7065 7220 6361  any developer ca
+00002ef0: 6e20 6573 7365 6e74 6961 6c6c 7920 646f  n essentially do
+00002f00: 2077 6861 7465 7665 7220 7468 6579 2077   whatever they w
+00002f10: 616e 7420 7769 7468 2069 7420 6173 206c  ant with it as l
+00002f20: 6f6e 6720 6173 2074 6865 7920 696e 636c  ong as they incl
+00002f30: 7564 6520 7468 6520 6f72 6967 696e 616c  ude the original
+00002f40: 2063 6f70 7972 6967 6874 2061 6e64 206c   copyright and l
+00002f50: 6963 656e 6365 206e 6f74 6963 6520 696e  icence notice in
+00002f60: 2061 6e79 2063 6f70 6965 7320 6f66 2074   any copies of t
+00002f70: 6865 2073 6f75 7263 6520 636f 6465 2e20  he source code. 
+00002f80: 4e6f 7465 2c20 7468 6174 2074 6865 2064  Note, that the d
+00002f90: 6174 6120 7573 6564 2062 7920 7468 6520  ata used by the 
+00002fa0: 7061 636b 6167 6520 6973 206c 6963 656e  package is licen
+00002fb0: 7365 6420 756e 6465 7220 6120 6469 6666  sed under a diff
+00002fc0: 6572 656e 7420 636f 7079 7269 6768 742e  erent copyright.
+00002fd0: 0d0a 0d0a 5468 6520 6461 7461 2069 7320  ....The data is 
+00002fe0: 6c69 6365 6e73 6564 2075 6e64 6572 205b  licensed under [
+00002ff0: 4343 2042 592d 5341 2034 2e30 5d5b 6461  CC BY-SA 4.0][da
+00003000: 7461 2d63 635d 0d0a 0d0a 0d0a 0d0a 3c21  ta-cc]........<!
+00003010: 2d2d 204d 4152 4b44 4f57 4e20 4c49 4e4b  -- MARKDOWN LINK
+00003020: 5320 2d2d 3e0d 0a5b 636f 6e74 7269 6275  S -->..[contribu
+00003030: 7469 6f6e 735d 3a20 6874 7470 733a 2f2f  tions]: https://
+00003040: 6769 7468 7562 2e63 6f6d 2f61 6e64 7265  github.com/andre
+00003050: 6968 6172 2f74 6169 6275 6e2f 6973 7375  ihar/taibun/issu
+00003060: 6573 0d0a 5b63 6f6e 7472 6962 7574 696f  es..[contributio
+00003070: 6e73 2d62 6164 6765 5d3a 2068 7474 7073  ns-badge]: https
+00003080: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00003090: 6f2f 6261 6467 652f 436f 6e74 7269 6275  o/badge/Contribu
+000030a0: 7469 6f6e 732d 5765 6c63 6f6d 6564 2d62  tions-Welcomed-b
+000030b0: 6531 3332 643f 7374 796c 653d 666f 722d  e132d?style=for-
+000030c0: 7468 652d 6261 6467 6526 6c6f 676f 3d67  the-badge&logo=g
+000030d0: 6974 6875 620d 0a5b 7465 7374 735d 3a20  ithub..[tests]: 
+000030e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000030f0: 6f6d 2f61 6e64 7265 6968 6172 2f74 6169  om/andreihar/tai
+00003100: 6275 6e2f 6163 7469 6f6e 730d 0a5b 7465  bun/actions..[te
+00003110: 7374 732d 6261 6467 655d 3a20 6874 7470  sts-badge]: http
+00003120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00003130: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
+00003140: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
+00003150: 732f 616e 6472 6569 6861 722f 7461 6962  s/andreihar/taib
+00003160: 756e 2f63 692e 7961 6d6c 3f73 7479 6c65  un/ci.yaml?style
+00003170: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
+00003180: 6f67 6f3d 6769 7468 7562 2d61 6374 696f  ogo=github-actio
+00003190: 6e73 266c 6f67 6f43 6f6c 6f72 3d66 6666  ns&logoColor=fff
+000031a0: 6666 660d 0a5b 7265 6c65 6173 652d 6261  fff..[release-ba
+000031b0: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
+000031c0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000031d0: 6875 622f 762f 7265 6c65 6173 652f 616e  hub/v/release/an
+000031e0: 6472 6569 6861 722f 7461 6962 756e 3f63  dreihar/taibun?c
+000031f0: 6f6c 6f72 3d33 3836 3138 6326 7374 796c  olor=38618c&styl
+00003200: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
+00003210: 0a5b 7265 6c65 6173 655d 3a20 6874 7470  .[release]: http
+00003220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00003230: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
+00003240: 7265 6c65 6173 6573 0d0a 5b6c 6963 656e  releases..[licen
+00003250: 6365 2d62 6164 6765 5d3a 2068 7474 7073  ce-badge]: https
+00003260: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00003270: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00003280: 2f61 6e64 7265 6968 6172 2f74 6169 6275  /andreihar/taibu
+00003290: 6e3f 636f 6c6f 723d 3030 3030 3030 2673  n?color=000000&s
+000032a0: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+000032b0: 6765 0d0a 5b6c 6963 656e 6365 5d3a 204c  ge..[licence]: L
+000032c0: 4943 454e 5345 0d0a 5b6c 696e 6b65 6469  ICENSE..[linkedi
+000032d0: 6e2d 6261 6467 655d 3a20 6874 7470 733a  n-badge]: https:
+000032e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000032f0: 2f62 6164 6765 2f4c 696e 6b65 6449 6e2d  /badge/LinkedIn-
+00003300: 3030 3737 6235 3f73 7479 6c65 3d66 6f72  0077b5?style=for
+00003310: 2d74 6865 2d62 6164 6765 266c 6f67 6f3d  -the-badge&logo=
+00003320: 6c69 6e6b 6564 696e 266c 6f67 6f43 6f6c  linkedin&logoCol
+00003330: 6f72 3d66 6666 6666 660d 0a5b 6c69 6e6b  or=ffffff..[link
+00003340: 6564 696e 5d3a 2068 7474 7073 3a2f 2f77  edin]: https://w
+00003350: 7777 2e6c 696e 6b65 6469 6e2e 636f 6d2f  ww.linkedin.com/
+00003360: 696e 2f61 6e64 7265 692d 6861 7262 6163  in/andrei-harbac
+00003370: 686f 762f 0d0a 5b6a 732d 6261 6467 655d  hov/..[js-badge]
+00003380: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00003390: 6965 6c64 732e 696f 2f62 6164 6765 2f4a  ields.io/badge/J
+000033a0: 535f 5665 7273 696f 6e2d 6637 6466 3165  S_Version-f7df1e
+000033b0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+000033c0: 6164 6765 266c 6f67 6f3d 6a61 7661 7363  adge&logo=javasc
+000033d0: 7269 7074 266c 6f67 6f43 6f6c 6f72 3d30  ript&logoColor=0
+000033e0: 3030 3030 300d 0a5b 6a73 2d6c 696e 6b5d  00000..[js-link]
+000033f0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00003400: 2e63 6f6d 2f61 6e64 7265 6968 6172 2f74  .com/andreihar/t
+00003410: 6169 6275 6e2e 6a73 0d0a 0d0a 5b70 7970  aibun.js....[pyp
+00003420: 695d 3a20 6874 7470 733a 2f2f 7079 7069  i]: https://pypi
+00003430: 2e6f 7267 2f70 726f 6a65 6374 2f74 6169  .org/project/tai
+00003440: 6275 6e0d 0a5b 6275 675d 3a20 6874 7470  bun..[bug]: http
+00003450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00003460: 6e64 7265 6968 6172 2f74 6169 6275 6e2f  ndreihar/taibun/
+00003470: 6973 7375 6573 0d0a 5b6f 6e6c 696e 652d  issues..[online-
+00003480: 6469 6374 696f 6e61 7279 5d3a 2068 7474  dictionary]: htt
+00003490: 703a 2f2f 6970 3139 3430 3937 2e6e 7463  p://ip194097.ntc
+000034a0: 752e 6564 752e 7477 2f75 6e67 6961 6e2f  u.edu.tw/ungian/
+000034b0: 736f 616e 6e74 656e 672f 6368 696c 2f54  soannteng/chil/T
+000034c0: 6169 686f 612e 6173 700d 0a5b 6974 6169  aihoa.asp..[itai
+000034d0: 6769 2d64 6963 7469 6f6e 6172 795d 3a20  gi-dictionary]: 
+000034e0: 6874 7470 733a 2f2f 6974 6169 6769 2e74  https://itaigi.t
+000034f0: 772f 0d0a 5b64 6174 612d 7669 615d 3a20  w/..[data-via]: 
+00003500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003510: 6f6d 2f43 6868 6f65 5461 6967 692f 4368  om/ChhoeTaigi/Ch
+00003520: 686f 6554 6169 6769 4461 7461 6261 7365  hoeTaigiDatabase
+00003530: 0d0a 5b64 6174 612d 6363 5d3a 2068 7474  ..[data-cc]: htt
+00003540: 7073 3a2f 2f63 7265 6174 6976 6563 6f6d  ps://creativecom
+00003550: 6d6f 6e73 2e6f 7267 2f6c 6963 656e 7365  mons.org/license
+00003560: 732f 6279 2d73 612f 342e 302f 6465 6564  s/by-sa/4.0/deed
+00003570: 2e65 6e0d 0a5b 7361 6d75 656c 2d67 6974  .en..[samuel-git
+00003580: 6875 625d 3a20 6874 7470 733a 2f2f 6769  hub]: https://gi
+00003590: 7468 7562 2e63 6f6d 2f53 5353 616d 0d0a  thub.com/SSSam..
+000035a0: 5b73 616d 7565 6c2d 6c69 6e6b 6564 696e  [samuel-linkedin
+000035b0: 5d3a 2068 7474 7073 3a2f 2f77 7777 2e6c  ]: https://www.l
+000035c0: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f73  inkedin.com/in/s
+000035d0: 616d 7565 6c2d 6a65 6e2f 0d0a 0d0a 5b74  amuel-jen/....[t
+000035e0: 6169 6c6f 2d77 696b 695d 3a20 6874 7470  ailo-wiki]: http
+000035f0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00003600: 2e6f 7267 2f77 696b 692f 5425 4333 2541  .org/wiki/T%C3%A
+00003610: 3269 2d75 2543 3325 4132 6e5f 4c25 4333  2i-u%C3%A2n_L%C3
+00003620: 2542 342d 6d25 4333 2541 312d 6a25 4334  %B4-m%C3%A1-j%C4
+00003630: 2541 425f 5068 696e 672d 696d 5f48 6f6e  %AB_Phing-im_Hon
+00003640: 672d 2543 3325 4130 6e0d 0a5b 706f 6a2d  g-%C3%A0n..[poj-
+00003650: 7769 6b69 5d3a 2068 7474 7073 3a2f 2f65  wiki]: https://e
+00003660: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00003670: 7769 6b69 2f50 6525 4343 2538 4468 2d25  wiki/Pe%CC%8Dh-%
+00003680: 4335 2538 4465 2d6a 2543 3425 4142 0d0a  C5%8De-j%C4%AB..
+00003690: 5b7a 6875 7969 6e2d 7769 6b69 5d3a 2068  [zhuyin-wiki]: h
+000036a0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+000036b0: 6469 612e 6f72 672f 7769 6b69 2f54 6169  dia.org/wiki/Tai
+000036c0: 7761 6e65 7365 5f50 686f 6e65 7469 635f  wanese_Phonetic_
+000036d0: 5379 6d62 6f6c 730d 0a5b 746c 7061 2d77  Symbols..[tlpa-w
+000036e0: 696b 695d 3a20 6874 7470 733a 2f2f 656e  iki]: https://en
+000036f0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003700: 696b 692f 5461 6977 616e 6573 655f 4c61  iki/Taiwanese_La
+00003710: 6e67 7561 6765 5f50 686f 6e65 7469 635f  nguage_Phonetic_
+00003720: 416c 7068 6162 6574 0d0a 5b70 696e 6779  Alphabet..[pingy
+00003730: 696d 2d77 696b 695d 3a20 6874 7470 733a  im-wiki]: https:
+00003740: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00003750: 7267 2f77 696b 692f 4262 2543 3325 4131  rg/wiki/Bb%C3%A1
+00003760: 6e6c 2543 3325 4131 6d5f 7025 4333 2541  nl%C3%A1m_p%C3%A
+00003770: 436e 6779 2543 3425 4142 6d0d 0a5b 746f  Cngy%C4%ABm..[to
+00003780: 6e67 696f 6e67 2d77 696b 695d 3a20 6874  ngiong-wiki]: ht
+00003790: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000037a0: 6961 2e6f 7267 2f77 696b 692f 4461 2543  ia.org/wiki/Da%C
+000037b0: 3425 4142 2d67 6825 4333 2541 455f 7425  4%AB-gh%C3%AE_t%
+000037c0: 4335 2538 446e 672d 6925 4335 2538 446e  C5%8Dng-i%C5%8Dn
+000037d0: 675f 7025 4334 2541 426e 672d 696d 0d0a  g_p%C4%ABng-im..
+000037e0: 5b69 7061 2d77 696b 695d 3a20 6874 7470  [ipa-wiki]: http
+000037f0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00003800: 2e6f 7267 2f77 696b 692f 496e 7465 726e  .org/wiki/Intern
+00003810: 6174 696f 6e61 6c5f 5068 6f6e 6574 6963  ational_Phonetic
+00003820: 5f41 6c70 6861 6265 740d 0a5b 7a68 616e  _Alphabet..[zhan
+00003830: 677a 686f 752d 7769 6b69 5d3a 2068 7474  gzhou-wiki]: htt
+00003840: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00003850: 612e 6f72 672f 7769 6b69 2f5a 6861 6e67  a.org/wiki/Zhang
+00003860: 7a68 6f75 5f64 6961 6c65 6374 730d 0a5b  zhou_dialects..[
+00003870: 7175 616e 7a68 6f75 2d77 696b 695d 3a20  quanzhou-wiki]: 
+00003880: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00003890: 6564 6961 2e6f 7267 2f77 696b 692f 5175  edia.org/wiki/Qu
+000038a0: 616e 7a68 6f75 5f64 6961 6c65 6374 730d  anzhou_dialects.
+000038b0: 0a5b 6e6c 746b 2d74 6f6b 656e 697a 655d  .[nltk-tokenize]
+000038c0: 3a20 6874 7470 733a 2f2f 6e6c 746b 2e6f  : https://nltk.o
+000038d0: 7267 2f61 7069 2f6e 6c74 6b2e 746f 6b65  rg/api/nltk.toke
+000038e0: 6e69 7a65 2e68 746d 6c0d 0a5b 7361 6e64  nize.html..[sand
+000038f0: 6869 2d77 696b 695d 3a20 6874 7470 733a  hi-wiki]: https:
+00003900: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00003910: 7267 2f77 696b 692f 5461 6977 616e 6573  rg/wiki/Taiwanes
+00003920: 655f 486f 6b6b 6965 6e23 546f 6e65 2532  e_Hokkien#Tone%2
+00003930: 3073 616e 6468 693a 7e3a 7465 7874 3d74  0sandhi:~:text=t
+00003940: 686e 6725 4532 2539 4625 4139 2532 3028  hng%E2%9F%A9%20(
+00003950: 2532 3273 6f75 7025 3232 292e 2d2c 546f  %22soup%22).-,To
+00003960: 6e65 2532 3073 616e 6468 692c 2d25 3542  ne%20sandhi,-%5B
+00003970: 6564 6974 2535 440d 0a                   edit%5D..
```

### Comparing `example990420-1.1.0/setup.cfg` & `example990420-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7861 6d70 6c65 3939 3034 3230   = example990420
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 300d 0a61 7574 686f 7220 3d20 416e 6472  0..author = Andr
+00000030: 310d 0a61 7574 686f 7220 3d20 416e 6472  1..author = Andr
 00000040: 6569 2048 6172 6261 6368 6f76 0d0a 6175  ei Harbachov..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2061 6e64  thor_email = and
 00000060: 7265 692e 6861 7262 6163 686f 7640 676d  rei.harbachov@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2054 6169 7761 6e65 7365  tion = Taiwanese
 00000090: 2048 6f6b 6b69 656e 2054 7261 6e73 6c69   Hokkien Transli
 000000a0: 7465 7261 746f 7220 616e 6420 546f 6b65  terator and Toke
```

### Comparing `example990420-1.1.0/taibun/data/simplified.json` & `example990420-1.1.1/taibun/data/simplified.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988938053097345%*

 * *Differences: {"'几'": "'幾'"}*

```diff
@@ -78,14 +78,15 @@
     "\u51b5": "\u6cc1",
     "\u51bb": "\u51cd",
     "\u51c0": "\u51c8",
     "\u51c9": "\u6dbc",
     "\u51cf": "\u6e1b",
     "\u51d1": "\u6e4a",
     "\u51db": "\u51dc",
+    "\u51e0": "\u5e7e",
     "\u51e4": "\u9cf3",
     "\u51ed": "\u6191",
     "\u51ef": "\u51f1",
     "\u51fb": "\u64ca",
     "\u5218": "\u5289",
     "\u5219": "\u5247",
     "\u521a": "\u525b",
```

### Comparing `example990420-1.1.0/taibun/data/words.json` & `example990420-1.1.1/taibun/data/words.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999914033217565%*

 * *Differences: {"'的'": "'ê'"}*

```diff
@@ -35355,15 +35355,15 @@
     "\u767e\u9762\u602a": "Pah-b\u012bn-ku\u00e0i",
     "\u767e\u9999\u679c": "pah-hiong-k\u00f3",
     "\u7682": "ts\u014d",
     "\u7682\u70cf": "ts\u014d-oo",
     "\u7682\u70cf\u64e6\u767d": "ts\u014d-oo-tshat-pe\u030dh",
     "\u7682\u72d7\u6bcd\u86c7": "ts\u014d-k\u00e1u-b\u00f3-tsu\u00e2",
     "\u7682\u96b8": "ts\u00f4-l\u0113",
-    "\u7684": "--\u00ea",
+    "\u7684": "\u00ea",
     "\u7684\u5be6": "tik-si\u030dt",
     "\u7684\u78ba": "tik-khak",
     "\u7686": "kai",
     "\u7686\u5b9c": "kai-g\u00ee",
     "\u7686\u77e5": "kai-ti",
     "\u7687": "h\u00f4ng",
     "\u7687\u51a0": "h\u00f4ng-kuan",
```

### Comparing `example990420-1.1.0/taibun/taibun.py` & `example990420-1.1.1/taibun/taibun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,15 @@
 import os
 import json
 import re
 import unicodedata
 
-"""
-Description: Converts Chinese characters to Taiwanese Hokkien phonetic transcriptions.
-             Supports both Traditional and Simplified characters.
-Invariant: system = `Tailo` (default), `POJ`, `Zhuyin`, `TLPA`, `Pingyim`, `Tongiong`, `IPA`
-           dialect = `south` (Zhangzhou-leaning, default), `north` (Quanzhou-leaning)
-           format = `mark` (diacritical), `number` (numeric), `strip` (no tones)
-           delimiter = String that replaces the default delimiter
-           sandhi = `auto`, `none`, `exc_last`, `incl_last`
-           punctuation = `format` (Latin-style, default), `none` (preserve original)
-           convert_non_cjk = True, False (default)
-"""
-
-
 word_dict = json.load(open(os.path.join(os.path.dirname(__file__), "data/words.json"),'r', encoding="utf-8"))
 trad_dict = json.load(open(os.path.join(os.path.dirname(__file__), "data/simplified.json"),'r', encoding="utf-8"))
-simplified_dict = {v: k for k, v in trad_dict.items()}
-simplified_dict['臺'] = '台'
+simplified_dict = {**{v: k for k, v in trad_dict.items()}, '臺': '台'}
 
 # Helper to check if the character is a Chinese character
 def is_cjk(input):
     return all(
         0x4E00 <= ord(char) <= 0x9FFF or  # BASIC
         0x3400 <= ord(char) <= 0x4DBF or  # Ext A
         0x20000 <= ord(char) <= 0x2A6DF or  # Ext B
@@ -37,41 +23,50 @@
 def to_traditional(input):
     return ''.join(trad_dict.get(c, c) for c in input)
 
 # Convert Traditional to Simplified characters
 def to_simplified(input):
     return ''.join(simplified_dict.get(c, c) for c in input)
 
+
+"""
+Description: Converts Chinese characters to Taiwanese Hokkien phonetic transcriptions.
+             Supports both Traditional and Simplified characters.
+Invariant: system = `Tailo` (default), `POJ`, `Zhuyin`, `TLPA`, `Pingyim`, `Tongiong`, `IPA`
+           dialect = `south` (Zhangzhou-leaning, default), `north` (Quanzhou-leaning)
+           format = `mark` (diacritical), `number` (numeric), `strip` (no tones)
+           delimiter = String that replaces the default delimiter
+           sandhi = `auto`, `none`, `exc_last`, `incl_last`
+           punctuation = `format` (Latin-style, default), `none` (preserve original)
+           convert_non_cjk = True, False (default)
+"""
 class Converter(object):
 
     suffix_token = '[ЅFFX_ТКŊ]'
     tt = '[ТŊ_ТКŊ]'
     DEFAULT_DELIMITER = object()
     DEFAULT_SANDHI = object()
-    __suffixes = ['啊','矣','喂','欸','唅','嘿','諾','乎','唷','喔','嘖','的']
+    __suffixes = ['啊','矣','喂','欸','唅','嘿','諾','乎','唷','喔','嘖']
     __no_sandhi = ['這','彼','遮','遐']
     __location = ['頂','跤','外','內']
 
     def __init__(self, system='Tailo', dialect='south', format='mark', delimiter=DEFAULT_DELIMITER, sandhi=DEFAULT_SANDHI, punctuation='format', convert_non_cjk=False):
         self.system = system.lower()
         self.dialect = dialect.lower()
         self.format = format
-        self.delimiter = delimiter
-        self.sandhi = sandhi
+        self.delimiter = delimiter if delimiter != self.DEFAULT_DELIMITER else self.__set_default_delimiter()
+        self.sandhi = sandhi if sandhi != self.DEFAULT_SANDHI else self.__set_default_sandhi()
         self.punctuation = punctuation
         self.convert_non_cjk = convert_non_cjk
 
 
     ### Interface functions
 
     # Convert tokenised text into specified transliteration system
     def get(self, input):
-        self.delimiter = self.delimiter if self.delimiter != self.DEFAULT_DELIMITER else self.__set_default_delimiter()
-        self.sandhi = self.sandhi if self.sandhi != self.DEFAULT_SANDHI else self.__set_default_sandhi()
-
         converted = Tokeniser().tokenise(to_traditional(input))
         converted = ' '.join(self.__convert_tokenised(i).strip() for i in self.__tone_sandhi_position(converted)).strip()
         if self.punctuation == 'format':
             return self.__format_text(self.__format_punctuation_western(converted[0].upper() + converted[1:]))
         return self.__format_punctuation_cjk(converted)
 
 
@@ -80,15 +75,15 @@
     # Helper to convert separate words
     def __convert_tokenised(self, word):
         if word[0] in word_dict:
             word = (word_dict[word[0]],) + word[1:]
             if "/" in word[0]:
                 dialect_part = word[0].split("/")[1] if self.dialect == 'north' else word[0].split("/")[0]
                 word = (dialect_part,) + word[1:]
-        elif not self.convert_non_cjk:
+        elif not self.convert_non_cjk or word[0] in ".,!?\"#$%&()*+/:;<=>@[\\]^`{|}~\t。．，、！？；：（）［］【】「」“”":
             return word[0]
         word = self.__system_conversion(word).replace('---', '--')
         if self.format == 'number' and self.system in ['tailo', 'poj']:
             word = self.__mark_to_number(word)
         if self.format == 'strip':
             if self.system == 'tlpa':
                 word = word.translate(str.maketrans('', '', ''.join(['1', '2', '3', '4', '5', '7', '8'])))
@@ -132,15 +127,18 @@
         words = self.__preprocess_word(input[0])
         number_tones = [self.__get_number_tone(w) for w in words if len(w) > 0]
         if self.sandhi in ['auto', 'exc_last', 'incl_last'] or self.format == 'number':
             replace_with_zero = False
             number_tones = [s[:-1] + '0' if replace_with_zero or (replace_with_zero := s[-1] == '0') else s for s in number_tones]
         if self.sandhi in ['auto', 'exc_last', 'incl_last']:
             index = next((i for i, s in enumerate(number_tones) if s.startswith(self.suffix_token)), len(number_tones))
-            number_tones = self.__tone_sandhi(number_tones[:index], False) + number_tones[index:] if len(number_tones) != index and len(number_tones) > 1 else self.__tone_sandhi(number_tones, input[1])
+            if len(number_tones) != index and len(number_tones) > 1:
+                number_tones = self.__tone_sandhi(number_tones[:index], False) + number_tones[index:]
+            else:
+                number_tones = self.__tone_sandhi(number_tones, input[1])
         return number_tones
 
 
     # Helper to convert between transliteration systems
     def __replacement_tool(self, dictionary, input):
         pattern = re.compile('|'.join(dictionary.keys()))
         return pattern.sub(lambda m: dictionary[re.escape(m.group(0))], input)
@@ -186,15 +184,19 @@
 
     # Helper to apply tone sandhi to a word
     def __tone_sandhi(self, words, last):
         sandhi = {'1':'7', '7':'3', '3':'2', '2':'1', '5':'7', 'p4':'p8', 't4':'t8', 'k4':'k8', 'h4':'2', 'p8':'p4', 't8':'t4', 'k8':'k4', 'h8':'3'}
         a_sandhi = {'1':'7', '2':'1', '3':'1', '5':'7', 'p4':'p8', 't4':'t8', 'k4':'k8', 'h4':'1', 'p8':'p4', 't8':'t4', 'k8':'k4', 'h8':'7'}
         if self.dialect == 'north':
             sandhi.update({'5':'3'})
-        indices = range(len(words)-2) if last == 'a suff' and len(words) > 1 else range(len(words)-1) if not last else range(len(words))
+        indices = (
+            list(range(len(words) - 2)) if last == 'a suff' and len(words) > 1 
+            else list(range(len(words) - 1)) if not last 
+            else list(range(len(words)))
+        )
         sandhi_words = [self.__replacement_tool(sandhi, words[i]) for i in indices]
         if last == 'a suff' and len(words) > 1:
             sandhi_words.append(self.__replacement_tool(a_sandhi, words[-2]))
         if not last or last == 'a suff':
             sandhi_words.append(words[-1])
         return sandhi_words
     
@@ -210,19 +212,20 @@
             if i < len(input) - 1 and input[i+1] in self.__location:
                 result = False
             elif word in self.__location or word in self.__no_sandhi:
                 result = False
             elif len(word) > 1 and word[-1] == "仔":
                 result = "a suff"
             else:
-                result = i < len(input) - 1 and is_cjk(input[i+1])
+                last = i < len(input) - 1
+                result = last if self.convert_non_cjk else last and is_cjk(input[i+1])
             result_list.append((word, result))
         result_list = sandhi_logic.get(self.sandhi, result_list)
         for i in range(len(result_list) - 2, -1, -1):
-            if result_list[i+1][0] in self.__suffixes:
+            if self.convert_non_cjk and result_list[i+1][0].startswith('--') or result_list[i+1][0] in self.__suffixes:
                 result_list[i] = (result_list[i][0], False)
         return result_list
 
 
     ### Tai-lo to other transliteration systems converting
 
     # Helper to convert syllable from Tai-lo to Tai-lo
@@ -247,15 +250,19 @@
             'a'+self.tt+'i', 'a'+self.tt+'u', 'ia'+self.tt, 'iu'+self.tt, 'io'+self.tt, 'a'+self.tt,
             'o'+self.tt, 'o͘'+self.tt, 'e'+self.tt, 'i'+self.tt, 'u'+self.tt, 'n'+self.tt+'g', 'm'+self.tt
         ]
         convert = {'nng':'nng', 'nnh':'hⁿ', 'nn':'ⁿ', 'ts':'ch', 'ing':'eng', 'uai':'oai', 'uan':'oan', 'ik':'ek', 'ua':'oa', 'ue':'oe', 'oo':'o͘'}
         tones = ['', '', '́', '̀', '', '̂', '', '̄', '̍', '']
         placement += [s.capitalize() for s in placement]
         convert.update({k.capitalize(): v.capitalize() for k, v in convert.items()})
-        input = '-'.join(self.__get_mark_tone(self.__replacement_tool(convert, nt), placement, tones) for nt in self.__get_number_tones(input))
+        number_tones = self.__get_number_tones(input)
+        input = '-'.join(
+            self.__get_mark_tone(self.__replacement_tool(convert, nt), placement, tones) 
+            for nt in number_tones
+        )
         return input.replace(self.suffix_token, '--')
 
 
     # Helper to convert syllable from Tai-lo to 方音符號 (zhuyin)
     def __tailo_to_zhuyin(self, input):
         convert = {
             'p4':'ㆴ4', 'p8':'ㆴ8', 'k4':'ㆶ4', 'k8':'ㆶ8', 't4':'ㆵ4', 't8':'ㆵ8', 'h4':'ㆷ4', 'h8':'ㆷ8', 'h0': '0',
@@ -345,15 +352,20 @@
             'oo':'o', 'om':'om', 'ong':'ong', 'ir':'i', 'tsh':'c',
             'ts':'z', 'nng':'nng', 'ng':'ng', 'g':'gh', 'kh':'k', 'k':'g',
             'ph':'p', 'p':'b', 'b':'bh', 'th':'t', 't':'d', 'j':'r'}
         tones = ["̊", "", "̀", "̂", "̄", "̆", "", "̄", "", "́"]
         placement += [s.capitalize() for s in placement]
         convert.update({k.capitalize(): v.capitalize() for k, v in convert.items()})
         number_tones = [nt[:-2] + 'or' + nt[-1] if nt[-2] == 'o' else nt for nt in self.__get_number_tones(input)]
-        input = '-'.join(self.__get_mark_tone(self.__replacement_tool(convert, nt), placement, tones) if self.format != 'number' else self.__replacement_tool(convert, nt) for nt in number_tones)
+        input = '-'.join(
+            self.__get_mark_tone(self.__replacement_tool(convert, nt), placement, tones) 
+            if self.format != 'number' 
+            else self.__replacement_tool(convert, nt) 
+            for nt in number_tones
+        )
         return input.replace(self.suffix_token, '--')
     
 
     # Helper to convert syllable from Tai-lo to International Phonetic Alphabet
     def __tailo_to_ipa(self, input):
         convert = {
             'tsing':'tɕiɪŋ','jiang':'dʑiaŋ','tshing':'tɕʰiɪŋ','tsik':'tɕiɪk','tshik':'tɕʰiɪk',
@@ -447,10 +459,22 @@
                         tokenised.append(word)
                     traditional = traditional[j:]
                     break
             else:
                 traditional = ""
         punctuations = re.compile("([.,!?\"#$%&()*+/:;<=>@[\\]^`{|}~\t。．，、！？；：（）［］【】「」“”]\s*)")
         indices = [0] + [len(item) for item in tokenised]
-        tokenised = [input[sum(indices[:i+1]):sum(indices[:i+2])] for i in range(len(tokenised))]
-        tokenised = [item for word in tokenised for subword in punctuations.split(word) if subword for item in subword.split(" ") if item]
-        return [subword for word in tokenised for subword in ((word[:-1], word[-1]) if (word[-1] == '的' or word[-1] == '矣') and len(word) > 1 else (word,))]
+        tokenised = [input[sum(indices[:i+1]):sum(indices[:i+2])] for i in range(len(indices)-1)]
+        tokenised = [
+            item 
+            for word in tokenised 
+            for subword in re.split(punctuations, word) if subword 
+            for item in subword.split(" ") if item
+        ]
+        return [
+            subword 
+            for word in tokenised 
+            for subword in (
+                (word[:-1], word[-1]) if (word[-1] == '的' or word[-1] == '矣') and len(word) > 1 
+                else (word,)
+            )
+        ]
```

