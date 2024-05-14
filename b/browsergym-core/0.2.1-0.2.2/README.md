# Comparing `tmp/browsergym_core-0.2.1.tar.gz` & `tmp/browsergym_core-0.2.2.tar.gz`

## Comparing `browsergym_core-0.2.1.tar` & `browsergym_core-0.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/constants.py
--rw-r--r--   0        0        0    21281 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/env.py
--rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/observation.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/registration.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/spaces.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/__init__.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/base.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/functions.py
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/highlevel.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/parsers.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/python.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/action/utils.py
--rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/chat_files/assistant.png
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/chat_files/chatbox.html
--rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/chat_files/chatbox_modern.html
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/chat_files/img/send.svg
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/javascript/frame_mark_elements.js
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/core/javascript/frame_unmark_elements.js
--rw-r--r--   0        0        0    18053 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/src/browsergym/utils/obs.py
--rw-r--r--   0        0        0    39100 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/test_actions_highlevel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/test_actions_python.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/test_gym_envs.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/test_observation.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/utils.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/example.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/hover.html
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/long_page.html
--rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/screenshot.png
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/test_page.html
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/test_page_2.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/textbox.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/button_input.html
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/checkbox_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/color_picker_input.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/date_input.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/date_min_max_input.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/date_time_local_input.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/email_input.html
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/file_input.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/hidden_field_input.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/image_input.html
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/img_submit.gif
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/number_input.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/number_step_input.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/password_input.html
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/radio_input.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/range_input.html
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/reset_input.html
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/search_input.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/submit_input.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/submit_nn_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/telephone_input.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/text_input.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/time_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/url_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/tests/data/input_type/week_input.html
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/.gitignore
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/constants.py
+-rw-r--r--   0        0        0    21281 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/env.py
+-rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/observation.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/registration.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/spaces.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/base.py
+-rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/functions.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/highlevel.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/parsers.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/python.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/action/utils.py
+-rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/chat_files/assistant.png
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/chat_files/chatbox.html
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/chat_files/chatbox_modern.html
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/chat_files/img/send.svg
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/javascript/frame_mark_elements.js
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/core/javascript/frame_unmark_elements.js
+-rw-r--r--   0        0        0    18053 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/src/browsergym/utils/obs.py
+-rw-r--r--   0        0        0    39837 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/test_actions_highlevel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/test_actions_python.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/test_gym_envs.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/test_observation.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/utils.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/example.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/hover.html
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/long_page.html
+-rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/screenshot.png
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/test_page.html
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/test_page_2.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/textbox.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/button_input.html
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/checkbox_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/color_picker_input.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/date_input.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/date_min_max_input.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/date_time_local_input.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/email_input.html
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/file_input.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/hidden_field_input.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/image_input.html
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/img_submit.gif
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/number_input.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/number_step_input.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/password_input.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/radio_input.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/range_input.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/reset_input.html
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/search_input.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/submit_input.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/submit_nn_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/telephone_input.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/text_input.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/time_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/url_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/tests/data/input_type/week_input.html
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/.gitignore
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.2.2/PKG-INFO
```

### Comparing `browsergym_core-0.2.1/src/browsergym/core/__init__.py` & `browsergym_core-0.2.2/src/browsergym/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 import playwright.sync_api
 
 # we use a global playwright instance
 _PLAYWRIGHT = None
```

### Comparing `browsergym_core-0.2.1/src/browsergym/core/chat.py` & `browsergym_core-0.2.2/src/browsergym/core/chat.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/env.py` & `browsergym_core-0.2.2/src/browsergym/core/env.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/observation.py` & `browsergym_core-0.2.2/src/browsergym/core/observation.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/registration.py` & `browsergym_core-0.2.2/src/browsergym/core/registration.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/spaces.py` & `browsergym_core-0.2.2/src/browsergym/core/spaces.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/task.py` & `browsergym_core-0.2.2/src/browsergym/core/task.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/base.py` & `browsergym_core-0.2.2/src/browsergym/core/action/base.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/functions.py` & `browsergym_core-0.2.2/src/browsergym/core/action/functions.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/highlevel.py` & `browsergym_core-0.2.2/src/browsergym/core/action/highlevel.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/parsers.py` & `browsergym_core-0.2.2/src/browsergym/core/action/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 import ast
 import pyparsing as pp
 
+from dataclasses import dataclass
+from typing import Any
+
+
+@dataclass
+class NamedArgument:
+    name: str
+    value: Any
+
+    def __repr__(self):
+        return f"{self.name}={repr(self.value)}"
+
 
 def _build_highlevel_action_parser() -> pp.ParserElement:
     """
     Returns:
         An action parser that accepts Python-like function calls with string, number, list or dict literals as arguments.
         Example:
             func("a", 42, None, True, [2, 4, "s"], {"a_key": "a_value"}, )
@@ -34,26 +46,32 @@
     def literal_eval(toks):
         return ast.literal_eval(toks[0])
 
     string = pp.python_quoted_string().set_parse_action(literal_eval)
     number = pp.pyparsing_common.number()
     dict = pp.Forward().set_name("dict")  # will be defined later
     list = pp.Forward().set_name("list")  # will be defined later
-    element = (string | number | dict | list | TRUE | FALSE | NONE).set_name("element")
+    _tuple = pp.Forward().set_name("tuple")  # will be defined later
+    element = (string | number | dict | list | _tuple | TRUE | FALSE | NONE).set_name("element")
 
     list_items = pp.DelimitedList(element, allow_trailing_delim=True).set_name(None)
     list << pp.Group(LBRACK + pp.Optional(list_items) + RBRACK, aslist=True)
+    _tuple << pp.Group(LPAREN + pp.Optional(list_items) + RPAREN, aslist=True).set_parse_action(
+        lambda tokens: tuple(tokens[0])
+    )
 
     dict_item = pp.Group(string + COLON + element, aslist=True).set_name("dict item")
     dict_items = pp.DelimitedList(dict_item, allow_trailing_delim=True).set_name(None)
     dict << pp.Dict(LBRACE + pp.Optional(dict_items) + RBRACE, asdict=True)
 
     arg = element
     list_args = pp.DelimitedList(arg, allow_trailing_delim=True).set_name(None)
-    named_arg = (pp.pyparsing_common.identifier() + pp.Literal("=")).suppress() + element
+    named_arg = (pp.pyparsing_common.identifier() + pp.Literal("=") + element).set_parse_action(
+        lambda tokens: NamedArgument(name=tokens[0], value=tokens[2])
+    )
     list_named_args = pp.DelimitedList(named_arg, allow_trailing_delim=True).set_name(None)
     function_call = pp.pyparsing_common.identifier() + pp.Group(
         LPAREN + pp.Optional(list_args) + pp.Optional(list_named_args) + RPAREN, aslist=True
     )
 
     multiple_function_calls = pp.DelimitedList(pp.Group(function_call), delim="")
     multiple_function_calls.ignore(pp.python_style_comment())
```

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/python.py` & `browsergym_core-0.2.2/src/browsergym/core/action/python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/action/utils.py` & `browsergym_core-0.2.2/src/browsergym/core/action/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/chat_files/assistant.png` & `browsergym_core-0.2.2/src/browsergym/core/chat_files/assistant.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/chat_files/chatbox.html` & `browsergym_core-0.2.2/src/browsergym/core/chat_files/chatbox.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/chat_files/chatbox_modern.html` & `browsergym_core-0.2.2/src/browsergym/core/chat_files/chatbox_modern.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/chat_files/img/send.svg` & `browsergym_core-0.2.2/src/browsergym/core/chat_files/img/send.svg`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/javascript/frame_mark_elements.js` & `browsergym_core-0.2.2/src/browsergym/core/javascript/frame_mark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/core/javascript/frame_unmark_elements.js` & `browsergym_core-0.2.2/src/browsergym/core/javascript/frame_unmark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/src/browsergym/utils/obs.py` & `browsergym_core-0.2.2/src/browsergym/utils/obs.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/test_actions_highlevel.py` & `browsergym_core-0.2.2/tests/test_actions_highlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import browsergym.core
 
 # bugfix: use same playwright instance in browsergym and pytest
 from utils import setup_playwright
 
 from browsergym.utils.obs import flatten_dom_to_str
 from browsergym.core.action.highlevel import HighLevelActionSet
-from browsergym.core.action.parsers import highlevel_action_parser
+from browsergym.core.action.parsers import highlevel_action_parser, NamedArgument
 from browsergym.core.constants import BROWSERGYM_ID_ATTRIBUTE as BID_ATTR
 
 
 _IS_MAC_OS = platform.system() == "Darwin"
 
 __SLOW_MO = 1000 if "DISPLAY_BROWSER" in os.environ else None
 __HEADLESS = False if "DISPLAY_BROWSER" in os.environ else True
@@ -52,30 +52,41 @@
 
     function_calls = parser.parse_string("  a ( ) \n\n\t", parseAll=True)
     assert len(function_calls) == 1
 
     function_calls = parser.parse_string("  a ( ) b() \n \tc()", parseAll=True)
     assert [function_name for function_name, _ in function_calls] == ["a", "b", "c"]
 
-    function_calls = parser.parse_string('a(12, 12.2, "text")', parseAll=True)
+    function_calls = parser.parse_string('a(12, 12.2, "text", (1, 2, 3), ["a", 23])', parseAll=True)
     _, function_args = function_calls[0]
-    assert function_args == [12, 12.2, "text"]
+    assert function_args == [12, 12.2, "text", (1, 2, 3), ["a", 23]]
 
     function_calls = parser.parse_string('a(x=12, y = 12.2, other = "text")', parseAll=True)
     _, function_args = function_calls[0]
-    assert function_args == [12, 12.2, "text"]
+    assert function_args == [
+        NamedArgument(name="x", value=12),
+        NamedArgument(name="y", value=12.2),
+        NamedArgument(name="other", value="text"),
+    ]
 
     function_calls = parser.parse_string('a(12, y = 12.2, other = "text")', parseAll=True)
     _, function_args = function_calls[0]
-    assert function_args == [12, 12.2, "text"]
+    assert function_args == [
+        12,
+        NamedArgument(name="y", value=12.2),
+        NamedArgument(name="other", value="text"),
+    ]
 
     with pytest.raises(ParseException):
         function_calls = parser.parse_string('a(x = 12, 12.2, other = "text")', parseAll=True)
 
     with pytest.raises(ParseException):
+        function_calls = parser.parse_string('a(12, 12.2, 1 = "text")', parseAll=True)
+
+    with pytest.raises(ParseException):
         function_calls = parser.parse_string("a(1-)", parseAll=True)
 
     with pytest.raises(ParseException):
         function_calls = parser.parse_string("a(1/2)", parseAll=True)
 
     function_calls = parser.parse_string('a("""\nsome\ntext\\"\\"""")', parseAll=True)
     _, function_args = function_calls[0]
@@ -87,14 +98,23 @@
 
     function_calls = parser.parse_string('#comment\na("# not comment") #comment \n ', parseAll=True)
     assert len(function_calls) == 1
     function_name, function_args = function_calls[0]
     assert function_name == "a"
     assert function_args == ["# not comment"]
 
+    function_calls = parser.parse_string('fun(12, x="val", y={"aaa": 23})', parseAll=True)
+    function_name, function_args = function_calls[0]
+    assert function_name == "fun"
+    assert function_args == [
+        12,
+        NamedArgument(name="x", value="val"),
+        NamedArgument(name="y", value={"aaa": 23}),
+    ]
+
 
 def test_valid_action():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
         task_kwargs={"start_url": CHECKBOX_URL},
```

### Comparing `browsergym_core-0.2.1/tests/test_actions_python.py` & `browsergym_core-0.2.2/tests/test_actions_python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/test_gym_envs.py` & `browsergym_core-0.2.2/tests/test_gym_envs.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/test_observation.py` & `browsergym_core-0.2.2/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/utils.py` & `browsergym_core-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/example.html` & `browsergym_core-0.2.2/tests/data/example.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/long_page.html` & `browsergym_core-0.2.2/tests/data/long_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/screenshot.png` & `browsergym_core-0.2.2/tests/data/screenshot.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/test_page.html` & `browsergym_core-0.2.2/tests/data/test_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/test_page_2.html` & `browsergym_core-0.2.2/tests/data/test_page_2.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_iframe_site/basic_iframe.html` & `browsergym_core-0.2.2/tests/data/basic_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_iframe_site/inner-iframe.html` & `browsergym_core-0.2.2/tests/data/basic_iframe_site/inner-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_iframe_site/outer-iframe.html` & `browsergym_core-0.2.2/tests/data/basic_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_shadow_dom_site/basic_shadow_dom.html` & `browsergym_core-0.2.2/tests/data/basic_shadow_dom_site/basic_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_shadow_dom_site/simple_shadow_dom.html` & `browsergym_core-0.2.2/tests/data/basic_shadow_dom_site/simple_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/basic_iframe.html` & `browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/basic_shadow_iframe_site/outer-iframe.html` & `browsergym_core-0.2.2/tests/data/basic_shadow_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/checkbox_input.html` & `browsergym_core-0.2.2/tests/data/input_type/checkbox_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/color_picker_input.html` & `browsergym_core-0.2.2/tests/data/input_type/color_picker_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/date_min_max_input.html` & `browsergym_core-0.2.2/tests/data/input_type/date_min_max_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/date_time_local_input.html` & `browsergym_core-0.2.2/tests/data/input_type/date_time_local_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/image_input.html` & `browsergym_core-0.2.2/tests/data/input_type/image_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/img_submit.gif` & `browsergym_core-0.2.2/tests/data/input_type/img_submit.gif`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/password_input.html` & `browsergym_core-0.2.2/tests/data/input_type/password_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/reset_input.html` & `browsergym_core-0.2.2/tests/data/input_type/reset_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/submit_input.html` & `browsergym_core-0.2.2/tests/data/input_type/submit_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/telephone_input.html` & `browsergym_core-0.2.2/tests/data/input_type/telephone_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/text_input.html` & `browsergym_core-0.2.2/tests/data/input_type/text_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/tests/data/input_type/time_input.html` & `browsergym_core-0.2.2/tests/data/input_type/time_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/pyproject.toml` & `browsergym_core-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.2.1/PKG-INFO` & `browsergym_core-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: browsergym-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

