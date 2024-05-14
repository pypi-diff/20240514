# Comparing `tmp/bdbag-1.7.2.tar.gz` & `tmp/bdbag-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdbag-1.7.2.tar", last modified: Thu Mar 14 20:55:31 2024, max compression
+gzip compressed data, was "bdbag-1.7.3.tar", last modified: Tue May 14 19:15:18 2024, max compression
```

## Comparing `bdbag-1.7.2.tar` & `bdbag-1.7.3.tar`

### file list

```diff
@@ -1,468 +1,468 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.160357 bdbag-1.7.2/
--rw-rw-rw-   0        0        0       18 2024-02-21 06:15:39.000000 bdbag-1.7.2/.gitattributes
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.738863 bdbag-1.7.2/.github/
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.771747 bdbag-1.7.2/.github/workflows/
--rw-rw-rw-   0        0        0     1607 2024-03-05 04:03:01.000000 bdbag-1.7.2/.github/workflows/bdbag.yml
--rw-rw-rw-   0        0        0    21505 2024-03-14 20:33:46.000000 bdbag-1.7.2/CHANGELOG.md
--rw-rw-rw-   0        0        0    11357 2024-02-21 06:15:39.000000 bdbag-1.7.2/LICENSE
--rw-rw-rw-   0        0        0     7813 2024-03-14 20:55:31.160357 bdbag-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-03-13 19:36:59.000000 bdbag-1.7.2/Pipfile
--rw-rw-rw-   0        0        0    48220 2024-03-13 22:09:29.000000 bdbag-1.7.2/Pipfile.lock
--rw-rw-rw-   0        0        0     5778 2024-02-21 06:15:39.000000 bdbag-1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.781617 bdbag-1.7.2/bdbag/
--rw-rw-rw-   0        0        0    10515 2024-03-13 20:43:17.000000 bdbag-1.7.2/bdbag/__init__.py
--rw-rw-rw-   0        0        0    34188 2024-03-13 22:44:11.000000 bdbag-1.7.2/bdbag/bdbag_api.py
--rw-rw-rw-   0        0        0    20617 2024-03-14 18:54:11.000000 bdbag-1.7.2/bdbag/bdbag_cli.py
--rw-rw-rw-   0        0        0    10046 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/bdbag_config.py
--rw-rw-rw-   0        0        0    13883 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/bdbag_ro.py
--rw-rw-rw-   0        0        0    27410 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/bdbag_utils.py
--rw-rw-rw-   0        0        0    24451 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/bdbagit.py
--rw-rw-rw-   0        0        0     2357 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/bdbagit_profile.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.791642 bdbag-1.7.2/bdbag/fetch/
--rw-rw-rw-   0        0        0     2233 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.795386 bdbag-1.7.2/bdbag/fetch/auth/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/auth/__init__.py
--rw-rw-rw-   0        0        0     3282 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/auth/cookies.py
--rw-rw-rw-   0        0        0     6159 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/auth/keychain.py
--rw-rw-rw-   0        0        0     4980 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/fetcher.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.803144 bdbag-1.7.2/bdbag/fetch/resolvers/
--rw-rw-rw-   0        0        0     2486 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/resolvers/__init__.py
--rw-rw-rw-   0        0        0     2802 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/resolvers/ark_resolver.py
--rw-rw-rw-   0        0        0     3142 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/resolvers/base_resolver.py
--rw-rw-rw-   0        0        0     2271 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/resolvers/dataguid_resolver.py
--rw-rw-rw-   0        0        0     2600 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/resolvers/doi_resolver.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.815118 bdbag-1.7.2/bdbag/fetch/transports/
--rw-rw-rw-   0        0        0     2701 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/base_transport.py
--rw-rw-rw-   0        0        0     7061 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_boto3.py
--rw-rw-rw-   0        0        0     3348 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_ftp.py
--rw-rw-rw-   0        0        0     5071 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_gcs.py
--rw-rw-rw-   0        0        0     5133 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_globus.py
--rw-rw-rw-   0        0        0    12739 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_http.py
--rw-rw-rw-   0        0        0     1389 2024-02-21 06:15:39.000000 bdbag-1.7.2/bdbag/fetch/transports/fetch_tag.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.158147 bdbag-1.7.2/bdbag.egg-info/
--rw-rw-rw-   0        0        0     7813 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19309 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      266 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-14 20:55:30.000000 bdbag-1.7.2/bdbag.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.818311 bdbag-1.7.2/doc/
--rw-rw-rw-   0        0        0    43813 2024-03-14 20:36:18.000000 bdbag-1.7.2/doc/api.md
--rw-rw-rw-   0        0        0    40083 2024-03-14 20:36:18.000000 bdbag-1.7.2/doc/cli.md
--rw-rw-rw-   0        0        0    30778 2024-03-14 20:01:56.000000 bdbag-1.7.2/doc/config.md
--rw-rw-rw-   0        0        0    10987 2024-02-21 06:15:39.000000 bdbag-1.7.2/doc/utils.md
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.742214 bdbag-1.7.2/examples/
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.820422 bdbag-1.7.2/examples/bagofbags/
--rw-rw-rw-   0        0        0     1519 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/bagofbags/README.md
--rw-rw-rw-   0        0        0     7342 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/bagofbags/bagofbags.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.823585 bdbag-1.7.2/examples/bagofbags/images/
--rw-rw-rw-   0        0        0   127142 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/bagofbags/images/MetaBags.png
--rw-rw-rw-   0        0        0    48632 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/bagofbags/images/MetaBags.pptx
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.824587 bdbag-1.7.2/examples/metamanifests/
--rw-rw-rw-   0        0        0      840 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/metamanifests/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.743216 bdbag-1.7.2/examples/metamanifests/samples/
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.828301 bdbag-1.7.2/examples/metamanifests/samples/sample1/
--rw-rw-rw-   0        0        0      236 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/metamanifests/samples/sample1/metadata.json
--rw-rw-rw-   0        0        0      741 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/metamanifests/samples/sample1/remote-files.json
--rw-rw-rw-   0        0        0     4729 2024-02-21 06:15:39.000000 bdbag-1.7.2/examples/metamanifests/samples/sample1/ro_metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.830433 bdbag-1.7.2/profiles/
--rw-rw-rw-   0        0        0      940 2024-02-21 06:15:39.000000 bdbag-1.7.2/profiles/bdbag-profile.json
--rw-rw-rw-   0        0        0     1091 2024-02-21 06:15:39.000000 bdbag-1.7.2/profiles/bdbag-ro-profile.json
--rw-rw-rw-   0        0        0      560 2024-03-14 20:55:31.161382 bdbag-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     3277 2024-03-13 22:57:31.000000 bdbag-1.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.837967 bdbag-1.7.2/test/
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.764307 bdbag-1.7.2/test/test-data/
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.851759 bdbag-1.7.2/test/test-data/test-archives/
--rw-rw-rw-   0        0        0     2355 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag-fetch-http.zip
--rw-rw-rw-   0        0        0     2460 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag-multi-parent.tgz
--rw-rw-rw-   0        0        0     5253 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag-multi-parent.zip
--rw-rw-rw-   0        0        0     2369 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag-no-parent.tgz
--rw-rw-rw-   0        0        0     4596 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag-no-parent.zip
--rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.7z
--rw-rw-rw-   0        0        0     2319 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.bz2
--rw-rw-rw-   0        0        0    20480 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.tar
--rw-rw-rw-   0        0        0     2370 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.tgz
--rw-rw-rw-   0        0        0     2336 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.xz
--rw-rw-rw-   0        0        0     5257 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-archives/test-bag.zip
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.860376 bdbag-1.7.2/test/test-data/test-bag/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.105763 bdbag-1.7.2/test/test-data/test-bag/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.106765 bdbag-1.7.2/test/test-data/test-bag/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.107818 bdbag-1.7.2/test/test-data/test-bag/data/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.871071 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/
--rw-rw-rw-   0        0        0      351 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/bagit.txt
--rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/fetch.txt
--rw-rw-rw-   0        0        0      124 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/manifest-md5.txt
--rw-rw-rw-   0        0        0      140 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
--rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
--rw-rw-rw-   0        0        0      316 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.872119 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/metadata/
--rw-rw-rw-   0        0        0     1207 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/metadata/manifest.json
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      459 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      651 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1163 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.879509 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.897499 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/data/README.txt
--rw-rw-rw-   0        0        0       53 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/fetch.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.887206 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.887268 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/data/README.txt
--rw-rw-rw-   0        0        0       44 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/fetch.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.895346 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.896395 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/data/README.txt
--rw-rw-rw-   0        0        0       62 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/fetch.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.903786 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.904846 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/data/README.txt
--rw-rw-rw-   0        0        0       90 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/fetch.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.912493 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.912493 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/data/README.txt
--rw-rw-rw-   0        0        0       59 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/fetch.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.919291 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/
--rw-rw-rw-   0        0        0      349 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.931112 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/data/
--rw-rw-rw-   0        0        0     1024 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/data/README.txt
--rw-rw-rw-   0        0        0       52 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/fetch.txt
--rw-rw-rw-   0        0        0       97 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.927039 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/
--rw-rw-rw-   0        0        0      349 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.929620 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/data/
--rw-rw-rw-   0        0        0     1024 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
--rw-rw-rw-   0        0        0       52 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
--rw-rw-rw-   0        0        0       97 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
--rw-rw-rw-   0        0        0      161 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.937804 bdbag-1.7.2/test/test-data/test-bag-fetch-http/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.972144 bdbag-1.7.2/test/test-data/test-bag-fetch-http/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/data/README.txt
--rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/fetch.txt
--rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.945840 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.945903 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/data/README.txt
--rw-rw-rw-   0        0        0      409 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/fetch.txt
--rw-rw-rw-   0        0        0      232 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
--rw-rw-rw-   0        0        0      360 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.952962 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.955047 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
--rw-rw-rw-   0        0        0      153 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
--rw-rw-rw-   0        0        0      111 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
--rw-rw-rw-   0        0        0      175 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.963186 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.963186 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
--rw-rw-rw-   0        0        0      269 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
--rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.971078 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.972144 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
--rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.981085 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.981140 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/data/README.txt
--rw-rw-rw-   0        0        0       48 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/fetch.txt
--rw-rw-rw-   0        0        0      115 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/manifest-md5.txt
--rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.988304 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.989374 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/data/README.txt
--rw-rw-rw-   0        0        0      113 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/fetch.txt
--rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:30.999673 bdbag-1.7.2/test/test-data/test-bag-incomplete/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.008038 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.009580 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.010583 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/data/test2/test2.txt
--rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/fetch.txt
--rw-rw-rw-   0        0        0      219 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/manifest-sha1.txt
--rw-rw-rw-   0        0        0      444 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.005952 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/
--rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.008038 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      282 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.017327 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.019521 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      284 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
--rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.028266 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.031834 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
--rw-rw-rw-   0        0        0      199 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
--rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
--rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
--rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.036340 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/
--rw-rw-rw-   0        0        0      320 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.037380 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
--rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      192 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.047403 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.048406 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.049545 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.050545 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
--rw-rw-rw-   0        0        0      187 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
--rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
--rw-rw-rw-   0        0        0      339 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      563 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0     1011 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.059962 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.061067 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.062130 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.063182 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
--rw-rw-rw-   0        0        0      105 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
--rw-rw-rw-   0        0        0      121 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
--rw-rw-rw-   0        0        0      169 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
--rw-rw-rw-   0        0        0      297 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.072176 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.073638 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.074719 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
--rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.084505 bdbag-1.7.2/test/test-data/test-bag-no-data/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/bagit.txt
--rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.094148 bdbag-1.7.2/test/test-data/test-bag-profile/
--rw-rw-rw-   0        0        0      292 2024-03-13 22:13:24.000000 bdbag-1.7.2/test/test-data/test-bag-profile/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.096297 bdbag-1.7.2/test/test-data/test-bag-profile/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/data/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.097299 bdbag-1.7.2/test/test-data/test-bag-profile/data/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/data/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.098340 bdbag-1.7.2/test/test-data/test-bag-profile/data/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/data/test2/test2.txt
--rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/manifest-md5.txt
--rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/manifest-sha1.txt
--rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/manifest-sha256.txt
--rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-profile/manifest-sha512.txt
--rw-rw-rw-   0        0        0      296 2024-03-13 22:13:24.000000 bdbag-1.7.2/test/test-data/test-bag-profile/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      344 2024-03-13 22:13:24.000000 bdbag-1.7.2/test/test-data/test-bag-profile/tagmanifest-sha1.txt
--rw-rw-rw-   0        0        0      488 2024-03-13 22:13:24.000000 bdbag-1.7.2/test/test-data/test-bag-profile/tagmanifest-sha256.txt
--rw-rw-rw-   0        0        0      872 2024-03-13 22:13:24.000000 bdbag-1.7.2/test/test-data/test-bag-profile/tagmanifest-sha512.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.104649 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/
--rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
--rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/bagit.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.105763 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/data/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/data/README.txt
--rw-rw-rw-   0        0        0      135 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/fetch.txt
--rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
--rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
--rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
--rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.108855 bdbag-1.7.2/test/test-data/test-bdbagit/
--rw-rw-rw-   0        0        0      221 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bdbagit/README
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.111006 bdbag-1.7.2/test/test-data/test-bdbagit/loc/
--rw-rw-rw-   0        0        0   139367 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
--rw-rw-rw-   0        0        0   143435 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.115278 bdbag-1.7.2/test/test-data/test-bdbagit/si/
--rw-rw-rw-   0        0        0   381813 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
--rw-rw-rw-   0        0        0   326929 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.151859 bdbag-1.7.2/test/test-data/test-config/
--rw-rw-rw-   0        0        0      415 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/base-config.json
--rw-rw-rw-   0        0        0      806 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-10.json
--rw-rw-rw-   0        0        0      513 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-11.json
--rw-rw-rw-   0        0        0      576 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-12.json
--rw-rw-rw-   0        0        0      400 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-13.json
--rw-rw-rw-   0        0        0      401 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-2.json
--rw-rw-rw-   0        0        0     2773 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-3.json
--rw-rw-rw-   0        0        0     1243 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-4.json
--rw-rw-rw-   0        0        0     1199 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-5.json
--rw-rw-rw-   0        0        0     1052 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-6.json
--rw-rw-rw-   0        0        0      825 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-7.json
--rw-rw-rw-   0        0        0      861 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-8.json
--rw-rw-rw-   0        0        0      828 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config-9.json
--rw-rw-rw-   0        0        0      354 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-config.json
--rw-rw-rw-   0        0        0      244 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-cookies-1.txt
--rw-rw-rw-   0        0        0      244 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-cookies-2.txt
--rw-rw-rw-   0        0        0       83 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-cookies-bad.txt
--rw-rw-rw-   0        0        0      861 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-2.json
--rw-rw-rw-   0        0        0     1574 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-encoding.json
--rw-rw-rw-   0        0        0      616 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
--rw-rw-rw-   0        0        0      944 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest.json
--rw-rw-rw-   0        0        0      312 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-invalid-fetch-manifest-1.json
--rw-rw-rw-   0        0        0      187 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-invalid-fetch-manifest-2.json
--rw-rw-rw-   0        0        0      199 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-1.json
--rw-rw-rw-   0        0        0      233 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-2.json
--rw-rw-rw-   0        0        0      288 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-3.json
--rw-rw-rw-   0        0        0      212 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-4.json
--rw-rw-rw-   0        0        0      191 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-5.json
--rw-rw-rw-   0        0        0      278 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-6.json
--rw-rw-rw-   0        0        0      279 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-7.json
--rw-rw-rw-   0        0        0      704 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-8.json
--rw-rw-rw-   0        0        0      672 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-9.json
--rw-rw-rw-   0        0        0      146 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-keychain-bad-1.json
--rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-metadata.json
--rw-rw-rw-   0        0        0     1259 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-config/test-ro-metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.152958 bdbag-1.7.2/test/test-data/test-dir/
--rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-dir/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.153960 bdbag-1.7.2/test/test-data/test-dir/test1/
--rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-dir/test1/test1.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.154997 bdbag-1.7.2/test/test-data/test-dir/test2/
--rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-dir/test2/test2.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.157097 bdbag-1.7.2/test/test-data/test-http/
--rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-http/test-fetch-http.txt
--rw-rw-rw-   0        0        0      223 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-http/test-fetch-identifier.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 20:55:31.157097 bdbag-1.7.2/test/test-data/test-http-encoded/
--rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test-data/test-http-encoded/test fetch%http®.txt
--rw-rw-rw-   0        0        0    55309 2024-03-13 21:41:26.000000 bdbag-1.7.2/test/test_api.py
--rw-rw-rw-   0        0        0    48971 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test_bdbagit.py
--rw-rw-rw-   0        0        0    14498 2024-03-13 21:43:49.000000 bdbag-1.7.2/test/test_cli.py
--rw-rw-rw-   0        0        0     8155 2024-02-21 06:15:39.000000 bdbag-1.7.2/test/test_common.py
--rw-rw-rw-   0        0        0    57435 2024-03-13 18:21:39.000000 bdbag-1.7.2/test/test_remote.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.203431 bdbag-1.7.3/
+-rw-rw-rw-   0        0        0       18 2024-02-21 06:15:39.000000 bdbag-1.7.3/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.559315 bdbag-1.7.3/.github/
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.606599 bdbag-1.7.3/.github/workflows/
+-rw-rw-rw-   0        0        0     1607 2024-03-05 04:03:01.000000 bdbag-1.7.3/.github/workflows/bdbag.yml
+-rw-rw-rw-   0        0        0    22632 2024-05-10 19:31:32.000000 bdbag-1.7.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11357 2024-02-21 06:15:39.000000 bdbag-1.7.3/LICENSE
+-rw-rw-rw-   0        0        0     7813 2024-05-14 19:15:18.203431 bdbag-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-03-13 19:36:59.000000 bdbag-1.7.3/Pipfile
+-rw-rw-rw-   0        0        0    48220 2024-03-13 22:09:29.000000 bdbag-1.7.3/Pipfile.lock
+-rw-rw-rw-   0        0        0     5778 2024-03-15 05:21:49.000000 bdbag-1.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.622222 bdbag-1.7.3/bdbag/
+-rw-rw-rw-   0        0        0    10559 2024-05-09 22:06:10.000000 bdbag-1.7.3/bdbag/__init__.py
+-rw-rw-rw-   0        0        0    34790 2024-05-10 19:31:32.000000 bdbag-1.7.3/bdbag/bdbag_api.py
+-rw-rw-rw-   0        0        0    21268 2024-05-10 19:31:32.000000 bdbag-1.7.3/bdbag/bdbag_cli.py
+-rw-rw-rw-   0        0        0    10046 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/bdbag_config.py
+-rw-rw-rw-   0        0        0    13902 2024-05-09 22:06:10.000000 bdbag-1.7.3/bdbag/bdbag_ro.py
+-rw-rw-rw-   0        0        0    27410 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/bdbag_utils.py
+-rw-rw-rw-   0        0        0    24470 2024-05-09 22:06:10.000000 bdbag-1.7.3/bdbag/bdbagit.py
+-rw-rw-rw-   0        0        0     2357 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/bdbagit_profile.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.622222 bdbag-1.7.3/bdbag/fetch/
+-rw-rw-rw-   0        0        0     2233 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.622222 bdbag-1.7.3/bdbag/fetch/auth/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/auth/__init__.py
+-rw-rw-rw-   0        0        0     3282 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/auth/cookies.py
+-rw-rw-rw-   0        0        0     6159 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/auth/keychain.py
+-rw-rw-rw-   0        0        0     4980 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.638975 bdbag-1.7.3/bdbag/fetch/resolvers/
+-rw-rw-rw-   0        0        0     2486 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/resolvers/__init__.py
+-rw-rw-rw-   0        0        0     2802 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/resolvers/ark_resolver.py
+-rw-rw-rw-   0        0        0     3142 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/resolvers/base_resolver.py
+-rw-rw-rw-   0        0        0     2271 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/resolvers/dataguid_resolver.py
+-rw-rw-rw-   0        0        0     2600 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/resolvers/doi_resolver.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.653985 bdbag-1.7.3/bdbag/fetch/transports/
+-rw-rw-rw-   0        0        0     2701 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/base_transport.py
+-rw-rw-rw-   0        0        0     7061 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_boto3.py
+-rw-rw-rw-   0        0        0     3348 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_ftp.py
+-rw-rw-rw-   0        0        0     5071 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_gcs.py
+-rw-rw-rw-   0        0        0     5133 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_globus.py
+-rw-rw-rw-   0        0        0    12739 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_http.py
+-rw-rw-rw-   0        0        0     1389 2024-02-21 06:15:39.000000 bdbag-1.7.3/bdbag/fetch/transports/fetch_tag.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.203431 bdbag-1.7.3/bdbag.egg-info/
+-rw-rw-rw-   0        0        0     7813 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19309 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      266 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 19:15:17.000000 bdbag-1.7.3/bdbag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.653985 bdbag-1.7.3/doc/
+-rw-rw-rw-   0        0        0    44363 2024-05-10 19:31:32.000000 bdbag-1.7.3/doc/api.md
+-rw-rw-rw-   0        0        0    40872 2024-05-10 19:31:32.000000 bdbag-1.7.3/doc/cli.md
+-rw-rw-rw-   0        0        0    30778 2024-03-14 20:01:56.000000 bdbag-1.7.3/doc/config.md
+-rw-rw-rw-   0        0        0    10987 2024-02-21 06:15:39.000000 bdbag-1.7.3/doc/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.571326 bdbag-1.7.3/examples/
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.653985 bdbag-1.7.3/examples/bagofbags/
+-rw-rw-rw-   0        0        0     1519 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/bagofbags/README.md
+-rw-rw-rw-   0        0        0     7342 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/bagofbags/bagofbags.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.653985 bdbag-1.7.3/examples/bagofbags/images/
+-rw-rw-rw-   0        0        0   127142 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/bagofbags/images/MetaBags.png
+-rw-rw-rw-   0        0        0    48632 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/bagofbags/images/MetaBags.pptx
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.671170 bdbag-1.7.3/examples/metamanifests/
+-rw-rw-rw-   0        0        0      840 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/metamanifests/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.571326 bdbag-1.7.3/examples/metamanifests/samples/
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.671170 bdbag-1.7.3/examples/metamanifests/samples/sample1/
+-rw-rw-rw-   0        0        0      236 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/metamanifests/samples/sample1/metadata.json
+-rw-rw-rw-   0        0        0      741 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/metamanifests/samples/sample1/remote-files.json
+-rw-rw-rw-   0        0        0     4729 2024-02-21 06:15:39.000000 bdbag-1.7.3/examples/metamanifests/samples/sample1/ro_metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.671170 bdbag-1.7.3/profiles/
+-rw-rw-rw-   0        0        0      940 2024-02-21 06:15:39.000000 bdbag-1.7.3/profiles/bdbag-profile.json
+-rw-rw-rw-   0        0        0     1091 2024-02-21 06:15:39.000000 bdbag-1.7.3/profiles/bdbag-ro-profile.json
+-rw-rw-rw-   0        0        0      560 2024-05-14 19:15:18.203431 bdbag-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     3277 2024-03-13 22:57:31.000000 bdbag-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.685684 bdbag-1.7.3/test/
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.590975 bdbag-1.7.3/test/test-data/
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.716951 bdbag-1.7.3/test/test-data/test-archives/
+-rw-rw-rw-   0        0        0     2355 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag-fetch-http.zip
+-rw-rw-rw-   0        0        0     2460 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag-multi-parent.tgz
+-rw-rw-rw-   0        0        0     5253 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag-multi-parent.zip
+-rw-rw-rw-   0        0        0     2369 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag-no-parent.tgz
+-rw-rw-rw-   0        0        0     4596 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag-no-parent.zip
+-rw-rw-rw-   0        0        0        0 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.7z
+-rw-rw-rw-   0        0        0     2319 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.bz2
+-rw-rw-rw-   0        0        0    20480 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.tar
+-rw-rw-rw-   0        0        0     2370 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.tgz
+-rw-rw-rw-   0        0        0     2336 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.xz
+-rw-rw-rw-   0        0        0     5257 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-archives/test-bag.zip
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.748204 bdbag-1.7.3/test/test-data/test-bag/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.109222 bdbag-1.7.3/test/test-data/test-bag/data/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.771345 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/
+-rw-rw-rw-   0        0        0      351 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/bagit.txt
+-rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/fetch.txt
+-rw-rw-rw-   0        0        0      124 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/manifest-md5.txt
+-rw-rw-rw-   0        0        0      140 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      316 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/manifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.771345 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/metadata/
+-rw-rw-rw-   0        0        0     1207 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/metadata/manifest.json
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      459 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      651 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1163 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.795501 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.826777 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/data/README.txt
+-rw-rw-rw-   0        0        0       53 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/fetch.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.811147 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.811147 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/data/README.txt
+-rw-rw-rw-   0        0        0       44 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/fetch.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.826777 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.826777 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/data/README.txt
+-rw-rw-rw-   0        0        0       62 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/fetch.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ark2/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.842391 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.842391 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/data/README.txt
+-rw-rw-rw-   0        0        0       90 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/fetch.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-dataguid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.858000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.858000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/data/README.txt
+-rw-rw-rw-   0        0        0       59 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/fetch.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-doi/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.874024 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/
+-rw-rw-rw-   0        0        0      349 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.905292 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/data/
+-rw-rw-rw-   0        0        0     1024 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/data/README.txt
+-rw-rw-rw-   0        0        0       52 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/fetch.txt
+-rw-rw-rw-   0        0        0       97 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.889689 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/
+-rw-rw-rw-   0        0        0      349 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.889689 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/data/
+-rw-rw-rw-   0        0        0     1024 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/data/1KB.zip
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/data/README.txt
+-rw-rw-rw-   0        0        0       52 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/fetch.txt
+-rw-rw-rw-   0        0        0       97 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/manifest-md5.txt
+-rw-rw-rw-   0        0        0      161 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-ftp-auth/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.920941 bdbag-1.7.3/test/test-data/test-bag-fetch-http/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.952163 bdbag-1.7.3/test/test-data/test-bag-fetch-http/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/data/README.txt
+-rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/fetch.txt
+-rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.920941 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.920941 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/data/README.txt
+-rw-rw-rw-   0        0        0      409 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/fetch.txt
+-rw-rw-rw-   0        0        0      232 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/manifest-md5.txt
+-rw-rw-rw-   0        0        0      360 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-bad/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.936541 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.936541 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/data/README.txt
+-rw-rw-rw-   0        0        0      153 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/fetch.txt
+-rw-rw-rw-   0        0        0      111 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/manifest-md5.txt
+-rw-rw-rw-   0        0        0      175 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-encoded-filename/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.952163 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.952163 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/data/README.txt
+-rw-rw-rw-   0        0        0      269 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/fetch.txt
+-rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-no-redirect/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.952163 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.952163 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-http-unexpected-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.971795 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.971795 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/data/README.txt
+-rw-rw-rw-   0        0        0       48 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/fetch.txt
+-rw-rw-rw-   0        0        0      115 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/manifest-md5.txt
+-rw-rw-rw-   0        0        0      179 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-minid/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.971795 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.971795 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/data/README.txt
+-rw-rw-rw-   0        0        0      113 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/fetch.txt
+-rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-fetch-tag/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.983805 bdbag-1.7.3/test/test-data/test-bag-incomplete/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      188 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/fetch.txt
+-rw-rw-rw-   0        0        0      219 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      444 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/
+-rw-rw-rw-   0        0        0      348 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      282 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-incomplete-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:17.999442 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      284 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-duplicate-manifest-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.015067 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.015067 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/data/README.txt
+-rw-rw-rw-   0        0        0      199 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/data/test-fetch-identifier.txt
+-rw-rw-rw-   0        0        0      280 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/fetch.txt
+-rw-rw-rw-   0        0        0      174 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-md5.txt
+-rw-rw-rw-   0        0        0      270 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-fetch-filesize/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.015067 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/
+-rw-rw-rw-   0        0        0      320 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.030692 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/data/README.txt
+-rw-rw-rw-   0        0        0       50 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      192 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-state-manifest-fetch/tagmanifest-md5.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.030692 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.030692 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.046347 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.046347 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      187 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      339 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      563 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0     1011 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.046347 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.046347 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.061941 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.061941 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      105 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/manifest-md5.txt
+-rw-rw-rw-   0        0        0      121 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      169 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      297 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.071949 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.071949 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.071949 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/data/test1/test1.txt
+-rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.077959 bdbag-1.7.3/test/test-data/test-bag-no-data/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/bagit.txt
+-rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-no-data/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-profile/
+-rw-rw-rw-   0        0        0      292 2024-03-13 22:13:24.000000 bdbag-1.7.3/test/test-data/test-bag-profile/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-profile/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/data/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-profile/data/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/data/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-profile/data/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/data/test2/test2.txt
+-rw-rw-rw-   0        0        0      160 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/manifest-md5.txt
+-rw-rw-rw-   0        0        0      184 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/manifest-sha1.txt
+-rw-rw-rw-   0        0        0      256 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      448 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-profile/manifest-sha512.txt
+-rw-rw-rw-   0        0        0      296 2024-03-13 22:13:24.000000 bdbag-1.7.3/test/test-data/test-bag-profile/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      344 2024-03-13 22:13:24.000000 bdbag-1.7.3/test/test-data/test-bag-profile/tagmanifest-sha1.txt
+-rw-rw-rw-   0        0        0      488 2024-03-13 22:13:24.000000 bdbag-1.7.3/test/test-data/test-bag-profile/tagmanifest-sha256.txt
+-rw-rw-rw-   0        0        0      872 2024-03-13 22:13:24.000000 bdbag-1.7.3/test/test-data/test-bag-profile/tagmanifest-sha512.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/
+-rw-rw-rw-   0        0        0      321 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/bag-info.txt
+-rw-rw-rw-   0        0        0       55 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/bagit.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.093597 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/data/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/data/README.txt
+-rw-rw-rw-   0        0        0      135 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/fetch.txt
+-rw-rw-rw-   0        0        0      109 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/manifest-md5.txt
+-rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/manifest-sha256.txt
+-rw-rw-rw-   0        0        0      235 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/tagmanifest-md5.txt
+-rw-rw-rw-   0        0        0      395 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bag-update-invalid-fetch/tagmanifest-sha256.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.109222 bdbag-1.7.3/test/test-data/test-bdbagit/
+-rw-rw-rw-   0        0        0      221 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bdbagit/README
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.109222 bdbag-1.7.3/test/test-data/test-bdbagit/loc/
+-rw-rw-rw-   0        0        0   139367 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg
+-rw-rw-rw-   0        0        0   143435 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.109222 bdbag-1.7.3/test/test-data/test-bdbagit/si/
+-rw-rw-rw-   0        0        0   381813 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg
+-rw-rw-rw-   0        0        0   326929 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.172269 bdbag-1.7.3/test/test-data/test-config/
+-rw-rw-rw-   0        0        0      415 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/base-config.json
+-rw-rw-rw-   0        0        0      806 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-10.json
+-rw-rw-rw-   0        0        0      513 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-11.json
+-rw-rw-rw-   0        0        0      576 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-12.json
+-rw-rw-rw-   0        0        0      400 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-13.json
+-rw-rw-rw-   0        0        0      401 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-2.json
+-rw-rw-rw-   0        0        0     2773 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-3.json
+-rw-rw-rw-   0        0        0     1243 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-4.json
+-rw-rw-rw-   0        0        0     1199 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-5.json
+-rw-rw-rw-   0        0        0     1052 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-6.json
+-rw-rw-rw-   0        0        0      825 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-7.json
+-rw-rw-rw-   0        0        0      861 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-8.json
+-rw-rw-rw-   0        0        0      828 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config-9.json
+-rw-rw-rw-   0        0        0      354 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-config.json
+-rw-rw-rw-   0        0        0      244 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-cookies-1.txt
+-rw-rw-rw-   0        0        0      244 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-cookies-2.txt
+-rw-rw-rw-   0        0        0       83 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-cookies-bad.txt
+-rw-rw-rw-   0        0        0      861 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0     1583 2024-05-09 22:06:10.000000 bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-encoding.json
+-rw-rw-rw-   0        0        0      616 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json
+-rw-rw-rw-   0        0        0      944 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest.json
+-rw-rw-rw-   0        0        0      312 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-invalid-fetch-manifest-1.json
+-rw-rw-rw-   0        0        0      187 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-invalid-fetch-manifest-2.json
+-rw-rw-rw-   0        0        0      199 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-1.json
+-rw-rw-rw-   0        0        0      233 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-2.json
+-rw-rw-rw-   0        0        0      288 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-3.json
+-rw-rw-rw-   0        0        0      212 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-4.json
+-rw-rw-rw-   0        0        0      191 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-5.json
+-rw-rw-rw-   0        0        0      278 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-6.json
+-rw-rw-rw-   0        0        0      279 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-7.json
+-rw-rw-rw-   0        0        0      704 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-8.json
+-rw-rw-rw-   0        0        0      672 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-9.json
+-rw-rw-rw-   0        0        0      146 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-keychain-bad-1.json
+-rw-rw-rw-   0        0        0      173 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-metadata.json
+-rw-rw-rw-   0        0        0     1259 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-config/test-ro-metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.187785 bdbag-1.7.3/test/test-data/test-dir/
+-rw-rw-rw-   0        0        0       66 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-dir/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.187785 bdbag-1.7.3/test/test-data/test-dir/test1/
+-rw-rw-rw-   0        0        0       45 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-dir/test1/test1.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.187785 bdbag-1.7.3/test/test-data/test-dir/test2/
+-rw-rw-rw-   0        0        0       56 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-dir/test2/test2.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.187785 bdbag-1.7.3/test/test-data/test-http/
+-rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-http/test-fetch-http.txt
+-rw-rw-rw-   0        0        0      223 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-http/test-fetch-identifier.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:18.187785 bdbag-1.7.3/test/test-data/test-http-encoded/
+-rw-rw-rw-   0        0        0      201 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test-data/test-http-encoded/test fetch%http®.txt
+-rw-rw-rw-   0        0        0    56384 2024-05-10 19:33:48.000000 bdbag-1.7.3/test/test_api.py
+-rw-rw-rw-   0        0        0    48971 2024-02-21 06:15:39.000000 bdbag-1.7.3/test/test_bdbagit.py
+-rw-rw-rw-   0        0        0    15102 2024-05-10 18:48:27.000000 bdbag-1.7.3/test/test_cli.py
+-rw-rw-rw-   0        0        0     8247 2024-05-10 18:45:47.000000 bdbag-1.7.3/test/test_common.py
+-rw-rw-rw-   0        0        0    57435 2024-05-09 22:06:10.000000 bdbag-1.7.3/test/test_remote.py
```

### Comparing `bdbag-1.7.2/.github/workflows/bdbag.yml` & `bdbag-1.7.3/.github/workflows/bdbag.yml`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/CHANGELOG.md` & `bdbag-1.7.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # CHANGE LOG
 
+## 1.7.3
+
+* Fix erroneous encoding of `%` char in URL field of `fetch.txt` which could break already properly encoded URLs. 
+This was due to a misinterpretation of the spec which states that `%` (along with `CR` and `LF`) should _only_ be URL 
+encoded for the `filename` field and that whitespace (` ` and `\t`) should _only_ be encoded in the URL field.
+  * NOTE: As a best practice, applications should always pre-encode URLs that are added to `fetch.txt` and not rely on `bdbag` to do so, since only whitespace will be encoded.
+* Added a new option `strict` to the `make_bag` API function, along with a corresponding CLI argument. If `strict` is enabled, 
+`make_bag` will automatically validate a newly created or updated bag for structural validity and fail if the resultant bag is invalid. 
+This can be used to ensure that a bag is not persisted without payload file manifests. Additionally, if a created output 
+bag is not structurally valid, the bag will subsequently be reverted back to a normal directory. An updated bag will _not_ be reverted. 
+In either case, a BagValidationError exception will be thrown.
+
 ## 1.7.2
 
 * Introducing support for _bag idempotentcy_, or reproducible bags. A reproducible bag is a bag that has content-equivalence (in both payload _and_ metadata, including manifests) 
-to another bag created a different time with the same content, structure, bagging tool, and profile (if used). When this bag creation and bag archive mode is enabled, 
+to another bag created at a different time, but with the same content, structure, bagging tool, and profile (if used). When this bag creation and bag archive mode is enabled, 
 two separately created bags (or bag archive files) with content-equivalence will _hash equally_, whether the hash is calculated on the bytes of the resultant archive file or calculated on the equivalently ordered set of individual file hashes of the bag's contents. See the [API Guide](https://github.com/fair-research/bdbag/blob/master/doc/api.md) for additional information. 
 * PR: [#59](https://github.com/fair-research/bdbag/pull/59) Only require the external package `importlib_metadata` for Python < 3.8. This module is already included as `importlib.metadata` in Python versions 3.8 and above.  
 * Fix issue with HTTP fetch handler and auth header bearer-token stripping on redirects not getting restored to the cached `requests` session after redirect.
 * Remove dependency on deprecated `distutils` and `distutils.util.strtobool` function.
 * The `is_bag` API function will no longer attempt to instantiate a `Bag` object on non-directories.
 
 ## 1.7.1
```

### Comparing `bdbag-1.7.2/LICENSE` & `bdbag-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/PKG-INFO` & `bdbag-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdbag
-Version: 1.7.2
+Version: 1.7.3
 Summary: Big Data Bag Utilities
 Home-page: https://github.com/fair-research/bdbag/
 Author: Mike D'Arcy
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
@@ -92,15 +92,15 @@
 ["I'll take that to go: Big data bags and minimal identifiers for exchange of large, complex datasets"](https://zenodo.org/record/820878) explains the motivation for BDBags and the related Minid construct, provides details on design and implementation, and gives examples of use. 
 
 ["Reproducible big data science: A case study in continuous FAIRness"](https://www.biorxiv.org/content/early/2018/02/27/268755) presents a data analysis use case in which BDBags and Minids are used to capture a transcription factor binding site analysis.
 
 ### Python Dependencies
 
 *  Python 2.7 is the minimum Python version required. Please note however that Python 2.7 is officially end-of-life and ongoing compatibility between Python 2.7 and `bdbag` (and its dependencies) is not officially supported and cannot be guaranteed.
-*  Python 3, versions 3.7 through 3.11 are the current officially supported releases.
+*  Python 3, versions 3.8 through 3.12 are the current officially supported releases.
 
 ### Installation
 The latest `bdbag` release is available on PyPi and can be installed using `pip`:
 
 ```sh
 pip install bdbag
 ```
```

### Comparing `bdbag-1.7.2/Pipfile.lock` & `bdbag-1.7.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/README.md` & `bdbag-1.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ["I'll take that to go: Big data bags and minimal identifiers for exchange of large, complex datasets"](https://zenodo.org/record/820878) explains the motivation for BDBags and the related Minid construct, provides details on design and implementation, and gives examples of use. 
 
 ["Reproducible big data science: A case study in continuous FAIRness"](https://www.biorxiv.org/content/early/2018/02/27/268755) presents a data analysis use case in which BDBags and Minids are used to capture a transcription factor binding site analysis.
 
 ### Python Dependencies
 
 *  Python 2.7 is the minimum Python version required. Please note however that Python 2.7 is officially end-of-life and ongoing compatibility between Python 2.7 and `bdbag` (and its dependencies) is not officially supported and cannot be guaranteed.
-*  Python 3, versions 3.7 through 3.11 are the current officially supported releases.
+*  Python 3, versions 3.8 through 3.12 are the current officially supported releases.
 
 ### Installation
 The latest `bdbag` release is available on PyPi and can be installed using `pip`:
 
 ```sh
 pip install bdbag
 ```
```

### Comparing `bdbag-1.7.2/bdbag/__init__.py` & `bdbag-1.7.3/bdbag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if sys.version_info >= (3,8):
     from importlib.metadata import distribution, PackageNotFoundError
 else:
     from importlib_metadata import distribution, PackageNotFoundError
 
 logger = logging.getLogger(__name__)
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 __bagit_version__ = "1.8.1"
 __bagit_profile_version__ = "1.3.1"
 
 if sys.version_info > (3,):  # pragma: no cover
     from urllib.parse import quote as urlquote, unquote as urlunquote, urlsplit, urlunsplit, urlparse
     from urllib.request import urlretrieve, urlopen, urlcleanup
 else:  # pragma: no cover
@@ -142,19 +142,19 @@
         raise ValueError('Invalid UTF-8 encoding of content-disposition filename component. %s.' % e)
 
     return n
 
 
 # Per the bagit spec, we just want to replace (%,\r,\n,\t, ) for storage in fetch.txt, but this is also applicable
 # to URI/IRI storage in ro-metadata as well
-def escape_uri(uri, encode_whitespace=True):
+def escape_uri(uri, encode_whitespace=True, encode_other=False):
     if not uri:
         return uri
-
-    uri = uri.replace("%", "%25").replace("\n", "%0A").replace("\r", "%0D")
+    if encode_other:
+        uri = uri.replace("%", "%25").replace("\n", "%0A").replace("\r", "%0D")
     if encode_whitespace:
         uri = uri.replace(" ", "%20").replace("\t", "%09")
 
     return uri
 
 
 def filter_dict(expr, entry):
```

### Comparing `bdbag-1.7.2/bdbag/bdbag_api.py` & `bdbag-1.7.3/bdbag/bdbag_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,16 @@
              prune_manifests=False,
              metadata=None,
              metadata_file=None,
              remote_file_manifest=None,
              config_file=None,
              ro_metadata=None,
              ro_metadata_file=None,
-             idempotent=None):
+             idempotent=None,
+             strict=False):
     bag = None
     try:
         bag = bdbagit.BDBag(bag_path)
     except (bdbagit.BagError, bdbagit.BagValidationError):
         pass
 
     config = read_config(config_file)
@@ -329,14 +330,27 @@
                                checksums=bag_algorithms,
                                remote_entries=remote_files,
                                spec_version=bag_version)
         logger.info('Created bag: %s' % bag_path)
         if bag_ro_metadata:
             bdbro.serialize_bag_ro_metadata(bag_ro_metadata, bag_path)
             bag.save(bag_processes)
+
+    if strict:
+        try:
+            bag._validate_structure()
+        except bdbagit.BagValidationError as e:
+            error = ("The newly created/updated bag is not structurally valid and strict checking has been requested.%s"
+                     " Exception: %s\n" % (" The bag will be reverted back to a normal directory." if not update else "",
+                                           get_typed_exception(e)))
+            logger.error(error)
+            if not update:
+                revert_bag(bag_path)
+            raise bdbagit.BagValidationError(error)
+
     return bag
 
 
 def archive_bag(bag_path, bag_archiver, config_file=None, idempotent=None):
     bag_archiver = bag_archiver.lower()
     bag_path = bag_path.rstrip(os.path.sep)
```

### Comparing `bdbag-1.7.2/bdbag/bdbag_cli.py` & `bdbag-1.7.3/bdbag/bdbag_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,23 @@
     standard_args = parser.add_argument_group('Bag arguments')
 
     update_arg = "--update"
     standard_args.add_argument(
         update_arg, action="store_true",
         help="Update an existing bag dir, regenerating manifests and fetch.txt if necessary.")
 
+    strict_arg = "--strict"
+    standard_args.add_argument(
+        strict_arg, action="store_true",
+        help="Automatically validate a newly created or updated bag for structural validity and fail if the resultant "
+             "bag is invalid. This can be used to ensure that a bag is not persisted without payload file manifests. "
+             "If this flag is set and a created output bag is not structurally valid, the bag will "
+             "subsequently be reverted back to a normal directory. An updated bag will not be reverted. "
+             "In either case, an error is returned.")
+
     revert_arg = "--revert"
     standard_args.add_argument(
         revert_arg, action="store_true",
         help="Revert an existing bag directory back to a normal directory, deleting all bag metadata files. "
              "Payload files in the \'data\' directory will be moved back to the directory root, and the \'data\' "
              "directory will be deleted.")
 
@@ -366,15 +375,16 @@
                              save_manifests=not args.skip_manifests,
                              prune_manifests=args.prune_manifests,
                              metadata=BAG_METADATA if BAG_METADATA else None,
                              metadata_file=args.metadata_file,
                              remote_file_manifest=args.remote_file_manifest,
                              config_file=args.config_file,
                              ro_metadata_file=args.ro_metadata_file,
-                             idempotent=args.idempotent)
+                             idempotent=args.idempotent,
+                             strict=args.strict)
 
         # otherwise just extract the bag if it is an archive and no other conflicting options specified
         elif not (args.validate or args.validate_profile or args.resolve_fetch):
             bdb.extract_bag(path, output_path=args.output_path)
             if not args.quiet:
                 sys.stdout.write('\n')
             return result
```

### Comparing `bdbag-1.7.2/bdbag/bdbag_config.py` & `bdbag-1.7.3/bdbag/bdbag_config.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/bdbag_ro.py` & `bdbag-1.7.3/bdbag/bdbag_ro.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     if not media_type:
         media_type = guess_mime_type(path)
 
     uri = source_url = escape_uri(source_url)
     retrieved_from = None
 
     if local_path:
-        uri = escape_uri(ensure_payload_path_prefix(local_path), encode_whitespace=False)
+        uri = escape_uri(ensure_payload_path_prefix(local_path), encode_whitespace=False, encode_other=True)
         if source_url:
             retrieved_from = dict(retrievedFrom=source_url)
 
     add_provenance(
         add_aggregate(manifest,
                       uri=uri,
                       mediatype=media_type,
```

### Comparing `bdbag-1.7.2/bdbag/bdbag_utils.py` & `bdbag-1.7.3/bdbag/bdbag_utils.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/bdbagit.py` & `bdbag-1.7.3/bdbag/bdbagit.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     LOGGER.info('Writing fetch.txt')
 
     with open_text_file(fetch_file_path, 'w') as fetch_file:
         for filename in sorted(remote_entries.keys()):
             fetch_file.write("%s\t%s\t%s\n" %
                              (escape_uri(remote_entries[filename]['url']),
                               remote_entries[filename]['length'],
-                              escape_uri(_denormalize_filename(filename), encode_whitespace=False)))
+                              escape_uri(_denormalize_filename(filename), encode_whitespace=False, encode_other=True)))
 
 
 def _find_tag_files(bag_dir):
     for dir in os.listdir(bag_dir):
         if dir != 'data':
             if os.path.isfile(dir) and not dir.startswith('tagmanifest-'):
                 yield dir
```

### Comparing `bdbag-1.7.2/bdbag/bdbagit_profile.py` & `bdbag-1.7.3/bdbag/bdbagit_profile.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/__init__.py` & `bdbag-1.7.3/bdbag/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/auth/cookies.py` & `bdbag-1.7.3/bdbag/fetch/auth/cookies.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/auth/keychain.py` & `bdbag-1.7.3/bdbag/fetch/auth/keychain.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/fetcher.py` & `bdbag-1.7.3/bdbag/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/resolvers/__init__.py` & `bdbag-1.7.3/bdbag/fetch/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/resolvers/ark_resolver.py` & `bdbag-1.7.3/bdbag/fetch/resolvers/ark_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/resolvers/base_resolver.py` & `bdbag-1.7.3/bdbag/fetch/resolvers/base_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/resolvers/dataguid_resolver.py` & `bdbag-1.7.3/bdbag/fetch/resolvers/dataguid_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/resolvers/doi_resolver.py` & `bdbag-1.7.3/bdbag/fetch/resolvers/doi_resolver.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/__init__.py` & `bdbag-1.7.3/bdbag/fetch/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/base_transport.py` & `bdbag-1.7.3/bdbag/fetch/transports/base_transport.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_boto3.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_boto3.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_ftp.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_ftp.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_gcs.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_gcs.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_globus.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_globus.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_http.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_http.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag/fetch/transports/fetch_tag.py` & `bdbag-1.7.3/bdbag/fetch/transports/fetch_tag.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/bdbag.egg-info/PKG-INFO` & `bdbag-1.7.3/bdbag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdbag
-Version: 1.7.2
+Version: 1.7.3
 Summary: Big Data Bag Utilities
 Home-page: https://github.com/fair-research/bdbag/
 Author: Mike D'Arcy
 Maintainer: USC Information Sciences Institute, Informatics Systems Research Division
 Maintainer-email: isrd-support@isi.edu
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
@@ -92,15 +92,15 @@
 ["I'll take that to go: Big data bags and minimal identifiers for exchange of large, complex datasets"](https://zenodo.org/record/820878) explains the motivation for BDBags and the related Minid construct, provides details on design and implementation, and gives examples of use. 
 
 ["Reproducible big data science: A case study in continuous FAIRness"](https://www.biorxiv.org/content/early/2018/02/27/268755) presents a data analysis use case in which BDBags and Minids are used to capture a transcription factor binding site analysis.
 
 ### Python Dependencies
 
 *  Python 2.7 is the minimum Python version required. Please note however that Python 2.7 is officially end-of-life and ongoing compatibility between Python 2.7 and `bdbag` (and its dependencies) is not officially supported and cannot be guaranteed.
-*  Python 3, versions 3.7 through 3.11 are the current officially supported releases.
+*  Python 3, versions 3.8 through 3.12 are the current officially supported releases.
 
 ### Installation
 The latest `bdbag` release is available on PyPi and can be installed using `pip`:
 
 ```sh
 pip install bdbag
 ```
```

### Comparing `bdbag-1.7.2/bdbag.egg-info/SOURCES.txt` & `bdbag-1.7.3/bdbag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/doc/api.md` & `bdbag-1.7.3/doc/api.md`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,16 @@
          prune_manifests=False,
          metadata=None,
          metadata_file=None,
          remote_file_manifest=None,
          config_file=None,
          ro_metadata=None,
          ro_metadata_file=None,
-         idempotent=None)
+         idempotent=None,
+         strict=False)
 ```
 Creates or updates the bag denoted by the `bag_path` argument.
 
 ##### Parameters
 | Param                | Type      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 |----------------------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | bag_path             | `string`  | A normalized, absolute path to a bag directory.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
@@ -204,14 +205,15 @@
 | metadata             | `dict`    | A dictionary of key-value pairs that will be written directly to the bag's 'bag-info.txt' file.                                                                                                                                                                                                                                                                                                                                                                                                         |
 | metadata_file        | `string`  | A JSON file representation of metadata that will be written directly to the bag's 'bag-info.txt' file. The format of this metadata is described [here](./config.md#metadata).                                                                                                                                                                                                                                                                                                                           |
 | remote_file_manifest | `string`  | A path to a JSON file representation of remote file entries that will be used to add remote files to the bag file manifest(s) and used to create the bag's `fetch.txt`. The format of this file is described [here](./config.md/#remote-file-manifest).                                                                                                                                                                                                                                                 |
 | config_file          | `string`  | A JSON file representation of configuration data that is used during bag creation and update. The format of this file is described [here](./config.md#bdbag.json).                                                                                                                                                                                                                                                                                                                                      |
 | ro_metadata          | `dict`    | A dictionary that will be used to serialize data into one or more JSON files into the bag's `metadata` directory. The format of this metadata is described [here](./config.md#ro_metadata).                                                                                                                                                                                                                                                                                                             |
 | ro_metadata_file     | `string`  | A path to a JSON file representation of RO metadata that will be used to serialize data into one or more JSON files into the bag's `metadata` directory. The format of this metadata is described [here](./config.md#ro_metadata).                                                                                                                                                                                                                                                                      |
 | idempotent           | `boolean` | If `True`, date and time specific metadata such as `Bagging-Date` and `Bagging-Time` will be _removed_ (if present) from `bag-info.txt`. This value defaults to `False` if not passed via argument. However, a global override default value of `True` can be enabled in the [config file](./config.md). NOTE: use of `ro_metadata` and `ro_metadata_file` in conjunction with `idempotent` is not recommended at this time due to the generated RO Metadata not being compatible with bag idempotency. |
+| strict               | `boolean` | If `True`, automatically validate a newly created or updated bag for structural validity and fail if the resultant bag is invalid. This can be used to ensure that a bag is not persisted without payload file manifests. Furthermore, if this argument is `True` and a created output bag is not structurally valid, the bag will subsequently be reverted back to a normal directory. An updated bag will not be reverted. In either case, a BagValidationError exception is thrown.                  |
 
 **Returns**: `bag` - An instantiated [bagit-python](https://github.com/LibraryOfCongress/bagit-python/blob/master/bagit.py) `bag` compatible class object.
 
 -----
 <a name="materialize"></a>
 ## materialize
 ```python
```

### Comparing `bdbag-1.7.2/doc/cli.md` & `bdbag-1.7.3/doc/cli.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 The only mandatory argument is a valid path to a local bag directory, a local bag archive file, or a URL/URI resolving to a remote bag archive file. All other arguments are optional.
 
 ### Basic arguments:
 ```
 usage: bdbag
 [--version]
 [--update]
+[--strict]
 [--revert]
 [--archiver {zip,tar,tgz,bz2,xz}]
 [--idempotent]
 [--checksum {md5,sha1,sha256,sha512,all}]
 [--skip-manifests]
 [--prune-manifests]
 [--materialize]
@@ -81,14 +82,21 @@
 operating on bag _archive_ files) can be configured to write such output to the specified `output-path`.
 
 ----
 #### `--update`
 Update an existing bag dir, recalculating tag-manifest checksums and regenerating manifests and fetch.txt if necessary.
 
 ----
+#### `--strict`
+Automatically validate a newly created or updated bag for structural validity and fail if the resultant bag is invalid. 
+This can be used to ensure that a bag is not persisted without payload file manifests. If this flag is set and a 
+created output bag is not structurally valid, the bag will subsequently be reverted back to a normal directory. 
+An updated bag will _not_ be reverted. In either case, an error is returned.
+
+----
 #### `--revert`
 Revert an existing bag directory back to a normal directory, deleting all bag metadata files. Payload files in the `data` directory will be moved back to the directory root, and the `data` directory will be deleted.
 
 ----
 #### `--archiver {zip,tar,tgz,bz2,xz}`
 Archive a bag using the specified format. Note that `xz` (LZMA) compression is not available on Python versions lower than `3.3`.
 
@@ -248,14 +256,15 @@
 This following table enumerates the various arguments and compatibility modes.
 
 |                 Argument |                           Context                           | Description                                                                                                                                                                                                                                   |
 |-------------------------:|:-----------------------------------------------------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 |                 `<path>` |                             all                             | Required argument. When no other options are specified, creates a bag from the target path if that path is a directory and not already a bag; otherwise, if the path represents an archive file in a supported format, the file is extracted. |
 |          `--output-path` |                      bag archive only                       | For a certain set of functions that may extract bag archive files (currently only `materialize`, `extract`, or `validate`), this argument dictates the directory where the output results of the extraction should be placed.                 |
 |               `--update` |                        bag dir only                         | An existing bag archive cannot be updated in-place. The bag must first be extracted and then updated.                                                                                                                                         |
+|               `--strict` |     regular dir or bag dir only, create or update only      | Strict checking is valid only when creating a new bag from a regular directory or updating an existing bag directory.                                                                                                                         |
 |               `--revert` |                        bag dir only                         | Only a bag directory may be reverted to a non-bag directory.                                                                                                                                                                                  |
 |             `--archiver` |                        bag dir only                         | A bag archive cannot be created from an existing bag archive.                                                                                                                                                                                 |
 |             `--checksum` |                        bag dir only                         | A checksum manifest cannot be added to an existing bag archive. The bag must be extracted, updated, and re-archived.                                                                                                                          |
 |      `--prune-manifests` |                  bag dir only, update only                  | Unused manifests may only be pruned from an existing bag during an update operation.                                                                                                                                                          |
 |       `--skip-manifests` |                  bag dir only, update only                  | Skipping the recalculation of payload checksums may only be performed on an existing bag during an update operation.                                                                                                                          |
 |          `--materialize` |       bag archive, bag dir, or actionable bag URL/URI       | The `--materialze` argument cannot be combined with any other arguments except for `--config-file`, `--keychain-file`, and `--fetch-filter`.                                                                                                  |
 |        `--resolve-fetch` |              bag dir only, no create or update              | The resolution (download) of files listed in fetch.txt cannot be executed when creating or updating a bag.                                                                                                                                    |
```

### Comparing `bdbag-1.7.2/doc/config.md` & `bdbag-1.7.3/doc/config.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/doc/utils.md` & `bdbag-1.7.3/doc/utils.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/bagofbags/README.md` & `bdbag-1.7.3/examples/bagofbags/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/bagofbags/bagofbags.py` & `bdbag-1.7.3/examples/bagofbags/bagofbags.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/bagofbags/images/MetaBags.png` & `bdbag-1.7.3/examples/bagofbags/images/MetaBags.png`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/bagofbags/images/MetaBags.pptx` & `bdbag-1.7.3/examples/bagofbags/images/MetaBags.pptx`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/metamanifests/README.md` & `bdbag-1.7.3/examples/metamanifests/README.md`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/metamanifests/samples/sample1/remote-files.json` & `bdbag-1.7.3/examples/metamanifests/samples/sample1/remote-files.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/examples/metamanifests/samples/sample1/ro_metadata.json` & `bdbag-1.7.3/examples/metamanifests/samples/sample1/ro_metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/profiles/bdbag-profile.json` & `bdbag-1.7.3/profiles/bdbag-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/profiles/bdbag-ro-profile.json` & `bdbag-1.7.3/profiles/bdbag-ro-profile.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/setup.cfg` & `bdbag-1.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/setup.py` & `bdbag-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag-fetch-http.zip` & `bdbag-1.7.3/test/test-data/test-archives/test-bag-fetch-http.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag-multi-parent.tgz` & `bdbag-1.7.3/test/test-data/test-archives/test-bag-multi-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag-multi-parent.zip` & `bdbag-1.7.3/test/test-data/test-archives/test-bag-multi-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag-no-parent.tgz` & `bdbag-1.7.3/test/test-data/test-archives/test-bag-no-parent.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag-no-parent.zip` & `bdbag-1.7.3/test/test-data/test-archives/test-bag-no-parent.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag.bz2` & `bdbag-1.7.3/test/test-data/test-archives/test-bag.bz2`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag.tar` & `bdbag-1.7.3/test/test-data/test-archives/test-bag.tar`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag.tgz` & `bdbag-1.7.3/test/test-data/test-archives/test-bag.tgz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag.xz` & `bdbag-1.7.3/test/test-data/test-archives/test-bag.xz`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-archives/test-bag.zip` & `bdbag-1.7.3/test/test-data/test-archives/test-bag.zip`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-empty-dirs/metadata/manifest.json` & `bdbag-1.7.3/test/test-data/test-bag-empty-dirs/metadata/manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt` & `bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-empty-dirs/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt` & `bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-incomplete/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt` & `bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha256.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-invalid-structure-fetch/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-invalid-structure-filesystem/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-invalid-structure-manifest/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-no-data/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-no-data/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bag-profile/tagmanifest-sha512.txt` & `bdbag-1.7.3/test/test-data/test-bag-profile/tagmanifest-sha512.txt`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg` & `bdbag-1.7.3/test/test-data/test-bdbagit/loc/2478433644_2839c5e8b8_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg` & `bdbag-1.7.3/test/test-data/test-bdbagit/loc/3314493806_6f1db86d66_o_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg` & `bdbag-1.7.3/test/test-data/test-bdbagit/si/2584174182_ffd5c24905_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg` & `bdbag-1.7.3/test/test-data/test-bdbagit/si/4011399822_65987a4806_b_d.jpg`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-10.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-10.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-11.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-11.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-12.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-12.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-3.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-3.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-4.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-4.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-5.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-5.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-6.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-6.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-7.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-7.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-8.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-config-9.json` & `bdbag-1.7.3/test/test-data/test-config/test-config-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-2.json` & `bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-2.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-encoding.json` & `bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-encoding.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714285%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test "*

 * *      "fetch%25http®.txt'}",*

 * * '1': "{'url': "*

 * *      "'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test\\tfetch%25http®.txt'}",*

 * * '2': "{'url': "*

 * *      "'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test%20fetch%25http®.txt'}"}*

```diff
@@ -2,28 +2,28 @@
     {
         "filename": "test fetch http\u00ae.txt",
         "length": 201,
         "md5": "f3ad851f4213d41ce9690542010bffa0",
         "sha1": "93656178967a53104eb30324d4e028a7a30eecb4",
         "sha256": "861236468065b9b0ae369ae99bbc7df08b4db919438e288d923efc0e77775bbf",
         "sha512": "1bdbb4fc33dbea55ee0e5473062cbd003221c571c6110e2b3d2ebe5288a95a74ccd60fbbbcbd42fcfa4cd320b980ca27d537e6d29e60f73822e301a7ba6c1bfa",
-        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test fetch%http\u00ae.txt"
+        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test fetch%25http\u00ae.txt"
     },
     {
         "filename": "test\nfetch\nhttp\u00ae.txt",
         "length": 201,
         "md5": "f3ad851f4213d41ce9690542010bffa0",
         "sha1": "93656178967a53104eb30324d4e028a7a30eecb4",
         "sha256": "861236468065b9b0ae369ae99bbc7df08b4db919438e288d923efc0e77775bbf",
         "sha512": "1bdbb4fc33dbea55ee0e5473062cbd003221c571c6110e2b3d2ebe5288a95a74ccd60fbbbcbd42fcfa4cd320b980ca27d537e6d29e60f73822e301a7ba6c1bfa",
-        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test fetch%http\u00ae.txt"
+        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test\tfetch%25http\u00ae.txt"
     },
     {
         "filename": "test%fetch http\u00ae\r\n.txt",
         "length": 201,
         "md5": "f3ad851f4213d41ce9690542010bffa0",
         "sha1": "93656178967a53104eb30324d4e028a7a30eecb4",
         "sha256": "861236468065b9b0ae369ae99bbc7df08b4db919438e288d923efc0e77775bbf",
         "sha512": "1bdbb4fc33dbea55ee0e5473062cbd003221c571c6110e2b3d2ebe5288a95a74ccd60fbbbcbd42fcfa4cd320b980ca27d537e6d29e60f73822e301a7ba6c1bfa",
-        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test fetch%http\u00ae.txt"
+        "url": "https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/test%20fetch%25http\u00ae.txt"
     }
 ]
```

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json` & `bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest-mixed-checksums.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-fetch-manifest.json` & `bdbag-1.7.3/test/test-data/test-config/test-fetch-manifest.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-keychain-8.json` & `bdbag-1.7.3/test/test-data/test-config/test-keychain-8.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-keychain-9.json` & `bdbag-1.7.3/test/test-data/test-config/test-keychain-9.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test-data/test-config/test-ro-metadata.json` & `bdbag-1.7.3/test/test-data/test-config/test-ro-metadata.json`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test_api.py` & `bdbag-1.7.3/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,37 @@
         logger.info(self.getTestHeader('create bag'))
         try:
             bag = bdb.make_bag(self.test_data_dir)
             self.assertIsInstance(bag, bdbagit.BDBag)
         except Exception as e:
             self.fail(get_typed_exception(e))
 
+    def test_create_bag_strict(self):
+        logger.info(self.getTestHeader('create bag strict'))
+        try:
+            os.mkdir(self.test_data_dir_empty)
+            with self.assertRaises(bdbagit.BagValidationError) as ar:
+                bdb.make_bag(self.test_data_dir_empty, strict=True)
+                self.assertFalse(bdb.is_bag(self.test_data_dir_empty))
+            logger.error(get_typed_exception(ar.exception))
+        except Exception as e:
+            self.fail(get_typed_exception(e))
+
+    def test_update_bag_strict(self):
+        logger.info(self.getTestHeader('update bag strict'))
+        try:
+            os.mkdir(self.test_data_dir_empty)
+            bdb.make_bag(self.test_data_dir_empty)
+            with self.assertRaises(bdbagit.BagValidationError) as ar:
+                bdb.make_bag(self.test_data_dir_empty, update=True, strict=True)
+                self.assertTrue(bdb.is_bag(self.test_data_dir_empty))
+            logger.error(get_typed_exception(ar.exception))
+        except Exception as e:
+            self.fail(get_typed_exception(e))
+
     def test_create_bag_idempotent(self):
         logger.info(self.getTestHeader('create bag idempotent'))
         try:
             bag_metadata = dict()
             bag_metadata['Bagging-Date'] = date.strftime(date.today(), "%Y-%m-%d")
             bag_metadata['Bagging-Time'] = datetime.strftime(datetime.now(tz=get_localzone()), "%H:%M:%S %Z")
             bag = bdb.make_bag(self.test_data_dir, metadata=bag_metadata, idempotent=True)
```

### Comparing `bdbag-1.7.2/test/test_bdbagit.py` & `bdbag-1.7.3/test/test_bdbagit.py`

 * *Files identical despite different names*

### Comparing `bdbag-1.7.2/test/test_cli.py` & `bdbag-1.7.3/test/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import os
 import sys
 import atexit
 import unittest
 import subprocess
 from os.path import join as ospj
 from test.test_common import BaseTest
 
@@ -54,14 +55,27 @@
         self._test_successful_invocation(args)
 
     def test_create(self):
         args = ARGS + [self.test_data_dir]
         logfile.writelines(self.getTestHeader('create bag', args))
         self._test_successful_invocation(args)
 
+    def test_create_strict(self):
+        os.mkdir(self.test_data_dir_empty)
+        args = ARGS + [self.test_data_dir_empty, "--strict"]
+        logfile.writelines(self.getTestHeader('create bag strict', args))
+        output = ''
+        try:
+            output = subprocess.check_output(args, stderr=subprocess.STDOUT, universal_newlines=True)
+        except subprocess.CalledProcessError as e:
+            output = e.output
+        finally:
+            logfile.writelines(output)
+            self.assertExpectedMessages(["Exception: [BagValidationError] No manifest files found"], output)
+
     def test_create_idempotent(self):
         args = ARGS + [self.test_data_dir, "--idempotent"]
         logfile.writelines(self.getTestHeader('create bag idempotent', args))
         self._test_successful_invocation(args)
 
     def test_create_with_metadata(self):
         args = ARGS + [self.test_data_dir,
```

### Comparing `bdbag-1.7.2/test/test_common.py` & `bdbag-1.7.3/test/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             self.assertRaisesRegex = self.assertRaisesRegexp
 
         self.tmpdir = tempfile.mkdtemp(prefix="bdbag_test_")
         shutil.copytree(os.path.abspath(os.path.join('test', 'test-data')), os.path.join(self.tmpdir, 'test-data'))
 
         self.test_data_dir = os.path.join(self.tmpdir, 'test-data', 'test-dir')
         self.assertTrue(os.path.isdir(self.test_data_dir))
+        self.test_data_dir_empty = os.path.join(self.tmpdir, 'test-data', 'test-dir-empty')
         self.test_archive_dir = os.path.join(self.tmpdir, 'test-data', 'test-archives')
         self.assertTrue(os.path.isdir(self.test_archive_dir))
         self.test_config_dir = os.path.join(self.tmpdir, 'test-data', 'test-config')
         self.assertTrue(os.path.isdir(self.test_config_dir))
         self.test_http_dir = os.path.join(self.tmpdir, 'test-data', 'test-http')
         self.assertTrue(os.path.isdir(self.test_http_dir))
```

### Comparing `bdbag-1.7.2/test/test_remote.py` & `bdbag-1.7.3/test/test_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             self.assertExpectedMessages(['Generating remote file references from', filename], output)
             fetch_file = ospj(bag_dir, 'fetch.txt')
             self.assertTrue(ospif(fetch_file))
             with io.open(fetch_file, encoding='utf-8') as ff:
                 fetch_txt = ff.read()
             self.assertIn(
                 u'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/'
-                u'test%20fetch%25http®.txt\t201\tdata/test%0Afetch%0Ahttp®.txt', fetch_txt)
+                u'test%09fetch%25http®.txt\t201\tdata/test%0Afetch%0Ahttp®.txt', fetch_txt)
             self.assertIn(
                 u'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/'
                 u'test%20fetch%25http®.txt\t201\tdata/test fetch http®.txt', fetch_txt)
             self.assertIn(
                 u'https://raw.githubusercontent.com/fair-research/bdbag/master/test/test-data/test-http-encoded/'
                 u'test%20fetch%25http®.txt\t201\tdata/test%25fetch http®%0D%0A.txt', fetch_txt)
             bdb.validate_bag_structure(bag_dir, True)
```

