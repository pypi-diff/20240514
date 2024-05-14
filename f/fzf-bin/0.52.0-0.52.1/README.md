# Comparing `tmp/fzf_bin-0.52.0.tar.gz` & `tmp/fzf_bin-0.52.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_bin-0.52.0.tar", last modified: Wed May  8 10:11:22 2024, max compression
+gzip compressed data, was "fzf_bin-0.52.1.tar", last modified: Tue May 14 04:47:43 2024, max compression
```

## Comparing `fzf_bin-0.52.0.tar` & `fzf_bin-0.52.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     1074 2024-05-08 10:10:12.462575 fzf_bin-0.52.0/LICENSE
--rw-r--r--   0        0        0      469 2024-05-08 10:10:12.462575 fzf_bin-0.52.0/README.md
--rw-r--r--   0        0        0       35 2024-05-08 10:10:13.230570 fzf_bin-0.52.0/fzf/.git
--rw-r--r--   0        0        0       17 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/FUNDING.yml
--rw-r--r--   0        0        0     1162 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
--rw-r--r--   0        0        0      209 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/dependabot.yml
--rw-r--r--   0        0        0     1111 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      296 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/depsreview.yaml
--rw-r--r--   0        0        0     1119 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/linux.yml
--rw-r--r--   0        0        0     1001 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/macos.yml
--rw-r--r--   0        0        0      555 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/sponsors.yml
--rw-r--r--   0        0        0      193 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/typos.yml
--rw-r--r--   0        0        0      382 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.github/workflows/winget.yml
--rw-r--r--   0        0        0      104 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.gitignore
--rw-r--r--   0        0        0     2512 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.goreleaser.yml
--rw-r--r--   0        0        0      578 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.rubocop.yml
--rw-r--r--   0        0        0       15 2024-05-08 10:10:13.238570 fzf_bin-0.52.0/fzf/.tool-versions
--rw-r--r--   0        0        0    28068 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/ADVANCED.md
--rw-r--r--   0        0        0     1718 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/BUILD.md
--rw-r--r--   0        0        0    77620 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/CHANGELOG.md
--rw-r--r--   0        0        0      486 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/Dockerfile
--rw-r--r--   0        0        0     1085 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/LICENSE
--rw-r--r--   0        0        0     5228 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/Makefile
--rw-r--r--   0        0        0    17711 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/README-VIM.md
--rw-r--r--   0        0        0    36006 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/README.md
--rwxr-xr-x   0        0        0     2419 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/bin/fzf-preview.sh
--rwxr-xr-x   0        0        0     7069 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/bin/fzf-tmux
--rw-r--r--   0        0        0    21398 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/doc/fzf.txt
--rw-r--r--   0        0        0      496 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/go.mod
--rw-r--r--   0        0        0     5203 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/go.sum
--rwxr-xr-x   0        0        0    10216 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/install
--rw-r--r--   0        0        0     1881 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/install.ps1
--rw-r--r--   0        0        0     1550 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/main.go
--rw-r--r--   0        0        0     1992 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/man/man1/fzf-tmux.1
--rw-r--r--   0        0        0    51810 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/man/man1/fzf.1
--rw-r--r--   0        0        0    32189 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/plugin/fzf.vim
--rw-r--r--   0        0        0    16103 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/shell/completion.bash
--rw-r--r--   0        0        0    12697 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/shell/completion.zsh
--rw-r--r--   0        0        0     5488 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/shell/key-bindings.bash
--rw-r--r--   0        0        0     5965 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/shell/key-bindings.fish
--rw-r--r--   0        0        0     4138 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/shell/key-bindings.zsh
--rw-r--r--   0        0        0     1085 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/LICENSE
--rw-r--r--   0        0        0     5502 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/actiontype_string.go
--rw-r--r--   0        0        0    26644 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/algo/algo.go
--rw-r--r--   0        0        0     8883 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/algo/algo_test.go
--rw-r--r--   0        0        0    21765 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/algo/normalize.go
--rw-r--r--   0        0        0     9963 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/ansi.go
--rw-r--r--   0        0        0    11138 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/ansi_test.go
--rw-r--r--   0        0        0     1733 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/cache.go
--rw-r--r--   0        0        0      859 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/cache_test.go
--rw-r--r--   0        0        0     1806 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/chunklist.go
--rw-r--r--   0        0        0     1862 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/chunklist_test.go
--rw-r--r--   0        0        0     1704 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/constants.go
--rw-r--r--   0        0        0    10620 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/core.go
--rw-r--r--   0        0        0      678 2024-05-08 10:10:13.242570 fzf_bin-0.52.0/fzf/src/functions.go
--rw-r--r--   0        0        0     2071 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/history.go
--rw-r--r--   0        0        0     1507 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/history_test.go
--rw-r--r--   0        0        0      957 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/item.go
--rw-r--r--   0        0        0      484 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/item_test.go
--rw-r--r--   0        0        0     5637 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/matcher.go
--rw-r--r--   0        0        0     3302 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/merger.go
--rw-r--r--   0        0        0     1989 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/merger_test.go
--rw-r--r--   0        0        0    72964 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/options.go
--rw-r--r--   0        0        0      332 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/options_no_pprof.go
--rw-r--r--   0        0        0     1628 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/options_pprof.go
--rw-r--r--   0        0        0     2069 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/options_pprof_test.go
--rw-r--r--   0        0        0    14608 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/options_test.go
--rw-r--r--   0        0        0    10435 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/pattern.go
--rw-r--r--   0        0        0     8097 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/pattern_test.go
--rw-r--r--   0        0        0      122 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/protector/protector.go
--rw-r--r--   0        0        0      217 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/protector/protector_openbsd.go
--rw-r--r--   0        0        0     6257 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/reader.go
--rw-r--r--   0        0        0     1315 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/reader_test.go
--rw-r--r--   0        0        0     5998 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/result.go
--rw-r--r--   0        0        0      338 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/result_others.go
--rw-r--r--   0        0        0     6064 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/result_test.go
--rw-r--r--   0        0        0      364 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/result_x86.go
--rw-r--r--   0        0        0     6230 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/server.go
--rw-r--r--   0        0        0   117432 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/terminal.go
--rw-r--r--   0        0        0    27967 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/terminal_test.go
--rw-r--r--   0        0        0      449 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/terminal_unix.go
--rw-r--r--   0        0        0      219 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/terminal_windows.go
--rw-r--r--   0        0        0     5661 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tokenizer.go
--rw-r--r--   0        0        0     2878 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tokenizer_test.go
--rw-r--r--   0        0        0     1794 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/dummy.go
--rw-r--r--   0        0        0     3494 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/eventtype_string.go
--rw-r--r--   0        0        0    24916 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/light.go
--rw-r--r--   0        0        0     2578 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/light_unix.go
--rw-r--r--   0        0        0     4807 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/light_windows.go
--rw-r--r--   0        0        0    18671 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/tcell.go
--rw-r--r--   0        0        0    17392 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/tcell_test.go
--rw-r--r--   0        0        0      908 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/ttyname_unix.go
--rw-r--r--   0        0        0      164 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/ttyname_windows.go
--rw-r--r--   0        0        0    22629 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/tui.go
--rw-r--r--   0        0        0      399 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/tui/tui_test.go
--rw-r--r--   0        0        0      554 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/atexit.go
--rw-r--r--   0        0        0      452 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/atexit_test.go
--rw-r--r--   0        0        0      748 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/atomicbool.go
--rw-r--r--   0        0        0      301 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/atomicbool_test.go
--rw-r--r--   0        0        0     4308 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/chars.go
--rw-r--r--   0        0        0      981 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/chars_test.go
--rw-r--r--   0        0        0     1976 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/eventbox.go
--rw-r--r--   0        0        0      899 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/eventbox_test.go
--rw-r--r--   0        0        0      185 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/slab.go
--rw-r--r--   0        0        0     3733 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/util.go
--rw-r--r--   0        0        0     4194 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/util_test.go
--rw-r--r--   0        0        0     2229 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/util_unix.go
--rw-r--r--   0        0        0     4725 2024-05-08 10:10:13.246570 fzf_bin-0.52.0/fzf/src/util/util_windows.go
--rw-r--r--   0        0        0     5860 2024-05-08 10:10:13.250570 fzf_bin-0.52.0/fzf/test/fzf.vader
--rwxr-xr-x   0        0        0   128883 2024-05-08 10:10:13.250570 fzf_bin-0.52.0/fzf/test/test_go.rb
--rw-r--r--   0        0        0      216 2024-05-08 10:10:13.250570 fzf_bin-0.52.0/fzf/typos.toml
--rwxr-xr-x   0        0        0     2520 2024-05-08 10:10:13.250570 fzf_bin-0.52.0/fzf/uninstall
--rw-r--r--   0        0        0        0 2024-05-08 10:10:12.462575 fzf_bin-0.52.0/fzf_bin/__init__.py
--rw-r--r--   0        0        0     1392 2024-05-08 10:10:12.462575 fzf_bin-0.52.0/pdm_build.py
--rw-r--r--   0        0        0     1073 2024-05-08 10:11:22.586143 fzf_bin-0.52.0/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.52.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-14 04:46:27.413795 fzf_bin-0.52.1/LICENSE
+-rw-r--r--   0        0        0      469 2024-05-14 04:46:27.413795 fzf_bin-0.52.1/README.md
+-rw-r--r--   0        0        0       35 2024-05-14 04:46:28.249800 fzf_bin-0.52.1/fzf/.git
+-rw-r--r--   0        0        0       17 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1162 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
+-rw-r--r--   0        0        0      209 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/dependabot.yml
+-rw-r--r--   0        0        0     1111 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      296 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/depsreview.yaml
+-rw-r--r--   0        0        0     1119 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     1001 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/macos.yml
+-rw-r--r--   0        0        0      555 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/sponsors.yml
+-rw-r--r--   0        0        0      193 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/typos.yml
+-rw-r--r--   0        0        0      382 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.github/workflows/winget.yml
+-rw-r--r--   0        0        0      104 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.gitignore
+-rw-r--r--   0        0        0     2512 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.goreleaser.yml
+-rw-r--r--   0        0        0      578 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.rubocop.yml
+-rw-r--r--   0        0        0       15 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/.tool-versions
+-rw-r--r--   0        0        0    28068 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/ADVANCED.md
+-rw-r--r--   0        0        0     1718 2024-05-14 04:46:28.261800 fzf_bin-0.52.1/fzf/BUILD.md
+-rw-r--r--   0        0        0    77752 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/CHANGELOG.md
+-rw-r--r--   0        0        0      486 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/Dockerfile
+-rw-r--r--   0        0        0     1085 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/LICENSE
+-rw-r--r--   0        0        0     5228 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/Makefile
+-rw-r--r--   0        0        0    17711 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/README-VIM.md
+-rw-r--r--   0        0        0    36238 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/README.md
+-rwxr-xr-x   0        0        0     2419 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/bin/fzf-preview.sh
+-rwxr-xr-x   0        0        0     7069 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/bin/fzf-tmux
+-rw-r--r--   0        0        0    21398 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/doc/fzf.txt
+-rw-r--r--   0        0        0      496 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/go.mod
+-rw-r--r--   0        0        0     5203 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/go.sum
+-rwxr-xr-x   0        0        0    10216 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/install
+-rw-r--r--   0        0        0     1881 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/install.ps1
+-rw-r--r--   0        0        0     1550 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/main.go
+-rw-r--r--   0        0        0     1992 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0        0        0    51843 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/man/man1/fzf.1
+-rw-r--r--   0        0        0    32255 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/plugin/fzf.vim
+-rw-r--r--   0        0        0    16134 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/shell/completion.bash
+-rw-r--r--   0        0        0    12697 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/shell/completion.zsh
+-rw-r--r--   0        0        0     5488 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/shell/key-bindings.bash
+-rw-r--r--   0        0        0     5965 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/shell/key-bindings.fish
+-rw-r--r--   0        0        0     4138 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/shell/key-bindings.zsh
+-rw-r--r--   0        0        0     1085 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/LICENSE
+-rw-r--r--   0        0        0     5502 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/actiontype_string.go
+-rw-r--r--   0        0        0    26644 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/algo/algo.go
+-rw-r--r--   0        0        0     8883 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/algo/algo_test.go
+-rw-r--r--   0        0        0    21765 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/algo/normalize.go
+-rw-r--r--   0        0        0     9963 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/ansi.go
+-rw-r--r--   0        0        0    11138 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/ansi_test.go
+-rw-r--r--   0        0        0     1733 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/cache.go
+-rw-r--r--   0        0        0      859 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/cache_test.go
+-rw-r--r--   0        0        0     1806 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/chunklist.go
+-rw-r--r--   0        0        0     1862 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/chunklist_test.go
+-rw-r--r--   0        0        0     1704 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/constants.go
+-rw-r--r--   0        0        0    10620 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/core.go
+-rw-r--r--   0        0        0      678 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/functions.go
+-rw-r--r--   0        0        0     2071 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/history.go
+-rw-r--r--   0        0        0     1507 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/history_test.go
+-rw-r--r--   0        0        0      957 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/item.go
+-rw-r--r--   0        0        0      484 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/item_test.go
+-rw-r--r--   0        0        0     5637 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/matcher.go
+-rw-r--r--   0        0        0     3302 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/merger.go
+-rw-r--r--   0        0        0     1989 2024-05-14 04:46:28.265800 fzf_bin-0.52.1/fzf/src/merger_test.go
+-rw-r--r--   0        0        0    73001 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/options.go
+-rw-r--r--   0        0        0      332 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/options_no_pprof.go
+-rw-r--r--   0        0        0     1628 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/options_pprof.go
+-rw-r--r--   0        0        0     2069 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/options_pprof_test.go
+-rw-r--r--   0        0        0    14608 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/options_test.go
+-rw-r--r--   0        0        0    10435 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/pattern.go
+-rw-r--r--   0        0        0     8097 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/pattern_test.go
+-rw-r--r--   0        0        0      122 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/protector/protector.go
+-rw-r--r--   0        0        0      217 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/protector/protector_openbsd.go
+-rw-r--r--   0        0        0     6257 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/reader.go
+-rw-r--r--   0        0        0     1315 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/reader_test.go
+-rw-r--r--   0        0        0     5998 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/result.go
+-rw-r--r--   0        0        0      338 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/result_others.go
+-rw-r--r--   0        0        0     6064 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/result_test.go
+-rw-r--r--   0        0        0      364 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/result_x86.go
+-rw-r--r--   0        0        0     6230 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/server.go
+-rw-r--r--   0        0        0   117432 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/terminal.go
+-rw-r--r--   0        0        0    27967 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/terminal_test.go
+-rw-r--r--   0        0        0      449 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/terminal_unix.go
+-rw-r--r--   0        0        0      219 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/terminal_windows.go
+-rw-r--r--   0        0        0     5661 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tokenizer.go
+-rw-r--r--   0        0        0     2878 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tokenizer_test.go
+-rw-r--r--   0        0        0     1794 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/dummy.go
+-rw-r--r--   0        0        0     3494 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/eventtype_string.go
+-rw-r--r--   0        0        0    24916 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/light.go
+-rw-r--r--   0        0        0     2578 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/light_unix.go
+-rw-r--r--   0        0        0     4807 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/light_windows.go
+-rw-r--r--   0        0        0    18671 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/tcell.go
+-rw-r--r--   0        0        0    17392 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/tcell_test.go
+-rw-r--r--   0        0        0      908 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/ttyname_unix.go
+-rw-r--r--   0        0        0      164 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/ttyname_windows.go
+-rw-r--r--   0        0        0    22629 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/tui.go
+-rw-r--r--   0        0        0      399 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/tui/tui_test.go
+-rw-r--r--   0        0        0      554 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/atexit.go
+-rw-r--r--   0        0        0      452 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/atexit_test.go
+-rw-r--r--   0        0        0      748 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/atomicbool.go
+-rw-r--r--   0        0        0      301 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/atomicbool_test.go
+-rw-r--r--   0        0        0     4308 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/chars.go
+-rw-r--r--   0        0        0      981 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/chars_test.go
+-rw-r--r--   0        0        0     1976 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/eventbox.go
+-rw-r--r--   0        0        0      899 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/eventbox_test.go
+-rw-r--r--   0        0        0      185 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/slab.go
+-rw-r--r--   0        0        0     3733 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/util.go
+-rw-r--r--   0        0        0     4194 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/util_test.go
+-rw-r--r--   0        0        0     2229 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/util_unix.go
+-rw-r--r--   0        0        0     4876 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/src/util/util_windows.go
+-rw-r--r--   0        0        0     5860 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/test/fzf.vader
+-rwxr-xr-x   0        0        0   128883 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/test/test_go.rb
+-rw-r--r--   0        0        0      216 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/typos.toml
+-rwxr-xr-x   0        0        0     2520 2024-05-14 04:46:28.269800 fzf_bin-0.52.1/fzf/uninstall
+-rw-r--r--   0        0        0        0 2024-05-14 04:46:27.413795 fzf_bin-0.52.1/fzf_bin/__init__.py
+-rw-r--r--   0        0        0     1392 2024-05-14 04:46:27.413795 fzf_bin-0.52.1/pdm_build.py
+-rw-r--r--   0        0        0     1073 2024-05-14 04:47:43.230242 fzf_bin-0.52.1/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.52.1/PKG-INFO
```

### Comparing `fzf_bin-0.52.0/LICENSE` & `fzf_bin-0.52.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml` & `fzf_bin-0.52.1/fzf/.github/ISSUE_TEMPLATE/issue_template.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.github/workflows/codeql-analysis.yml` & `fzf_bin-0.52.1/fzf/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.github/workflows/linux.yml` & `fzf_bin-0.52.1/fzf/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.github/workflows/macos.yml` & `fzf_bin-0.52.1/fzf/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.github/workflows/sponsors.yml` & `fzf_bin-0.52.1/fzf/.github/workflows/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.goreleaser.yml` & `fzf_bin-0.52.1/fzf/.goreleaser.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/.rubocop.yml` & `fzf_bin-0.52.1/fzf/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/ADVANCED.md` & `fzf_bin-0.52.1/fzf/ADVANCED.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/BUILD.md` & `fzf_bin-0.52.1/fzf/BUILD.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/CHANGELOG.md` & `fzf_bin-0.52.1/fzf/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGELOG
 =========
 
+0.52.1
+------
+- Fixed a critical bug in the Windows version
+    - Windows users are strongly encouraged to upgrade to this version
+
 0.52.0
 ------
 - Added `--highlight-line` to highlight the whole current line (à la `set cursorline` of Vim)
 - Added color names for selected lines: `selected-fg`, `selected-bg`, and `selected-hl`
   ```sh
   fzf --border --multi --info inline-right --layout reverse --marker ▏ --pointer ▌ --prompt '▌ '  \
       --highlight-line --color gutter:-1,selected-bg:238,selected-fg:146,current-fg:189
```

### Comparing `fzf_bin-0.52.0/fzf/LICENSE` & `fzf_bin-0.52.1/fzf/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/Makefile` & `fzf_bin-0.52.1/fzf/Makefile`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/README-VIM.md` & `fzf_bin-0.52.1/fzf/README-VIM.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/README.md` & `fzf_bin-0.52.1/fzf/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Sponsors ❤️
 -----------
 
 I would like to thank all the sponsors of this project who make it possible for me to continue to improve fzf.
 
 If you'd like to sponsor this project, please visit https://github.com/sponsors/junegunn.
 
-<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/warpdotdev"><img src="https://github.com/warpdotdev.png" width="60px" alt="Warp" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><a href="https://github.com/jamesob"><img src="https://github.com/jamesob.png" width="60px" alt="James O'Beirne" /></a><a href="https://github.com/joshuatz"><img src="https://github.com/joshuatz.png" width="60px" alt="Joshua Tzucker" /></a><a href="https://github.com/gpopides"><img src="https://github.com/gpopides.png" width="60px" alt="gpopides" /></a><a href="https://github.com/jlebray"><img src="https://github.com/jlebray.png" width="60px" alt="Johan Le Bray" /></a><!-- sponsors -->
+<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/warpdotdev"><img src="https://github.com/warpdotdev.png" width="60px" alt="Warp" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><a href="https://github.com/jamesob"><img src="https://github.com/jamesob.png" width="60px" alt="James O'Beirne" /></a><a href="https://github.com/gpopides"><img src="https://github.com/gpopides.png" width="60px" alt="gpopides" /></a><a href="https://github.com/jlebray"><img src="https://github.com/jlebray.png" width="60px" alt="Johan Le Bray" /></a><a href="https://github.com/cskeeters"><img src="https://github.com/cskeeters.png" width="60px" alt="Chad Skeeters" /></a><a href="https://github.com/Konfekt"><img src="https://github.com/Konfekt.png" width="60px" alt="Enno" /></a><a href="https://github.com/joclement"><img src="https://github.com/joclement.png" width="60px" alt="Joris Clement" /></a><!-- sponsors -->
 
 Table of Contents
 -----------------
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
```

#### html2text {}

```diff
@@ -22,191 +22,191 @@
 _[_M_o_r_i_t_z_ _D_i_e_t_z_]_[_M_i_k_k_e_l_ _M_a_l_m_b_e_r_g_]_[_P_i_e_r_r_e_ _D_u_b_o_u_i_l_h_]_[_R_y_a_n_ _R_o_d_e_n_-_C_o_r_r_e_n_t_]_[_J_o_r_d_a_n
 _A_r_e_n_t_s_e_n_]_[_M_i_s_l_a_v_ _M_a_r_o_h_n_i_Ä__]_[_A_l_e_x_ _V_i_s_c_r_e_a_n_u_]_[_D_a_v_i_d_ _B_a_l_a_t_e_r_o_]_[_O_n_d_r_e_j_ _S_y_n_a_c_e_k_]
 _[_M_a_t_h_i_a_s_ _J_e_a_n_ _J_o_h_a_n_s_e_n_]_[_B_e_n_ _E_l_a_n_]_[_P_a_w_e_Å__ _D_u_d_a_]_[_S_a_n_t_i_a_g_o_ _L_e_z_i_c_a_]_[_T_i_m_o_ _S_u_l_g_]
 _[_D_a_m_i_e_n_ _R_a_j_o_n_]_[_A_r_t_B_I_T_]_[_H_o_v_i_s_]_[_D_a_r_i_u_s_ _J_o_n_d_a_]_[_C_r_i_s_t_i_a_n_ _D_o_m_i_n_g_u_e_z_]_[_C_h_a_n_g_-_H_u_n_g
 _L_i_a_n_g_]_[_B_e_n_ _L_e_c_h_l_i_t_n_e_r_]_[_y_a_s_h_]_[_g_e_o_r_g_e_ _l_o_o_s_h_c_h_]_[_T_a_k_u_m_i_ _K_A_G_I_Y_A_M_A_]_[_P_a_u_l_ _O_'_L_e_a_r_y
 _M_c_C_a_n_n_]_[_R_o_b_e_r_t_ _B_e_e_g_e_r_]_[_V_E_E_B_ _P_r_o_j_e_c_t_s_]_[_K_h_u_e_ _D_o_a_n_]_[_Y_o_w_a_y_ _B_u_o_r_n_]_[_J_o_s_h_ _S_c_a_l_i_s_i_]
 _[_A_l_e_c_ _S_c_o_t_t_]_[_t_h_a_n_k_s_._d_e_v_]_[_A_r_t_u_r_ _S_a_p_e_k_]_[_G_u_i_l_l_a_u_m_e_ _G_e_l_i_n_]_[_M_a_r_c_i_n_ _S_._]_[_R_o_b_ _L_e_v_y_]
-_[_W_a_r_p_]_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_M_a_r_k_u_s_ _K_o_l_l_e_r_]_[_J_a_m_e_s_ _O_'_B_e_i_r_n_e_]_[_J_o_s_h_u_a
-_T_z_u_c_k_e_r_]_[_g_p_o_p_i_d_e_s_]_[_J_o_h_a_n_ _L_e_ _B_r_a_y_]Table of Contents ----------------- *
-[Installation](#installation) * [Using Homebrew](#using-homebrew) * [Using git]
-(#using-git) * [Using Linux package managers](#using-linux-package-managers) *
-[Windows](#windows) * [Setting up shell integration](#setting-up-shell-
-integration) * [As Vim plugin](#as-vim-plugin) * [Upgrading fzf](#upgrading-
-fzf) * [Building fzf](#building-fzf) * [Usage](#usage) * [Using the finder]
-(#using-the-finder) * [Layout](#layout) * [Search syntax](#search-syntax) *
-[Environment variables](#environment-variables) * [Options](#options) * [Demo]
-(#demo) * [Examples](#examples) * [`fzf-tmux` script](#fzf-tmux-script) * [Key
-bindings for command-line](#key-bindings-for-command-line) * [Fuzzy completion
-for bash and zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and directories]
-(#files-and-directories) * [Process IDs](#process-ids) * [Host names](#host-
-names) * [Environment variables / Aliases](#environment-variables--aliases) *
-[Settings](#settings) * [Supported commands](#supported-commands) * [Custom
-fuzzy completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin) *
-[Advanced topics](#advanced-topics) * [Performance](#performance) * [Executing
-external programs](#executing-external-programs) * [Turning into a different
-process](#turning-into-a-different-process) * [Reloading the candidate list]
-(#reloading-the-candidate-list) * [1. Update the list of processes by pressing
-CTRL-R](#1-update-the-list-of-processes-by-pressing-ctrl-r) * [2. Switch
-between sources by pressing CTRL-D or CTRL-F](#2-switch-between-sources-by-
-pressing-ctrl-d-or-ctrl-f) * [3. Interactive ripgrep integration](#3-
-interactive-ripgrep-integration) * [Preview window](#preview-window) *
-[Previewing an image](#previewing-an-image) * [Tips](#tips) * [Respecting
-`.gitignore`](#respecting-gitignore) * [Fish shell](#fish-shell) * [fzf Theme
-Playground](#fzf-theme-playground) * [Related projects](#related-projects) *
-[License](#license) Installation ------------ fzf project consists of the
-following components: - `fzf` executable - `fzf-tmux` script for launching fzf
-in a tmux pane - Shell integration - Key bindings (`CTRL-T`, `CTRL-R`, and
-`ALT-C`) (bash, zsh, fish) - Fuzzy completion (bash, zsh) - Vim/Neovim plugin
-You can [download fzf executable][bin] alone if you don't need the extra stuff.
-[bin]: https://github.com/junegunn/fzf/releases ### Using Homebrew You can use
-[Homebrew](https://brew.sh/) (on macOS or Linux) to install fzf. ```sh brew
-install fzf # To build fzf from the latest source: brew install --HEAD fzf ```
-> [!IMPORTANT] > To set up shell integration (key bindings and fuzzy
-completion), > see [the instructions below](#setting-up-shell-integration). fzf
-is also available [via MacPorts][portfile]: `sudo port install fzf` [portfile]:
-https://github.com/macports/macports-ports/blob/master/sysutils/fzf/Portfile
-### Using git Alternatively, you can "git clone" this repository to any
-directory and run [install](https://github.com/junegunn/fzf/blob/master/
-install) script. ```sh git clone --depth 1 https://github.com/junegunn/fzf.git
-~/.fzf ~/.fzf/install ``` The install script will add lines to your shell
-configuration file to modify `$PATH` and set up shell integration. ### Using
-Linux package managers | Package Manager | Linux Distribution | Command | | ---
------------- | ----------------------- | ---------------------------------- | |
-APK | Alpine Linux | `sudo apk add fzf` | | APT | Debian 9+/Ubuntu 19.10+ |
-`sudo apt install fzf` | | Conda | | `conda install -c conda-forge fzf` | | DNF
-| Fedora | `sudo dnf install fzf` | | Nix | NixOS, etc. | `nix-env -iA
-nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman -S fzf` | | pkg | FreeBSD |
-`pkg install fzf` | | pkgin | NetBSD | `pkgin install fzf` | | pkg_add |
-OpenBSD | `pkg_add fzf` | | Portage | Gentoo | `emerge --ask app-shells/fzf` |
-| Spack | | `spack install fzf` | | XBPS | Void Linux | `sudo xbps-install -
-S fzf` | | Zypper | openSUSE | `sudo zypper install fzf` | > [!IMPORTANT] > To
-set up shell integration (key bindings and fuzzy completion), > see [the
-instructions below](#setting-up-shell-integration). [![Packaging status](https:
-//repology.org/badge/vertical-allrepos/fzf.svg)](https://repology.org/project/
-fzf/versions) ### Windows Pre-built binaries for Windows can be downloaded
-[here][bin]. fzf is also available via [Chocolatey][choco], [Scoop][scoop],
-[Winget][winget], and [MSYS2][msys2]: | Package manager | Command | | ---------
------- | ------------------------------------- | | Chocolatey | `choco install
-fzf` | | Scoop | `scoop install fzf` | | Winget | `winget install fzf` | |
-MSYS2 (pacman) | `pacman -S $MINGW_PACKAGE_PREFIX-fzf` | [choco]: https://
-chocolatey.org/packages/fzf [scoop]: https://github.com/ScoopInstaller/Main/
-blob/master/bucket/fzf.json [winget]: https://github.com/microsoft/winget-pkgs/
-tree/master/manifests/j/junegunn/fzf [msys2]: https://packages.msys2.org/base/
-mingw-w64-fzf Known issues and limitations on Windows can be found on [the wiki
-page][windows-wiki]. [windows-wiki]: https://github.com/junegunn/fzf/wiki/
-Windows ### Setting up shell integration Add the following line to your shell
-configuration file. * bash ```sh # Set up fzf key bindings and fuzzy completion
-eval "$(fzf --bash)" ``` * zsh ```sh # Set up fzf key bindings and fuzzy
-completion eval "$(fzf --zsh)" ``` * fish ```fish # Set up fzf key bindings fzf
---fish | source ``` > [!NOTE] > `--bash`, `--zsh`, and `--fish` options are
-only available in fzf 0.48.0 or > later. If you have an older version of fzf,
-or want finer control, you can > source individual script files in the [/shell]
-(/shell) directory. The > location of the files may vary depending on the
-package manager you use. > Please refer to the package documentation for more
-information. > (e.g. `apt show fzf`) > [!TIP] > You can disable CTRL-T or ALT-
-C binding by setting `FZF_CTRL_T_COMMAND` or > `FZF_ALT_C_COMMAND` to an empty
-string when sourcing the script. > For example, to disable ALT-C binding: > > *
-bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"` > * zsh: `FZF_ALT_C_COMMAND=
-eval "$(fzf --zsh)"` > * fish: `fzf --fish | FZF_ALT_C_COMMAND= source` > >
-Setting the variables after sourcing the script will have no effect. ### As Vim
-plugin If you use [vim-plug](https://github.com/junegunn/vim-plug), add this
-line to your Vim configuration file: ```vim Plug 'junegunn/fzf', { 'do': { -
-> fzf#install() } } ``` `fzf#install()` makes sure that you have the latest
-binary, but it's optional, so you can omit it if you use a plugin manager that
-doesn't support hooks. For more installation options, see [README-VIM.md]
-(README-VIM.md). Upgrading fzf ------------- fzf is being actively developed,
-and you might want to upgrade it once in a while. Please follow the instruction
-below depending on the installation method used. - git: `cd ~/.fzf && git pull
-&& ./install` - brew: `brew update; brew upgrade fzf` - macports: `sudo port
-upgrade fzf` - chocolatey: `choco upgrade fzf` - vim-plug: `:PlugUpdate fzf`
-Building fzf ------------ See [BUILD.md](BUILD.md). Usage ----- fzf will launch
-interactive finder, read the list from STDIN, and write the selected item to
-STDOUT. ```sh find * -type f | fzf > selected ``` Without STDIN pipe, fzf will
-traverse the file system under the current directory to get the list of files.
-```sh vim $(fzf) ``` > [!NOTE] > You can override the default behavior > *
-Either by setting `$FZF_DEFAULT_COMMAND` to a command that generates the
-desired list > * Or by setting `--walker`, `--walker-root`, and `--walker-skip`
-options in `$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be
-to use `xargs` but we've presented > the above as it's easier to grasp > ```sh
-> fzf --print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to
-turn itself into a different process. > > ```sh > fzf --bind 'enter:become(vim
-{})' > ``` > > *See [Turning into a different process](#turning-into-a-
-different-process) > for more information.* ### Using the finder - `CTRL-K` /
-`CTRL-J` (or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to
-select the item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-
-m`), `TAB` and `Shift-TAB` to mark multiple items - Emacs style key bindings -
-Mouse: scroll, click, double-click; shift-click and shift-scroll on multi-
-select mode ### Layout fzf by default starts in fullscreen mode, but you can
-make it start below the cursor with `--height` option. ```sh vim $(fzf --height
-40%) ``` Also, check out `--reverse` and `--layout` options if you prefer "top-
-down" layout instead of the default "bottom-up" layout. ```sh vim $(fzf --
-height 40% --reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so
-that they're applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--
-height 40% --layout=reverse --border' ``` ### Search syntax Unless otherwise
-specified, fzf starts in "extended-search mode" where you can type in multiple
-search terms delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token |
-Match type | Description | | --------- | -------------------------- | ---------
---------------------------- | | `sbtrkt` | fuzzy-match | Items that match
-`sbtrkt` | | `'wild` | exact-match (quoted) | Items that include `wild` | |
-`^music` | prefix-exact-match | Items that start with `music` | | `.mp3$` |
-suffix-exact-match | Items that end with `.mp3` | | `!fire` | inverse-exact-
-match | Items that do not include `fire` | | `!^music` | inverse-prefix-exact-
-match | Items that do not start with `music` | | `!.mp3$` | inverse-suffix-
-exact-match | Items that do not end with `.mp3` | If you don't prefer fuzzy
-matching and do not wish to "quote" every word, start fzf with `-e` or `--
-exact` option. Note that when `--exact` is set, `'`-prefix "unquotes" the term.
-A single bar character term acts as an OR operator. For example, the following
-query matches entries that start with `core` and end with either `go`, `rb`, or
-`py`. ``` ^core go$ | rb$ | py$ ``` ### Environment variables -
-`FZF_DEFAULT_COMMAND` - Default command to use when input is tty - e.g. `export
-FZF_DEFAULT_COMMAND='fd --type f'` - `FZF_DEFAULT_OPTS` - Default options -
-e.g. `export FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` -
-`FZF_DEFAULT_OPTS_FILE` - If you prefer to manage default options in a file,
-set this variable to point to the location of the file - e.g. `export
-FZF_DEFAULT_OPTS_FILE=~/.fzfrc` > [!WARNING] > `FZF_DEFAULT_COMMAND` is not
-used by shell integration due to the > slight difference in requirements. > > *
-`CTRL-T` runs `$FZF_CTRL_T_COMMAND` to get a list of files and directories > *
-`ALT-C` runs `$FZF_ALT_C_COMMAND` to get a list of directories > * `vim ~/**`
-runs `fzf_compgen_path()` with the prefix (`~/`) as the first argument > * `cd
-foo**` runs `fzf_compgen_dir()` with the prefix (`foo`) as the first argument >
-> The available options are described later in this document. ### Options See
-the man page (`man fzf`) for the full list of options. ### Demo If you learn by
-watching videos, check out this screencast by [@samoshkin](https://github.com/
-samoshkin) to explore `fzf` features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples
--------- * [Wiki page of examples](https://github.com/junegunn/fzf/wiki/
-examples) * *Disclaimer: The examples on this page are maintained by the
-community and are not thoroughly tested* * [Advanced fzf examples](https://
-github.com/junegunn/fzf/blob/master/ADVANCED.md) `fzf-tmux` script ------------
------ [fzf-tmux](bin/fzf-tmux) is a bash script that opens fzf in a tmux pane.
-```sh # usage: fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS] # See available
-options fzf-tmux --help # select git branches in horizontal split below (15
-lines) git branch | fzf-tmux -d 15 # select multiple words in vertical split on
-the left (20% of screen width) cat /usr/share/dict/words | fzf-tmux -l 20% --
-multi --reverse ``` It will still work even when you're not on tmux, silently
-ignoring `-[pudlr]` options, so you can invariably use `fzf-tmux` in your
-scripts. Alternatively, you can use `--height HEIGHT[%]` option not to start
-fzf in fullscreen mode. ```sh fzf --height 40% ``` Key bindings for command-
-line ----------------------------- The install script will setup the following
-key bindings for bash, zsh, and fish. - `CTRL-T` - Paste the selected files and
-directories onto the command-line - The list is generated using `--walker
-file,dir,follow,hidden` option - You can override the behavior by setting
-`FZF_CTRL_T_COMMAND` to a custom command that generates the desired list - Or
-you can set `--walker*` options in `FZF_CTRL_T_OPTS` - Set `FZF_CTRL_T_OPTS` to
-pass additional options to fzf ```sh # Preview file content using bat (https://
-github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --walker-skip
-.git,node_modules,target --preview 'bat -n --color=always {}' --bind 'ctrl-/:
-change-preview-window(down|hidden|)'" ``` - Can be disabled by setting
-`FZF_CTRL_T_COMMAND` to an empty string when sourcing the script - `CTRL-R` -
-Paste the selected command from history onto the command-line - If you want to
-see the commands in chronological order, press `CTRL-R` again which toggles
-sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options to fzf
-```sh # CTRL-/ to toggle small preview window to see the full command # CTRL-
-Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS=" --
-preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
+_[_W_a_r_p_]_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_M_a_r_k_u_s_ _K_o_l_l_e_r_]_[_J_a_m_e_s_ _O_'_B_e_i_r_n_e_]_[_g_p_o_p_i_d_e_s_]
+_[_J_o_h_a_n_ _L_e_ _B_r_a_y_]_[_C_h_a_d_ _S_k_e_e_t_e_r_s_]_[_E_n_n_o_]_[_J_o_r_i_s_ _C_l_e_m_e_n_t_]Table of Contents ----------
+------- * [Installation](#installation) * [Using Homebrew](#using-homebrew) *
+[Using git](#using-git) * [Using Linux package managers](#using-linux-package-
+managers) * [Windows](#windows) * [Setting up shell integration](#setting-up-
+shell-integration) * [As Vim plugin](#as-vim-plugin) * [Upgrading fzf]
+(#upgrading-fzf) * [Building fzf](#building-fzf) * [Usage](#usage) * [Using the
+finder](#using-the-finder) * [Layout](#layout) * [Search syntax](#search-
+syntax) * [Environment variables](#environment-variables) * [Options](#options)
+* [Demo](#demo) * [Examples](#examples) * [`fzf-tmux` script](#fzf-tmux-script)
+* [Key bindings for command-line](#key-bindings-for-command-line) * [Fuzzy
+completion for bash and zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and
+directories](#files-and-directories) * [Process IDs](#process-ids) * [Host
+names](#host-names) * [Environment variables / Aliases](#environment-variables-
+-aliases) * [Settings](#settings) * [Supported commands](#supported-commands) *
+[Custom fuzzy completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin)
+* [Advanced topics](#advanced-topics) * [Performance](#performance) *
+[Executing external programs](#executing-external-programs) * [Turning into a
+different process](#turning-into-a-different-process) * [Reloading the
+candidate list](#reloading-the-candidate-list) * [1. Update the list of
+processes by pressing CTRL-R](#1-update-the-list-of-processes-by-pressing-ctrl-
+r) * [2. Switch between sources by pressing CTRL-D or CTRL-F](#2-switch-
+between-sources-by-pressing-ctrl-d-or-ctrl-f) * [3. Interactive ripgrep
+integration](#3-interactive-ripgrep-integration) * [Preview window](#preview-
+window) * [Previewing an image](#previewing-an-image) * [Tips](#tips) *
+[Respecting `.gitignore`](#respecting-gitignore) * [Fish shell](#fish-shell) *
+[fzf Theme Playground](#fzf-theme-playground) * [Related projects](#related-
+projects) * [License](#license) Installation ------------ fzf project consists
+of the following components: - `fzf` executable - `fzf-tmux` script for
+launching fzf in a tmux pane - Shell integration - Key bindings (`CTRL-T`,
+`CTRL-R`, and `ALT-C`) (bash, zsh, fish) - Fuzzy completion (bash, zsh) - Vim/
+Neovim plugin You can [download fzf executable][bin] alone if you don't need
+the extra stuff. [bin]: https://github.com/junegunn/fzf/releases ### Using
+Homebrew You can use [Homebrew](https://brew.sh/) (on macOS or Linux) to
+install fzf. ```sh brew install fzf # To build fzf from the latest source: brew
+install --HEAD fzf ``` > [!IMPORTANT] > To set up shell integration (key
+bindings and fuzzy completion), > see [the instructions below](#setting-up-
+shell-integration). fzf is also available [via MacPorts][portfile]: `sudo port
+install fzf` [portfile]: https://github.com/macports/macports-ports/blob/
+master/sysutils/fzf/Portfile ### Using git Alternatively, you can "git clone"
+this repository to any directory and run [install](https://github.com/junegunn/
+fzf/blob/master/install) script. ```sh git clone --depth 1 https://github.com/
+junegunn/fzf.git ~/.fzf ~/.fzf/install ``` The install script will add lines to
+your shell configuration file to modify `$PATH` and set up shell integration.
+### Using Linux package managers | Package Manager | Linux Distribution |
+Command | | --------------- | ----------------------- | -----------------------
+----------- | | APK | Alpine Linux | `sudo apk add fzf` | | APT | Debian 9+/
+Ubuntu 19.10+ | `sudo apt install fzf` | | Conda | | `conda install -c conda-
+forge fzf` | | DNF | Fedora | `sudo dnf install fzf` | | Nix | NixOS, etc. |
+`nix-env -iA nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman -S fzf` | |
+pkg | FreeBSD | `pkg install fzf` | | pkgin | NetBSD | `pkgin install fzf` | |
+pkg_add | OpenBSD | `pkg_add fzf` | | Portage | Gentoo | `emerge --ask app-
+shells/fzf` | | Spack | | `spack install fzf` | | XBPS | Void Linux | `sudo
+xbps-install -S fzf` | | Zypper | openSUSE | `sudo zypper install fzf` | >
+[!IMPORTANT] > To set up shell integration (key bindings and fuzzy completion),
+> see [the instructions below](#setting-up-shell-integration). [![Packaging
+status](https://repology.org/badge/vertical-allrepos/fzf.svg)](https://
+repology.org/project/fzf/versions) ### Windows Pre-built binaries for Windows
+can be downloaded [here][bin]. fzf is also available via [Chocolatey][choco],
+[Scoop][scoop], [Winget][winget], and [MSYS2][msys2]: | Package manager |
+Command | | --------------- | ------------------------------------- | |
+Chocolatey | `choco install fzf` | | Scoop | `scoop install fzf` | | Winget |
+`winget install fzf` | | MSYS2 (pacman) | `pacman -S $MINGW_PACKAGE_PREFIX-fzf`
+| [choco]: https://chocolatey.org/packages/fzf [scoop]: https://github.com/
+ScoopInstaller/Main/blob/master/bucket/fzf.json [winget]: https://github.com/
+microsoft/winget-pkgs/tree/master/manifests/j/junegunn/fzf [msys2]: https://
+packages.msys2.org/base/mingw-w64-fzf Known issues and limitations on Windows
+can be found on [the wiki page][windows-wiki]. [windows-wiki]: https://
+github.com/junegunn/fzf/wiki/Windows ### Setting up shell integration Add the
+following line to your shell configuration file. * bash ```sh # Set up fzf key
+bindings and fuzzy completion eval "$(fzf --bash)" ``` * zsh ```sh # Set up fzf
+key bindings and fuzzy completion eval "$(fzf --zsh)" ``` * fish ```fish # Set
+up fzf key bindings fzf --fish | source ``` > [!NOTE] > `--bash`, `--zsh`, and
+`--fish` options are only available in fzf 0.48.0 or > later. If you have an
+older version of fzf, or want finer control, you can > source individual script
+files in the [/shell](/shell) directory. The > location of the files may vary
+depending on the package manager you use. > Please refer to the package
+documentation for more information. > (e.g. `apt show fzf`) > [!TIP] > You can
+disable CTRL-T or ALT-C binding by setting `FZF_CTRL_T_COMMAND` or >
+`FZF_ALT_C_COMMAND` to an empty string when sourcing the script. > For example,
+to disable ALT-C binding: > > * bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"`
+> * zsh: `FZF_ALT_C_COMMAND= eval "$(fzf --zsh)"` > * fish: `fzf --fish |
+FZF_ALT_C_COMMAND= source` > > Setting the variables after sourcing the script
+will have no effect. ### As Vim plugin If you use [vim-plug](https://
+github.com/junegunn/vim-plug), add this line to your Vim configuration file:
+```vim Plug 'junegunn/fzf', { 'do': { -> fzf#install() } } ``` `fzf#install()`
+makes sure that you have the latest binary, but it's optional, so you can omit
+it if you use a plugin manager that doesn't support hooks. For more
+installation options, see [README-VIM.md](README-VIM.md). Upgrading fzf -------
+------ fzf is being actively developed, and you might want to upgrade it once
+in a while. Please follow the instruction below depending on the installation
+method used. - git: `cd ~/.fzf && git pull && ./install` - brew: `brew update;
+brew upgrade fzf` - macports: `sudo port upgrade fzf` - chocolatey: `choco
+upgrade fzf` - vim-plug: `:PlugUpdate fzf` Building fzf ------------ See
+[BUILD.md](BUILD.md). Usage ----- fzf will launch interactive finder, read the
+list from STDIN, and write the selected item to STDOUT. ```sh find * -type f |
+fzf > selected ``` Without STDIN pipe, fzf will traverse the file system under
+the current directory to get the list of files. ```sh vim $(fzf) ``` > [!NOTE]
+> You can override the default behavior > * Either by setting
+`$FZF_DEFAULT_COMMAND` to a command that generates the desired list > * Or by
+setting `--walker`, `--walker-root`, and `--walker-skip` options in
+`$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be to use
+`xargs` but we've presented > the above as it's easier to grasp > ```sh > fzf -
+-print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to turn
+itself into a different process. > > ```sh > fzf --bind 'enter:become(vim {})'
+> ``` > > *See [Turning into a different process](#turning-into-a-different-
+process) > for more information.* ### Using the finder - `CTRL-K` / `CTRL-J`
+(or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to select the
+item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-m`), `TAB`
+and `Shift-TAB` to mark multiple items - Emacs style key bindings - Mouse:
+scroll, click, double-click; shift-click and shift-scroll on multi-select mode
+### Layout fzf by default starts in fullscreen mode, but you can make it start
+below the cursor with `--height` option. ```sh vim $(fzf --height 40%) ```
+Also, check out `--reverse` and `--layout` options if you prefer "top-down"
+layout instead of the default "bottom-up" layout. ```sh vim $(fzf --height 40%
+--reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so that they're
+applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--height 40% --
+layout=reverse --border' ``` ### Search syntax Unless otherwise specified, fzf
+starts in "extended-search mode" where you can type in multiple search terms
+delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token | Match type |
+Description | | --------- | -------------------------- | ----------------------
+-------------- | | `sbtrkt` | fuzzy-match | Items that match `sbtrkt` | |
+`'wild` | exact-match (quoted) | Items that include `wild` | | `^music` |
+prefix-exact-match | Items that start with `music` | | `.mp3$` | suffix-exact-
+match | Items that end with `.mp3` | | `!fire` | inverse-exact-match | Items
+that do not include `fire` | | `!^music` | inverse-prefix-exact-match | Items
+that do not start with `music` | | `!.mp3$` | inverse-suffix-exact-match |
+Items that do not end with `.mp3` | If you don't prefer fuzzy matching and do
+not wish to "quote" every word, start fzf with `-e` or `--exact` option. Note
+that when `--exact` is set, `'`-prefix "unquotes" the term. A single bar
+character term acts as an OR operator. For example, the following query matches
+entries that start with `core` and end with either `go`, `rb`, or `py`. ```
+^core go$ | rb$ | py$ ``` ### Environment variables - `FZF_DEFAULT_COMMAND` -
+Default command to use when input is tty - e.g. `export FZF_DEFAULT_COMMAND='fd
+--type f'` - `FZF_DEFAULT_OPTS` - Default options - e.g. `export
+FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` - `FZF_DEFAULT_OPTS_FILE` -
+If you prefer to manage default options in a file, set this variable to point
+to the location of the file - e.g. `export FZF_DEFAULT_OPTS_FILE=~/.fzfrc` >
+[!WARNING] > `FZF_DEFAULT_COMMAND` is not used by shell integration due to the
+> slight difference in requirements. > > * `CTRL-T` runs `$FZF_CTRL_T_COMMAND`
+to get a list of files and directories > * `ALT-C` runs `$FZF_ALT_C_COMMAND` to
+get a list of directories > * `vim ~/**` runs `fzf_compgen_path()` with the
+prefix (`~/`) as the first argument > * `cd foo**` runs `fzf_compgen_dir()`
+with the prefix (`foo`) as the first argument > > The available options are
+described later in this document. ### Options See the man page (`man fzf`) for
+the full list of options. ### Demo If you learn by watching videos, check out
+this screencast by [@samoshkin](https://github.com/samoshkin) to explore `fzf`
+features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples -------- * [Wiki page of
+examples](https://github.com/junegunn/fzf/wiki/examples) * *Disclaimer: The
+examples on this page are maintained by the community and are not thoroughly
+tested* * [Advanced fzf examples](https://github.com/junegunn/fzf/blob/master/
+ADVANCED.md) `fzf-tmux` script ----------------- [fzf-tmux](bin/fzf-tmux) is a
+bash script that opens fzf in a tmux pane. ```sh # usage: fzf-tmux [LAYOUT
+OPTIONS] [--] [FZF OPTIONS] # See available options fzf-tmux --help # select
+git branches in horizontal split below (15 lines) git branch | fzf-tmux -d 15 #
+select multiple words in vertical split on the left (20% of screen width) cat /
+usr/share/dict/words | fzf-tmux -l 20% --multi --reverse ``` It will still work
+even when you're not on tmux, silently ignoring `-[pudlr]` options, so you can
+invariably use `fzf-tmux` in your scripts. Alternatively, you can use `--height
+HEIGHT[%]` option not to start fzf in fullscreen mode. ```sh fzf --height 40%
+``` Key bindings for command-line ----------------------------- The install
+script will setup the following key bindings for bash, zsh, and fish. - `CTRL-
+T` - Paste the selected files and directories onto the command-line - The list
+is generated using `--walker file,dir,follow,hidden` option - You can override
+the behavior by setting `FZF_CTRL_T_COMMAND` to a custom command that generates
+the desired list - Or you can set `--walker*` options in `FZF_CTRL_T_OPTS` -
+Set `FZF_CTRL_T_OPTS` to pass additional options to fzf ```sh # Preview file
+content using bat (https://github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --
+walker-skip .git,node_modules,target --preview 'bat -n --color=always {}' --
+bind 'ctrl-/:change-preview-window(down|hidden|)'" ``` - Can be disabled by
+setting `FZF_CTRL_T_COMMAND` to an empty string when sourcing the script -
+`CTRL-R` - Paste the selected command from history onto the command-line - If
+you want to see the commands in chronological order, press `CTRL-R` again which
+toggles sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options
+to fzf ```sh # CTRL-/ to toggle small preview window to see the full command #
+CTRL-Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS="
+--preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
 preview' --bind 'ctrl-y:execute-silent(echo -n {2..} | pbcopy)+abort' --color
 header:italic --header 'Press CTRL-Y to copy command into clipboard'" ``` -
 `ALT-C` - cd into the selected directory - The list is generated using `--
 walker dir,follow,hidden` option - Set `FZF_ALT_C_COMMAND` to override the
 default command - Or you can set `--walker-*` options in `FZF_ALT_C_OPTS` - Set
 `FZF_ALT_C_OPTS` to pass additional options to fzf ```sh # Print tree structure
 in the preview window export FZF_ALT_C_OPTS=" --walker-skip
```

### Comparing `fzf_bin-0.52.0/fzf/bin/fzf-preview.sh` & `fzf_bin-0.52.1/fzf/bin/fzf-preview.sh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/bin/fzf-tmux` & `fzf_bin-0.52.1/fzf/bin/fzf-tmux`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/doc/fzf.txt` & `fzf_bin-0.52.1/fzf/doc/fzf.txt`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/go.sum` & `fzf_bin-0.52.1/fzf/go.sum`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/install` & `fzf_bin-0.52.1/fzf/install`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 
 set -u
 
-version=0.52.0
+version=0.52.1
 auto_completion=
 key_bindings=
 update_config=2
 shells="bash zsh fish"
 prefix='~/.fzf'
 prefix_expand=~/.fzf
 fish_dir=${XDG_CONFIG_HOME:-$HOME/.config}/fish
```

### Comparing `fzf_bin-0.52.0/fzf/install.ps1` & `fzf_bin-0.52.1/fzf/install.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-$version="0.52.0"
+$version="0.52.1"
 
 $fzf_base=Split-Path -Parent $MyInvocation.MyCommand.Definition
 
 function check_binary () {
   Write-Host "  - Checking fzf executable ... " -NoNewline
   $output=cmd /c $fzf_base\bin\fzf.exe --version 2>&1
   if (-not $?) {
```

### Comparing `fzf_bin-0.52.0/fzf/main.go` & `fzf_bin-0.52.1/fzf/main.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/man/man1/fzf-tmux.1` & `fzf_bin-0.52.1/fzf/man/man1/fzf-tmux.1`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf-tmux 1 "May 2024" "fzf 0.52.0" "fzf-tmux - open fzf in tmux split pane"
+.TH fzf-tmux 1 "May 2024" "fzf 0.52.1" "fzf-tmux - open fzf in tmux split pane"
 
 .SH NAME
 fzf-tmux - open fzf in tmux split pane
 
 .SH SYNOPSIS
 .B fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS]
```

### Comparing `fzf_bin-0.52.0/fzf/man/man1/fzf.1` & `fzf_bin-0.52.1/fzf/man/man1/fzf.1`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf 1 "May 2024" "fzf 0.52.0" "fzf - a command-line fuzzy finder"
+.TH fzf 1 "May 2024" "fzf 0.52.1" "fzf - a command-line fuzzy finder"
 
 .SH NAME
 fzf - a command-line fuzzy finder
 
 .SH SYNOPSIS
 fzf [options]
 
@@ -42,18 +42,18 @@
 .B "-x, --extended"
 Extended-search mode. Since 0.10.9, this is enabled by default. You can disable
 it with \fB+x\fR or \fB--no-extended\fR.
 .TP
 .B "-e, --exact"
 Enable exact-match
 .TP
-.B "-i"
+.B "-i, --ignore-case"
 Case-insensitive match (default: smart-case match)
 .TP
-.B "+i"
+.B "+i, --no-ignore-case"
 Case-sensitive match
 .TP
 .B "--literal"
 Do not normalize latin script letters for matching.
 .TP
 .BI "--scheme=" SCHEME
 Choose scoring scheme tailored for different types of input.
```

### Comparing `fzf_bin-0.52.0/fzf/plugin/fzf.vim` & `fzf_bin-0.52.1/fzf/plugin/fzf.vim`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
       let slashes = 0
     else
       let slashes = 0
     endif
     let e .= c
   endfor
   let e .= repeat('\', slashes) .'"'
-  return e
+  return substitute(substitute(e, '[&|<>()^!"]', '^&', 'g'), '%', '%%', 'g')
 endfunction
 
 function! fzf#shellescape(arg, ...)
   let shell = get(a:000, 0, s:is_win ? 'cmd.exe' : 'sh')
   if shell =~# 'cmd.exe$'
     return s:shellesc_cmd(a:arg)
   endif
```

### Comparing `fzf_bin-0.52.0/fzf/shell/completion.bash` & `fzf_bin-0.52.1/fzf/shell/completion.bash`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,16 @@
     --color
     -d --delimiter
     -n --nth
     --with-nth
     +s --no-sort
     --track
     --tac
-    -i
-    +i
+    -i --ignore-case
+    +i --no-ignore-case
     -m --multi
     --ansi
     --no-mouse
     +c --no-color
     --no-bold
     --layout
     --reverse
```

### Comparing `fzf_bin-0.52.0/fzf/shell/completion.zsh` & `fzf_bin-0.52.1/fzf/shell/completion.zsh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/shell/key-bindings.bash` & `fzf_bin-0.52.1/fzf/shell/key-bindings.bash`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/shell/key-bindings.fish` & `fzf_bin-0.52.1/fzf/shell/key-bindings.fish`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/shell/key-bindings.zsh` & `fzf_bin-0.52.1/fzf/shell/key-bindings.zsh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/LICENSE` & `fzf_bin-0.52.1/fzf/src/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/actiontype_string.go` & `fzf_bin-0.52.1/fzf/src/actiontype_string.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/algo/algo.go` & `fzf_bin-0.52.1/fzf/src/algo/algo.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/algo/algo_test.go` & `fzf_bin-0.52.1/fzf/src/algo/algo_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/algo/normalize.go` & `fzf_bin-0.52.1/fzf/src/algo/normalize.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/ansi.go` & `fzf_bin-0.52.1/fzf/src/ansi.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/ansi_test.go` & `fzf_bin-0.52.1/fzf/src/ansi_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/cache.go` & `fzf_bin-0.52.1/fzf/src/cache.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/cache_test.go` & `fzf_bin-0.52.1/fzf/src/cache_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/chunklist.go` & `fzf_bin-0.52.1/fzf/src/chunklist.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/chunklist_test.go` & `fzf_bin-0.52.1/fzf/src/chunklist_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/constants.go` & `fzf_bin-0.52.1/fzf/src/constants.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/core.go` & `fzf_bin-0.52.1/fzf/src/core.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/functions.go` & `fzf_bin-0.52.1/fzf/src/functions.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/history.go` & `fzf_bin-0.52.1/fzf/src/history.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/history_test.go` & `fzf_bin-0.52.1/fzf/src/history_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/item.go` & `fzf_bin-0.52.1/fzf/src/item.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/matcher.go` & `fzf_bin-0.52.1/fzf/src/matcher.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/merger.go` & `fzf_bin-0.52.1/fzf/src/merger.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/merger_test.go` & `fzf_bin-0.52.1/fzf/src/merger_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/options.go` & `fzf_bin-0.52.1/fzf/src/options.go`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 const Usage = `usage: fzf [options]
 
   Search
     -x, --extended         Extended-search mode
                            (enabled by default; +x or --no-extended to disable)
     -e, --exact            Enable Exact-match
-    -i                     Case-insensitive match (default: smart-case match)
-    +i                     Case-sensitive match
+    -i, --ignore-case      Case-insensitive match (default: smart-case match)
+    +i, --no-ignore-case   Case-sensitive match
     --scheme=SCHEME        Scoring scheme [default|path|history]
     --literal              Do not normalize latin script letters before matching
     -n, --nth=N[,..]       Comma-separated list of field index expressions
                            for limiting search scope. Each can be a non-zero
                            integer or a range expression ([BEGIN]..[END]).
     --with-nth=N[,..]      Transform the presentation of each line using
                            field index expressions
@@ -1910,17 +1910,17 @@
 			opts.Track = trackEnabled
 		case "--no-track":
 			opts.Track = trackDisabled
 		case "--tac":
 			opts.Tac = true
 		case "--no-tac":
 			opts.Tac = false
-		case "-i":
+		case "-i", "--ignore-case":
 			opts.Case = CaseIgnore
-		case "+i":
+		case "+i", "--no-ignore-case":
 			opts.Case = CaseRespect
 		case "-m", "--multi":
 			if opts.Multi, err = optionalNumeric(allArgs, &i, maxMulti); err != nil {
 				return err
 			}
 		case "+m", "--no-multi":
 			opts.Multi = 0
```

### Comparing `fzf_bin-0.52.0/fzf/src/options_pprof.go` & `fzf_bin-0.52.1/fzf/src/options_pprof.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/options_pprof_test.go` & `fzf_bin-0.52.1/fzf/src/options_pprof_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/options_test.go` & `fzf_bin-0.52.1/fzf/src/options_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/pattern.go` & `fzf_bin-0.52.1/fzf/src/pattern.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/pattern_test.go` & `fzf_bin-0.52.1/fzf/src/pattern_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/reader.go` & `fzf_bin-0.52.1/fzf/src/reader.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/reader_test.go` & `fzf_bin-0.52.1/fzf/src/reader_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/result.go` & `fzf_bin-0.52.1/fzf/src/result.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/result_test.go` & `fzf_bin-0.52.1/fzf/src/result_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/server.go` & `fzf_bin-0.52.1/fzf/src/server.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/terminal.go` & `fzf_bin-0.52.1/fzf/src/terminal.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/terminal_test.go` & `fzf_bin-0.52.1/fzf/src/terminal_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tokenizer.go` & `fzf_bin-0.52.1/fzf/src/tokenizer.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tokenizer_test.go` & `fzf_bin-0.52.1/fzf/src/tokenizer_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/dummy.go` & `fzf_bin-0.52.1/fzf/src/tui/dummy.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/eventtype_string.go` & `fzf_bin-0.52.1/fzf/src/tui/eventtype_string.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/light.go` & `fzf_bin-0.52.1/fzf/src/tui/light.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/light_unix.go` & `fzf_bin-0.52.1/fzf/src/tui/light_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/light_windows.go` & `fzf_bin-0.52.1/fzf/src/tui/light_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/tcell.go` & `fzf_bin-0.52.1/fzf/src/tui/tcell.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/tcell_test.go` & `fzf_bin-0.52.1/fzf/src/tui/tcell_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/ttyname_unix.go` & `fzf_bin-0.52.1/fzf/src/tui/ttyname_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/tui/tui.go` & `fzf_bin-0.52.1/fzf/src/tui/tui.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/atexit.go` & `fzf_bin-0.52.1/fzf/src/util/atexit.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/atomicbool.go` & `fzf_bin-0.52.1/fzf/src/util/atomicbool.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/chars.go` & `fzf_bin-0.52.1/fzf/src/util/chars.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/chars_test.go` & `fzf_bin-0.52.1/fzf/src/util/chars_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/eventbox.go` & `fzf_bin-0.52.1/fzf/src/util/eventbox.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/eventbox_test.go` & `fzf_bin-0.52.1/fzf/src/util/eventbox_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/util.go` & `fzf_bin-0.52.1/fzf/src/util/util.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/util_test.go` & `fzf_bin-0.52.1/fzf/src/util/util_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/util_unix.go` & `fzf_bin-0.52.1/fzf/src/util/util_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/src/util/util_windows.go` & `fzf_bin-0.52.1/fzf/src/util/util_windows.go`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 package util
 
 import (
 	"fmt"
 	"os"
 	"os/exec"
 	"path/filepath"
+	"regexp"
 	"strings"
 	"sync/atomic"
 	"syscall"
 )
 
 type shellType int
 
 const (
 	shellTypeUnknown shellType = iota
 	shellTypeCmd
 	shellTypePowerShell
 )
 
+var escapeRegex = regexp.MustCompile(`[&|<>()^%!"]`)
+
 type Executor struct {
 	shell     string
 	shellType shellType
 	args      []string
 	shellPath atomic.Value
 }
 
@@ -127,15 +130,17 @@
 		}
 		b = append(b, c)
 	}
 	for ; slashes > 0; slashes-- {
 		b = append(b, '\\')
 	}
 	b = append(b, '"')
-	return string(b)
+	return escapeRegex.ReplaceAllStringFunc(string(b), func(match string) string {
+		return "^" + match
+	})
 }
 
 func (x *Executor) QuoteEntry(entry string) string {
 	switch x.shellType {
 	case shellTypeCmd:
 		/* Manually tested with the following commands:
 		   fzf --preview "echo {}"
```

### Comparing `fzf_bin-0.52.0/fzf/test/fzf.vader` & `fzf_bin-0.52.1/fzf/test/fzf.vader`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/test/test_go.rb` & `fzf_bin-0.52.1/fzf/test/test_go.rb`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/fzf/uninstall` & `fzf_bin-0.52.1/fzf/uninstall`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.52.0/pdm_build.py` & `fzf_bin-0.52.1/pdm_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "fzf"
-VERSION = "0.52.0"
+VERSION = "0.52.1"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `fzf_bin-0.52.0/pyproject.toml` & `fzf_bin-0.52.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fzf-bin"
 description = "fzf - 🌸 A command-line fuzzy finder"
-version = "0.52.0"
+version = "0.52.1"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `fzf_bin-0.52.0/PKG-INFO` & `fzf_bin-0.52.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fzf-bin
-Version: 0.52.0
+Version: 0.52.1
 Summary: fzf - 🌸 A command-line fuzzy finder
 Keywords: fzf,tui,fuzzy finder
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: User Interfaces
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

