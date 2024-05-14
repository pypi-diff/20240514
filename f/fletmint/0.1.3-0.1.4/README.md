# Comparing `tmp/fletmint-0.1.3.tar.gz` & `tmp/fletmint-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fletmint-0.1.3.tar", last modified: Thu May  9 19:37:35 2024, max compression
+gzip compressed data, was "fletmint-0.1.4.tar", last modified: Tue May 14 13:16:30 2024, max compression
```

## Comparing `fletmint-0.1.3.tar` & `fletmint-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 19:37:35.804101 fletmint-0.1.3/
--rw-rw-rw-   0        0        0      794 2024-05-09 19:37:35.804101 fletmint-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 19:37:35.788475 fletmint-0.1.3/fletmint/
--rw-rw-rw-   0        0        0      618 2024-05-09 08:23:35.000000 fletmint-0.1.3/fletmint/__init__.py
--rw-rw-rw-   0        0        0     6402 2024-05-08 07:02:01.000000 fletmint-0.1.3/fletmint/audioplayer.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 07:35:28.000000 fletmint-0.1.3/fletmint/badge.py
--rw-rw-rw-   0        0        0     5419 2024-05-08 15:24:34.000000 fletmint-0.1.3/fletmint/button.py
--rw-rw-rw-   0        0        0     4341 2024-05-08 16:20:00.000000 fletmint-0.1.3/fletmint/carousel.py
--rw-rw-rw-   0        0        0     5505 2024-05-07 07:52:05.000000 fletmint-0.1.3/fletmint/checkbox.py
--rw-rw-rw-   0        0        0    13220 2024-05-09 07:52:07.000000 fletmint-0.1.3/fletmint/datepicker.py
--rw-rw-rw-   0        0        0     7784 2024-05-09 07:55:00.000000 fletmint-0.1.3/fletmint/dropdown.py
--rw-rw-rw-   0        0        0     3875 2024-05-07 08:56:00.000000 fletmint-0.1.3/fletmint/profile.py
--rw-rw-rw-   0        0        0      408 2024-05-09 07:29:27.000000 fletmint-0.1.3/fletmint/radio.py
--rw-rw-rw-   0        0        0     1572 2024-05-07 14:45:09.000000 fletmint-0.1.3/fletmint/slider.py
--rw-rw-rw-   0        0        0     4954 2024-05-07 07:52:19.000000 fletmint-0.1.3/fletmint/stepper.py
--rw-rw-rw-   0        0        0     3558 2024-05-07 07:52:22.000000 fletmint-0.1.3/fletmint/tab_switch.py
--rw-rw-rw-   0        0        0     4007 2024-05-06 20:07:39.000000 fletmint-0.1.3/fletmint/table.py
--rw-rw-rw-   0        0        0     3297 2024-05-09 08:25:59.000000 fletmint-0.1.3/fletmint/tags_input.py
--rw-rw-rw-   0        0        0     5694 2024-05-07 07:50:29.000000 fletmint-0.1.3/fletmint/text_input.py
--rw-rw-rw-   0        0        0     3012 2024-05-07 15:21:55.000000 fletmint-0.1.3/fletmint/toggle.py
--rw-rw-rw-   0        0        0     3510 2024-05-07 14:46:28.000000 fletmint-0.1.3/fletmint/toggle_switch.py
--rw-rw-rw-   0        0        0     3739 2024-05-08 08:32:44.000000 fletmint-0.1.3/fletmint/videoplayer.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:37:35.804101 fletmint-0.1.3/fletmint.egg-info/
--rw-rw-rw-   0        0        0      794 2024-05-09 19:37:35.000000 fletmint-0.1.3/fletmint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-09 19:37:35.000000 fletmint-0.1.3/fletmint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 19:37:35.000000 fletmint-0.1.3/fletmint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 19:37:35.000000 fletmint-0.1.3/fletmint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 19:37:35.000000 fletmint-0.1.3/fletmint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 19:37:35.804101 fletmint-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-05-09 19:37:28.000000 fletmint-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:30.387040 fletmint-0.1.4/
+-rw-rw-rw-   0        0        0      896 2024-05-14 13:16:30.387040 fletmint-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:30.376592 fletmint-0.1.4/fletmint/
+-rw-rw-rw-   0        0        0      618 2024-05-09 08:23:35.000000 fletmint-0.1.4/fletmint/__init__.py
+-rw-rw-rw-   0        0        0     6402 2024-05-08 07:02:01.000000 fletmint-0.1.4/fletmint/audioplayer.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 07:35:28.000000 fletmint-0.1.4/fletmint/badge.py
+-rw-rw-rw-   0        0        0     5471 2024-05-14 12:43:49.000000 fletmint-0.1.4/fletmint/button.py
+-rw-rw-rw-   0        0        0     4341 2024-05-08 16:20:00.000000 fletmint-0.1.4/fletmint/carousel.py
+-rw-rw-rw-   0        0        0     5505 2024-05-07 07:52:05.000000 fletmint-0.1.4/fletmint/checkbox.py
+-rw-rw-rw-   0        0        0    14078 2024-05-14 12:59:01.000000 fletmint-0.1.4/fletmint/datepicker.py
+-rw-rw-rw-   0        0        0     7784 2024-05-09 07:55:00.000000 fletmint-0.1.4/fletmint/dropdown.py
+-rw-rw-rw-   0        0        0     3875 2024-05-07 08:56:00.000000 fletmint-0.1.4/fletmint/profile.py
+-rw-rw-rw-   0        0        0      408 2024-05-09 07:29:27.000000 fletmint-0.1.4/fletmint/radio.py
+-rw-rw-rw-   0        0        0     1572 2024-05-07 14:45:09.000000 fletmint-0.1.4/fletmint/slider.py
+-rw-rw-rw-   0        0        0     4954 2024-05-07 07:52:19.000000 fletmint-0.1.4/fletmint/stepper.py
+-rw-rw-rw-   0        0        0     3558 2024-05-07 07:52:22.000000 fletmint-0.1.4/fletmint/tab_switch.py
+-rw-rw-rw-   0        0        0     4007 2024-05-06 20:07:39.000000 fletmint-0.1.4/fletmint/table.py
+-rw-rw-rw-   0        0        0     3297 2024-05-09 08:25:59.000000 fletmint-0.1.4/fletmint/tags_input.py
+-rw-rw-rw-   0        0        0     5694 2024-05-07 07:50:29.000000 fletmint-0.1.4/fletmint/text_input.py
+-rw-rw-rw-   0        0        0     3012 2024-05-07 15:21:55.000000 fletmint-0.1.4/fletmint/toggle.py
+-rw-rw-rw-   0        0        0     3510 2024-05-07 14:46:28.000000 fletmint-0.1.4/fletmint/toggle_switch.py
+-rw-rw-rw-   0        0        0     3739 2024-05-08 08:32:44.000000 fletmint-0.1.4/fletmint/videoplayer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:30.387040 fletmint-0.1.4/fletmint.egg-info/
+-rw-rw-rw-   0        0        0      896 2024-05-14 13:16:30.000000 fletmint-0.1.4/fletmint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-14 13:16:30.000000 fletmint-0.1.4/fletmint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:16:30.000000 fletmint-0.1.4/fletmint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-14 13:16:30.000000 fletmint-0.1.4/fletmint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 13:16:30.000000 fletmint-0.1.4/fletmint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:16:30.388482 fletmint-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2024-05-14 13:16:19.000000 fletmint-0.1.4/setup.py
```

### Comparing `fletmint-0.1.3/fletmint/__init__.py` & `fletmint-0.1.4/fletmint/__init__.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/audioplayer.py` & `fletmint-0.1.4/fletmint/audioplayer.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/badge.py` & `fletmint-0.1.4/fletmint/badge.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/button.py` & `fletmint-0.1.4/fletmint/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     ):
         # Override the background color for a destructive button (red)
         secondary_style = ButtonStyle(
             color={
                 MaterialState.DEFAULT: colors.BLACK,  # MaterialState.DEFAULT
             },
             bgcolor={
-                "": "#f0f0f0"
+                "": colors.with_opacity(0.1, ButtonColors.button_backgound_color)
                 if not disabled
                 else ButtonColors.button_disabled_background_color,
                 "disabled": ButtonColors.button_disabled_background_color,
             },
             padding=18,
             shape=ContinuousRectangleBorder(radius=20),
         )
```

### Comparing `fletmint-0.1.3/fletmint/carousel.py` & `fletmint-0.1.4/fletmint/carousel.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/checkbox.py` & `fletmint-0.1.4/fletmint/checkbox.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/datepicker.py` & `fletmint-0.1.4/fletmint/datepicker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import flet as ft
 from .text_input import TextInput
-from .button import Button
+from .button import Button, SecondaryButton
 from datetime import datetime, timedelta, timezone
 from dataclasses import dataclass
 import locale
 
 
 @dataclass
 class DatePickerColors:
@@ -47,54 +47,66 @@
         )
 
 
 class DatePicker(ft.UserControl):
     def __init__(
         self,
         tz_info=timezone.utc,
+        left_content=None,
         max_width=300,
         is_dropdown=True,
         multi_select_mode=True,
         on_date_choosen=None,
+        on_cancel=None,
         theme: ft.ThemeMode | str = ft.ThemeMode.DARK,
         drodown_icons=[
             ft.icons.ARROW_DROP_DOWN_ROUNDED,
             ft.icons.ARROW_DROP_UP_ROUNDED,
         ],
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.tz_info = tz_info
+        self.left_content = left_content
         self.max_width = max_width
         self.is_dropdown = is_dropdown
         self.on_date_choosen = on_date_choosen
+        self.on_cancel = on_cancel
         self.multi_select_mode = multi_select_mode
         self.dropdown_icons = drodown_icons
         self.selected_dates = set()
-        self.current_month = datetime.now().month
-        self.current_year = datetime.now().year
+        self.current_month = datetime.now(self.tz_info).month
+        self.current_year = datetime.now(self.tz_info).year
         self.colors = (
             DatePickerColors.dark()
             if theme == ft.ThemeMode.DARK
             else DatePickerColors.light()
         )
         self.show_splash = False
         self.dropdown_starter_bounds = None
+        self.previous_selected_button = None
 
     def __on_selected_date(self, e):
-        # return self.selected_dates
         dates = [date.strftime("%Y-%m-%d") for date in self.selected_dates]
-        self.dropdown_starter.content.content.controls[0].content.content.controls[
-            0
-        ].value = ", ".join(dates)
-        self.unfocus_dropdown()
-        self.close_calendar_dropdown()
+        if self.is_dropdown:
+            self.dropdown_starter.content.content.controls[0].content.content.controls[
+                0
+            ].value = ", ".join(dates)
+            self.unfocus_dropdown()
+            self.close_calendar_dropdown()
         if self.on_date_choosen:
             self.on_date_choosen(self.selected_dates)
 
+    def __on_cancel(self, e):
+        if self.is_dropdown:
+            self.unfocus_dropdown()
+            self.close_calendar_dropdown()
+        if self.on_cancel:
+            self.on_cancel()
+
     def unfocus_dropdown(self):
         self.dropdown_starter.content.content.controls[0].remove_hover_state(None)
         self.dropdown_starter.content.content.controls[1].content = ft.Icon(
             name=self.dropdown_icons[0],
             color=self.colors.dropdown_starter_icon_color,
             size=25,
         )
@@ -102,25 +114,24 @@
 
     def close_calendar_dropdown(self):
         self.page.splash = None
         self.show_splash = False
         self.page.update()
 
     def adjust_month(self, change):
-        # Adjusts the current month and year
         new_month = self.current_month + change
         if new_month > 12:
             self.current_month = 1
             self.current_year += 1
         elif new_month < 1:
             self.current_month = 12
             self.current_year -= 1
         else:
             self.current_month = new_month
-        self.update_calendar()  # Rebuild the calendar with the new month
+        self.update_calendar()
 
     def update_calendar(self):
         self.calendarpicker.content.controls[1] = self.build_calendar()
         self.calendarpicker.content.controls[0].controls[1].value = datetime(
             self.current_year, self.current_month, 1
         ).strftime("%B %Y")
         self.calendarpicker.update()
@@ -130,42 +141,43 @@
             controls=[
                 ft.Container(
                     ft.Text(day, color=self.colors.weekday_color),
                     alignment=ft.alignment.center,
                 )
                 for day in ("Mo", "Tu", "We", "Th", "Fr", "Sa", "Su")
             ],
-            runs_count=7,  # 7 days a week
+            runs_count=7,
             spacing=4,
             run_spacing=4,
             padding=ft.padding.all(10),
         )
 
-        self.today = datetime.now()
+        self.today = datetime.now(self.tz_info)
         start_of_month = datetime(self.current_year, self.current_month, 1)
-        start_day_of_week = start_of_month.weekday()  # 0=Monday, 6=Sunday
+        start_day_of_week = start_of_month.weekday()
         end_of_month = start_of_month.replace(
             month=start_of_month.month % 12 + 1, day=1
         ) - timedelta(days=1)
         days_in_month = end_of_month.day
 
-        # Add filler days from previous month
         filler_days = (start_day_of_week + 7) % 7
         for i in range(filler_days):
             day = (start_of_month - timedelta(days=filler_days - i)).day
             grid.controls.append(self.create_day_button(str(day), is_filler=True))
 
-        # Create buttons for each day
         for i in range(1, days_in_month + 1):
-            day = datetime(self.today.year, self.today.month, i)
-            is_today = i == self.today.day
+            day = datetime(self.current_year, self.current_month, i)
+            is_today = (
+                self.current_month == self.today.month
+                and self.current_year == self.today.year
+                and i == self.today.day
+            )
             button = self.create_day_button(str(i), is_today=is_today, day_date=day)
             grid.controls.append(button)
 
-        # Add filler days for the next month
         next_month_day_count = (7 - (end_of_month.weekday() + 1)) % 7
         for i in range(1, next_month_day_count + 1):
             grid.controls.append(self.create_day_button(str(i), is_filler=True))
 
         return grid
 
     def create_day_button(self, text, is_today=False, is_filler=False, day_date=None):
@@ -197,38 +209,51 @@
             button.enabled = False
         return button
 
     def select_day(self, e):
         day_button = e.control
         day_date = day_button.data
         if not day_date:
-            return  # Ignore clicks on filler days
+            return
 
         if self.multi_select_mode:
             if day_date in self.selected_dates:
                 self.selected_dates.remove(day_date)
                 day_button.style.bgcolor = self.colors.default_day_background_color
                 day_button.style.color = self.colors.default_day_text_color
             else:
                 self.selected_dates.add(day_date)
                 day_button.style.bgcolor = self.colors.today_button_background_color
                 day_button.style.color = self.colors.today_text_color
         else:
-            # Clear previous selections
-            for btn in e.control.parent.controls:
-                if btn.data and btn.data in self.selected_dates:
-                    btn.style.bgcolor = self.colors.default_day_background_color
-            self.selected_dates = {day_date}
-            day_button.style.bgcolor = "#0D47A1"
+            for button in self.calendarpicker.content.controls[1].controls:
+                if (
+                    isinstance(button, ft.TextButton)
+                    and button.data in self.selected_dates
+                ):
+                    button.style.bgcolor = self.colors.default_day_background_color
+                    button.style.color = self.colors.default_day_text_color
+                    button.update()
+
+            self.selected_dates.clear()
+            self.selected_dates.add(day_date)
+            day_button.style.bgcolor = self.colors.today_button_background_color
+            day_button.style.color = self.colors.today_text_color
+
         day_button.update()
 
     def build_calendarpicker(self):
         def on_control_click(e):
             print(e.control)
 
+        if not self.left_content:
+            self.left_content = SecondaryButton(
+                height=40, width=130, on_click=self.__on_cancel
+            )
+
         self.calendarpicker = ft.Container(
             ft.Column(
                 [
                     ft.Row(
                         [
                             ft.IconButton(
                                 icon=ft.icons.ARROW_CIRCLE_LEFT_ROUNDED,
@@ -248,23 +273,24 @@
                             ),
                         ],
                         alignment=ft.MainAxisAlignment.SPACE_BETWEEN,
                     ),
                     self.build_calendar(),
                     ft.Row(
                         [
-                            Button(disabled=True, height=40, width=130),
+                            self.left_content,
                             Button(
                                 height=40,
                                 width=130,
                                 label="Choose Date",
                                 on_click=self.__on_selected_date,
                             ),
                         ],
                         spacing=10,
+                        alignment=ft.MainAxisAlignment.SPACE_BETWEEN,
                     ),
                 ],
                 spacing=2,
             ),
             padding=10,
             bgcolor=self.colors.container_background_color,
             border=ft.border.all(2, self.colors.container_border_color),
```

### Comparing `fletmint-0.1.3/fletmint/dropdown.py` & `fletmint-0.1.4/fletmint/dropdown.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/profile.py` & `fletmint-0.1.4/fletmint/profile.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/slider.py` & `fletmint-0.1.4/fletmint/slider.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/stepper.py` & `fletmint-0.1.4/fletmint/stepper.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/tab_switch.py` & `fletmint-0.1.4/fletmint/tab_switch.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/table.py` & `fletmint-0.1.4/fletmint/table.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/tags_input.py` & `fletmint-0.1.4/fletmint/tags_input.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/text_input.py` & `fletmint-0.1.4/fletmint/text_input.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/toggle.py` & `fletmint-0.1.4/fletmint/toggle.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/toggle_switch.py` & `fletmint-0.1.4/fletmint/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint/videoplayer.py` & `fletmint-0.1.4/fletmint/videoplayer.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/fletmint.egg-info/SOURCES.txt` & `fletmint-0.1.4/fletmint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.3/setup.py` & `fletmint-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 from os import path
 
+description = path.join(path.dirname(__file__), "description.md")
+
 setup(
     name="fletmint",
-    version="0.1.3",
+    version="0.1.4",
     author="Edoardo Balducci",
     author_email="edoardoba2004@gmail.com",
     description="A sharp and modern components library for Flet",
-    # long_description=long_description,
+    long_description=description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["flet"],
     python_requires=">=3.8",
     project_urls={
         "support": "https://www.patreon.com/edoardobalducci",
         "repository": "https://github.com/Bbalduzz/fletmint",
         "tracker": "https://github.com/Bbalduzz/fletmint/issues",
```

