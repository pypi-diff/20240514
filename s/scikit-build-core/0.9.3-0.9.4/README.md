# Comparing `tmp/scikit_build_core-0.9.3.tar.gz` & `tmp/scikit_build_core-0.9.4.tar.gz`

## Comparing `scikit_build_core-0.9.3.tar` & `scikit_build_core-0.9.4.tar`

### file list

```diff
@@ -1,335 +1,335 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.gitattributes
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.packit.yaml
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.readthedocs.yml
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/noxfile.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/.fmf/version
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/plans/examples.fmf
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/plans/rpminspect.fmf
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/codecov.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/build.md
--rw-r--r--   0        0        0    31204 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/changelog.md
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/cmakelists.md
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/conf.py
--rw-r--r--   0        0        0    19684 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/configuration.md
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/crosscompile.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/faqs.md
--rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/getting_started.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/index.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/man.md
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/migration_guide.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/.fmf/version
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.hatch.rst
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/main.fmf
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/test.sh
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/main.fmf
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/main.fmf
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/main.fmf
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/abi3/main.fmf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/c/main.fmf
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/cython/main.fmf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/fortran/main.fmf
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/nanobind/example.cpp
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/nanobind/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/nanobind/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/pybind11/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/swig/main.fmf
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/ext/conftabs.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/plugins/hatchling.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/docs/plugins/setuptools.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_editable.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/generate.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/metadata.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/__main__.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/hatch/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/hatch/hooks.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/hatch/plugin.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/metadata/regex.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0    20596 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/scikit-build.schema.json
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/documentation.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/json_schema.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_docs.py
--rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_schema.py
--rw-r--r--   0        0        0    21975 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/conftest.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/constraints.txt
--rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_builder.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_cmake_config.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_custom_modules.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_editable.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_editable_redirect.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_editable_unit.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_file_processor.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_fileapi.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_generator_default.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_get_requires.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_hatchling.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_json_schema.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_logging.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_name_main.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_printouts.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_pyproject_purelib.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_schema.py
--rw-r--r--   0        0        0    19424 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_settings.py
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_settings_overrides.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_shutil.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_simple_pure.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_simplest_c.py
--rw-r--r--   0        0        0    18913 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/.gitignore
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/pyproject.toml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/cpp/CMakeLists.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/cpp/example.cpp
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/src/hatchling_example/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/hatchling/src/hatchling_example/_core.pyi
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/CMakeLists.txt
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/pyproject.toml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/python/shared_pkg/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/python/shared_pkg/py_module.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/src/shared_pkg/c_module.c
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/sdist_config/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/sdist_config/CMakeLists.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/sdist_config/input.cmake
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/sdist_config/main.cpp
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/sdist_config/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_purelib_package/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_script_with_flags/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_script_with_flags/LICENSE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_script_with_flags/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_script_with_flags/src/main.c
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/LICENSE
--rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/README.md
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    19706 2020-02-02 00:00:00.000000 scikit_build_core-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.gitattributes
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.packit.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.readthedocs.yml
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/noxfile.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/.fmf/version
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/examples.fmf
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/rpminspect.fmf
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/codecov.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/release.yml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/build.md
+-rw-r--r--   0        0        0    32025 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/changelog.md
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/cmakelists.md
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/conf.py
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/configuration.md
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/crosscompile.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/faqs.md
+-rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/getting_started.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/man.md
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/migration_guide.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/.fmf/version
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.hatch.rst
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/test.sh
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/main.fmf
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/main.fmf
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/main.fmf
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/ext/conftabs.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/plugins/hatchling.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/plugins/setuptools.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_editable.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/generate.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/metadata.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/__main__.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/hooks.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/plugin.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/regex.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0    21268 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/documentation.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/json_schema.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_docs.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_schema.py
+-rw-r--r--   0        0        0    21975 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/conftest.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/constraints.txt
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_builder.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable_redirect.py
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable_unit.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_generator_default.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_get_requires.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_hatchling.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_json_schema.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_logging.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_name_main.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_printouts.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_program_search.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_purelib.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_schema.py
+-rw-r--r--   0        0        0    19424 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_settings.py
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_settings_overrides.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_shutil.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/.gitignore
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/pyproject.toml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/cpp/example.cpp
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/src/hatchling_example/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/src/hatchling_example/_core.pyi
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/CMakeLists.txt
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/pyproject.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/py_module.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/c_module.c
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/CMakeLists.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/input.cmake
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/main.cpp
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_purelib_package/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/src/main.c
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/LICENSE
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/README.md
+-rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/PKG-INFO
```

### Comparing `scikit_build_core-0.9.3/.packit.yaml` & `scikit_build_core-0.9.4/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/.pre-commit-config.yaml` & `scikit_build_core-0.9.4/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         args: ["--pytest-test-first"]
         exclude: "^tests/packages/"
       - id: requirements-txt-fixer
       - id: trailing-whitespace
         exclude: "^tests"
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.1
+    rev: v0.4.4
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
@@ -54,15 +54,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests|src/scikit_build_core/resources/scikit-build.schema.json"
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         exclude: |
           (?x)^(
             tests/packages/simplest_c/src/simplest/__init__.py|
             tests/packages/dynamic_metadata/src/dynamic/__init__.py|
             tests/packages/.*/setup.py
@@ -84,15 +84,15 @@
           - pytest<8
           - rich
           - setuptools-scm
           - tomli
           - types-setuptools>=69.2
 
   - repo: https://github.com/henryiii/check-sdist
-    rev: "v0.1.3"
+    rev: "v1.0.0rc2"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
           - hatch-vcs
 
@@ -115,7 +115,21 @@
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
       - id: disallow-expressions
         name: Disallow expressions
         language: pygrep
         entry: tool\.cmake
         exclude: .pre-commit-config.yaml
+
+  - repo: https://github.com/henryiii/validate-pyproject-schema-store
+    rev: 2024.04.29
+    hooks:
+      - id: validate-pyproject
+
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.3
+    hooks:
+      - id: check-dependabot
+      - id: check-github-workflows
+      - id: check-readthedocs
+      - id: check-metaschema
+        files: \.schema\.json
```

### Comparing `scikit_build_core-0.9.3/noxfile.py` & `scikit_build_core-0.9.4/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 @nox.session(reuse_venv=True)
 def pylint(session: nox.Session) -> None:
     """
     Run PyLint.
     """
     # This needs to be installed into the package environment, and is slower
     # than a pre-commit check
-    session.install("-e.[dev,test,test-meta]", "pylint")
+    session.install("-e.[dev,test,test-meta]", "pylint==3.2.*")
+    session.run("pylint", "--version")
     session.run("pylint", "scikit_build_core", *session.posargs)
 
 
 def _run_tests(
     session: nox.Session,
     *,
     install_args: Sequence[str] = (),
```

### Comparing `scikit_build_core-0.9.3/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.9.4/.distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/.github/CONTRIBUTING.md` & `scikit_build_core-0.9.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/.github/workflows/cd.yml` & `scikit_build_core-0.9.4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/.github/workflows/ci.yml` & `scikit_build_core-0.9.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,15 @@
       - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - uses: pre-commit/action@v3.0.1
         with:
           extra_args: --hook-stage manual --all-files
       - name: Run PyLint
-        run: |
-          echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
-          pipx run nox -s pylint
+        run: pipx run nox -s pylint -- --output-format=github
       - name: Run nox generator
         run: |
           pipx run nox -s generate_schema -s readme
           git diff --exit-code
 
   checks:
     name:
@@ -171,14 +169,33 @@
 
       - name: Show installed packages
         run: pip list
 
       - name: Test min package
         run: pytest -ra --showlocals -Wdefault
 
+  manylinux:
+    name: Manylinux on 🐍 3.13 • Free-threaded
+    runs-on: ubuntu-latest
+    timeout-minutes: 40
+    container: quay.io/pypa/musllinux_1_2_x86_64:latest
+    steps:
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Prepare venv
+        run: python3.13t -m venv /venv
+
+      - name: Install deps
+        run: /venv/bin/pip install -e .[test] ninja
+
+      - name: Test package
+        run: /venv/bin/pytest
+
   cygwin:
     name: Tests on 🐍 3.9 • cygwin
     runs-on: windows-latest
     timeout-minutes: 40
 
     steps:
       - uses: actions/checkout@v4
```

### Comparing `scikit_build_core-0.9.3/docs/build.md` & `scikit_build_core-0.9.4/docs/build.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/changelog.md` & `scikit_build_core-0.9.4/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # Changelog
 
+## Version 0.9.4
+
+This version supports the newly available free-threading variant of Python
+3.13b1 (mostly related to skipping the stable ABI). We test this via the
+manylinux/musllinux images. There's also a new feature requested by third-party
+packagers; the ability to pass args directly to the build tool
+
+Features:
+
+- Add `build.tool-args` by @henryiii in #733
+
+Fixes:
+
+- Support free-threaded builds of Python 3.13+ by @henryiii in #741
+- Slightly better stable ABI behavior using PyPy by @henryiii in #741
+
+Documentation:
+
+- Fix example of configuration overrides in configuration.md by @wu-vincent in
+  #739
+- Update stable ABI instructions by @henryiii in #740
+
+CI and testing:
+
+- Use pylint 3.2, gha reporter by @henryiii in #745
+- Some minor improvements to running tests on some systems by @henryiii in #741
+
 ## Version 0.9.3
 
 This version ensures the Hatchling plugin correctly indicates editable mode is
 not yet supported, supports `CMAKE_ARGS` that have spaces, and has a bit of
 other minor cleanup.
 
 Fixes:
```

### Comparing `scikit_build_core-0.9.3/docs/cmakelists.md` & `scikit_build_core-0.9.4/docs/cmakelists.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 You always want to find at least `Interpreter` and the "Module" component of the
 "Development" package. You do not want to find the entire "Development" package,
 as that include "Embed" component, which is not always present and is not
 related to making Python extension modules.
 
 If you are making a Limited ABI / Stable API package, you'll need the
-`Development.SABIModule` component instead. You can use the
+`Development.SABIModule` component instead (CMake 3.26+). You can use the
 `SKBUILD_LIMITED_API` variable to check to see if it was requested.
 
 <!-- prettier-ignore-start -->
 :::{warning}
 :name: soabi
 
 If you want to cross-compile to Windows ARM, you'll need to use
@@ -124,11 +124,30 @@
 find_package(Python REQUIRED COMPONENTS Interpreter Development.Module ${SKBUILD_SABI_COMPONENT})
 ```
 
 This will add this only if scikit-build-core is driving the compilation and is
 targeting ABI3. If you want to support limited ABI from outside
 scikit-build-core, look into the `OPTIONAL_COMPONENTS` flag for `find_package`.
 
+When defining your module, if you only support the Stable ABI after some point,
+you should use (for example for 3.11):
+
+```cmake
+if(NOT "${SKBUILD_SABI_COMPONENT}" STREQUAL "")
+  python_add_library(some_ext MODULE WITH_SOABI USE_SABI 3.11 ...)
+else()
+  python_add_library(some_ext MODULE WITH_SOABI ...)
+endif()
+```
+
+This will define `Py_LIMITED_API` for you. If you want to support building
+directly from CMake, you need to protect this for Python version,
+`Python_INTERPRETER_ID STREQUAL Python`, and free-threading Python 3.13+ doesn't
+support ABI3 either.
+
+If you are using `nanobind`'s `nanobind_add_module`, the `STABLE_ABI` flag does
+this automatically for you for 3.12+.
+
 ## Future additions
 
 Scikit-build-core does not include helpers for F2Py or Cython like scikit-build
 classic yet. These will be carefully reimagined soon.
```

### Comparing `scikit_build_core-0.9.3/docs/conf.py` & `scikit_build_core-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/configuration.md` & `scikit_build_core-0.9.4/docs/configuration.md`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,24 @@
 You can also specify only specific targets to build (leaving this off builds the
 default targets):
 
 ```{conftabs} cmake.targets ["python"]
 
 ```
 
+You can pass raw arguments directly to the build tool, as well:
+
+```{conftabs} build.tool-args ["-j12", "-l13"]
+
+```
+
+```{versionadded} 0.9.4
+
+```
+
 ## Dynamic metadata
 
 Scikit-build-core 0.3.0+ supports dynamic metadata with two built-in plugins.
 
 :::{warning}
 
 This is not ready for plugin development outside of scikit-build-core;
@@ -675,15 +685,15 @@
 
 At least one must be provided. Then you can specify any collection of valid
 options, and those will override if all the items in the `if` are true. They
 will match top to bottom, overriding previous matches. For example:
 
 ```toml
 [[tool.scikit-build.overrides]]
-if.sys-platform = "darwin"
+if.platform-system = "darwin"
 cmake.version = ">=3.18"
 ```
 
 If you use `if.any` instead of `if`, then the override is true if any one of the
 items in it are true.
 
 ## Full schema
```

### Comparing `scikit_build_core-0.9.3/docs/crosscompile.md` & `scikit_build_core-0.9.4/docs/crosscompile.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/faqs.md` & `scikit_build_core-0.9.4/docs/faqs.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/getting_started.md` & `scikit_build_core-0.9.4/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/index.md` & `scikit_build_core-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/migration_guide.md` & `scikit_build_core-0.9.4/docs/migration_guide.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.hatch.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.hatch.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.9.4/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/test.sh` & `scikit_build_core-0.9.4/docs/examples/test.sh`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.9.4/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.9.4/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.9.4/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.9.4/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.9.4/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/ext/conftabs.py` & `scikit_build_core-0.9.4/docs/ext/conftabs.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         ````
 
         `````
 
         ````{{tab}} Environment
 
         ```yaml
-        {env_name}: {joined_result}
+        {env_name}: "{joined_result}"
         ```
 
         ````
         """
         )
 
         content = nodes.container("")
```

### Comparing `scikit_build_core-0.9.3/docs/plugins/hatchling.md` & `scikit_build_core-0.9.4/docs/plugins/hatchling.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/docs/plugins/setuptools.md` & `scikit_build_core-0.9.4/docs/plugins/setuptools.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_logging.py` & `scikit_build_core-0.9.4/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.9.4/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/cmake.py` & `scikit_build_core-0.9.4/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/errors.py` & `scikit_build_core-0.9.4/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/program_search.py` & `scikit_build_core-0.9.4/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.9.4/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE` & `scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py` & `scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_editable.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_editable.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/generate.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/generate.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/metadata.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.9.4/src/scikit_build_core/build/wheel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/__main__.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def configure(
         self,
         *,
         defines: Mapping[str, str | bool],
         cache_entries: Mapping[str, str | Path] | None = None,
         name: str | None = None,
         version: Version | None = None,
-        limited_abi: bool | None = None,
+        limited_api: bool | None = None,
         configure_args: Iterable[str] = (),
     ) -> None:
         cmake_defines = {
             k: ("TRUE" if v else "FALSE") if isinstance(v, bool) else v
             for k, v in defines.items()
         }
 
@@ -158,24 +158,34 @@
         if name is not None:
             canonical_name = name.replace("-", "_").replace(".", "_")
             cache_config["SKBUILD_PROJECT_NAME"] = canonical_name
         if version is not None:
             cache_config["SKBUILD_PROJECT_VERSION"] = version.base_version
             cache_config["SKBUILD_PROJECT_VERSION_FULL"] = str(version)
 
-        if limited_abi is None:
+        if limited_api is None:
             if self.settings.wheel.py_api.startswith("cp3"):
                 target_minor_version = int(self.settings.wheel.py_api[3:])
-                limited_abi = target_minor_version <= sys.version_info.minor
+                limited_api = target_minor_version <= sys.version_info.minor
             else:
-                limited_abi = False
+                limited_api = False
+
+        if limited_api and sys.implementation.name != "cpython":
+            limited_api = False
+            logger.info("PyPy doesn't support the Limited API, ignoring")
+
+        if limited_api and sysconfig.get_config_var("Py_GIL_DISABLED"):
+            limited_api = False
+            logger.info(
+                "Free-threaded Python doesn't support the Limited API currently, ignoring"
+            )
 
         python_library = get_python_library(self.config.env, abi3=False)
         python_sabi_library = (
-            get_python_library(self.config.env, abi3=True) if limited_abi else None
+            get_python_library(self.config.env, abi3=True) if limited_api else None
         )
         python_include_dir = get_python_include_dir()
         numpy_include_dir = get_numpy_include_dir()
 
         # Classic Find Python
         cache_config["PYTHON_EXECUTABLE"] = sys.executable
         cache_config["PYTHON_INCLUDE_DIR"] = python_include_dir
@@ -192,19 +202,19 @@
             if python_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_LIBRARY"] = python_library
             if python_sabi_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_SABI_LIBRARY"] = python_sabi_library
             if numpy_include_dir:
                 cache_config[f"{prefix}_NumPy_INCLUDE_DIR"] = numpy_include_dir
 
-        cache_config["SKBUILD_SOABI"] = get_soabi(self.config.env, abi3=limited_abi)
+        cache_config["SKBUILD_SOABI"] = get_soabi(self.config.env, abi3=limited_api)
 
         # Allow CMakeLists to detect this is supposed to be a limited ABI build
         cache_config["SKBUILD_SABI_COMPONENT"] = (
-            "Development.SABIModule" if limited_abi else ""
+            "Development.SABIModule" if limited_api else ""
         )
 
         if cache_entries:
             cache_config.update(cache_entries)
 
         self.config.init_cache(cache_config)
 
@@ -223,15 +233,19 @@
         )
 
         self.config.configure(
             defines=cmake_defines,
             cmake_args=[*self.get_cmake_args(), *configure_args],
         )
 
-    def build(self, build_args: list[str]) -> None:
+    def build(self, build_args: Sequence[str]) -> None:
+        build_tool_args = self.settings.build.tool_args
+        if build_tool_args:
+            build_args = [*build_args, "--", *build_tool_args]
+
         self.config.build(
             build_args=build_args,
             targets=self.settings.cmake.targets,
             verbose=self.settings.cmake.verbose,
         )
 
     def install(self, install_dir: Path) -> None:
```

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.9.4/src/scikit_build_core/builder/wheel_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import itertools
 import sys
+import sysconfig
 from typing import TYPE_CHECKING
 
 import packaging.tags
 
 from .._logging import logger
 from .macos import get_macosx_deployment_target
 
@@ -100,19 +101,20 @@
                     msg = f"Unexpected py-api, since platlib is set to false, must be Pythonless (e.g. py2.py3), not {py_api}"
                     raise AssertionError(msg)
 
                 minor = int(pyvers_new[0][3:])
                 if (
                     sys.implementation.name == "cpython"
                     and minor <= sys.version_info.minor
+                    and not sysconfig.get_config_var("Py_GIL_DISABLED")
                 ):
                     pyvers = pyvers_new
                     abi = "abi3"
                 else:
-                    msg = "Ignoring py-api, not a CPython interpreter ({}) or version (3.{}) is too high"
+                    msg = "Ignoring py-api, not a CPython interpreter ({}) or version (3.{}) is too high or free-threaded"
                     logger.debug(msg, sys.implementation.name, minor)
             elif all(x.startswith("py") and x[2:].isdecimal() for x in pyvers_new):
                 pyvers = pyvers_new
                 abi = "none"
             else:
                 msg = f"Unexpected py-api, must be abi3 (e.g. cp39) or Pythonless (e.g. py2.py3), not {py_api}"
                 raise AssertionError(msg)
```

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/hatch/plugin.py` & `scikit_build_core-0.9.4/src/scikit_build_core/hatch/plugin.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.9.4/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/metadata/regex.py` & `scikit_build_core-0.9.4/src/scikit_build_core/metadata/regex.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.9.4/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/scikit-build.schema.json` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/scikit-build.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955334894374417%*

 * *Differences: {"'properties'": "{'overrides': {'items': {'properties': {'inherit': {'properties': {'build': "*

 * *                 "OrderedDict([('type', 'object'), ('additionalProperties', False), ('properties', "*

 * *                 "OrderedDict([('tool-args', OrderedDict([('$ref', '#/$defs/inherit')]))]))])}}, "*

 * *                 "'build': OrderedDict([('$ref', '#/properties/build')])}}}, 'build': "*

 * *                 "OrderedDict([('type', 'object'), ('additionalProperties', False), ('properties', "*

 * *                 "OrderedDi […]*

```diff
@@ -85,14 +85,27 @@
                     "default": "3.26.1",
                     "description": "If CMake is less than this value, backport a copy of FindPython. Set to 0 disable this, or the empty string.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "build": {
+            "additionalProperties": false,
+            "properties": {
+                "tool-args": {
+                    "description": "Extra args to pass directly to the builder in the build step.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
+            },
+            "type": "object"
+        },
         "build-dir": {
             "default": "",
             "description": "The build directory. Defaults to a temporary directory, but can be set.",
             "type": "string"
         },
         "cmake": {
             "additionalProperties": false,
@@ -393,14 +406,17 @@
             "items": {
                 "additionalProperties": false,
                 "minProperties": 2,
                 "properties": {
                     "backport": {
                         "$ref": "#/properties/backport"
                     },
+                    "build": {
+                        "$ref": "#/properties/build"
+                    },
                     "build-dir": {
                         "$ref": "#/properties/build-dir"
                     },
                     "cmake": {
                         "$ref": "#/properties/cmake"
                     },
                     "editable": {
@@ -430,14 +446,23 @@
                                 "type": "object"
                             }
                         ]
                     },
                     "inherit": {
                         "additionalProperties": false,
                         "properties": {
+                            "build": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "tool-args": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
                             "cmake": {
                                 "additionalProperties": false,
                                 "properties": {
                                     "args": {
                                         "$ref": "#/$defs/inherit"
                                     },
                                     "define": {
```

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/documentation.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/documentation.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/json_schema.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_docs.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_docs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 __all__ = [
     "BackportSettings",
     "CMakeSettings",
     "EditableSettings",
     "GenerateSettings",
     "InstallSettings",
+    "BuildSettings",
     "LoggingSettings",
     "NinjaSettings",
     "SDistSettings",
     "ScikitBuildSettings",
     "WheelSettings",
 ]
 
@@ -229,14 +230,22 @@
     """
     Rebuild the project when the package is imported. The build-directory must
     be set.
     """
 
 
 @dataclasses.dataclass
+class BuildSettings:
+    tool_args: List[str] = dataclasses.field(default_factory=list)
+    """
+    Extra args to pass directly to the builder in the build step.
+    """
+
+
+@dataclasses.dataclass
 class InstallSettings:
     components: List[str] = dataclasses.field(default_factory=list)
     """
     The components to install. If empty, all default components are installed.
     """
 
     strip: Optional[bool] = None
@@ -277,14 +286,15 @@
     cmake: CMakeSettings = dataclasses.field(default_factory=CMakeSettings)
     ninja: NinjaSettings = dataclasses.field(default_factory=NinjaSettings)
     logging: LoggingSettings = dataclasses.field(default_factory=LoggingSettings)
     sdist: SDistSettings = dataclasses.field(default_factory=SDistSettings)
     wheel: WheelSettings = dataclasses.field(default_factory=WheelSettings)
     backport: BackportSettings = dataclasses.field(default_factory=BackportSettings)
     editable: EditableSettings = dataclasses.field(default_factory=EditableSettings)
+    build: BuildSettings = dataclasses.field(default_factory=BuildSettings)
     install: InstallSettings = dataclasses.field(default_factory=InstallSettings)
     generate: List[GenerateSettings] = dataclasses.field(default_factory=list)
 
     metadata: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
     """
     List dynamic metadata fields and hook locations in this table.
     """
```

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/skbuild_schema.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.9.4/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
         builder.config.build_type = "Debug" if self.debug else settings.cmake.build_type
 
         builder.configure(
             name=dist.get_name(),
             version=Version(dist.get_version()),
             defines={},
-            limited_abi=limited_api,
+            limited_api=limited_api,
             configure_args=configure_args,
         )
 
         # Set CMAKE_BUILD_PARALLEL_LEVEL to control the parallel build level
         # across all generators.
         build_args = []
```

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/conftest.py` & `scikit_build_core-0.9.4/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         ],
         check=True,
     )
     packages = [
         "build",
         "cython",
         "hatchling",
-        "pip>=23",
+        "pip>=23; python_version<'3.13'",
+        "pip>=24.1b1; python_version>='3.13'",
         "pybind11",
         "setuptools",
         "virtualenv",
         "wheel",
     ]
 
     if importlib.util.find_spec("cmake") is not None:
@@ -90,14 +91,16 @@
         self.env_dir = env_dir.resolve()
         self.platlib = Path(
             self.execute("import sysconfig; print(sysconfig.get_path('platlib'))")
         )
         self.purelib = Path(
             self.execute("import sysconfig; print(sysconfig.get_path('purelib'))")
         )
+        if sys.version_info >= (3, 13):
+            self.run("pip", "install", "-U", "pip>=24.1b1")
 
     @overload
     def run(self, *args: str, capture: Literal[True]) -> str: ...
 
     @overload
     def run(self, *args: str, capture: Literal[False] = ...) -> None: ...
```

### Comparing `scikit_build_core-0.9.3/tests/test_cmake_config.py` & `scikit_build_core-0.9.4/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_custom_modules.py` & `scikit_build_core-0.9.4/tests/test_custom_modules.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_dynamic_metadata.py` & `scikit_build_core-0.9.4/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_editable.py` & `scikit_build_core-0.9.4/tests/test_editable.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,22 @@
     package1 = PackageInfo(
         "cython_pxd_editable/pkg1",
     )
     tmp_path1 = tmp_path / "pkg1"
     tmp_path1.mkdir()
     process_package(package1, tmp_path1, monkeypatch)
 
-    isolated.install("pip>23", "cython", "scikit-build-core")
+    ninja = [
+        "ninja" for f in isolated.wheelhouse.iterdir() if f.name.startswith("ninja-")
+    ]
+    cmake = [
+        "cmake" for f in isolated.wheelhouse.iterdir() if f.name.startswith("cmake-")
+    ]
+
+    isolated.install("pip>23", "cython", "scikit-build-core", *ninja, *cmake)
 
     isolated.install(
         "-v",
         *config_mode_flags,
         "--no-build-isolation",
         *editable_flag,
         ".",
```

### Comparing `scikit_build_core-0.9.3/tests/test_editable_redirect.py` & `scikit_build_core-0.9.4/tests/test_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_editable_unit.py` & `scikit_build_core-0.9.4/tests/test_editable_unit.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_file_processor.py` & `scikit_build_core-0.9.4/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_fileapi.py` & `scikit_build_core-0.9.4/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_fortran.py` & `scikit_build_core-0.9.4/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_generator_default.py` & `scikit_build_core-0.9.4/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_get_requires.py` & `scikit_build_core-0.9.4/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_hatchling.py` & `scikit_build_core-0.9.4/tests/test_hatchling.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_json_schema.py` & `scikit_build_core-0.9.4/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_logging.py` & `scikit_build_core-0.9.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_module_dir.py` & `scikit_build_core-0.9.4/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_name_main.py` & `scikit_build_core-0.9.4/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_prepare_metadata.py` & `scikit_build_core-0.9.4/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_process_scripts.py` & `scikit_build_core-0.9.4/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_program_search.py` & `scikit_build_core-0.9.4/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_abi3.py` & `scikit_build_core-0.9.4/tests/test_pyproject_abi3.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 ABI_PKG = DIR / "packages/abi3_pyproject_ext"
 SYSCONFIGPLAT = sysconfig.get_platform()
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
-    sys.implementation.name == "pypy", reason="pypy does not support abi3"
-)
-@pytest.mark.skipif(
     sysconfig.get_platform().startswith(("msys", "mingw")),
     reason="abi3 FindPython on MSYS/MinGW reports not found",
 )
 def test_abi3_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(ABI_PKG)
@@ -30,32 +27,47 @@
         shutil.rmtree("dist")
     if Path("build").is_dir():
         shutil.rmtree("build")
 
     out = build_wheel(str(dist))
     (wheel,) = dist.glob("abi3_example-0.0.1-*.whl")
     assert wheel == dist / out
-    assert "-cp37-abi3-" in out
+    abi3 = sys.implementation.name == "cpython" and not sysconfig.get_config_var(
+        "Py_GIL_DISABLED"
+    )
+
+    if abi3:
+        assert "-cp37-abi3-" in out
+    else:
+        assert "-cp37-abi3-" not in out
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
 
         assert len(file_names) == 2
         assert "abi3_example-0.0.1.dist-info" in file_names
         file_names.remove("abi3_example-0.0.1.dist-info")
         (so_file,) = file_names
 
         if sysconfig.get_platform().startswith("win"):
-            assert so_file == "abi3_example.pyd"
+            if sys.implementation.name == "cpython":
+                assert so_file == "abi3_example.pyd"
+            else:
+                assert so_file.endswith(".pyd")
         elif sys.platform.startswith("cygwin"):
-            assert so_file == "abi3_example.abi3.dll"
-        else:
+            if abi3:
+                assert so_file == "abi3_example.abi3.dll"
+            else:
+                assert so_file != "abi3_example.abi3.dll"
+        elif abi3:
             assert so_file == "abi3_example.abi3.so"
+        else:
+            assert so_file != "abi3_example.abi3.so"
 
     virtualenv.install(wheel)
 
     output = virtualenv.execute(
         "import abi3_example; print(abi3_example.square(2))",
     )
     assert output.strip() == "4.0"
```

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.9.4/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_pep517.py` & `scikit_build_core-0.9.4/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_pep518.py` & `scikit_build_core-0.9.4/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_pep660.py` & `scikit_build_core-0.9.4/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_pyproject_purelib.py` & `scikit_build_core-0.9.4/tests/test_pyproject_purelib.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_schema.py` & `scikit_build_core-0.9.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_settings.py` & `scikit_build_core-0.9.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_settings_overrides.py` & `scikit_build_core-0.9.4/tests/test_settings_overrides.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_setuptools_abi3.py` & `scikit_build_core-0.9.4/tests/test_setuptools_abi3.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
     sys.implementation.name == "pypy", reason="pypy does not support abi3"
 )
 @pytest.mark.skipif(
+    sysconfig.get_config_var("Py_GIL_DISABLED"),
+    reason="Free-threaded Python does not support abi3",
+)
+@pytest.mark.skipif(
     SYSCONFIGPLAT.startswith(("msys", "mingw")),
     reason="abi3 FindPython on MSYS/MinGW reports not found",
 )
 def test_abi3_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
```

### Comparing `scikit_build_core-0.9.3/tests/test_setuptools_pep517.py` & `scikit_build_core-0.9.4/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_setuptools_pep518.py` & `scikit_build_core-0.9.4/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_shutil.py` & `scikit_build_core-0.9.4/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_simple_pure.py` & `scikit_build_core-0.9.4/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_simplest_c.py` & `scikit_build_core-0.9.4/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/test_skbuild_settings.py` & `scikit_build_core-0.9.4/tests/test_skbuild_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     assert not settings.experimental
     assert settings.minimum_version is None
     assert settings.build_dir == ""
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert not settings.editable.rebuild
     assert settings.editable.verbose
+    assert settings.build.tool_args == []
     assert settings.install.components == []
     assert settings.install.strip
     assert settings.generate == []
 
 
 def test_skbuild_settings_envvar(tmp_path: Path, monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(
@@ -95,14 +96,15 @@
     monkeypatch.setenv("SKBUILD_STRICT_CONFIG", "0")
     monkeypatch.setenv("SKBUILD_EXPERIMENTAL", "1")
     monkeypatch.setenv("SKBUILD_MINIMUM_VERSION", "0.1")
     monkeypatch.setenv("SKBUILD_CMAKE_VERBOSE", "TRUE")
     monkeypatch.setenv("SKBUILD_BUILD_DIR", "a/b/c")
     monkeypatch.setenv("SKBUILD_EDITABLE_REBUILD", "True")
     monkeypatch.setenv("SKBUILD_EDITABLE_VERBOSE", "False")
+    monkeypatch.setenv("SKBUILD_BUILD_TOOL_ARGS", "a;b")
     monkeypatch.setenv("SKBUILD_INSTALL_COMPONENTS", "a;b;c")
     monkeypatch.setenv("SKBUILD_INSTALL_STRIP", "False")
 
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text("", encoding="utf-8")
 
     config_settings: dict[str, list[str] | str] = {}
@@ -136,14 +138,15 @@
     assert settings.experimental
     assert settings.minimum_version == Version("0.1")
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.build.tool_args == ["a", "b"]
     assert settings.install.components == ["a", "b", "c"]
     assert not settings.install.strip
 
 
 @pytest.mark.parametrize("prefix", [True, False], ids=["skbuild", "noprefix"])
 def test_skbuild_settings_config_settings(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch, prefix: bool
@@ -181,14 +184,15 @@
         "strict-config": "false",
         "experimental": "1",
         "minimum-version": "0.1",
         "build-dir": "a/b/c",
         "editable.mode": "redirect",
         "editable.rebuild": "True",
         "editable.verbose": "False",
+        "build.tool-args": ["a", "b"],
         "install.components": ["a", "b", "c"],
         "install.strip": "True",
     }
 
     if prefix:
         config_settings = {f"skbuild.{k}": v for k, v in config_settings.items()}
 
@@ -221,14 +225,15 @@
     assert settings.experimental
     assert settings.minimum_version == Version("0.1")
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.build.tool_args == ["a", "b"]
     assert settings.install.components == ["a", "b", "c"]
     assert settings.install.strip
 
 
 def test_skbuild_settings_pyproject_toml(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch
 ):
@@ -265,14 +270,15 @@
             experimental = true
             minimum-version = "0.1"
             build-dir = "a/b/c"
             metadata.version.provider = "a"
             editable.mode = "redirect"
             editable.rebuild = true
             editable.verbose = false
+            build.tool-args = ["a", "b"]
             install.components = ["a", "b", "c"]
             install.strip = true
             [[tool.scikit-build.generate]]
             path = "a/b/c"
             template = "hello"
             [[tool.scikit-build.generate]]
             path = "d/e/f"
@@ -314,14 +320,15 @@
     assert settings.experimental
     assert settings.minimum_version == Version("0.1")
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {"version": {"provider": "a"}}
     assert settings.editable.mode == "redirect"
     assert settings.editable.rebuild
     assert not settings.editable.verbose
+    assert settings.build.tool_args == ["a", "b"]
     assert settings.install.components == ["a", "b", "c"]
     assert settings.install.strip
     assert settings.generate == [
         GenerateSettings(path=Path("a/b/c"), template="hello", location="install"),
         GenerateSettings(
             path=Path("d/e/f"), template_path=Path("g/h/i"), location="build"
         ),
```

### Comparing `scikit_build_core-0.9.3/tests/test_wheelfile_utils.py` & `scikit_build_core-0.9.4/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 find_package(
   Python
   COMPONENTS Interpreter Development.Module
   REQUIRED)
 
 add_custom_command(
-  OUTPUT src/pkg1/one.c
-  DEPENDS src/pkg1/one.pyx
+  OUTPUT "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c"
+  DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/src/pkg1/one.pyx"
   VERBATIM
   COMMAND
     Python::Interpreter -m cython
     "${CMAKE_CURRENT_SOURCE_DIR}/src/pkg1/one.pyx" --output-file
     "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c")
 
 python_add_library(one MODULE "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c"
```

### Comparing `scikit_build_core-0.9.3/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/hatchling/.gitignore` & `scikit_build_core-0.9.4/tests/packages/hatchling/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/hatchling/cpp/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/hatchling/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/hatchling/cpp/example.cpp` & `scikit_build_core-0.9.4/tests/packages/hatchling/cpp/example.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/navigate_editable/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/navigate_editable/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/navigate_editable/python/shared_pkg/py_module.py` & `scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/py_module.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/navigate_editable/src/shared_pkg/c_module.c` & `scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/c_module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/sdist_config/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/sdist_config/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/sdist_config/pyproject.toml` & `scikit_build_core-0.9.4/tests/packages/sdist_config/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_pyproject_script_with_flags/LICENSE` & `scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.9.4/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.9.4/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/.gitignore` & `scikit_build_core-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/LICENSE` & `scikit_build_core-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.3/README.md` & `scikit_build_core-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,17 @@
 # Turn on verbose output for the editable mode rebuilds.
 editable.verbose = true
 
 # Rebuild the project when the package is imported. The build-directory must be
 # set.
 editable.rebuild = false
 
+# Extra args to pass directly to the builder in the build step.
+build.tool-args = []
+
 # The components to install. If empty, all default components are installed.
 install.components = []
 
 # Whether to strip the binaries. True for scikit-build-core 0.5+.
 install.strip = true
 
 # The path (relative to platlib) for the file to generate.
```

### Comparing `scikit_build_core-0.9.3/pyproject.toml` & `scikit_build_core-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Development Status :: 4 - Beta",
     "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
@@ -47,15 +48,16 @@
 
 [project.optional-dependencies]
 pyproject = [
 ]
 test = [
     "build >=0.8",
     "cattrs >=22.2.0",
-    "pip >=22",
+    "pip >=22; python_version<'3.13'",
+    "pip >=24.1b1; python_version>='3.13'",
     "pybind11 >=2.11",
     "pytest >=7.0",  # 7.2+ recommended for better tracebacks with ExceptionGroup
     "pytest-subprocess >=1.5",
     'setuptools >=43; python_version<"3.9"',
     'setuptools >=45; python_version=="3.9"',
     'setuptools >=49; python_version>="3.10" and python_version<"3.12"',
     'setuptools >=66.1; python_version>="3.12"',
@@ -171,15 +173,14 @@
 
 
 [tool.pylint]
 py-version = "3.7"
 jobs = "0"
 reports.output-format = "colorized"
 good-names = ["f"]
-ignore-patterns = ['.*\.pyi']
 messages_control.disable = [
     "design",
     "fixme",
     "import-outside-toplevel",
     "invalid-name",
     "line-too-long",
     "missing-class-docstring",
```

### Comparing `scikit_build_core-0.9.3/PKG-INFO` & `scikit_build_core-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scikit_build_core
-Version: 0.9.3
+Version: 0.9.4
 Summary: Build backend for CMake based projects
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: exceptiongroup>=1.0; python_version < '3.11'
 Requires-Dist: importlib-metadata>=4.13; python_version < '3.8'
 Requires-Dist: importlib-resources>=1.3; python_version < '3.9'
@@ -48,15 +49,16 @@
 Requires-Dist: sphinx-inline-tabs; extra == 'docs'
 Requires-Dist: sphinx-jsonschema; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: pyproject
 Provides-Extra: test
 Requires-Dist: build>=0.8; extra == 'test'
 Requires-Dist: cattrs>=22.2.0; extra == 'test'
-Requires-Dist: pip>=22; extra == 'test'
+Requires-Dist: pip>=22; (python_version < '3.13') and extra == 'test'
+Requires-Dist: pip>=24.1b1; (python_version >= '3.13') and extra == 'test'
 Requires-Dist: pybind11>=2.11; extra == 'test'
 Requires-Dist: pytest-subprocess>=1.5; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: setuptools>=43; (python_version < '3.9') and extra == 'test'
 Requires-Dist: setuptools>=45; (python_version == '3.9') and extra == 'test'
 Requires-Dist: setuptools>=49; (python_version >= '3.10' and python_version < '3.12') and extra == 'test'
 Requires-Dist: setuptools>=66.1; (python_version >= '3.12') and extra == 'test'
@@ -350,14 +352,17 @@
 # Turn on verbose output for the editable mode rebuilds.
 editable.verbose = true
 
 # Rebuild the project when the package is imported. The build-directory must be
 # set.
 editable.rebuild = false
 
+# Extra args to pass directly to the builder in the build step.
+build.tool-args = []
+
 # The components to install. If empty, all default components are installed.
 install.components = []
 
 # Whether to strip the binaries. True for scikit-build-core 0.5+.
 install.strip = true
 
 # The path (relative to platlib) for the file to generate.
```

