# Comparing `tmp/tuf-4.0.0.tar.gz` & `tmp/tuf-5.0.0.tar.gz`

## Comparing `tuf-4.0.0.tar` & `tuf-5.0.0.tar`

### file list

```diff
@@ -1,182 +1,175 @@
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 tuf-4.0.0/tox.ini
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/1.0.0-ANNOUNCEMENT.md
--rw-r--r--   0        0        0    31474 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/CONTRIBUTING.rst
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/GOVERNANCE.md
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/INSTALLATION.rst
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/MAINTAINERS.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/RELEASE.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/SECURITY.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_config.yml
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/conf.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/index.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/index.rst
--rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/repository-library-design-ownership.jpg
--rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/repository-library-design-usage.jpg
--rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/repository-library-design.md
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/tuf-horizontal-white.png
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/tuf-icon-200.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/tuf-icon-32.png
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_posts/2022-02-21-release-1-0-0.md
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_posts/2022-05-04-ngclient-design.md
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_posts/2022-06-15-testing-ngclient.md
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0001-python-version-3-6-plus.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0005-use-google-python-style-guide.md
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0008-accept-unrecognised-fields.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0009-what-is-a-reference-implementation.md
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/0010-repository-library-design.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/index.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/adr/template.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/api-reference.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.metadata.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.root.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.snapshot.rst
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.supporting.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.targets.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.metadata.timestamp.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.api.serialization.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.ngclient.config.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.ngclient.fetcher.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.ngclient.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-4.0.0/docs/api/tuf.ngclient.updater.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/client/README.md
--rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/client/client
--rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/manual_repo/basic_repo.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/manual_repo/hashed_bin_delegation.py
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/manual_repo/succinct_hash_bin_delegations.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/repository/README.md
--rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/repository/_simplerepo.py
--rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/repository/repo
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/uploader/README.md
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/uploader/_localrepo.py
--rwxr-xr-x   0        0        0     4262 2020-02-02 00:00:00.000000 tuf-4.0.0/examples/uploader/uploader
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/build.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/dev.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/docs.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/lint.txt
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/main.txt
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/pinned.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 tuf-4.0.0/requirements/test.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/.coveragerc
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/__init__.py
--rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/aggregate_tests.py
--rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_simulator.py
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/simple_server.py
--rwxr-xr-x   0        0        0    50715 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_api.py
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_examples.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_fetcher_ng.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_metadata_eq_.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_metadata_generation.py
--rw-r--r--   0        0        0    33619 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_metadata_serialization.py
--rw-r--r--   0        0        0    22922 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_trusted_metadata_set.py
--rw-r--r--   0        0        0     9932 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_consistent_snapshot.py
--rw-r--r--   0        0        0    22631 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_delegation_graphs.py
--rw-r--r--   0        0        0     8486 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_fetch_target.py
--rw-r--r--   0        0        0    11958 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_key_rotations.py
--rw-r--r--   0        0        0    13078 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_ng.py
--rw-r--r--   0        0        0    31495 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_top_level_update.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_updater_validation.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/test_utils.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/__init__.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/generate_md.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/map.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/1.a.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1...json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1.ö.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/timestamp.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/delegation_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/delegation_key.pub
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key2
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key2.pub
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key3
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/root_key3.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/snapshot_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/snapshot_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/targets_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/targets_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/timestamp_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/keystore/timestamp_key.pub
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/role1.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/metadata/timestamp.json
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/targets/file1.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/targets/file2.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-4.0.0/tests/repository_data/repository/targets/file3.txt
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/__init__.py
--rw-r--r--   0        0        0    64454 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/_payload.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/dsse.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/exceptions.py
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/metadata.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/serialization/__init__.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/api/serialization/json.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/README.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/__init__.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/config.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/fetcher.py
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/updater.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/_internal/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/_internal/requests_fetcher.py
--rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/ngclient/_internal/trusted_metadata_set.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/repository/__init__.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 tuf-4.0.0/tuf/repository/_repository.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-4.0.0/.gitignore
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-4.0.0/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-4.0.0/LICENSE-MIT
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 tuf-4.0.0/README.md
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 tuf-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 tuf-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 tuf-5.0.0/tox.ini
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/1.0.0-ANNOUNCEMENT.md
+-rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/GOVERNANCE.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/INSTALLATION.rst
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/MAINTAINERS.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/RELEASE.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/SECURITY.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_config.yml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/conf.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/index.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/index.rst
+-rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/repository-library-design-ownership.jpg
+-rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/repository-library-design-usage.jpg
+-rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/repository-library-design.md
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/tuf-horizontal-white.png
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/tuf-icon-200.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/tuf-icon-32.png
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_posts/2022-02-21-release-1-0-0.md
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_posts/2022-05-04-ngclient-design.md
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_posts/2022-06-15-testing-ngclient.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0001-python-version-3-6-plus.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0005-use-google-python-style-guide.md
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0008-accept-unrecognised-fields.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0009-what-is-a-reference-implementation.md
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/0010-repository-library-design.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/index.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/adr/template.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/api-reference.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.metadata.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.root.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.snapshot.rst
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.supporting.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.targets.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.metadata.timestamp.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.api.serialization.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.ngclient.config.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.ngclient.fetcher.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.ngclient.rst
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-5.0.0/docs/api/tuf.ngclient.updater.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/client/README.md
+-rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/client/client
+-rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/manual_repo/basic_repo.py
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/manual_repo/hashed_bin_delegation.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/manual_repo/succinct_hash_bin_delegations.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/repository/README.md
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/repository/_simplerepo.py
+-rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/repository/repo
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/uploader/README.md
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/uploader/_localrepo.py
+-rwxr-xr-x   0        0        0     4262 2020-02-02 00:00:00.000000 tuf-5.0.0/examples/uploader/uploader
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/build.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/dev.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/docs.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/lint.txt
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/main.txt
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/pinned.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 tuf-5.0.0/requirements/test.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/.coveragerc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/aggregate_tests.py
+-rw-r--r--   0        0        0    15245 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_simulator.py
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/simple_server.py
+-rw-r--r--   0        0        0    49909 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_api.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_examples.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_fetcher_ng.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_metadata_eq_.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_metadata_generation.py
+-rw-r--r--   0        0        0    33619 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_metadata_serialization.py
+-rw-r--r--   0        0        0    22748 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_trusted_metadata_set.py
+-rw-r--r--   0        0        0     9909 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_consistent_snapshot.py
+-rw-r--r--   0        0        0    22608 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_delegation_graphs.py
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_fetch_target.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_key_rotations.py
+-rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_ng.py
+-rw-r--r--   0        0        0    31464 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_top_level_update.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_updater_validation.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0    12376 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/__init__.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/generate_md.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/map.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/1.a.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1...json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1.ö.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/timestamp.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/delegation_key
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/root_key
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/root_key2
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/root_key3
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/snapshot_key
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/targets_key
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/keystore/timestamp_key
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/role1.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/metadata/timestamp.json
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/targets/file1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/targets/file2.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-5.0.0/tests/repository_data/repository/targets/file3.txt
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/__init__.py
+-rw-r--r--   0        0        0    64472 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/_payload.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/dsse.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/exceptions.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/metadata.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/serialization/__init__.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/api/serialization/json.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/config.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/fetcher.py
+-rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/updater.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/_internal/__init__.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/_internal/requests_fetcher.py
+-rw-r--r--   0        0        0    20107 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/ngclient/_internal/trusted_metadata_set.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/repository/__init__.py
+-rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 tuf-5.0.0/tuf/repository/_repository.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-5.0.0/.gitignore
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-5.0.0/LICENSE
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-5.0.0/LICENSE-MIT
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 tuf-5.0.0/README.md
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 tuf-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 tuf-5.0.0/PKG-INFO
```

### Comparing `tuf-4.0.0/tox.ini` & `tuf-5.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/1.0.0-ANNOUNCEMENT.md` & `tuf-5.0.0/docs/1.0.0-ANNOUNCEMENT.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/CHANGELOG.md` & `tuf-5.0.0/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## v5.0.0
+
+This release, most notably, marks stable securesystemslib v1.0.0 as minimum
+requirement. The update causes a minor break in the new DSSE API (see below)
+and affects users who also directly depend on securesystemslib. See the [securesystemslib release
+notes](https://github.com/secure-systems-lab/securesystemslib/blob/main/CHANGELOG.md#securesystemslib-v100)
+and the updated python-tuf `examples` (#2617) for details. ngclient API remains
+backwards-compatible.
+
+### Changed
+* DSSE API: change `SimpleEnvelope.signatures` type to `dict`, remove
+  `SimpleEnvelope.signatures_dict` (#2617)
+* ngclient: support app-specific user-agents (#2612)
+* Various build, test and lint improvements
+
+
 ## v4.0.0
 
 This release is a small API change for Metadata API users (see below).
 ngclient API is compatible but optional DSSE support has been added.
 
 ### Added
 * Added optional DSSE support to Metadata API and ngclient (#2436)
```

### Comparing `tuf-4.0.0/docs/CONTRIBUTING.rst` & `tuf-5.0.0/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/GOVERNANCE.md` & `tuf-5.0.0/docs/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/INSTALLATION.rst` & `tuf-5.0.0/docs/INSTALLATION.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/MAINTAINERS.txt` & `tuf-5.0.0/docs/MAINTAINERS.txt`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/RELEASE.md` & `tuf-5.0.0/docs/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/SECURITY.md` & `tuf-5.0.0/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/conf.py` & `tuf-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/index.rst` & `tuf-5.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/repository-library-design-ownership.jpg` & `tuf-5.0.0/docs/repository-library-design-ownership.jpg`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/repository-library-design-usage.jpg` & `tuf-5.0.0/docs/repository-library-design-usage.jpg`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/repository-library-design.md` & `tuf-5.0.0/docs/repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/tuf-horizontal-white.png` & `tuf-5.0.0/docs/tuf-horizontal-white.png`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/tuf-icon-200.png` & `tuf-5.0.0/docs/tuf-icon-200.png`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/tuf-icon-32.png` & `tuf-5.0.0/docs/tuf-icon-32.png`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/_posts/2022-02-21-release-1-0-0.md` & `tuf-5.0.0/docs/_posts/2022-02-21-release-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/_posts/2022-05-04-ngclient-design.md` & `tuf-5.0.0/docs/_posts/2022-05-04-ngclient-design.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/_posts/2022-06-15-testing-ngclient.md` & `tuf-5.0.0/docs/_posts/2022-06-15-testing-ngclient.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md` & `tuf-5.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md` & `tuf-5.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md` & `tuf-5.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0001-python-version-3-6-plus.md` & `tuf-5.0.0/docs/adr/0001-python-version-3-6-plus.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md` & `tuf-5.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md` & `tuf-5.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md` & `tuf-5.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0005-use-google-python-style-guide.md` & `tuf-5.0.0/docs/adr/0005-use-google-python-style-guide.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md` & `tuf-5.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0008-accept-unrecognised-fields.md` & `tuf-5.0.0/docs/adr/0008-accept-unrecognised-fields.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0009-what-is-a-reference-implementation.md` & `tuf-5.0.0/docs/adr/0009-what-is-a-reference-implementation.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/0010-repository-library-design.md` & `tuf-5.0.0/docs/adr/0010-repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/index.md` & `tuf-5.0.0/docs/adr/index.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/adr/template.md` & `tuf-5.0.0/docs/adr/template.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/api/api-reference.rst` & `tuf-5.0.0/docs/api/api-reference.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/api/tuf.api.metadata.supporting.rst` & `tuf-5.0.0/docs/api/tuf.api.metadata.supporting.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/docs/api/tuf.ngclient.rst` & `tuf-5.0.0/docs/api/tuf.ngclient.rst`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/client/README.md` & `tuf-5.0.0/examples/client/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/client/client` & `tuf-5.0.0/examples/client/client`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/manual_repo/basic_repo.py` & `tuf-5.0.0/examples/manual_repo/basic_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 
 """
 
 import os
 import tempfile
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from typing import Any, Dict
+from typing import Dict
 
-from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner, Signer
 
 from tuf.api.metadata import (
     SPECIFICATION_VERSION,
     DelegatedRole,
     Delegations,
     Metadata,
     MetaFile,
@@ -85,15 +84,15 @@
 # keys (root, delegating targets) may have longer expiration intervals.
 
 SPEC_VERSION = ".".join(SPECIFICATION_VERSION)
 
 # Define containers for role objects and cryptographic keys created below. This
 # allows us to sign and write metadata in a batch more easily.
 roles: Dict[str, Metadata] = {}
-keys: Dict[str, Dict[str, Any]] = {}
+signers: Dict[str, Signer] = {}
 
 
 # Targets (integrity)
 # -------------------
 # The targets role guarantees integrity for the files that TUF aims to protect,
 # i.e. target files. It does so by listing the relevant target files, along
 # with their hash and length.
@@ -153,45 +152,39 @@
 roles["root"] = Metadata(Root(expires=_in(365)))
 
 # For this example, we generate one 'ed25519' key pair for each top-level role
 # using python-tuf's in-house crypto library.
 # See https://github.com/secure-systems-lab/securesystemslib for more details
 # about key handling, and don't forget to password-encrypt your private keys!
 for name in ["targets", "snapshot", "timestamp", "root"]:
-    keys[name] = generate_ed25519_key()
-    roles["root"].signed.add_key(
-        SSlibKey.from_securesystemslib_key(keys[name]), name
-    )
+    signers[name] = CryptoSigner.generate_ecdsa()
+    roles["root"].signed.add_key(signers[name].public_key, name)
 
 # NOTE: We only need the public part to populate root, so it is possible to use
 # out-of-band mechanisms to generate key pairs and only expose the public part
 # to whoever maintains the root role. As a matter of fact, the very purpose of
 # signature thresholds is to avoid having private keys all in one place.
 
 # Signature thresholds
 # --------------------
 # Given the importance of the root role, it is highly recommended to require a
 # threshold of multiple keys to sign root metadata. For this example we
 # generate another root key (you can pretend it's out-of-band) and increase the
 # required signature threshold.
-another_root_key = generate_ed25519_key()
-roles["root"].signed.add_key(
-    SSlibKey.from_securesystemslib_key(another_root_key), "root"
-)
+another_root_signer = CryptoSigner.generate_ecdsa()
+roles["root"].signed.add_key(another_root_signer.public_key, "root")
 roles["root"].signed.roles["root"].threshold = 2
 
 
 # Sign top-level metadata (in-band)
 # =================================
 # In this example we have access to all top-level signing keys, so we can use
 # them to create and add a signature for each role metadata.
 for name in ["targets", "snapshot", "timestamp", "root"]:
-    key = keys[roles[name].signed.type]
-    signer = SSlibSigner(key)
-    roles[name].sign(signer)
+    roles[name].sign(signers[name])
 
 
 # Persist metadata (consistent snapshot)
 # ======================================
 # It is time to publish the first set of metadata for a client to safely
 # download the target file that we have registered for this example repository.
 #
@@ -223,31 +216,31 @@
 # As mentioned above, using signature thresholds usually entails that not all
 # signing keys for a given role are in the same place. Let's briefly pretend
 # this is the case for the second root key we registered above, and we are now
 # on that key owner's computer. All the owner has to do is read the metadata
 # file, sign it, and write it back to the same file, and this can be repeated
 # until the threshold is satisfied.
 root_path = os.path.join(TMP_DIR, "1.root.json")
-roles["root"].from_file(root_path)
-roles["root"].sign(SSlibSigner(another_root_key), append=True)
-roles["root"].to_file(root_path, serializer=PRETTY)
+root = Metadata.from_file(root_path)
+root.sign(another_root_signer, append=True)
+root.to_file(root_path, serializer=PRETTY)
 
 
 # Targets delegation
 # ==================
 # Similar to how the root role delegates responsibilities about integrity,
 # consistency and freshness to the corresponding top-level roles, a targets
 # role may further delegate its responsibility for target files (or a subset
 # thereof) to other targets roles. This allows creation of a granular trust
 # hierarchy, and further reduces the impact of a single role compromise.
 #
 # In this example the top-level targets role trusts a new "python-scripts"
 # targets role to provide integrity for any target file that ends with ".py".
 delegatee_name = "python-scripts"
-keys[delegatee_name] = generate_ed25519_key()
+signers[delegatee_name] = CryptoSigner.generate_ecdsa()
 
 # Delegatee
 # ---------
 # Create a new targets role, akin to how we created top-level targets above, and
 # add target file info from above according to the delegatee's responsibility.
 roles[delegatee_name] = Metadata[Targets](
     signed=Targets(
@@ -267,24 +260,21 @@
 # signatures for the delegatee metadata. It also provides the corresponding
 # public key store.
 # The delegation info defined by the delegator further requires the provision
 # of a unique delegatee name and constraints about the target files the
 # delegatee is responsible for, e.g. a list of path patterns. For details about
 # all configuration parameters see
 # https://theupdateframework.github.io/specification/latest/#delegations
+delegatee_key = signers[delegatee_name].public_key
 roles["targets"].signed.delegations = Delegations(
-    keys={
-        keys[delegatee_name]["keyid"]: SSlibKey.from_securesystemslib_key(
-            keys[delegatee_name]
-        )
-    },
+    keys={delegatee_key.keyid: delegatee_key},
     roles={
         delegatee_name: DelegatedRole(
             name=delegatee_name,
-            keyids=[keys[delegatee_name]["keyid"]],
+            keyids=[delegatee_key.keyid],
             threshold=1,
             terminating=True,
             paths=["*.py"],
         ),
     },
 )
 
@@ -315,16 +305,15 @@
 roles["timestamp"].signed.snapshot_meta.version = roles[
     "snapshot"
 ].signed.version
 roles["timestamp"].signed.version += 1
 
 # Sign and write metadata for all changed roles, i.e. all but root
 for role_name in ["targets", "python-scripts", "snapshot", "timestamp"]:
-    signer = SSlibSigner(keys[role_name])
-    roles[role_name].sign(signer)
+    roles[role_name].sign(signers[role_name])
 
     # Prefix all but timestamp with version number (see consistent snapshot)
     filename = f"{role_name}.json"
     if role_name != "timestamp":
         filename = f"{roles[role_name].signed.version}.{filename}"
 
     roles[role_name].to_file(os.path.join(TMP_DIR, filename), serializer=PRETTY)
@@ -339,23 +328,21 @@
 # However, since root authorizes its own keys, it always has to be signed with
 # both the threshold of keys from the previous version and the threshold of
 # keys from the new version. This establishes a trusted line of continuity.
 #
 # In this example we will replace a root key, and sign a new version of root
 # with the threshold of old and new keys. Since one of the previous root keys
 # remains in place, it can be used to count towards the old and new threshold.
-new_root_key = generate_ed25519_key()
+new_root_signer = CryptoSigner.generate_ecdsa()
 
-roles["root"].signed.revoke_key(keys["root"]["keyid"], "root")
-roles["root"].signed.add_key(
-    SSlibKey.from_securesystemslib_key(new_root_key), "root"
-)
+roles["root"].signed.revoke_key(signers["root"].public_key.keyid, "root")
+roles["root"].signed.add_key(new_root_signer.public_key, "root")
 roles["root"].signed.version += 1
 
 roles["root"].signatures.clear()
-for key in [keys["root"], another_root_key, new_root_key]:
-    roles["root"].sign(SSlibSigner(key), append=True)
+for signer in [signers["root"], another_root_signer, new_root_signer]:
+    roles["root"].sign(signer, append=True)
 
 roles["root"].to_file(
     os.path.join(TMP_DIR, f"{roles['root'].signed.version}.root.json"),
     serializer=PRETTY,
 )
```

### Comparing `tuf-4.0.0/examples/manual_repo/hashed_bin_delegation.py` & `tuf-5.0.0/examples/manual_repo/hashed_bin_delegation.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 """
 
 import hashlib
 import os
 import tempfile
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from typing import Any, Dict, Iterator, List, Tuple
+from typing import Dict, Iterator, List, Tuple
 
-from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner, Signer
 
 from tuf.api.metadata import (
     DelegatedRole,
     Delegations,
     Metadata,
     TargetFile,
     Targets,
@@ -40,15 +39,15 @@
     """Adds 'days' to now and returns datetime object w/o microseconds."""
     return datetime.now(timezone.utc).replace(microsecond=0) + timedelta(
         days=days
     )
 
 
 roles: Dict[str, Metadata[Targets]] = {}
-keys: Dict[str, Dict[str, Any]] = {}
+signers: Dict[str, Signer] = {}
 
 # Hash bin delegation
 # ===================
 # Hash bin delegation allows to distribute a large number of target files over
 # multiple delegated targets metadata. The consequence is smaller metadata
 # files and thus a lower network overhead for repository-client communication.
 #
@@ -134,26 +133,26 @@
 # targets role (bins). Considering the high responsibility but also low
 # volatility of the bins role, it is recommended to require signature
 # thresholds and keep the keys offline in a real-world scenario.
 
 # NOTE: See "Targets delegation" and "Signature thresholds" paragraphs in
 # 'basic_repo.py' for more details
 for name in ["bin-n", "bins"]:
-    keys[name] = generate_ed25519_key()
+    signers[name] = CryptoSigner.generate_ecdsa()
 
 
 # Targets roles
 # -------------
 # NOTE: See "Targets" and "Targets delegation" paragraphs in 'basic_repo.py'
 # example for more details about the Targets object.
 
 # Create preliminary delegating targets role (bins) and add public key for
 # delegated targets (bin_n) to key store. Delegation details are update below.
 roles["bins"] = Metadata(Targets(expires=_in(365)))
-bin_n_key = SSlibKey.from_securesystemslib_key(keys["bin-n"])
+bin_n_key = signers["bin-n"].public_key
 roles["bins"].signed.delegations = Delegations(
     keys={bin_n_key.keyid: bin_n_key},
     roles={},
 )
 
 # The hash bin generator yields an ordered list of incremental hash bin names
 # (ranges), plus the hash prefixes each bin is responsible for, e.g.:
@@ -165,15 +164,15 @@
 #              f8-ff                       f8 f9 fa fb fc fd fe ff
 assert roles["bins"].signed.delegations.roles is not None
 for bin_n_name, bin_n_hash_prefixes in generate_hash_bins():
     # Update delegating targets role (bins) with delegation details for each
     # delegated targets role (bin_n).
     roles["bins"].signed.delegations.roles[bin_n_name] = DelegatedRole(
         name=bin_n_name,
-        keyids=[keys["bin-n"]["keyid"]],
+        keyids=[signers["bin-n"].public_key.keyid],
         threshold=1,
         terminating=False,
         path_hash_prefixes=bin_n_hash_prefixes,
     )
 
     # Create delegated targets roles (bin_n)
     roles[bin_n_name] = Metadata(Targets(expires=_in(7)))
@@ -206,14 +205,13 @@
 
 # NOTE: See "Persist metadata" paragraph in 'basic_repo.py' example for more
 # details about serialization formats and metadata file name conventions.
 PRETTY = JSONSerializer(compact=False)
 TMP_DIR = tempfile.mkdtemp(dir=os.getcwd())
 
 for role_name, role in roles.items():
-    key = keys["bins"] if role_name == "bins" else keys["bin-n"]
-    signer = SSlibSigner(key)
+    signer = signers["bins"] if role_name == "bins" else signers["bin-n"]
     role.sign(signer)
 
     filename = f"1.{role_name}.json"
     filepath = os.path.join(TMP_DIR, filename)
     role.to_file(filepath, serializer=PRETTY)
```

### Comparing `tuf-4.0.0/examples/manual_repo/succinct_hash_bin_delegations.py` & `tuf-5.0.0/examples/manual_repo/succinct_hash_bin_delegations.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 """
 
 import math
 import os
 import tempfile
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from typing import Dict, Tuple
+from typing import Dict
 
-from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner
 
 from tuf.api.metadata import (
     Delegations,
     Key,
     Metadata,
     SuccinctRoles,
     TargetFile,
@@ -76,23 +75,18 @@
 # ------------------
 # Succinct hash bin delegation uses the same key(s) to sign all bins. This is
 # acceptable because the primary concern of this type of delegation is to reduce
 # network overhead. For the purpose of this example only one key is required.
 THRESHOLD = 1
 
 
-def create_key() -> Tuple[Key, SSlibSigner]:
-    """Generates a new Key and Signer."""
-    sslib_key = generate_ed25519_key()
-    return SSlibKey.from_securesystemslib_key(sslib_key), SSlibSigner(sslib_key)
-
-
 # Create one signing key for all bins, and one for the delegating targets role.
-bins_key, bins_signer = create_key()
-_, targets_signer = create_key()
+bins_signer = CryptoSigner.generate_ecdsa()
+bins_key = bins_signer.public_key
+targets_signer = CryptoSigner.generate_ecdsa()
 
 # Delegating targets role
 # -----------------------
 # Akin to regular targets delegation, the delegating role ships the public keys
 # of the delegated roles. However, instead of providing individual delegation
 # information about each role, one single `SuccinctRoles` object is used to
 # provide the information for all delegated roles (bins).
```

### Comparing `tuf-4.0.0/examples/repository/README.md` & `tuf-5.0.0/examples/repository/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/repository/_simplerepo.py` & `tuf-5.0.0/examples/repository/_simplerepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import copy
 import json
 import logging
 from collections import defaultdict
 from datetime import datetime, timedelta, timezone
 from typing import Dict, List, Union
 
-from securesystemslib import keys
-from securesystemslib.signer import Key, Signer, SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner, Key, Signer
 
 from tuf.api.exceptions import RepositoryError
 from tuf.api.metadata import (
     DelegatedRole,
     Delegations,
     Metadata,
     MetaFile,
@@ -72,17 +71,17 @@
         self._targets_infos: Dict[str, MetaFile] = defaultdict(
             lambda: MetaFile(1)
         )
 
         # setup a basic repository, generate signing key per top-level role
         with self.edit_root() as root:
             for role in ["root", "timestamp", "snapshot", "targets"]:
-                key = keys.generate_ed25519_key()
-                self.signer_cache[role].append(SSlibSigner(key))
-                root.add_key(SSlibKey.from_securesystemslib_key(key), role)
+                signer = CryptoSigner.generate_ecdsa()
+                self.signer_cache[role].append(signer)
+                root.add_key(signer.public_key, role)
 
         for role in ["timestamp", "snapshot", "targets"]:
             with self.edit(role):
                 pass
 
     @property
     def targets_infos(self) -> Dict[str, MetaFile]:
```

### Comparing `tuf-4.0.0/examples/repository/repo` & `tuf-5.0.0/examples/repository/repo`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/uploader/README.md` & `tuf-5.0.0/examples/uploader/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/examples/uploader/_localrepo.py` & `tuf-5.0.0/examples/uploader/_localrepo.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import json
 import logging
 import os
 from datetime import datetime, timedelta, timezone
 from typing import Dict
 
 import requests
-from securesystemslib import keys
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner, Signer
 
 from tuf.api.exceptions import RepositoryError
 from tuf.api.metadata import Metadata, MetaFile, TargetFile, Targets
 from tuf.api.serialization.json import JSONSerializer
 from tuf.ngclient import Updater
 from tuf.repository import Repository
 
@@ -59,38 +58,43 @@
         raise NotImplementedError  # we never call timestamp
 
     def open(self, role: str) -> Metadata:
         """Return cached (or fetched) metadata"""
 
         # if there is a metadata version fetched from remote, use that
         # HACK: access Updater internals
-        if role in self.updater._trusted_set:
+        trusted_set = self.updater._trusted_set  # noqa: SLF001
+        if role in trusted_set:
             # NOTE: The original signature wrapper (Metadata) was verified and
             # discarded upon inclusion in the trusted set. It is safe to use
             # a fresh wrapper. `close` will override existing signatures anyway.
-            return Metadata(copy.deepcopy(self.updater._trusted_set[role]))
+            return Metadata(copy.deepcopy(trusted_set[role]))
 
         # otherwise we're creating metadata from scratch
         md = Metadata(Targets())
         # this makes version bumping in close() simpler
         md.signed.version = 0
         return md
 
-    def close(self, role: str, md: Metadata) -> None:
+    def close(self, role_name: str, md: Metadata) -> None:
         """Store a version of metadata. Handle version bumps, expiry, signing"""
+        targets = self.targets()
+        role = targets.get_delegated_role(role_name)
+        public_key = targets.get_key(role.keyids[0])
+        uri = f"file2:{self.key_dir}/{role_name}"
+
+        signer = Signer.from_priv_key_uri(uri, public_key)
+
         md.signed.version += 1
         md.signed.expires = datetime.now(timezone.utc) + self.expiry_period
 
-        with open(f"{self.key_dir}/{role}", encoding="utf-8") as f:
-            signer = SSlibSigner(json.loads(f.read()))
-
         md.sign(signer, append=False)
 
         # Upload using "api/role"
-        uri = f"{self.base_url}/api/role/{role}"
+        uri = f"{self.base_url}/api/role/{role_name}"
         r = requests.post(uri, data=md.to_bytes(JSONSerializer()), timeout=5)
         r.raise_for_status()
 
     def add_target(self, role: str, targetpath: str) -> bool:
         """Add target to roles metadata and submit new metadata version"""
 
         # HACK: make sure we have the roles metadata in updater._trusted_set
@@ -102,32 +106,31 @@
 
         data = bytes(targetpath, "utf-8")
         targetfile = TargetFile.from_data(targetpath, data)
         try:
             with self.edit_targets(role) as delegated:
                 delegated.targets[targetpath] = targetfile
 
-        except Exception as e:
+        except Exception as e:  # noqa: BLE001
             print(f"Failed to submit new {role} with added target: {e}")
             return False
 
         print(f"Uploaded role {role} v{delegated.version}")
         return True
 
     def add_delegation(self, role: str) -> bool:
         """Use the (unauthenticated) delegation adding API endpoint"""
-        keydict = keys.generate_ed25519_key()
-        pubkey = SSlibKey.from_securesystemslib_key(keydict)
+        signer = CryptoSigner.generate_ecdsa()
 
-        data = {pubkey.keyid: pubkey.to_dict()}
+        data = {signer.public_key.keyid: signer.public_key.to_dict()}
         url = f"{self.base_url}/api/delegation/{role}"
         r = requests.post(url, data=json.dumps(data), timeout=5)
         if r.status_code != 200:
             print(f"delegation failed with {r}")
             return False
 
         # Store the private key using rolename as filename
-        with open(f"{self.key_dir}/{role}", "w", encoding="utf-8") as f:
-            f.write(json.dumps(keydict))
+        with open(f"{self.key_dir}/{role}", "wb") as f:
+            f.write(signer.private_bytes)
 
         print(f"Uploaded new delegation, stored key in {self.key_dir}/{role}")
         return True
```

### Comparing `tuf-4.0.0/examples/uploader/uploader` & `tuf-5.0.0/examples/uploader/uploader`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/aggregate_tests.py` & `tuf-5.0.0/tests/aggregate_tests.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_simulator.py` & `tuf-5.0.0/tests/repository_simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test utility to simulate a repository
 
 RepositorySimulator provides methods to modify repository metadata so that it's
 easy to "publish" new repository versions with modified metadata, while serving
@@ -49,24 +47,22 @@
 import os
 import tempfile
 from dataclasses import dataclass, field
 from typing import Dict, Iterator, List, Optional, Tuple
 from urllib import parse
 
 import securesystemslib.hash as sslib_hash
-from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from securesystemslib.signer import CryptoSigner, Signer
 
 from tuf.api.exceptions import DownloadHTTPError
 from tuf.api.metadata import (
     SPECIFICATION_VERSION,
     TOP_LEVEL_ROLE_NAMES,
     DelegatedRole,
     Delegations,
-    Key,
     Metadata,
     MetaFile,
     Root,
     Snapshot,
     SuccinctRoles,
     TargetFile,
     Targets,
@@ -104,15 +100,15 @@
 
         # other metadata is signed on-demand (when fetched) but roots must be
         # explicitly published with publish_root() which maintains this list
         self.signed_roots: List[bytes] = []
 
         # signers are used on-demand at fetch time to sign metadata
         # keys are roles, values are dicts of {keyid: signer}
-        self.signers: Dict[str, Dict[str, SSlibSigner]] = {}
+        self.signers: Dict[str, Dict[str, Signer]] = {}
 
         # target downloads are served from this dict
         self.target_files: Dict[str, RepositoryTarget] = {}
 
         # Whether to compute hashes and length for meta in snapshot/timestamp
         self.compute_metafile_hashes_length = False
 
@@ -149,44 +145,39 @@
 
     def all_targets(self) -> Iterator[Tuple[str, Targets]]:
         """Yield role name and signed portion of targets one by one."""
         yield Targets.type, self.md_targets.signed
         for role, md in self.md_delegates.items():
             yield role, md.signed
 
-    @staticmethod
-    def create_key() -> Tuple[Key, SSlibSigner]:
-        key = generate_ed25519_key()
-        return SSlibKey.from_securesystemslib_key(key), SSlibSigner(key)
-
-    def add_signer(self, role: str, signer: SSlibSigner) -> None:
+    def add_signer(self, role: str, signer: Signer) -> None:
         if role not in self.signers:
             self.signers[role] = {}
-        self.signers[role][signer.key_dict["keyid"]] = signer
+        self.signers[role][signer.public_key.keyid] = signer
 
     def rotate_keys(self, role: str) -> None:
         """remove all keys for role, then add threshold of new keys"""
         self.root.roles[role].keyids.clear()
         self.signers[role].clear()
-        for _ in range(0, self.root.roles[role].threshold):
-            key, signer = self.create_key()
-            self.root.add_key(key, role)
+        for _ in range(self.root.roles[role].threshold):
+            signer = CryptoSigner.generate_ed25519()
+            self.root.add_key(signer.public_key, role)
             self.add_signer(role, signer)
 
     def _initialize(self) -> None:
         """Setup a minimal valid repository."""
 
         self.md_targets = Metadata(Targets(expires=self.safe_expiry))
         self.md_snapshot = Metadata(Snapshot(expires=self.safe_expiry))
         self.md_timestamp = Metadata(Timestamp(expires=self.safe_expiry))
         self.md_root = Metadata(Root(expires=self.safe_expiry))
 
         for role in TOP_LEVEL_ROLE_NAMES:
-            key, signer = self.create_key()
-            self.md_root.signed.add_key(key, role)
+            signer = CryptoSigner.generate_ed25519()
+            self.md_root.signed.add_key(signer.public_key, role)
             self.add_signer(role, signer)
 
         self.publish_root()
 
     def publish_root(self) -> None:
         """Sign and store a new serialized version of root."""
         self.md_root.signatures.clear()
@@ -366,16 +357,16 @@
             delegator.delegations = Delegations({}, roles={})
 
         assert delegator.delegations.roles is not None
         # put delegation last by default
         delegator.delegations.roles[role.name] = role
 
         # By default add one new key for the role
-        key, signer = self.create_key()
-        delegator.add_key(key, role.name)
+        signer = CryptoSigner.generate_ed25519()
+        delegator.add_key(signer.public_key, role.name)
         self.add_signer(role.name, signer)
 
         # Add metadata for the role
         if role.name not in self.md_delegates:
             self.md_delegates[role.name] = Metadata(targets, {})
 
     def add_succinct_roles(
@@ -392,27 +383,27 @@
             delegator.delegations is not None
             and delegator.delegations.roles is not None
         ):
             raise ValueError(
                 "Can't add a succinct_roles when delegated roles are used"
             )
 
-        key, signer = self.create_key()
+        signer = CryptoSigner.generate_ed25519()
         succinct_roles = SuccinctRoles([], 1, bit_length, name_prefix)
         delegator.delegations = Delegations({}, None, succinct_roles)
 
         # Add targets metadata for all bins.
         for delegated_name in succinct_roles.get_roles():
             self.md_delegates[delegated_name] = Metadata(
                 Targets(expires=self.safe_expiry)
             )
 
             self.add_signer(delegated_name, signer)
 
-        delegator.add_key(key)
+        delegator.add_key(signer.public_key)
 
     def write(self) -> None:
         """Dump current repository metadata to self.dump_dir
 
         This is a debugging tool: dumping repository state before running
         Updater refresh may be useful while debugging a test.
         """
```

### Comparing `tuf-4.0.0/tests/simple_server.py` & `tuf-5.0.0/tests/simple_server.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/test_api.py` & `tuf-5.0.0/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,39 @@
-#!/usr/bin/env python
-
 # Copyright 2020, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 """Unit tests for api/metadata.py"""
 
 import json
 import logging
 import os
 import shutil
 import sys
 import tempfile
 import unittest
 from copy import copy, deepcopy
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from typing import Any, ClassVar, Dict, Optional
+from typing import ClassVar, Dict, Optional
 
 from securesystemslib import exceptions as sslib_exceptions
 from securesystemslib import hash as sslib_hash
-from securesystemslib.interface import (
-    import_ed25519_privatekey_from_file,
-    import_ed25519_publickey_from_file,
-)
-from securesystemslib.keys import generate_ed25519_key
 from securesystemslib.signer import (
+    CryptoSigner,
+    Key,
     SecretsHandler,
     Signer,
-    SSlibKey,
-    SSlibSigner,
 )
 
 from tests import utils
 from tuf.api import exceptions
 from tuf.api.dsse import SimpleEnvelope
 from tuf.api.metadata import (
     TOP_LEVEL_ROLE_NAMES,
     DelegatedRole,
     Delegations,
-    Key,
     Metadata,
     MetaFile,
     Root,
     RootVerificationResult,
     Signature,
     Snapshot,
     SuccinctRoles,
@@ -58,15 +50,15 @@
 
 class TestMetadata(unittest.TestCase):
     """Tests for public API of all classes in 'tuf/api/metadata.py'."""
 
     temporary_directory: ClassVar[str]
     repo_dir: ClassVar[str]
     keystore_dir: ClassVar[str]
-    keystore: ClassVar[Dict[str, Dict[str, Any]]]
+    signers: ClassVar[Dict[str, Signer]]
 
     @classmethod
     def setUpClass(cls) -> None:
         # Create a temporary directory to store the repository, metadata, and
         # target files.  'temporary_directory' must be deleted in
         # TearDownClass() so that temporary files are always removed, even when
         # exceptions occur.
@@ -82,21 +74,25 @@
         )
 
         cls.keystore_dir = os.path.join(cls.temporary_directory, "keystore")
         shutil.copytree(
             os.path.join(test_repo_data, "keystore"), cls.keystore_dir
         )
 
-        # Load keys into memory
-        cls.keystore = {}
-        for role in ["delegation", Snapshot.type, Targets.type, Timestamp.type]:
-            cls.keystore[role] = import_ed25519_privatekey_from_file(
-                os.path.join(cls.keystore_dir, role + "_key"),
-                password="password",
-            )
+        path = os.path.join(cls.repo_dir, "metadata", "root.json")
+        root = Metadata[Root].from_file(path).signed
+
+        # Load signers
+
+        cls.signers = {}
+        for role in [Snapshot.type, Targets.type, Timestamp.type]:
+            uri = f"file2:{os.path.join(cls.keystore_dir, role + '_key')}"
+            role_obj = root.get_delegated_role(role)
+            key = root.get_key(role_obj.keyids[0])
+            cls.signers[role] = CryptoSigner.from_priv_key_uri(uri, key)
 
     @classmethod
     def tearDownClass(cls) -> None:
         # Remove the temporary repository directory, which should contain all
         # the metadata, targets, and key files generated for the test cases.
         shutil.rmtree(cls.temporary_directory)
 
@@ -214,28 +210,26 @@
         # ... it has a single existing signature,
         self.assertEqual(len(md_obj.signatures), 1)
         # ... which is valid for the correct key.
         targets_key.verify_signature(sig, data)
         with self.assertRaises(sslib_exceptions.VerificationError):
             snapshot_key.verify_signature(sig, data)
 
-        sslib_signer = SSlibSigner(self.keystore[Snapshot.type])
         # Append a new signature with the unrelated key and assert that ...
-        snapshot_sig = md_obj.sign(sslib_signer, append=True)
+        snapshot_sig = md_obj.sign(self.signers[Snapshot.type], append=True)
         # ... there are now two signatures, and
         self.assertEqual(len(md_obj.signatures), 2)
         # ... both are valid for the corresponding keys.
         targets_key.verify_signature(sig, data)
         snapshot_key.verify_signature(snapshot_sig, data)
         # ... the returned (appended) signature is for snapshot key
         self.assertEqual(snapshot_sig.keyid, snapshot_keyid)
 
-        sslib_signer = SSlibSigner(self.keystore[Timestamp.type])
         # Create and assign (don't append) a new signature and assert that ...
-        ts_sig = md_obj.sign(sslib_signer, append=False)
+        ts_sig = md_obj.sign(self.signers[Timestamp.type], append=False)
         # ... there now is only one signature,
         self.assertEqual(len(md_obj.signatures), 1)
         # ... valid for that key.
         timestamp_key.verify_signature(ts_sig, data)
         with self.assertRaises(sslib_exceptions.VerificationError):
             targets_key.verify_signature(ts_sig, data)
 
@@ -255,15 +249,15 @@
             ) -> "Signer":
                 pass
 
             @property
             def public_key(self) -> Key:
                 raise RuntimeError("Not a real signer")
 
-            def sign(self, payload: bytes) -> Signature:
+            def sign(self, _payload: bytes) -> Signature:
                 raise RuntimeError("signing failed")
 
         failing_signer = FailingSigner()
 
         with self.assertRaises(exceptions.UnsignedMetadataError):
             md.sign(failing_signer)
 
@@ -464,17 +458,15 @@
         with self.assertRaises(exceptions.UnsignedMetadataError):
             root.verify_delegate(
                 Snapshot.type, snapshot_md.signed_bytes, snapshot_md.signatures
             )
 
         # verify succeeds when we correct the new signature and reach the
         # threshold of 2 keys
-        snapshot_md.sign(
-            SSlibSigner(self.keystore[Timestamp.type]), append=True
-        )
+        snapshot_md.sign(self.signers[Timestamp.type], append=True)
         root.verify_delegate(
             Snapshot.type, snapshot_md.signed_bytes, snapshot_md.signatures
         )
 
     def test_verification_result(self) -> None:
         vr = VerificationResult(3, {"a": None}, {"b": None})
         self.assertEqual(vr.missing, 2)
@@ -522,19 +514,18 @@
         root = Metadata[Root].from_file(root_path)
 
         key1_id = root.signed.roles[Root.type].keyids[0]
         key1 = root.signed.get_key(key1_id)
 
         key2_id = root.signed.roles[Timestamp.type].keyids[0]
         key2 = root.signed.get_key(key2_id)
-        priv_key2 = self.keystore[Timestamp.type]
 
         key3_id = "123456789abcdefg"
-        priv_key4 = self.keystore[Snapshot.type]
-        key4_id = priv_key4["keyid"]
+
+        key4_id = self.signers[Snapshot.type].public_key.keyid
 
         # Test: 1 authorized key, 1 valid signature
         result = root.signed.get_verification_result(
             Root.type, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key1_id: key1})
@@ -559,25 +550,25 @@
         )
         self.assertFalse(result)
         self.assertEqual(result.signed, {})
         self.assertEqual(result.unsigned, {key1_id: key1, key2_id: key2})
 
         # Test: 3 authorized keys, 1 valid signature, 1 invalid signature, 1
         # key missing key data
-        root.sign(SSlibSigner(priv_key2), append=True)
+        root.sign(self.signers[Timestamp.type], append=True)
         result = root.signed.get_verification_result(
             Root.type, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key2_id: key2})
         self.assertEqual(result.unsigned, {key1_id: key1})
 
         # Test: 3 authorized keys, 1 valid signature, 1 invalid signature, 1
         # key missing key data, 1 ignored unrelated signature
-        root.sign(SSlibSigner(priv_key4), append=True)
+        root.sign(self.signers[Snapshot.type], append=True)
         self.assertEqual(
             set(root.signatures.keys()), {key1_id, key2_id, key4_id}
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key2_id: key2})
         self.assertEqual(result.unsigned, {key1_id: key1})
 
@@ -589,17 +580,14 @@
         root = Metadata[Root].from_file(root_path)
 
         key1_id = root.signed.roles[Root.type].keyids[0]
         key1 = root.signed.get_key(key1_id)
 
         key2_id = root.signed.roles[Timestamp.type].keyids[0]
         key2 = root.signed.get_key(key2_id)
-        priv_key2 = self.keystore[Timestamp.type]
-
-        priv_key4 = self.keystore[Snapshot.type]
 
         # Test: Verify with no previous root version
         result = root.signed.get_root_verification_result(
             None, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key1_id: key1})
@@ -636,24 +624,24 @@
             prev_root.signed, root.signed_bytes, root.signatures
         )
         self.assertFalse(result)
         self.assertEqual(result.signed, {key1_id: key1})
         self.assertEqual(result.unsigned, {key2_id: key2})
 
         # Test: Sign root with both keys
-        root.sign(SSlibSigner(priv_key2), append=True)
+        root.sign(self.signers[Timestamp.type], append=True)
         result = root.signed.get_root_verification_result(
             prev_root.signed, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key1_id: key1, key2_id: key2})
         self.assertEqual(result.unsigned, {})
 
         # Test: Sign root with an unrelated key
-        root.sign(SSlibSigner(priv_key4), append=True)
+        root.sign(self.signers[Snapshot.type], append=True)
         result = root.signed.get_root_verification_result(
             prev_root.signed, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key1_id: key1, key2_id: key2})
         self.assertEqual(result.unsigned, {})
 
@@ -671,82 +659,67 @@
         result = root.signed.get_root_verification_result(
             prev_root.signed, root.signed_bytes, root.signatures
         )
         self.assertTrue(result)
         self.assertEqual(result.signed, {key1_id: key1, key2_id: key2})
         self.assertEqual(result.unsigned, {})
 
-    def test_key_class(self) -> None:
-        # Test if from_securesystemslib_key removes the private key from keyval
-        # of a securesystemslib key dictionary.
-        sslib_key = generate_ed25519_key()
-        key = SSlibKey.from_securesystemslib_key(sslib_key)
-        self.assertFalse("private" in key.keyval)
-
     def test_root_add_key_and_revoke_key(self) -> None:
         root_path = os.path.join(self.repo_dir, "metadata", "root.json")
         root = Metadata[Root].from_file(root_path)
 
         # Create a new key
-        root_key2 = import_ed25519_publickey_from_file(
-            os.path.join(self.keystore_dir, "root_key2.pub")
-        )
-        keyid = root_key2["keyid"]
-        key_metadata = SSlibKey(
-            keyid,
-            root_key2["keytype"],
-            root_key2["scheme"],
-            root_key2["keyval"],
-        )
+        signer = CryptoSigner.generate_ecdsa()
+        key = signer.public_key
 
         # Assert that root does not contain the new key
-        self.assertNotIn(keyid, root.signed.roles[Root.type].keyids)
-        self.assertNotIn(keyid, root.signed.keys)
+        self.assertNotIn(key.keyid, root.signed.roles[Root.type].keyids)
+        self.assertNotIn(key.keyid, root.signed.keys)
 
         # Assert that add_key with old argument order will raise an error
         with self.assertRaises(ValueError):
-            root.signed.add_key(Root.type, key_metadata)
+            root.signed.add_key(Root.type, key)
 
         # Add new root key
-        root.signed.add_key(key_metadata, Root.type)
+        root.signed.add_key(key, Root.type)
 
         # Assert that key is added
-        self.assertIn(keyid, root.signed.roles[Root.type].keyids)
-        self.assertIn(keyid, root.signed.keys)
+        self.assertIn(key.keyid, root.signed.roles[Root.type].keyids)
+        self.assertIn(key.keyid, root.signed.keys)
 
         # Confirm that the newly added key does not break
         # the object serialization
         root.to_dict()
 
         # Try adding the same key again and assert its ignored.
         pre_add_keyid = root.signed.roles[Root.type].keyids.copy()
-        root.signed.add_key(key_metadata, Root.type)
+        root.signed.add_key(key, Root.type)
         self.assertEqual(pre_add_keyid, root.signed.roles[Root.type].keyids)
 
         # Add the same key to targets role as well
-        root.signed.add_key(key_metadata, Targets.type)
+        root.signed.add_key(key, Targets.type)
 
         # Add the same key to a nonexistent role.
         with self.assertRaises(ValueError):
-            root.signed.add_key(key_metadata, "nosuchrole")
+            root.signed.add_key(key, "nosuchrole")
 
         # Remove the key from root role (targets role still uses it)
-        root.signed.revoke_key(keyid, Root.type)
-        self.assertNotIn(keyid, root.signed.roles[Root.type].keyids)
-        self.assertIn(keyid, root.signed.keys)
+        root.signed.revoke_key(key.keyid, Root.type)
+        self.assertNotIn(key.keyid, root.signed.roles[Root.type].keyids)
+        self.assertIn(key.keyid, root.signed.keys)
 
         # Remove the key from targets as well
-        root.signed.revoke_key(keyid, Targets.type)
-        self.assertNotIn(keyid, root.signed.roles[Targets.type].keyids)
-        self.assertNotIn(keyid, root.signed.keys)
+        root.signed.revoke_key(key.keyid, Targets.type)
+        self.assertNotIn(key.keyid, root.signed.roles[Targets.type].keyids)
+        self.assertNotIn(key.keyid, root.signed.keys)
 
         with self.assertRaises(ValueError):
             root.signed.revoke_key("nosuchkey", Root.type)
         with self.assertRaises(ValueError):
-            root.signed.revoke_key(keyid, "nosuchrole")
+            root.signed.revoke_key(key.keyid, "nosuchrole")
 
     def test_is_target_in_pathpattern(self) -> None:
         supported_use_cases = [
             ("foo.tgz", "foo.tgz"),
             ("foo.tgz", "*"),
             ("foo.tgz", "*.tgz"),
             ("foo-version-a.tgz", "foo-version-?.tgz"),
@@ -1139,35 +1112,37 @@
         # test succinct delegation
         bit_len = 3
         role2 = SuccinctRoles([], 1, bit_len, "prefix")
         delegations.succinct_roles = role2
         for name in ["prefix-", "prefix--1", f"prefix-{2**bit_len:0x}"]:
             with self.assertRaises(ValueError, msg=f"role name '{name}'"):
                 targets.get_delegated_role(name)
-        for i in range(0, 2**bit_len):
+        for i in range(2**bit_len):
             self.assertEqual(
                 targets.get_delegated_role(f"prefix-{i:0x}"), role2
             )
 
 
 class TestSimpleEnvelope(unittest.TestCase):
     """Tests for public API in 'tuf/api/dsse.py'."""
 
     @classmethod
     def setUpClass(cls) -> None:
         repo_data_dir = Path(utils.TESTS_DIR) / "repository_data"
         cls.metadata_dir = repo_data_dir / "repository" / "metadata"
-        cls.signer_store = {}
+        cls.keystore_dir = repo_data_dir / "keystore"
+        cls.signers = {}
+        root_path = os.path.join(cls.metadata_dir, "root.json")
+        root: Root = Metadata.from_file(root_path).signed
+
         for role in [Snapshot, Targets, Timestamp]:
-            key_path = repo_data_dir / "keystore" / f"{role.type}_key"
-            key = import_ed25519_privatekey_from_file(
-                str(key_path),
-                password="password",
-            )
-            cls.signer_store[role.type] = SSlibSigner(key)
+            uri = f"file2:{os.path.join(cls.keystore_dir, role.type + '_key')}"
+            role_obj = root.get_delegated_role(role.type)
+            key = root.get_key(role_obj.keyids[0])
+            cls.signers[role.type] = CryptoSigner.from_priv_key_uri(uri, key)
 
     def test_serialization(self) -> None:
         """Basic de/serialization test.
 
         1. Load test metadata for each role
         2. Wrap metadata payloads in envelope serializing the payload
         3. Serialize envelope
@@ -1194,15 +1169,15 @@
 
     def test_fail_envelope_deserialization(self) -> None:
         with self.assertRaises(DeserializationError):
             SimpleEnvelope.from_bytes(b"[")
 
     def test_fail_payload_serialization(self) -> None:
         with self.assertRaises(SerializationError):
-            SimpleEnvelope.from_signed("foo")  # type: ignore
+            SimpleEnvelope.from_signed("foo")  # type: ignore[type-var]
 
     def test_fail_payload_deserialization(self) -> None:
         payloads = [b"[", b'{"_type": "foo"}']
         for payload in payloads:
             envelope = SimpleEnvelope(payload, "bar", [])
             with self.assertRaises(DeserializationError):
                 envelope.get_signed()
@@ -1220,25 +1195,21 @@
         root = Metadata[Root].from_file(str(root_path)).signed
 
         for role in [Timestamp, Snapshot, Targets]:
             metadata_path = self.metadata_dir / f"{role.type}.json"
             metadata = Metadata.from_file(str(metadata_path))
             self.assertIsInstance(metadata.signed, role)
 
-            signer = self.signer_store[role.type]
-            self.assertIn(
-                signer.key_dict["keyid"], root.roles[role.type].keyids
-            )
+            signer = self.signers[role.type]
+            self.assertIn(signer.public_key.keyid, root.roles[role.type].keyids)
 
             envelope = SimpleEnvelope.from_signed(metadata.signed)
             envelope.sign(signer)
             self.assertTrue(len(envelope.signatures) == 1)
 
-            root.verify_delegate(
-                role.type, envelope.pae(), envelope.signatures_dict
-            )
+            root.verify_delegate(role.type, envelope.pae(), envelope.signatures)
 
 
 # Run unit test.
 if __name__ == "__main__":
     utils.configure_test_logging(sys.argv)
     unittest.main()
```

### Comparing `tuf-4.0.0/tests/test_examples.py` & `tuf-5.0.0/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # Copyright 2020, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 """Unit tests for 'examples' scripts."""
 
 import glob
 import os
 import shutil
```

### Comparing `tuf-4.0.0/tests/test_fetcher_ng.py` & `tuf-5.0.0/tests/test_fetcher_ng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Unit test for RequestsFetcher."""
 
 import io
 import logging
@@ -42,15 +40,15 @@
         with tempfile.NamedTemporaryFile(
             dir=os.getcwd(), delete=False
         ) as cls.target_file:
             cls.target_file.write(cls.file_contents)
 
         cls.url_prefix = (
             f"http://{utils.TEST_HOST_ADDRESS}:"
-            f"{str(cls.server_process_handler.port)}"
+            f"{cls.server_process_handler.port!s}"
         )
         target_filename = os.path.basename(cls.target_file.name)
         cls.url = f"{cls.url_prefix}/{target_filename}"
 
     @classmethod
     def tearDownClass(cls) -> None:
         # Stop server process and perform clean up.
@@ -103,15 +101,15 @@
         with self.assertRaises(exceptions.DownloadHTTPError) as cm:
             self.url = f"{self.url_prefix}/non-existing-path"
             self.fetcher.fetch(self.url)
         self.assertEqual(cm.exception.status_code, 404)
 
     # Response read timeout error
     @patch.object(requests.Session, "get")
-    def test_response_read_timeout(self, mock_session_get: Any) -> None:
+    def test_response_read_timeout(self, mock_session_get: Mock) -> None:
         mock_response = Mock()
         attr = {
             "iter_content.side_effect": requests.exceptions.ConnectionError(
                 "Simulated timeout"
             )
         }
         mock_response.configure_mock(**attr)
@@ -123,15 +121,15 @@
 
     # Read/connect session timeout error
     @patch.object(
         requests.Session,
         "get",
         side_effect=requests.exceptions.Timeout("Simulated timeout"),
     )
-    def test_session_get_timeout(self, mock_session_get: Any) -> None:
+    def test_session_get_timeout(self, mock_session_get: Mock) -> None:
         with self.assertRaises(exceptions.SlowRetrievalError):
             self.fetcher.fetch(self.url)
         mock_session_get.assert_called_once()
 
     # Simple bytes download
     def test_download_bytes(self) -> None:
         data = self.fetcher.download_bytes(self.url, self.file_length)
```

### Comparing `tuf-4.0.0/tests/test_metadata_eq_.py` & `tuf-5.0.0/tests/test_metadata_eq_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test __eq__ implementations of classes inside tuf/api/metadata.py."""
 
 import copy
 import os
@@ -128,15 +126,15 @@
         self.assertNotEqual(md, md_2)
 
         # Test that metadata objects with empty signatures are equal
         md.signatures = {}
         self.assertEqual(md, md_2)
 
         # Metadata objects with different signatures types are not equal.
-        md_2.signatures = ""  # type: ignore
+        md_2.signatures = ""  # type: ignore[assignment]
         self.assertNotEqual(md, md_2)
 
     def test_delegations_eq_roles_reversed_order(self) -> None:
         # Test comparing objects with same delegated roles but different order.
         role_one_dict = {
             "keyids": ["keyid1"],
             "name": "a",
```

### Comparing `tuf-4.0.0/tests/test_metadata_generation.py` & `tuf-5.0.0/tests/test_metadata_generation.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/test_metadata_serialization.py` & `tuf-5.0.0/tests/test_metadata_serialization.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/test_trusted_metadata_set.py` & `tuf-5.0.0/tests/test_trusted_metadata_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 import logging
 import os
 import sys
 import unittest
 from datetime import datetime, timezone
 from typing import Callable, ClassVar, Dict, List, Optional, Tuple
 
-from securesystemslib.interface import (
-    import_ed25519_privatekey_from_file,
-    import_rsa_privatekey_from_file,
-)
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import Signer
 
 from tests import utils
 from tuf.api import exceptions
 from tuf.api.dsse import SimpleEnvelope
 from tuf.api.metadata import (
     Metadata,
     MetaFile,
@@ -34,15 +30,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class TestTrustedMetadataSet(unittest.TestCase):
     """Tests for all public API of the TrustedMetadataSet class."""
 
-    keystore: ClassVar[Dict[str, SSlibSigner]]
+    keystore: ClassVar[Dict[str, Signer]]
     metadata: ClassVar[Dict[str, bytes]]
     repo_dir: ClassVar[str]
 
     @classmethod
     def modify_metadata(
         cls, rolename: str, modification_func: Callable
     ) -> bytes:
@@ -75,24 +71,27 @@
         ]:
             with open(os.path.join(cls.repo_dir, f"{md}.json"), "rb") as f:
                 cls.metadata[md] = f.read()
 
         keystore_dir = os.path.join(
             utils.TESTS_DIR, "repository_data", "keystore"
         )
+        root = Metadata[Root].from_bytes(cls.metadata[Root.type]).signed
+
         cls.keystore = {}
-        root_key_dict = import_rsa_privatekey_from_file(
-            os.path.join(keystore_dir, Root.type + "_key"), password="password"
-        )
-        cls.keystore[Root.type] = SSlibSigner(root_key_dict)
-        for role in ["delegation", Snapshot.type, Targets.type, Timestamp.type]:
-            key_dict = import_ed25519_privatekey_from_file(
-                os.path.join(keystore_dir, role + "_key"), password="password"
-            )
-            cls.keystore[role] = SSlibSigner(key_dict)
+        for role in [
+            Root.type,
+            Snapshot.type,
+            Targets.type,
+            Timestamp.type,
+        ]:
+            uri = f"file2:{os.path.join(keystore_dir, role + '_key')}"
+            role_obj = root.get_delegated_role(role)
+            key = root.get_key(role_obj.keyids[0])
+            cls.keystore[role] = Signer.from_priv_key_uri(uri, key)
 
         def hashes_length_modifier(timestamp: Timestamp) -> None:
             timestamp.snapshot_meta.hashes = None
             timestamp.snapshot_meta.length = None
 
         cls.metadata[Timestamp.type] = cls.modify_metadata(
             Timestamp.type, hashes_length_modifier
```

### Comparing `tuf-4.0.0/tests/test_updater_consistent_snapshot.py` & `tuf-5.0.0/tests/test_updater_consistent_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test ngclient Updater toggling consistent snapshot"""
 
 import os
 import sys
```

### Comparing `tuf-4.0.0/tests/test_updater_delegation_graphs.py` & `tuf-5.0.0/tests/test_updater_delegation_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test updating delegated targets roles and searching for
 target files with various delegation graphs"""
 
 import os
```

### Comparing `tuf-4.0.0/tests/test_updater_fetch_target.py` & `tuf-5.0.0/tests/test_updater_fetch_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test 'Fetch target' from 'Detailed client workflow' as well as
 target files storing/loading from cache.
 """
```

### Comparing `tuf-4.0.0/tests/test_updater_key_rotations.py` & `tuf-5.0.0/tests/test_updater_key_rotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test ngclient Updater key rotation handling"""
 
 import os
 import sys
 import tempfile
 import unittest
 from dataclasses import dataclass
 from typing import ClassVar, Dict, List, Optional, Type
 
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import CryptoSigner, Signer
 
 from tests import utils
 from tests.repository_simulator import RepositorySimulator
 from tests.utils import run_sub_tests_with_dataset
 from tuf.api.exceptions import UnsignedMetadataError
 from tuf.api.metadata import Key, Root
 from tuf.ngclient import Updater
@@ -33,26 +31,24 @@
 class TestUpdaterKeyRotations(unittest.TestCase):
     """Test ngclient root rotation handling"""
 
     # set dump_dir to trigger repository state dumps
     dump_dir: Optional[str] = None
     temp_dir: ClassVar[tempfile.TemporaryDirectory]
     keys: ClassVar[List[Key]]
-    signers: ClassVar[List[SSlibSigner]]
+    signers: ClassVar[List[Signer]]
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.temp_dir = tempfile.TemporaryDirectory()
 
         # Pre-create a bunch of keys and signers
-        cls.keys = []
         cls.signers = []
         for _ in range(10):
-            key, signer = RepositorySimulator.create_key()
-            cls.keys.append(key)
+            signer = CryptoSigner.generate_ed25519()
             cls.signers.append(signer)
 
     @classmethod
     def tearDownClass(cls) -> None:
         cls.temp_dir.cleanup()
 
     def setup_subtest(self) -> None:
@@ -176,15 +172,15 @@
         for rootver in root_versions:
             # clear root keys, signers
             self.sim.root.roles[Root.type].keyids.clear()
             self.sim.signers[Root.type].clear()
 
             self.sim.root.roles[Root.type].threshold = rootver.threshold
             for i in rootver.keys:
-                self.sim.root.add_key(self.keys[i], Root.type)
+                self.sim.root.add_key(self.signers[i].public_key, Root.type)
             for i in rootver.sigs:
                 self.sim.add_signer(Root.type, self.signers[i])
             self.sim.root.version += 1
             self.sim.publish_root()
 
         # run client workflow, assert success/failure
         expected_error = root_versions[-1].res
@@ -245,15 +241,15 @@
         for role in roles:
             # clear role keys, signers
             self.sim.root.roles[role].keyids.clear()
             self.sim.signers[role].clear()
 
             self.sim.root.roles[role].threshold = md_version.threshold
             for i in md_version.keys:
-                self.sim.root.add_key(self.keys[i], role)
+                self.sim.root.add_key(self.signers[i].public_key, role)
 
             for i in md_version.sigs:
                 self.sim.add_signer(role, self.signers[i])
 
             self.sim.root.version += 1
             self.sim.publish_root()
```

### Comparing `tuf-4.0.0/tests/test_updater_ng.py` & `tuf-5.0.0/tests/test_updater_ng.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test Updater class"""
 
 import logging
 import os
 import shutil
 import sys
 import tempfile
 import unittest
 from typing import Callable, ClassVar, List
 from unittest.mock import MagicMock, patch
 
-from securesystemslib.interface import import_rsa_privatekey_from_file
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import Signer
 
 from tests import utils
-from tuf import ngclient
 from tuf.api import exceptions
 from tuf.api.metadata import (
     Metadata,
     Root,
     Snapshot,
     TargetFile,
     Targets,
     Timestamp,
 )
+from tuf.ngclient import Updater, UpdaterConfig
 
 logger = logging.getLogger(__name__)
 
 
 class TestUpdater(unittest.TestCase):
     """Test the Updater class from 'tuf/ngclient/updater.py'."""
 
@@ -103,15 +100,15 @@
         )
 
         self.metadata_url = f"{url_prefix}/metadata/"
         self.targets_url = f"{url_prefix}/targets/"
         self.dl_dir = tempfile.mkdtemp(dir=self.tmp_test_dir)
         # Creating a repository instance.  The test cases will use this client
         # updater to refresh metadata, fetch target files, etc.
-        self.updater = ngclient.Updater(
+        self.updater = Updater(
             metadata_dir=self.client_directory,
             metadata_base_url=self.metadata_url,
             target_dir=self.dl_dir,
             target_base_url=self.targets_url,
         )
 
     def tearDown(self) -> None:
@@ -123,23 +120,25 @@
         modification_func: Callable[[Metadata], None],
         bump_version: bool = False,
     ) -> None:
         """Apply 'modification_func' to root and persist it."""
         role_path = os.path.join(
             self.repository_directory, "metadata", "root.json"
         )
-        root = Metadata.from_file(role_path)
+        root = Metadata[Root].from_file(role_path)
         modification_func(root)
         if bump_version:
             root.signed.version += 1
         root_key_path = os.path.join(self.keystore_directory, "root_key")
-        root_key_dict = import_rsa_privatekey_from_file(
-            root_key_path, password="password"
-        )
-        signer = SSlibSigner(root_key_dict)
+
+        uri = f"file2:{root_key_path}"
+        role = root.signed.get_delegated_role(Root.type)
+        key = root.signed.get_key(role.keyids[0])
+        signer = Signer.from_priv_key_uri(uri, key)
+
         root.sign(signer)
         root.to_file(
             os.path.join(self.repository_directory, "metadata", "root.json")
         )
         root.to_file(
             os.path.join(
                 self.repository_directory,
@@ -238,24 +237,22 @@
         # Get targetinfo for 'file3.txt' listed in the delegated role1
         self.updater.get_targetinfo("file3.txt")
         expected_files = ["role1", "root", "snapshot", "targets", "timestamp"]
         self._assert_files(expected_files)
 
     def test_both_target_urls_not_set(self) -> None:
         # target_base_url = None and Updater._target_base_url = None
-        updater = ngclient.Updater(
-            self.client_directory, self.metadata_url, self.dl_dir
-        )
+        updater = Updater(self.client_directory, self.metadata_url, self.dl_dir)
         info = TargetFile(1, {"sha256": ""}, "targetpath")
         with self.assertRaises(ValueError):
             updater.download_target(info)
 
     def test_no_target_dir_no_filepath(self) -> None:
         # filepath = None and Updater.target_dir = None
-        updater = ngclient.Updater(self.client_directory, self.metadata_url)
+        updater = Updater(self.client_directory, self.metadata_url)
         info = TargetFile(1, {"sha256": ""}, "targetpath")
         with self.assertRaises(ValueError):
             updater.find_cached_target(info)
         with self.assertRaises(ValueError):
             updater.download_target(info)
 
     def test_external_targets_url(self) -> None:
@@ -278,15 +275,15 @@
         with self.assertRaises(exceptions.RepositoryError):
             targetinfo.length = length
             targetinfo.hashes = {"sha256": "abcd"}
             self.updater.download_target(targetinfo)
 
     def test_updating_root(self) -> None:
         # Bump root version, resign and refresh
-        self._modify_repository_root(lambda root: None, bump_version=True)
+        self._modify_repository_root(lambda _: None, bump_version=True)
         self.updater.refresh()
         self.assertEqual(self.updater._trusted_set.root.version, 2)
 
     def test_missing_targetinfo(self) -> None:
         self.updater.refresh()
 
         # Get targetinfo for non-existing file
@@ -319,11 +316,32 @@
     def test_non_existing_target_file(self) -> None:
         info = TargetFile(1, {"sha256": ""}, "/non_existing_file.txt")
         # When non-existing target file is given, download fails with
         # "404 Client Error: File not found for url"
         with self.assertRaises(exceptions.DownloadHTTPError):
             self.updater.download_target(info)
 
+    def test_user_agent(self) -> None:
+        # test default
+        self.updater.refresh()
+        session = next(iter(self.updater._fetcher._sessions.values()))
+        ua = session.headers["User-Agent"]
+        self.assertEqual(ua[:4], "tuf/")
+
+        # test custom UA
+        updater = Updater(
+            self.client_directory,
+            self.metadata_url,
+            self.dl_dir,
+            self.targets_url,
+            config=UpdaterConfig(app_user_agent="MyApp/1.2.3"),
+        )
+        updater.refresh()
+        session = next(iter(updater._fetcher._sessions.values()))
+        ua = session.headers["User-Agent"]
+
+        self.assertEqual(ua[:16], "MyApp/1.2.3 tuf/")
+
 
 if __name__ == "__main__":
     utils.configure_test_logging(sys.argv)
     unittest.main()
```

### Comparing `tuf-4.0.0/tests/test_updater_top_level_update.py` & `tuf-5.0.0/tests/test_updater_top_level_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test ngclient Updater top-level metadata update workflow"""
 
 import builtins
 import datetime
@@ -443,15 +441,15 @@
         self.sim.timestamp.version = 1
 
         # client refresh the metadata and see the initial timestamp version
         self._run_refresh()
         self._assert_version_equals(Timestamp.type, 1)
 
     def test_new_snapshot_hash_mismatch(self) -> None:
-        # Check against timestamp role’s snapshot hash
+        # Check against timestamp role's snapshot hash
 
         # Update timestamp with snapshot's hashes
         self.sim.compute_metafile_hashes_length = True
         self.sim.update_timestamp()  # timestamp v2
         self._run_refresh()
 
         # Modify snapshot contents without updating
@@ -473,15 +471,15 @@
         self.sim.signers[Snapshot.type].clear()
         with self.assertRaises(UnsignedMetadataError):
             self._run_refresh()
 
         self._assert_files_exist([Root.type, Timestamp.type])
 
     def test_new_snapshot_version_mismatch(self) -> None:
-        # Check against timestamp role’s snapshot version
+        # Check against timestamp role's snapshot version
 
         # Increase snapshot version without updating timestamp
         self.sim.snapshot.version += 1
         with self.assertRaises(BadVersionNumberError):
             self._run_refresh()
 
         self._assert_files_exist([Root.type, Timestamp.type])
@@ -540,15 +538,15 @@
 
         with self.assertRaises(ExpiredMetadataError):
             self._run_refresh()
 
         self._assert_files_exist([Root.type, Timestamp.type])
 
     def test_new_targets_hash_mismatch(self) -> None:
-        # Check against snapshot role’s targets hashes
+        # Check against snapshot role's targets hashes
 
         # Update snapshot with target's hashes
         self.sim.compute_metafile_hashes_length = True
         self.sim.update_snapshot()
         self._run_refresh()
 
         # Modify targets contents without updating
@@ -571,15 +569,15 @@
         self.sim.signers[Targets.type].clear()
         with self.assertRaises(UnsignedMetadataError):
             self._run_refresh()
 
         self._assert_files_exist([Root.type, Timestamp.type, Snapshot.type])
 
     def test_new_targets_version_mismatch(self) -> None:
-        # Check against snapshot role’s targets version
+        # Check against snapshot role's targets version
 
         # Increase targets version without updating snapshot
         self.sim.targets.version += 1
         with self.assertRaises(BadVersionNumberError):
             self._run_refresh()
 
         self._assert_files_exist([Root.type, Timestamp.type, Snapshot.type])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tuf-4.0.0/tests/test_updater_validation.py` & `tuf-5.0.0/tests/test_updater_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2022, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Test ngclient Updater validations."""
 
 import os
 import sys
```

### Comparing `tuf-4.0.0/tests/test_utils.py` & `tuf-5.0.0/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2020, TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """
 <Program Name>
   test_utils.py
 
@@ -32,15 +30,15 @@
 
 def can_connect(port: int) -> bool:
     """Check if a socket can connect on the given port"""
     try:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.connect(("localhost", port))
         return True
-    except Exception:
+    except Exception:  # noqa: BLE001
         return False
     finally:
         # The process will always enter in finally even after return.
         if sock:
             sock.close()
```

### Comparing `tuf-4.0.0/tests/utils.py` & `tuf-5.0.0/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2020, TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """
 <Program Name>
   utils.py
 
@@ -216,21 +214,21 @@
         """
 
         self._start_process(extra_cmd_args, popen_cwd)
         self._start_redirect_thread()
 
         self._wait_for_port(timeout)
 
-        self.__logger.info(self.server + " serving on " + str(self.port))
+        self.__logger.info("%s serving on %d", self.server, self.port)
 
     def _start_process(self, extra_cmd_args: List[str], popen_cwd: str) -> None:
         """Starts the process running the server."""
 
         # The "-u" option forces stdin, stdout and stderr to be unbuffered.
-        command = [sys.executable, "-u", self.server] + extra_cmd_args
+        command = [sys.executable, "-u", self.server, *extra_cmd_args]
 
         # Reusing one subprocess in multiple tests, but split up the logs
         # for each.
         self.__server_process = subprocess.Popen(
             command,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
@@ -317,17 +315,15 @@
 
     def _kill_server_process(self) -> None:
         """Kills the server subprocess if it's running."""
 
         assert isinstance(self.__server_process, subprocess.Popen)
         if self.is_process_running():
             self.__logger.info(
-                "Server process "
-                + str(self.__server_process.pid)
-                + " terminated."
+                "Server process %d terminated", self.__server_process.pid
             )
             self.__server_process.kill()
             self.__server_process.wait()
 
     def flush_log(self) -> None:
         """Flushes the log lines from the logging queue."""
 
@@ -340,15 +336,15 @@
                     self.__logged_messages.append(line)
             except queue.Empty:
                 # No more lines are logged in the queue.
                 break
 
         if len(self.__logged_messages) > 0:
             title = "Test server (" + self.server + ") output:\n"
-            message = [title] + self.__logged_messages
+            message = [title, *self.__logged_messages]
             self.__logger.info("| ".join(message))
             self.__logged_messages = []
 
     def clean(self) -> None:
         """
         Kills the subprocess and closes the TempFile.
         Calls flush_log to check for logged information, but not yet flushed.
```

### Comparing `tuf-4.0.0/tests/generated_data/generate_md.py` & `tuf-5.0.0/tests/generated_data/generate_md.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,55 +2,61 @@
 
 # Copyright New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 import os
 import sys
 from datetime import datetime, timezone
-from typing import Dict, List, Optional
+from typing import List, Optional
 
-from securesystemslib.signer import SSlibKey, SSlibSigner
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
+from securesystemslib.signer import CryptoSigner, Signer, SSlibKey
 
 from tests import utils
-from tuf.api.metadata import Key, Metadata, Root, Snapshot, Targets, Timestamp
+from tuf.api.metadata import Metadata, Root, Snapshot, Targets, Timestamp
 from tuf.api.serialization.json import JSONSerializer
 
 # Hardcode keys and expiry time to achieve reproducibility.
 public_values: List[str] = [
     "b11d2ff132c033a657318c74c39526476c56de7556c776f11070842dbc4ac14c",
     "250f9ae3d1d3d5c419a73cfb4a470c01de1d5d3d61a3825416b5f5d6b88f4a30",
     "82380623abb9666d4bf274b1a02577469445a972e5650d270101faa5107b19c8",
     "0e6738fc1ac6fb4de680b4be99ecbcd99b030f3963f291277eef67bb9bd123e9",
 ]
-private_values: List[str] = [
-    "510e5e04d7a364af850533856eacdf65d30cc0f8803ecd5fdc0acc56ca2aa91c",
-    "e6645b00312c8a257782e3e61e85bafda4317ad072c52251ef933d480c387abd",
-    "cd13dd2180334b24c19b32aaf27f7e375a614d7ba0777220d5c2290bb2f9b868",
-    "7e2e751145d1b22f6e40d4ba2aa47158207acfd3c003f1cbd5a08141dfc22a15",
+private_values: List[bytes] = [
+    bytes.fromhex(
+        "510e5e04d7a364af850533856eacdf65d30cc0f8803ecd5fdc0acc56ca2aa91c"
+    ),
+    bytes.fromhex(
+        "e6645b00312c8a257782e3e61e85bafda4317ad072c52251ef933d480c387abd"
+    ),
+    bytes.fromhex(
+        "cd13dd2180334b24c19b32aaf27f7e375a614d7ba0777220d5c2290bb2f9b868"
+    ),
+    bytes.fromhex(
+        "7e2e751145d1b22f6e40d4ba2aa47158207acfd3c003f1cbd5a08141dfc22a15"
+    ),
 ]
 keyids: List[str] = [
     "5822582e7072996c1eef1cec24b61115d364987faa486659fe3d3dce8dae2aba",
     "09d440e3725cec247dcb8703b646a87dd2a4d75343e8095c036c32795eefe3b9",
     "3458204ed467519c19a5316eb278b5608472a1bbf15850ebfb462d5315e4f86d",
     "2be5c21e3614f9f178fb49c4a34d0c18ffac30abd14ced917c60a52c8d8094b7",
 ]
 
-keys: Dict[str, Key] = {}
-for index in range(4):
-    keys[f"ed25519_{index}"] = SSlibKey.from_securesystemslib_key(
-        {
-            "keytype": "ed25519",
-            "scheme": "ed25519",
-            "keyid": keyids[index],
-            "keyval": {
-                "public": public_values[index],
-                "private": private_values[index],
-            },
-        }
+signers: List[Signer] = []
+for index in range(len(keyids)):
+    key = SSlibKey(
+        keyids[index],
+        "ed25519",
+        "ed25519",
+        {"public": public_values[index]},
     )
+    private_key = Ed25519PrivateKey.from_private_bytes(private_values[index])
+    signers.append(CryptoSigner(private_key, key))
 
 EXPIRY = datetime(2050, 1, 1, tzinfo=timezone.utc)
 OUT_DIR = "generated_data/ed25519_metadata"
 if not os.path.exists(OUT_DIR):
     os.mkdir(OUT_DIR)
 
 SERIALIZER = JSONSerializer()
@@ -84,33 +90,22 @@
             local staored.
     """
     md_root = Metadata(Root(expires=EXPIRY))
     md_timestamp = Metadata(Timestamp(expires=EXPIRY))
     md_snapshot = Metadata(Snapshot(expires=EXPIRY))
     md_targets = Metadata(Targets(expires=EXPIRY))
 
-    md_root.signed.add_key(keys["ed25519_0"], "root")
-    md_root.signed.add_key(keys["ed25519_1"], "timestamp")
-    md_root.signed.add_key(keys["ed25519_2"], "snapshot")
-    md_root.signed.add_key(keys["ed25519_3"], "targets")
+    md_root.signed.add_key(signers[0].public_key, "root")
+    md_root.signed.add_key(signers[1].public_key, "timestamp")
+    md_root.signed.add_key(signers[2].public_key, "snapshot")
+    md_root.signed.add_key(signers[3].public_key, "targets")
 
     for i, md in enumerate([md_root, md_timestamp, md_snapshot, md_targets]):
         assert isinstance(md, Metadata)
-        signer = SSlibSigner(
-            {
-                "keytype": "ed25519",
-                "scheme": "ed25519",
-                "keyid": keyids[i],
-                "keyval": {
-                    "public": public_values[i],
-                    "private": private_values[i],
-                },
-            }
-        )
-        md.sign(signer)
+        md.sign(signers[i])
         path = os.path.join(OUT_DIR, f"{md.signed.type}_with_ed25519.json")
         if verify:
             verify_generation(md, path)
 
         if dump:
             md.to_file(path, SERIALIZER)
```

### Comparing `tuf-4.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json` & `tuf-5.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/README.md` & `tuf-5.0.0/tests/repository_data/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json` & `tuf-5.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json` & `tuf-5.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json` & `tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json` & `tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json` & `tuf-5.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/keystore/root_key2` & `tuf-5.0.0/tests/repository_data/keystore/root_key2`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/keystore/root_key3` & `tuf-5.0.0/tests/repository_data/keystore/root_key3`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/1.root.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/role1.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/root.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/root.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/snapshot.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/targets.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tests/repository_data/repository/metadata/timestamp.json` & `tuf-5.0.0/tests/repository_data/repository/metadata/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/api/_payload.py` & `tuf-5.0.0/tuf/api/_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         self.version = version
 
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Signed):
             return False
 
         return (
             self.type == other.type
             and self.version == other.version
             and self.spec_version == other.spec_version
@@ -249,15 +249,15 @@
         self.keyids = keyids
         self.threshold = threshold
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Role):
             return False
 
         return (
             self.keyids == other.keyids
             and self.threshold == other.threshold
             and self.unrecognized_fields == other.unrecognized_fields
@@ -500,15 +500,15 @@
 
         if roles is None:
             roles = {r: Role([], 1) for r in TOP_LEVEL_ROLE_NAMES}
         elif set(roles) != TOP_LEVEL_ROLE_NAMES:
             raise ValueError("Role names must be the top-level metadata roles")
         self.roles = roles
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Root):
             return False
 
         return (
             super().__eq__(other)
             and self.keys == other.keys
             and self.roles == other.roles
@@ -602,15 +602,15 @@
         Raises ValueError if delegated_role is not actually delegated.
         """
         if delegated_role not in self.roles:
             raise ValueError(f"Delegated role {delegated_role} not found")
 
         return self.roles[delegated_role]
 
-    def get_key(self, keyid: str) -> Key:  # noqa: D102
+    def get_key(self, keyid: str) -> Key:
         if keyid not in self.keys:
             raise ValueError(f"Key {keyid} not found")
 
         return self.keys[keyid]
 
     def get_root_verification_result(
         self,
@@ -791,15 +791,15 @@
         self.length = length
         self.hashes = hashes
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, MetaFile):
             return False
 
         return (
             self.version == other.version
             and self.length == other.length
             and self.hashes == other.hashes
@@ -908,15 +908,15 @@
         expires: Optional[datetime] = None,
         snapshot_meta: Optional[MetaFile] = None,
         unrecognized_fields: Optional[Dict[str, Any]] = None,
     ):
         super().__init__(version, spec_version, expires, unrecognized_fields)
         self.snapshot_meta = snapshot_meta or MetaFile(1)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Timestamp):
             return False
 
         return (
             super().__eq__(other) and self.snapshot_meta == other.snapshot_meta
         )
 
@@ -971,15 +971,15 @@
         expires: Optional[datetime] = None,
         meta: Optional[Dict[str, MetaFile]] = None,
         unrecognized_fields: Optional[Dict[str, Any]] = None,
     ):
         super().__init__(version, spec_version, expires, unrecognized_fields)
         self.meta = meta if meta is not None else {"targets.json": MetaFile(1)}
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Snapshot):
             return False
 
         return super().__eq__(other) and self.meta == other.meta
 
     @classmethod
     def from_dict(cls, signed_dict: Dict[str, Any]) -> "Snapshot":
@@ -1062,15 +1062,15 @@
             not isinstance(p, str) for p in path_hash_prefixes
         ):
             raise ValueError("Path_hash_prefixes must be strings")
 
         self.paths = paths
         self.path_hash_prefixes = path_hash_prefixes
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, DelegatedRole):
             return False
 
         return (
             super().__eq__(other)
             and self.name == other.name
             and self.terminating == other.terminating
@@ -1222,15 +1222,15 @@
         # have a suffix between "000" and "3ff" in hex and suffix_len will be 3
         # meaning the third bin will have a suffix of "003".
         self.number_of_bins = 2**bit_length
         # suffix_len is calculated based on "number_of_bins - 1" as the name
         # of the last bin contains the number "number_of_bins -1" as a suffix.
         self.suffix_len = len(f"{self.number_of_bins-1:x}")
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, SuccinctRoles):
             return False
 
         return (
             super().__eq__(other)
             and self.bit_length == other.bit_length
             and self.name_prefix == other.name_prefix
@@ -1282,15 +1282,15 @@
         bin_number = int.from_bytes(hash_bytes, byteorder="big") >> shift_value
         # Add zero padding if necessary and cast to hex the suffix.
         suffix = f"{bin_number:0{self.suffix_len}x}"
         return f"{self.name_prefix}-{suffix}"
 
     def get_roles(self) -> Iterator[str]:
         """Yield the names of all different delegated roles one by one."""
-        for i in range(0, self.number_of_bins):
+        for i in range(self.number_of_bins):
             suffix = f"{i:0{self.suffix_len}x}"
             yield f"{self.name_prefix}-{suffix}"
 
     def is_delegated_role(self, role_name: str) -> bool:
         """Determine whether the given ``role_name`` is in one of
         the delegated roles that ``SuccinctRoles`` represents.
 
@@ -1364,15 +1364,15 @@
         self.roles = roles
         self.succinct_roles = succinct_roles
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Delegations):
             return False
 
         all_attributes_check = (
             self.keys == other.keys
             and self.roles == other.roles
             and self.succinct_roles == other.succinct_roles
@@ -1487,22 +1487,22 @@
         self.path = path
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
     @property
-    def custom(self) -> Any:
+    def custom(self) -> Any:  # noqa: ANN401
         """Get implementation specific data related to the target.
 
         python-tuf does not use or validate this data.
         """
         return self.unrecognized_fields.get("custom")
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, TargetFile):
             return False
 
         return (
             self.length == other.length
             and self.hashes == other.hashes
             and self.path == other.path
@@ -1638,15 +1638,15 @@
         delegations: Optional[Delegations] = None,
         unrecognized_fields: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__(version, spec_version, expires, unrecognized_fields)
         self.targets = targets if targets is not None else {}
         self.delegations = delegations
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Targets):
             return False
 
         return (
             super().__eq__(other)
             and self.targets == other.targets
             and self.delegations == other.delegations
@@ -1774,14 +1774,14 @@
                 role = succinct
 
         if not role:
             raise ValueError(f"Delegated role {delegated_role} not found")
 
         return role
 
-    def get_key(self, keyid: str) -> Key:  # noqa: D102
+    def get_key(self, keyid: str) -> Key:
         if self.delegations is None:
             raise ValueError("No delegations found")
         if keyid not in self.delegations.keys:
             raise ValueError(f"Key {keyid} not found")
 
         return self.delegations.keys[keyid]
```

### Comparing `tuf-4.0.0/tuf/api/dsse.py` & `tuf-5.0.0/tuf/api/dsse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Low-level TUF DSSE API. (experimental!)"""
 
 import json
-from typing import Dict, Generic, Type, cast
+from typing import Generic, Type, cast
 
 from securesystemslib.dsse import Envelope as BaseSimpleEnvelope
 
 # Expose all payload classes to use API independently of ``tuf.api.metadata``.
 from tuf.api._payload import (  # noqa: F401
     _ROOT,
     _SNAPSHOT,
@@ -38,33 +38,26 @@
     * Sign with ``self.sign()`` (inherited).
     * Verify with ``verify_delegate`` on a ``Root`` or ``Targets``
       object::
 
         delegator.verify_delegate(
             role_name,
             envelope.pae(),  # Note, how we don't pass ``envelope.payload``!
-            envelope.signatures_dict,
+            envelope.signatures,
             )
 
     Attributes:
         payload: Serialized payload bytes.
         payload_type: Payload string identifier.
-        signatures: List of ``Signature`` objects.
-        signatures_dict: Ordered dictionary of keyids to ``Signature`` objects.
+        signatures: Ordered dictionary of keyids to ``Signature`` objects.
 
     """
 
     _DEFAULT_PAYLOAD_TYPE = "application/vnd.tuf+json"
 
-    @property
-    def signatures_dict(self) -> Dict:
-        """Convenience alias for ``self.signatures`` mapped to keyids."""
-        # TODO: Propose changing ``signatures`` list to dict upstream
-        return {sig.keyid: sig for sig in self.signatures}
-
     @classmethod
     def from_bytes(cls, data: bytes) -> "SimpleEnvelope[T]":
         """Load envelope from JSON bytes.
 
         NOTE: Unlike ``tuf.api.metadata.Metadata.from_bytes``, this method
         does not deserialize the contained payload. Use ``self.get_signed`` to
         deserialize the payload into a ``Signed`` object.
@@ -122,15 +115,15 @@
         try:
             signed_dict = signed.to_dict()
             json_bytes = json.dumps(signed_dict).encode()
 
         except Exception as e:
             raise SerializationError from e
 
-        return cls(json_bytes, cls._DEFAULT_PAYLOAD_TYPE, [])
+        return cls(json_bytes, cls._DEFAULT_PAYLOAD_TYPE, {})
 
     def get_signed(self) -> T:
         """Extract and deserialize payload JSON bytes from envelope.
 
         Raises:
             tuf.api.serialization.DeserializationError:
                 The signed object cannot be deserialized.
```

### Comparing `tuf-4.0.0/tuf/api/exceptions.py` & `tuf-5.0.0/tuf/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/api/metadata.py` & `tuf-5.0.0/tuf/api/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 import logging
 import tempfile
 from typing import Any, Dict, Generic, Optional, Type, cast
 
 from securesystemslib.signer import Signature, Signer
 from securesystemslib.storage import FilesystemBackend, StorageBackendInterface
-from securesystemslib.util import persist_temp_file
 
 # Expose payload classes via ``tuf.api.metadata`` to maintain the API,
 # even if they are unused in the local scope.
 from tuf.api._payload import (  # noqa: F401
     _ROOT,
     _SNAPSHOT,
     _TARGETS,
@@ -128,15 +127,15 @@
         self.signed: T = signed
         self.signatures = signatures if signatures is not None else {}
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Metadata):
             return False
 
         return (
             self.signatures == other.signatures
             # Order of the signatures matters (see issue #1788).
             and list(self.signatures.items()) == list(other.signatures.items())
@@ -328,34 +327,35 @@
 
         Raises:
             tuf.api.serialization.SerializationError:
                 The metadata object cannot be serialized.
             StorageError: The file cannot be written.
         """
 
+        if storage_backend is None:
+            storage_backend = FilesystemBackend()
+
         bytes_data = self.to_bytes(serializer)
 
         with tempfile.TemporaryFile() as temp_file:
             temp_file.write(bytes_data)
-            persist_temp_file(temp_file, filename, storage_backend)
+            storage_backend.put(temp_file, filename)
 
     # Signatures.
     def sign(
         self,
         signer: Signer,
         append: bool = False,
         signed_serializer: Optional[SignedSerializer] = None,
     ) -> Signature:
         """Create signature over ``signed`` and assigns it to ``signatures``.
 
         Args:
             signer: A ``securesystemslib.signer.Signer`` object that provides a
-            private key and signing implementation to generate the signature. A
-            standard implementation is available in
-            ``securesystemslib.signer.SSlibSigner``.
+                signing implementation to generate the signature.
             append: ``True`` if the signature should be appended to
                 the list of signatures or replace any existing signatures. The
                 default behavior is to replace signatures.
             signed_serializer: ``SignedSerializer`` that implements the desired
                 serialization format. Default is ``CanonicalJSONSerializer``.
 
         Raises:
```

### Comparing `tuf-4.0.0/tuf/api/serialization/__init__.py` & `tuf-5.0.0/tuf/api/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/api/serialization/json.py` & `tuf-5.0.0/tuf/api/serialization/json.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/ngclient/README.md` & `tuf-5.0.0/tuf/ngclient/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/ngclient/__init__.py` & `tuf-5.0.0/tuf/ngclient/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/ngclient/config.py` & `tuf-5.0.0/tuf/ngclient/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2021, New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """Configuration options for ``Updater`` class."""
 
 from dataclasses import dataclass
 from enum import Flag, unique
+from typing import Optional
 
 
 @unique
 class EnvelopeType(Flag):
     """Configures deserialization and verification mode of TUF metadata.
 
     Args:
@@ -35,17 +36,20 @@
             <https://theupdateframework.github.io/specification/latest/#consistent-snapshots>`_
             are used, target download URLs are formed by prefixing the filename
             with a hash digest of file content by default. This can be
             overridden by setting ``prefix_targets_with_hash`` to ``False``.
         envelope_type: Configures deserialization and verification mode of TUF
             metadata. Per default, it is treated as traditional canonical JSON
             -based TUF Metadata.
+        app_user_agent: Application user agent, e.g. "MyApp/1.0.0". This will be
+            prefixed to ngclient user agent when the default fetcher is used.
     """
 
     max_root_rotations: int = 32
     max_delegations: int = 32
     root_max_length: int = 512000  # bytes
     timestamp_max_length: int = 16384  # bytes
     snapshot_max_length: int = 2000000  # bytes
     targets_max_length: int = 5000000  # bytes
     prefix_targets_with_hash: bool = True
     envelope_type: EnvelopeType = EnvelopeType.METADATA
+    app_user_agent: Optional[str] = None
```

### Comparing `tuf-4.0.0/tuf/ngclient/fetcher.py` & `tuf-5.0.0/tuf/ngclient/fetcher.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/ngclient/updater.py` & `tuf-5.0.0/tuf/ngclient/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,26 +89,33 @@
         self._metadata_base_url = _ensure_trailing_slash(metadata_base_url)
         self.target_dir = target_dir
         if target_base_url is None:
             self._target_base_url = None
         else:
             self._target_base_url = _ensure_trailing_slash(target_base_url)
 
-        # Read trusted local root metadata
-        data = self._load_local_metadata(Root.type)
-        self._fetcher = fetcher or requests_fetcher.RequestsFetcher()
         self.config = config or UpdaterConfig()
 
+        if fetcher is not None:
+            self._fetcher = fetcher
+        else:
+            self._fetcher = requests_fetcher.RequestsFetcher(
+                app_user_agent=self.config.app_user_agent
+            )
+
         supported_envelopes = [EnvelopeType.METADATA, EnvelopeType.SIMPLE]
         if self.config.envelope_type not in supported_envelopes:
             raise ValueError(
                 f"config: envelope_type must be one of {supported_envelopes}, "
                 f"got '{self.config.envelope_type}'"
             )
 
+        # Read trusted local root metadata
+        data = self._load_local_metadata(Root.type)
+
         self._trusted_set = trusted_metadata_set.TrustedMetadataSet(
             data, self.config.envelope_type
         )
 
     def refresh(self) -> None:
         """Refresh top-level metadata.
```

### Comparing `tuf-4.0.0/tuf/ngclient/_internal/requests_fetcher.py` & `tuf-5.0.0/tuf/ngclient/_internal/requests_fetcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 # requests_fetcher is public but comes from _internal for now (because
 # sigstore-python 1.0 still uses the module from there). requests_fetcher
 # can be moved out of _internal once sigstore-python 1.0 is not relevant.
 
 import logging
-from typing import Dict, Iterator, Tuple
+from typing import Dict, Iterator, Optional, Tuple
 from urllib import parse
 
 # Imports
 import requests
 
 import tuf
 from tuf.api import exceptions
@@ -31,15 +31,18 @@
     Attributes:
         socket_timeout: Timeout in seconds, used for both initial connection
             delay and the maximum delay between bytes received.
         chunk_size: Chunk size in bytes used when downloading.
     """
 
     def __init__(
-        self, socket_timeout: int = 30, chunk_size: int = 400000
+        self,
+        socket_timeout: int = 30,
+        chunk_size: int = 400000,
+        app_user_agent: Optional[str] = None,
     ) -> None:
         # http://docs.python-requests.org/en/master/user/advanced/#session-objects:
         #
         # "The Session object allows you to persist certain parameters across
         # requests. It also persists cookies across all requests made from the
         # Session instance, and will use urllib3's connection pooling. So if
         # you're making several requests to the same host, the underlying TCP
@@ -52,14 +55,15 @@
         # hosts-scheme combinations to minimize subtle security issues.
         # Some cookies may not be HTTP-safe.
         self._sessions: Dict[Tuple[str, str], requests.Session] = {}
 
         # Default settings
         self.socket_timeout: int = socket_timeout  # seconds
         self.chunk_size: int = chunk_size  # bytes
+        self.app_user_agent = app_user_agent
 
     def _fetch(self, url: str) -> Iterator[bytes]:
         """Fetch the contents of HTTP/HTTPS url from a remote server.
 
         Args:
             url: URL string that represents a file location.
 
@@ -134,14 +138,16 @@
         session = self._sessions.get(session_index)
 
         if not session:
             session = requests.Session()
             self._sessions[session_index] = session
 
             ua = f"tuf/{tuf.__version__} {session.headers['User-Agent']}"
+            if self.app_user_agent is not None:
+                ua = f"{self.app_user_agent} {ua}"
             session.headers["User-Agent"] = ua
 
             logger.debug("Made new session %s", session_index)
         else:
             logger.debug("Reusing session %s", session_index)
 
         return session
```

### Comparing `tuf-4.0.0/tuf/ngclient/_internal/trusted_metadata_set.py` & `tuf-5.0.0/tuf/ngclient/_internal/trusted_metadata_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             if new_timestamp.version < self.timestamp.version:
                 raise exceptions.BadVersionNumberError(
                     f"New timestamp version {new_timestamp.version} must"
                     f" be >= {self.timestamp.version}"
                 )
             # Keep using old timestamp if versions are equal.
             if new_timestamp.version == self.timestamp.version:
-                raise exceptions.EqualVersionNumberError()
+                raise exceptions.EqualVersionNumberError
 
             # Prevent rolling back snapshot version
             snapshot_meta = self.timestamp.snapshot_meta
             new_snapshot_meta = new_timestamp.snapshot_meta
             if new_snapshot_meta.version < snapshot_meta.version:
                 raise exceptions.BadVersionNumberError(
                     f"New snapshot version must be >= {snapshot_meta.version}"
@@ -450,15 +450,15 @@
 
 
 def _load_from_metadata(
     role: Type[T],
     data: bytes,
     delegator: Optional[Delegator] = None,
     role_name: Optional[str] = None,
-) -> Tuple[T, bytes, Dict[str, Signature]]:  # noqa: D102
+) -> Tuple[T, bytes, Dict[str, Signature]]:
     """Load traditional metadata bytes, and extract and verify payload.
 
     If no delegator is passed, verification is skipped. Returns a tuple of
     deserialized payload, signed payload bytes, and signatures.
     """
     md = Metadata[T].from_bytes(data)
 
@@ -477,36 +477,36 @@
 
 
 def _load_from_simple_envelope(
     role: Type[T],
     data: bytes,
     delegator: Optional[Delegator] = None,
     role_name: Optional[str] = None,
-) -> Tuple[T, bytes, Dict[str, Signature]]:  # noqa: D102
+) -> Tuple[T, bytes, Dict[str, Signature]]:
     """Load simple envelope bytes, and extract and verify payload.
 
     If no delegator is passed, verification is skipped. Returns a tuple of
     deserialized payload, signed payload bytes, and signatures.
     """
 
     envelope = SimpleEnvelope[T].from_bytes(data)
 
-    if envelope.payload_type != SimpleEnvelope._DEFAULT_PAYLOAD_TYPE:
+    if envelope.payload_type != SimpleEnvelope._DEFAULT_PAYLOAD_TYPE:  # noqa: SLF001
         raise exceptions.RepositoryError(
-            f"Expected '{SimpleEnvelope._DEFAULT_PAYLOAD_TYPE}', "
+            f"Expected '{SimpleEnvelope._DEFAULT_PAYLOAD_TYPE}', "  # noqa: SLF001
             f"got '{envelope.payload_type}'"
         )
 
     if delegator:
         if role_name is None:
             role_name = role.type
         delegator.verify_delegate(
-            role_name, envelope.pae(), envelope.signatures_dict
+            role_name, envelope.pae(), envelope.signatures
         )
 
     signed = envelope.get_signed()
     if signed.type != role.type:
         raise exceptions.RepositoryError(
             f"Expected '{role.type}', got '{signed.type}'"
         )
 
-    return signed, envelope.pae(), envelope.signatures_dict
+    return signed, envelope.pae(), envelope.signatures
```

### Comparing `tuf-4.0.0/tuf/repository/__init__.py` & `tuf-5.0.0/tuf/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/tuf/repository/_repository.py` & `tuf-5.0.0/tuf/repository/_repository.py`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/LICENSE` & `tuf-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/LICENSE-MIT` & `tuf-5.0.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/README.md` & `tuf-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tuf-4.0.0/pyproject.toml` & `tuf-5.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Security",
   "Topic :: Software Development",
 ]
 dependencies = [
   "requests>=2.19.1",
-  "securesystemslib>=0.26.0,<0.32.0",
+  "securesystemslib~=1.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://theupdateframework.readthedocs.io/en/stable/"
 Homepage = "https://www.updateframework.com"
 Issues = "https://github.com/theupdateframework/python-tuf/issues"
@@ -77,52 +77,61 @@
 
 # Ruff section
 # Read more here: https://docs.astral.sh/ruff/linter/#rule-selection
 [tool.ruff]
 line-length=80
 
 [tool.ruff.lint]
-select = [
-    "A",   # flake8-builtins
-    "B",   # flake8-bugbear
-    "C4",  # flake8-comprehensions
-    "D",   # pydocstyle
-    "DTZ", # flake8-datetimez
-    "E",   # pycodestyle
-    "F",   # pyflakes
-    "I",   # isort
-    "ISC", # flake8-implicit-str-concat
-    "N",   # pep8-naming
-    "PL",  # pylint
-    "RET", # flake8-return
-    "S",   # flake8-bandit
-    "SIM", # flake8-simplify
-    "UP",  # pyupgrade
-    "W",   # pycodestyle-warning
-] 
+select = ["ALL"]
 ignore = [
+    # Rulesets we do not use at this moment
+    "COM",
+    "EM",
+    "FA",
+    "FIX",
+    "FBT",
+    "PERF",
+    "PT",
+    "PTH",
+    "TD",
+    "TRY",
+
+    # Individual rules that have been disabled
+    "ANN101", "ANN102", # nonsense, deprecated in ruff
     "D400", "D415", "D213", "D205", "D202", "D107", "D407", "D413", "D212", "D104", "D406", "D105", "D411", "D401", "D200", "D203",
-    "PLR0913", "PLR2004",
     "ISC001", # incompatible with ruff formatter
+    "PLR0913", "PLR2004",
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = [
-    "D",    # pydocstyle: no docstrings required for tests
-    "E501", # line-too-long: embedded test data in "fmt: off" blocks is ok
-    "S",    # bandit: Not running bandit on tests
+    "D",      # pydocstyle: no docstrings required for tests
+    "E501",   # line-too-long: embedded test data in "fmt: off" blocks is ok
+    "ERA001", # commented code is fine in tests
+    "RUF012", # ruff: mutable-class-default
+    "S",      # bandit: Not running bandit on tests
+    "SLF001", # private member access is ok in tests
+    "T201",   # print is ok in tests
 ]
 "examples/*/*" = [
-    "D", # pydocstyle: no docstrings required for examples
-    "S"  # bandit: Not running bandit on examples
+    "D",      # pydocstyle: no docstrings required for examples
+    "ERA001", # commented code is fine in examples
+    "INP001", # implicit package is fine in examples
+    "S",      # bandit: Not running bandit on examples
+    "T201",   # print is ok in examples
 ]
 "verify_release" = [
-    "S603", # bandit: this flags all uses of subprocess.run as vulnerable
+    "ERA001", # commented code is fine here
+    "S603",   # bandit: this flags all uses of subprocess.run as vulnerable
+    "T201",   # print is ok in verify_release
 ]
 
+[tool.ruff.lint.flake8-annotations]
+mypy-init-return = true
+
 # mypy section
 # Read more here: https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 [tool.mypy]
 warn_unused_configs = "True"
 warn_redundant_casts = "True"
 warn_unused_ignores = "True"
 warn_unreachable = "True"
```

### Comparing `tuf-4.0.0/PKG-INFO` & `tuf-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tuf
-Version: 4.0.0
+Version: 5.0.0
 Summary: A secure updater framework for Python
 Project-URL: Documentation, https://theupdateframework.readthedocs.io/en/stable/
 Project-URL: Homepage, https://www.updateframework.com
 Project-URL: Issues, https://github.com/theupdateframework/python-tuf/issues
 Project-URL: Source, https://github.com/theupdateframework/python-tuf
 Author-email: theupdateframework@googlegroups.com
 License: MIT OR Apache-2.0
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: requests>=2.19.1
-Requires-Dist: securesystemslib<0.32.0,>=0.26.0
+Requires-Dist: securesystemslib~=1.0
 Description-Content-Type: text/markdown
 
 # <img src="https://cdn.rawgit.com/theupdateframework/artwork/3a649fa6/tuf-logo.svg" height="100" valign="middle" alt="TUF"/> A Framework for Securing Software Update Systems
 
 ![Build](https://github.com/theupdateframework/python-tuf/actions/workflows/ci.yml/badge.svg)
 [![Coveralls](https://coveralls.io/repos/theupdateframework/python-tuf/badge.svg?branch=develop)](https://coveralls.io/r/theupdateframework/python-tuf?branch=develop)
 [![Docs](https://readthedocs.org/projects/theupdateframework/badge/)](https://theupdateframework.readthedocs.io/)
```

