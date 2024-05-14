# Comparing `tmp/youqu-2.5.5.tar.gz` & `tmp/youqu-2.6.0.tar.gz`

## Comparing `youqu-2.5.5.tar` & `youqu-2.6.0.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/CURRENT
--rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/conftest.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/env.sh
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/manage.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/ruff.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/__init__.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/_env_base.sh
--rwxr-xr-x   0        0        0     3272 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/env_dev.sh
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/env_vir.sh
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/playbook.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/subcmd.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/__init__.py
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/calculate.py
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/desktop.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/filectl.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/filter_image.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/mouse_key.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/read_csv.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/read_toml.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/requestx.py
--rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/singleton.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/startapp.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/webui.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/_cargo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/check.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/mng.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/_cargo.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_base.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_remote_dogtail_ctl.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_remote_other_ctl.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/_cargo.py
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/playbook.py
--rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/command_complete.sh
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/docs_env.sh
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/pylint.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_remote.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.5/pyproject.toml
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/README.md
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 youqu-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/CURRENT
+-rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/conftest.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/env.sh
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/manage.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/pytest.ini
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/ruff.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/__init__.py
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/playbook.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/subcmd.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/calculate.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/filter_image.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/read_csv.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/read_toml.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/singleton.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/_cargo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/mng.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/_cargo.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/_cargo.py
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/playbook.py
+-rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/_env_base.sh
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/command_complete.sh
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/docs_env.sh
+-rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/env_dev.sh
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/env_vir.sh
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/opencv_rpc_server.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/pylint.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/vnc.sh
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/README.md
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 youqu-2.6.0/PKG-INFO
```

### Comparing `youqu-2.5.5/youqu/conftest.py` & `youqu-2.6.0/youqu/conftest.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/env.sh` & `youqu-2.6.0/youqu/env.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
-
+export PIPENV_VERBOSITY=-1
 ROOT_DIR=$(dirname $(realpath "${BASH_SOURCE[0]}"))
 tag=$(echo "$(cat ${ROOT_DIR}/CURRENT | grep "tag = ")" | cut -d "=" -f2 | python3 -c "s=input();print(s.strip())")
 config_pwd=$(cat ${ROOT_DIR}/setting/globalconfig.ini | grep -v "CLIENT_PASSWORD" | grep "PASSWORD = ")
 PASSWORD=$(echo "${config_pwd}" | cut -d "=" -f2 | python3 -c "s=input();print(s.strip())")
 DEV=false
 while getopts ":p:D" opt
 do
@@ -32,22 +32,26 @@
     debian_platform=true
     yq=apt
 else
     yq=yum
 fi
 
 DISPLAY_SERVER=$(cat ${HOME}/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1 | cut -d "=" -f2)
+if [ "${DISPLAY_SERVER}" = "" ]; then
+    ps -ef | grep -v grep | grep kwin_x11
+    [ $? = 0 ] && DISPLAY_SERVER=x11 || DISPLAY_SERVER=wayland
+fi
 PYTHON_VERSION=$(python3 -c "import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')")
 whitelist="/usr/share/deepin-elf-verify/whitelist"
 pypi_mirror="https://pypi.tuna.tsinghua.edu.cn/simple"
 
 echo "${PASSWORD}" | sudo -S su
 
 if [ ! -f "$HOME/.Xauthority" ]; then
         touch $HOME/.Xauthority
 fi
 
 if [ "${DEV}" = "true" ]; then
-    source ./setting/env_dev.sh
+    source ./src/utils/env_dev.sh
 else
-    source ./setting/env_vir.sh
+    source ./src/utils/env_vir.sh
 fi
```

### Comparing `youqu-2.5.5/youqu/manage.py` & `youqu-2.6.0/youqu/manage.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/ruff.toml` & `youqu-2.6.0/youqu/ruff.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/startproject.py` & `youqu-2.6.0/youqu/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/_env_base.sh` & `youqu-2.6.0/youqu/src/utils/_env_base.sh`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     sudo pip3 install -U pip > /tmp/env.log 2>&1
     sudo pip3 cache purge > /tmp/env.log 2>&1
     sudo pip3 config set global.timeout 10000 > /tmp/env.log 2>&1
 }
 
 install_py_deb(){
     rm -rf ${1}*
-    apt download ${1} > /tmp/env.log 2>&1
+    ${yq} download ${1} > /tmp/env.log 2>&1
     if [ $? != 0 ]; then
         cat /tmp/env.log
         exit 120
     fi
     dpkg -x ${1}*.deb ${1}
     cp -r ./${1}/usr/lib/python3/dist-packages/* ${2}/lib/python${PYTHON_VERSION}/site-packages/
     rm -rf ${1}*
```

### Comparing `youqu-2.5.5/youqu/setting/env_dev.sh` & `youqu-2.6.0/youqu/src/utils/env_dev.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
-source ${ROOT_DIR}/setting/_env_base.sh
+source ${ROOT_DIR}/src/utils/_env_base.sh
 
 env(){
 
     if [ "${debian_platform}" = "true" ]; then
         sudo apt update
     fi
```

### Comparing `youqu-2.5.5/youqu/setting/env_vir.sh` & `youqu-2.6.0/youqu/src/utils/env_vir.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 #!/bin/bash
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
-source ${ROOT_DIR}/setting/_env_base.sh
+source ${ROOT_DIR}/src/utils/_env_base.sh
 echo "
  ██╗   ██╗  ██████╗      ███████╗ ███╗   ██╗ ██╗   ██╗
  ╚██╗ ██╔╝ ██╔═══██╗     ██╔════╝ ████╗  ██║ ██║   ██║
   ╚████╔╝  ██║   ██║     █████╗   ██╔██╗ ██║ ██║   ██║
    ╚██╔╝   ██║▄▄ ██║     ██╔══╝   ██║╚██╗██║ ╚██╗ ██╔╝
     ██║    ╚██████╔╝     ███████╗ ██║ ╚████║  ╚████╔╝
     ╚═╝     ╚══▀▀═╝      ╚══════╝ ╚═╝  ╚═══╝   ╚═══╝
     ${tag}
 "
 
 env(){
-    sudo apt update
+    if [ "${debian_platform}" = "true" ]; then
+        sudo apt update
+    fi
 
     deb_array=(
         python3-pip
         python3-tk
         sshpass
         scrot
-        openjdk-8-jdk
+        openjdk-11-jdk-headless
         gir1.2-atspi-2.0
         libatk-adaptor
         at-spi2-core
         python3-opencv
     )
     cd ${ROOT_DIR}/src/utils
     BASICENV=$(python3 sub_env_cut.py)
     if [ "${BASICENV}" = "BASICENV" ]; then
         ENV_CUT_FLAG="cut"
         deb_array=(
             python3-pip
             sshpass
-            openjdk-8-jdk
+            openjdk-11-jdk-headless
         )
     fi
 
+    if [ "${debian_platform}" = "false" ]; then
+        deb_array[${#deb_array[@]}]=java-11-openjdk-headless
+        deb_array[${#deb_array[@]}]=python3-tkinter
+        deb_array[${#deb_array[@]}]=xdotool
+        deb_array[${#deb_array[@]}]=opencv
+    fi
+
     for deb in ${deb_array[*]}
     do
-        sudo apt install -y ${deb} > /tmp/env.log 2>&1
+        sudo ${yq} install -y ${deb} > /tmp/env.log 2>&1
         check_status ${deb}
     done
 
     if [ "${DISPLAY_SERVER}" = "wayland" ]; then
         wayland_env
     fi
 }
@@ -65,19 +74,21 @@
 pipenv --python ${PYTHON_VERSION} > /tmp/env.log 2>&1
 if [ $? != 0 ]; then
     echo -e "AT环境创建失败"
     exit 121
 fi
 python_virtualenv_path=$(pipenv --venv)
 whitelist_path=`echo "${python_virtualenv_path}" | sed "s/\/home\/$USER\//\//"`
-result=`sudo cat ${whitelist} | grep ${whitelist_path}`
-if [ -z "$result" ]; then
-    sudo sed -i '$a\'"${whitelist_path}"'' ${whitelist}
-    sudo sed -i '$a\'"${python_virtualenv_path}"'' ${whitelist}
-    sudo systemctl restart deepin-elf-verify.service || true
+if [ -f "${whitelist}" ]; then
+    result=`sudo cat ${whitelist} | grep ${whitelist_path}`
+    if [ -z "$result" ]; then
+        sudo sed -i '$a\'"${whitelist_path}"'' ${whitelist}
+        sudo sed -i '$a\'"${python_virtualenv_path}"'' ${whitelist}
+        sudo systemctl restart deepin-elf-verify.service || true
+    fi
 fi
 
 py_debs=(
     python3-gi
     python3-pyatspi
     python3-dbus
     python3-cairo
@@ -88,15 +99,15 @@
     python3-opencv
 )
 for pd in ${py_debs[*]}
 do
     install_py_deb ${pd} ${python_virtualenv_path}
 done
 
-apt download python3-gi-cairo > /tmp/env.log 2>&1
+${yq} download python3-gi-cairo > /tmp/env.log 2>&1
 dpkg -x python3-gi-cairo*.deb python3-gi-cairo
 cp -r ./python3-gi-cairo/usr/lib/python3/dist-packages/gi/* ${python_virtualenv_path}/lib/python${PYTHON_VERSION}/site-packages/gi/
 rm -rf python3-gi-cairo*
 
 cd ${ROOT_DIR}/src/utils/
 sub_py_debs=$(python3 sub_deb.py)
 for spd in ${sub_py_debs[*]}
```

### Comparing `youqu-2.5.5/youqu/setting/globalconfig.ini` & `youqu-2.6.0/youqu/setting/globalconfig.ini`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ;单条用例的超时时间，如果一条用例的执行时间超时，这条用例会被停止，后续用例继续执行。
 ;单位为秒
 ;这是一个全局统一配置，如果某条用例需要单独配置超时时间，可以在用例中这样写：
 ;@pytest.mark.timeout(500)
 ;def test_xxx_001():
 ;    ...
 ;会话超时（所有用例执行的超时时间）是根据全局超时配置和用例单独超时配置自动计算的。
-CASE_TIME_OUT = 200
+CASE_TIME_OUT = 300
 
 ;失败用例重跑次数
 ;注意，RERUN = 1 表示重跑 1 次，即第一次用例执行失败会自动重跑 1 次，总共执行 2 次；
 ;如果第 2 次执行成功，结果成功，失败亦为失败。
 RERUN = 1
 
 ;失败录屏从第几次失败开始录制视频。
@@ -105,15 +105,15 @@
 TMPDIR = /tmp/tmpdir
 
 ;系统主题
 SYS_THEME = deepin
 
 ;=============================== OCR CONFIG ===================================
 ;OCR服务端地址
-OCR_SERVER_HOST = youqu.uniontech.com
+OCR_SERVER_HOST = 10.8.13.7/10.8.13.66/10.8.13.55/10.8.13.100
 
 ;OCR端口
 OCR_PORT = 8890
 
 ;网络重试次数
 OCR_NETWORK_RETRY = 1
```

### Comparing `youqu-2.5.5/youqu/setting/globalconfig.py` & `youqu-2.6.0/youqu/setting/globalconfig.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/playbook.toml` & `youqu-2.6.0/youqu/setting/playbook.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/pylintrc.cfg` & `youqu-2.6.0/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/skipif.py` & `youqu-2.6.0/youqu/setting/skipif.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.6.0/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.6.0/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.6.0/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/__init__.py` & `youqu-2.6.0/youqu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/assert_common.py` & `youqu-2.6.0/youqu/src/assert_common.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/button_center.py` & `youqu-2.6.0/youqu/src/button_center.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/calculate.py` & `youqu-2.6.0/youqu/src/calculate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/cmdctl.py` & `youqu-2.6.0/youqu/src/cmdctl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
+import os
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 import subprocess
-import os
 
-from src.custom_exception import ShellExecutionFailed
-from src import logger
 from setting import conf
+from src import logger
+from src.custom_exception import ShellExecutionFailed
 
 
 class CmdCtl:
     """命令行工具"""
 
     # pylint: disable=too-many-arguments,too-many-locals,too-many-public-methods
     # clean_env也要用
@@ -67,21 +67,21 @@
             exitcode = -1
         if data[-1:] == "\n":
             data = data[:-1]
         return exitcode, data
 
     @classmethod
     def sudo_run_cmd(
-        cls,
-        command,
-        interrupt=False,
-        timeout=25,
-        out_debug_flag=True,
-        command_log=True,
-        password=None,
+            cls,
+            command,
+            interrupt=False,
+            timeout=25,
+            out_debug_flag=True,
+            command_log=True,
+            password=None,
     ):
         if password is None:
             password = conf.PASSWORD
         return cls.run_cmd(
             f"echo '{password}' | sudo -S {command}",
             interrupt=interrupt,
             timeout=timeout,
@@ -248,7 +248,18 @@
         # 杀进程要过滤的进程
         if grep_list:
             cls.GREP_LIST = grep_list
         cmd = ""
         for i in cls.GREP_LIST:
             cmd += f"grep -v {i} | "
         os.system(f"ps -ef | grep {process} | {cmd}cut -c 9-15 | xargs kill -9 > /dev/null 2>&1")
+
+    @classmethod
+    def sudo_kill_process(cls, process, grep_list: [list, tuple] = None):
+        if grep_list:
+            cls.GREP_LIST = grep_list
+        cmd = ""
+        for i in cls.GREP_LIST:
+            cmd += f"grep -v {i} | "
+        os.system(
+            f"process=$(ps -ef | grep {process} | {cmd}cut -c 9-15);echo '1' | sudo -S kill -9 $process > /dev/null 2>&1"
+        )
```

### Comparing `youqu-2.5.5/youqu/src/csvctl.py` & `youqu-2.6.0/youqu/src/csvctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/custom_exception.py` & `youqu-2.6.0/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/dbus_utils.py` & `youqu-2.6.0/youqu/src/dbus_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/desktop.py` & `youqu-2.6.0/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/dogtail_utils.py` & `youqu-2.6.0/youqu/src/dogtail_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/filectl.py` & `youqu-2.6.0/youqu/src/filectl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/filter_image.py` & `youqu-2.6.0/youqu/src/filter_image.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/mouse_key.py` & `youqu-2.6.0/youqu/src/mouse_key.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pinyin.py` & `youqu-2.6.0/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/read_csv.py` & `youqu-2.6.0/youqu/src/read_csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/recording_screen.py` & `youqu-2.6.0/youqu/src/recording_screen.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/requestx.py` & `youqu-2.6.0/youqu/src/requestx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/shortcut.py` & `youqu-2.6.0/youqu/src/shortcut.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,22 @@
         """
          ctrl_a
         :return:
         """
         cls.hot_key("ctrl", "a")
 
     @classmethod
+    def ctrl_l(cls):
+        """
+         ctrl_l
+        :return:
+        """
+        cls.hot_key("ctrl", "l")
+
+    @classmethod
     def ctrl_g(cls):
         """
          ctrl_g
         :return:
         """
         cls.hot_key("ctrl", "g")
```

### Comparing `youqu-2.5.5/youqu/src/singleton.py` & `youqu-2.6.0/youqu/src/singleton.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/sleepx.py` & `youqu-2.6.0/youqu/src/sleepx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/startapp.py` & `youqu-2.6.0/youqu/src/startapp.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/startproject.py` & `youqu-2.6.0/youqu/src/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/video_utils.py` & `youqu-2.6.0/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/wayland_wininfo.py` & `youqu-2.6.0/youqu/src/wayland_wininfo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/webui.py` & `youqu-2.6.0/youqu/src/webui.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/ydotool.py` & `youqu-2.6.0/youqu/src/ydotool.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/cli.py` & `youqu-2.6.0/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/colors.py` & `youqu-2.6.0/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/consts.py` & `youqu-2.6.0/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/core.py` & `youqu-2.6.0/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.6.0/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/colorama/ansi.py` & `youqu-2.6.0/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.6.0/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/colorama/initialise.py` & `youqu-2.6.0/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/colorama/win32.py` & `youqu-2.6.0/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/colorama/winterm.py` & `youqu-2.6.0/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/COPYING` & `youqu-2.6.0/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/__init__.py` & `youqu-2.6.0/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/config.py` & `youqu-2.6.0/youqu/src/depends/dogtail/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,16 +230,21 @@
     def reset(self):
         """
         Resets all settings to their defaults.
         """
         _Config.options = {}
 
         # 显示服务器
-    DISPLAY_SERVER = os.popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1").read().split("=")[
-        -1].strip("\n")
+
+    DISPLAY_SERVER = (
+                         os.popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
+                             .read()
+                             .split("=")[-1]
+                             .strip("\n")
+                     ) or ("x11" if os.popen("ps -ef | grep -v grep | grep kwin_x11").read() else "wayland")
 
     class DisplayServer:
         wayland = "wayland"
         x11 = "x11"
 
     IS_X11 = (DISPLAY_SERVER == DisplayServer.x11)
     IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland)
```

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/distro.py` & `youqu-2.6.0/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/dump.py` & `youqu-2.6.0/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/errors.py` & `youqu-2.6.0/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/i18n.py` & `youqu-2.6.0/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/logging.py` & `youqu-2.6.0/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/path.py` & `youqu-2.6.0/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/predicate.py` & `youqu-2.6.0/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/procedural.py` & `youqu-2.6.0/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.6.0/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.6.0/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/sessions.py` & `youqu-2.6.0/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/tc.py` & `youqu-2.6.0/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/tree.py` & `youqu-2.6.0/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/utils.py` & `youqu-2.6.0/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/version.py` & `youqu-2.6.0/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.6.0/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.6.0/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.6.0/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.6.0/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.6.0/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.6.0/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/sniff` & `youqu-2.6.0/youqu/src/depends/sniff/sniff`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/sniff.ui` & `youqu-2.6.0/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.6.0/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.6.0/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.6.0/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.6.0/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/LICENSE` & `youqu-2.6.0/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/git/_cargo.py` & `youqu-2.6.0/youqu/src/git/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/git/clone.py` & `youqu-2.6.0/youqu/src/git/clone.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/git/code_statistics.py` & `youqu-2.6.0/youqu/src/git/code_statistics.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/git/commit.py` & `youqu-2.6.0/youqu/src/git/commit.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/plugins/allure_report_extend.py` & `youqu-2.6.0/youqu/src/plugins/allure_report_extend.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/plugins/emoji_hooks.py` & `youqu-2.6.0/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/plugins/mng.py` & `youqu-2.6.0/youqu/src/plugins/mng.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/_base.py` & `youqu-2.6.0/youqu/src/pms/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/_cargo.py` & `youqu-2.6.0/youqu/src/pms/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/csv2pms.py` & `youqu-2.6.0/youqu/src/pms/csv2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/pms2csv.py` & `youqu-2.6.0/youqu/src/pms/pms2csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/send2pms.py` & `youqu-2.6.0/youqu/src/pms/send2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/suite.py` & `youqu-2.6.0/youqu/src/pms/suite.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/pms/task.py` & `youqu-2.6.0/youqu/src/pms/task.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/remotectl/_base.py` & `youqu-2.6.0/youqu/src/remotectl/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,18 @@
 
 def remote_client(ip, port):
     try:
         import zerorpc
     except ImportError:
         raise ImportError("Please install zerorpc")
 
-    r = zerorpc.Client(timeout=50, heartbeat=None)
+    c = zerorpc.Client(timeout=50, heartbeat=None)
     try:
-        r.connect(f"tcp://{ip}:{port}")
-        return r
+        c.connect(f"tcp://{ip}:{port}")
+        return c
     except Exception as e:
         raise e
 
 
 def remote_server(obj, port):
     try:
         import zerorpc
@@ -167,7 +167,11 @@
 
 def _remote_server(obj, port):
     server = ThreadXMLRPCServer(("0.0.0.0", port), allow_none=True)
     for func, _ in inspect.getmembers(obj):
         if not func.startswith("_"):
             server.register_function(getattr(obj, func), func)
     server.serve_forever()
+
+if __name__ == '__main__':
+    from src import Src
+    _remote_server(Src(), 4242)
```

### Comparing `youqu-2.5.5/youqu/src/remotectl/_remote_dogtail_ctl.py` & `youqu-2.6.0/youqu/src/remotectl/_remote_dogtail_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/remotectl/_remote_other_ctl.py` & `youqu-2.6.0/youqu/src/remotectl/_remote_other_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/remotectl/remote.py` & `youqu-2.6.0/youqu/src/remotectl/remote.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/rtk/_base.py` & `youqu-2.6.0/youqu/src/rtk/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 def collect_result(results):
     res = Counter([results.get(i).get("result") for i in results])
     total = sum(res.values())
     skiped = res.get("skip", 0)
     passed = res.get("pass", 0)
-    failed = total - passed
+    failed = total - skiped - passed
     pass_rate = f"{round((passed / (total - skiped)) * 100, 2)}%" if passed else "0%"
     return total, failed, passed, skiped, pass_rate
 
 
 def get_result(ci_result):
     with open(ci_result, "r", encoding="utf-8") as _f:
         results_dict = json.load(_f)
```

### Comparing `youqu-2.5.5/youqu/src/rtk/_cargo.py` & `youqu-2.6.0/youqu/src/rtk/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/rtk/local_runner.py` & `youqu-2.6.0/youqu/src/rtk/local_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/rtk/playbook.py` & `youqu-2.6.0/youqu/src/rtk/playbook.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/rtk/remote_runner.py` & `youqu-2.6.0/youqu/src/rtk/remote_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/check_python_source.py` & `youqu-2.6.0/youqu/src/utils/check_python_source.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/docs_env.sh` & `youqu-2.6.0/youqu/src/utils/docs_env.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/opencv_rpc_server.py` & `youqu-2.6.0/youqu/src/utils/opencv_rpc_server.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/pylint.sh` & `youqu-2.6.0/youqu/src/utils/pylint.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/sslclone.sh` & `youqu-2.6.0/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/sub_deb.py` & `youqu-2.6.0/youqu/src/utils/sub_deb.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/youqu/src/utils/vnc.sh` & `youqu-2.6.0/youqu/src/utils/vnc.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.5/pyproject.toml` & `youqu-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youqu"
-version = "2.5.5"
+version = "2.6.0"
 authors = [
     { name = "mikigo", email = "huangmingqiang@uniontech.com" },
 ]
 
 description = "youqu"
 readme = "youqu/README.md"
 requires-python = ">=3.7"
```

### Comparing `youqu-2.5.5/youqu/README.md` & `youqu-2.6.0/youqu/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,45 +7,39 @@
     <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
 
 
 
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
-[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
-
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
-![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
-![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
+![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431)
 
-[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
-[![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
-[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
+[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
 <a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
 <a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
 
 ---
 
-YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
+YouQu(有趣)是统信公司(Deepin/UOS)开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
 
 ## YouQu（有趣）能做什么
 
 - [x] 💻 Linux 桌面应用 UI 自动化测试
 - [x] 🌏 Web UI 自动化测试
 - [x] 🚌 Linux DBus 接口自动化测试
 - [x] 🚀 命令行自动化测试
 - [x] 🕷️ HTTP 接口自动化测试
 - [ ] ⏲️ Linux 桌面应用性能自动化测试
+- [ ]    💥 Fuzzy Desktop 桌面模糊测试
 
 ## 安装
 
 从 PyPI 安装:
 
 
 ```shell
@@ -94,15 +88,15 @@
 自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
 在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 my_project
 ├── apps
-│   ├── autotest_deepin_some  # <----- APP 工程
+│   ├── autotest_deepin_some  # <-- APP 工程
 ...     ├── ...
 ```
 
 在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
 
 `autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
```

#### html2text {}

```diff
@@ -1,35 +1,28 @@
                                     _[_Y_o_u_Q_u_]
 YYoouuQQuu?ï?¼??æ???è?¶?£?ï?¼??ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![GitHub
-pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls) [![GitHub
-Discussions](https://img.shields.io/github/discussions/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions) [!
-[PyPI](https://img.shields.io/pypi/v/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![PyPI]
+(https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
-(https://pypi.org/project/youqu/) ![PyPI - License](https://img.shields.io/
-pypi/l/youqu?color=%23F79431) ![PyPI - Python Version](https://img.shields.io/
-pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
-badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
-project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
-(https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
-youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
-linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
-github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --
-- YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
+(https://pypi.org/project/youqu/) ![Static Badge](https://img.shields.io/badge/
+UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431) [!
+[Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/
+youqu) [![Hits](https://hits.sh/github.com/linuxdeepin/
+youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/
+linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --- YouQu
+(æè¶£)æ¯ç»ä¿¡å¬å¸(Deepin/UOS)å¼æºçä¸ä¸ªç¨äº Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æãð¥ ##
 YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] ð» Linux æ¡é¢åºç¨ UI èªå¨åæµè¯
 - [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus æ¥å£èªå¨åæµè¯ -
 [x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP æ¥å£èªå¨åæµè¯ -
-[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ ## å®è£ ä» PyPI å®è£:
-```shell $ sudo pip3 install youqu ``` ä¸å  sudo ?
+[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ - [ ] ð¥ Fuzzy Desktop
+æ¡é¢æ¨¡ç³æµè¯ ## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install
+youqu ``` ä¸å  sudo ?
 å¶å®ä¸å  sudo ä¹æ¯å¯ä»¥çï¼
 
   pip3 install youqu
 
 ä½æäºæåµä¸å¯è½åºç° youqu-startproject
 å½ä»¤æ æ³ä½¿ç¨ï¼è¿æ¯å ä¸ºä¸å  sudo æ¶ï¼å®è£åè·¯å¾æ¯å¨
 $HOME/.local/lib/pythonX.X/site-
@@ -44,16 +37,16 @@
 æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
 å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
 manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
 å·¥ç¨éµå¾ªå®æ´ç PO
 è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
 `apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
 å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell my_project âââ apps â âââ autotest_deepin_some # <----
-- APP å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
+```shell my_project âââ apps â âââ autotest_deepin_some # <-- APP
+å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
 ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
 `autotest_deepin_some` æ¯ä½ ç APP
 å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
 ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
 æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
```

### Comparing `youqu-2.5.5/PKG-INFO` & `youqu-2.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youqu
-Version: 2.5.5
+Version: 2.6.0
 Summary: youqu
 Project-URL: Source, https://github.com/linuxdeepin/youqu
 Project-URL: Documentation, https://linuxdeepin.github.io/youqu
 Author-email: mikigo <huangmingqiang@uniontech.com>
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -20,45 +20,39 @@
     <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
 
 
 
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
-[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
-
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
-![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
-![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
+![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431)
 
-[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
-[![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
-[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
+[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
 <a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
 <a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
 
 ---
 
-YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
+YouQu(有趣)是统信公司(Deepin/UOS)开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
 
 ## YouQu（有趣）能做什么
 
 - [x] 💻 Linux 桌面应用 UI 自动化测试
 - [x] 🌏 Web UI 自动化测试
 - [x] 🚌 Linux DBus 接口自动化测试
 - [x] 🚀 命令行自动化测试
 - [x] 🕷️ HTTP 接口自动化测试
 - [ ] ⏲️ Linux 桌面应用性能自动化测试
+- [ ]    💥 Fuzzy Desktop 桌面模糊测试
 
 ## 安装
 
 从 PyPI 安装:
 
 
 ```shell
@@ -107,15 +101,15 @@
 自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
 在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 my_project
 ├── apps
-│   ├── autotest_deepin_some  # <----- APP 工程
+│   ├── autotest_deepin_some  # <-- APP 工程
 ...     ├── ...
 ```
 
 在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
 
 `autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
```

#### html2text {}

```diff
@@ -1,42 +1,35 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.5.5 Summary: youqu Project-URL:
+Metadata-Version: 2.1 Name: youqu Version: 2.6.0 Summary: youqu Project-URL:
 Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
 //linuxdeepin.github.io/youqu Author-email: mikigo
 uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
 YYoouuQQuu?ï?¼??æ???è?¶?£?ï?¼??ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![GitHub
-pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls) [![GitHub
-Discussions](https://img.shields.io/github/discussions/linuxdeepin/
-youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions) [!
-[PyPI](https://img.shields.io/pypi/v/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![PyPI]
+(https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
-(https://pypi.org/project/youqu/) ![PyPI - License](https://img.shields.io/
-pypi/l/youqu?color=%23F79431) ![PyPI - Python Version](https://img.shields.io/
-pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
-badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
-project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
-(https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
-youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
-linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
-github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --
-- YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
+(https://pypi.org/project/youqu/) ![Static Badge](https://img.shields.io/badge/
+UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431) [!
+[Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/
+youqu) [![Hits](https://hits.sh/github.com/linuxdeepin/
+youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/
+linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --- YouQu
+(æè¶£)æ¯ç»ä¿¡å¬å¸(Deepin/UOS)å¼æºçä¸ä¸ªç¨äº Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æãð¥ ##
 YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] ð» Linux æ¡é¢åºç¨ UI èªå¨åæµè¯
 - [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus æ¥å£èªå¨åæµè¯ -
 [x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP æ¥å£èªå¨åæµè¯ -
-[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ ## å®è£ ä» PyPI å®è£:
-```shell $ sudo pip3 install youqu ``` ä¸å  sudo ?
+[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ - [ ] ð¥ Fuzzy Desktop
+æ¡é¢æ¨¡ç³æµè¯ ## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install
+youqu ``` ä¸å  sudo ?
 å¶å®ä¸å  sudo ä¹æ¯å¯ä»¥çï¼
 
   pip3 install youqu
 
 ä½æäºæåµä¸å¯è½åºç° youqu-startproject
 å½ä»¤æ æ³ä½¿ç¨ï¼è¿æ¯å ä¸ºä¸å  sudo æ¶ï¼å®è£åè·¯å¾æ¯å¨
 $HOME/.local/lib/pythonX.X/site-
@@ -51,16 +44,16 @@
 æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
 å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
 manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
 å·¥ç¨éµå¾ªå®æ´ç PO
 è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
 `apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
 å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell my_project âââ apps â âââ autotest_deepin_some # <----
-- APP å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
+```shell my_project âââ apps â âââ autotest_deepin_some # <-- APP
+å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
 ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
 `autotest_deepin_some` æ¯ä½ ç APP
 å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
 ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
 æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
```

