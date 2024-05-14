# Comparing `tmp/elia_chat-1.3.0.tar.gz` & `tmp/elia_chat-1.4.0.tar.gz`

## Comparing `elia_chat-1.3.0.tar` & `elia_chat-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.python-version
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.3.0/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/__main__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/app.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/config.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/constants.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/locations.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/models.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/models.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.gitignore
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elia_chat-1.3.0/README.md
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 elia_chat-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.4.0/.python-version
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.4.0/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.4.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.4.0/.gitignore
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elia_chat-1.4.0/README.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 elia_chat-1.4.0/PKG-INFO
```

### Comparing `elia_chat-1.3.0/.pre-commit-config.yaml` & `elia_chat-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/requirements-dev.lock` & `elia_chat-1.4.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/requirements.lock` & `elia_chat-1.4.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/__main__.py` & `elia_chat-1.4.0/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/app.py` & `elia_chat-1.4.0/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/chats_manager.py` & `elia_chat-1.4.0/elia_chat/chats_manager.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/config.py` & `elia_chat-1.4.0/elia_chat/config.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/elia.scss` & `elia_chat-1.4.0/elia_chat/elia.scss`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/locations.py` & `elia_chat-1.4.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/models.py` & `elia_chat-1.4.0/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/time_display.py` & `elia_chat-1.4.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/database/converters.py` & `elia_chat-1.4.0/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/database/database.py` & `elia_chat-1.4.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/database/import_chatgpt.py` & `elia_chat-1.4.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/database/models.py` & `elia_chat-1.4.0/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/screens/chat_details.py` & `elia_chat-1.4.0/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/screens/chat_screen.py` & `elia_chat-1.4.0/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/screens/help_screen.py` & `elia_chat-1.4.0/elia_chat/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/screens/home_screen.py` & `elia_chat-1.4.0/elia_chat/screens/home_screen.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     @on(ChatList.ChatOpened)
     async def open_chat_screen(self, event: ChatList.ChatOpened):
         chat_id = event.chat.id
         assert chat_id is not None
         chat = await self.chats_manager.get_chat(chat_id)
         await self.app.push_screen(ChatScreen(chat))
 
+    @on(ChatList.CursorEscapingTop)
+    def cursor_escaping_top(self):
+        self.query_one(HomePromptInput).focus()
+
     @on(PromptInput.PromptSubmitted)
     async def create_new_chat(self, event: PromptInput.PromptSubmitted) -> None:
         text = event.text
         await self.elia.launch_chat(  # type: ignore
             prompt=text,
             model=self.elia.runtime_config.selected_model,
         )
```

### Comparing `elia_chat-1.3.0/elia_chat/widgets/app_header.py` & `elia_chat-1.4.0/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/widgets/chat.py` & `elia_chat-1.4.0/elia_chat/widgets/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,18 @@
             user_message = event.text
             await self.new_user_message(user_message)
 
     @on(PromptInput.CursorEscapingTop)
     async def on_cursor_up_from_prompt(self) -> None:
         self.focus_latest_message()
 
+    @on(Chatbox.CursorEscapingBottom)
+    def move_focus_to_prompt(self) -> None:
+        self.query_one(ChatPromptInput).focus()
+
     def get_latest_chatbox(self) -> Chatbox:
         return self.query(Chatbox).last()
 
     def focus_latest_message(self) -> None:
         try:
             self.get_latest_chatbox().focus()
         except NoMatches:
```

### Comparing `elia_chat-1.3.0/elia_chat/widgets/chat_header.py` & `elia_chat-1.4.0/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/widgets/chat_list.py` & `elia_chat-1.4.0/elia_chat/widgets/chat_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,31 @@
 class ChatList(OptionList):
     BINDINGS = [
         Binding(
             "escape", "screen.focus('home-prompt')", "Focus prompt", key_display="esc"
         ),
         Binding("j,down", "cursor_down", "Down", show=False),
         Binding("k,up", "cursor_up", "Up", show=False),
-        Binding("G,end", "last", "Last", show=False),
-        Binding("l,enter", "select", "Select", show=False),
+        Binding("l,right,enter", "select", "Select", show=False),
         Binding("g,home", "first", "First", show=False),
+        Binding("G,end", "last", "Last", show=False),
         Binding("pagedown", "page_down", "Page Down", show=False),
         Binding("pageup", "page_up", "Page Up", show=False),
     ]
 
     @dataclass
     class ChatOpened(Message):
         chat: ChatData
 
+    class CursorEscapingTop(Message):
+        """Cursor attempting to move out-of-bounds at top of list."""
+
+    class CursorEscapingBottom(Message):
+        """Cursor attempting to move out-of-bounds at bottom of list."""
+
     async def on_mount(self) -> None:
         await self.reload_and_refresh()
 
     @on(OptionList.OptionSelected)
     async def post_chat_opened(self, event: OptionList.OptionSelected) -> None:
         assert isinstance(event.option, ChatListItem)
         chat = event.option.chat
@@ -127,7 +133,13 @@
             new_chat_list_item,
             *self.options,
         ]
         option_list.clear_options()
         option_list.add_options(self.options)
         option_list.highlighted = 0
         self.refresh()
+
+    def action_cursor_up(self) -> None:
+        if self.highlighted == 0:
+            self.post_message(self.CursorEscapingTop())
+        else:
+            return super().action_cursor_up()
```

### Comparing `elia_chat-1.3.0/elia_chat/widgets/chat_options.py` & `elia_chat-1.4.0/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/widgets/chatbox.py` & `elia_chat-1.4.0/elia_chat/widgets/chatbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,17 @@
             key="escape",
             action="screen.focus('prompt')",
             description="Focus prompt",
             key_display="esc",
         ),
     ]
 
+    class CursorEscapingBottom(Message):
+        """Sent when the cursor moves down from the bottom message."""
+
     selection_mode = reactive(False, init=False)
 
     def __init__(
         self,
         message: ChatMessage,
         model: EliaChatModel,
         name: str | None = None,
@@ -181,15 +184,18 @@
             self.add_class("human-message")
             self.border_title = "You"
 
     def action_up(self) -> None:
         self.screen.focus_previous(Chatbox)
 
     def action_down(self) -> None:
-        self.screen.focus_next(Chatbox)
+        if self.parent and self is self.parent.children[-1]:
+            self.post_message(self.CursorEscapingBottom())
+        else:
+            self.screen.focus_next(Chatbox)
 
     def action_select(self) -> None:
         self.selection_mode = not self.selection_mode
         self.set_class(self.selection_mode, "selecting")
 
     def action_copy_to_clipboard(self) -> None:
         if not self.selection_mode:
```

### Comparing `elia_chat-1.3.0/elia_chat/widgets/prompt_input.py` & `elia_chat-1.4.0/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/elia_chat/widgets/token_analysis.py` & `elia_chat-1.4.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/.gitignore` & `elia_chat-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/README.md` & `elia_chat-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `elia_chat-1.3.0/pyproject.toml` & `elia_chat-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.3.0"
+version = "1.4.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.3.0/PKG-INFO` & `elia_chat-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.3.0
+Version: 1.4.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: greenlet>=3.0.3
```

