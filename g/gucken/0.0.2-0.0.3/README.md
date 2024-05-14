# Comparing `tmp/gucken-0.0.2.tar.gz` & `tmp/gucken-0.0.3.tar.gz`

## Comparing `gucken-0.0.2.tar` & `gucken-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/__main__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/aniskip.py
--rw-r--r--   0        0        0    22807 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/gucken.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/gucken.tcss
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/android.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/common.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/mpv.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.2/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gucken-0.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 gucken-0.0.2/README.md
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 gucken-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 gucken-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/aniskip.py
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/gucken.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/gucken.tcss
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/android.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/common.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gucken-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 gucken-0.0.3/README.md
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 gucken-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 gucken-0.0.3/PKG-INFO
```

### Comparing `gucken-0.0.2/src/gucken/aniskip.py` & `gucken-0.0.3/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/gucken.py` & `gucken-0.0.3/src/gucken/gucken.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 import sys
 from atexit import register as register_atexit
 from asyncio import gather
 from os import name as os_name, getenv, remove
 from os.path import join
 from pathlib import Path
@@ -11,88 +10,118 @@
 from subprocess import PIPE, Popen, DEVNULL
 from time import sleep, time
 from typing import Union
 
 from pypresence import AioPresence, DiscordNotFound
 from textual import events, on, work
 from textual.app import App, ComposeResult
-from textual.containers import (Center, Container, Horizontal,
-                                ScrollableContainer)
+from textual.containers import Center, Container, Horizontal, ScrollableContainer
 from textual.reactive import reactive
 from textual.screen import ModalScreen
-from textual.widgets import (Button, Checkbox, DataTable, Footer, Header,
-                             Input, Label, ListItem, ListView, Markdown,
-                             RadioButton, TabbedContent, TabPane)
+from textual.widgets import (
+    Button,
+    Checkbox,
+    DataTable,
+    Footer,
+    Header,
+    Input,
+    Label,
+    ListItem,
+    ListView,
+    Markdown,
+    RadioButton,
+    TabbedContent,
+    TabPane,
+)
 
 from .update import check
-from .aniskip import (get_timings_from_search, timings_to_mpv_options, generate_chapters_file,
-                      get_chapters_file_mpv_option)
+from .aniskip import (
+    get_timings_from_search,
+    timings_to_mpv_options,
+    generate_chapters_file,
+    get_chapters_file_mpv_option,
+)
 from .hoster.common import DirectLink, Hoster
 from .hoster.doodstream import DoodstreamHoster
 from .hoster.streamtape import StreamtapeHoster
 from .hoster.veo import VOEHoster
 from .hoster.vidoza import VidozaHoster
-from .player.android import (AndroidChoosePlayer, AndroidMPVPlayer,
-                             AndroidVLCPlayer)
+from .player.android import AndroidChoosePlayer, AndroidMPVPlayer, AndroidVLCPlayer
 from .player.common import Player
 from .player.ffplay import FFPlayPlayer
-from .player.mpv import MPVPlayer, MPV_NETPlayer, CelluloidPlayer
+from .player.mpv import MPVPlayer, MPVNETPlayer, CelluloidPlayer
 from .player.vlc import VLCPlayer
 from .player.wmplayer import WMPlayer
 from .player.flatpak import FlatpakMPVPlayer, FlatpakVLCPlayer, FlatpakCelluloidPlayer
 from .provider.aniworld import AniWorldProvider
 from .provider.common import Episode, Language, SearchResult, Series
 from .provider.serienstream import SerienStreamProvider
 
 # TODO: fix this mess
 logs_path = Path(__file__).parent.parent.parent.joinpath("logs")
 logs_path.mkdir(exist_ok=True, parents=True)
-logging.basicConfig(filename=logs_path.joinpath("gucken.log"), encoding='utf-8', level=logging.INFO)
+logging.basicConfig(
+    filename=logs_path.joinpath("gucken.log"), encoding="utf-8", level=logging.INFO
+)
 
 
 def detect_player() -> Union[Player, None]:
-    if hasattr(sys, 'getandroidapilevel'):
+    if hasattr(sys, "getandroidapilevel"):
         # TODO: detect right
         return AndroidMPVPlayer()
         # return AndroidVLCPlayer()
         # return AndroidChoosePlayer()
         # return None
 
     if os_name == "nt":
         if which("mpv.exe"):
             return MPVPlayer("mpv.exe")
     elif which("mpv"):
         return MPVPlayer()
 
     if os_name == "nt":
         if which("mpvnet.exe"):
-            return MPV_NETPlayer()
+            return MPVNETPlayer()
         if getenv("LOCALAPPDATA"):
             mpvnet = join(getenv("LOCALAPPDATA"), "Programs", "mpv.net", "mpvnet.exe")
             if which(mpvnet):
-                return MPV_NETPlayer(mpvnet)
+                return MPVNETPlayer(mpvnet)
 
     if os_name == "posix":
         if which("celluloid"):
             return CelluloidPlayer()
 
     if which("vlc"):
         return VLCPlayer()
 
     if os_name == "posix":
         # TODO: fix this will slow down
         if which("flatpak"):
-            p = Popen(["flatpak", "info", "io.mpv.Mpv"], stdout=DEVNULL, stderr=DEVNULL, stdin=DEVNULL)
+            p = Popen(
+                ["flatpak", "info", "io.mpv.Mpv"],
+                stdout=DEVNULL,
+                stderr=DEVNULL,
+                stdin=DEVNULL,
+            )
             if p.wait() == 0:
                 return FlatpakMPVPlayer()
-            p = Popen(["flatpak", "info", "io.github.celluloid_player.Celluloid"], stdout=DEVNULL, stderr=DEVNULL,
-                      stdin=DEVNULL)
+            p = Popen(
+                ["flatpak", "info", "io.github.celluloid_player.Celluloid"],
+                stdout=DEVNULL,
+                stderr=DEVNULL,
+                stdin=DEVNULL,
+            )
             if p.wait() == 0:
                 return FlatpakCelluloidPlayer()
-            p = Popen(["flatpak", "info", "org.videolan.VLC"], stdout=DEVNULL, stderr=DEVNULL, stdin=DEVNULL)
+            p = Popen(
+                ["flatpak", "info", "org.videolan.VLC"],
+                stdout=DEVNULL,
+                stderr=DEVNULL,
+                stdin=DEVNULL,
+            )
             if p.wait() == 0:
                 return FlatpakVLCPlayer()
 
     if os_name == "nt":
         vlc = r"C:\Program Files\VideoLAN\VLC\vlc.exe"
         if which(vlc):
             return VLCPlayer(vlc)
@@ -103,35 +132,46 @@
     if os_name == "nt":
         return WMPlayer()
 
     return None
 
 
 def sort_favorite_lang(language_list: list[Language]) -> list[Language]:
-    return sorted(language_list, key=lambda x: (
-        x != Language.DE,
-        x != Language.JP_DESUB,
-        x != Language.JP_ENSUB,
-    ))
+    return sorted(
+        language_list,
+        key=lambda x: (
+            x != Language.DE,
+            x != Language.JP_DESUB,
+            x != Language.JP_ENSUB,
+        ),
+    )
 
 
 def sort_favorite_hoster(hoster_list: list[Hoster]) -> list[Hoster]:
-    return sorted(hoster_list, key=lambda x: (
-        not isinstance(x, StreamtapeHoster),
-        not isinstance(x, VOEHoster),
-        not isinstance(x, VidozaHoster),
-        not isinstance(x, DoodstreamHoster),
-    ))
+    return sorted(
+        hoster_list,
+        key=lambda x: (
+            not isinstance(x, StreamtapeHoster),
+            not isinstance(x, VOEHoster),
+            not isinstance(x, VidozaHoster),
+            not isinstance(x, DoodstreamHoster),
+        ),
+    )
 
 
 async def get_working_direct_link(hosters: list[Hoster]) -> Union[DirectLink, None]:
     for hoster in hosters:
         direct_link = await hoster.get_direct_link()
         is_working = await direct_link.check_is_working()
-        logging.info('Check: "%s" Working: "%s" URL: "%s"', type(hoster).__name__, is_working, direct_link)
+        logging.info(
+            'Check: "%s" Working: "%s" URL: "%s"',
+            type(hoster).__name__,
+            is_working,
+            direct_link,
+        )
         if is_working:
             return direct_link
     return None
 
 
 class Next(ModalScreen):
     time = reactive(3)
@@ -268,15 +308,15 @@
         except DiscordNotFound:
             pass
 
     async def disable_RPC(self):
         if self.RPC is not None:
             await self.RPC.clear()
             # close without closing event loop
-            self.RPC.send_data(2, {'v': 1, 'client_id': self.RPC.client_id})
+            self.RPC.send_data(2, {"v": 1, "client_id": self.RPC.client_id})
             self.RPC.sock_writer.close()
             self.RPC = None
 
     async def on_checkbox_changed(self):
         self.lookup_anime(self.query_one("#input", Input).value)
 
     async def on_radio_button_changed(self, event: RadioButton.Changed):
@@ -286,14 +326,15 @@
             else:
                 await self.disable_RPC()
 
     async def on_input_changed(self, message: Input.Changed) -> None:
         if message.value:
             self.lookup_anime(message.value)
         else:
+            # TODO: fix sometimes wont clear
             await self.query_one("#results", ListView).clear()
 
     # TODO: https://textual.textualize.io/guide/workers/#thread-workers
     @work(exclusive=True)
     async def lookup_anime(self, keyword: str) -> None:
         search_providers = []
         if self.query_one("#aniworld_to", Checkbox).value:
@@ -312,24 +353,27 @@
                 for e in l:
                     final_results.append(e)
 
         # TODO: Sort final_results with fuzzy-sort
         if len(final_results) > 0:
             self.current = final_results
             for series in final_results:
+                # TODO: show provider
                 await results_list_view.append(ClickableListItem(Markdown(
                     f"##### **{series.name}** {series.production_year}\n{series.description}"
                 )))
         results_list_view.loading = False
         if len(final_results) > 0:
+
             def select_first_index():
                 try:
                     results_list_view.index = 0
                 except AssertionError:
                     pass
+
             self.app.call_later(select_first_index)
 
     async def on_key(self, event: events.Key) -> None:
         key = event.key
         if self.screen.id == "_default":
             if self.query_one(TabbedContent).active == "search":
                 lv = self.query_one("#results", ListView)
@@ -360,19 +404,15 @@
     @work(exclusive=True)
     async def play_selected(self):
         dt = self.query_one(DataTable)
         # TODO: show loading
         dt.loading = True
         index = self.app.query_one("#results", ListView).index
         series_search_result = self.current[index]
-        self.play(
-            series_search_result=series_search_result,
-            episodes=self.current_info.episodes,
-            index=dt.cursor_row
-        )
+        self.play(series_search_result=series_search_result, episodes=self.current_info.episodes, index=dt.cursor_row)
         dt.loading = False
 
     @work(exclusive=True)
     async def open_info(self) -> None:
         series_search_result: SearchResult = self.current[self.app.query_one("#results", ListView).index]
         info_tab = self.query_one("#info", TabPane)
         info_tab.disabled = False
@@ -463,21 +503,21 @@
 
         title = f"{series_search_result.name} - {episode.title}"
         args = self.player.play(direct_link.url, title, fullscreen, direct_link.headers)
 
         if self.RPC and self.RPC.sock_writer:
             async def update():
                 await self.RPC.update(
-                    #state="00:20:00 / 00:25:00 57% complete",
+                    # state="00:20:00 / 00:25:00 57% complete",
                     details=title[:128],
                     large_text=title,
                     large_image=series_search_result.cover,
                     # small_image as playing or stopped ?
-                    #small_image="https://jooinn.com/images/lonely-tree-reflection-3.jpg",
-                    #small_text="ff 15",
+                    # small_image="https://jooinn.com/images/lonely-tree-reflection-3.jpg",
+                    # small_text="ff 15",
                     # start=time.time(), # for paused
                     # end=time.time() + timedelta(minutes=20).seconds   # for time left
                 )
 
             self.app.call_later(update)
 
         chapters_file = None
@@ -530,20 +570,15 @@
                     self.notify(
                         "Your player is not supported by Syncplay",
                         title="Player not supported",
                         severity="warning",
                     )
 
         logging.info("Running: %s", args)
-        process = Popen(
-            args,
-            stderr=PIPE,
-            stdout=DEVNULL,
-            stdin=DEVNULL
-        )
+        process = Popen(args, stderr=PIPE, stdout=DEVNULL, stdin=DEVNULL)
         while not self.app._exit:
             sleep(0.1)
 
             resume_time = None
 
             # only if mpv
             while not self.app._exit:
```

### Comparing `gucken-0.0.2/src/gucken/gucken.tcss` & `gucken-0.0.3/src/gucken/gucken.tcss`

 * *Files 26% similar despite different names*

```diff
@@ -44,8 +44,12 @@
 TabbedContent #--content-tab-setting {
     dock: right;
     margin-right: 1;
 }
 
 #setting > RadioButton {
     margin-bottom: 1;
-}
+}
+
+ClickableListItem {
+    padding-bottom: -1;
+}
```

### Comparing `gucken-0.0.2/src/gucken/update.py` & `gucken-0.0.3/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/hoster/common.py` & `gucken-0.0.3/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/hoster/doodstream.py` & `gucken-0.0.3/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/hoster/streamtape.py` & `gucken-0.0.3/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/hoster/veo.py` & `gucken-0.0.3/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/hoster/vidoza.py` & `gucken-0.0.3/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/player/android.py` & `gucken-0.0.3/src/gucken/player/android.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-from dataclasses import dataclass
-
 from .common import Player
 
 
-@dataclass
 class AndroidChoosePlayer(Player):
-    supports_headers = False
-
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
             override_executable: str = None
@@ -26,18 +21,15 @@
             url,
             "-c",
             "android.intent.category.BROWSABLE"
         ]
 
 
 # http://mpv-android.github.io/mpv-android/intent.html
-@dataclass
 class AndroidMPVPlayer(Player):
-    supports_headers = False
-
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
             override_executable: str = None
@@ -53,18 +45,15 @@
             url,
             "-n",
             "is.xyz.mpv/.MPVActivity"
         ]
 
 
 # https://wiki.videolan.org/Android_Player_Intents/
-@dataclass
 class AndroidVLCPlayer(Player):
-    supports_headers = False
-
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
             override_executable: str = None
```

### Comparing `gucken-0.0.2/src/gucken/player/common.py` & `gucken-0.0.3/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/player/ffplay.py` & `gucken-0.0.3/src/gucken/player/ffplay.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 
 from .common import Player, dict_to_string
 
 
 @dataclass
 class FFPlayPlayer(Player):
-    executable = "ffplay"
-    supports_headers = True
+    executable: str = "ffplay"
+    supports_headers: bool = True
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
```

### Comparing `gucken-0.0.2/src/gucken/player/flatpak.py` & `gucken-0.0.3/src/gucken/player/flatpak.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .mpv import MPVPlayer, CelluloidPlayer
 from .vlc import VLCPlayer
 
 
 @dataclass
 class FlatpakMPVPlayer(MPVPlayer):
-    executable = None
+    executable: str = None
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
@@ -24,15 +24,15 @@
         )
         uf_args.pop(0)
         return ["flatpak", "run", "io.mpv.Mpv"] + uf_args
 
 
 @dataclass
 class FlatpakCelluloidPlayer(CelluloidPlayer):
-    executable = None
+    executable: str = None
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
@@ -46,15 +46,15 @@
         )
         uf_args.pop(0)
         return ["flatpak", "run", "io.github.celluloid_player.Celluloid"] + uf_args
 
 
 @dataclass
 class FlatpakVLCPlayer(VLCPlayer):
-    executable = None
+    executable: str = None
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
```

### Comparing `gucken-0.0.2/src/gucken/player/mpv.py` & `gucken-0.0.3/src/gucken/player/mpv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .common import Player, dict_to_string
 from dataclasses import dataclass
 
 
 @dataclass
 class MPVPlayer(Player):
-    executable = "mpv"
-    supports_headers = True
+    executable: str = "mpv"
+    supports_headers: bool = True
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
@@ -25,16 +25,16 @@
             args.append(f"--force-media-title={title}")
         if headers:
             args.append(f"--http-header-fields={dict_to_string(headers)}")
         return args
 
 
 @dataclass
-class MPV_NETPlayer(MPVPlayer):
-    executable = "mpvnet"
+class MPVNETPlayer(MPVPlayer):
+    executable: str = "mpvnet"
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
@@ -47,15 +47,15 @@
             headers,
             override_executable or self.executable
         ) + ["--process-instance=multi"]
 
 
 @dataclass
 class CelluloidPlayer(MPVPlayer):
-    executable = "celluloid"
+    executable: str = "celluloid"
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
```

### Comparing `gucken-0.0.2/src/gucken/player/vlc.py` & `gucken-0.0.3/src/gucken/player/vlc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 
 from .common import Player
 
 
 @dataclass
 class VLCPlayer(Player):
-    executable = "vlc"
+    executable: str = "vlc"
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
```

### Comparing `gucken-0.0.2/src/gucken/player/wmplayer.py` & `gucken-0.0.3/src/gucken/player/wmplayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 
 from .common import Player
 
 
 @dataclass
 class WMPlayer(Player):
-    executable = r"C:\Program Files (x86)\Windows Media Player\wmplayer.exe"
+    executable: str = r"C:\Program Files (x86)\Windows Media Player\wmplayer.exe"
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
```

### Comparing `gucken-0.0.2/src/gucken/provider/aniworld.py` & `gucken-0.0.3/src/gucken/provider/aniworld.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     @property
     def url(self) -> str:
         return f"https://{self.host}/anime/stream/{self.link}"
 
 
 @dataclass
 class AniWorldProvider(Provider):
-    host = "aniworld.to"
+    host: str = "aniworld.to"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[AniWorldSearchResult], None]:
         if keyword.strip() == "":
             return None
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"https://{AniWorldProvider.host}/ajax/seriesSearch?keyword={keyword}")
```

### Comparing `gucken-0.0.2/src/gucken/provider/common.py` & `gucken-0.0.3/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/src/gucken/provider/serienstream.py` & `gucken-0.0.3/src/gucken/provider/serienstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     @property
     def url(self) -> str:
         return f"https://{self.host}/serie/stream/{self.link}"
 
 
 @dataclass
 class SerienStreamProvider(Provider):
-    host = "186.2.175.5"
+    host: str = "186.2.175.5"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[SerienStreamSearchResult], None]:
         if keyword.strip() == "":
             return None
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"https://{SerienStreamProvider.host}/ajax/seriesSearch?keyword={keyword}")
```

### Comparing `gucken-0.0.2/src/gucken/tracker/anilist.py` & `gucken-0.0.3/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/LICENSE.txt` & `gucken-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/README.md` & `gucken-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/pyproject.toml` & `gucken-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.0.2/PKG-INFO` & `gucken-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
```

