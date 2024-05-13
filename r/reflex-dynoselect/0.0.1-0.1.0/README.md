# Comparing `tmp/reflex_dynoselect-0.0.1.tar.gz` & `tmp/reflex_dynoselect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_dynoselect-0.0.1.tar", last modified: Wed Apr 17 20:04:51 2024, max compression
+gzip compressed data, was "reflex_dynoselect-0.1.0.tar", last modified: Mon May 13 22:07:29 2024, max compression
```

## Comparing `reflex_dynoselect-0.0.1.tar` & `reflex_dynoselect-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 20:04:51.850333 reflex_dynoselect-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-17 16:48:40.000000 reflex_dynoselect-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6038 2024-04-17 20:04:51.850333 reflex_dynoselect-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5086 2024-04-17 19:18:24.000000 reflex_dynoselect-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 20:04:51.819111 reflex_dynoselect-0.0.1/custom_components/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:04:51.819111 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect/
--rw-rw-rw-   0        0        0       25 2024-04-15 16:15:30.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect/__init__.py
--rw-rw-rw-   0        0        0    15658 2024-04-17 16:42:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect/dynoselect.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:04:51.850333 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/
--rw-rw-rw-   0        0        0     6038 2024-04-17 20:04:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-17 20:04:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 20:04:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-17 20:04:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 20:04:51.000000 reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2024-04-17 20:02:40.000000 reflex_dynoselect-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 20:04:51.850333 reflex_dynoselect-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 22:07:29.324778 reflex_dynoselect-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 16:48:40.000000 reflex_dynoselect-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9241 2024-05-13 22:07:29.324778 reflex_dynoselect-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8543 2024-05-13 20:43:29.000000 reflex_dynoselect-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 22:07:29.293574 reflex_dynoselect-0.1.0/custom_components/
+drwxrwxrwx   0        0        0        0 2024-05-13 22:07:29.309185 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/
+-rw-rw-rw-   0        0        0       49 2024-04-28 18:07:14.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/__init__.py
+-rw-rw-rw-   0        0        0    23136 2024-05-13 19:48:14.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/dynoselect.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:07:29.324778 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/options/
+-rw-rw-rw-   0        0        0     6300 2024-05-11 15:29:59.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/options/__init__.py
+-rw-rw-rw-   0        0        0      860 2024-04-22 20:38:55.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:07:29.324778 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/
+-rw-rw-rw-   0        0        0     9241 2024-05-13 22:07:29.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-13 22:07:29.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 22:07:29.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-13 22:07:29.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 22:07:29.000000 reflex_dynoselect-0.1.0/custom_components/reflex_dynoselect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      872 2024-05-13 21:54:27.000000 reflex_dynoselect-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 22:07:29.324778 reflex_dynoselect-0.1.0/setup.cfg
```

### Comparing `reflex_dynoselect-0.0.1/LICENSE` & `reflex_dynoselect-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_dynoselect-0.0.1/PKG-INFO` & `reflex_dynoselect-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-Metadata-Version: 2.1
-Name: reflex-dynoselect
-Version: 0.0.1
-Summary: Reflex select component which allows the user to search for options and create new ones.
-Author-email: Marcus Wörner <woernerm@protonmail.com>
-License: Apache-2.0
-Project-URL: homepage, https://github.com/woernerm/dynoselect
-Keywords: reflex,reflex-custom-components,select,search,creatable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.6
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
 # Dynoselect
 
-This is a select component for [Reflex](https://reflex.dev) which allows users to 
-search for options and create new ones:
+Dynoselect is a collection of select components for [Reflex](https://reflex.dev). 
+The base component allows users to search for options and create new ones:
+
+<img src="data/demo.gif" height="300px">
+
+In addition, there are specialized components for standard use-cases like time zone and 
+language selection. The options listed by them are available in over 100 
+languages (and over 400 language variants!) so you don't have to translate them yourself.
+Just specify the [IETF language tag](https://en.wikipedia.org/wiki/IETF_language_tag) 
+you would like to use, e.g. _"de"_ for German (as spoken in Germany) or _"en-GB"_ for 
+English (as spoken in the United Kingdom).
+
+There is a special "locale" available for the language select component: Displaying 
+each language option in the respective language itself. For this, just specify 
+`None` for the `locale` parameter of the component:
+
+<img src="data/language.gif" height="480px">
+
+Selecting one's own time zone is a surprisingly difficult task for most users. 
+This has been studied quite extensively in [this Article](https://www.nngroup.com/articles/time-zone-selectors/).
+The time zone selection component makes this task as simple as possible.
 
-<img src="data/demo.gif" height="400px">
+Not having to select your time zone at all is of course most user-friendly. 
+Therefore, the component tries to automatically detect the user's time zone. Manual
+selection is only necessary if the result turns out to be incorrect. 
 
-The following example shows how to use the component within a Reflex project:
+Following the advice given in the above article, the component lists time zones as 
+__city, country (UTC offset)__. This is because most people can name a city or country 
+representative of their time zone. The offset is given last, because people expect the 
+list to be ordered alphabetically and often do not know their offset anyway. It mainly
+serves as confirmation. The offset displayed takes into 
+account whether daylight saving time is currently in effect in each listed time zone and 
+is updated every time the dropdown is opened.
+
+<img src="data/timezone.gif" height="480px">
+
+
+The following example shows how to use the components within a Reflex project:
 
 ```py
 import reflex as rx
-from reflex_dynoselect import dynoselect
+from reflex_dynoselect import dynoselect, dynotimezone, dynolanguage
 
 options = [
     {"value": "ocean", "label": "Ocean"},
     {"value": "blue", "label": "Blue"},
     {"value": "purple", "label": "Purple"},
     {"value": "green", "label": "Green"},
     {"value": "red", "label": "Red"},
@@ -44,21 +53,32 @@
 ]
 
 class State(rx.State):
     """The app state."""
     pass
 
 def index() -> rx.Component:
-    return rx.center(
-        rx.theme_panel(),
+    return rx.vstack(
         dynoselect(
             options,
             placeholder="Select a color",
             search_placeholder="Search for a color",
         ),
+        dynotimezone(
+            "en",
+            placeholder="Timezone", 
+            search_placeholder="Search timezone..."
+        ),        
+        dynolanguage(
+            "en",
+            placeholder="Language", 
+            search_placeholder="Search for a language..."
+        ),
+        align="center",
+        spacing="4"
     )
 
 # Add state and page to the app.
 app = rx.App()
 app.add_page(index)
 ```
 
@@ -71,65 +91,89 @@
 The `selected` attribute contains the complete dictionary of the currently selected 
 option. In addition to the `value`, `label`, and `keywords` keys, one can add
 arbitrary keys to the dictionary to store additional information about an option.
 
 ### Parameters
 - `options`: A list of dictionaries containing the options. The dictionary
     must contain a `label` and a `value` key with strings as values. The value of the
-    `label` key is displayed to the user while the `value` key can be used for internal
-    identifiers. Optionally, one can provide a `keywords` key to include alternative 
+    `label` key is displayed to the user while the `value` key can be used as internal
+    identifier. Optionally, one can provide a `keywords` key to include alternative 
     phrases that are included in the search but not displayed to the user. This is 
     intended to improve the search tolerance so that users can find options even 
-    if synonyms are used. You may provide keywords either as a string or as a list
+    if they enter synonyms. You may provide keywords either as a string or as a list
     of strings. For example, the option
     ```py
     {"value": "ocean", "label": "Ocean", "keywords": ["blue", "water"]}
     ```
-    allows to input _"water"_ in order to search for the color _Ocean_ as shown below:
+    allows to input _"water"_ or _"blue"_ in order to search for the color _Ocean_.
 
-    <img src="data/keyword-search.jpg" height="300px">
 - `default_option`: The default option to select. By default, no option is selected.
 - `placeholder`: The placeholder text that is shown when no option is selected.
 - `search_placeholder`: The placeholder text for the search input field.
 - `size`: Relative size of the component. Allowed values are "1", "2", and "3".
 - `weight`: The weight of the text. Allowed values are "none", "light", "regular", 
     "medium", and "bold".
 - `radius`: The edge radius of the component. Allowed values are "none", "small", 
     "medium", "large", and "full".
 - `height`: The height of the component menu. Can be given as a CSS value like "10rem" 
     or "100%".
 - `padding`: The padding around the border of the select menu.
-- `indent`: The indentation of the select menu. If `align` is chosen to be "center", the 
+- `indent`: The indentation of the select menu. If "center" is given, the 
     indentation is applied horizontally to both sides and therefore acts as padding. 
     Otherwise, it is applied to one side only and works as indentation.
 - `align`: The alignment of the options. Allowed values are "left", "center", and 
     "right".
 - `create_option`: The option dictionary to create a new entry. If `create_option` is 
-    None, the feature is deactivated. If the option is a dictionary, it determines the 
-    `value` and `label` of the create option. You may either provide a static text
-    or refer to the current search phrase by using "{}" as placeholder in the
-    `label`. For example:
+    None, the feature is deactivated. If the option is a dictionary, it specifies the 
+    `value` and `label` attributes used for the create option. You may either provide a 
+    static text or refer to the current search phrase by using "{}" as placeholder. 
+    For example:
     ```py
     dynoselect(
         options,
         placeholder="Select a color",
         search_placeholder="Search for a color",
         create_option=dict(value="custom", label='Create new "{}"'),
     )
     ```
     The `label` given in the example above would be displayed as _Create new "Apple"_ if 
     the search phrase is _"Apple"_. Regarding the `value` key, you can use any value you 
     like.   
-- `modal`: Directly passed on to PopoverRoot. If true, interaction on screen 
-    readers with other elements is disabled and only popover content is visible.
 - `on_select`: Event handler that is called when the user selects an option. Note
     that the event handler is called even if the user selects the same value as before.
+- `icon`: The name of the [lucide icon](https://lucide.dev/icons/) to display.
+- `content_props`: Additional properties that are passed on to the 
+    [reflex.popover.content](https://reflex.dev/docs/library/overlay/popover/#popovercontent) 
+    component used by Dynoselect.
+- `root_props`: Additional properties that are passed on to the 
+    [reflex.popover.root](https://reflex.dev/docs/library/overlay/popover/#popoverroot) 
+    component used by Dynoselect.
+
+#### Additional options for `dynotimezone`:
+- `locale`: The locale to display the time zone options in. 
+
+#### Additional options for `dynolanguage`:
+- `locale`: The locale to use for the displayed language options. If None, the names 
+    of all languages are displayed in the respective languages themselves.
+- `only` : Optional iterable with [IETF language tags](https://en.wikipedia.org/wiki/IETF_language_tag) 
+    to display. Default is None, so that all available language options are displayed. 
+    Example:
+    ```py
+    dynolanguage(
+        placeholder="Language", 
+        search_placeholder="Search for a language...",
+        only={"de", "en", "en-GB", "es", "fr", "fr-CH"},
+    ),
+    ```
+    This will display options for German (as spoken in Germany), English (as spoken in 
+    the United States), English (as spoken in the UK), Spanish (as spoken in Spain), 
+    French (as spoken in France), and French (as spoken in Switzerland).
 
 ## Installation
-The component has been tested without activating [Tailwind](https://tailwindcss.com/) 
+The components have been tested without activating [Tailwind](https://tailwindcss.com/) 
 explicitly. However, if the component looks strange, you may want to activate it as 
 described in the [official documentation](https://reflex.dev/docs/styling/overview/#tailwind).
 
-The component can be installed using the following command:
+The components can be installed using the following command:
 ```bash
 pip install reflex-dynoselect
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reflex_dynoselect-0.0.1/custom_components/reflex_dynoselect.egg-info/PKG-INFO` & `reflex_dynoselect-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,67 @@
 Metadata-Version: 2.1
 Name: reflex-dynoselect
-Version: 0.0.1
-Summary: Reflex select component which allows the user to search for options and create new ones.
+Version: 0.1.0
+Summary: Generic and specialized Reflex select components. Users can search for options and create new ones. Includes specialized time zone and language select components in over 100 languages.
 Author-email: Marcus Wörner <woernerm@protonmail.com>
 License: Apache-2.0
-Project-URL: homepage, https://github.com/woernerm/dynoselect
-Keywords: reflex,reflex-custom-components,select,search,creatable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
+Keywords: reflex,reflex-custom-components,select,timezone,time zone,locale,language,language select
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reflex>=0.4.6
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # Dynoselect
 
-This is a select component for [Reflex](https://reflex.dev) which allows users to 
-search for options and create new ones:
+Dynoselect is a collection of select components for [Reflex](https://reflex.dev). 
+The base component allows users to search for options and create new ones:
 
-<img src="data/demo.gif" height="400px">
+<img src="data/demo.gif" height="300px">
 
-The following example shows how to use the component within a Reflex project:
+In addition, there are specialized components for standard use-cases like time zone and 
+language selection. The options listed by them are available in over 100 
+languages (and over 400 language variants!) so you don't have to translate them yourself.
+Just specify the [IETF language tag](https://en.wikipedia.org/wiki/IETF_language_tag) 
+you would like to use, e.g. _"de"_ for German (as spoken in Germany) or _"en-GB"_ for 
+English (as spoken in the United Kingdom).
+
+There is a special "locale" available for the language select component: Displaying 
+each language option in the respective language itself. For this, just specify 
+`None` for the `locale` parameter of the component:
+
+<img src="data/language.gif" height="480px">
+
+Selecting one's own time zone is a surprisingly difficult task for most users. 
+This has been studied quite extensively in [this Article](https://www.nngroup.com/articles/time-zone-selectors/).
+The time zone selection component makes this task as simple as possible.
+
+Not having to select your time zone at all is of course most user-friendly. 
+Therefore, the component tries to automatically detect the user's time zone. Manual
+selection is only necessary if the result turns out to be incorrect. 
+
+Following the advice given in the above article, the component lists time zones as 
+__city, country (UTC offset)__. This is because most people can name a city or country 
+representative of their time zone. The offset is given last, because people expect the 
+list to be ordered alphabetically and often do not know their offset anyway. It mainly
+serves as confirmation. The offset displayed takes into 
+account whether daylight saving time is currently in effect in each listed time zone and 
+is updated every time the dropdown is opened.
+
+<img src="data/timezone.gif" height="480px">
+
+
+The following example shows how to use the components within a Reflex project:
 
 ```py
 import reflex as rx
-from reflex_dynoselect import dynoselect
+from reflex_dynoselect import dynoselect, dynotimezone, dynolanguage
 
 options = [
     {"value": "ocean", "label": "Ocean"},
     {"value": "blue", "label": "Blue"},
     {"value": "purple", "label": "Purple"},
     {"value": "green", "label": "Green"},
     {"value": "red", "label": "Red"},
@@ -44,21 +69,32 @@
 ]
 
 class State(rx.State):
     """The app state."""
     pass
 
 def index() -> rx.Component:
-    return rx.center(
-        rx.theme_panel(),
+    return rx.vstack(
         dynoselect(
             options,
             placeholder="Select a color",
             search_placeholder="Search for a color",
         ),
+        dynotimezone(
+            "en",
+            placeholder="Timezone", 
+            search_placeholder="Search timezone..."
+        ),        
+        dynolanguage(
+            "en",
+            placeholder="Language", 
+            search_placeholder="Search for a language..."
+        ),
+        align="center",
+        spacing="4"
     )
 
 # Add state and page to the app.
 app = rx.App()
 app.add_page(index)
 ```
 
@@ -71,65 +107,89 @@
 The `selected` attribute contains the complete dictionary of the currently selected 
 option. In addition to the `value`, `label`, and `keywords` keys, one can add
 arbitrary keys to the dictionary to store additional information about an option.
 
 ### Parameters
 - `options`: A list of dictionaries containing the options. The dictionary
     must contain a `label` and a `value` key with strings as values. The value of the
-    `label` key is displayed to the user while the `value` key can be used for internal
-    identifiers. Optionally, one can provide a `keywords` key to include alternative 
+    `label` key is displayed to the user while the `value` key can be used as internal
+    identifier. Optionally, one can provide a `keywords` key to include alternative 
     phrases that are included in the search but not displayed to the user. This is 
     intended to improve the search tolerance so that users can find options even 
-    if synonyms are used. You may provide keywords either as a string or as a list
+    if they enter synonyms. You may provide keywords either as a string or as a list
     of strings. For example, the option
     ```py
     {"value": "ocean", "label": "Ocean", "keywords": ["blue", "water"]}
     ```
-    allows to input _"water"_ in order to search for the color _Ocean_ as shown below:
+    allows to input _"water"_ or _"blue"_ in order to search for the color _Ocean_.
 
-    <img src="data/keyword-search.jpg" height="300px">
 - `default_option`: The default option to select. By default, no option is selected.
 - `placeholder`: The placeholder text that is shown when no option is selected.
 - `search_placeholder`: The placeholder text for the search input field.
 - `size`: Relative size of the component. Allowed values are "1", "2", and "3".
 - `weight`: The weight of the text. Allowed values are "none", "light", "regular", 
     "medium", and "bold".
 - `radius`: The edge radius of the component. Allowed values are "none", "small", 
     "medium", "large", and "full".
 - `height`: The height of the component menu. Can be given as a CSS value like "10rem" 
     or "100%".
 - `padding`: The padding around the border of the select menu.
-- `indent`: The indentation of the select menu. If `align` is chosen to be "center", the 
+- `indent`: The indentation of the select menu. If "center" is given, the 
     indentation is applied horizontally to both sides and therefore acts as padding. 
     Otherwise, it is applied to one side only and works as indentation.
 - `align`: The alignment of the options. Allowed values are "left", "center", and 
     "right".
 - `create_option`: The option dictionary to create a new entry. If `create_option` is 
-    None, the feature is deactivated. If the option is a dictionary, it determines the 
-    `value` and `label` of the create option. You may either provide a static text
-    or refer to the current search phrase by using "{}" as placeholder in the
-    `label`. For example:
+    None, the feature is deactivated. If the option is a dictionary, it specifies the 
+    `value` and `label` attributes used for the create option. You may either provide a 
+    static text or refer to the current search phrase by using "{}" as placeholder. 
+    For example:
     ```py
     dynoselect(
         options,
         placeholder="Select a color",
         search_placeholder="Search for a color",
         create_option=dict(value="custom", label='Create new "{}"'),
     )
     ```
     The `label` given in the example above would be displayed as _Create new "Apple"_ if 
     the search phrase is _"Apple"_. Regarding the `value` key, you can use any value you 
     like.   
-- `modal`: Directly passed on to PopoverRoot. If true, interaction on screen 
-    readers with other elements is disabled and only popover content is visible.
 - `on_select`: Event handler that is called when the user selects an option. Note
     that the event handler is called even if the user selects the same value as before.
+- `icon`: The name of the [lucide icon](https://lucide.dev/icons/) to display.
+- `content_props`: Additional properties that are passed on to the 
+    [reflex.popover.content](https://reflex.dev/docs/library/overlay/popover/#popovercontent) 
+    component used by Dynoselect.
+- `root_props`: Additional properties that are passed on to the 
+    [reflex.popover.root](https://reflex.dev/docs/library/overlay/popover/#popoverroot) 
+    component used by Dynoselect.
+
+#### Additional options for `dynotimezone`:
+- `locale`: The locale to display the time zone options in. 
+
+#### Additional options for `dynolanguage`:
+- `locale`: The locale to use for the displayed language options. If None, the names 
+    of all languages are displayed in the respective languages themselves.
+- `only` : Optional iterable with [IETF language tags](https://en.wikipedia.org/wiki/IETF_language_tag) 
+    to display. Default is None, so that all available language options are displayed. 
+    Example:
+    ```py
+    dynolanguage(
+        placeholder="Language", 
+        search_placeholder="Search for a language...",
+        only={"de", "en", "en-GB", "es", "fr", "fr-CH"},
+    ),
+    ```
+    This will display options for German (as spoken in Germany), English (as spoken in 
+    the United States), English (as spoken in the UK), Spanish (as spoken in Spain), 
+    French (as spoken in France), and French (as spoken in Switzerland).
 
 ## Installation
-The component has been tested without activating [Tailwind](https://tailwindcss.com/) 
+The components have been tested without activating [Tailwind](https://tailwindcss.com/) 
 explicitly. However, if the component looks strange, you may want to activate it as 
 described in the [official documentation](https://reflex.dev/docs/styling/overview/#tailwind).
 
-The component can be installed using the following command:
+The components can be installed using the following command:
 ```bash
 pip install reflex-dynoselect
 ```
```

