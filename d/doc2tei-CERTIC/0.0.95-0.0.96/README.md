# Comparing `tmp/doc2tei-CERTIC-0.0.95.tar.gz` & `tmp/doc2tei-CERTIC-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc2tei-CERTIC-0.0.95.tar", last modified: Mon Apr 22 08:03:03 2024, max compression
+gzip compressed data, was "doc2tei-CERTIC-0.0.96.tar", last modified: Mon Apr 22 12:52:21 2024, max compression
```

## Comparing `doc2tei-CERTIC-0.0.95.tar` & `doc2tei-CERTIC-0.0.96.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.005378 doc2tei-CERTIC-0.0.95/doc2tei/
--rw-rw-rw-   0 root         (0) root         (0)    21029 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.005378 doc2tei-CERTIC-0.0.95/doc2tei/resources/
--rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/saxon9.jar
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.097384 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/
--rw-rw-rw-   0 root         (0) root         (0)   357736 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng
--rw-rw-rw-   0 root         (0) root         (0)   176870 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/openedition.rng
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.117385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/
--rw-rw-rw-   0 root         (0) root         (0)     4312 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8141 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4404 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
--rw-rw-rw-   0 root         (0) root         (0)    33450 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3098 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.121385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/
--rw-rw-rw-   0 root         (0) root         (0)     3431 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8617 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.121385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/
--rw-rw-rw-   0 root         (0) root         (0)     3552 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/enrich.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.125386 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/
--rw-rw-rw-   0 root         (0) root         (0)     4975 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3685 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4512 2024-04-08 16:08:32.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4093 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3746 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-review.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-sp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4248 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     5996 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.153387 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/
--rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-errors.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4036 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12240 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-styles-id.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.157388 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/
--rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.165388 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/
--rw-rw-rw-   0 root         (0) root         (0)     8786 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/organise.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.181389 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/
--rw-rw-rw-   0 root         (0) root         (0)     4102 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/back.xsl
--rw-rw-rw-   0 root         (0) root         (0)    14220 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_code.xsl
--rw-rw-rw-   0 root         (0) root         (0)     9140 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_div-para.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12822 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_linking.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4335 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_list.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3468 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_note.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3592 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_typo.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12206 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/front.xsl
--rw-rw-rw-   0 root         (0) root         (0)    37403 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3499 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/totei.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.193390 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/
--rwxrwxrwx   0 root         (0) root         (0)     9839 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/
--rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2286 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.768768 doc2tei-CERTIC-0.0.96/doc2tei/
+-rw-rw-rw-   0 root         (0) root         (0)    21029 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.768768 doc2tei-CERTIC-0.0.96/doc2tei/resources/
+-rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/saxon9.jar
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.780769 doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/
+-rw-rw-rw-   0 root         (0) root         (0)   357868 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/metopes.rng
+-rw-rw-rw-   0 root         (0) root         (0)   176870 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/openedition.rng
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.780769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8141 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    33450 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.780769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/
+-rw-rw-rw-   0 root         (0) root         (0)     3431 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8617 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.780769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-03-enrich/
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-03-enrich/enrich.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.784769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4512 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-review.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-sp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.784769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-errors.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12240 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-styles-id.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.784769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-06-hierarchize/
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.784769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-07-organise/
+-rw-rw-rw-   0 root         (0) root         (0)     8786 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-07-organise/organise.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/
+-rw-rw-rw-   0 root         (0) root         (0)     4102 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/back.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    14220 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4026 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_code.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     9140 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_div-para.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_linking.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4335 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_list.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_note.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3592 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_typo.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12206 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/front.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    37403 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/teiHeader.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/totei.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-09-toOpenedition/
+-rwxrwxrwx   0 root         (0) root         (0)     9839 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 12:52:21.000000 doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 12:52:21.788769 doc2tei-CERTIC-0.0.96/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-22 12:52:02.000000 doc2tei-CERTIC-0.0.96/setup.py
```

### Comparing `doc2tei-CERTIC-0.0.95/PKG-INFO` & `doc2tei-CERTIC-0.0.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.95
+Version: 0.0.96
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.95/README.md` & `doc2tei-CERTIC-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/__init__.py` & `doc2tei-CERTIC-0.0.96/doc2tei/__init__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/__main__.py` & `doc2tei-CERTIC-0.0.96/doc2tei/__main__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/saxon9.jar` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/saxon9.jar`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/metopes.rng`

 * *Files 1% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/metopes.rng`

```diff
@@ -6328,24 +6328,26 @@
       <ref name="att.global.attribute.xmlspace"/>
       <ref name="att.global.rendition.attribute.rend"/>
       <ref name="att.global.rendition.attribute.rendition"/>
       <optional>
         <attribute name="type">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">classifies the title according to some convenient typology.</a:documentation>
           <choice>
-            <value>collection</value>
-            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>compl</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>full</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>main</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>orig</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>series</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>set</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>short</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>sub</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>sup</value>
             <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
             <value>trl</value>
```

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/openedition.rng` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/schema/openedition.rng`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-01-cleanup/cleanup.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/enrich.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-03-enrich/enrich.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-cit.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure-grp.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-figure-grp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-figure.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-floatingText.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-review.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-review.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-sp.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/group-sp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-review.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-04-group/hierarchize-review.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-errors.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-errors.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-hierarchy.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-hierarchy.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-styles-id.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-05-control/control-styles-id.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/organise.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-07-organise/organise.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/back.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/back.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_cit.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_code.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_code.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_div-para.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_div-para.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_figure.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_figure.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_linking.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_linking.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_list.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_list.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_note.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_note.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_typo.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/core_typo.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/front.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/front.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

 * *Files 0% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

```diff
@@ -307,15 +307,15 @@
               <xsl:value-of select="//meta:user-defined[@meta:name='tplVersion']"/>
             </xsl:attribute>
             <label>Word template</label>
             <desc>Version of MS Word template used</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
-          <application version="0.0.95">
+          <application version="0.0.96">
             <xsl:attribute name="ident" select="concat('circe-',$source)"/>
             <label>Circé</label>
             <desc>Document converted into TEI using Circé application (doc2tei pipeline)</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
         </appInfo>
```

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/totei.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-08-totei/totei.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl` & `doc2tei-CERTIC-0.0.96/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/PKG-INFO` & `doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.95
+Version: 0.0.96
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/SOURCES.txt` & `doc2tei-CERTIC-0.0.96/doc2tei_CERTIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.95/setup.py` & `doc2tei-CERTIC-0.0.96/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="doc2tei-CERTIC",
-    version="0.0.95",
+    version="0.0.96",
     author="Mickaël Desfrênes",
     author_email="mickael.desfrenes@unicaen.fr",
     description="Convert ODT and DOCX files to TEI",
     long_description="Convert ODT and DOCX files to TEI",
     long_description_content_type="text/plain",
     url="https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe",
     packages=setuptools.find_packages(),
```

