# Comparing `tmp/urwid-2.6.8.tar.gz` & `tmp/urwid-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urwid-2.6.8.tar", last modified: Mon Mar  4 08:36:07 2024, max compression
+gzip compressed data, was "urwid-2.6.9.tar", last modified: Wed Mar 13 12:21:12 2024, max compression
```

## Comparing `urwid-2.6.8.tar` & `urwid-2.6.9.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.128993 urwid-2.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 08:36:02.000000 urwid-2.6.8/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.080993 urwid-2.6.8/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-04 08:36:02.000000 urwid-2.6.8/.devcontainer/dev.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-04 08:36:02.000000 urwid-2.6.8/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-04 08:36:02.000000 urwid-2.6.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.080993 urwid-2.6.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.080993 urwid-2.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.080993 urwid-2.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/workflows/isolated_static_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 08:36:02.000000 urwid-2.6.8/.github/workflows/yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-04 08:36:02.000000 urwid-2.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-04 08:36:02.000000 urwid-2.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-04 08:36:02.000000 urwid-2.6.8/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-03-04 08:36:02.000000 urwid-2.6.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-04 08:36:02.000000 urwid-2.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-04 08:36:07.128993 urwid-2.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-03-04 08:36:02.000000 urwid-2.6.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-04 08:36:02.000000 urwid-2.6.8/black-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-04 08:36:02.000000 urwid-2.6.8/classifiers.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.080993 urwid-2.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    41852 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.088993 urwid-2.6.8/docs/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/bigtext.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/bigtext.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/bigtext1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/bigtext2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/bigtext3.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/browse.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/browse1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/browse2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/edit.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/edit1.png
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/edit2.png
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/edit_text.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    11747 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/graph.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/graph1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/graph2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    21848 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/palette_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/palette_test.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/palette_test1.png
--rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/palette_test2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/pop_up.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/pop_up.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/pop_up1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/pop_up2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12009 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/real_browse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8054 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/real_edit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/subproc.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/subproc1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/subproc2.png
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/subproc2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14714 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/tour.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/tour.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/tour1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/examples/tour2.png
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.092993 urwid-2.6.8/docs/manual/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/bright_combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/bright_combinations.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/bright_combinations1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/canvascache.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/displayattributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/displaymodules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/encodings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.092993 urwid-2.6.8/docs/manual/images/
--rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/display_modules.png
--rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/introduction.png
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/urwid_widgets.svgz
--rw-r--r--   0 runner    (1001) docker     (127)    51992 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/urwid_widgets_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    64748 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/urwid_widgets_1.xcf
--rw-r--r--   0 runner    (1001) docker     (127)    70443 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/urwid_widgets_2.png
--rw-r--r--   0 runner    (1001) docker     (127)   206466 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/urwid_widgets_2.xcf
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/images/widget_layout.png
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/mainloop.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/overview.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/safe_combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/safe_combinations.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/safe_combinations1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/textlayout.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/userinput.rst
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wanat.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wanat_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wcur1.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wcur2.py
--rw-r--r--   0 runner    (1001) docker     (127)    33853 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/manual/wsel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.096993 urwid-2.6.8/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/attrspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/canvas.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/command_map.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/constants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/deprecated.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/display_modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/global_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/list_walkers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/main_loop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/meta.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/text_layout.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/reference/widget.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.096993 urwid-2.6.8/docs/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      411 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/compile_pngs.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/screenshots.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.096993 urwid-2.6.8/docs/tools/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/static/.placeholder
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.096993 urwid-2.6.8/docs/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/templates/indexcontent.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/templates/indexsidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tools/templates/localtoc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.104993 urwid-2.6.8/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/adventure4.png
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/cmenu4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/highcolors.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/highcolors.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/highcolors1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/hmenu4.png
--rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input1.png
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input2.png
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input3.png
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input4.png
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/input5.png
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/menu25.png
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/minimal.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/minimal1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple1.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/multiple4.png
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/qa.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/qa1.png
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/qa2.png
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/qa3.png
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig1.png
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig2.png
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig3.png
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/sig4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/smenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/smenu.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/smenu1.png
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/smenu2.png
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/smenu3.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr.py.xdotool
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr1.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr2.png
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr3.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/tutorial/urwid_attr4.png
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-04 08:36:02.000000 urwid-2.6.8/docs/urwid-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.108993 urwid-2.6.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5564 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/asyncio_socket_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/bigtext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12009 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/browse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27351 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/calc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11463 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/dialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8054 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/edit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4209 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/fib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11747 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4821 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/input_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10044 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/lcd_cf635.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21848 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/palette_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/pop_up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/subproc2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2710 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/terminal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14714 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/tour.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4883 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/treesample.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/twisted_serve_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-04 08:36:02.000000 urwid-2.6.8/examples/twisted_serve_ssh.tac
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 08:36:02.000000 urwid-2.6.8/isort-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-04 08:36:02.000000 urwid-2.6.8/pylint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-03-04 08:36:02.000000 urwid-2.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-04 08:36:02.000000 urwid-2.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-04 08:36:02.000000 urwid-2.6.8/ruff-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 08:36:07.128993 urwid-2.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-04 08:36:02.000000 urwid-2.6.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-04 08:36:02.000000 urwid-2.6.8/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.112993 urwid-2.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21234 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35895 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_escapes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_event_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_filler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_floatedit.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_font.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_grid_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_line_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    43876 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_listbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_moved_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_pile.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_raw_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_scrollable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_str_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16278 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_text_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_vterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-04 08:36:02.000000 urwid-2.6.8/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-04 08:36:02.000000 urwid-2.6.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.116993 urwid-2.6.8/urwid/
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46750 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/command_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/decoration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.120993 urwid-2.6.8/urwid/display/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_posix_raw_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_raw_display_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_web.css
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_web.js
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_win32.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/_win32_raw_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    39528 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/curses.py
--rw-r--r--   0 runner    (1001) docker     (127)    17968 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/html_fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17607 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/lcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    19250 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/display/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.120993 urwid-2.6.8/urwid/event_loop/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/abstract_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/asyncio_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/glib_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    26000 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/main_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/select_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/tornado_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/trio_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/twisted_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/event_loop/zmq_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    31932 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/font.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/numedit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/split_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/str_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    22821 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/text_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-04 08:36:06.000000 urwid-2.6.8/urwid/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    58410 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/vterm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.128993 urwid-2.6.8/urwid/widget/
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/attr_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/attr_wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/bar_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/big_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/box_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    46508 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7177 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)    23732 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/filler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21834 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    21514 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/grid_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/line_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    69495 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/listbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/monitored_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    34505 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    38628 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/pile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/popup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/scrollable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/solid_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/treetools.py
--rw-r--r--   0 runner    (1001) docker     (127)    29550 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/widget_decoration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27305 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/widget/wimp.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-04 08:36:02.000000 urwid-2.6.8/urwid/wimp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:36:07.128993 urwid-2.6.8/urwid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 08:36:07.000000 urwid-2.6.8/urwid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.673275 urwid-2.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-13 12:21:07.000000 urwid-2.6.9/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.629275 urwid-2.6.9/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-13 12:21:07.000000 urwid-2.6.9/.devcontainer/dev.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-13 12:21:07.000000 urwid-2.6.9/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-13 12:21:07.000000 urwid-2.6.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.629275 urwid-2.6.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.629275 urwid-2.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.629275 urwid-2.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/workflows/isolated_static_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/workflows/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-13 12:21:07.000000 urwid-2.6.9/.github/workflows/yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-13 12:21:07.000000 urwid-2.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-13 12:21:07.000000 urwid-2.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-13 12:21:07.000000 urwid-2.6.9/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-03-13 12:21:07.000000 urwid-2.6.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-13 12:21:07.000000 urwid-2.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-13 12:21:12.673275 urwid-2.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-03-13 12:21:07.000000 urwid-2.6.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-13 12:21:07.000000 urwid-2.6.9/black-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-13 12:21:07.000000 urwid-2.6.9/classifiers.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.633275 urwid-2.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    41852 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.637275 urwid-2.6.9/docs/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/bigtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/bigtext.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/bigtext1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/bigtext2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/bigtext3.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/browse.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/browse1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/browse2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/edit.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/edit1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/edit2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/edit_text.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11747 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/graph.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/graph1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/graph2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21848 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/palette_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/palette_test.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/palette_test1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/palette_test2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/pop_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/pop_up.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/pop_up1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/pop_up2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12026 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/real_browse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8054 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/real_edit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/subproc.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/subproc1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/subproc2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/subproc2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14714 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/tour.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/tour1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/examples/tour2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.641275 urwid-2.6.9/docs/manual/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/bright_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/bright_combinations.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/bright_combinations1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/canvascache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/displayattributes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/displaymodules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/encodings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.641275 urwid-2.6.9/docs/manual/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/display_modules.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/introduction.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/urwid_widgets.svgz
+-rw-r--r--   0 runner    (1001) docker     (127)    51992 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/urwid_widgets_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64748 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/urwid_widgets_1.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)    70443 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/urwid_widgets_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   206466 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/urwid_widgets_2.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/images/widget_layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/mainloop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/overview.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/safe_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/safe_combinations.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/safe_combinations1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/textlayout.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/userinput.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wanat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wanat_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wcur1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wcur2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33853 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/manual/wsel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.645275 urwid-2.6.9/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/attrspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/canvas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/command_map.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/deprecated.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/display_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/global_settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/list_walkers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/main_loop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/text_layout.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/reference/widget.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.645275 urwid-2.6.9/docs/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      411 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/compile_pngs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/screenshots.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.645275 urwid-2.6.9/docs/tools/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/static/.placeholder
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.645275 urwid-2.6.9/docs/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/templates/indexcontent.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/templates/indexsidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tools/templates/localtoc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.653275 urwid-2.6.9/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/adventure4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/cmenu4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/highcolors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/highcolors.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/highcolors1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/hmenu4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/input5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/menu25.png
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/minimal.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/minimal1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/multiple4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/qa.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/qa1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/qa2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/qa3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/sig4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/smenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/smenu.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/smenu1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/smenu2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/smenu3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr.py.xdotool
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/tutorial/urwid_attr4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-13 12:21:07.000000 urwid-2.6.9/docs/urwid-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.657275 urwid-2.6.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5564 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/asyncio_socket_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/bigtext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12026 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/browse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27351 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/calc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11463 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/dialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8054 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/edit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4209 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/fib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11747 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4821 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/input_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10044 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/lcd_cf635.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21848 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/palette_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/pop_up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/subproc2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2710 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/terminal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14714 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/tour.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4883 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/treesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/twisted_serve_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-13 12:21:07.000000 urwid-2.6.9/examples/twisted_serve_ssh.tac
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 12:21:07.000000 urwid-2.6.9/isort-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 12:21:07.000000 urwid-2.6.9/pylint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-03-13 12:21:07.000000 urwid-2.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-13 12:21:07.000000 urwid-2.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-13 12:21:07.000000 urwid-2.6.9/ruff-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:21:12.673275 urwid-2.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-13 12:21:07.000000 urwid-2.6.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-13 12:21:07.000000 urwid-2.6.9/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.661275 urwid-2.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21234 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35895 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_escapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_event_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_filler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_floatedit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_grid_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_line_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43876 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_listbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_moved_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_raw_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_scrollable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_str_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16278 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_text_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_vterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-13 12:21:07.000000 urwid-2.6.9/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-13 12:21:07.000000 urwid-2.6.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.665275 urwid-2.6.9/urwid/
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46750 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/command_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/decoration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.665275 urwid-2.6.9/urwid/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_posix_raw_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_raw_display_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_web.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_web.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_win32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/_win32_raw_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39528 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/curses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17826 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/html_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17607 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/lcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19250 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/display/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.669275 urwid-2.6.9/urwid/event_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/abstract_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/asyncio_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/glib_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26000 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/select_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/tornado_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/trio_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/twisted_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/event_loop/zmq_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31932 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/numedit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/split_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/str_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22821 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/text_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58410 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/vterm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.673275 urwid-2.6.9/urwid/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/attr_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/attr_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/bar_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/big_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/box_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46508 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7177 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23732 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/filler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21834 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21514 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/grid_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/line_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73579 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/listbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/monitored_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34505 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38628 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/popup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/scrollable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/solid_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17387 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/treetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29550 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/widget_decoration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27305 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/widget/wimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-13 12:21:07.000000 urwid-2.6.9/urwid/wimp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:21:12.673275 urwid-2.6.9/urwid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 12:21:12.000000 urwid-2.6.9/urwid.egg-info/top_level.txt
```

### Comparing `urwid-2.6.8/.devcontainer/devcontainer.json` & `urwid-2.6.9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.dockerignore` & `urwid-2.6.9/.dockerignore`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/CODE_OF_CONDUCT.md` & `urwid-2.6.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/ISSUE_TEMPLATE/feature_request.md` & `urwid-2.6.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/PULL_REQUEST_TEMPLATE.md` & `urwid-2.6.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/dependabot.yml` & `urwid-2.6.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/labeler.yml` & `urwid-2.6.9/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/release.yml` & `urwid-2.6.9/.github/release.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/workflows/documentation.yml` & `urwid-2.6.9/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/workflows/isolated_static_check.yml` & `urwid-2.6.9/.github/workflows/isolated_static_check.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.github/workflows/pythonpackage.yml` & `urwid-2.6.9/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.gitignore` & `urwid-2.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/.pre-commit-config.yaml` & `urwid-2.6.9/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   - repo: https://github.com/psf/black
     rev: 24.2.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.2.2
+    rev: v0.3.2
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/adrienverge/yamllint.git
     rev: v1.35.1
     hooks:
```

### Comparing `urwid-2.6.8/.yamllint.yml` & `urwid-2.6.9/.yamllint.yml`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/COPYING` & `urwid-2.6.9/COPYING`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/PKG-INFO` & `urwid-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urwid
-Version: 2.6.8
+Version: 2.6.9
 Summary: A full-featured console (xterm et al.) user interface library
 Home-page: https://urwid.org/
 Author-email: Ian Ward <ian@excess.org>
 License: LGPL-2.1-only
 Project-URL: Homepage, https://urwid.org/
 Project-URL: Documentation, https://urwid.org/manual/index.html
 Project-URL: Repository, https://github.com/urwid/urwid
```

### Comparing `urwid-2.6.8/README.rst` & `urwid-2.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/classifiers.txt` & `urwid-2.6.9/classifiers.txt`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/changelog.rst` & `urwid-2.6.9/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/conf.py` & `urwid-2.6.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,19 +222,19 @@
 htmlhelp_basename = "Urwiddoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
-    #'papersize': 'letterpaper',
+    # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
-    #'pointsize': '10pt',
+    # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
-    #'preamble': '',
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
     ("index", "Urwid.tex", "Urwid Documentation", "Ian Ward", "manual"),
 ]
```

### Comparing `urwid-2.6.8/docs/examples/bigtext.py` & `urwid-2.6.9/docs/examples/bigtext.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/bigtext1.png` & `urwid-2.6.9/docs/examples/bigtext1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/bigtext2.png` & `urwid-2.6.9/docs/examples/bigtext2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/bigtext3.png` & `urwid-2.6.9/docs/examples/bigtext3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/browse1.png` & `urwid-2.6.9/docs/examples/browse1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/browse2.png` & `urwid-2.6.9/docs/examples/browse2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/edit1.png` & `urwid-2.6.9/docs/examples/edit1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/edit2.png` & `urwid-2.6.9/docs/examples/edit2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/edit_text.txt` & `urwid-2.6.9/docs/examples/edit_text.txt`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/graph.py` & `urwid-2.6.9/docs/examples/graph.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/graph1.png` & `urwid-2.6.9/docs/examples/graph1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/graph2.png` & `urwid-2.6.9/docs/examples/graph2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/index.rst` & `urwid-2.6.9/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/palette_test.py` & `urwid-2.6.9/docs/examples/palette_test.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/palette_test1.png` & `urwid-2.6.9/docs/examples/palette_test1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/palette_test2.png` & `urwid-2.6.9/docs/examples/palette_test2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/pop_up.py` & `urwid-2.6.9/docs/examples/pop_up.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/pop_up1.png` & `urwid-2.6.9/docs/examples/pop_up1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/pop_up2.png` & `urwid-2.6.9/docs/examples/pop_up2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/real_browse.py` & `urwid-2.6.9/docs/examples/real_browse.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         cwd = os.getcwd()
         store_initial_cwd(cwd)
         self.header = urwid.Text("")
         self.listbox = urwid.TreeListBox(urwid.TreeWalker(DirectoryNode(cwd)))
         self.listbox.offset_rows = 1
         self.footer = urwid.AttrMap(urwid.Text(self.footer_text), "foot")
         self.view = urwid.Frame(
-            urwid.AttrMap(self.listbox, "body"),
+            urwid.AttrMap(urwid.ScrollBar(self.listbox), "body"),
             header=urwid.AttrMap(self.header, "head"),
             footer=self.footer,
         )
 
     def main(self) -> None:
         """Run the program."""
```

### Comparing `urwid-2.6.8/docs/examples/real_edit.py` & `urwid-2.6.9/docs/examples/real_edit.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/subproc.py` & `urwid-2.6.9/docs/examples/subproc.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/subproc1.png` & `urwid-2.6.9/docs/examples/subproc1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/subproc2.png` & `urwid-2.6.9/docs/examples/subproc2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/tour.py` & `urwid-2.6.9/docs/examples/tour.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/tour1.png` & `urwid-2.6.9/docs/examples/tour1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/examples/tour2.png` & `urwid-2.6.9/docs/examples/tour2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/bright_combinations.py` & `urwid-2.6.9/docs/manual/bright_combinations.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/bright_combinations1.png` & `urwid-2.6.9/docs/manual/bright_combinations1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/canvascache.rst` & `urwid-2.6.9/docs/manual/canvascache.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/displayattributes.rst` & `urwid-2.6.9/docs/manual/displayattributes.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/displaymodules.rst` & `urwid-2.6.9/docs/manual/displaymodules.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/encodings.rst` & `urwid-2.6.9/docs/manual/encodings.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/display_modules.png` & `urwid-2.6.9/docs/manual/images/display_modules.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/introduction.png` & `urwid-2.6.9/docs/manual/images/introduction.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/urwid_widgets.svgz` & `urwid-2.6.9/docs/manual/images/urwid_widgets.svgz`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/urwid_widgets_1.png` & `urwid-2.6.9/docs/manual/images/urwid_widgets_1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/urwid_widgets_1.xcf` & `urwid-2.6.9/docs/manual/images/urwid_widgets_1.xcf`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/urwid_widgets_2.png` & `urwid-2.6.9/docs/manual/images/urwid_widgets_2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/urwid_widgets_2.xcf` & `urwid-2.6.9/docs/manual/images/urwid_widgets_2.xcf`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/images/widget_layout.png` & `urwid-2.6.9/docs/manual/images/widget_layout.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/mainloop.rst` & `urwid-2.6.9/docs/manual/mainloop.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/overview.rst` & `urwid-2.6.9/docs/manual/overview.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/safe_combinations.py` & `urwid-2.6.9/docs/manual/safe_combinations.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/safe_combinations1.png` & `urwid-2.6.9/docs/manual/safe_combinations1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/textlayout.rst` & `urwid-2.6.9/docs/manual/textlayout.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/userinput.rst` & `urwid-2.6.9/docs/manual/userinput.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/wanat.py` & `urwid-2.6.9/docs/manual/wanat.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/wanat_multi.py` & `urwid-2.6.9/docs/manual/wanat_multi.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/wcur1.py` & `urwid-2.6.9/docs/manual/wcur1.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/widgets.rst` & `urwid-2.6.9/docs/manual/widgets.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/wmod.py` & `urwid-2.6.9/docs/manual/wmod.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/manual/wsel.py` & `urwid-2.6.9/docs/manual/wsel.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/reference/constants.rst` & `urwid-2.6.9/docs/reference/constants.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/reference/display_modules.rst` & `urwid-2.6.9/docs/reference/display_modules.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/reference/main_loop.rst` & `urwid-2.6.9/docs/reference/main_loop.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/reference/signals.rst` & `urwid-2.6.9/docs/reference/signals.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/reference/widget.rst` & `urwid-2.6.9/docs/reference/widget.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tools/screenshots.sh` & `urwid-2.6.9/docs/tools/screenshots.sh`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tools/templates/indexcontent.html` & `urwid-2.6.9/docs/tools/templates/indexcontent.html`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/adventure.py` & `urwid-2.6.9/docs/tutorial/adventure.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/adventure1.png` & `urwid-2.6.9/docs/tutorial/adventure1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/adventure2.png` & `urwid-2.6.9/docs/tutorial/adventure2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/adventure3.png` & `urwid-2.6.9/docs/tutorial/adventure3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/adventure4.png` & `urwid-2.6.9/docs/tutorial/adventure4.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/cmenu.py` & `urwid-2.6.9/docs/tutorial/cmenu.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/cmenu1.png` & `urwid-2.6.9/docs/tutorial/cmenu1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/cmenu2.png` & `urwid-2.6.9/docs/tutorial/cmenu2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/cmenu3.png` & `urwid-2.6.9/docs/tutorial/cmenu3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/cmenu4.png` & `urwid-2.6.9/docs/tutorial/cmenu4.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/highcolors.py` & `urwid-2.6.9/docs/tutorial/highcolors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import urwid
 
 
 def exit_on_q(key):
-    if key in ("q", "Q"):
+    if key in {"q", "Q"}:
         raise urwid.ExitMainLoop()
 
 
 palette = [
     ("banner", "", "", "", "#ffa", "#60d"),
     ("streak", "", "", "", "g50", "#60a"),
     ("inside", "", "", "", "g38", "#808"),
```

### Comparing `urwid-2.6.8/docs/tutorial/hmenu.py` & `urwid-2.6.9/docs/tutorial/hmenu.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/hmenu1.png` & `urwid-2.6.9/docs/tutorial/hmenu1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/hmenu2.png` & `urwid-2.6.9/docs/tutorial/hmenu2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/hmenu3.png` & `urwid-2.6.9/docs/tutorial/hmenu3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/hmenu4.png` & `urwid-2.6.9/docs/tutorial/hmenu4.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/index.rst` & `urwid-2.6.9/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/multiple.py` & `urwid-2.6.9/docs/tutorial/multiple.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/multiple2.png` & `urwid-2.6.9/docs/tutorial/multiple2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/multiple3.png` & `urwid-2.6.9/docs/tutorial/multiple3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/multiple4.png` & `urwid-2.6.9/docs/tutorial/multiple4.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/qa.py` & `urwid-2.6.9/docs/tutorial/qa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import urwid
 
 
 def exit_on_q(key: str) -> None:
-    if key in ("q", "Q"):
+    if key in {"q", "Q"}:
         raise urwid.ExitMainLoop()
 
 
 class QuestionBox(urwid.Filler):
     def keypress(self, size, key: str) -> str | None:
         if key != "enter":
             return super().keypress(size, key)
```

### Comparing `urwid-2.6.8/docs/tutorial/qa2.png` & `urwid-2.6.9/docs/tutorial/qa2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/qa3.png` & `urwid-2.6.9/docs/tutorial/qa3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/sig.py` & `urwid-2.6.9/docs/tutorial/sig.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/sig2.png` & `urwid-2.6.9/docs/tutorial/sig2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/sig3.png` & `urwid-2.6.9/docs/tutorial/sig3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/sig4.png` & `urwid-2.6.9/docs/tutorial/sig4.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/smenu.py` & `urwid-2.6.9/docs/tutorial/smenu.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/smenu1.png` & `urwid-2.6.9/docs/tutorial/smenu1.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/smenu2.png` & `urwid-2.6.9/docs/tutorial/smenu2.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/tutorial/smenu3.png` & `urwid-2.6.9/docs/tutorial/smenu3.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/docs/urwid-logo.png` & `urwid-2.6.9/docs/urwid-logo.png`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/asyncio_socket_server.py` & `urwid-2.6.9/examples/asyncio_socket_server.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/bigtext.py` & `urwid-2.6.9/examples/bigtext.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/browse.py` & `urwid-2.6.9/examples/browse.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         cwd = os.getcwd()
         store_initial_cwd(cwd)
         self.header = urwid.Text("")
         self.listbox = urwid.TreeListBox(urwid.TreeWalker(DirectoryNode(cwd)))
         self.listbox.offset_rows = 1
         self.footer = urwid.AttrMap(urwid.Text(self.footer_text), "foot")
         self.view = urwid.Frame(
-            urwid.AttrMap(self.listbox, "body"),
+            urwid.AttrMap(urwid.ScrollBar(self.listbox), "body"),
             header=urwid.AttrMap(self.header, "head"),
             footer=self.footer,
         )
 
     def main(self) -> None:
         """Run the program."""
```

### Comparing `urwid-2.6.8/examples/calc.py` & `urwid-2.6.9/examples/calc.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/dialog.py` & `urwid-2.6.9/examples/dialog.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/edit.py` & `urwid-2.6.9/examples/edit.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/fib.py` & `urwid-2.6.9/examples/fib.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/graph.py` & `urwid-2.6.9/examples/graph.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/input_test.py` & `urwid-2.6.9/examples/input_test.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/lcd_cf635.py` & `urwid-2.6.9/examples/lcd_cf635.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/palette_test.py` & `urwid-2.6.9/examples/palette_test.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/pop_up.py` & `urwid-2.6.9/examples/pop_up.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/subproc.py` & `urwid-2.6.9/examples/subproc.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/terminal.py` & `urwid-2.6.9/examples/terminal.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/tour.py` & `urwid-2.6.9/examples/tour.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/treesample.py` & `urwid-2.6.9/examples/treesample.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/examples/twisted_serve_ssh.py` & `urwid-2.6.9/examples/twisted_serve_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         """Render a canvas to the terminal.
 
         The canvas contains all the information required to render the Urwid
         UI. The content method returns a list of rows as (attr, cs, text)
         tuples. This very simple implementation iterates each row and simply
         writes it out.
         """
-        (maxcol, maxrow) = size
+        (_maxcol, _maxrow) = size
         # self.terminal.eraseDisplay()
         lasta = None
         for i, row in enumerate(canvas.content()):
             self.terminal.cursorPosition(0, i)
             for attr, _cs, text in row:
                 if attr != lasta:
                     text = f"{self._attr_to_escape(attr)}{text}"  # noqa: PLW2901
@@ -396,15 +396,15 @@
     def openShell(self, proto):
         """Open a shell."""
         self.chained_protocol = UrwidServerProtocol(UrwidTerminalProtocol, IUrwidMind(self.original))
         TerminalSessionTransport(proto, self.chained_protocol, IConchUser(self.original), self.height, self.width)
 
     def windowChanged(self, dimensions):
         """Called when the window size has changed."""
-        (h, w, x, y) = dimensions
+        (h, w, _x, _y) = dimensions
         self.chained_protocol.terminalProtocol.terminalSize(h, w)
 
 
 class UrwidRealm(TerminalRealm):
     """Custom terminal realm class-configured to use our custom Terminal User
     Terminal Session.
     """
```

### Comparing `urwid-2.6.8/examples/twisted_serve_ssh.tac` & `urwid-2.6.9/examples/twisted_serve_ssh.tac`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/pyproject.toml` & `urwid-2.6.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -174,15 +174,15 @@
   "RET", "SIM", "C4",  # flake8-return, flake8-simplify, flake8-comprehensions
   "ICN", "PGH",  # flake8-import-conventions, pygrep-hooks
   "Q",  # quotes
   "FLY",  # Flynt
   "TRY", "UP", "I", "PL", "PERF", "RUF",  # tryceratops, pyupgrade, isort, pylint + perflint, Ruff-specific
 ]
 extend-ignore = [
-  "PLR6301", "E203", "PLW3201",
+  "PLR6301", "E203",
     # refactor rules (too many statements/arguments/branches)
   "PLR0904", "PLR0911", "PLR0912", "PLR0913", "PLR0914", "PLR0915", "PLR0917", "PLR2004",
   "PLC0415",  # We have a lot of imports outside of top-level
   "RET504",  # Unnecessary variable assignment before return statement
   "SIM108",  # Use ternary operator,
   "TRY003",  #long messages prepare outside, ...
 ]
@@ -193,14 +193,23 @@
 
 [tool.ruff.lint.isort]
 known-third-party = []
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
+[tool.ruff.lint.pylint]
+allow-dunder-method-names = [
+  "__rich_repr__",
+  # class generation
+  "_contents__getitem__",
+  "_contents__setitem__",
+  "_contents__delitem__",
+]
+
 [tool.pylint]
 extension-pkg-whitelist = []
 ignore = ["CVS", "_version.py"]
 
 jobs = 0
 py-version = "3.7"
 
@@ -232,26 +241,23 @@
   "too-many-instance-attributes",
   "too-many-lines",
   "too-many-nested-blocks",
   "broad-except",
   "broad-exception-raised",
   "logging-fstring-interpolation",
   "logging-format-interpolation",
-  "consider-alternative-union-syntax",
-  "deprecated-typing-alias",
   "fixme",
   "invalid-name",
   "import-outside-toplevel",
   "cyclic-import",
   "missing-docstring",
   "use-implicit-booleaness-not-comparison-to-zero",
   "unused-argument",
   "unused-private-member",
   "arguments-differ",
-  "consider-alternative-union-syntax",
   "consider-using-assignment-expr",
   "superfluous-parens",
   # Magic part
   "invalid-overridden-method",
   "attribute-defined-outside-init",  # old bad practice, fixed step-by-step
   "redefined-variable-type",  # makes not happy typechecking, but super common
   # too complex union
```

### Comparing `urwid-2.6.8/setup.py` & `urwid-2.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_canvas.py` & `urwid-2.6.9/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_columns.py` & `urwid-2.6.9/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_container.py` & `urwid-2.6.9/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_doctests.py` & `urwid-2.6.9/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_escapes.py` & `urwid-2.6.9/tests/test_escapes.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_event_loops.py` & `urwid-2.6.9/tests/test_event_loops.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_filler.py` & `urwid-2.6.9/tests/test_filler.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_floatedit.py` & `urwid-2.6.9/tests/test_floatedit.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_font.py` & `urwid-2.6.9/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_frame.py` & `urwid-2.6.9/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_graphics.py` & `urwid-2.6.9/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_grid_flow.py` & `urwid-2.6.9/tests/test_grid_flow.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_line_box.py` & `urwid-2.6.9/tests/test_line_box.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_listbox.py` & `urwid-2.6.9/tests/test_listbox.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_main_loop.py` & `urwid-2.6.9/tests/test_main_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_moved_imports.py` & `urwid-2.6.9/tests/test_moved_imports.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_overlay.py` & `urwid-2.6.9/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_padding.py` & `urwid-2.6.9/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_pile.py` & `urwid-2.6.9/tests/test_pile.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_scrollable.py` & `urwid-2.6.9/tests/test_scrollable.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,17 +188,36 @@
     def test_negative(self):
         with self.assertRaises(ValueError):
             urwid.ScrollBar(urwid.Text(" "))
 
         with self.assertRaises(TypeError):
             urwid.ScrollBar(urwid.SolidFill(" "))
 
+    def test_no_scrollbar(self):
+        """If widget fit without scroll - no scrollbar needed"""
+        widget = urwid.ScrollBar(
+            urwid.Scrollable(urwid.BigText("1", urwid.HalfBlockHeavy6x5Font())),
+            trough_char=urwid.ScrollBar.Symbols.LITE_SHADE,
+            thumb_char=urwid.ScrollBar.Symbols.DARK_SHADE,
+        )
+        reduced_size = (8, 5)
+        self.assertEqual(
+            (
+                " ▐█▌    ",
+                " ▀█▌    ",
+                "  █▌    ",
+                "  █▌    ",
+                " ███▌   ",
+            ),
+            widget.render(reduced_size).decoded_text,
+        )
+
 
 class TestScrollBarListBox(unittest.TestCase):
-    def test_non_selectable(self):
+    def test_relative_non_selectable(self):
         widget = urwid.ScrollBar(
             urwid.ListBox(urwid.SimpleListWalker(urwid.Text(line) for line in LGPL_HEADER.splitlines()))
         )
 
         reduced_size = (40, 5)
 
         top_position_rendered = (
@@ -241,21 +260,23 @@
 
         widget.keypress(reduced_size, "page up")
 
         self.assertEqual(top_position_rendered, widget.render(reduced_size).decoded_text)
 
         widget.keypress(reduced_size, "end")
 
+        # Here we have ListBox issue: "end" really scroll not to the "dead end"
+        # in case of the bottom focus position is multiline
         self.assertEqual(
             (
+                "GNU Lesser General Public               ",
                 "License along with this library; if     ",
                 "not, write to the Free Software         ",
                 "Foundation, Inc., 51 Franklin Street,   ",
-                "Fifth Floor, Boston, MA  02110-1301     ",
-                "USA                                    █",
+                "Fifth Floor, Boston, MA  02110-1301    █",
             ),
             widget.render(reduced_size).decoded_text,
         )
 
         widget.keypress(reduced_size, "home")
 
         self.assertEqual(top_position_rendered, widget.render(reduced_size).decoded_text)
```

### Comparing `urwid-2.6.8/tests/test_signals.py` & `urwid-2.6.9/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_str_util.py` & `urwid-2.6.9/tests/test_str_util.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_text_layout.py` & `urwid-2.6.9/tests/test_text_layout.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_tree.py` & `urwid-2.6.9/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_util.py` & `urwid-2.6.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_vterm.py` & `urwid-2.6.9/tests/test_vterm.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tests/test_widget.py` & `urwid-2.6.9/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/tox.ini` & `urwid-2.6.9/tox.ini`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/__init__.py` & `urwid-2.6.9/urwid/__init__.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/canvas.py` & `urwid-2.6.9/urwid/canvas.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/command_map.py` & `urwid-2.6.9/urwid/command_map.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/container.py` & `urwid-2.6.9/urwid/container.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/decoration.py` & `urwid-2.6.9/urwid/decoration.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/__init__.py` & `urwid-2.6.9/urwid/display/__init__.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/_posix_raw_display.py` & `urwid-2.6.9/urwid/display/_posix_raw_display.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/_raw_display_base.py` & `urwid-2.6.9/urwid/display/_raw_display_base.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/_web.js` & `urwid-2.6.9/urwid/display/_web.js`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/_win32.py` & `urwid-2.6.9/urwid/display/_win32.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/_win32_raw_display.py` & `urwid-2.6.9/urwid/display/_win32_raw_display.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/common.py` & `urwid-2.6.9/urwid/display/common.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/curses.py` & `urwid-2.6.9/urwid/display/curses.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/escape.py` & `urwid-2.6.9/urwid/display/escape.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,25 +306,23 @@
         if not found_m:
             if more_available:
                 raise MoreInputRequired()
             return None
 
         (b, x, y) = (int(val) for val in value[:-1].split(";"))
         action = value[-1]
-
-        # shift, etc. is not communicated on my machine, so I
-        # can't and won't be able to add support for it.
-        # Double and triple clicks are not supported as well. They can be
-        # implemented by using a timer. This timer can check if the last
-        # registered click is below a certain threshold. This threshold
-        # is normally set in the operating system itself, so setting one
-        # here will cause an inconsistent behaviour. I do not plan to use
-        # that feature, so I won't implement it.
+        # Double and triple clicks are not supported.
+        # They can be implemented by using a timer.
+        # This timer can check if the last registered click is below a certain threshold.
+        # This threshold is normally set in the operating system itself,
+        # so setting one here will cause an inconsistent behaviour.
 
         prefixes = []
+        if b & 4:
+            prefixes.append("shift ")
         if b & 8:
             prefixes.append("meta ")
         if b & 16:
             prefixes.append("ctrl ")
         prefix = "".join(prefixes)
 
         wheel_used: typing.Literal[0, 1] = (b & 64) >> 6
```

### Comparing `urwid-2.6.8/urwid/display/html_fragment.py` & `urwid-2.6.9/urwid/display/html_fragment.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/lcd.py` & `urwid-2.6.9/urwid/display/lcd.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/raw.py` & `urwid-2.6.9/urwid/display/raw.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/display/web.py` & `urwid-2.6.9/urwid/display/web.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/__init__.py` & `urwid-2.6.9/urwid/event_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/abstract_loop.py` & `urwid-2.6.9/urwid/event_loop/abstract_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/asyncio_loop.py` & `urwid-2.6.9/urwid/event_loop/asyncio_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,17 +218,18 @@
             if not isinstance(exc, ExitMainLoop):
                 # Store the exc_info so we can re-raise after the loop stops
                 self._exc = exc
         else:
             loop.default_exception_handler(context)
 
     def run(self) -> None:
-        """
-        Start the event loop.  Exit the loop when any callback raises
-        an exception.  If ExitMainLoop is raised, exit cleanly.
+        """Start the event loop.
+
+        Exit the loop when any callback raises an exception.
+        If ExitMainLoop is raised, exit cleanly.
         """
         self._loop.set_exception_handler(self._exception_handler)
         self._loop.run_forever()
         if self._exc:
             exc = self._exc
             self._exc = None
             raise exc.with_traceback(exc.__traceback__)
```

### Comparing `urwid-2.6.8/urwid/event_loop/glib_loop.py` & `urwid-2.6.9/urwid/event_loop/glib_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/main_loop.py` & `urwid-2.6.9/urwid/event_loop/main_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/select_loop.py` & `urwid-2.6.9/urwid/event_loop/select_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/tornado_loop.py` & `urwid-2.6.9/urwid/event_loop/tornado_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/trio_loop.py` & `urwid-2.6.9/urwid/event_loop/trio_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,17 +156,18 @@
 
         emulate_idle_callbacks = _TrioIdleCallbackInstrument(self._idle_callbacks)
 
         with exceptiongroup.catch({BaseException: self._handle_main_loop_exception}):
             trio.run(self._main_task, instruments=[emulate_idle_callbacks])
 
     async def run_async(self) -> None:
-        """Starts the main loop and blocks asynchronously until the main loop
-        exits. This allows one to embed an urwid app in a Trio app even if the
-        Trio event loop is already running. Example::
+        """Starts the main loop and blocks asynchronously until the main loop exits.
+
+        This allows one to embed an urwid app in a Trio app even if the Trio event loop is already running.
+        Example::
 
             with trio.open_nursery() as nursery:
                 event_loop = urwid.TrioEventLoop()
 
                 # [...launch other async tasks in the nursery...]
 
                 loop = urwid.MainLoop(widget, event_loop=event_loop)
```

### Comparing `urwid-2.6.8/urwid/event_loop/twisted_loop.py` & `urwid-2.6.9/urwid/event_loop/twisted_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/event_loop/zmq_loop.py` & `urwid-2.6.9/urwid/event_loop/zmq_loop.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/font.py` & `urwid-2.6.9/urwid/font.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/graphics.py` & `urwid-2.6.9/urwid/graphics.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/numedit.py` & `urwid-2.6.9/urwid/numedit.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/signals.py` & `urwid-2.6.9/urwid/signals.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/split_repr.py` & `urwid-2.6.9/urwid/split_repr.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/str_util.py` & `urwid-2.6.9/urwid/str_util.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/text_layout.py` & `urwid-2.6.9/urwid/text_layout.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/util.py` & `urwid-2.6.9/urwid/util.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/vterm.py` & `urwid-2.6.9/urwid/vterm.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/__init__.py` & `urwid-2.6.9/urwid/widget/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,26 +57,23 @@
 )
 from .widget_decoration import WidgetDecoration, WidgetDisable, WidgetPlaceholder
 from .wimp import Button, CheckBox, CheckBoxError, RadioButton, SelectableIcon
 
 __all__ = (
     "ANY",
     "BOTTOM",
-    "MonitoredList",
-    "MonitoredFocusList",
     "BOX",
     "CENTER",
     "CLIP",
     "ELLIPSIS",
     "FIXED",
     "FLOW",
     "GIVEN",
     "LEFT",
     "MIDDLE",
-    "GridFlowWarning",
     "PACK",
     "RELATIVE",
     "RELATIVE_100",
     "RIGHT",
     "SPACE",
     "TOP",
     "WEIGHT",
@@ -87,28 +84,16 @@
     "BarGraph",
     "BarGraphError",
     "BarGraphMeta",
     "BigText",
     "BoxAdapter",
     "BoxAdapterError",
     "BoxWidget",
-    "ListWalkerError",
-    "ListWalker",
-    "SimpleListWalker",
-    "SimpleFocusListWalker",
-    "ListBoxError",
-    "ListBox",
     "Button",
     "CheckBox",
-    "TreeWidgetError",
-    "TreeWidget",
-    "TreeNode",
-    "ParentNode",
-    "TreeWalker",
-    "TreeListBox",
     "CheckBoxError",
     "Columns",
     "ColumnsError",
     "ColumnsWarning",
     "Divider",
     "Edit",
     "EditError",
@@ -117,37 +102,52 @@
     "FixedWidget",
     "FlowWidget",
     "Frame",
     "FrameError",
     "GraphVScale",
     "GridFlow",
     "GridFlowError",
+    "GridFlowWarning",
     "IntEdit",
     "LineBox",
+    "ListBox",
+    "ListBoxError",
+    "ListWalker",
+    "ListWalkerError",
+    "MonitoredFocusList",
+    "MonitoredList",
     "Overlay",
     "OverlayError",
     "OverlayWarning",
     "Padding",
     "PaddingError",
     "PaddingWarning",
+    "ParentNode",
     "Pile",
     "PileError",
     "PileWarning",
     "PopUpLauncher",
     "PopUpTarget",
     "ProgressBar",
     "RadioButton",
     "ScrollBar",
     "Scrollable",
     "ScrollableError",
     "SelectableIcon",
+    "SimpleFocusListWalker",
+    "SimpleListWalker",
     "Sizing",
     "SolidFill",
     "Text",
     "TextError",
+    "TreeListBox",
+    "TreeNode",
+    "TreeWalker",
+    "TreeWidget",
+    "TreeWidgetError",
     "VAlign",
     "WHSettings",
     "Widget",
     "WidgetContainerListContentsMixin",
     "WidgetContainerMixin",
     "WidgetDecoration",
     "WidgetDisable",
```

### Comparing `urwid-2.6.8/urwid/widget/attr_map.py` & `urwid-2.6.9/urwid/widget/attr_map.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/attr_wrap.py` & `urwid-2.6.9/urwid/widget/attr_wrap.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/bar_graph.py` & `urwid-2.6.9/urwid/widget/bar_graph.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/big_text.py` & `urwid-2.6.9/urwid/widget/big_text.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/box_adapter.py` & `urwid-2.6.9/urwid/widget/box_adapter.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/columns.py` & `urwid-2.6.9/urwid/widget/columns.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/constants.py` & `urwid-2.6.9/urwid/widget/constants.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/container.py` & `urwid-2.6.9/urwid/widget/container.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/divider.py` & `urwid-2.6.9/urwid/widget/divider.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/edit.py` & `urwid-2.6.9/urwid/widget/edit.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/filler.py` & `urwid-2.6.9/urwid/widget/filler.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/frame.py` & `urwid-2.6.9/urwid/widget/frame.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/grid_flow.py` & `urwid-2.6.9/urwid/widget/grid_flow.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/line_box.py` & `urwid-2.6.9/urwid/widget/line_box.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/listbox.py` & `urwid-2.6.9/urwid/widget/listbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,36 +39,43 @@
 if typing.TYPE_CHECKING:
     from collections.abc import Callable, Hashable
 
     from typing_extensions import Literal, Self
 
     from urwid.canvas import Canvas, CompositeCanvas
 
-__all__ = ("ListWalkerError", "ListWalker", "SimpleListWalker", "SimpleFocusListWalker", "ListBoxError", "ListBox")
+__all__ = (
+    "ListBox",
+    "ListBoxError",
+    "ListWalker",
+    "ListWalkerError",
+    "SimpleFocusListWalker",
+    "SimpleListWalker",
+    "VisibleInfo",
+    "VisibleInfoFillItem",
+    "VisibleInfoMiddle",
+    "VisibleInfoTopBottom",
+)
 
 _T = typing.TypeVar("_T")
 _K = typing.TypeVar("_K")
 
 
 class ListWalkerError(Exception):
     pass
 
 
 @runtime_checkable
-class ScrollSupportingBody(Sized, Protocol):
-    """Protocol for ListWalkers that support Scrolling."""
+class ScrollSupportingBody(Protocol):
+    """Protocol for ListWalkers."""
 
     def get_focus(self) -> tuple[Widget, _K]: ...
 
     def set_focus(self, position: _K) -> None: ...
 
-    def __getitem__(self, index: _K) -> _T: ...
-
-    def positions(self, reverse: bool = False) -> Iterable[_K]: ...
-
     def get_next(self, position: _K) -> tuple[Widget, _K] | tuple[None, None]: ...
 
     def get_prev(self, position: _K) -> tuple[Widget, _K] | tuple[None, None]: ...
 
 
 class ListWalker(metaclass=signals.MetaSignals):  # pylint: disable=no-member, unsubscriptable-object
     # mixin not named as mixin
@@ -272,37 +279,71 @@
         return range(len(self))
 
 
 class ListBoxError(Exception):
     pass
 
 
-class _Middle(typing.NamedTuple):
+class VisibleInfoMiddle(typing.NamedTuple):
     """Named tuple for ListBox internals."""
 
     offset: int
     focus_widget: Widget
     focus_pos: Hashable
     focus_rows: int
     cursor: tuple[int, int] | tuple[int] | None
 
 
-class _FillItem(typing.NamedTuple):
+class VisibleInfoFillItem(typing.NamedTuple):
     """Named tuple for ListBox internals."""
 
     widget: Widget
     position: Hashable
     rows: int
 
 
-class _TopBottom(typing.NamedTuple):
+class VisibleInfoTopBottom(typing.NamedTuple):
     """Named tuple for ListBox internals."""
 
     trim: int
-    fill: list[_FillItem]
+    fill: list[VisibleInfoFillItem]
+
+    @classmethod
+    def from_raw_data(
+        cls,
+        trim: int,
+        fill: Iterable[tuple[Widget, Hashable, int]],
+    ) -> Self:
+        """Construct from not typed data.
+
+        Useful for overridden cases."""
+        return cls(trim=trim, fill=[VisibleInfoFillItem(*item) for item in fill])  # pragma: no cover
+
+
+class VisibleInfo(typing.NamedTuple):
+    middle: VisibleInfoMiddle
+    top: VisibleInfoTopBottom
+    bottom: VisibleInfoTopBottom
+
+    @classmethod
+    def from_raw_data(
+        cls,
+        middle: tuple[int, Widget, Hashable, int, tuple[int, int] | tuple[int] | None],
+        top: tuple[int, Iterable[tuple[Widget, Hashable, int]]],
+        bottom: tuple[int, Iterable[tuple[Widget, Hashable, int]]],
+    ) -> Self:
+        """Construct from not typed data.
+
+        Useful for overridden cases.
+        """
+        return cls(  # pragma: no cover
+            middle=VisibleInfoMiddle(*middle),
+            top=VisibleInfoTopBottom.from_raw_data(*top),
+            bottom=VisibleInfoTopBottom.from_raw_data(*bottom),
+        )
 
 
 class ListBox(Widget, WidgetContainerMixin):
     """
     Vertically stacked list of widgets
     """
 
@@ -395,15 +436,15 @@
             return len(self._body)
         raise AttributeError(f"{self._body.__class__.__name__} is not Sized")
 
     def calculate_visible(
         self,
         size: tuple[int, int],
         focus: bool = False,
-    ) -> tuple[_Middle, _TopBottom, _TopBottom] | tuple[None, None, None]:
+    ) -> VisibleInfo | tuple[None, None, None]:
         """
         Returns the widgets that would be displayed in
         the ListBox given the current *size* and *focus*.
 
         see :meth:`Widget.render` for parameter details
 
         :returns: (*middle*, *top*, *bottom*) or (``None``, ``None``, ``None``)
@@ -466,15 +507,15 @@
             if prev is None:  # run out of widgets above?
                 offset_rows -= fill_lines
                 break
             top_pos = pos
 
             p_rows = prev.rows((maxcol,))
             if p_rows:  # filter out 0-height widgets
-                fill_above.append(_FillItem(prev, pos, p_rows))
+                fill_above.append(VisibleInfoFillItem(prev, pos, p_rows))
             if p_rows > fill_lines:  # crosses top edge?
                 trim_top = p_rows - fill_lines
                 break
             fill_lines -= p_rows
 
         trim_bottom = max(focus_rows + offset_rows - inset_rows - maxrow, 0)
 
@@ -485,15 +526,15 @@
         while fill_lines > 0:
             next_pos, pos = self._body.get_next(pos)
             if next_pos is None:  # run out of widgets below?
                 break
 
             n_rows = next_pos.rows((maxcol,))
             if n_rows:  # filter out 0-height widgets
-                fill_below.append(_FillItem(next_pos, pos, n_rows))
+                fill_below.append(VisibleInfoFillItem(next_pos, pos, n_rows))
             if n_rows > fill_lines:  # crosses bottom edge?
                 trim_bottom = n_rows - fill_lines
                 fill_lines -= n_rows
                 break
             fill_lines -= n_rows
 
         # 4. fill from top again if necessary & possible
@@ -511,34 +552,48 @@
         pos = top_pos
         while fill_lines > 0:
             prev, pos = self._body.get_prev(pos)
             if prev is None:
                 break
 
             p_rows = prev.rows((maxcol,))
-            fill_above.append(_FillItem(prev, pos, p_rows))
+            fill_above.append(VisibleInfoFillItem(prev, pos, p_rows))
             if p_rows > fill_lines:  # more than required
                 trim_top = p_rows - fill_lines
                 offset_rows += fill_lines
                 break
             fill_lines -= p_rows
             offset_rows += p_rows
 
         # 5. return the interesting bits
-        return (
-            _Middle(offset_rows - inset_rows, focus_widget, focus_pos, focus_rows, cursor),
-            _TopBottom(trim_top, fill_above),
-            _TopBottom(trim_bottom, fill_below),
+        return VisibleInfo(
+            VisibleInfoMiddle(offset_rows - inset_rows, focus_widget, focus_pos, focus_rows, cursor),
+            VisibleInfoTopBottom(trim_top, fill_above),
+            VisibleInfoTopBottom(trim_bottom, fill_below),
         )
 
-    def get_scrollpos(self, size: tuple[int, int] | None = None, focus: bool = False) -> int:
-        """Current scrolling position."""
+    def _check_support_scrolling(self) -> None:
+        from .treetools import TreeWalker
+
         if not isinstance(self._body, ScrollSupportingBody):
             raise ListBoxError(f"{self} body do not implement methods required for scrolling protocol")
 
+        if not isinstance(self._body, (Sized, TreeWalker)):
+            raise ListBoxError(
+                f"{self} body is not a Sized and not a TreeWalker."
+                f"Scroll is not allowed due to risk of infinite cycle of widgets load."
+            )
+
+        if getattr(self._body, "wrap_around", False):
+            raise ListBoxError("Body is wrapped around. Scroll position calculation is undefined.")
+
+    def get_scrollpos(self, size: tuple[int, int] | None = None, focus: bool = False) -> int:
+        """Current scrolling position."""
+        self._check_support_scrolling()
+
         if not self._body:
             return 0
 
         if size is not None:
             self._rendered_size = size
 
         mid, top, _bottom = self.calculate_visible(self._rendered_size, focus)
@@ -556,30 +611,73 @@
             start_row += prev.rows((maxcol,))
             prev, pos = self._body.get_prev(pos)
 
         return start_row
 
     def rows_max(self, size: tuple[int, int] | None = None, focus: bool = False) -> int:
         """Scrollable protocol for sized iterable and not wrapped around contents."""
-        if not isinstance(self._body, ScrollSupportingBody):
-            raise ListBoxError(f"{self} body do not implement methods required for scrolling protocol")
-
-        if getattr(self._body, "wrap_around", False):
-            raise ListBoxError("Body is wrapped around")
+        self._check_support_scrolling()
 
         if size is not None:
             self._rendered_size = size
 
         if size or not self._rows_max_cached:
-            self._rows_max_cached = sum(
-                self._body[position].rows((self._rendered_size[0],), focus) for position in self._body.positions()
-            )
+            cols = self._rendered_size[0]
+            rows = 0
+
+            focused_w, idx = self.body.get_focus()
+            rows += focused_w.rows((cols,), focus)
+
+            prev, pos = self._body.get_prev(idx)
+            while prev is not None:
+                rows += prev.rows((cols,), False)
+                prev, pos = self._body.get_prev(pos)
+
+            next_, pos = self.body.get_next(idx)
+            while next_ is not None:
+                rows += next_.rows((cols,), True)
+                next_, pos = self._body.get_next(pos)
+
+            self._rows_max_cached = rows
 
         return self._rows_max_cached
 
+    def require_relative_scroll(self, size: tuple[int, int], focus: bool = False) -> bool:
+        """Widget require relative scroll due to performance limitations of real lines count calculation."""
+        return isinstance(self._body, Sized) and (size[1] * 3 < len(self))
+
+    def get_first_visible_pos(self, size: tuple[int, int], focus: bool = False) -> int:
+        self._check_support_scrolling()
+
+        if not self._body:
+            return 0
+
+        _mid, top, _bottom = self.calculate_visible(size, focus)
+        if top.fill:
+            first_pos = top.fill[-1].position
+        else:
+            first_pos = self.focus_position
+
+        over = 0
+        _widget, first_pos = self.body.get_prev(first_pos)
+        while first_pos is not None:
+            over += 1
+            _widget, first_pos = self.body.get_prev(first_pos)
+
+        return over
+
+    def get_visible_amount(self, size: tuple[int, int], focus: bool = False) -> int:
+        self._check_support_scrolling()
+
+        if not self._body:
+            return 1
+
+        _mid, top, bottom = self.calculate_visible(size, focus)
+        return 1 + len(top.fill) + len(bottom.fill)
+
     def render(
         self,
         size: tuple[int, int],  # type: ignore[override]
         focus: bool = False,
     ) -> CompositeCanvas | SolidCanvas:
         """
         Render ListBox and return canvas.
@@ -590,17 +688,17 @@
 
         self._rendered_size = size
 
         middle, top, bottom = self.calculate_visible((maxcol, maxrow), focus=focus)
         if middle is None:
             return SolidCanvas(" ", maxcol, maxrow)
 
-        _ignore, focus_widget, focus_pos, focus_rows, cursor = middle
-        trim_top, fill_above = top
-        trim_bottom, fill_below = bottom
+        _ignore, focus_widget, focus_pos, focus_rows, cursor = middle  # pylint: disable=unpacking-non-sequence
+        trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
+        trim_bottom, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         combinelist: list[tuple[Canvas, int, bool]] = []
         rows = 0
         fill_above.reverse()  # fill_above is in bottom-up order
         for widget, w_pos, w_rows in fill_above:
             canvas = widget.render((maxcol,))
             if w_rows != canvas.rows():
@@ -702,15 +800,15 @@
         """
         (maxcol, maxrow) = size
 
         middle, _top, _bottom = self.calculate_visible((maxcol, maxrow), True)
         if middle is None:
             return None
 
-        offset_inset, _ignore1, _ignore2, _ignore3, cursor = middle
+        offset_inset, _ignore1, _ignore2, _ignore3, cursor = middle  # pylint: disable=unpacking-non-sequence
         if not cursor:
             return None
 
         x, y = cursor
         y += offset_inset
         if y < 0 or y >= maxrow:
             return None
@@ -893,17 +991,17 @@
         (maxcol, maxrow) = size
         self.set_focus_valign_pending = None
         self.set_focus_pending = None
         middle, top, bottom = self.calculate_visible((maxcol, maxrow), focus=focus)
         if middle is None:
             return
 
-        row_offset, focus_widget, _focus_pos, focus_rows, _cursor = middle
-        _trim_top, _fill_above = top
-        trim_bottom, fill_below = bottom
+        row_offset, focus_widget, _focus_pos, focus_rows, _cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_top, _fill_above = top  # pylint: disable=unpacking-non-sequence
+        trim_bottom, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         if focus_widget.selectable():
             return
 
         if trim_bottom:
             fill_below = fill_below[:-1]
         new_row_offset = row_offset + focus_rows
@@ -931,17 +1029,17 @@
             # do nothing
             return None
 
         # restore old focus temporarily
         self._body.set_focus(focus_pos)
 
         middle, top, bottom = self.calculate_visible((maxcol, maxrow), focus)
-        focus_offset, _focus_widget, focus_pos, focus_rows, _cursor = middle
-        _trim_top, fill_above = top
-        _trim_bottom, fill_below = bottom
+        focus_offset, _focus_widget, focus_pos, focus_rows, _cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
+        _trim_bottom, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         offset = focus_offset
         for _widget, pos, rows in fill_above:
             offset -= rows
             if pos == position:
                 self.change_focus((maxcol, maxrow), pos, offset, "below")
                 return None
@@ -1247,16 +1345,16 @@
     def _keypress_up(self, size: tuple[int, int]) -> bool | None:
         (maxcol, maxrow) = size
 
         middle, top, _bottom = self.calculate_visible((maxcol, maxrow), True)
         if middle is None:
             return True
 
-        focus_row_offset, focus_widget, focus_pos, _ignore, cursor = middle
-        _trim_top, fill_above = top
+        focus_row_offset, focus_widget, focus_pos, _ignore, cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
 
         row_offset = focus_row_offset
 
         # look for selectable widget above
         pos = focus_pos
         widget = None
         for widget, pos, rows in fill_above:
@@ -1320,16 +1418,16 @@
     def _keypress_down(self, size: tuple[int, int]) -> bool | None:
         (maxcol, maxrow) = size
 
         middle, _top, bottom = self.calculate_visible((maxcol, maxrow), True)
         if middle is None:
             return True
 
-        focus_row_offset, focus_widget, focus_pos, focus_rows, cursor = middle
-        _trim_bottom, fill_below = bottom
+        focus_row_offset, focus_widget, focus_pos, focus_rows, cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_bottom, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         row_offset = focus_row_offset + focus_rows
         rows = focus_rows
 
         # look for selectable widget below
         pos = focus_pos
         widget = None
@@ -1359,17 +1457,14 @@
 
         if not focus_widget.selectable() or focus_row_offset + focus_rows - 1 <= 0:
             # just take bottom one if current is not selectable
             # or if focus has moved out of view
             if widget is None:
                 self.shift_focus((maxcol, maxrow), row_offset - rows)
                 return None
-            # FIXME: catch this bug in testcase
-            # self.change_focus((maxcol,maxrow), pos,
-            #    row_offset+rows, 'above')
             self.change_focus((maxcol, maxrow), pos, row_offset - rows, "above")
             return None
 
         # check if cursor will stop scroll from taking effect
         if cursor is not None:
             _x, y = cursor
             if y + focus_row_offset - 1 < 0:
@@ -1402,16 +1497,16 @@
     def _keypress_page_up(self, size: tuple[int, int]) -> bool | None:
         (maxcol, maxrow) = size
 
         middle, top, _bottom = self.calculate_visible((maxcol, maxrow), True)
         if middle is None:
             return True
 
-        row_offset, focus_widget, focus_pos, focus_rows, cursor = middle
-        _trim_top, fill_above = top
+        row_offset, focus_widget, focus_pos, focus_rows, cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
 
         # topmost_visible is row_offset rows above top row of
         # focus (+ve) or -row_offset rows below top row of focus (-ve)
         topmost_visible = row_offset
 
         # scroll_from_row is (first match)
         # 1. topmost visible row if focus is not selectable
@@ -1512,15 +1607,15 @@
 
             # if we're as far up as we can scroll, take this one
             if fill_above and self._body.get_prev(fill_above[-1][1]) == (None, None):
                 pass  # return
 
             # find out where that actually puts us
             middle, top, _bottom = self.calculate_visible((maxcol, maxrow), True)
-            act_row_offset, _ign1, _ign2, _ign3, _ign4 = middle
+            act_row_offset, _ign1, _ign2, _ign3, _ign4 = middle  # pylint: disable=unpacking-non-sequence
 
             # discard chosen widget if it will reduce scroll amount
             # because of a fixed cursor (absolute last resort)
             if act_row_offset > row_offset + snap_rows:
                 bad_choices.append(i)
                 continue
             if act_row_offset < row_offset:
@@ -1562,15 +1657,15 @@
             return None
 
         # no choices available, just shift current one
         self.shift_focus((maxcol, maxrow), min(maxrow - 1, row_offset))
 
         # final check for pathological case where we may fall short
         middle, top, _bottom = self.calculate_visible((maxcol, maxrow), True)
-        act_row_offset, _ign1, pos, _ign2, _ign3 = middle
+        act_row_offset, _ign1, pos, _ign2, _ign3 = middle  # pylint: disable=unpacking-non-sequence
         if act_row_offset >= row_offset:
             # no problem
             return None
 
         # fell short, try to select anything else above
         if not t:
             return None
@@ -1594,16 +1689,16 @@
     def _keypress_page_down(self, size: tuple[int, int]) -> bool | None:
         (maxcol, maxrow) = size
 
         middle, _top, bottom = self.calculate_visible((maxcol, maxrow), True)
         if middle is None:
             return True
 
-        row_offset, focus_widget, focus_pos, focus_rows, cursor = middle
-        _trim_bottom, fill_below = bottom
+        row_offset, focus_widget, focus_pos, focus_rows, cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_bottom, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         # bottom_edge is maxrow-focus_pos rows below top row of focus
         bottom_edge = maxrow - row_offset
 
         # scroll_from_row is (first match)
         # 1. bottom edge if focus is not selectable
         # 2. row containing cursor + 1 if focus has a cursor
@@ -1700,15 +1795,15 @@
                     "above",
                     (self.pref_col, pref_row),
                     snap_rows,
                 )
 
             # find out where that actually puts us
             middle, _top, bottom = self.calculate_visible((maxcol, maxrow), True)
-            act_row_offset, _ign1, _ign2, _ign3, _ign4 = middle
+            act_row_offset, _ign1, _ign2, _ign3, _ign4 = middle  # pylint: disable=unpacking-non-sequence
 
             # discard chosen widget if it will reduce scroll amount
             # because of a fixed cursor (absolute last resort)
             if act_row_offset < row_offset - snap_rows:
                 bad_choices.append(i)
                 continue
             if act_row_offset > row_offset:
@@ -1746,15 +1841,15 @@
             return None
 
         # no choices available, just shift current one
         self.shift_focus((maxcol, maxrow), max(1 - focus_rows, row_offset))
 
         # final check for pathological case where we may fall short
         middle, _top, bottom = self.calculate_visible((maxcol, maxrow), True)
-        act_row_offset, _ign1, pos, _ign2, _ign3 = middle
+        act_row_offset, _ign1, pos, _ign2, _ign3 = middle  # pylint: disable=unpacking-non-sequence
         if act_row_offset <= row_offset:
             # no problem
             return None
 
         # fell short, try to select anything else below
         if not t:
             return None
@@ -1791,17 +1886,17 @@
         from urwid.util import is_mouse_press
 
         (maxcol, maxrow) = size
         middle, top, bottom = self.calculate_visible((maxcol, maxrow), focus=True)
         if middle is None:
             return False
 
-        _ignore, focus_widget, focus_pos, focus_rows, _cursor = middle
-        trim_top, fill_above = top
-        _ignore, fill_below = bottom
+        _ignore, focus_widget, focus_pos, focus_rows, _cursor = middle  # pylint: disable=unpacking-non-sequence
+        trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
+        _ignore, fill_below = bottom  # pylint: disable=unpacking-non-sequence
 
         fill_above.reverse()  # fill_above is in bottom-up order
         w_list = [*fill_above, (focus_widget, focus_pos, focus_rows), *fill_below]
 
         wrow = -trim_top
         for w, w_pos, w_rows in w_list:  # noqa: B007  # magic with scope
             if wrow + w_rows > row:
@@ -1846,27 +1941,27 @@
         of the list are visible
         """
         (maxcol, maxrow) = size
         result = []
         middle, top, bottom = self.calculate_visible((maxcol, maxrow), focus=focus)
         if middle is None:  # empty listbox
             return ["top", "bottom"]
-        trim_top, above = top
-        trim_bottom, below = bottom
+        trim_top, above = top  # pylint: disable=unpacking-non-sequence
+        trim_bottom, below = bottom  # pylint: disable=unpacking-non-sequence
 
         if trim_bottom == 0:
-            row_offset, _w, pos, rows, _c = middle
+            row_offset, _w, pos, rows, _c = middle  # pylint: disable=unpacking-non-sequence
             row_offset += rows
             for _w, pos, rows in below:  # noqa: B007  # magic with scope
                 row_offset += rows
             if row_offset < maxrow or (self._body.get_next(pos) == (None, None)):
                 result.append("bottom")
 
         if trim_top == 0:
-            row_offset, _w, pos, _rows, _c = middle
+            row_offset, _w, pos, _rows, _c = middle  # pylint: disable=unpacking-non-sequence
             for _w, pos, rows in above:  # noqa: B007  # magic with scope
                 row_offset -= rows
             if self._body.get_prev(pos) == (None, None):
                 result.insert(0, "top")
 
         return result
```

### Comparing `urwid-2.6.8/urwid/widget/monitored_list.py` & `urwid-2.6.9/urwid/widget/monitored_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from collections.abc import Callable, Collection, Iterator
 
     from typing_extensions import Concatenate, ParamSpec
 
     ArgSpec = ParamSpec("ArgSpec")
     Ret = typing.TypeVar("Ret")
 
-__all__ = ("MonitoredList", "MonitoredFocusList")
+__all__ = ("MonitoredFocusList", "MonitoredList")
 
 _T = typing.TypeVar("_T")
 
 
 def _call_modified(
     fn: Callable[Concatenate[MonitoredList, ArgSpec], Ret]
 ) -> Callable[Concatenate[MonitoredList, ArgSpec], Ret]:
```

### Comparing `urwid-2.6.8/urwid/widget/overlay.py` & `urwid-2.6.9/urwid/widget/overlay.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/padding.py` & `urwid-2.6.9/urwid/widget/padding.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/pile.py` & `urwid-2.6.9/urwid/widget/pile.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/popup.py` & `urwid-2.6.9/urwid/widget/popup.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/progress_bar.py` & `urwid-2.6.9/urwid/widget/progress_bar.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/scrollable.py` & `urwid-2.6.9/urwid/widget/scrollable.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     DRAWING_HEAVY_3_DASH = BOX_SYMBOLS.HEAVY.VERTICAL_3_DASH
     DRAWING_HEAVY_4_DASH = BOX_SYMBOLS.HEAVY.VERTICAL_4_DASH
 
     DRAWING_DOUBLE = BOX_SYMBOLS.DOUBLE.VERTICAL
 
 
 @runtime_checkable
-class SupportsScroll(Protocol):
-    """Protocol for scroll supporting widget.
+class WidgetProto(Protocol):
+    """Protocol for widget.
 
-    Due to protocol can not inherit non-protocol bases, require also several obligatory Widget methods.
+    Due to protocol cannot inherit non-protocol bases, define several obligatory Widget methods.
     """
 
     # Base widget methods (from Widget)
     def sizing(self) -> frozenset[Sizing]: ...
 
     def selectable(self) -> bool: ...
 
@@ -112,20 +112,37 @@
         col: int,
         row: int,
         focus: bool,
     ) -> bool | None: ...
 
     def render(self, size: tuple[int, int], focus: bool = False) -> Canvas: ...
 
-    # Scroll specific methods
+
+@runtime_checkable
+class SupportsScroll(WidgetProto, Protocol):
+    """Scroll specific methods."""
+
     def get_scrollpos(self, size: tuple[int, int], focus: bool = False) -> int: ...
 
     def rows_max(self, size: tuple[int, int] | None = None, focus: bool = False) -> int: ...
 
 
+@runtime_checkable
+class SupportsRelativeScroll(WidgetProto, Protocol):
+    """Relative scroll-specific methods."""
+
+    def __len__(self) -> int: ...
+
+    def require_relative_scroll(self, size: tuple[int, int], focus: bool = False) -> bool: ...
+
+    def get_first_visible_pos(self, size: tuple[int, int], focus: bool = False) -> int: ...
+
+    def get_visible_amount(self, size: tuple[int, int], focus: bool = False) -> int: ...
+
+
 class Scrollable(WidgetDecoration[WrappedWidget]):
     def sizing(self) -> frozenset[Sizing]:
         return frozenset((Sizing.BOX,))
 
     def selectable(self) -> bool:
         return True
 
@@ -282,23 +299,23 @@
         from urwid.command_map import Command
 
         # Maybe offer key to original widget
         if self._forward_keypress or self.force_forward_keypress:
             ow = self._original_widget
             ow_size = self._get_original_widget_size(size)
 
-            # Remember previous cursor position if possible
+            # Remember the previous cursor position if possible
             if hasattr(ow, "get_cursor_coords"):
                 self._old_cursor_coords = ow.get_cursor_coords(ow_size)
 
             key = ow.keypress(ow_size, key)
             if key is None:
                 return None
 
-        # Handle up/down, page up/down, etc
+        # Handle up/down, page up/down, etc.
         command_map = self._command_map
         if command_map[key] == Command.UP:
             self._scroll_action = SCROLL_LINE_UP
         elif command_map[key] == Command.DOWN:
             self._scroll_action = SCROLL_LINE_DOWN
 
         elif command_map[key] == Command.PAGE_UP:
@@ -434,18 +451,18 @@
                 raise ScrollableError(f"Not a flow/box widget: {self._original_widget!r}")
         return self._rows_max_cached
 
 
 class ScrollBar(WidgetDecoration[WrappedWidget]):
     Symbols = ScrollbarSymbols
 
-    def sizing(self):
+    def sizing(self) -> frozenset[Sizing]:
         return frozenset((Sizing.BOX,))
 
-    def selectable(self):
+    def selectable(self) -> bool:
         return True
 
     def __init__(
         self,
         widget: WrappedWidget,
         thumb_char: str = ScrollbarSymbols.FULL_BLOCK,
         trough_char: str = " ",
@@ -479,38 +496,54 @@
     def render(
         self,
         size: tuple[int, int],  # type: ignore[override]
         focus: bool = False,
     ) -> Canvas:
         from urwid import canvas
 
+        def render_no_scrollbar() -> Canvas:
+            self._original_widget_size = size
+            return ow.render(size, focus)
+
+        def render_for_scrollbar() -> Canvas:
+            self._original_widget_size = ow_size
+            return ow.render(ow_size, focus)
+
         maxcol, maxrow = size
 
-        sb_width = self._scrollbar_width
-        ow_size = (max(0, maxcol - sb_width), maxrow)
+        ow_size = (max(0, maxcol - self._scrollbar_width), maxrow)
         sb_width = maxcol - ow_size[0]
 
         ow = self._original_widget
         ow_base = self.scrolling_base_widget
-        ow_rows_max = ow_base.rows_max(size, focus)
-        if ow_rows_max <= maxrow:
-            # Canvas fits without scrolling - no scrollbar needed
-            self._original_widget_size = size
-            return ow.render(size, focus)
-        ow_rows_max = ow_base.rows_max(ow_size, focus)
 
-        ow_canv = ow.render(ow_size, focus)
-        self._original_widget_size = ow_size
+        if isinstance(ow, SupportsRelativeScroll) and ow.require_relative_scroll(size, focus):
+            if len(ow) == ow.get_visible_amount(size, focus):
+                # Canvas fits without scrolling - no scrollbar needed
+                return render_no_scrollbar()
+
+            ow_canv = render_for_scrollbar()
+            visible_amount = ow.get_visible_amount(ow_size, focus)
+            pos = ow_base.get_first_visible_pos(ow_size, focus)
+            posmax = len(ow) - visible_amount
+            thumb_weight = min(1.0, visible_amount / max(1, len(ow)))
 
-        pos = ow_base.get_scrollpos(ow_size, focus)
-        posmax = ow_rows_max - maxrow
+        else:
+            ow_rows_max = ow_base.rows_max(size, focus)
+            if ow_rows_max <= maxrow:
+                # Canvas fits without scrolling - no scrollbar needed
+                return render_no_scrollbar()
+
+            ow_canv = render_for_scrollbar()
+            ow_rows_max = ow_base.rows_max(ow_size, focus)
+            pos = ow_base.get_scrollpos(ow_size, focus)
+            posmax = ow_rows_max - maxrow
+            thumb_weight = min(1.0, maxrow / max(1, ow_rows_max))
 
-        # Thumb shrinks/grows according to the ratio of
-        # <number of visible lines> / <number of total lines>
-        thumb_weight = min(1.0, maxrow / max(1, ow_rows_max))
+        # Thumb shrinks/grows according to the ratio of <number of visible lines> / <number of total lines>
         thumb_height = max(1, round(thumb_weight * maxrow))
 
         # Thumb may only touch top/bottom if the first/last row is visible
         top_weight = float(pos) / max(1, posmax)
         top_height = int((maxrow - thumb_height) * top_weight)
         if top_height == 0 and top_weight > 0:
             top_height = 1
@@ -560,15 +593,15 @@
     def scrollbar_side(self, side: Literal["left", "right"]) -> None:
         if side not in {SCROLLBAR_LEFT, SCROLLBAR_RIGHT}:
             raise ValueError(f'scrollbar_side must be "left" or "right", not {side!r}')
         self._scrollbar_side = side
         self._invalidate()
 
     @property
-    def scrolling_base_widget(self) -> SupportsScroll:
+    def scrolling_base_widget(self) -> SupportsScroll | SupportsRelativeScroll:
         """Nearest `original_widget` that is compatible with the scrolling API"""
 
         def orig_iter(w: Widget) -> Iterator[Widget]:
             while hasattr(w, "original_widget"):
                 w = w.original_widget
                 yield w
             yield w
```

### Comparing `urwid-2.6.8/urwid/widget/solid_fill.py` & `urwid-2.6.9/urwid/widget/solid_fill.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/text.py` & `urwid-2.6.9/urwid/widget/text.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/treetools.py` & `urwid-2.6.9/urwid/widget/treetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from .text import Text
 from .widget import WidgetWrap
 from .wimp import SelectableIcon
 
 if typing.TYPE_CHECKING:
     from collections.abc import Hashable, Sequence
 
-__all__ = ("TreeWidgetError", "TreeWidget", "TreeNode", "ParentNode", "TreeWalker", "TreeListBox")
+__all__ = ("ParentNode", "TreeListBox", "TreeNode", "TreeWalker", "TreeWidget", "TreeWidgetError")
 
 
 class TreeWidgetError(RuntimeError):
     pass
 
 
 class TreeWidget(WidgetWrap[Padding[typing.Union[Text, Columns]]]):
@@ -81,15 +81,15 @@
         indent_cols = self.get_indent_cols()
         return Padding(widget, width=(WHSettings.RELATIVE, 100), left=indent_cols)
 
     def update_expanded_icon(self) -> None:
         """Update display widget text for parent widgets"""
         # icon is first element in columns indented widget
         icon = [self.unexpanded_icon, self.expanded_icon][self.expanded]
-        self._w.original_widget.contents[0] = (icon, (WHSettings.GIVEN, 1, False))
+        self._w.base_widget.contents[0] = (icon, (WHSettings.GIVEN, 1, False))
 
     def get_indent_cols(self) -> int:
         return self.indent_cols * self.get_node().get_depth()
 
     def get_inner_widget(self) -> Text:
         if self._innerwidget is None:
             self._innerwidget = self.load_inner_widget()
@@ -492,16 +492,16 @@
         parentpos = pos.get_parent()
 
         if parentpos is None:
             return
 
         middle, top, _bottom = self.calculate_visible(size)
 
-        row_offset, _focus_widget, _focus_pos, _focus_rows, _cursor = middle
-        _trim_top, fill_above = top
+        row_offset, _focus_widget, _focus_pos, _focus_rows, _cursor = middle  # pylint: disable=unpacking-non-sequence
+        _trim_top, fill_above = top  # pylint: disable=unpacking-non-sequence
 
         for _widget, pos, rows in fill_above:
             row_offset -= rows
             if pos == parentpos:
                 self.change_focus(size, pos, row_offset)
                 return
```

### Comparing `urwid-2.6.8/urwid/widget/widget.py` & `urwid-2.6.9/urwid/widget/widget.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/widget_decoration.py` & `urwid-2.6.9/urwid/widget/widget_decoration.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/widget/wimp.py` & `urwid-2.6.9/urwid/widget/wimp.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid/wimp.py` & `urwid-2.6.9/urwid/wimp.py`

 * *Files identical despite different names*

### Comparing `urwid-2.6.8/urwid.egg-info/PKG-INFO` & `urwid-2.6.9/urwid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urwid
-Version: 2.6.8
+Version: 2.6.9
 Summary: A full-featured console (xterm et al.) user interface library
 Home-page: https://urwid.org/
 Author-email: Ian Ward <ian@excess.org>
 License: LGPL-2.1-only
 Project-URL: Homepage, https://urwid.org/
 Project-URL: Documentation, https://urwid.org/manual/index.html
 Project-URL: Repository, https://github.com/urwid/urwid
```

### Comparing `urwid-2.6.8/urwid.egg-info/SOURCES.txt` & `urwid-2.6.9/urwid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

