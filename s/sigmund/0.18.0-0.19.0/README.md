# Comparing `tmp/sigmund-0.18.0.tar.gz` & `tmp/sigmund-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmund-0.18.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigmund-0.19.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigmund-0.18.0.tar` & `sigmund-0.19.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    35147 2024-05-09 14:33:21.301315 sigmund-0.18.0/COPYING
--rw-r--r--   0        0        0     1036 2024-05-09 14:33:21.301315 sigmund-0.18.0/pyproject.toml
--rw-r--r--   0        0        0     3037 2024-05-09 14:33:21.301315 sigmund-0.18.0/readme.md
--rw-r--r--   0        0        0      101 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/__init__.py
--rw-r--r--   0        0        0     2746 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/attachments.py
--rw-r--r--   0        0        0    10431 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/config.py
--rw-r--r--   0        0        0        0 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/database/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/database/encryption.py
--rw-r--r--   0        0        0    14378 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/database/manager.py
--rw-r--r--   0        0        0     3213 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/database/models.py
--rw-r--r--   0        0        0     7190 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/documentation.py
--rw-r--r--   0        0        0      389 2024-05-09 14:33:21.301315 sigmund-0.18.0/sigmund/forms.py
--rw-r--r--   0        0        0     2643 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/library.py
--rw-r--r--   0        0        0    10115 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/messages.py
--rw-r--r--   0        0        0     1415 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/__init__.py
--rw-r--r--   0        0        0     5297 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/_anthropic_model.py
--rw-r--r--   0        0        0     4756 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/_base_model.py
--rw-r--r--   0        0        0      379 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/_dummy_model.py
--rw-r--r--   0        0        0     2700 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/_mistral_model.py
--rw-r--r--   0        0        0     3428 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/model/_openai_model.py
--rw-r--r--   0        0        0     2384 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/prompt.py
--rw-r--r--   0        0        0      197 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/__init__.py
--rw-r--r--   0        0        0     7334 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/api.py
--rw-r--r--   0        0        0     5776 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/app.py
--rw-r--r--   0        0        0     3769 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/google_login.py
--rw-r--r--   0        0        0     1838 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/public.py
--rw-r--r--   0        0        0     7733 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/routes/subscribe.py
--rw-r--r--   0        0        0     1580 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/server.py
--rw-r--r--   0        0        0     9430 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/sigmund.py
--rw-r--r--   0        0        0     4471 2024-05-09 14:33:21.305315 sigmund-0.18.0/sigmund/static/about.md
--rw-r--r--   0        0        0  4708018 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/background.png
--rw-r--r--   0        0        0      386 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/favicon.svg
--rw-r--r--   0        0        0     1433 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/login.md
--rw-r--r--   0        0        0     4976 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/pygments.css
--rw-r--r--   0        0        0   708136 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/sofa-with-sigmund.png
--rw-r--r--   0        0        0   684883 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/sofa.png
--rw-r--r--   0        0        0     3428 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/static/terms.md
--rw-r--r--   0        0        0     1359 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/chat.html
--rw-r--r--   0        0        0      242 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/footer.html
--rw-r--r--   0        0        0      574 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/head.html
--rw-r--r--   0        0        0      244 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/header.html
--rw-r--r--   0        0        0      329 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/info-page.html
--rw-r--r--   0        0        0     3739 2024-05-09 14:33:21.313315 sigmund-0.18.0/sigmund/templates/login.html
--rw-r--r--   0        0        0    10786 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/main.js
--rw-r--r--   0        0        0    12359 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/menu.html
--rw-r--r--   0        0        0      503 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/search-widget.html
--rw-r--r--   0        0        0     7676 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/search-widget.js
--rw-r--r--   0        0        0       80 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/sign-out.html
--rw-r--r--   0        0        0     6380 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/stylesheet.css.jinja
--rw-r--r--   0        0        0      531 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/subscribe-error.html
--rw-r--r--   0        0        0     1555 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/subscribe-now.html
--rw-r--r--   0        0        0      515 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/templates/subscribe-success.html
--rw-r--r--   0        0        0      265 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/__init__.py
--rw-r--r--   0        0        0     2231 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_base_tool.py
--rw-r--r--   0        0        0     2920 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_download.py
--rw-r--r--   0        0        0     2085 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_execute_code.py
--rw-r--r--   0        0        0     1846 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_read_attachment.py
--rw-r--r--   0        0        0     2076 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_search_documentation.py
--rw-r--r--   0        0        0     1275 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/tools/_search_google_scholar.py
--rw-r--r--   0        0        0     4335 2024-05-09 14:33:21.317315 sigmund-0.18.0/sigmund/utils.py
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 sigmund-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-14 12:06:02.087592 sigmund-0.19.0/COPYING
+-rw-r--r--   0        0        0     1036 2024-05-14 12:06:02.087592 sigmund-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0     3037 2024-05-14 12:06:02.087592 sigmund-0.19.0/readme.md
+-rw-r--r--   0        0        0      101 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/__init__.py
+-rw-r--r--   0        0        0     2746 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/attachments.py
+-rw-r--r--   0        0        0    10431 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/config.py
+-rw-r--r--   0        0        0        0 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/database/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/database/encryption.py
+-rw-r--r--   0        0        0    14378 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/database/manager.py
+-rw-r--r--   0        0        0     3213 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/database/models.py
+-rw-r--r--   0        0        0     7190 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/documentation.py
+-rw-r--r--   0        0        0      389 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/forms.py
+-rw-r--r--   0        0        0     2643 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/library.py
+-rw-r--r--   0        0        0    10115 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/messages.py
+-rw-r--r--   0        0        0     1410 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/__init__.py
+-rw-r--r--   0        0        0     5297 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/_anthropic_model.py
+-rw-r--r--   0        0        0     4756 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/_base_model.py
+-rw-r--r--   0        0        0      379 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/_dummy_model.py
+-rw-r--r--   0        0        0     2700 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/_mistral_model.py
+-rw-r--r--   0        0        0     3428 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/model/_openai_model.py
+-rw-r--r--   0        0        0     2384 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/prompt.py
+-rw-r--r--   0        0        0      197 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/__init__.py
+-rw-r--r--   0        0        0     7334 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/api.py
+-rw-r--r--   0        0        0     5776 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/app.py
+-rw-r--r--   0        0        0     3769 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/google_login.py
+-rw-r--r--   0        0        0     1838 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/public.py
+-rw-r--r--   0        0        0     7733 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/routes/subscribe.py
+-rw-r--r--   0        0        0     1580 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/server.py
+-rw-r--r--   0        0        0     9430 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/sigmund.py
+-rw-r--r--   0        0        0     4471 2024-05-14 12:06:02.087592 sigmund-0.19.0/sigmund/static/about.md
+-rw-r--r--   0        0        0  4708018 2024-05-14 12:06:02.095592 sigmund-0.19.0/sigmund/static/background.png
+-rw-r--r--   0        0        0      386 2024-05-14 12:06:02.095592 sigmund-0.19.0/sigmund/static/favicon.svg
+-rw-r--r--   0        0        0     1433 2024-05-14 12:06:02.095592 sigmund-0.19.0/sigmund/static/login.md
+-rw-r--r--   0        0        0     4976 2024-05-14 12:06:02.095592 sigmund-0.19.0/sigmund/static/pygments.css
+-rw-r--r--   0        0        0   708136 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/static/sofa-with-sigmund.png
+-rw-r--r--   0        0        0   684883 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/static/sofa.png
+-rw-r--r--   0        0        0     3428 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/static/terms.md
+-rw-r--r--   0        0        0     1359 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/chat.html
+-rw-r--r--   0        0        0      242 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/footer.html
+-rw-r--r--   0        0        0      574 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/head.html
+-rw-r--r--   0        0        0      244 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/header.html
+-rw-r--r--   0        0        0      329 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/info-page.html
+-rw-r--r--   0        0        0     3739 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/login.html
+-rw-r--r--   0        0        0    10786 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/main.js
+-rw-r--r--   0        0        0    12359 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/menu.html
+-rw-r--r--   0        0        0      503 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/search-widget.html
+-rw-r--r--   0        0        0     7676 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/search-widget.js
+-rw-r--r--   0        0        0       80 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/sign-out.html
+-rw-r--r--   0        0        0     6380 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/stylesheet.css.jinja
+-rw-r--r--   0        0        0      531 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/subscribe-error.html
+-rw-r--r--   0        0        0     1555 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/subscribe-now.html
+-rw-r--r--   0        0        0      515 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/templates/subscribe-success.html
+-rw-r--r--   0        0        0      265 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/__init__.py
+-rw-r--r--   0        0        0     2231 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_base_tool.py
+-rw-r--r--   0        0        0     2920 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_download.py
+-rw-r--r--   0        0        0     2085 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_execute_code.py
+-rw-r--r--   0        0        0     1846 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_read_attachment.py
+-rw-r--r--   0        0        0     2076 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_search_documentation.py
+-rw-r--r--   0        0        0     1275 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/tools/_search_google_scholar.py
+-rw-r--r--   0        0        0     4335 2024-05-14 12:06:02.099592 sigmund-0.19.0/sigmund/utils.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 sigmund-0.19.0/PKG-INFO
```

### Comparing `sigmund-0.18.0/COPYING` & `sigmund-0.19.0/COPYING`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/pyproject.toml` & `sigmund-0.19.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/readme.md` & `sigmund-0.19.0/readme.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/attachments.py` & `sigmund-0.19.0/sigmund/attachments.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/config.py` & `sigmund-0.19.0/sigmund/config.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/database/encryption.py` & `sigmund-0.19.0/sigmund/database/encryption.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/database/manager.py` & `sigmund-0.19.0/sigmund/database/manager.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/database/models.py` & `sigmund-0.19.0/sigmund/database/models.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/documentation.py` & `sigmund-0.19.0/sigmund/documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/library.py` & `sigmund-0.19.0/sigmund/library.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/messages.py` & `sigmund-0.19.0/sigmund/messages.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/model/__init__.py` & `sigmund-0.19.0/sigmund/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ._base_model import BaseModel
 
 
 def model(sigmund, model, **kwargs):
     """A factory function that returns a Model instance."""
     if model == 'gpt-4':
         from ._openai_model import OpenAIModel
-        return OpenAIModel(sigmund, 'gpt-4-turbo', **kwargs)
+        return OpenAIModel(sigmund, 'gpt-4o', **kwargs)
     if model == 'gpt-3.5':
         from ._openai_model import OpenAIModel
         return OpenAIModel(sigmund, 'gpt-3.5-turbo', **kwargs)
     if model == 'claude-2.1':
         from ._anthropic_model import AnthropicModel
         return AnthropicModel(sigmund, 'claude-2.1', **kwargs)
     if model == 'claude-3-opus':
```

### Comparing `sigmund-0.18.0/sigmund/model/_anthropic_model.py` & `sigmund-0.19.0/sigmund/model/_anthropic_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/model/_base_model.py` & `sigmund-0.19.0/sigmund/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/model/_mistral_model.py` & `sigmund-0.19.0/sigmund/model/_mistral_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/model/_openai_model.py` & `sigmund-0.19.0/sigmund/model/_openai_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/prompt.py` & `sigmund-0.19.0/sigmund/prompt.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/routes/api.py` & `sigmund-0.19.0/sigmund/routes/api.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/routes/app.py` & `sigmund-0.19.0/sigmund/routes/app.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/routes/google_login.py` & `sigmund-0.19.0/sigmund/routes/google_login.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/routes/public.py` & `sigmund-0.19.0/sigmund/routes/public.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/routes/subscribe.py` & `sigmund-0.19.0/sigmund/routes/subscribe.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/server.py` & `sigmund-0.19.0/sigmund/server.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/sigmund.py` & `sigmund-0.19.0/sigmund/sigmund.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/about.md` & `sigmund-0.19.0/sigmund/static/about.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/background.png` & `sigmund-0.19.0/sigmund/static/background.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/login.md` & `sigmund-0.19.0/sigmund/static/login.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/pygments.css` & `sigmund-0.19.0/sigmund/static/pygments.css`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/sofa-with-sigmund.png` & `sigmund-0.19.0/sigmund/static/sofa-with-sigmund.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/sofa.png` & `sigmund-0.19.0/sigmund/static/sofa.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/static/terms.md` & `sigmund-0.19.0/sigmund/static/terms.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/chat.html` & `sigmund-0.19.0/sigmund/templates/chat.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/head.html` & `sigmund-0.19.0/sigmund/templates/head.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/login.html` & `sigmund-0.19.0/sigmund/templates/login.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/main.js` & `sigmund-0.19.0/sigmund/templates/main.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/menu.html` & `sigmund-0.19.0/sigmund/templates/menu.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/search-widget.js` & `sigmund-0.19.0/sigmund/templates/search-widget.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/stylesheet.css.jinja` & `sigmund-0.19.0/sigmund/templates/stylesheet.css.jinja`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/subscribe-error.html` & `sigmund-0.19.0/sigmund/templates/subscribe-error.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/subscribe-now.html` & `sigmund-0.19.0/sigmund/templates/subscribe-now.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/templates/subscribe-success.html` & `sigmund-0.19.0/sigmund/templates/subscribe-success.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_base_tool.py` & `sigmund-0.19.0/sigmund/tools/_base_tool.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_download.py` & `sigmund-0.19.0/sigmund/tools/_download.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_execute_code.py` & `sigmund-0.19.0/sigmund/tools/_execute_code.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_read_attachment.py` & `sigmund-0.19.0/sigmund/tools/_read_attachment.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_search_documentation.py` & `sigmund-0.19.0/sigmund/tools/_search_documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/tools/_search_google_scholar.py` & `sigmund-0.19.0/sigmund/tools/_search_google_scholar.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/sigmund/utils.py` & `sigmund-0.19.0/sigmund/utils.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.18.0/PKG-INFO` & `sigmund-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmund
-Version: 0.18.0
+Version: 0.19.0
 Summary: AI-based chatbot that provides sensible answers based on documentation
 Keywords: ai,chatbot,llm
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anthropic
 Requires-Dist: cryptography
```

