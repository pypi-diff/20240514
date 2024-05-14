# Comparing `tmp/PyAibote-1.4.6.tar.gz` & `tmp/PyAibote-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.4.6.tar", last modified: Sat May 11 09:24:39 2024, max compression
+gzip compressed data, was "PyAibote-1.4.7.tar", last modified: Tue May 14 09:24:23 2024, max compression
```

## Comparing `PyAibote-1.4.6.tar` & `PyAibote-1.4.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.973655 PyAibote-1.4.6/
--rw-rw-rw-   0        0        0     1089 2024-05-11 09:24:38.971657 PyAibote-1.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.052936 PyAibote-1.4.6/PyAibote/
--rw-rw-rw-   0        0        0     2679 2024-04-25 13:20:13.000000 PyAibote-1.4.6/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.474604 PyAibote-1.4.6/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6152 2024-04-22 14:05:18.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.6/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.525609 PyAibote-1.4.6/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.6/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.6/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.629602 PyAibote-1.4.6/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.4.6/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0      992 2024-04-25 13:18:13.000000 PyAibote-1.4.6/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.6/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.757636 PyAibote-1.4.6/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.4.6/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.4.6/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.4.6/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.6/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.4.6/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.6/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.4.6/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.4.6/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.4.6/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.4.6/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.6/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.6/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.968655 PyAibote-1.4.6/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    21648 2024-04-30 02:11:24.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.6/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.6/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:24:38.104932 PyAibote-1.4.6/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-05-11 09:24:37.000000 PyAibote-1.4.6/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-05-11 09:24:37.000000 PyAibote-1.4.6/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 09:24:37.000000 PyAibote-1.4.6/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 09:24:37.000000 PyAibote-1.4.6/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 09:24:37.000000 PyAibote-1.4.6/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.4.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 09:24:38.973655 PyAibote-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-05-11 09:22:14.000000 PyAibote-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:23.303782 PyAibote-1.4.7/
+-rw-rw-rw-   0        0        0     1089 2024-05-14 09:24:23.286777 PyAibote-1.4.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:21.739566 PyAibote-1.4.7/PyAibote/
+-rw-rw-rw-   0        0        0     2679 2024-04-25 13:20:13.000000 PyAibote-1.4.7/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:22.211569 PyAibote-1.4.7/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6178 2024-05-14 09:14:47.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.7/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:22.288575 PyAibote-1.4.7/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.7/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.7/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:22.420575 PyAibote-1.4.7/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.4.7/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0      992 2024-04-25 13:18:13.000000 PyAibote-1.4.7/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.7/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:22.619572 PyAibote-1.4.7/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.4.7/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.4.7/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.4.7/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.7/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.4.7/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.7/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.4.7/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.4.7/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.4.7/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.4.7/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.7/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.7/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:23.276781 PyAibote-1.4.7/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    23558 2024-05-14 08:46:42.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.7/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.7/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:24:21.802572 PyAibote-1.4.7/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-05-14 09:24:21.000000 PyAibote-1.4.7/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-05-14 09:24:21.000000 PyAibote-1.4.7/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 09:24:21.000000 PyAibote-1.4.7/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-14 09:24:21.000000 PyAibote-1.4.7/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 09:24:21.000000 PyAibote-1.4.7/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 09:24:23.304778 PyAibote-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-05-14 09:23:47.000000 PyAibote-1.4.7/setup.py
```

### Comparing `PyAibote-1.4.6/PKG-INFO` & `PyAibote-1.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.6
+Version: 1.4.7
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBot.py` & `PyAibote-1.4.7/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/Control.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,22 @@
             width: the width of the control, which is 400 by default
             height: control height, default is 60
             is_select: whether it is checked or not; the default value is False
             return: True or False
         """
         return "true" in self.SendData("createCheckBox", _id, text, coordinate[0], coordinate[1], width, height, is_select) 
 
-    def create_list_text(self, _id: int, hint_text: str, list_text: list, coordinate: tuple = (400,500), width: int = 400, height: int = 400) -> bool:
+    def create_list_text(self, _id: int, hint_text: str, list_text: str, coordinate: tuple = (400,500), width: int = 400, height: int = 400) -> bool:
         """
             创建ListText控件
             Create ListText control
 
             _id:  控件ID，不可与其他控件重复
             hint_text:  提示文本
-            list_text:  列表文本
+            list_text:  下拉列表中的文本以逗号分割
             coordinate: x,y坐标 默认 (400,500)
             width:  控件宽度
             height:  控件高度
             return: True或者False
 
             _ID: control id, which cannot be duplicated with other controls
             Hint_text: prompt text
```

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.4.7/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.4.7/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.4.7/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.4.7/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/Logger.py` & `PyAibote-1.4.7/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.4.7/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.4.7/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/SocketServer.py` & `PyAibote-1.4.7/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.4.7/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.4.7/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.4.7/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/Tool/__init__.py` & `PyAibote-1.4.7/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBot.py` & `PyAibote-1.4.7/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/DrivingOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.4.7/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBot.py` & `PyAibote-1.4.7/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files 6% similar despite different names*

```diff
@@ -269,15 +269,14 @@
             This function only makes sense when the waitPlaySound parameter of metahumanSpeech and metahumanSpeechCache is set to false
 
             return: 返回true打断正在说话， 返回false 则为未说话状态
             return true to interrupt talking, return false to be silent
         """
         return "true" in self.SendData("metahumanSpeechBreak") 
 
-
     def make_metahuman_speech_file(self, save_audio_path: str, text: str, language: str = "zh-cn", voice_name: str = "", quality: int = 0, speech_rate: int = 0, voice_style: str = "General") -> bool:
         """
             生成数字人说话文件，生成MP3文件和 lab文件，提供给 metahumanSpeechByFile 和使用
             Generate digital human speech files, MP3 files and lab files, and provide them to metahumanSpeechByFile and use
 
             save_audio_path: 保存的音频文件路径，扩展为.MP3格式。同名的 .lab文件需要和音频文件在同一目录下
             text: 要转换语音的文本
@@ -294,7 +293,42 @@
             voice_name: speaker, refer to the development document language and speaker
             quality: sound quality, 0 low quality 1 medium quality 2 high quality, and 0 low quality by default
             speech_rate: speech speed, which is 0 by default, and the value range is -100 to 200
             voice_style: voice style, the default General style, and other styles refer to the development document language and speaker
             return: True or False
         """
         return "true" in self.SendData("makeMetahumanSpeechFile", save_audio_path, text, language, voice_name, quality, speech_rate, voice_style) 
+
+    def switch_action(self, call_apiKey: str, action_video_or_image: str) -> bool:
+        """
+            切换新的人物形象动作，此函数无需训练数字人模型，直接切换各种人物形象动作和场景
+            Switch new character movements. This function can directly switch various character movements and scenes without training digital human models
+
+            call_apiKey: 调用函数的密钥
+            action_video_or_image: 闭嘴的人物视频或者图片
+            return: True或者False
+
+            call_apiKey: String, the key of the calling function
+            action_video_or_image: a string, shut-up character video or picture
+            return: True or False
+        """
+        return "true" in self.SendData("switchAction", call_apiKey, action_video_or_image) 
+
+    def train_human_model(self, call_apiKey: str, train_video_or_image: str, src_metahuman_model_path: str, save_human_model_folder: str) -> bool:
+        """
+            训练数字人，训练时长为10-30分钟
+            Train digital people for 10-30 minutes
+
+            call_apiKey: 调用函数的密钥
+            train_video_or_image: 闭嘴的人物视频或者图片 素材
+            src_metahuman_model_path: 预训练数字人模型路径
+            save_human_model_folder: 保存训练完成的模型目录
+            return: True或者False
+
+            call_apiKey: the key of the calling function
+            train_video_or_image: shut up the character video or picture material
+            src_metahuman_model_path: the path of pre-training digital human model
+            save_human_model_folder: save the model directory after training
+            return: True or False
+        """
+        return "true" in self.SendData("trainHumanModel", call_apiKey, train_video_or_image, src_metahuman_model_path, save_human_model_folder) 
+
```

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.4.7/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.4.7/PyAibote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.6
+Version: 1.4.7
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.6/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.4.7/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/README.md` & `PyAibote-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.6/setup.py` & `PyAibote-1.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.4.6", 
+    version="1.4.7", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

