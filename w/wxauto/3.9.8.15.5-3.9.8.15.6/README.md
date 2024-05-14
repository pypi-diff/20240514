# Comparing `tmp/wxauto-3.9.8.15.5.tar.gz` & `tmp/wxauto-3.9.8.15.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.5.tar", last modified: Tue Apr 23 06:26:23 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.6.tar", last modified: Tue May 14 06:00:52 2024, max compression
```

## Comparing `wxauto-3.9.8.15.5.tar` & `wxauto-3.9.8.15.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/
--rw-rw-rw-   0        0        0     3648 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/PKG-INFO
--rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/setup.cfg
--rw-rw-rw-   0        0        0      736 2024-04-23 06:26:16.000000 wxauto-3.9.8.15.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/wxauto/
--rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/color.py
--rw-rw-rw-   0        0        0    24361 2024-04-23 06:25:46.000000 wxauto-3.9.8.15.5/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/languages.py
--rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/utils.py
--rw-rw-rw-   0        0        0    26412 2024-04-22 02:27:46.000000 wxauto-3.9.8.15.5/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3648 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/
+-rw-rw-rw-   0        0        0     3698 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3333 2024-05-14 06:00:05.000000 wxauto-3.9.8.15.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-14 05:58:42.000000 wxauto-3.9.8.15.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto/
+-rw-rw-rw-   0        0        0      148 2024-05-14 04:47:09.000000 wxauto-3.9.8.15.6/wxauto/__init__.py
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/color.py
+-rw-rw-rw-   0        0        0    24759 2024-05-14 05:52:10.000000 wxauto-3.9.8.15.6/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.6/wxauto/languages.py
+-rw-rw-rw-   0        0        0   366752 2024-05-14 04:11:30.000000 wxauto-3.9.8.15.6/wxauto/uiautomation.py
+-rw-rw-rw-   0        0        0    10935 2024-05-14 05:18:00.000000 wxauto-3.9.8.15.6/wxauto/utils.py
+-rw-rw-rw-   0        0        0    29336 2024-05-14 05:36:01.000000 wxauto-3.9.8.15.6/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3698 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 06:00:52.000000 wxauto-3.9.8.15.6/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.5/PKG-INFO` & `wxauto-3.9.8.15.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.5
+Version: 3.9.8.15.6
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -12,14 +12,16 @@
 
 # wxauto  (适用PC微信3.9.8.15版本）
 
 ### 2023-11-20重写wxauto，欢迎指出bug，欢迎pull requests
 
 Windows版本微信客户端自动化，可实现简单的发送、接收微信消息、保存聊天图片
 
+项目地址：https://github.com/cluic/wxauto
+
 **相关版本安装包下载**：
 [OneDrive](https://1drv.ms/f/s!AqQw88ELOBiTgcAN_bBQlBaz60PTBg?e=oGoeju) |
 [百度云](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj)
 
 **文档**：
 [使用文档](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md) |
 [云服务器wxauto部署指南](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md#%E4%BA%94%E4%BA%91%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%83%A8%E7%BD%B2)
```

### Comparing `wxauto-3.9.8.15.5/README.md` & `wxauto-3.9.8.15.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # wxauto  (适用PC微信3.9.8.15版本）
 
 ### 2023-11-20重写wxauto，欢迎指出bug，欢迎pull requests
 
 Windows版本微信客户端自动化，可实现简单的发送、接收微信消息、保存聊天图片
 
+项目地址：https://github.com/cluic/wxauto
+
 **相关版本安装包下载**：
 [OneDrive](https://1drv.ms/f/s!AqQw88ELOBiTgcAN_bBQlBaz60PTBg?e=oGoeju) |
 [百度云](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj)
 
 **文档**：
 [使用文档](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md) |
 [云服务器wxauto部署指南](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md#%E4%BA%94%E4%BA%91%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%83%A8%E7%BD%B2)
```

### Comparing `wxauto-3.9.8.15.5/setup.py` & `wxauto-3.9.8.15.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.5',
+    version='3.9.8.15.6',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
-        'uiautomation',
         'pywin32',
         'pyperclip',
         'Pillow',
         'psutil',
         'typing_extensions',
+        'comtypes',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
     ],
     python_requires='>=3.6',
```

### Comparing `wxauto-3.9.8.15.5/wxauto/color.py` & `wxauto-3.9.8.15.6/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.5/wxauto/elements.py` & `wxauto-3.9.8.15.6/wxauto/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-import uiautomation as uia
+from . import uiautomation as uia
 from .languages import *
 from .utils import *
 from .color import *
 import datetime
 import time
 import os
 import re
 
+
+
 class WxParam:
     SYS_TEXT_HEIGHT = 33
     TIME_TEXT_HEIGHT = 34
     RECALL_TEXT_HEIGHT = 45
     CHAT_TEXT_HEIGHT = 52
     CHAT_IMG_HEIGHT = 117
+    DEFALUT_IMAGE_SAVEPATH = os.path.join(os.getcwd(), '微信图片')
 
 class WeChatBase:
     def _lang(self, text, langtype='MAIN'):
         if langtype == 'MAIN':
             return MAIN_LANGUAGE[text][self.language]
         elif langtype == 'WARNING':
             return WARNING[text][self.language]
@@ -137,14 +140,16 @@
             self.editbox.Click(simulateMove=False)
 
         self.editbox.SendKeys('@')
         atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
         if atwnd.Exists(maxSearchSeconds=0.1):
             atwnd.ListItemControl(Name='所有人').Click(simulateMove=False)
             if msg:
+                if not msg.startswith('\n'):
+                    msg = '\n' + msg
                 self.SendMsg(msg)
             else:
                 self.editbox.SendKeys('{Enter}')
 
     def SendMsg(self, msg, at=None):
         """发送文本消息
 
@@ -160,24 +165,24 @@
             if isinstance(at, str):
                 at = [at]
             for i in at:
                 self.editbox.SendKeys('@'+i)
                 atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
                 if atwnd.Exists(maxSearchSeconds=0.1):
                     atwnd.SendKeys('{ENTER}')
+                    if msg and not msg.startswith('\n'):
+                        msg = '\n' + msg
 
         t0 = time.time()
         while True:
             if time.time() - t0 > 10:
                 raise TimeoutError(f'发送消息超时 --> {self.who} - {msg}')
-            self.editbox.SetFocus()
-            time.sleep(0.1)
             SetClipboardText(msg)
             self.editbox.SendKeys('{Ctrl}v')
-            if self.editbox.GetValuePattern().Value.strip('￼'):
+            if self.editbox.GetValuePattern().Value:
                 break
         self.editbox.SendKeys('{Enter}')
 
     def SendFiles(self, filepath):
         """向当前聊天窗口发送文件
         
         Args:
@@ -317,14 +322,15 @@
         self.api = uia.WindowControl(ClassName='ImagePreviewWnd', searchDepth=1)
         MainControl1 = [i for i in self.api.GetChildren() if not i.ClassName][0]
         self.ToolsBox, self.PhotoBox = MainControl1.GetChildren()
         
         # tools按钮
         self.t_previous = self.ToolsBox.ButtonControl(Name=self._lang('上一张'))
         self.t_next = self.ToolsBox.ButtonControl(Name=self._lang('下一张'))
+        self.t_zoom = self.ToolsBox.ButtonControl(Name=self._lang('放大'))
         self.t_translate = self.ToolsBox.ButtonControl(Name=self._lang('翻译'))
         self.t_ocr = self.ToolsBox.ButtonControl(Name=self._lang('提取文字'))
         self.t_save = self.ToolsBox.ButtonControl(Name=self._lang('另存为...'))
         self.t_qrcode = self.ToolsBox.ButtonControl(Name=self._lang('识别图中二维码'))
 
     def __repr__(self) -> str:
         return f"<wxauto WeChat Image at {hex(id(self))}>"
@@ -357,20 +363,24 @@
         Args:
             savepath (str): 绝对路径，包括文件名和后缀，例如："D:/Images/微信图片_xxxxxx.jpg"
             （如果不填，则默认为当前脚本文件夹下，新建一个“微信图片”的文件夹，保存在该文件夹内）
         
         Returns:
             str: 文件保存路径，即savepath
         """
+        
         if not savepath:
-            savepath = os.path.join(os.getcwd(), '微信图片', f"微信图片_{datetime.datetime.now().strftime('%Y%m%d%H%M%S%f')}.jpg")
+            savepath = os.path.join(WxParam.DEFALUT_IMAGE_SAVEPATH, f"微信图片_{datetime.datetime.now().strftime('%Y%m%d%H%M%S%f')}.jpg")
         if not os.path.exists(os.path.split(savepath)[0]):
             os.makedirs(os.path.split(savepath)[0])
             
-        self.t_save.Click(simulateMove=False)
+        if self.t_zoom.Exists(maxSearchSeconds=5):
+            self.t_save.Click(simulateMove=False)
+        else:
+            raise TimeoutError('下载超时')
         t0 = time.time()
         while True:
             if time.time() - t0 > timeout:
                 raise TimeoutError('下载超时')
             handle = FindWindow(name='另存为...')
             if handle:
                 break
```

### Comparing `wxauto-3.9.8.15.5/wxauto/languages.py` & `wxauto-3.9.8.15.6/wxauto/languages.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.5/wxauto/utils.py` & `wxauto-3.9.8.15.6/wxauto/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from datetime import datetime, timedelta
+from . import uiautomation as uia
 from PIL import ImageGrab
 import win32clipboard
 import win32process
 import win32gui
 import win32api
 import win32con
 import pyperclip
-from ctypes import (
-    Structure,
-    c_uint,
-    c_long,
-    c_int,
-    c_bool,
-    sizeof
-)
+import ctypes
 import psutil
 import shutil
+import winreg
 import time
 import os
 import re
 
+VERSION = "3.9.8.15"
 
 def set_cursor_pos(x, y):
     win32api.SetCursorPos((x, y))
     
 def Click(rect):
     x = (rect.left + rect.right) // 2
     y = (rect.top + rect.bottom) // 2
@@ -54,25 +50,25 @@
 
 def IsRedPixel(uicontrol):
     rect = uicontrol.BoundingRectangle
     bbox = (rect.left, rect.top, rect.right, rect.bottom)
     img = ImageGrab.grab(bbox=bbox, all_screens=True)
     return any(p[0] > p[1] and p[0] > p[2] for p in img.getdata())
 
-class DROPFILES(Structure):
+class DROPFILES(ctypes.Structure):
     _fields_ = [
-    ("pFiles", c_uint),
-    ("x", c_long),
-    ("y", c_long),
-    ("fNC", c_int),
-    ("fWide", c_bool),
+    ("pFiles", ctypes.c_uint),
+    ("x", ctypes.c_long),
+    ("y", ctypes.c_long),
+    ("fNC", ctypes.c_int),
+    ("fWide", ctypes.c_bool),
     ]
 
 pDropFiles = DROPFILES()
-pDropFiles.pFiles = sizeof(DROPFILES)
+pDropFiles.pFiles = ctypes.sizeof(DROPFILES)
 pDropFiles.fWide = True
 matedata = bytes(pDropFiles)
 
 def SetClipboardText(text: str):
     pyperclip.copy(text)
     # if not isinstance(text, str):
     #     raise TypeError(f"参数类型必须为str --> {text}")
@@ -262,7 +258,60 @@
         target_day = datetime.now() - timedelta(days=delta_days)
         return target_day.strftime('%Y-%m-%d') + f' {hour}:{minute}'
 
     match = re.match(r'^(\d{4})年(\d{1,2})月(\d{1,2})日 (\d{1,2}):(\d{1,2})$', time_str)
     if match:
         year, month, day, hour, minute = match.groups()
         return datetime(*[int(i) for i in [year, month, day, hour, minute]]).strftime('%Y-%m-%d') + f' {hour}:{minute}'
+
+
+def FindPid(process_name):
+    procs = psutil.process_iter(['pid', 'name'])
+    for proc in procs:
+        if process_name in proc.info['name']:
+            return proc.info['pid']
+
+
+def Mver(pid):
+    exepath = psutil.Process(pid).exe()
+    if GetVersionByPath(exepath) != VERSION:
+        Warning(f"该修复方法仅适用于版本号为{VERSION}的微信！")
+        return
+    if not uia.Control(ClassName='WeChatLoginWndForPC', searchDepth=1).Exists(maxSearchSeconds=2):
+        Warning("请先打开微信启动页面再次尝试运行该方法！")
+        return
+    path = os.path.join(os.path.dirname(__file__), 'a.dll')
+    dll = ctypes.WinDLL(path)
+    dll.GetDllBaseAddress.argtypes = [ctypes.c_uint, ctypes.c_wchar_p]
+    dll.GetDllBaseAddress.restype = ctypes.c_void_p
+    dll.WriteMemory.argtypes = [ctypes.c_ulong, ctypes.c_void_p, ctypes.c_ulong]
+    dll.WriteMemory.restype = ctypes.c_bool
+    dll.GetMemory.argtypes = [ctypes.c_ulong, ctypes.c_void_p]
+    dll.GetMemory.restype = ctypes.c_ulong
+    mname = 'WeChatWin.dll'
+    tar = 1661536787
+    base_address = dll.GetDllBaseAddress(pid, mname)
+    address = base_address + 64761648
+    if dll.GetMemory(pid, address) != tar:
+        dll.WriteMemory(pid, address, tar)
+    handle = ctypes.c_void_p(dll._handle)
+    ctypes.windll.kernel32.FreeLibrary(handle)
+
+def FixVersionError():
+    """修复版本低无法登录的问题"""
+    pid = FindPid('WeChat.exe')
+    if pid:
+        Mver(pid)
+        return
+    else:
+        try:
+            registry_key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Tencent\WeChat", 0, winreg.KEY_READ)
+            path, _ = winreg.QueryValueEx(registry_key, "InstallPath")
+            winreg.CloseKey(registry_key)
+            wxpath = os.path.join(path, "WeChat.exe")
+            if os.path.exists(wxpath):
+                os.system(f'start "" "{wxpath}"')
+                FixVersionError()
+            else:
+                raise Exception('nof found')
+        except WindowsError:
+            Warning("未找到微信安装路径，请先打开微信启动页面再次尝试运行该方法！")
```

### Comparing `wxauto-3.9.8.15.5/wxauto/wxauto.py` & `wxauto-3.9.8.15.6/wxauto/wxauto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Author: Cluic
-Update: 2024-04-21
-Version: 3.9.8.15.3
+Update: 2024-05-14
+Version: 3.9.8.15.6
 """
 
-import uiautomation as uia
+from . import uiautomation as uia
 from .languages import *
 from .utils import *
 from .elements import *
 from .errors import *
 from .color import *
-import datetime
 import time
 import os
 import re
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
@@ -70,14 +69,15 @@
         self.HWND = FindWindow(classname='WeChatMainWndForPC')
         wxpath = GetPathByHwnd(self.HWND)
         wxversion = GetVersionByPath(wxpath)
         if wxversion != self.VERSION:
             Warnings.lightred(self._lang('版本不一致', 'WARNING').format(wxversion, self.VERSION), stacklevel=2)
             return False
     
+    
     def _show(self):
         self.HWND = FindWindow(classname='WeChatMainWndForPC')
         win32gui.ShowWindow(self.HWND, 1)
         win32gui.SetWindowPos(self.HWND, -1, 0, 0, 0, 0, 3)
         win32gui.SetWindowPos(self.HWND, -2, 0, 0, 0, 0, 3)
         self.UiaAPI.SwitchToThisWindow()
     
@@ -210,16 +210,18 @@
         self.B_Search.SendKeys(who, waitTime=1.5)
         SearchResut = self.SessionBox.GetChildren()[1].GetChildren()[1]
         firstresult = [i for i in SearchResut.GetChildren()[0].GetChildren() if who in i.Name][0]
         if firstresult.Name == f'搜索 {who}':
             if len(self.SessionBox.GetChildren()[1].GetChildren()) > 1:
                 self.B_Search.SendKeys('{Esc}')
             if notfound == 'raise':
+                self.B_Search.SendKeys('{Esc}')
                 raise TargetNotFoundError(f'未查询到目标：{who}')
             elif notfound == 'ignore':
+                self.B_Search.SendKeys('{Esc}')
                 return None
         chatname = firstresult.Name
         firstresult.Click(simulateMove=False)
         return chatname
     
     def AtAll(self, msg=None, who=None):
         """@所有人
@@ -248,15 +250,17 @@
         else:
             editbox = self.ChatBox.EditControl(searchDepth=10)
         editbox.SendKeys('@')
         atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
         if atwnd.Exists(maxSearchSeconds=0.1):
             atwnd.ListItemControl(Name='所有人').Click(simulateMove=False)
             if msg:
-                self.SendMsg(msg, clear=False)
+                if not msg.startswith('\n'):
+                    msg = '\n' + msg
+                self.SendMsg(msg, who=who, clear=False)
             else:
                 editbox.SendKeys('{Enter}')
 
     def SendMsg(self, msg, who=None, clear=True, at=None):
         """发送文本消息
 
         Args:
@@ -294,25 +298,25 @@
             if isinstance(at, str):
                 at = [at]
             for i in at:
                 editbox.SendKeys('@'+i)
                 atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
                 if atwnd.Exists(maxSearchSeconds=0.1):
                     atwnd.SendKeys('{ENTER}')
+                    if msg and not msg.startswith('\n'):
+                        msg = '\n' + msg
 
         if msg:
             t0 = time.time()
             while True:
                 if time.time() - t0 > 10:
                     raise TimeoutError(f'发送消息超时 --> {editbox.Name} - {msg}')
-                editbox.SetFocus()
-                time.sleep(0.1)
                 SetClipboardText(msg)
                 editbox.SendKeys('{Ctrl}v')
-                if editbox.GetValuePattern().Value.strip('￼'):
+                if editbox.GetValuePattern().Value:
                     break
         editbox.SendKeys('{Enter}')
         
     def SendFiles(self, filepath, who=None):
         """向当前聊天窗口发送文件
         
         Args:
@@ -551,14 +555,71 @@
     
     def RemoveListenChat(self, who):
         """移除监听对象"""
         if who in self.listen:
             del self.listen[who]
         else:
             Warnings.lightred(f'未找到监听对象：{who}', stacklevel=2)
+
+    def AddNewFriend(self, keywords, addmsg=None, remark=None, tags=None):
+        """添加新的好友
+
+        Args:
+            keywords (str): 搜索关键词，微信号、手机号、QQ号
+            addmsg (str, optional): 添加好友的消息
+            remark (str, optional): 备注名
+            tags (list, optional): 标签列表
+
+        Example:
+            >>> wx = WeChat()
+            >>> keywords = '13800000000'      # 微信号、手机号、QQ号
+            >>> addmsg = '你好，我是xxxx'      # 添加好友的消息
+            >>> remark = '备注名字'            # 备注名
+            >>> tags = ['朋友', '同事']        # 标签列表
+            >>> wx.AddNewFriend(keywords, addmsg=addmsg, remark=remark, tags=tags)
+        """
+        self._show()
+        self.SwitchToContact()
+        self.SessionBox.ButtonControl(Name='添加朋友').Click(simulateMove=False)
+        edit = self.SessionBox.EditControl(Name='微信号/手机号')
+        edit.Click(simulateMove=False)
+        edit.SendKeys(keywords)
+        self.SessionBox.TextControl(Name=f'搜索：{keywords}').Click(simulateMove=False)
+
+        ContactProfileWnd = uia.PaneControl(ClassName='ContactProfileWnd')
+        if ContactProfileWnd.Exists(maxSearchSeconds=2):
+            # 点击添加到通讯录
+            ContactProfileWnd.ButtonControl(Name='添加到通讯录').Click(simulateMove=False)
+        else:
+            print('未找到联系人')
+            return False
+
+        NewFriendsWnd = self.UiaAPI.WindowControl(ClassName='WeUIDialog')
+        if NewFriendsWnd.Exists(maxSearchSeconds=2):
+            if addmsg:
+                msgedit = NewFriendsWnd.TextControl(Name="发送添加朋友申请").GetParentControl().EditControl()
+                msgedit.Click(simulateMove=False)
+                msgedit.SendKeys('{Ctrl}a', waitTime=0)
+                msgedit.SendKeys(addmsg)
+
+            if remark:
+                remarkedit = NewFriendsWnd.TextControl(Name='备注名').GetParentControl().EditControl()
+                remarkedit.Click(simulateMove=False)
+                remarkedit.SendKeys('{Ctrl}a', waitTime=0)
+                remarkedit.SendKeys(remark)
+
+            if tags:
+                tagedit = NewFriendsWnd.TextControl(Name='标签').GetParentControl().EditControl()
+                for tag in tags:
+                    tagedit.Click(simulateMove=False)
+                    tagedit.SendKeys(tag)
+                    NewFriendsWnd.PaneControl(ClassName='DropdownWindow').TextControl().Click(simulateMove=False)
+
+            NewFriendsWnd.ButtonControl(Name='确定').Click(simulateMove=False)
+        return True
     
 class WeChatFiles:
     def __init__(self, language='cn') -> None:
         self.language = language
         self.api = uia.WindowControl(ClassName='FileListMgrWnd', searchDepth=1)
         MainControl3 = [i for i in self.api.GetChildren() if not i.ClassName][0]
         self.FileBox ,self.Search ,self.SessionBox = MainControl3.GetChildren()
```

### Comparing `wxauto-3.9.8.15.5/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.6/wxauto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.5
+Version: 3.9.8.15.6
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -12,14 +12,16 @@
 
 # wxauto  (适用PC微信3.9.8.15版本）
 
 ### 2023-11-20重写wxauto，欢迎指出bug，欢迎pull requests
 
 Windows版本微信客户端自动化，可实现简单的发送、接收微信消息、保存聊天图片
 
+项目地址：https://github.com/cluic/wxauto
+
 **相关版本安装包下载**：
 [OneDrive](https://1drv.ms/f/s!AqQw88ELOBiTgcAN_bBQlBaz60PTBg?e=oGoeju) |
 [百度云](https://pan.baidu.com/s/1FvSw0Fk54GGvmQq8xSrNjA?pwd=vsmj)
 
 **文档**：
 [使用文档](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md) |
 [云服务器wxauto部署指南](https://github.com/cluic/wxauto/blob/WeChat3.9.8/%E4%BD%BF%E7%94%A8%E6%96%87%E6%A1%A3.md#%E4%BA%94%E4%BA%91%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%83%A8%E7%BD%B2)
```

