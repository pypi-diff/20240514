# Comparing `tmp/airtestproject-0.1.6.tar.gz` & `tmp/airtestproject-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-1qp0zq78\airtestproject-0.1.6.tar", last modified: Sat May 11 07:51:18 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-ng2y3l89\airtestproject-0.1.7.tar", last modified: Tue May 14 08:08:14 2024, max compression
```

## Comparing `airtestproject-0.1.6.tar` & `airtestproject-0.1.7.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.128913 airtestproject-0.1.6/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      786 2024-05-11 07:51:18.128024 airtestproject-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-05-11 00:14:26.000000 airtestproject-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.047133 airtestproject-0.1.6/airtestProject/
--rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.6/airtestProject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.059100 airtestproject-0.1.6/airtestProject/abstractBase/
--rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.6/airtestProject/abstractBase/OperateBase.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/abstractBase/__init__.py
--rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.6/airtestProject/abstractBase/loginBase.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.062121 airtestproject-0.1.6/airtestProject/commons/
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.064111 airtestproject-0.1.6/airtestProject/commons/Position/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/Position/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.066082 airtestproject-0.1.6/airtestProject/commons/Position/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/Position/odin/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.6/airtestProject/commons/Position/odin/odinPos.py
--rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.6/airtestProject/commons/UWA.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.068077 airtestproject-0.1.6/airtestProject/commons/page/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/page/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.074060 airtestproject-0.1.6/airtestProject/commons/page/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/page/odin/__init__.py
--rw-rw-rw-   0        0        0    18812 2024-05-11 07:50:17.000000 airtestproject-0.1.6/airtestProject/commons/page/odin/funcListCheck.py
--rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/page/odin/login.py
--rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/page/odin/run.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.076083 airtestproject-0.1.6/airtestProject/commons/process/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/process/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.079071 airtestproject-0.1.6/airtestProject/commons/process/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/process/odin/__init__.py
--rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/process/odin/profile.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.107970 airtestproject-0.1.6/airtestProject/commons/utils/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/air.py
--rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.6/airtestProject/commons/utils/appStart.py
--rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/command.py
--rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.6/airtestProject/commons/utils/deploy.py
--rw-rw-rw-   0        0        0     5655 2024-05-11 00:07:48.000000 airtestproject-0.1.6/airtestProject/commons/utils/excel_image.py
--rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.6/airtestProject/commons/utils/exception.py
--rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.6/airtestProject/commons/utils/factory.py
--rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/ganaratePyCase.py
--rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/genaratePy.py
--rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/gotCommon.py
--rw-rw-rw-   0        0        0     5448 2024-05-11 07:35:53.000000 airtestproject-0.1.6/airtestProject/commons/utils/logger.py
--rw-rw-rw-   0        0        0    11125 2024-05-10 23:59:21.000000 airtestproject-0.1.6/airtestProject/commons/utils/myAirtest.py
--rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/myPoco.py
--rw-rw-rw-   0        0        0     8139 2024-05-10 23:57:10.000000 airtestproject-0.1.6/airtestProject/commons/utils/ocrTemplate.py
--rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/page.py
--rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.6/airtestProject/commons/utils/reportUtil.py
--rw-rw-rw-   0        0        0     1744 2024-05-11 00:02:22.000000 airtestproject-0.1.6/airtestProject/commons/utils/tools.py
--rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/commons/utils/utils.py
--rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.6/airtestProject/config.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.112956 airtestproject-0.1.6/airtestProject/factory/
--rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.6/airtestProject/factory/SingletonFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/factory/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/factory/operateFactory.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.122929 airtestproject-0.1.6/airtestProject/manager/
--rw-rw-rw-   0        0        0     9352 2024-05-11 06:07:00.000000 airtestproject-0.1.6/airtestProject/manager/DeviceManager.py
--rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.6/airtestProject/manager/LogManager.py
--rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/manager/PackageManager.py
--rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/manager/ReportManager.py
--rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/manager/TaskManager.py
--rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.6/airtestProject/manager/TestCaseManager.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.6/airtestProject/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.124925 airtestproject-0.1.6/airtestProject/scripts/
--rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.6/airtestProject/scripts/OdinExample.py
--rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.6/airtestProject/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:51:18.126919 airtestproject-0.1.6/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      786 2024-05-11 07:51:17.000000 airtestproject-0.1.6/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2192 2024-05-11 07:51:18.000000 airtestproject-0.1.6/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 07:51:17.000000 airtestproject-0.1.6/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-05-11 07:51:17.000000 airtestproject-0.1.6/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-11 07:51:17.000000 airtestproject-0.1.6/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 07:51:18.129911 airtestproject-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      848 2024-05-11 07:50:39.000000 airtestproject-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.232102 airtestproject-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      786 2024-05-14 08:08:14.231104 airtestproject-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-11 00:14:26.000000 airtestproject-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.147936 airtestproject-0.1.7/airtestProject/
+-rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.7/airtestProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.160902 airtestproject-0.1.7/airtestProject/abstractBase/
+-rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.7/airtestProject/abstractBase/OperateBase.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/abstractBase/__init__.py
+-rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.7/airtestProject/abstractBase/loginBase.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.163893 airtestproject-0.1.7/airtestProject/commons/
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.165887 airtestproject-0.1.7/airtestProject/commons/Position/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/Position/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.168880 airtestproject-0.1.7/airtestProject/commons/Position/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/Position/odin/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.7/airtestProject/commons/Position/odin/odinPos.py
+-rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.7/airtestProject/commons/UWA.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.169876 airtestproject-0.1.7/airtestProject/commons/page/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/page/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.177857 airtestproject-0.1.7/airtestProject/commons/page/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/__init__.py
+-rw-rw-rw-   0        0        0    18812 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/funcListCheck.py
+-rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/login.py
+-rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/page/odin/run.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.179852 airtestproject-0.1.7/airtestProject/commons/process/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/process/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.182842 airtestproject-0.1.7/airtestProject/commons/process/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/process/odin/__init__.py
+-rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/process/odin/profile.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.212120 airtestproject-0.1.7/airtestProject/commons/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/air.py
+-rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.7/airtestProject/commons/utils/appStart.py
+-rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/command.py
+-rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.7/airtestProject/commons/utils/deploy.py
+-rw-rw-rw-   0        0        0     5655 2024-05-11 00:07:48.000000 airtestproject-0.1.7/airtestProject/commons/utils/excel_image.py
+-rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.7/airtestProject/commons/utils/exception.py
+-rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.7/airtestProject/commons/utils/factory.py
+-rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/ganaratePyCase.py
+-rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/genaratePy.py
+-rw-rw-rw-   0        0        0     3786 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/gotCommon.py
+-rw-rw-rw-   0        0        0     5616 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/logger.py
+-rw-rw-rw-   0        0        0    11825 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/myAirtest.py
+-rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/myPoco.py
+-rw-rw-rw-   0        0        0     8139 2024-05-10 23:57:10.000000 airtestproject-0.1.7/airtestProject/commons/utils/ocrTemplate.py
+-rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/page.py
+-rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.7/airtestProject/commons/utils/reportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/commons/utils/test.py
+-rw-rw-rw-   0        0        0     1744 2024-05-11 00:02:22.000000 airtestproject-0.1.7/airtestProject/commons/utils/tools.py
+-rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/commons/utils/utils.py
+-rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.7/airtestProject/config.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.216141 airtestproject-0.1.7/airtestProject/factory/
+-rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.7/airtestProject/factory/SingletonFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/factory/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/factory/operateFactory.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.226117 airtestproject-0.1.7/airtestProject/manager/
+-rw-rw-rw-   0        0        0     9352 2024-05-14 03:10:27.000000 airtestproject-0.1.7/airtestProject/manager/DeviceManager.py
+-rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.7/airtestProject/manager/LogManager.py
+-rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/PackageManager.py
+-rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/ReportManager.py
+-rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/TaskManager.py
+-rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.7/airtestProject/manager/TestCaseManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.7/airtestProject/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.229110 airtestproject-0.1.7/airtestProject/scripts/
+-rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.7/airtestProject/scripts/OdinExample.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.7/airtestProject/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:08:14.230106 airtestproject-0.1.7/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      786 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 08:08:14.000000 airtestproject-0.1.7/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:08:14.233103 airtestproject-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      848 2024-05-14 08:07:14.000000 airtestproject-0.1.7/setup.py
```

### Comparing `airtestproject-0.1.6/LICENSE` & `airtestproject-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/PKG-INFO` & `airtestproject-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.6
+Version: 0.1.7
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.6/airtestProject/abstractBase/OperateBase.py` & `airtestproject-0.1.7/airtestProject/abstractBase/OperateBase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/UWA.py` & `airtestproject-0.1.7/airtestProject/commons/UWA.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/page/odin/funcListCheck.py` & `airtestproject-0.1.7/airtestProject/commons/page/odin/funcListCheck.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/page/odin/login.py` & `airtestproject-0.1.7/airtestProject/commons/page/odin/login.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/page/odin/run.py` & `airtestproject-0.1.7/airtestProject/commons/page/odin/run.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/process/odin/profile.py` & `airtestproject-0.1.7/airtestProject/commons/process/odin/profile.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/air.py` & `airtestproject-0.1.7/airtestProject/commons/utils/air.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/appStart.py` & `airtestproject-0.1.7/airtestProject/commons/utils/appStart.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/command.py` & `airtestproject-0.1.7/airtestProject/commons/utils/command.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/deploy.py` & `airtestproject-0.1.7/airtestProject/commons/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/excel_image.py` & `airtestproject-0.1.7/airtestProject/commons/utils/excel_image.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/exception.py` & `airtestproject-0.1.7/airtestProject/commons/utils/exception.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/factory.py` & `airtestproject-0.1.7/airtestProject/commons/utils/factory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/ganaratePyCase.py` & `airtestproject-0.1.7/airtestProject/commons/utils/ganaratePyCase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/genaratePy.py` & `airtestproject-0.1.7/airtestProject/commons/utils/genaratePy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/gotCommon.py` & `airtestproject-0.1.7/airtestProject/commons/utils/gotCommon.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,82 +2,85 @@
 
 __author__ = "uwa"
 
 import sys,os
 sys.path.append(os.path.abspath(os.path.dirname(__file__)))
 import unittest
 from airtest.core.api import *
+
 auto_setup(__file__)
 
 # 导入UWA模块
 from airtestProject.commons.UWA import *
 from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 from airtestProject.commons.utils.page import Page
 # 获取 UWA Pipeline 中的信息必须导入run_airtest_config模块
 # import run_airtest_config
 import logging
-_logger = logging.getLogger("airtest")
+from airtestProject.commons.utils.logger import log as logger_log
 # deviceID = device().uuid
 
 class TestGot():
 
+    @logger_log.wrap("正在启动游戏")
     def got_init(self, apk_name):
         try:
             stop_app("com.netease.open.pocoservice")
             sleep(2)
             start_app("com.netease.open.pocoservice")
         except:
-            log("启动失败")
+            logger_log.step("启动失败")
         sleep(5)
 
         a_poco = AndroidUiautomationPoco()            # 初始化 原生 poco 对象
 
         try:
             home()
             stop_app(apk_name)
         except:
-            _logger.debug("APP is not running")
+            logger_log.step("APP is not running")
 
         start_app(apk_name)     # 运行App
         sleep(10)
         permission_buttons = [
             "同意",
             "允许",
             "始终允许",
             "总是允许",
-            "立即开始"
-            "确定"
+            "立即开始",
+            "确定",
+            "稍后"
         ]
 
-        log("%s :进行权限验证")
+        logger_log.test("进行权限验证")
         for i in range(5):
             for button in permission_buttons:         # 权限校验
                 if a_poco(text=button).exists():
                     a_poco(text=button).click()
                 sleep(0.1)
-        log("%s :权限验证结束")
+        logger_log.test("权限验证结束")
         sleep(10)
 
     def got_connect(self, poco):
         GOT_Test.Connect(poco)
         sleep(3)
-        log("%s :连接got")
+        logger_log.step("连接got")
 
     def got_start(self, poco, mode):
         GOT_Test.Start(poco, mode)
-        log("%s :开始执行测试用例")
+        logger_log.step("开始执行测试用例")
 
     def got_stop(self, poco):
         GOT_Test.Stop(poco)                   # 关闭 GOT 模式()
-        log("%s :开始上传")
+        logger_log.step("开始上传")
         sleep(10)
 
     def got_upload(self, poco):
         GOT_Test.Upload(poco, 3000)  # 运行结束后自动上传至UWA官网()
-        log("%s :上传结束")
+        logger_log.step("上传结束")
         sleep(2)
 
     def stop_app(self,apk_name):
         stop_app(apk_name)  # 退出 App
 
     @staticmethod
     def sb():
@@ -108,7 +111,9 @@
     #     Name = param_dict['Name']
     #     # Out: UWA
     #     log(f"参数化构建中Name参数的值为:{Name}")
     #
     #     BoolValue = param_dict['BoolValue']
     #     # Out: False
     #     log(f"参数化构建中BoolValue参数的值为:{BoolValue}")       # 获取UWA Pipeline中信息的接口
+if __name__ == '__main__':
+    TestGot().got_init("com.sanqi.odin2022.weekly")
```

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/logger.py` & `airtestproject-0.1.7/airtestProject/commons/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
 
     def warn(self, msg):
         self.logger.warning(f'{" ".join(self.random_emoji() * 2)} ：{msg}')
 
     def error(self, msg):
         self.logger.error(f'😈 😈 ：{msg}')
 
+    def test(self, msg):
+        self.logger.info(f'{" ".join(self.random_emoji() * 2)} ：{msg}')
+        air.log(f'{" ".join(self.random_emoji() * 2)} ：{msg}')
+
     def wrap(self, msg: str = None) -> Callable:
         """
         函数日志装饰器
         :param msg: 消息内容
         :return:
         """
         def wrapper(func):
@@ -97,18 +101,18 @@
                 try:
                     res = func(*args, **kwargs)
                     end_time = time.time()
                     duration = round(end_time - start_time, 2)
                     self.step(f"{msg} - func: {func.__name__} - duration: {duration} s")
                     if self.adb_log is not None:
                         air.log(self.adb_log,
-                                desc=f"{' '.join(self.random_emoji() * 2)}: {msg} - func: {func.__name__}",
+                                desc=f":😈 😈 {msg} - func: {func.__name__}",
                                 snapshot=True)
                     else:
-                        air.log(f"😈 😈 : {msg} - func: {func.__name__}", snapshot=True)
+                        air.log(f"{' '.join(self.random_emoji() * 2)}: {msg} - func: {func.__name__}", snapshot=True)
                     self.adb_log = None
                     return res
                 except Exception as e:
                     air.log(e, desc=f"😈 😈  : {msg} - func: {func.__name__}", snapshot=True)
                     return func
             return inner
         return wrapper
```

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/myAirtest.py` & `airtestproject-0.1.7/airtestProject/commons/utils/myAirtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,30 @@
 class AirTest(OperateABC):
 
     def __init__(self, language):
         super(AirTest, self).__init__()
         self.this_dict = None
         self.language = language
 
-    def set_dict(self, script_root, project):
+    def set_dict(self, script_root: str, project: str):
+        """
+        各种兼容还有路径转换。ps images文件夹只能在脚本的上级或者同级否则无法正常工作
+        :param script_root: 脚本当前目录
+        :param project: 定位到的具体图片文件夹
+        :return:
+        """
         if self.this_dict is None:
             files_dict = {}
-            abs_directory = os.path.join(get_folder_path_up(script_root, 'images'), project)
+            images_abs_path = get_folder_path_up(script_root, 'images')  # 获取图片文件夹的绝对路径
+            # script_root_dir = os.path.dirname(script_root)  # 获取脚本文件夹的绝对路径
+            # images_relative_path = os.path.relpath(images_abs_path, script_root_dir)  # 构造为图片文件夹的相对路径
+            images_project_relative_path = os.path.join(images_abs_path, project)  # 构造为图片文件夹和project的相对路径
             # 遍历指定目录下的所有文件
-            for filename in os.listdir(abs_directory):
-                file_path = os.path.join(abs_directory, filename)
+            for filename in os.listdir(images_project_relative_path):
+                file_path = os.path.join(images_project_relative_path, filename)
                 if os.path.isfile(file_path):
                     file_name_without_ext, _ = os.path.splitext(filename)
                     files_dict[file_name_without_ext] = Template(file_path)
             print(files_dict)
             self.this_dict = files_dict
 
     def init_device(self, platform=None, uuid=None, **kwargs):
```

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/myPoco.py` & `airtestproject-0.1.7/airtestProject/commons/utils/myPoco.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/ocrTemplate.py` & `airtestproject-0.1.7/airtestProject/commons/utils/ocrTemplate.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/page.py` & `airtestproject-0.1.7/airtestProject/commons/utils/page.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/reportUtil.py` & `airtestproject-0.1.7/airtestProject/commons/utils/reportUtil.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/tools.py` & `airtestproject-0.1.7/airtestProject/commons/utils/tools.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/commons/utils/utils.py` & `airtestproject-0.1.7/airtestProject/commons/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/factory/operateFactory.py` & `airtestproject-0.1.7/airtestProject/factory/operateFactory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/DeviceManager.py` & `airtestproject-0.1.7/airtestProject/manager/DeviceManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/LogManager.py` & `airtestproject-0.1.7/airtestProject/manager/LogManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/PackageManager.py` & `airtestproject-0.1.7/airtestProject/manager/PackageManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/ReportManager.py` & `airtestproject-0.1.7/airtestProject/manager/ReportManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/TaskManager.py` & `airtestproject-0.1.7/airtestProject/manager/TaskManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/manager/TestCaseManager.py` & `airtestproject-0.1.7/airtestProject/manager/TestCaseManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject/scripts/OdinExample.py` & `airtestproject-0.1.7/airtestProject/scripts/OdinExample.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.6/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.7/airtestProject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.6
+Version: 0.1.7
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.6/airtestProject.egg-info/SOURCES.txt` & `airtestproject-0.1.7/airtestProject.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 airtestProject/commons/utils/gotCommon.py
 airtestProject/commons/utils/logger.py
 airtestProject/commons/utils/myAirtest.py
 airtestProject/commons/utils/myPoco.py
 airtestProject/commons/utils/ocrTemplate.py
 airtestProject/commons/utils/page.py
 airtestProject/commons/utils/reportUtil.py
+airtestProject/commons/utils/test.py
 airtestProject/commons/utils/tools.py
 airtestProject/commons/utils/utils.py
 airtestProject/factory/SingletonFactory.py
 airtestProject/factory/__init__.py
 airtestProject/factory/operateFactory.py
 airtestProject/manager/DeviceManager.py
 airtestProject/manager/LogManager.py
```

### Comparing `airtestproject-0.1.6/setup.py` & `airtestproject-0.1.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
```

