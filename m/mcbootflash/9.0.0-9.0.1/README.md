# Comparing `tmp/mcbootflash-9.0.0.tar.gz` & `tmp/mcbootflash-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbootflash-9.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mcbootflash-9.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mcbootflash-9.0.0.tar` & `mcbootflash-9.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     3090 2022-06-08 18:37:37.758584 mcbootflash-9.0.0/.gitignore
--rw-r--r--   0        0        0    11498 2024-05-13 19:58:10.674425 mcbootflash-9.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1058 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/LICENSE
--rw-r--r--   0        0        0     3583 2023-11-10 18:57:54.826438 mcbootflash-9.0.0/README.md
--rw-r--r--   0        0        0      465 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/docs/api.md
--rw-r--r--   0        0        0       44 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/changelog.md
--rw-r--r--   0        0        0     3473 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/develop.md
--rw-r--r--   0        0        0       41 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/index.md
--rw-r--r--   0        0        0      836 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/mkdocs.yml
--rw-r--r--   0        0        0     1732 2024-02-10 19:54:03.191436 mcbootflash-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      685 2024-05-13 20:06:51.233865 mcbootflash-9.0.0/src/mcbootflash/__init__.py
--rw-r--r--   0        0        0     7250 2024-05-13 19:54:58.266181 mcbootflash-9.0.0/src/mcbootflash/__main__.py
--rw-r--r--   0        0        0      989 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/src/mcbootflash/error.py
--rw-r--r--   0        0        0    11757 2024-05-13 19:54:06.757043 mcbootflash-9.0.0/src/mcbootflash/flash.py
--rw-r--r--   0        0        0     8642 2024-05-13 19:54:06.757043 mcbootflash-9.0.0/src/mcbootflash/types.py
--rw-r--r--   0        0        0     1545 2024-05-13 19:51:55.886146 mcbootflash-9.0.0/src/mcbootflash/util.py
--rw-r--r--   0        0        0   101873 2024-05-13 19:56:09.803760 mcbootflash-9.0.0/tests/test_mcbootflash.json
--rw-r--r--   0        0        0     5427 2024-05-13 19:56:09.803760 mcbootflash-9.0.0/tests/test_mcbootflash.py
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/checksum_error/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/flash/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/flash_empty/test.hex
--rw-r--r--   0        0        0     2932 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/no_data/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/no_response/test.hex
--rw-r--r--   0        0        0      565 2024-02-10 19:54:03.191436 mcbootflash-9.0.0/tox.ini
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 mcbootflash-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-02-08 10:24:45.013478 mcbootflash-9.0.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3090 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/.gitignore
+-rw-r--r--   0        0        0    11910 2024-05-14 06:55:44.128737 mcbootflash-9.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1058 2024-02-08 10:24:45.021478 mcbootflash-9.0.1/LICENSE
+-rw-r--r--   0        0        0     3632 2024-05-14 06:38:49.247168 mcbootflash-9.0.1/README.md
+-rw-r--r--   0        0        0      465 2024-02-07 12:53:19.752024 mcbootflash-9.0.1/docs/api.md
+-rw-r--r--   0        0        0       44 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/docs/changelog.md
+-rw-r--r--   0        0        0     3473 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/docs/develop.md
+-rw-r--r--   0        0        0       41 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/docs/index.md
+-rw-r--r--   0        0        0      836 2024-02-08 10:24:45.021478 mcbootflash-9.0.1/mkdocs.yml
+-rw-r--r--   0        0        0     1732 2024-02-08 11:43:20.300736 mcbootflash-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0      685 2024-05-14 06:18:56.819648 mcbootflash-9.0.1/src/mcbootflash/__init__.py
+-rw-r--r--   0        0        0     7259 2024-05-14 06:29:04.639814 mcbootflash-9.0.1/src/mcbootflash/__main__.py
+-rw-r--r--   0        0        0      989 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/src/mcbootflash/error.py
+-rw-r--r--   0        0        0    11757 2024-05-14 06:18:56.831648 mcbootflash-9.0.1/src/mcbootflash/flash.py
+-rw-r--r--   0        0        0     8642 2024-05-14 06:18:56.875650 mcbootflash-9.0.1/src/mcbootflash/types.py
+-rw-r--r--   0        0        0     1545 2024-05-14 06:18:56.879650 mcbootflash-9.0.1/src/mcbootflash/util.py
+-rw-r--r--   0        0        0   101873 2024-05-14 06:18:56.887650 mcbootflash-9.0.1/tests/test_mcbootflash.json
+-rw-r--r--   0        0        0     5427 2024-05-14 06:18:56.887650 mcbootflash-9.0.1/tests/test_mcbootflash.py
+-rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.921739 mcbootflash-9.0.1/tests/testcases/checksum_error/test.hex
+-rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-9.0.1/tests/testcases/flash/test.hex
+-rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-9.0.1/tests/testcases/flash_empty/test.hex
+-rw-r--r--   0        0        0     2932 2024-02-05 09:08:21.925739 mcbootflash-9.0.1/tests/testcases/no_data/test.hex
+-rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-9.0.1/tests/testcases/no_response/test.hex
+-rw-r--r--   0        0        0      565 2024-02-08 10:24:45.021478 mcbootflash-9.0.1/tox.ini
+-rw-r--r--   0        0        0     5074 1970-01-01 00:00:00.000000 mcbootflash-9.0.1/PKG-INFO
```

### Comparing `mcbootflash-9.0.0/.github/workflows/main.yml` & `mcbootflash-9.0.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/.gitignore` & `mcbootflash-9.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/CHANGELOG.md` & `mcbootflash-9.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # Changelog
 
-## [9.0.1] - Development
+## [9.0.2] - Development
+
+## [9.0.1] - 2024-05-14
+
+### Changed
+
+- Make minor improvements to CLI output ([`fb17948`](https://github.com/bessman/mcbootflash/commit/fb17948310d85f30b3f7b451e02dfded53b7faa7))
+
+### Fixed
+
+- Update README to reflect changes made in v9.0.0 ([`e6dc42c`](https://github.com/bessman/mcbootflash/commit/e6dc42c2747dc42efb2ce03f15dc535907796f11))
 
 ## [9.0.0] - 2024-05-13
 
 ### Changed
 
 - Disable checksumming by default in CLI, enable with `--checksum` flag ([`b685bb5`](https://github.com/bessman/mcbootflash/commit/b685bb56165805706fdc87adcba76c1285cc3416))
 - Unconditionally erase before flashing with CLI ([`9a4ddc6`](https://github.com/bessman/mcbootflash/commit/9a4ddc629b1df47fe06149ceafdc3f4131a5e6e6))
@@ -260,14 +270,15 @@
 
 - Fix off-by-one error when firmware uses all available space
 
 ## [1.0.0] - 2022-05-27
 
 _Initial release._
 
+[9.0.1]: https://github.com/bessman/mcbootflash/releases/tag/9.0.1
 [9.0.0]: https://github.com/bessman/mcbootflash/releases/tag/9.0.0
 [8.0.2]: https://github.com/bessman/mcbootflash/releases/tag/8.0.2
 [8.0.1]: https://github.com/bessman/mcbootflash/releases/tag/8.0.1
 [8.0.0]: https://github.com/bessman/mcbootflash/releases/tag/v8.0.0
 [7.0.6]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.6
 [7.0.5]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.5
 [7.0.4]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.4
```

### Comparing `mcbootflash-9.0.0/LICENSE` & `mcbootflash-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/README.md` & `mcbootflash-9.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,42 +41,42 @@
 
 Mcbootflash can be used as both a command-line application and a library.
 
 ### Command-line
 
 ```shellsession
 $ mcbootflash --help
-usage: mcbootflash [-h] -p PORT -b BAUDRATE [-t TIMEOUT] [-v] [-q] [--version] hexfile
+usage: mcbootflash [-h] -p PORT -b BAUDRATE [-t TIMEOUT] [-c] [-r] [-v] [-q] [--version] hexfile
 
 Flash firmware over serial connection to a device running Microchip's 16-bit bootloader.
 
 positional arguments:
-  hexfile               an Intel HEX file containing application firmware
+  hexfile               a HEX file containing application firmware
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -p PORT, --port PORT  serial port connected to the device you want to flash
   -b BAUDRATE, --baudrate BAUDRATE
                         symbol rate of device's serial bus
   -t TIMEOUT, --timeout TIMEOUT
                         try to read data from the bus for this many seconds before giving up
+  -c, --checksum        verify flashed data by checksumming after write
+  -r, --reset           reset device after flashing is complete
   -v, --verbose         print debug messages
   -q, --quiet           suppress output
   --version             show program's version number and exit
 ```
 
 #### Example
 
 ```shellsession
 $ mcbootflash --port /dev/ttyUSB0 --baudrate 460800 firmware.hex
 Connecting to bootloader...
-Connected
-Existing application detected, erasing...
-Application erased
-Flashing firmware.hex
+Erasing program area...
+Flashing firmware.hex...
 100%  88.7 KiB |########################################| Elapsed Time: 0:00:05
 Self verify OK
 ```
 
 ### Library
 
 When using mcbootflash as a library, typical workflow looks something like this:
@@ -96,16 +96,15 @@
 bf.erase_flash(connection, bootattrs.memory_range, bootattrs.erase_size)
 
 # Write the firmware chunks to the bootloader in a loop.
 for chunk in chunks:
     bf.write_flash(connection, chunk)
 
     # Optionally, check that the write is OK by checksumming.
-    if bootattrs.has_checksum:
-        bf.checksum(connection, chunk)
+    bf.checksum(connection, chunk)
 
     # At this point, you may want to give an indication of the flashing progress,
     # like updating a progress bar.
 
 # Verify that the new application is detected.
 bf.self_verify(connection)
 ```
```

### Comparing `mcbootflash-9.0.0/docs/develop.md` & `mcbootflash-9.0.1/docs/develop.md`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/mkdocs.yml` & `mcbootflash-9.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/pyproject.toml` & `mcbootflash-9.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/src/mcbootflash/__init__.py` & `mcbootflash-9.0.1/src/mcbootflash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "erase_flash",
     "get_boot_attrs",
     "reset",
     "self_verify",
     "write_flash",
 ]
 
-__version__ = "9.0.0"
+__version__ = "9.0.1"
```

### Comparing `mcbootflash-9.0.0/src/mcbootflash/__main__.py` & `mcbootflash-9.0.1/src/mcbootflash/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,30 +114,30 @@
         _logger.info("Connecting to bootloader...")
         connection = Serial(
             port=args.port,
             baudrate=args.baudrate,
             timeout=args.timeout,
         )
         bootattrs = mcbf.get_boot_attrs(connection)
-        _logger.info("Connected")
         total_bytes, chunks = mcbf.chunked(args.hexfile, bootattrs)
-        _logger.debug("Erasing program area...")
+        _logger.info("Erasing program area...")
         mcbf.erase_flash(connection, bootattrs.memory_range, bootattrs.erase_size)
-        _logger.info(f"Flashing {args.hexfile}")
+        _logger.info(f"Flashing {args.hexfile}...")
         flash(
             connection=connection,
             chunks=chunks,
             total_bytes=total_bytes,
             checksum=args.checksum,
         )
         mcbf.self_verify(connection)
         _logger.info("Self verify OK")
 
         if args.reset:
             mcbf.reset(connection)
+            _logger.info("Device reset")
     except Exception:
         _logger.exception("An error occurred:")
 
 
 def flash(
     connection: Serial,
     chunks: Iterator[mcbf.Chunk],
```

### Comparing `mcbootflash-9.0.0/src/mcbootflash/error.py` & `mcbootflash-9.0.1/src/mcbootflash/error.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/src/mcbootflash/flash.py` & `mcbootflash-9.0.1/src/mcbootflash/flash.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/src/mcbootflash/types.py` & `mcbootflash-9.0.1/src/mcbootflash/types.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/src/mcbootflash/util.py` & `mcbootflash-9.0.1/src/mcbootflash/util.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/test_mcbootflash.json` & `mcbootflash-9.0.1/tests/test_mcbootflash.json`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/test_mcbootflash.py` & `mcbootflash-9.0.1/tests/test_mcbootflash.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/testcases/checksum_error/test.hex` & `mcbootflash-9.0.1/tests/testcases/checksum_error/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/testcases/flash/test.hex` & `mcbootflash-9.0.1/tests/testcases/flash/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/testcases/flash_empty/test.hex` & `mcbootflash-9.0.1/tests/testcases/flash_empty/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/testcases/no_data/test.hex` & `mcbootflash-9.0.1/tests/testcases/no_data/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tests/testcases/no_response/test.hex` & `mcbootflash-9.0.1/tests/testcases/no_response/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/tox.ini` & `mcbootflash-9.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `mcbootflash-9.0.0/PKG-INFO` & `mcbootflash-9.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcbootflash
-Version: 9.0.0
+Version: 9.0.1
 Summary: Flash firmware to devices running Microchip's 16-bit bootloader.
 Keywords: firmware,flashing,bootloader,serial,uart,microchip,pic24,dspic33,16-bit
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -76,42 +76,42 @@
 
 Mcbootflash can be used as both a command-line application and a library.
 
 ### Command-line
 
 ```shellsession
 $ mcbootflash --help
-usage: mcbootflash [-h] -p PORT -b BAUDRATE [-t TIMEOUT] [-v] [-q] [--version] hexfile
+usage: mcbootflash [-h] -p PORT -b BAUDRATE [-t TIMEOUT] [-c] [-r] [-v] [-q] [--version] hexfile
 
 Flash firmware over serial connection to a device running Microchip's 16-bit bootloader.
 
 positional arguments:
-  hexfile               an Intel HEX file containing application firmware
+  hexfile               a HEX file containing application firmware
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -p PORT, --port PORT  serial port connected to the device you want to flash
   -b BAUDRATE, --baudrate BAUDRATE
                         symbol rate of device's serial bus
   -t TIMEOUT, --timeout TIMEOUT
                         try to read data from the bus for this many seconds before giving up
+  -c, --checksum        verify flashed data by checksumming after write
+  -r, --reset           reset device after flashing is complete
   -v, --verbose         print debug messages
   -q, --quiet           suppress output
   --version             show program's version number and exit
 ```
 
 #### Example
 
 ```shellsession
 $ mcbootflash --port /dev/ttyUSB0 --baudrate 460800 firmware.hex
 Connecting to bootloader...
-Connected
-Existing application detected, erasing...
-Application erased
-Flashing firmware.hex
+Erasing program area...
+Flashing firmware.hex...
 100%  88.7 KiB |########################################| Elapsed Time: 0:00:05
 Self verify OK
 ```
 
 ### Library
 
 When using mcbootflash as a library, typical workflow looks something like this:
@@ -131,16 +131,15 @@
 bf.erase_flash(connection, bootattrs.memory_range, bootattrs.erase_size)
 
 # Write the firmware chunks to the bootloader in a loop.
 for chunk in chunks:
     bf.write_flash(connection, chunk)
 
     # Optionally, check that the write is OK by checksumming.
-    if bootattrs.has_checksum:
-        bf.checksum(connection, chunk)
+    bf.checksum(connection, chunk)
 
     # At this point, you may want to give an indication of the flashing progress,
     # like updating a progress bar.
 
 # Verify that the new application is detected.
 bf.self_verify(connection)
 ```
```

