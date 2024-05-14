# Comparing `tmp/in_toto-2.3.0.tar.gz` & `tmp/in_toto-3.0.0.tar.gz`

## Comparing `in_toto-2.3.0.tar` & `in_toto-3.0.0.tar`

### file list

```diff
@@ -1,134 +1,126 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-2.3.0/.coveragerc
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-build.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-dev.txt
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-docs.txt
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-lint.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-pinned.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements-test.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-2.3.0/requirements.txt
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 in_toto-2.3.0/tox.ini
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/__init__.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/common_args.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/exceptions.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/formats.py
--rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_match_products.py
--rwxr-xr-x   0        0        0     3843 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_mock.py
--rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_record.py
--rwxr-xr-x   0        0        0    10440 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_run.py
--rw-r--r--   0        0        0    13185 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_sign.py
--rwxr-xr-x   0        0        0     9784 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/in_toto_verify.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/log.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/rulelib.py
--rw-r--r--   0        0        0    40377 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/runlib.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/settings.py
--rw-r--r--   0        0        0    56646 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/verifylib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/__init__.py
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/_signer.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/common.py
--rw-r--r--   0        0        0    23587 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/layout.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/link.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/models/metadata.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/resolver/__init__.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 in_toto-2.3.0/in_toto/resolver/_resolver.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/common.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/runtests.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_common_args.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_directory_resolver.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_match_products.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_mock.py
--rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_record.py
--rwxr-xr-x   0        0        0    19109 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_run.py
--rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_sign.py
--rwxr-xr-x   0        0        0    19690 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_in_toto_verify.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_log.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_ostree_resolver.py
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_param_substitution.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_resolver.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_rulelib.py
--rwxr-xr-x   0        0        0    52785 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_runlib.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_settings.py
--rw-r--r--   0        0        0    69111 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/test_verifylib.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/demo.layout.template
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/package.2f89b927.link
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_dsse_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/alice
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/alice.pub
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/bob
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/bob.pub
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/carl
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/carl.pub
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/danny
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/danny.pub
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/foo.tar.gz
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/package.2f89b927.link
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/foo.tar.gz
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/package.7b3abb26.link
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/demo_files_gpg/write-code.8288ef56.link
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/__init__.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_common.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_envelope.py
--rwxr-xr-x   0        0        0     1967 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_inspection.py
--rwxr-xr-x   0        0        0    14784 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_layout.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_link.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_metadata.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_signer.py
--rwxr-xr-x   0        0        0     2864 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_step.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/models/test_supply_chain_item.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_private_encrypted.pem
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_private_unencrypted.pem
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ecdsa_public.pem
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_private_encrypted.pem
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_private_unencrypted.pem
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/ed25519_public.pem
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_private_encrypted.pem
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_private_unencrypted.pem
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/pems/rsa_public.pem
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/rc_test/.in_totorc
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/colliding_dir_resolver/subdir/0.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/README.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/0.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/1.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/Y.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/Z.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/a.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/dir_resolver/subdir/b.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/config
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/04/d3e76d327333f3a5fcfb2fd067b90cc36a906d23db28adb3819e02e99f0f6a.dirtree
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/17/57d5e638ba33b5b43bee22ad24f8eecd14487965c076225664e64787a772c4.file
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/46/33304404a9fb8b9c98145aa85851d285b491e3b77e9cef663392857c4b1000.file
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/57/3c8b6ed22f77d085206364b0fca4334ab88c429a4e3d335f9b863ca421adc6.dirtree
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/6d/f05c195832bd23b044a3fdd76b3a30011c762dea6c271133cb20f7309abcb5.dirtree
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/6e/340b9cffb37a989ca544e6bb780a2c78901d3fb33738768511a30617afa01d.dirtree
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/77/3e0833bada391e17908ef72be2f3bab9662b6223b5cd6064af8ce7753368d1.dirtree
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/85/b69cc1ae509c55992d4eb47572cebb0fcfdf640aa2cdc0ad4b517cb6cf8b5d.dirtree
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/a6/1f97fffc19dbe77a59de47641b16a03a6a835cbe3d7f8a86f4fbb85342b551.file
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/cd/1875c7cb1d1c169f4ae48baee61c00d1be51efe0f0c2777759644e3a62012f.dirmeta
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/cf/3e103a6aed64aec261e2161d1026aa26349d422d238b1ad9e2e2a7eeed8591.commit
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/e3/777ae4075244944a952fa9705d5b26fa24cf5a841e7ce278f390ee3fc1928b.dirtree
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/f3/43cfdc0f6c428bdb30fc0dbf6c230972564153579b68e5fe5261444cf65abe.file
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/objects/f7/d5cf77d40b20cbf35b0de40a6bc693d13afeac5c1e07b63f71754e0d6704a2.dirtree
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/resolver/ostree_repo/refs/heads/test-branch
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/expr
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/tar
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-2.3.0/tests/scripts/touch
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-2.3.0/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-2.3.0/LICENSE
--rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 in_toto-2.3.0/README.md
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 in_toto-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 in_toto-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-3.0.0/.coveragerc
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-build.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-docs.txt
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-lint.txt
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-pinned.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements-test.txt
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 in_toto-3.0.0/requirements.txt
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 in_toto-3.0.0/tox.ini
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/common_args.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/exceptions.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/formats.py
+-rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_match_products.py
+-rwxr-xr-x   0        0        0     3843 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_mock.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_record.py
+-rwxr-xr-x   0        0        0     9801 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_run.py
+-rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_sign.py
+-rwxr-xr-x   0        0        0     8090 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/in_toto_verify.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/log.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/rulelib.py
+-rw-r--r--   0        0        0    38704 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/runlib.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/settings.py
+-rw-r--r--   0        0        0    56648 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/verifylib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/__init__.py
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/_signer.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/common.py
+-rw-r--r--   0        0        0    23593 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/layout.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/link.py
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/models/metadata.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/resolver/__init__.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 in_toto-3.0.0/in_toto/resolver/_resolver.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/common.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/runtests.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_common_args.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_directory_resolver.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_match_products.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_mock.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_record.py
+-rwxr-xr-x   0        0        0    15298 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_run.py
+-rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_sign.py
+-rwxr-xr-x   0        0        0     7441 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_in_toto_verify.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_log.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_ostree_resolver.py
+-rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_param_substitution.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_resolver.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_rulelib.py
+-rwxr-xr-x   0        0        0    51054 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_runlib.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0    69119 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/test_verifylib.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_dsse_files/demo.layout.template
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_dsse_files/package.2f89b927.link
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_dsse_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files/foo.tar.gz
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files/package.2f89b927.link
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files_gpg/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files_gpg/foo.tar.gz
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files_gpg/package.7b3abb26.link
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/demo_files_gpg/write-code.8288ef56.link
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/__init__.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_common.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_envelope.py
+-rwxr-xr-x   0        0        0     1967 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_inspection.py
+-rwxr-xr-x   0        0        0    13672 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_layout.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_link.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_metadata.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_signer.py
+-rwxr-xr-x   0        0        0     2864 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_step.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/models/test_supply_chain_item.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ecdsa_private_encrypted.pem
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ecdsa_private_unencrypted.pem
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ecdsa_public.pem
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ed25519_private_encrypted.pem
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ed25519_private_unencrypted.pem
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/ed25519_public.pem
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/rsa_private_encrypted.pem
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/rsa_private_unencrypted.pem
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/pems/rsa_public.pem
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/rc_test/.in_totorc
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/colliding_dir_resolver/subdir/0.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/README.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/0.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/1.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/Y.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/Z.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/a.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/dir_resolver/subdir/b.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/config
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/04/d3e76d327333f3a5fcfb2fd067b90cc36a906d23db28adb3819e02e99f0f6a.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/17/57d5e638ba33b5b43bee22ad24f8eecd14487965c076225664e64787a772c4.file
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/46/33304404a9fb8b9c98145aa85851d285b491e3b77e9cef663392857c4b1000.file
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/57/3c8b6ed22f77d085206364b0fca4334ab88c429a4e3d335f9b863ca421adc6.dirtree
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/6d/f05c195832bd23b044a3fdd76b3a30011c762dea6c271133cb20f7309abcb5.dirtree
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/6e/340b9cffb37a989ca544e6bb780a2c78901d3fb33738768511a30617afa01d.dirtree
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/77/3e0833bada391e17908ef72be2f3bab9662b6223b5cd6064af8ce7753368d1.dirtree
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/85/b69cc1ae509c55992d4eb47572cebb0fcfdf640aa2cdc0ad4b517cb6cf8b5d.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/a6/1f97fffc19dbe77a59de47641b16a03a6a835cbe3d7f8a86f4fbb85342b551.file
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/cd/1875c7cb1d1c169f4ae48baee61c00d1be51efe0f0c2777759644e3a62012f.dirmeta
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/cf/3e103a6aed64aec261e2161d1026aa26349d422d238b1ad9e2e2a7eeed8591.commit
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/e3/777ae4075244944a952fa9705d5b26fa24cf5a841e7ce278f390ee3fc1928b.dirtree
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/f3/43cfdc0f6c428bdb30fc0dbf6c230972564153579b68e5fe5261444cf65abe.file
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/objects/f7/d5cf77d40b20cbf35b0de40a6bc693d13afeac5c1e07b63f71754e0d6704a2.dirtree
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/resolver/ostree_repo/refs/heads/test-branch
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/scripts/expr
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/scripts/tar
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-3.0.0/tests/scripts/touch
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-3.0.0/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-3.0.0/LICENSE
+-rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 in_toto-3.0.0/README.md
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 in_toto-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 in_toto-3.0.0/PKG-INFO
```

### Comparing `in_toto-2.3.0/tox.ini` & `in_toto-3.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     coverage report -m --fail-under 99
 
 
 # Develop test env to run tests against securesystemslib's main branch
 # Must to be invoked explicitly with, e.g. `tox -e with-sslib-main`
 [testenv:with-sslib-main]
 commands_pre =
-    pip install --force-reinstall git+https://github.com/secure-systems-lab/securesystemslib.git@main#egg=securesystemslib[crypto,pynacl]
+    pip install --force-reinstall git+https://github.com/secure-systems-lab/securesystemslib.git@main#egg=securesystemslib[crypto]
 
 commands =
     coverage run tests/runtests.py
     coverage report -m
 
 
 [testenv:lint]
```

### Comparing `in_toto-2.3.0/in_toto/common_args.py` & `in_toto-3.0.0/in_toto/common_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,20 +26,14 @@
   parser = argparse.ArgumentParser()
   parser.add_argument(*EXCLUDE_KWARGS, **EXCLUDE_KWARGS)
   ```
 
 """
 import sys
 
-from in_toto import (
-    KEY_TYPE_ECDSA,
-    KEY_TYPE_ED25519,
-    KEY_TYPE_RSA,
-    SUPPORTED_KEY_TYPES,
-)
 from in_toto.settings import LINK_CMD_EXEC_TIMEOUT
 
 EXCLUDE_ARGS = ["--exclude"]
 EXCLUDE_KWARGS = {
     "dest": "exclude_patterns",
     "required": False,
     "metavar": "<pattern>",
@@ -76,49 +70,21 @@
         " them to the resulting link metadata. If multiple prefixes are"
         " specified, only a single prefix can match the path of any"
         " artifact and that is then left-stripped. All prefixes are checked"
         " to ensure none of them are a left substring of another."
     ),
 }
 
-KEY_ARGS = ["-k", "--key"]
-KEY_KWARGS = {
-    "type": str,
-    "metavar": "<path>",
-    "help": (
-        "path to a private key file to sign the resulting link metadata."
-        " The keyid prefix is used as an infix for the link metadata"
-        " filename, i.e. '<name>.<keyid prefix>.link'. See '--key-type' for"
-        " available formats. Passing one of '--key' or '--gpg' is required."
-    ),
-}
-
-KEY_TYPE_ARGS = ["-t", "--key-type"]
-KEY_TYPE_KWARGS = {
-    "dest": "key_type",
-    "type": str,
-    "choices": SUPPORTED_KEY_TYPES,
-    "default": KEY_TYPE_RSA,
-    "help": (
-        "type of key specified by the '--key' option. '{rsa}' keys are"
-        " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are"
-        " expected to be in a custom 'securesystemslib/json' format."
-        " Default is '{rsa}'.".format(
-            rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
-        )
-    ),
-}
-
 KEY_PASSWORD_ARGS = ["-P", "--password"]
 KEY_PASSWORD_KWARGS = {
     "nargs": "?",
     "const": True,
     "metavar": "<password>",
     "help": (
-        "password for encrypted key specified with '--key'. Passing  '-P'"
+        "password for encrypted key specified with '--signing-key'. Passing '-P'"
         " without <password> opens a prompt. If no password is passed, or"
         " entered on the prompt, the key is treated as unencrypted. (Do "
         " not confuse with '-p/--products'!)"
     ),
 }
 OPTS_TITLE = "Optional Arguments" if sys.version_info < (3, 10) else "Options"
 
@@ -142,15 +108,15 @@
     "nargs": "?",
     "const": True,
     "metavar": "<id>",
     "help": (
         "GPG keyid to sign the resulting link metadata.  When '--gpg' is"
         " passed without the keyid, the default GPG key is used. The keyid"
         " prefix is used as an infix for the link metadata filename, i.e."
-        " '<name>.<keyid prefix>.link'. Passing one of '--key' or '--gpg'"
+        " '<name>.<keyid prefix>.link'. Passing one of '--signing-key' or '--gpg'"
         " is required."
     ),
 }
 
 GPG_HOME_ARGS = ["--gpg-home"]
 GPG_HOME_KWARGS = {
     "dest": "gpg_home",
@@ -165,18 +131,17 @@
 
 SIGNING_KEY_ARGS = ["--signing-key"]
 SIGNING_KEY_KWARGS = {
     "type": str,
     "metavar": "<path>",
     "dest": "signing_key",
     "help": (
-        "replacement for '--key' using a standard PKCS8/PEM format. Key type is"
-        " detected automatically and need not be specified with '--key-type'."
-        " Use '--password [<password>]' to pass a decryption password"
-        " or toggle a prompt, if the key es encrypted."
+        "signing key in a standard PKCS8/PEM format. Supported keytypes are"
+        " rsa, ed25519, ecdsa (nistp256). Use '--password [<password>]' to pass"
+        " a decryption password or toggle a prompt, if the key is encrypted."
     ),
 }
 
 VERBOSE_ARGS = ["-v", "--verbose"]
 VERBOSE_KWARGS = {
     "dest": "verbose",
     "action": "store_true",
```

### Comparing `in_toto-2.3.0/in_toto/exceptions.py` & `in_toto-3.0.0/in_toto/exceptions.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/formats.py` & `in_toto-3.0.0/in_toto/formats.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,17 +123,7 @@
 
 def _check_public_keys(arg):
     """Check dict of public key dicts."""
     _check_dict(arg)
     for k, v in arg.items():
         _check_hex(k)
         _check_public_key(v)
-
-
-def _check_signing_key(arg):
-    """Check legacy signing key dict format.
-
-    NOTE: signing key dict is deprecated, this check will be removed with it
-    """
-    _check_public_key(arg)
-    if not arg["keyval"].get("private"):
-        raise _err(arg, "private key data")
```

### Comparing `in_toto-2.3.0/in_toto/in_toto_match_products.py` & `in_toto-3.0.0/in_toto/in_toto_match_products.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/in_toto_mock.py` & `in_toto-3.0.0/in_toto/in_toto_mock.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/in_toto_record.py` & `in_toto-3.0.0/in_toto/in_toto_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,35 +27,29 @@
 
 """
 import argparse
 import logging
 import sys
 from getpass import getpass
 
-from securesystemslib import interface
-
 import in_toto.runlib
 from in_toto import __version__
 from in_toto.common_args import (
     BASE_PATH_ARGS,
     BASE_PATH_KWARGS,
     DSSE_ARGS,
     DSSE_KWARGS,
     EXCLUDE_ARGS,
     EXCLUDE_KWARGS,
     GPG_ARGS,
     GPG_HOME_ARGS,
     GPG_HOME_KWARGS,
     GPG_KWARGS,
-    KEY_ARGS,
-    KEY_KWARGS,
     KEY_PASSWORD_ARGS,
     KEY_PASSWORD_KWARGS,
-    KEY_TYPE_ARGS,
-    KEY_TYPE_KWARGS,
     LSTRIP_PATHS_ARGS,
     LSTRIP_PATHS_KWARGS,
     METADATA_DIRECTORY_ARGS,
     METADATA_DIRECTORY_KWARGS,
     OPTS_TITLE,
     QUIET_ARGS,
     QUIET_KWARGS,
@@ -87,31 +81,31 @@
 
     parser.epilog = """EXAMPLE USAGE
 
 Create link metadata file in two commands, signing it with the private key
 loaded from 'key_file', recording all files in the CWD as materials (on
 start), and as products (on stop).
 
-  {prog} start -n edit-files -k path/to/key_file -m .
-  {prog} stop -n edit-files -k path/to/key_file -p .
+  {prog} start -n edit-files --signing-key path/to/key_file -m .
+  {prog} stop -n edit-files --signing-key path/to/key_file -p .
 
 
 Create link metadata file signed with the default GPG key from the default
 GPG home directory and record a file named 'foo' as material and product.
 
   {prog} start -n edit-foo --gpg -m path/to/foo
   {prog} stop -n edit-foo --gpg -p path/to/foo
 
 
 Create link metadata file signed with the private key loaded from 'key_file',
 record all files in the CWD as material and product, and dump finished link
 file to the target directory (on stop).
 
-  {prog} start -n edit-files -k path/to/key_file -m .
-  {prog} stop -d path/to/target/dir -n edit-files -k path/to/key_file -p .
+  {prog} start -n edit-files --signing-key path/to/key_file -m .
+  {prog} stop -d path/to/target/dir -n edit-files --signing-key path/to/key_file -p .
 
 """.format(
         prog=parser.prog
     )
 
     # The subparsers inherit the arguments from the parent parser
     parent_parser = argparse.ArgumentParser(add_help=False)
@@ -134,16 +128,14 @@
         metavar="<name>",
         help=(
             "name for the resulting link metadata file. It is also used to associate"
             " the link with a step defined in an in-toto layout."
         ),
     )
 
-    parent_named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
-    parent_parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
     parent_parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
 
     parent_named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
     parent_parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
 
     parent_named_args.add_argument(*SIGNING_KEY_ARGS, **SIGNING_KEY_KWARGS)
 
@@ -234,48 +226,33 @@
     on the specified subcommand."""
 
     parser = create_parser()
     args = parser.parse_args()
 
     LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
 
-    # Use exactly one of legacy key, gpg or pkcs8 signing key
-    if sum([bool(args.key), bool(args.gpg), bool(args.signing_key)]) != 1:
+    # Use exactly one of gpg or pkcs8 signing key
+    if sum([bool(args.gpg), bool(args.signing_key)]) != 1:
         parser.print_usage()
         parser.error(
-            "Specify exactly one of '--key <key path>', "
-            "--gpg [<keyid>]' or --signing-key <key path>"
+            "Specify either '--signing-key <path>' or '--gpg [<keyid>]'"
         )
 
     password, prompt = parse_password_and_prompt_args(args)
 
     # If `--gpg` was set without argument it has the value `True` and
     # we will try to sign with the default key
     gpg_use_default = args.gpg is True
 
     # Otherwise gpg_keyid stays either None or gets the passed argument assigned
     gpg_keyid = None
     if not gpg_use_default and args.gpg:
         gpg_keyid = args.gpg
 
     try:
-        # We load the key here because it might prompt the user for a password in
-        # case the key is encrypted. Something that should not happen in the lib.
-        key = None
-        if args.key:
-            LOG.warning(
-                "'-k', '--key' is deprecated, use '--signing-key' instead."
-            )
-            key = interface.import_privatekey_from_file(
-                args.key,
-                key_type=args.key_type,
-                password=password,
-                prompt=prompt,
-            )
-
         signer = None
         if args.signing_key:
             if prompt:
                 password = getpass()
 
             if password is not None:
                 password = password.encode()
@@ -284,15 +261,14 @@
                 args.signing_key, password
             )
 
         if args.command == "start":
             in_toto.runlib.in_toto_record_start(
                 args.step_name,
                 args.materials,
-                signing_key=key,
                 gpg_keyid=gpg_keyid,
                 gpg_use_default=gpg_use_default,
                 gpg_home=args.gpg_home,
                 exclude_patterns=args.exclude_patterns,
                 base_path=args.base_path,
                 lstrip_paths=args.lstrip_paths,
                 use_dsse=args.use_dsse,
@@ -300,15 +276,14 @@
             )
 
         # Mutually exclusiveness is guaranteed by argparser
         else:  # args.command == "stop":
             in_toto.runlib.in_toto_record_stop(
                 args.step_name,
                 args.products,
-                signing_key=key,
                 gpg_keyid=gpg_keyid,
                 gpg_use_default=gpg_use_default,
                 gpg_home=args.gpg_home,
                 exclude_patterns=args.exclude_patterns,
                 base_path=args.base_path,
                 lstrip_paths=args.lstrip_paths,
                 metadata_directory=args.metadata_directory,
```

### Comparing `in_toto-2.3.0/in_toto/in_toto_run.py` & `in_toto-3.0.0/in_toto/in_toto_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,34 +27,28 @@
 """
 
 import argparse
 import logging
 import sys
 from getpass import getpass
 
-from securesystemslib import interface
-
 from in_toto import __version__, runlib
 from in_toto.common_args import (
     BASE_PATH_ARGS,
     BASE_PATH_KWARGS,
     DSSE_ARGS,
     DSSE_KWARGS,
     EXCLUDE_ARGS,
     EXCLUDE_KWARGS,
     GPG_ARGS,
     GPG_HOME_ARGS,
     GPG_HOME_KWARGS,
     GPG_KWARGS,
-    KEY_ARGS,
-    KEY_KWARGS,
     KEY_PASSWORD_ARGS,
     KEY_PASSWORD_KWARGS,
-    KEY_TYPE_ARGS,
-    KEY_TYPE_KWARGS,
     LSTRIP_PATHS_ARGS,
     LSTRIP_PATHS_KWARGS,
     METADATA_DIRECTORY_ARGS,
     METADATA_DIRECTORY_KWARGS,
     OPTS_TITLE,
     QUIET_ARGS,
     QUIET_KWARGS,
@@ -96,15 +90,15 @@
     )
 
     parser.epilog = """EXAMPLE USAGE
 
 Tag a git repo, storing files in CWD as products, signing the resulting link
 file with the private key loaded from 'key_file'.
 
-  {prog} -n tag -p . -k key_file -- git tag v1.0
+  {prog} -n tag -p . --signing-key key_file -- git tag v1.0
 
 
 Create a tarball, storing files in 'project' directory as materials and the
 tarball as product, signing the link file with a GPG key '...7E0C8A17'.
 
   {prog} -n package -m project -p project.tar.gz \\
          -g 8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17 \\
@@ -112,31 +106,31 @@
 
 
 Not all supply chain steps require that a command be executed. in-toto can
 still generate signed attestations, e.g. for review work. In that case, files
 may be marked as materials for the manual review process and the command be
 omitted.
 
-  {prog} -n review -k key_file -m document.pdf -x
+  {prog} -n review --signing-key key_file -m document.pdf -x
 
 
 If an artifact that should be recorded is not in the current working directory
 (or one of its subdirectories) it can be located using the base path option.
 Note that in this example only the relative path, 'document.pdf' is stored
 along with its hash in the resulting link metadata file.
 
-  {prog} -n review -k key_file -m document.pdf \\
+  {prog} -n review --signing-key key_file -m document.pdf \\
          --base-path /my/review/docs/ -x
 
 
 Similarly, it is possible to pass the full path to the artifact that should
 be recorded together with a left-strip path, to only store a relative path,
 e.g. 'document.pdf'.
 
-  {prog} -n review -k key_file \\
+  {prog} -n review --signing-key key_file \\
          -m /tmp/my/review/docs/document.pdf \\
          --lstrip-paths /tmp/my/review/docs/ -x
 
 
 """.format(
         prog=parser.prog
     )
@@ -206,16 +200,14 @@
         action="store_true",
         help=(
             "generate link metadata without executing a command, e.g. for a"
             " signed-off-by step."
         ),
     )
 
-    named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
-    parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
     parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
 
     named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
     parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
 
     named_args.add_argument(*SIGNING_KEY_ARGS, **SIGNING_KEY_KWARGS)
 
@@ -258,20 +250,19 @@
     """Parse arguments, load key from disk (prompts for password if key is
     encrypted) and call in_toto_run."""
     parser = create_parser()
     args = parser.parse_args()
 
     LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
 
-    # Use exactly one of legacy key, gpg or pkcs8 signing key
-    if sum([bool(args.key), bool(args.gpg), bool(args.signing_key)]) != 1:
+    # Use exactly one of gpg or pkcs8 signing key
+    if sum([bool(args.gpg), bool(args.signing_key)]) != 1:
         parser.print_usage()
         parser.error(
-            "Specify exactly one of '--key <key path>', "
-            "--gpg [<keyid>]' or --signing-key <key path>"
+            "Specify either '--signing-key <path>' or '--gpg [<keyid>]'"
         )
 
     password, prompt = parse_password_and_prompt_args(args)
 
     # If `--gpg` was set without argument it has the value `True` and
     # we will try to sign with the default key
     gpg_use_default = args.gpg is True
@@ -291,27 +282,14 @@
             "No command specified."
             " Please specify (or use the --no-command option)"
         )
 
     try:
         # We load the key here because it might prompt the user for a password in
         # case the key is encrypted. Something that should not happen in the lib.
-        key = None
-        if args.key:
-            LOG.warning(
-                "'-k', '--key' is deprecated, use '--signing-key' instead."
-            )
-
-            key = interface.import_privatekey_from_file(
-                args.key,
-                key_type=args.key_type,
-                password=password,
-                prompt=prompt,
-            )
-
         signer = None
         if args.signing_key:
             if prompt:
                 password = getpass()
 
             if password is not None:
                 password = password.encode()
@@ -322,15 +300,14 @@
 
         runlib.in_toto_run(
             args.step_name,
             args.materials,
             args.products,
             args.link_cmd,
             record_streams=args.record_streams,
-            signing_key=key,
             gpg_keyid=gpg_keyid,
             gpg_use_default=gpg_use_default,
             gpg_home=args.gpg_home,
             exclude_patterns=args.exclude_patterns,
             base_path=args.base_path,
             lstrip_paths=args.lstrip_paths,
             metadata_directory=args.metadata_directory,
```

### Comparing `in_toto-2.3.0/in_toto/in_toto_sign.py` & `in_toto-3.0.0/in_toto/in_toto_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 """
 import argparse
 import logging
 import sys
 from getpass import getpass
 
-from securesystemslib.gpg import functions as gpg_interface
+from securesystemslib._gpg import functions as gpg_interface
 
 from in_toto import __version__, exceptions
 from in_toto.common_args import (
     GPG_HOME_ARGS,
     GPG_HOME_KWARGS,
     QUIET_ARGS,
     QUIET_KWARGS,
@@ -68,15 +68,15 @@
       SystemExit(0) if signing is successful
       SystemExit(2) if any exception occurs
 
     """
 
     try:
         if not args.append:
-            metadata.signatures = []
+            metadata.signatures.clear()
 
         signature = None
         # If the cli tool was called with `--gpg [KEYID ...]` `args.gpg` is
         # a list (not None) and we will try to sign with gpg.
         # If `--gpg-home` was not set, args.gpg_home is None and the signer tries
         # to use the default gpg keyring.
         if args.gpg is not None:
```

### Comparing `in_toto-2.3.0/in_toto/in_toto_verify.py` & `in_toto-3.0.0/in_toto/in_toto_verify.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,25 +25,17 @@
   0 if no exception occurred (verification passed)
 
 """
 import argparse
 import logging
 import sys
 
-from securesystemslib import interface
-from securesystemslib.gpg import functions as gpg_interface
+from securesystemslib._gpg import functions as gpg_interface
 
-from in_toto import (
-    KEY_TYPE_ECDSA,
-    KEY_TYPE_ED25519,
-    KEY_TYPE_RSA,
-    SUPPORTED_KEY_TYPES,
-    __version__,
-    verifylib,
-)
+from in_toto import __version__, verifylib
 from in_toto.common_args import (
     GPG_HOME_ARGS,
     GPG_HOME_KWARGS,
     OPTS_TITLE,
     QUIET_ARGS,
     QUIET_KWARGS,
     VERBOSE_ARGS,
@@ -103,21 +95,21 @@
     parser.usage = "%(prog)s <named arguments> [{}]".format(OPTS_TITLE.lower())
 
     parser.epilog = """EXAMPLE USAGE
 
 Verify supply chain in 'root.layout', signed with private part of
 'key_file.pub'.
 
-  {prog} --layout root.layout --layout-keys key_file.pub
+  {prog} --layout root.layout --verification-keys key_file.pub
 
 
 Verify supply chain as above but load links corresponding to steps of
 'root.layout' from 'link_dir'.
 
-  {prog} --layout root.layout --layout-keys key_file.pub \\
+  {prog} --layout root.layout --verification-keys key_file.pub \\
       --link-dir link_dir
 
 
 Verify supply chain in 'root.layout', signed with GPG key '...7E0C8A17',
 for which the public part can be found in the GPG keyring at '~/.gnupg'.
 
   {prog} --layout root.layout \\
@@ -138,71 +130,38 @@
         required=True,
         metavar="<path>",
         help=(
             "path to root layout specifying the software supply chain to be"
             " verified."
         ),
     )
-
-    named_args.add_argument(
-        "-k",
-        "--layout-keys",
-        type=str,
-        metavar="<path>",
-        nargs="+",
-        help=(
-            "paths to public key files used to verify the passed root layout's"
-            " signatures. See '--key-types' for available formats. Passing at least"
-            " one key using '--layout-keys' and/or '--gpg' is required. For each"
-            " passed key the layout must carry a valid signature."
-        ),
-    )
-
-    parser.add_argument(
-        "-t",
-        "--key-types",
-        dest="key_types",
-        type=str,
-        choices=SUPPORTED_KEY_TYPES,
-        nargs="+",
-        help=(
-            "types of keys specified by the '--layout-keys' option. '{rsa}' keys are"
-            " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are expected"
-            " in a custom 'securesystemslib/json' format. If multiple keys are"
-            " passed via '--layout-keys' the same amount of key types must be"
-            " passed. Key types are then associated with keys by index. If"
-            " '--key-types' is omitted, the default of '{rsa}' is used for all"
-            " keys.".format(
-                rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
-            )
-        ),
-    )
-
     named_args.add_argument(
         "--verification-keys",
         type=str,
         dest="verification_keys",
         metavar="<path>",
         nargs="+",
         help=(
-            "replacement for '--layout-keys' using a standard "
-            "subjectPublicKeyInfo/PEM format. Key type is detected "
-            "automatically and need not be specified with '--key-type'."
+            "paths to public key files used to verify the passed root layout's"
+            " signatures. Supported keytypes are rsa, ed25519, ecdsa (nistp256)"
+            " in a standard subjectPublicKeyInfo/PEM format. Passing at least"
+            " one key using '--verification-keys' and/or '--gpg' is required."
+            " For each passed key the layout must carry a valid signature."
         ),
     )
 
     named_args.add_argument(
         "-g",
         "--gpg",
         nargs="+",
         metavar="<id>",
         help=(
             "GPG keyid, identifying a public key in the GPG keyring used to verify"
             " the passed root layout's signatures."
-            " Passing at least one key using '--layout-keys' and/or '--gpg' is"
+            " Passing at least one key using '--verification-keys' and/or '--gpg' is"
             " required. For each passed key the layout must carry a valid"
             " signature."
         ),
     )
 
     parser.add_argument(
         "--link-dir",
@@ -252,40 +211,26 @@
     """Parse arguments and call in_toto_verify."""
     parser = create_parser()
     args = parser.parse_args()
 
     LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
 
     # For verifying at least one public key must be specified
-    if not (args.layout_keys or args.gpg or args.verification_keys):
+    if not (args.gpg or args.verification_keys):
         parser.print_help()
         parser.error(
             "wrong arguments: specify at least one layout verification key:"
-            " '--layout-keys path [path ...]' or  '--gpg id [id ...]' or "
-            " '--verification-keys path [path ...]'."
+            " '--verification-keys path [path ...]' and/or '--gpg id [id ...]'."
         )
 
     try:
         LOG.info("Loading layout...")
         layout = Metadata.load(args.layout)
 
         layout_key_dict = {}
-        if args.layout_keys is not None:
-            LOG.info("Loading layout key(s)...")
-            LOG.warning(
-                "'-k', '--layout-keys' is deprecated, use "
-                "'--verification-keys' instead."
-            )
-
-            layout_key_dict.update(
-                interface.import_publickeys_from_file(
-                    args.layout_keys, args.key_types
-                )
-            )
-
         if args.gpg is not None:
             LOG.info("Loading layout gpg key(s)...")
             layout_key_dict.update(
                 gpg_interface.export_pubkeys(args.gpg, homedir=args.gpg_home)
             )
 
         if args.verification_keys:
```

### Comparing `in_toto-2.3.0/in_toto/log.py` & `in_toto-3.0.0/in_toto/log.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/rulelib.py` & `in_toto-3.0.0/in_toto/rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/runlib.py` & `in_toto-3.0.0/in_toto/runlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,28 +33,23 @@
 import os
 import subprocess  # nosec
 import sys
 import tempfile
 import time
 from collections import defaultdict
 
+import securesystemslib._gpg
 import securesystemslib.exceptions
 import securesystemslib.formats
-import securesystemslib.gpg
 import securesystemslib.hash
-from securesystemslib.signer import Key, Signature, Signer, SSlibSigner
+from securesystemslib.signer import Signer
 
 import in_toto.exceptions
 import in_toto.settings
-from in_toto.formats import (
-    _check_hex,
-    _check_signing_key,
-    _check_str,
-    _check_str_list,
-)
+from in_toto.formats import _check_hex, _check_str, _check_str_list
 from in_toto.models._signer import GPGSigner
 from in_toto.models.link import (
     FILENAME_FORMAT,
     FILENAME_FORMAT_SHORT,
     UNFINISHED_FILENAME_FORMAT,
     UNFINISHED_FILENAME_FORMAT_GLOB,
 )
@@ -395,37 +390,28 @@
     return link_metadata
 
 
 def _check_signer(signer):
     if not isinstance(signer, Signer):
         raise ValueError("signer must be a Signer instance")
 
-    if not (
-        hasattr(signer, "public_key") and isinstance(signer.public_key, Key)
-    ):
-        # TODO: add `public_key` to `Signer` interface upstream
-        # see secure-systems-lab/securesystemslib#605
-        raise ValueError("only Signer instances with public key supported")
-
 
-def _require_signing_arg(signer, signing_key, gpg_keyid, gpg_use_default):
-    if not any([signer, signing_key, gpg_keyid, gpg_use_default]):
+def _require_signing_arg(signer, gpg_keyid, gpg_use_default):
+    if not any([signer, gpg_keyid, gpg_use_default]):
         raise ValueError(
-            "Pass either a signer, a signing key, a gpg keyid or set"
-            " gpg_use_default to True!"
+            "Pass either a signer, a gpg keyid or set gpg_use_default to True!"
         )
 
 
 def in_toto_run(
     name,
     material_list,
     product_list,
     link_cmd_args,
     record_streams=False,
-    signing_key=None,
     gpg_keyid=None,
     gpg_use_default=False,
     gpg_home=None,
     exclude_patterns=None,
     base_path=None,
     compact_json=False,
     record_environment=False,
@@ -436,15 +422,15 @@
     timeout=in_toto.settings.LINK_CMD_EXEC_TIMEOUT,
     signer=None,
 ):
     """Performs a supply chain step or inspection generating link metadata.
 
   Executes link_cmd_args, recording paths and hashes of files before and after
   command execution (aka. artifacts) in a link metadata file. The metadata is
-  signed with the passed signer, signing_key, a gpg key identified by its ID, or
+  signed with the passed signer, a gpg key identified by its ID, or
   the default gpg key. If multiple key arguments are passed, only one key is
   used in above order of precedence. The resulting link file is written to
   ``STEP-NAME.KEYID-PREFIX.link``. If no key argument is passed the link
   metadata is neither signed nor written to disk.
 
   Arguments:
     name: A unique name to associate link metadata with a step or inspection.
@@ -458,19 +444,14 @@
     link_cmd_args: A list where the first element is a command and the
         remaining elements are arguments passed to that command.
 
     record_streams (optional): A boolean indicating if standard output and
         standard error of the link command should be recorded in the link
         metadata in addition to being displayed while the command is executed.
 
-    signing_key (optional): A key used to sign the resulting link metadata.
-
-        .. deprecated:: 2.2.0
-           Please pass a ``signer`` instead.
-
     gpg_keyid (optional): A keyid used to identify a local gpg key used to sign
         the resulting link metadata.
 
     gpg_use_default (optional): A boolean indicating if the default gpg key
         should be used to sign the resulting link metadata.
 
     gpg_home (optional): A path to the gpg home directory. If not set the
@@ -521,16 +502,16 @@
     IOError, FileNotFoundError, NotADirectoryError, PermissionError:
         Cannot write link metadata.
 
     securesystemslib.exceptions.CryptoError, \
             securesystemslib.exceptions.UnsupportedAlgorithmError:
         Signing errors.
 
-    ValueError, OSError, securesystemslib.gpg.exceptions.CommandError, \
-            securesystemslib.gpg.exceptions.KeyNotFoundError:
+    ValueError, OSError, securesystemslib._gpg.exceptions.CommandError, \
+            securesystemslib._gpg.exceptions.KeyNotFoundError:
         gpg signing errors.
 
   Side Effects:
     Reads artifact files from disk.
     Runs link command in subprocess.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes link metadata file to disk, if any key argument is passed.
@@ -543,17 +524,14 @@
 
     LOG.info("Running '%s'...", name)
 
     # Check key formats to fail early
     if signer:
         _check_signer(signer)
 
-    if signing_key:
-        _check_signing_key(signing_key)
-
     if gpg_keyid:
         _check_hex(gpg_keyid)
 
     if exclude_patterns:
         _check_str_list(exclude_patterns)
 
     if base_path:
@@ -614,18 +592,14 @@
     else:
         LOG.info("Generating link metadata using Metablock...")
         link_metadata = Metablock(signed=link, compact_json=compact_json)
 
     if signer:
         LOG.info("Signing link metadata using passed signer...")
 
-    elif signing_key:
-        LOG.info("Signing link metadata using passed key...")
-        signer = SSlibSigner(signing_key)
-
     elif gpg_keyid:
         LOG.info("Signing link metadata using passed GPG keyid...")
         signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
 
     elif gpg_use_default:
         LOG.info("Signing link metadata using default GPG key ...")
         signer = GPGSigner(keyid=None, homedir=gpg_home)
@@ -645,30 +619,29 @@
 
     return link_metadata
 
 
 def in_toto_record_start(
     step_name,
     material_list,
-    signing_key=None,
     gpg_keyid=None,
     gpg_use_default=False,
     gpg_home=None,
     exclude_patterns=None,
     base_path=None,
     record_environment=False,
     normalize_line_endings=False,
     lstrip_paths=None,
     use_dsse=False,
     signer=None,
 ):
     """Generates preliminary link metadata.
 
   Records paths and hashes of materials in a preliminary link metadata file. The
-  metadata is signed with the passed signer, signing_key, a gpg key identified
+  metadata is signed with the passed signer, a gpg key identified
   by its ID, or the default gpg key. If multiple key arguments are passed, only
   one key is used in above order of precedence. At least one key argument must
   be passed. The resulting link file is written to
   ``.STEP-NAME.KEYID-PREFIX.link-unfinished``.
 
   Use this function together with in_toto_record_stop as an alternative to
   in_toto_run, in order to provide evidence for supply chain steps that cannot
@@ -676,19 +649,14 @@
 
   Arguments:
     step_name: A unique name to associate link metadata with a step.
 
     material_list: A list of artifact paths to be recorded as materials.
         Directories are traversed recursively.
 
-    signing_key (optional): A key used to sign the resulting link metadata.
-
-        .. deprecated:: 2.2.0
-           Please pass a ``signer`` instead.
-
     gpg_keyid (optional): A keyid used to identify a local gpg key used to sign
         the resulting link metadata.
 
     gpg_use_default (optional): A boolean indicating if the default gpg key
         should be used to sign the resulting link metadata.
 
     gpg_home (optional): A path to the gpg home directory. If not set the
@@ -715,15 +683,15 @@
 
     signer (optional): A securesystemslib Signer instance used to
         sign the resulting link metadata.
 
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
-    ValueError: None of signing_key, gpg_keyid or gpg_use_default=True is
+    ValueError: None of signer, gpg_keyid or gpg_use_default=True is
         passed.
 
     securesystemslib.exceptions.StorageError: Cannot hash artifacts.
 
     PrefixError: Left-stripping artifact paths results in non-unique dict keys.
 
     subprocess.TimeoutExpired: Link command times out.
@@ -731,38 +699,35 @@
     IOError, PermissionError:
         Cannot write link metadata.
 
     securesystemslib.exceptions.CryptoError, \
             securesystemslib.exceptions.UnsupportedAlgorithmError:
         Signing errors.
 
-    ValueError, OSError, securesystemslib.gpg.exceptions.CommandError, \
-            securesystemslib.gpg.exceptions.KeyNotFoundError:
+    ValueError, OSError, securesystemslib._gpg.exceptions.CommandError, \
+            securesystemslib._gpg.exceptions.KeyNotFoundError:
         gpg signing errors.
 
   Side Effects:
     Reads artifact files from disk.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes preliminary link metadata file to disk.
 
   """
     # pylint: disable=too-many-locals,too-many-branches
 
     LOG.info("Start recording '%s'...", step_name)
 
     # Fail if there is no signing key arg at all
-    _require_signing_arg(signer, signing_key, gpg_keyid, gpg_use_default)
+    _require_signing_arg(signer, gpg_keyid, gpg_use_default)
 
     # Check key formats to fail early
     if signer:
         _check_signer(signer)
 
-    if signing_key:
-        _check_signing_key(signing_key)
-
     if gpg_keyid:
         _check_str(gpg_keyid)
 
     if exclude_patterns:
         _check_str_list(exclude_patterns)
 
     if base_path:
@@ -800,18 +765,14 @@
     else:
         LOG.info("Generating link metadata using Metablock...")
         link_metadata = Metablock(signed=link)
 
     if signer:
         LOG.info("Signing link metadata using passed signer...")
 
-    elif signing_key:
-        LOG.info("Signing link metadata using passed key...")
-        signer = SSlibSigner(signing_key)
-
     elif gpg_keyid:
         LOG.info("Signing link metadata using passed GPG keyid...")
         signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
 
     else:  # (gpg_use_default)
         LOG.info("Signing link metadata using default GPG key ...")
         signer = GPGSigner(keyid=None, homedir=gpg_home)
@@ -827,15 +788,14 @@
     LOG.info("Storing preliminary link metadata to '%s'...", unfinished_fn)
     link_metadata.dump(unfinished_fn)
 
 
 def in_toto_record_stop(
     step_name,
     product_list,
-    signing_key=None,
     gpg_keyid=None,
     gpg_use_default=False,
     gpg_home=None,
     exclude_patterns=None,
     base_path=None,
     normalize_line_endings=False,
     lstrip_paths=None,
@@ -845,15 +805,15 @@
     environment=None,
     signer=None,
 ):
     """Finalizes preliminary link metadata generated with in_toto_record_start.
 
   Loads preliminary link metadata file, verifies its signature, and records
   paths and hashes as products, thus finalizing the link metadata. The metadata
-  is signed with the passed signer, signing_key, a gpg key identified by its ID,
+  is signed with the passed signer, a gpg key identified by its ID,
   or the default gpg key. If multiple key arguments are passed, only one key is
   used in above order of precedence. At least one key argument must be passed
   and it must be the same as the one used to sign the preliminary link metadata
   file. The resulting link file is written to ``STEP-NAME.KEYID-PREFIX.link``.
 
   Use this function together with in_toto_record_start as an alternative to
   in_toto_run, in order to provide evidence for supply chain steps that cannot
@@ -861,19 +821,14 @@
 
   Arguments:
     step_name: A unique name to associate link metadata with a step.
 
     product_list: A list of artifact paths to be recorded as products.
         Directories are traversed recursively.
 
-    signing_key (optional): A key used to sign the resulting link metadata.
-
-        .. deprecated:: 2.2.0
-           Please pass a ``signer`` instead.
-
     gpg_keyid (optional): A keyid used to identify a local gpg key used to sign
         the resulting link metadata.
 
     gpg_use_default (optional): A boolean indicating if the default gpg key
         should be used to sign the resulting link metadata.
 
     gpg_home (optional): A path to the gpg home directory. If not set the
@@ -914,15 +869,15 @@
 
     signer (optional): A securesystemslib Signer instance used to
         sign the resulting link metadata.
 
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
-    ValueError: None of signing_key, gpg_keyid or gpg_use_default=True is
+    ValueError: None of gpg_keyid or gpg_use_default=True is
         passed.
 
     LinkNotFoundError: No preliminary link metadata file found.
 
     securesystemslib.exceptions.StorageError: Cannot hash artifacts.
 
     PrefixError: Left-stripping artifact paths results in non-unique dict keys.
@@ -932,38 +887,35 @@
     IOError, FileNotFoundError, NotADirectoryError, PermissionError:
         Cannot write link metadata.
 
     securesystemslib.exceptions.CryptoError, \
             securesystemslib.exceptions.UnsupportedAlgorithmError:
         Signing errors.
 
-    ValueError, OSError, securesystemslib.gpg.exceptions.CommandError, \
-            securesystemslib.gpg.exceptions.KeyNotFoundError:
+    ValueError, OSError, securesystemslib._gpg.exceptions.CommandError, \
+            securesystemslib._gpg.exceptions.KeyNotFoundError:
         gpg signing errors.
 
   Side Effects:
     Reads preliminary link metadata file from disk.
     Reads artifact files from disk.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes resulting link metadata file to disk.
     Removes preliminary link metadata file from disk.
 
   """
     # pylint: disable=too-many-branches, too-many-locals, too-many-statements
     LOG.info("Stop recording '%s'...", step_name)
 
     # Check that we have something to sign and if the formats are right
-    _require_signing_arg(signer, signing_key, gpg_keyid, gpg_use_default)
+    _require_signing_arg(signer, gpg_keyid, gpg_use_default)
 
     if signer:
         _check_signer(signer)
 
-    if signing_key:
-        _check_signing_key(signing_key)
-
     if gpg_keyid:
         _check_hex(gpg_keyid)
 
     if exclude_patterns:
         _check_str_list(exclude_patterns)
 
     if base_path:
@@ -975,19 +927,14 @@
     # Load preliminary link file
     # If we have a signing key we can use the keyid to construct the name
     if signer:
         unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(
             step_name=step_name, keyid=signer.public_key.keyid
         )
 
-    elif signing_key:
-        unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(
-            step_name=step_name, keyid=signing_key["keyid"]
-        )
-
     # FIXME: Currently there is no way to know the default GPG key's keyid and
     # so we glob for preliminary link files
     else:
         unfinished_fn_glob = UNFINISHED_FILENAME_FORMAT_GLOB.format(
             step_name=step_name, pattern="*"
         )
         unfinished_fn_list = glob.glob(unfinished_fn_glob)
@@ -1011,31 +958,24 @@
 
         unfinished_fn = unfinished_fn_list[0]
 
     LOG.info("Loading preliminary link metadata '%s'...", unfinished_fn)
     link_metadata = Metadata.load(unfinished_fn)
 
     # The file must have been signed by the same key
-    # If we have a signing_key we use it for verification as well
+    # If we have a signer we use it for verification as well
     if signer:
         LOG.info("Verifying preliminary link signature using passed signer...")
         keyid = signer.public_key.keyid
         verification_key = signer.public_key.to_dict()
         verification_key["keyid"] = keyid
 
-    elif signing_key:
-        LOG.info(
-            "Verifying preliminary link signature using passed signing key..."
-        )
-        keyid = signing_key["keyid"]
-        verification_key = signing_key
-
     elif gpg_keyid:
         LOG.info("Verifying preliminary link signature using passed gpg key...")
-        gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
+        gpg_pubkey = securesystemslib._gpg.functions.export_pubkey(  # pylint: disable=protected-access
             gpg_keyid, gpg_home
         )
         keyid = gpg_pubkey["keyid"]
         verification_key = gpg_pubkey
 
     else:  # must be gpg_use_default
         # FIXME: Currently there is no way to know the default GPG key's keyid
@@ -1043,21 +983,25 @@
         # Link file's signature and try to export a pubkey from the gpg
         # home directory. We do this even if a gpg_keyid was specified, because gpg
         # accepts many different ids (mail, name, parts of an id, ...) but we
         # need a specific format.
         LOG.info(
             "Verifying preliminary link signature using default gpg key..."
         )
-        # signatures are objects in DSSE.
-        sig = link_metadata.signatures[0]
-        if isinstance(sig, Signature):
-            keyid = sig.keyid
+
+        # The `signatures` field is not part of the common Envelope/Metablock
+        # interface, so we need to case handle. Note that we shouldn't be
+        # accessing `signatures` here in the first place (see FIXME above).
+        if isinstance(link_metadata, Envelope):
+            keyid = link_metadata.signatures.values()[0].keyid
+
         else:
-            keyid = sig["keyid"]
-        gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
+            keyid = link_metadata.signatures[0]["keyid"]
+
+        gpg_pubkey = securesystemslib._gpg.functions.export_pubkey(  # pylint: disable=protected-access
             keyid, gpg_home
         )
         verification_key = gpg_pubkey
 
     link_metadata.verify_signature(verification_key)
 
     LOG.info("Extracting Link from metadata...")
@@ -1095,18 +1039,14 @@
     if signer:
         LOG.info(
             "Updating signature with signer '{:.8}...'...".format(
                 signer.public_key.keyid
             )
         )
 
-    elif signing_key:
-        LOG.info("Updating signature with key '{:.8}...'...".format(keyid))
-        signer = SSlibSigner(signing_key)
-
     else:  # gpg_keyid or gpg_use_default
         # In both cases we use the keyid we got from verifying the preliminary
         # link signature above.
         LOG.info("Updating signature with gpg key '{:.8}...'...".format(keyid))
         signer = GPGSigner(keyid=keyid, homedir=gpg_home)
 
     link_metadata.create_signature(signer)
```

### Comparing `in_toto-2.3.0/in_toto/settings.py` & `in_toto-3.0.0/in_toto/settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/verifylib.py` & `in_toto-3.0.0/in_toto/verifylib.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import logging
 import os
 
 import iso8601
 import securesystemslib.exceptions
 import securesystemslib.formats
 from dateutil import tz
-from securesystemslib.gpg.exceptions import KeyExpirationError
+from securesystemslib._gpg.exceptions import KeyExpirationError
 
 import in_toto.formats
 import in_toto.models.layout
 import in_toto.models.link
 import in_toto.rulelib
 import in_toto.runlib
 import in_toto.settings
@@ -379,15 +379,15 @@
       securesystemslib.exceptions.FormatError
         if the passed key dict is invalid.
 
       SignatureVerificationError
         if an empty verification key dictionary was passed, or
         if any of the passed verification keys fails to verify a signature.
 
-      securesystemslib.gpg.exceptions.KeyExpirationError:
+      securesystemslib._gpg.exceptions.KeyExpirationError:
         if any of the passed verification keys is an expired gpg key
 
     """
     _check_public_keys(keys_dict)
 
     # Fail if an empty verification key dictionary was passed
     if len(keys_dict) < 1:
```

### Comparing `in_toto-2.3.0/in_toto/models/_signer.py` & `in_toto-3.0.0/in_toto/models/_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
   Provides in-toto flavored Signer implementations
 
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
-import securesystemslib.gpg.exceptions as gpg_exceptions
-import securesystemslib.gpg.functions as gpg
+import securesystemslib._gpg.exceptions as gpg_exceptions
+import securesystemslib._gpg.functions as gpg
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key,
 )
 from securesystemslib import exceptions
 from securesystemslib.signer import (
     CryptoSigner,
@@ -133,14 +133,18 @@
 
     def __init__(
         self, keyid: Optional[str] = None, homedir: Optional[str] = None
     ):
         self.keyid = keyid
         self.homedir = homedir
 
+    @property
+    def public_key(self) -> Key:
+        raise NotImplementedError  # pragma: no cover
+
     @classmethod
     def from_priv_key_uri(
         cls,
         priv_key_uri: str,
         public_key: Key,
         secrets_handler: Optional[SecretsHandler] = None,
     ) -> "GPGSigner":
@@ -159,17 +163,17 @@
         Raises:
           securesystemslib.exceptions.FormatError:
             If the keyid is invalid.
           ValueError: the gpg command failed to create a valid signature.
           OSError: the gpg command is not present or non-executable.
           securesystemslib.exceptions.UnsupportedLibraryError: the gpg command is
             not available, or the cryptography library is not installed.
-          securesystemslib.gpg.exceptions.CommandError: the gpg command returned a
+          securesystemslib._gpg.exceptions.CommandError: the gpg command returned a
             non-zero exit code.
-          securesystemslib.gpg.exceptions.KeyNotFoundError: the used gpg version is
+          securesystemslib._gpg.exceptions.KeyNotFoundError: the used gpg version is
             not fully supported and no public key can be found for short keyid.
           Returns:
             Returns a ``GPGSignature`` class instance.
         """
 
         sig_dict = gpg.create_signature(payload, self.keyid, self.homedir)
         return GPGSignature(**sig_dict)
```

### Comparing `in_toto-2.3.0/in_toto/models/common.py` & `in_toto-3.0.0/in_toto/models/common.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/models/layout.py` & `in_toto-3.0.0/in_toto/models/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,16 @@
       represents a hook that is run at verification
 """
 import json
 import shlex
 from datetime import datetime
 
 import attr
+import securesystemslib._gpg.functions
 import securesystemslib.exceptions
-import securesystemslib.gpg.functions
-import securesystemslib.interface
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 
 import in_toto.exceptions
 import in_toto.rulelib
 from in_toto.formats import (
     _check_hex,
@@ -337,28 +336,28 @@
         Arguments:
           gpg_keyid: A keyid used to identify a local gpg public key.
           gpg_home (optional): A path to the gpg home directory. If not set the
               default gpg home directory is used.
 
         Raises:
           securesystemslib.exceptions.FormatError: Arguments are malformed.
-          securesystemslib.gpg.execeptions.KeyNotFoundError: Key cannot be found.
+          securesystemslib._gpg.execeptions.KeyNotFoundError: Key cannot be found.
 
         Side Effects:
           Calls system gpg command in a subprocess.
 
         Returns:
           The added key.
 
         """
         _check_hex(gpg_keyid)
         if gpg_home:  # pragma: no branch
             _check_str(gpg_home)
 
-        key = securesystemslib.gpg.functions.export_pubkey(
+        key = securesystemslib._gpg.functions.export_pubkey(  # pylint: disable=protected-access
             gpg_keyid, homedir=gpg_home
         )
         return self.add_functionary_key(key)
 
     def add_functionary_keys_from_paths(self, key_path_list):
         """Loads keys from disk and adds as functionary keys to layout.
 
@@ -389,15 +388,15 @@
         Arguments:
           gpg_keyid_list: A list of keyids used to identify local gpg public keys.
           gpg_home (optional): A path to the gpg home directory. If not set the
               default gpg home directory is used.
 
         Raises:
           securesystemslib.exceptions.FormatError: Arguments are malformed.
-          securesystemslib.gpg.execeptions.KeyNotFoundError: A key cannot be found.
+          securesystemslib._gpg.execeptions.KeyNotFoundError: A key cannot be found.
 
         Side Effects:
           Calls system gpg command in a subprocess.
 
         Returns:
           A dictionary of the added functionary keys, with keyids as dictionary
           keys and keys as values.
```

### Comparing `in_toto-2.3.0/in_toto/models/link.py` & `in_toto-3.0.0/in_toto/models/link.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/models/metadata.py` & `in_toto-3.0.0/in_toto/models/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,30 +23,26 @@
 """
 
 import json
 from copy import deepcopy
 from typing import Union
 
 import attr
+import securesystemslib._gpg.functions
 import securesystemslib.exceptions
 import securesystemslib.formats
-import securesystemslib.gpg.functions
 from securesystemslib.dsse import Envelope as SSlibEnvelope
 from securesystemslib.exceptions import (
     UnverifiedSignatureError,
     VerificationError,
 )
 from securesystemslib.signer import Key, Signature, Signer
 
 from in_toto.exceptions import InvalidMetadata, SignatureVerificationError
-from in_toto.formats import (
-    _check_public_key,
-    _check_signature,
-    _check_signing_key,
-)
+from in_toto.formats import _check_public_key, _check_signature
 from in_toto.models._signer import GPGSigner
 from in_toto.models.common import Signable, ValidationMixin
 from in_toto.models.layout import Layout
 from in_toto.models.link import Link
 
 ENVELOPE_PAYLOAD_TYPE = "application/vnd.in-toto+json"
 
@@ -156,15 +152,15 @@
             attr.asdict(signable),
             sort_keys=True,
         ).encode("utf-8")
 
         return cls(
             payload=json_bytes,
             payload_type=ENVELOPE_PAYLOAD_TYPE,
-            signatures=[],
+            signatures={},
         )
 
     def create_signature(self, signer: Signer) -> Signature:
         if isinstance(signer, GPGSigner):
             raise NotImplementedError("GPG Signing is not implemented")
 
         return super().sign(signer)
@@ -293,72 +289,40 @@
 
     def create_signature(self, signer: Signer):
         signature = signer.sign(self.signed.signable_bytes)
         self.signatures.append(signature.to_dict())
 
         return signature
 
-    def sign(self, key):
-        """Creates signature over signable with key and adds it to signatures.
-
-    Uses the UTF-8 encoded canonical JSON byte representation of the signable
-    attribute to create signatures deterministically.
-
-    Attributes:
-      key: A signing key.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: Key argument is malformed.
-      securesystemslib.exceptions.CryptoError, \
-              securesystemslib.exceptions.UnsupportedAlgorithmError:
-          Signing errors.
-
-    Returns:
-      The signature.
-
-    .. deprecated:: 2.2.0
-        Please use ``Metablock.create_signature()`` instead.
-
-    """
-        _check_signing_key(key)
-
-        signature = securesystemslib.keys.create_signature(
-            key, self.signed.signable_bytes
-        )
-
-        self.signatures.append(signature)
-
-        return signature
-
     def sign_gpg(self, gpg_keyid=None, gpg_home=None):
         """Creates signature over signable with gpg and adds it to signatures.
 
     Uses the UTF-8 encoded canonical JSON byte representation of the signable
     attribute to create signatures deterministically.
 
     Arguments:
       gpg_keyid (optional): A keyid used to identify a local gpg signing key.
           If omitted the default signing key is used.
 
       gpg_home (optional): A path to the gpg home directory. If not set the
           default gpg home directory is used.
 
     Raises:
-      ValueError, OSError, securesystemslib.gpg.exceptions.CommandError, \
-            securesystemslib.gpg.exceptions.KeyNotFoundError:
+      ValueError, OSError, securesystemslib._gpg.exceptions.CommandError, \
+            securesystemslib._gpg.exceptions.KeyNotFoundError:
         gpg signing errors.
 
     Side Effects:
       Calls system gpg command in a subprocess.
 
     Returns:
       The signature.
 
     """
-        signature = securesystemslib.gpg.functions.create_signature(
+        signature = securesystemslib._gpg.functions.create_signature(  # pylint: disable=protected-access
             self.signed.signable_bytes, gpg_keyid, gpg_home
         )
 
         self.signatures.append(signature)
 
         return signature
 
@@ -378,15 +342,15 @@
         Raises:
           securesystemslib.exceptions.FormatError: The passed key is malformed.
 
           SignatureVerificationError: No signature keyid matches the verification
               key keyid, or the matching signature is malformed, or the matching
               signature is invalid.
 
-          securesystemslib.gpg.exceptions.KeyExpirationError: Passed verification
+          securesystemslib._gpg.exceptions.KeyExpirationError: Passed verification
               key is an expired gpg key.
 
         """
         _check_public_key(verification_key)
         verification_keyid = verification_key["keyid"]
 
         # Find a signature that corresponds to the keyid of the passed
@@ -404,15 +368,15 @@
         else:
             raise SignatureVerificationError(
                 "No signature found for key '{}'".format(verification_keyid)
             )
 
         valid = False
         if "signature" in signature and "other_headers" in signature:
-            valid = securesystemslib.gpg.functions.verify_signature(
+            valid = securesystemslib._gpg.functions.verify_signature(  # pylint: disable=protected-access
                 signature, verification_key, self.signed.signable_bytes
             )
 
         else:
             # Parse key and (below) signature dicts as `Key` and `Signature`
             # instances to use modern securesystemslib verification code.
             # Deepcopy to preserve original dicts, which are otherwise destroyed
```

### Comparing `in_toto-2.3.0/in_toto/resolver/__init__.py` & `in_toto-3.0.0/in_toto/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/in_toto/resolver/_resolver.py` & `in_toto-3.0.0/in_toto/resolver/_resolver.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/__init__.py` & `in_toto-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/common.py` & `in_toto-3.0.0/tests/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,22 +32,14 @@
 import sys
 import tempfile
 import unittest
 from pathlib import Path
 from typing import Any, Dict
 from unittest.mock import patch
 
-from securesystemslib.interface import (
-    generate_and_write_ecdsa_keypair,
-    generate_and_write_ed25519_keypair,
-    generate_and_write_rsa_keypair,
-    generate_and_write_unencrypted_ecdsa_keypair,
-    generate_and_write_unencrypted_ed25519_keypair,
-    generate_and_write_unencrypted_rsa_keypair,
-)
 from securesystemslib.signer import CryptoSigner
 
 from in_toto.models._signer import (
     load_crypto_signer_from_pkcs8_file as load_signer,
 )
 from in_toto.models._signer import load_public_key_from_file as load_pubkey
 
@@ -104,49 +96,14 @@
         gpg_keys = os.path.join(
             os.path.dirname(os.path.realpath(__file__)), "gpg_keyrings", "rsa"
         )
 
         shutil.copytree(gpg_keys, os.path.join(os.getcwd(), cls.gnupg_home))
 
 
-class GenKeysMixin:
-    """Mixin with classmethod to create cryptographic keys in cwd."""
-
-    key_pw = "pw"
-
-    @classmethod
-    def set_up_keys(cls):
-        """Generate securesystemslib test keys and write to CWD."""
-        # Generated unencrypted keys
-        cls.rsa_key_path = generate_and_write_unencrypted_rsa_keypair()
-        cls.rsa_key_id = os.path.basename(cls.rsa_key_path)
-
-        cls.ed25519_key_path = generate_and_write_unencrypted_ed25519_keypair()
-        cls.ed25519_key_id = os.path.basename(cls.ed25519_key_path)
-
-        cls.ecdsa_key_path = generate_and_write_unencrypted_ecdsa_keypair()
-        cls.ecdsa_key_id = os.path.basename(cls.ecdsa_key_path)
-
-        # Generate encrypted keys
-        cls.rsa_key_enc_path = generate_and_write_rsa_keypair(
-            password=cls.key_pw
-        )
-        cls.rsa_key_enc_id = os.path.basename(cls.rsa_key_enc_path)
-
-        cls.ed25519_key_enc_path = generate_and_write_ed25519_keypair(
-            password=cls.key_pw
-        )
-        cls.ed25519_key_enc_id = os.path.basename(cls.ed25519_key_enc_path)
-
-        cls.ecdsa_key_enc_path = generate_and_write_ecdsa_keypair(
-            password=cls.key_pw
-        )
-        cls.ecdsa_key_enc_id = os.path.basename(cls.ecdsa_key_enc_path)
-
-
 class CliTestCase(unittest.TestCase):
     """TestCase subclass providing a test helper that patches sys.argv with
     passed arguments and asserts a SystemExit with a return code equal
     to the passed status argument.
 
     Subclasses of CliTestCase require a class variable that stores the main
     function of the cli tool to test as staticmethod, e.g.:
```

### Comparing `in_toto-2.3.0/tests/runtests.py` & `in_toto-3.0.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_common_args.py` & `in_toto-3.0.0/tests/test_common_args.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_directory_resolver.py` & `in_toto-3.0.0/tests/test_directory_resolver.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_in_toto_match_products.py` & `in_toto-3.0.0/tests/test_in_toto_match_products.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_in_toto_mock.py` & `in_toto-3.0.0/tests/test_in_toto_mock.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_in_toto_run.py` & `in_toto-3.0.0/tests/test_in_toto_run.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,56 +24,39 @@
 import glob
 import os
 import tempfile
 import unittest
 from pathlib import Path
 from unittest import mock
 
-import securesystemslib.interface  # pylint: disable=unused-import
-
 from in_toto.in_toto_run import main as in_toto_run_main
 from in_toto.models.link import FILENAME_FORMAT
 from in_toto.models.metadata import Metablock, Metadata
-from tests.common import CliTestCase, GenKeysMixin, GPGKeysMixin, TmpDirMixin
+from tests.common import PEMS, CliTestCase, GPGKeysMixin, TmpDirMixin
 
 
-class TestInTotoRunTool(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
+class TestInTotoRunTool(CliTestCase, TmpDirMixin, GPGKeysMixin):
     """Test in_toto_run's main() - requires sys.argv patching; and
     in_toto_run- calls runlib and error logs/exits on Exception."""
 
     cli_main_func = staticmethod(in_toto_run_main)
 
     @classmethod
     def setUpClass(cls):
         """Create and change into temporary directory,
         generate key pair, dummy artifact and base arguments."""
         cls.set_up_test_dir()
         cls.set_up_gpg_keys()
-        cls.set_up_keys()
 
         cls.test_step = "test_step"
+
+        cls.rsa_key_path = str(PEMS / "rsa_private_unencrypted.pem")
         cls.test_link_rsa = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.rsa_key_id
-        )
-        cls.test_link_ed25519 = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ed25519_key_id
-        )
-        cls.test_link_ecdsa = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ecdsa_key_id
-        )
-        cls.test_link_rsa_enc = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.rsa_key_enc_id
-        )
-        cls.test_link_ed25519_enc = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ed25519_key_enc_id
+            step_name=cls.test_step, keyid="2f685fa7"
         )
-        cls.test_link_ecdsa_enc = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ecdsa_key_enc_id
-        )
-
         cls.test_artifact = "test_artifact"
         Path(cls.test_artifact).touch()
 
     @classmethod
     def tearDownClass(cls):
         cls.tear_down_test_dir()
 
@@ -83,15 +66,15 @@
 
     def test_main_required_args(self):
         """Test CLI command with required arguments."""
 
         args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--",
             "python",
             "--version",
         ]
 
         self.assert_cli_sys_exit(args, 0)
@@ -99,15 +82,15 @@
 
     def test_main_optional_args(self):
         """Test CLI command with optional arguments."""
 
         named_args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--materials",
             self.test_artifact,
             "--products",
             self.test_artifact,
             "--record-streams",
         ]
@@ -162,100 +145,29 @@
 
     def test_main_with_metadata_directory(self):
         """Test CLI command with metadata directory."""
         tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
         args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--metadata-directory",
             tmp_dir,
             "--",
             "python",
             "--version",
         ]
 
         self.assert_cli_sys_exit(args, 0)
 
         linkpath = os.path.join(tmp_dir, self.test_link_rsa)
 
         self.assertTrue(os.path.exists(linkpath))
 
-    def test_main_with_unencrypted_ed25519_key(self):
-        """Test CLI command with ed25519 key."""
-        args = [
-            "-n",
-            self.test_step,
-            "--key",
-            self.ed25519_key_path,
-            "--key-type",
-            "ed25519",
-            "--",
-            "ls",
-        ]
-
-        self.assert_cli_sys_exit(args, 0)
-        self.assertTrue(os.path.exists(self.test_link_ed25519))
-
-    def test_main_with_unencrypted_ecdsa_key(self):
-        """Test CLI command with ecdsa key."""
-        args = [
-            "-n",
-            self.test_step,
-            "--key",
-            self.ecdsa_key_path,
-            "--key-type",
-            "ecdsa",
-            "--",
-            "ls",
-        ]
-
-        self.assert_cli_sys_exit(args, 0)
-        self.assertTrue(os.path.exists(self.test_link_ecdsa))
-
-    def test_main_with_encrypted_keys(self):
-        """Test CLI command with encrypted ed25519 key."""
-
-        for key_type, key_path, link_path in [
-            ("rsa", self.rsa_key_enc_path, self.test_link_rsa_enc),
-            ("ed25519", self.ed25519_key_enc_path, self.test_link_ed25519_enc),
-            ("ecdsa", self.ecdsa_key_enc_path, self.test_link_ecdsa_enc),
-        ]:
-            # Define common arguments passed to in in-toto-run below
-            args = [
-                "-n",
-                self.test_step,
-                "--key",
-                key_path,
-                "--key-type",
-                key_type,
-            ]
-            cmd = ["--", "python", "--version"]
-
-            # Make sure the link file to be generated doesn't already exist
-            self.assertFalse(os.path.exists(link_path))
-
-            # Test 1: Call in-toto-run entering signing key password on prompt
-            with mock.patch(
-                "securesystemslib.interface.get_password",
-                return_value=self.key_pw,
-            ):
-                self.assert_cli_sys_exit(args + ["--password"] + cmd, 0)
-
-            self.assertTrue(os.path.exists(link_path))
-            os.remove(link_path)
-
-            # Test 2: Call in-toto-run passing signing key password
-            self.assert_cli_sys_exit(
-                args + ["--password", self.key_pw] + cmd, 0
-            )
-            self.assertTrue(os.path.exists(link_path))
-            os.remove(link_path)
-
     def test_main_with_specified_gpg_key(self):
         """Test CLI command with specified gpg key."""
         args = [
             "-n",
             self.test_step,
             "--gpg",
             self.gpg_key_85da58,
@@ -297,39 +209,45 @@
     def test_main_no_command_arg(self):
         """Test CLI command with --no-command argument."""
 
         args = [
             "in_toto_run.py",
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--no-command",
         ]
 
         self.assert_cli_sys_exit(args, 0)
 
         self.assertTrue(os.path.exists(self.test_link_rsa))
 
     def test_main_wrong_args(self):
         """Test CLI command with missing arguments."""
 
         wrong_args_list = [
             [],
             ["--step-name", "some"],
-            ["--key", self.rsa_key_path],
+            ["--signing-key", self.rsa_key_path],
             ["--", "echo", "blub"],
-            ["--step-name", "test-step", "--key", self.rsa_key_path],
+            ["--step-name", "test-step", "--signing-key", self.rsa_key_path],
             ["--step-name", "--", "echo", "blub"],
-            ["--key", self.rsa_key_path, "--", "echo", "blub"],
-            ["--step-name", "test-step", "--key", self.rsa_key_path, "--"],
+            ["--signing-key", self.rsa_key_path, "--", "echo", "blub"],
+            [
+                "--step-name",
+                "test-step",
+                "--signing-key",
+                self.rsa_key_path,
+                "--",
+            ],
             [
                 "--step-name",
                 "test-step",
-                "--key",
+                "--signing-key",
                 self.rsa_key_path,
                 "--gpg",
                 "--",
                 "echo",
                 "blub",
             ],
         ]
@@ -340,53 +258,42 @@
 
     def test_main_wrong_key_exits(self):
         """Test CLI command with wrong key argument, exits and logs error"""
 
         args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             "non-existing-key",
             "--",
             "echo",
             "test",
         ]
 
         self.assert_cli_sys_exit(args, 1)
         self.assertFalse(os.path.exists(self.test_link_rsa))
 
-    def test_main_encrypted_key_but_no_pw(self):
-        """Test CLI command exits 1 with encrypted key but no pw."""
-        args = ["-n", self.test_step, "--key", self.rsa_key_enc_path, "-x"]
-        self.assert_cli_sys_exit(args, 1)
-        self.assertFalse(os.path.exists(self.test_link_rsa_enc))
-
-        args = ["-n", self.test_step, "--key", self.ed25519_key_enc_path, "-x"]
-        self.assert_cli_sys_exit(args, 1)
-        self.assertFalse(os.path.exists(self.test_link_ed25519_enc))
-
     def test_pkcs8_signing_key(self):
         """Test in-toto-run, sign link with pkcs8 key file for each algo."""
-        pems_dir = Path(__file__).parent / "pems"
         args = ["-n", "foo", "-x", "--signing-key"]
         for algo, short_keyid in [
             ("rsa", "2f685fa7"),
             ("ecdsa", "50d7e110"),
             ("ed25519", "c6d8bf2e"),
         ]:
             link_path = Path(f"foo.{short_keyid}.link")
 
             # Use unencrypted key
-            pem_path = pems_dir / f"{algo}_private_unencrypted.pem"
+            pem_path = PEMS / f"{algo}_private_unencrypted.pem"
             self.assert_cli_sys_exit(args + [str(pem_path)], 0)
             self.assertTrue(link_path.exists())
             link_path.unlink()
 
             # Fail with encrypted key, but no pw
-            pem_path = pems_dir / f"{algo}_private_encrypted.pem"
+            pem_path = PEMS / f"{algo}_private_encrypted.pem"
             self.assert_cli_sys_exit(args + [str(pem_path)], 1)
             self.assertFalse(link_path.exists())
 
             # Use encrypted key, passing pw
             self.assert_cli_sys_exit(args + [str(pem_path), "-P", "hunter2"], 0)
             self.assertTrue(link_path.exists())
             link_path.unlink()
@@ -396,45 +303,33 @@
                 "in_toto.in_toto_run.getpass", return_value="hunter2"
             ):
                 self.assert_cli_sys_exit(args + [str(pem_path), "-P"], 0)
             self.assertTrue(link_path.exists())
             link_path.unlink()
 
 
-class TestInTotoRunToolWithDSSE(
-    CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin
-):
+class TestInTotoRunToolWithDSSE(CliTestCase, TmpDirMixin, GPGKeysMixin):
     """Test in_toto_run's main() with --use-dsse argument - requires sys.argv
     patching; and in_toto_run- calls runlib and error logs/exits on Exception.
     """
 
     cli_main_func = staticmethod(in_toto_run_main)
 
     @classmethod
     def setUpClass(cls):
         """Create and change into temporary directory,
         generate key pair, dummy artifact and base arguments."""
         cls.set_up_test_dir()
         cls.set_up_gpg_keys()
-        cls.set_up_keys()
 
         cls.test_step = "test_step"
+        cls.rsa_key_path = str(PEMS / "rsa_private_unencrypted.pem")
         cls.test_link_rsa = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.rsa_key_id
-        )
-        cls.test_link_ed25519 = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ed25519_key_id
-        )
-        cls.test_link_rsa_enc = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.rsa_key_enc_id
+            step_name=cls.test_step, keyid="2f685fa7"
         )
-        cls.test_link_ed25519_enc = FILENAME_FORMAT.format(
-            step_name=cls.test_step, keyid=cls.ed25519_key_enc_id
-        )
-
         cls.test_artifact = "test_artifact"
         Path(cls.test_artifact).touch()
 
     @classmethod
     def tearDownClass(cls):
         cls.tear_down_test_dir()
 
@@ -444,15 +339,15 @@
 
     def test_main_required_args(self):
         """Test CLI command with required arguments."""
 
         args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--use-dsse",
             "--",
             "python",
             "--version",
         ]
 
@@ -461,15 +356,15 @@
 
     def test_main_optional_args(self):
         """Test CLI command with optional arguments."""
 
         named_args = [
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--materials",
             self.test_artifact,
             "--products",
             self.test_artifact,
             "--record-streams",
             "--use-dsse",
@@ -535,43 +430,42 @@
     def test_main_no_command_arg(self):
         """Test CLI command with --no-command argument."""
 
         args = [
             "in_toto_run.py",
             "--step-name",
             self.test_step,
-            "--key",
+            "--signing-key",
             self.rsa_key_path,
             "--no-command",
             "--use-dsse",
         ]
 
         self.assert_cli_sys_exit(args, 0)
 
         self.assertTrue(os.path.exists(self.test_link_rsa))
 
     def test_pkcs8_signing_key(self):
-        """Test in-toto-run, sign link with pkcs8 key file for each algo."""
-        pems_dir = Path(__file__).parent / "pems"
+        """Test in-totqo-run, sign link with pkcs8 key file for each algo."""
         args = ["-n", "foo", "-x", "--use-dsse", "--signing-key"]
         for algo, short_keyid in [
             ("rsa", "2f685fa7"),
             ("ecdsa", "50d7e110"),
             ("ed25519", "c6d8bf2e"),
         ]:
             link_path = Path(f"foo.{short_keyid}.link")
 
             # Use unencrypted key
-            pem_path = pems_dir / f"{algo}_private_unencrypted.pem"
+            pem_path = PEMS / f"{algo}_private_unencrypted.pem"
             self.assert_cli_sys_exit(args + [str(pem_path)], 0)
             self.assertTrue(link_path.exists())
             link_path.unlink()
 
             # Fail with encrypted key, but no pw
-            pem_path = pems_dir / f"{algo}_private_encrypted.pem"
+            pem_path = PEMS / f"{algo}_private_encrypted.pem"
             self.assert_cli_sys_exit(args + [str(pem_path)], 1)
             self.assertFalse(link_path.exists())
 
             # Use encrypted key, passing pw
             self.assert_cli_sys_exit(args + [str(pem_path), "-P", "hunter2"], 0)
             self.assertTrue(link_path.exists())
             link_path.unlink()
```

### Comparing `in_toto-2.3.0/tests/test_in_toto_sign.py` & `in_toto-3.0.0/tests/test_in_toto_sign.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_log.py` & `in_toto-3.0.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_ostree_resolver.py` & `in_toto-3.0.0/tests/test_ostree_resolver.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_param_substitution.py` & `in_toto-3.0.0/tests/test_param_substitution.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_resolver.py` & `in_toto-3.0.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_rulelib.py` & `in_toto-3.0.0/tests/test_rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_runlib.py` & `in_toto-3.0.0/tests/test_runlib.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,22 +30,14 @@
 import sys
 import tempfile
 import unittest
 from pathlib import Path
 
 import securesystemslib.exceptions
 import securesystemslib.formats
-from securesystemslib.interface import (
-    generate_and_write_unencrypted_rsa_keypair,
-    import_ed25519_privatekey_from_file,
-    import_ed25519_publickey_from_file,
-    import_rsa_privatekey_from_file,
-    import_rsa_publickey_from_file,
-)
-from securesystemslib.signer import CryptoSigner, Signer
 
 import in_toto.exceptions
 import in_toto.settings
 from in_toto.exceptions import SignatureVerificationError
 from in_toto.formats import _check_hash_dict
 from in_toto.models.link import (
     FILENAME_FORMAT,
@@ -58,15 +50,15 @@
     _subprocess_run_duplicate_streams,
     in_toto_match_products,
     in_toto_record_start,
     in_toto_record_stop,
     in_toto_run,
     record_artifacts_as_dict,
 )
-from tests.common import TmpDirMixin
+from tests.common import SignerStore, TmpDirMixin
 
 
 def _apply_exclude_patterns(names, patterns):
     """Temporary bridge from old `runlib._apply_exclude_patterns` with new
     `FileResolver._exclude`.
 
      TODO: Replace tist once resolver interface evolves
@@ -728,18 +720,16 @@
     @classmethod
     def setUpClass(cls):
         """Create and change into temporary directory, generate key pair and dummy
         material, read key pair."""
         cls.set_up_test_dir()
 
         cls.step_name = "test_step"
-        cls.key_path = "test_key"
-        generate_and_write_unencrypted_rsa_keypair(cls.key_path)
-        cls.key = import_rsa_privatekey_from_file(cls.key_path)
-        cls.key_pub = import_rsa_publickey_from_file(cls.key_path + ".pub")
+        cls.signer = SignerStore.rsa
+        cls.key = SignerStore.rsa_pub
 
         cls.test_artifact = "test_artifact"
         Path(cls.test_artifact).touch()
 
     @classmethod
     def tearDownClass(cls):
         cls.tear_down_test_dir()
@@ -754,15 +744,20 @@
             )
         except OSError:
             pass
 
     def test_in_toto_run_verify_signature(self):
         """Successfully run, verify signed metadata."""
         link = in_toto_run(
-            self.step_name, None, None, ["python", "--version"], True, self.key
+            self.step_name,
+            None,
+            None,
+            ["python", "--version"],
+            True,
+            signer=self.signer,
         )
         link.verify_signature(self.key)
 
     def test_in_toto_run_no_signature(self):
         """Successfully run, verify empty signature field."""
         link = in_toto_run(self.step_name, None, None, ["python", "--version"])
         self.assertFalse(len(link.signatures))
@@ -804,15 +799,15 @@
         """Successfully run, compare dumped link is equal to returned link."""
         link = in_toto_run(
             self.step_name,
             [self.test_artifact],
             [self.test_artifact],
             ["python", "--version"],
             True,
-            self.key,
+            signer=self.signer,
         )
         link_dump = Metablock.load(
             FILENAME_FORMAT.format(
                 step_name=self.step_name, keyid=self.key["keyid"]
             )
         )
         self.assertEqual(repr(link), repr(link_dump))
@@ -823,15 +818,15 @@
         tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
         link = in_toto_run(
             self.step_name,
             [self.test_artifact],
             [self.test_artifact],
             ["python", "--version"],
             True,
-            self.key,
+            signer=self.signer,
             metadata_directory=tmp_dir,
         )
         file_path = os.path.join(
             tmp_dir,
             FILENAME_FORMAT.format(
                 step_name=self.step_name, keyid=self.key["keyid"]
             ),
@@ -845,15 +840,15 @@
         tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
         in_toto_run(
             self.step_name,
             [self.test_artifact],
             [self.test_artifact],
             ["python", "--version"],
             True,
-            self.key,
+            signer=self.signer,
             metadata_directory=tmp_dir,
         )
         file_path = os.path.join(
             tmp_dir,
             FILENAME_FORMAT.format(
                 step_name=self.step_name, keyid=self.key["keyid"]
             ),
@@ -862,15 +857,15 @@
 
         in_toto_run(
             self.step_name,
             [self.test_artifact],
             [self.test_artifact],
             ["python", "--version"],
             True,
-            self.key,
+            signer=self.signer,
         )
         link_dump_without_md = Metablock.load(
             FILENAME_FORMAT.format(
                 step_name=self.step_name, keyid=self.key["keyid"]
             )
         )
         self.assertEqual(
@@ -943,36 +938,24 @@
                 None,
                 None,
                 ["python", "--version"],
                 True,
                 "this-is-not-a-key",
             )
 
-    def test_in_toto_wrong_key(self):
-        """Fail run, passed key is a public key."""
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            in_toto_run(
-                self.step_name,
-                None,
-                None,
-                ["python", "--version"],
-                True,
-                self.key_pub,
-            )
-
     def test_nonexistent_directory(self):
         """Fail run, passed metadata_directory not exist."""
         with self.assertRaises(FileNotFoundError):
             in_toto_run(
                 self.step_name,
                 None,
                 None,
                 ["python", "--version"],
                 True,
-                self.key,
+                signer=self.signer,
                 metadata_directory="nonexistentDir",
             )
 
     def test_not_a_directory(self):
         """Fail run, passed metadata_directory is not a directory."""
         fd, path = tempfile.mkstemp()
         os.write(fd, b"hello in-toto")
@@ -981,15 +964,15 @@
         with self.assertRaises((NotADirectoryError, FileNotFoundError)):
             in_toto_run(
                 self.step_name,
                 None,
                 None,
                 ["python", "--version"],
                 True,
-                self.key,
+                signer=self.signer,
                 metadata_directory=path,
             )
         os.remove(path)
 
     @unittest.skipIf(os.name == "nt", "chmod doesn't work properly on Windows")
     def test_in_toto_read_only_metadata_directory(self):
         """Fail run, passed metadata directory is read only"""
@@ -999,29 +982,29 @@
         with self.assertRaises(PermissionError):
             in_toto_run(
                 self.step_name,
                 None,
                 None,
                 ["python", "--version"],
                 True,
-                self.key,
+                signer=self.signer,
                 metadata_directory=tmp_dir,
             )
         os.rmdir(tmp_dir)
 
     def test_in_toto_for_dsse(self):
         """Test metadata generation using dsse."""
 
         link_metadata = in_toto_run(
             self.step_name,
             None,
             None,
             ["python", "--version"],
             True,
-            self.key,
+            signer=self.signer,
             use_dsse=True,
         )
         self.assertIsInstance(link_metadata, Envelope)
         link_metadata.verify_signature(self.key)
 
 
 class TestInTotoRecordStart(unittest.TestCase, TmpDirMixin):
@@ -1029,17 +1012,16 @@
 
     @classmethod
     def setUpClass(cls):
         """Create and change into temporary directory, generate key pair and dummy
         material, read key pair."""
         cls.set_up_test_dir()
 
-        cls.key_path = "test_key"
-        generate_and_write_unencrypted_rsa_keypair(cls.key_path)
-        cls.key = import_rsa_privatekey_from_file(cls.key_path)
+        cls.signer = SignerStore.rsa
+        cls.key = SignerStore.rsa_pub
 
         cls.step_name = "test_step"
         cls.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(
             step_name=cls.step_name, keyid=cls.key["keyid"]
         )
 
         cls.test_material = "test_material"
@@ -1056,43 +1038,49 @@
             == ".{}.{:.8}.link-unfinished".format(
                 self.step_name, self.key["keyid"]
             )
         )
 
     def test_create_unfinished_metadata_with_expected_material(self):
         """Test record start creates metadata with expected material."""
-        in_toto_record_start(self.step_name, [self.test_material], self.key)
+        in_toto_record_start(
+            self.step_name, [self.test_material], signer=self.signer
+        )
         link = Metablock.load(self.link_name_unfinished)
         self.assertEqual(
             list(link.signed.materials.keys()), [self.test_material]
         )
         os.remove(self.link_name_unfinished)
 
     def test_create_unfinished_metadata_verify_signature(self):
         """Test record start creates metadata with expected signature."""
-        in_toto_record_start(self.step_name, [self.test_material], self.key)
+        in_toto_record_start(
+            self.step_name, [self.test_material], signer=self.signer
+        )
         link = Metablock.load(self.link_name_unfinished)
         link.verify_signature(self.key)
         os.remove(self.link_name_unfinished)
 
     def test_no_key_arguments(self):
         """Test record start without passing one required key argument."""
         with self.assertRaises(ValueError):
             in_toto_record_start(
                 self.step_name,
                 [],
-                signing_key=None,
                 gpg_keyid=None,
                 gpg_use_default=False,
             )
 
     def test_create_unfinished_metadata_using_dsse(self):
         """Test record start creates metadata using dsse."""
         in_toto_record_start(
-            self.step_name, [self.test_material], self.key, use_dsse=True
+            self.step_name,
+            [self.test_material],
+            signer=self.signer,
+            use_dsse=True,
         )
         link_metadata = Envelope.load(self.link_name_unfinished)
         link_metadata.verify_signature(self.key)
         os.remove(self.link_name_unfinished)
 
 
 class TestInTotoRecordStop(unittest.TestCase, TmpDirMixin):
@@ -1100,20 +1088,18 @@
 
     @classmethod
     def setUpClass(cls):
         """Create and change into temporary directory, generate two key pairs
         and dummy product."""
         cls.set_up_test_dir()
 
-        cls.key_path = "test-key"
-        cls.key_path2 = "test-key2"
-        generate_and_write_unencrypted_rsa_keypair(cls.key_path)
-        generate_and_write_unencrypted_rsa_keypair(cls.key_path2)
-        cls.key = import_rsa_privatekey_from_file(cls.key_path)
-        cls.key2 = import_rsa_privatekey_from_file(cls.key_path2)
+        cls.signer = SignerStore.rsa
+        cls.key = SignerStore.rsa_pub
+        cls.signer2 = SignerStore.ecdsa
+        cls.key2 = SignerStore.ecdsa_pub
 
         cls.step_name = "test-step"
         cls.link_name = "{}.{:.8}.link".format(cls.step_name, cls.key["keyid"])
         cls.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(
             step_name=cls.step_name, keyid=cls.key["keyid"]
         )
 
@@ -1122,104 +1108,109 @@
 
     @classmethod
     def tearDownClass(cls):
         cls.tear_down_test_dir()
 
     def test_create_metadata_with_expected_product(self):
         """Test record stop records expected product."""
-        in_toto_record_start(self.step_name, [], self.key)
-        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
+        in_toto_record_stop(
+            self.step_name, [self.test_product], signer=self.signer
+        )
         link = Metablock.load(self.link_name)
         self.assertEqual(list(link.signed.products.keys()), [self.test_product])
         os.remove(self.link_name)
 
     def test_compare_metadata_with_and_without_metadata_directory(self):
         """Test record stop with and without metadata directory,
         compare the expected product"""
         tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
-        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
         in_toto_record_stop(
             self.step_name,
             [self.test_product],
-            self.key,
+            signer=self.signer,
             metadata_directory=tmp_dir,
         )
         link_path = os.path.join(tmp_dir, self.link_name)
         link_with_md = Metablock.load(link_path)
 
-        in_toto_record_start(self.step_name, [], self.key)
-        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
+        in_toto_record_stop(
+            self.step_name, [self.test_product], signer=self.signer
+        )
         link_without_md = Metablock.load(self.link_name)
         self.assertEqual(link_with_md.signed, link_without_md.signed)
         os.remove(link_path)
         os.remove(self.link_name)
 
     def test_create_metadata_with_expected_cwd(self):
         """Test record start/stop run, verify cwd."""
         in_toto_record_start(
-            self.step_name, [], self.key, record_environment=True
+            self.step_name, [], signer=self.signer, record_environment=True
+        )
+        in_toto_record_stop(
+            self.step_name, [self.test_product], signer=self.signer
         )
-        in_toto_record_stop(self.step_name, [self.test_product], self.key)
         link = Metablock.load(self.link_name)
         self.assertEqual(
             link.signed.environment["workdir"], os.getcwd().replace("\\", "/")
         )
         os.remove(self.link_name)
 
     def test_create_metadata_verify_signature(self):
         """Test record start creates metadata with expected signature."""
-        in_toto_record_start(self.step_name, [], self.key)
-        in_toto_record_stop(self.step_name, [], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
+        in_toto_record_stop(self.step_name, [], signer=self.signer)
         link = Metablock.load(self.link_name)
         link.verify_signature(self.key)
         os.remove(self.link_name)
 
     def test_replace_unfinished_metadata(self):
         """Test record stop removes unfinished file and creates link file."""
-        in_toto_record_start(self.step_name, [], self.key)
-        in_toto_record_stop(self.step_name, [], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
+        in_toto_record_stop(self.step_name, [], signer=self.signer)
         with self.assertRaises(IOError):
             # pylint: disable-next=consider-using-with
             open(self.link_name_unfinished, "r", encoding="utf8")
         self.assertTrue(os.path.isfile(self.link_name))
         os.remove(self.link_name)
 
     def test_missing_unfinished_file(self):
         """Test record stop exits on missing unfinished file, no link recorded."""
         with self.assertRaises(IOError):
-            in_toto_record_stop(self.step_name, [], self.key)
+            in_toto_record_stop(self.step_name, [], signer=self.signer)
         with self.assertRaises(IOError):
             # pylint: disable-next=consider-using-with
             open(self.link_name, "r", encoding="utf8")
 
     def test_wrong_signature_in_unfinished_metadata(self):
         """Test record stop exits on wrong signature, no link recorded."""
-        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_start(self.step_name, [], signer=self.signer)
         link_name = UNFINISHED_FILENAME_FORMAT.format(
             step_name=self.step_name, keyid=self.key["keyid"]
         )
         changed_link_name = UNFINISHED_FILENAME_FORMAT.format(
             step_name=self.step_name, keyid=self.key2["keyid"]
         )
         os.rename(link_name, changed_link_name)
         with self.assertRaises(SignatureVerificationError):
-            in_toto_record_stop(self.step_name, [], self.key2)
+            in_toto_record_stop(self.step_name, [], signer=self.signer2)
         with self.assertRaises(IOError):
             # pylint: disable-next=consider-using-with
             open(self.link_name, "r", encoding="utf8")
         os.rename(changed_link_name, link_name)
         os.remove(self.link_name_unfinished)
 
     def test_no_key_arguments(self):
         """Test record stop without passing one required key argument."""
         with self.assertRaises(ValueError):
             in_toto_record_stop(
                 self.step_name,
                 [],
-                signing_key=None,
                 gpg_keyid=None,
                 gpg_use_default=False,
             )
 
     def test_normalize_line_endings(self):
         """Test cross-platform line ending normalization."""
         paths = []
@@ -1230,18 +1221,24 @@
                 paths.append(path)
                 os.write(fd, b"hello" + line_ending + b"toto")
                 os.close(fd)
 
             # Call in_toto_record start and stop and record artifacts as
             # materials and products with line ending normalization on
             in_toto_record_start(
-                self.step_name, paths, self.key, normalize_line_endings=True
+                self.step_name,
+                paths,
+                signer=self.signer,
+                normalize_line_endings=True,
             )
             in_toto_record_stop(
-                self.step_name, paths, self.key, normalize_line_endings=True
+                self.step_name,
+                paths,
+                signer=self.signer,
+                normalize_line_endings=True,
             )
             link = Metablock.load(self.link_name).signed
 
             # Check that all three hashes in materials and products are equal
             for artifact_dict in [link.materials, link.products]:
                 hash_dicts = list(artifact_dict.values())
                 self.assertTrue(hash_dicts[1:] == hash_dicts[:-1])
@@ -1250,52 +1247,59 @@
         finally:
             for path in paths:
                 os.remove(path)
 
     def test_nonexistent_directory(self):
         """Test record stop with nonexistent metadata directory"""
         with self.assertRaises(FileNotFoundError):
-            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_start(self.step_name, [], signer=self.signer)
             in_toto_record_stop(
                 self.step_name,
                 [],
-                self.key,
+                signer=self.signer,
                 metadata_directory="nonexistentDir",
             )
 
     def test_not_a_directory(self):
         """Test record stop, passed metadata directory is not a dir"""
         fd, path = tempfile.mkstemp()
         os.write(fd, b"hello in-toto")
         os.close(fd)
         # Windows will raise FileNotFoundError instead of NotADirectoryError
         with self.assertRaises((NotADirectoryError, FileNotFoundError)):
-            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_start(self.step_name, [], signer=self.signer)
             in_toto_record_stop(
-                self.step_name, [], self.key, metadata_directory=path
+                self.step_name, [], signer=self.signer, metadata_directory=path
             )
         os.remove(path)
 
     @unittest.skipIf(os.name == "nt", "chmod doesn't work properly on Windows")
     def test_read_only_metadata_directory(self):
         """Test record stop with read only metadata directory"""
         tmp_dir = os.path.realpath(tempfile.mkdtemp())
         # make the directory read only
         os.chmod(tmp_dir, stat.S_IREAD)
         with self.assertRaises(PermissionError):
-            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_start(self.step_name, [], signer=self.signer)
             in_toto_record_stop(
-                self.step_name, [], self.key, metadata_directory=tmp_dir
+                self.step_name,
+                [],
+                signer=self.signer,
+                metadata_directory=tmp_dir,
             )
         os.rmdir(tmp_dir)
 
     def test_created_metadata_using_dsse(self):
         """Test record stop records created metadata with dsse."""
-        in_toto_record_start(self.step_name, [], self.key, use_dsse=True)
-        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        in_toto_record_start(
+            self.step_name, [], signer=self.signer, use_dsse=True
+        )
+        in_toto_record_stop(
+            self.step_name, [self.test_product], signer=self.signer
+        )
 
         link_metadata = Envelope.load(self.link_name)
         link_metadata.verify_signature(self.key)
 
         link = link_metadata.get_payload()
         self.assertEqual(list(link.products.keys()), [self.test_product])
         os.remove(self.link_name)
@@ -1311,20 +1315,20 @@
         environment = {
             "variables": "ENV_NAME=ENV_VALUE",
             "filesystem": "<filesystem info>",
             "workdir": "./",
         }
 
         in_toto_record_start(
-            self.step_name, [], self.key, record_environment=True
+            self.step_name, [], signer=self.signer, record_environment=True
         )
         in_toto_record_stop(
             self.step_name,
             [self.test_product],
-            self.key,
+            signer=self.signer,
             command=command,
             byproducts=byproducts,
             environment=environment,
         )
         link = Metablock.load(self.link_name)
         self.assertEqual(link.signed.command, command)
         self.assertDictEqual(link.signed.byproducts, byproducts)
@@ -1404,25 +1408,20 @@
 
 class TestSigner(unittest.TestCase, TmpDirMixin):
     """Test signer argument in runlib API functions (run, record)."""
 
     @classmethod
     def setUpClass(cls):
         cls.set_up_test_dir()  # teardown is called implicitly
-        keys = Path(__file__).parent / "demo_files"
 
-        rsa = "alice"
-        rsa_priv = import_rsa_privatekey_from_file(str(keys / rsa))
-        cls.rsa_pub = import_rsa_publickey_from_file(str(keys / f"{rsa}.pub"))
-        cls.rsa_signer = CryptoSigner.from_securesystemslib_key(rsa_priv)
-
-        ed = "danny"
-        ed_priv = import_ed25519_privatekey_from_file(str(keys / ed))
-        cls.ed_pub = import_ed25519_publickey_from_file(str(keys / f"{ed}.pub"))
-        cls.ed_signer = CryptoSigner.from_securesystemslib_key(ed_priv)
+        cls.rsa_pub = SignerStore.rsa_pub
+        cls.rsa_signer = SignerStore.rsa
+
+        cls.ed_pub = SignerStore.ed25519_pub
+        cls.ed_signer = SignerStore.ed25519
 
     def test_run(self):
         # Successfully create, sign and verify link
         link = in_toto_run("foo", [], [], [], signer=self.rsa_signer)
         self.assertIsNone(link.verify_signature(self.rsa_pub))
 
         # Fail with wrong verification key
@@ -1432,47 +1431,14 @@
         # Fail with bad signer arg
         class NoSigner:
             pass
 
         with self.assertRaises(ValueError):
             link = in_toto_run("foo", [], [], [], signer=NoSigner())
 
-        # Fail with incompatible signers
-        class BadSigner(Signer):
-            """Signer implementation w/o public_key attribute.
-            secure-systems-lab/securesystemslib#605
-            """
-
-            @classmethod
-            def from_priv_key_uri(
-                cls,
-                priv_key_uri,
-                public_key,
-                secrets_handler=None,
-            ):
-                pass
-
-            def sign(self, payload):
-                pass
-
-        # Fail with missing public_key attribute.
-        bad_signer = BadSigner()
-        with self.assertRaises(ValueError):
-            link = in_toto_run("foo", [], [], [], signer=bad_signer)
-
-        class NoKey:
-            pass
-
-        # Fail with wrong tpe on public_key attribute
-        bad_signer.public_key = (  # pylint: disable=attribute-defined-outside-init
-            NoKey()
-        )
-        with self.assertRaises(ValueError):
-            link = in_toto_run("foo", [], [], [], signer=bad_signer)
-
     def test_record(self):
         # Successfully create, sign and verify link
         in_toto_record_start("bar", [], signer=self.ed_signer)
         in_toto_record_stop("bar", [], signer=self.ed_signer)
         link_name = FILENAME_FORMAT.format(
             step_name="bar", keyid=self.ed_signer.public_key.keyid
         )
```

### Comparing `in_toto-2.3.0/tests/test_settings.py` & `in_toto-3.0.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/test_verifylib.py` & `in_toto-3.0.0/tests/test_verifylib.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 import shlex
 import shutil
 import tempfile
 import unittest
 from datetime import datetime, timezone
 from unittest.mock import patch
 
+import securesystemslib._gpg.functions
 import securesystemslib.exceptions
-import securesystemslib.gpg.functions
 from dateutil.relativedelta import relativedelta
-from securesystemslib.gpg.constants import have_gpg
-from securesystemslib.gpg.exceptions import KeyExpirationError
+from securesystemslib._gpg.constants import have_gpg
+from securesystemslib._gpg.exceptions import KeyExpirationError
 
 import in_toto.exceptions
 import in_toto.settings
 from in_toto.exceptions import (
     BadReturnValueError,
     LayoutExpiredError,
     RuleVerificationError,
@@ -1344,22 +1344,22 @@
     """
 
     @classmethod
     def setUpClass(cls):
         cls.set_up_test_dir()
         cls.set_up_gpg_keys()
 
-        master_key = securesystemslib.gpg.functions.export_pubkey(
+        master_key = securesystemslib._gpg.functions.export_pubkey(
             cls.gpg_key_0c8a17, cls.gnupg_home
         )
         sub_key = master_key["subkeys"][cls.gpg_key_d92439]
 
         # We need a gpg key without subkeys to test the normal scenario (M M M),
         # because keys with signing subkeys always use that subkey for signing.
-        master_key2 = securesystemslib.gpg.functions.export_pubkey(
+        master_key2 = securesystemslib._gpg.functions.export_pubkey(
             cls.gpg_key_768c43, cls.gnupg_home
         )
 
         cls.pub_key_dict = {
             cls.gpg_key_0c8a17: master_key,
             cls.gpg_key_d92439: sub_key,
             cls.gpg_key_768c43: master_key2,
@@ -1396,15 +1396,15 @@
     def test_verify_link_signature_thresholds__m_m_s__m_s_m__m_s_s(self):
         """Cannot sign with master key if subkey is present."""
         # The scenarios MMS, MSM, MSS are impossible because we cannot sign
         # with a master key, if there is a subkey with signing capability
         # GPG will always use that subkey.
         # Even if gpg would use the masterkey, these scenarios are not allowed,
         # see table in docstring of testcase
-        signature = securesystemslib.gpg.functions.create_signature(
+        signature = securesystemslib._gpg.functions.create_signature(
             b"data", self.gpg_key_0c8a17, self.gnupg_home
         )
 
         self.assertTrue(signature["keyid"] == self.gpg_key_d92439)
 
     def test_verify_link_signature_thresholds__s_m_m(self):
         """Allowed trust delegation."""
@@ -1448,15 +1448,15 @@
         link2.sign_gpg(subkey2, self.gnupg_home)
 
         chain_link_dict = {self.step_name: {subkey1: link1, subkey2: link2}}
 
         layout = Layout(
             steps=[Step(name=self.step_name, pubkeys=[masterkey], threshold=2)],
             keys={
-                masterkey: securesystemslib.gpg.functions.export_pubkey(
+                masterkey: securesystemslib._gpg.functions.export_pubkey(
                     masterkey, self.gnupg_home
                 )
             },
         )
         with self.assertRaises(ThresholdVerificationError):
             verify_link_signature_thresholds(layout, chain_link_dict)
 
@@ -1464,15 +1464,15 @@
         """Verify that a link signed with an expired key is skipped.
 
         NOTE: This test would be a better fit for `TestInTotoVerifyThresholds`,
         but we make use of `TestInTotoVerifyThresholdsGpgSubkeys`'s gpg setup here.
 
         """
         expired_key_id = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
-        expired_key = securesystemslib.gpg.functions.export_pubkey(
+        expired_key = securesystemslib._gpg.functions.export_pubkey(
             expired_key_id, self.gnupg_home
         )
 
         # Chain link dict containing a single link for a single step
         # The link's signature is (supposedly) signed by an expired key and
         # hence does not count towards the link threshold as defined in the layout.
         chain_link_dict = {
```

### Comparing `in_toto-2.3.0/tests/demo_dsse_files/demo.layout.template` & `in_toto-3.0.0/tests/demo_dsse_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_dsse_files/package.2f89b927.link` & `in_toto-3.0.0/tests/demo_dsse_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_dsse_files/write-code.776a00e2.link` & `in_toto-3.0.0/tests/demo_dsse_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files/demo.layout.template` & `in_toto-3.0.0/tests/demo_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files/package.2f89b927.link` & `in_toto-3.0.0/tests/demo_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files/write-code.776a00e2.link` & `in_toto-3.0.0/tests/demo_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files_gpg/demo.layout.template` & `in_toto-3.0.0/tests/demo_files_gpg/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files_gpg/package.7b3abb26.link` & `in_toto-3.0.0/tests/demo_files_gpg/package.7b3abb26.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/demo_files_gpg/write-code.8288ef56.link` & `in_toto-3.0.0/tests/demo_files_gpg/write-code.8288ef56.link`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `in_toto-3.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/dsa/pubring.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/dsa/random_seed` & `in_toto-3.0.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/dsa/secring.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/dsa/trustdb.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/rsa/pubring.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/rsa/random_seed` & `in_toto-3.0.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/rsa/secring.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/gpg_keyrings/rsa/trustdb.gpg` & `in_toto-3.0.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_common.py` & `in_toto-3.0.0/tests/models/test_common.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_envelope.py` & `in_toto-3.0.0/tests/models/test_envelope.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_inspection.py` & `in_toto-3.0.0/tests/models/test_inspection.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_layout.py` & `in_toto-3.0.0/tests/models/test_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,57 +245,28 @@
 
         self.layout.expires = "2016-11-18T16:44:55Z"
         self.layout._validate_expires()
         self.layout.validate()
 
     def test_wrong_key_dictionary(self):
         """Test that the keys dictionary is properly populated."""
-        rsa_key_one = securesystemslib.keys.generate_rsa_key()
-        rsa_key_two = securesystemslib.keys.generate_rsa_key()
-
-        # FIXME: attr.ib reutilizes the default dictionary, so future constructor
-        # are not empty...
-        self.layout.keys = {"kek": rsa_key_one}
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            self.layout._validate_keys()
-
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            self.layout.validate()
-
-        self.layout.keys = {}
-        self.layout.keys[rsa_key_two["keyid"]] = "kek"
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            self.layout._validate_keys()
-
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            self.layout.validate()
-
         # ... more invalid keys
         for invalid_keys in [
             False,  # must be a dict
             {1234: {}},  # keyid must be string
             {"xyz": {}},  # keyid must be hex
+            {"deadbeef": "key must be a dict"},
             {"deadbeef": {"missing": "'keyval' field"}},
         ]:
             self.layout.keys = invalid_keys
             with self.assertRaises(securesystemslib.exceptions.FormatError):
                 self.layout._validate_keys()
 
-        self.layout.keys[rsa_key_two["keyid"]] = "kek"
-        with self.assertRaises(securesystemslib.exceptions.FormatError):
-            self.layout.validate()
-
-        self.layout.keys = {}
-        del rsa_key_one["keyval"]["private"]
-        del rsa_key_two["keyval"]["private"]
-        self.layout.keys[rsa_key_one["keyid"]] = rsa_key_one
-        self.layout.keys[rsa_key_two["keyid"]] = rsa_key_two
-
-        self.layout._validate_keys()
-        self.layout.validate()
+            with self.assertRaises(securesystemslib.exceptions.FormatError):
+                self.layout.validate()
 
     def test_wrong_steps_list(self):
         """Check that the validate method checks the steps' correctness."""
         self.layout.steps = "not-a-step"
         with self.assertRaises(securesystemslib.exceptions.FormatError):
             self.layout.validate()
 
@@ -352,32 +323,32 @@
             self.layout.validate()
 
         self.layout.step = [Step(name="name"), Step(name="othername")]
         self.layout.inspect = [Inspection(name="thirdname")]
         self.layout.validate()
 
     def test_import_step_metadata_wrong_type(self):
-        functionary_key = securesystemslib.keys.generate_rsa_key()
         name = "name"
+        functionary_keyid = (
+            "776a00e29f3559e0141b3b096f696abc6cfb0c657ab40f441132b345b08453f5"
+        )
 
         # Create and dump a link file with a wrong type
         link_name = in_toto.models.link.FILENAME_FORMAT.format(
-            step_name=name, keyid=functionary_key["keyid"]
+            step_name=name, keyid=functionary_keyid
         )
 
         link_path = os.path.abspath(link_name)
         link = in_toto.models.link.Link(name=name)
         metadata = Metablock(signed=link)
         metadata.signed._type = "wrong-type"
         metadata.dump(link_path)
 
         # Add the single step to the test layout and try to read the failing link
-        self.layout.steps.append(
-            Step(name=name, pubkeys=[functionary_key["keyid"]])
-        )
+        self.layout.steps.append(Step(name=name, pubkeys=[functionary_keyid]))
 
         with self.assertRaises(securesystemslib.exceptions.FormatError):
             in_toto.verifylib.load_links_for_layout(self.layout, ".")
 
         # Clean up
         os.remove(link_path)
```

### Comparing `in_toto-2.3.0/tests/models/test_link.py` & `in_toto-3.0.0/tests/models/test_link.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_metadata.py` & `in_toto-3.0.0/tests/models/test_metadata.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_signer.py` & `in_toto-3.0.0/tests/models/test_signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 <Purpose>
   Test GPGKey, GPGSigner and GPGSignature class methods.
 """
 
 import unittest
 from pathlib import Path
 
+from securesystemslib._gpg.constants import have_gpg
+from securesystemslib._gpg.functions import export_pubkey
 from securesystemslib.exceptions import (
     UnverifiedSignatureError,
     VerificationError,
 )
-from securesystemslib.gpg.constants import have_gpg
-from securesystemslib.gpg.functions import export_pubkey
 
 from in_toto.models._signer import (
     GPGKey,
     GPGSignature,
     GPGSigner,
     load_crypto_signer_from_pkcs8_file,
 )
```

### Comparing `in_toto-2.3.0/tests/models/test_step.py` & `in_toto-3.0.0/tests/models/test_step.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/models/test_supply_chain_item.py` & `in_toto-3.0.0/tests/models/test_supply_chain_item.py`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/pems/rsa_private_encrypted.pem` & `in_toto-3.0.0/tests/pems/rsa_private_encrypted.pem`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/pems/rsa_private_unencrypted.pem` & `in_toto-3.0.0/tests/pems/rsa_private_unencrypted.pem`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/scripts/expr` & `in_toto-3.0.0/tests/scripts/expr`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/scripts/tar` & `in_toto-3.0.0/tests/scripts/tar`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/tests/scripts/touch` & `in_toto-3.0.0/tests/scripts/touch`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/.gitignore` & `in_toto-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/LICENSE` & `in_toto-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/README.md` & `in_toto-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `in_toto-2.3.0/pyproject.toml` & `in_toto-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -38,29 +38,18 @@
     "Topic :: Software Development",
 ]
 dependencies = [
     "attrs",
     "iso8601",
     "pathspec",
     "python-dateutil",
-    "securesystemslib[crypto]~=0.31.0",
+    "securesystemslib[crypto]~=1.0",
 ]
 dynamic = ["version"]
 
-[project.optional-dependencies]
-# Install pynacl as optional dependency to use with securesystemslib, as a
-# workaround for `"ssl-pynacl": ["securesystemslib[pynacl]>=0.11.3"]`,
-# which currently is not supported in "extra_require" (see pypa/pip#4957).
-# TODO: Keep track of changes (version, additional requirements) under the
-# "pynacl" key in securesystemslib's setup.py.
-# https://github.com/secure-systems-lab/securesystemslib/blob/master/setup.py#L101
-pynacl = [
-    "pynacl>1.2.0",
-]
-
 [project.scripts]
 in-toto-mock = "in_toto.in_toto_mock:main"
 in-toto-record = "in_toto.in_toto_record:main"
 in-toto-run = "in_toto.in_toto_run:main"
 in-toto-sign = "in_toto.in_toto_sign:main"
 in-toto-verify = "in_toto.in_toto_verify:main"
 in-toto-match-products = "in_toto.in_toto_match_products:main"
```

### Comparing `in_toto-2.3.0/PKG-INFO` & `in_toto-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: in-toto
-Version: 2.3.0
+Version: 3.0.0
 Summary: A framework to define and secure the integrity of software supply chains
 Project-URL: Bug Reports, https://github.com/in-toto/in-toto/issues
 Project-URL: Homepage, https://in-toto.io
 Project-URL: Source, https://github.com/in-toto/in-toto
 Author-email: "New York University: Secure Systems Lab" <in-toto-dev@googlegroups.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,17 +26,15 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: ~=3.8
 Requires-Dist: attrs
 Requires-Dist: iso8601
 Requires-Dist: pathspec
 Requires-Dist: python-dateutil
-Requires-Dist: securesystemslib[crypto]~=0.31.0
-Provides-Extra: pynacl
-Requires-Dist: pynacl>1.2.0; extra == 'pynacl'
+Requires-Dist: securesystemslib[crypto]~=1.0
 Description-Content-Type: text/markdown
 
 # in-toto ![Build](https://github.com/in-toto/in-toto/workflows/Run%20in-toto%20tests%20and%20linter/badge.svg) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1523/badge)](https://bestpractices.coreinfrastructure.org/projects/1523) [![Documentation Status](https://readthedocs.org/projects/in-toto/badge/?version=latest)](https://in-toto.readthedocs.io/en/latest/?badge=latest)
 
 in-toto provides a framework to protect the integrity of the software supply chain. It does so by verifying that each task in the chain is carried out as planned, by authorized personnel only, and that the product is not tampered with in transit.
 
 in-toto requires a **project owner** to create a **layout**. A layout lists the sequence of **steps** of the software supply chain, and the **functionaries** authorized to perform these steps.
```

