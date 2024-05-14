# Comparing `tmp/tdrpa.tdworker-1.1.4.6-py3-none-any.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 421551 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1178112 b- defN 24-May-12 20:30 tdrpa/tdworker.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat    15621 b- defN 24-May-06 14:11 tdrpa/tdworker/WinElement.pyi
--rw-rw-rw-  2.0 fat     4815 b- defN 24-May-06 06:22 tdrpa/tdworker/WinKeyboard.pyi
--rw-rw-rw-  2.0 fat     6966 b- defN 24-May-06 06:18 tdrpa/tdworker/WinMouse.pyi
--rw-rw-rw-  2.0 fat     3672 b- defN 24-May-06 06:25 tdrpa/tdworker/WinWindow.pyi
--rw-rw-rw-  2.0 fat       60 b- defN 24-May-06 07:35 tdrpa/tdworker/__init__.pyi
--rw-rw-rw-  2.0 fat      663 b- defN 24-May-12 20:30 tdrpa.tdworker-1.1.4.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 20:30 tdrpa.tdworker-1.1.4.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-12 20:30 tdrpa.tdworker-1.1.4.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      850 b- defN 24-May-12 20:30 tdrpa.tdworker-1.1.4.6.dist-info/RECORD
-10 files, 1210857 bytes uncompressed, 420093 bytes compressed:  65.3%
+Zip file size: 422508 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1181696 b- defN 24-May-14 21:46 tdrpa/tdworker.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       57 b- defN 24-May-14 21:32 tdrpa/tdworker/__init__.pyi
+-rw-rw-rw-  2.0 fat    16314 b- defN 24-May-14 21:32 tdrpa/tdworker/winElement.pyi
+-rw-rw-rw-  2.0 fat     5063 b- defN 24-May-14 21:33 tdrpa/tdworker/winKeyboard.pyi
+-rw-rw-rw-  2.0 fat     7386 b- defN 24-May-14 21:33 tdrpa/tdworker/winMouse.pyi
+-rw-rw-rw-  2.0 fat     3655 b- defN 24-May-14 21:32 tdrpa/tdworker/window.pyi
+-rw-rw-rw-  2.0 fat      663 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      847 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/RECORD
+10 files, 1215779 bytes uncompressed, 421056 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
 Filename: tdrpa/tdworker.cp38-win_amd64.pyd
 Comment: 
 
-Filename: tdrpa/tdworker/WinElement.pyi
+Filename: tdrpa/tdworker/__init__.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/WinKeyboard.pyi
+Filename: tdrpa/tdworker/winElement.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/WinMouse.pyi
+Filename: tdrpa/tdworker/winKeyboard.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/WinWindow.pyi
+Filename: tdrpa/tdworker/winMouse.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/__init__.pyi
+Filename: tdrpa/tdworker/window.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.6.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.7.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.6.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.6.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.6.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/tdworker/__init__.pyi

```diff
@@ -1 +1 @@
-from . import WinElement, WinKeyboard, WinMouse, WinWindow
+from . import winElement, winKeyboard, winMouse, window
```

## Comparing `tdrpa/tdworker/WinElement.pyi` & `tdrpa/tdworker/winElement.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,213 @@
 import uiautomation as uia
 
-def findElement(selectorString: str = None, anchorsElement: uia.Control = None, searchDelay: int = 10000, continueOnError: bool = False) -> uia.Control | None:
+def findElement(tdTargetStr: str = None, anchorsElement: uia.Control = None, searchDelay: int = 10000, continueOnError: bool = False) -> uia.Control | None:
     """
     获取元素
 
-    WinElement.findElement('', anchorsElement=None, searchDelay=10000, continueOnError=False)
+    winElement.findElement('', anchorsElement=None, searchDelay=10000, continueOnError=False)
 
-    :param selectorString: 目标元素特征码
+    :param tdTargetStr: 目标元素特征码(tdrpa拾取器获取)
     :param anchorsElement: 从哪个元素开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）
     :param searchDelay: 查找延时（豪秒）。默认10000
     :param continueOnError: 错误继续执行。默认False
-    :return: 目标元素
+    :return: 目标元素 or None
     """
-
-def GetChildren(target: str | uia.Control, searchType: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> list | uia.Control:
+def getChildren(target: str | uia.Control, searchType: str = 'all', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> list | uia.Control:
     '''
     获取子元素
 
-    WinElement.GetChildren(element, \'all\', 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getChildren(target, searchType=\'all\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
-    :param searchType: [必选参数]搜索方式。全部子元素(默认):"all" 首个子元素:"first" 最后一个子元素:"last"
-    :param searchDelay: [必选参数]超时时间(毫秒)。
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchType: [可选参数]搜索方式。全部子元素:"all" 首个子元素:"first" 最后一个子元素:"last"。默认"all"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: 目标元素对象的子元素列表 或 首个子元素 或 最后一个子元素
     '''
-def GetParent(target: str | uia.Control, searchDelay: int, anchorsElement: uia.Control = None, searchTop: bool = False, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control:
+def getParent(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, searchTop: bool = False, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control:
     """
     获取父元素
 
-    WinElement.GetParent(element, 10000, anchorsElement=None, searchTop=False, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getParent(target, searchDelay=10000, anchorsElement=None, searchTop=False, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [必选参数]超时时间(毫秒)。
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
-    :param searchTop: [可选参数]是否搜索顶级父元素。搜索临近一层的父元素(默认):False 搜索顶级的父元素:True
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+    :param searchTop: [可选参数]是否搜索顶级父元素。搜索临近一层的父元素:False 搜索顶级的父元素:True。默认False
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: 目标元素对象的上一层父级元素 或 顶层父级元素
     """
-def GetSibling(target: str | uia.Control, position: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control | None:
+def getSibling(target: str | uia.Control, position: str = 'next', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control | None:
     '''
     获取相邻元素
 
-    WinElement.GetSibling(element, "next", 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getSibling(target, position="next", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param position: [必选参数]相邻位置。下一个："next"  上一个："previous"
-    :param searchDelay: [必选参数]超时时间(毫秒)。
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param position: [可选参数]相邻位置。下一个："next"  上一个："previous"。默认"next"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: 目标元素对象的下一个相邻元素对象 或 上一个相邻元素对象，没有返回None
     '''
-def Exists(target: str | uia.Control, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+def exists(target: str | uia.Control, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
     """
     判断元素是否存在
 
-    WinElement.Exists(element, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.exists(target, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: bool
     """
-def GetCheck(target: str | uia.Control, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+def getCheck(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
     """
     获取元素勾选
 
-    WinElement.GetCheck(element, 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getCheck(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: bool
     """
-def SetCheck(target: str | uia.Control, searchDelay: int, isCheck: bool, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def setCheck(target: str | uia.Control, searchDelay: int = 10000, isCheck: bool = True, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
     """
     设置元素勾选
 
-    WinElement.SetCheck(element, 10000, True, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.setCheck(target, searchDelay=10000, isCheck=True, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param isCheck: [必选参数]设置勾选:True 设置取消勾选:False
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param isCheck: [可选参数]设置勾选:True 设置取消勾选:False。默认True
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     """
-def GetSelect(target: str | uia.Control, searchDelay: int, mode: str, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str | int:
+def getSelect(target: str | uia.Control, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str | int:
     '''
     获取元素选择
 
-    WinElement.GetSelect(element, 10000, \'text\', anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getSelect(target, searchDelay=10000, mode=\'text\', anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param mode: [必选参数]获取文本："text" 获取序号：“index” 获取值：“value”
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param mode: [可选参数]获取文本："text" 获取序号：“index” 获取值：“value”。默认"text"
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: 已选项的文本 或 序号 或 值，没有则返回None
     '''
-def SetSelect(target: str | uia.Control, option: str | int, searchDelay: int, mode: str, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, simulateType: str = 'simulate') -> None:
+def setSelect(target: str | uia.Control, option: str | int, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, simulateType: str = 'simulate') -> None:
     '''
     设置元素选择
 
-    WinElement.SetSelect(element, \'\', 10000, \'text\', anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, simulateType=\'simulate\')
+    winElement.setSelect(target, \'\', searchDelay=10000, mode="text", anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, simulateType=\'simulate\')
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param option: [必选参数]选择选项
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param mode: [必选参数]选择文本："text" 选择序号：“index” 选择值：“value”
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param mode: [可选参数]选择文本："text" 选择序号：“index” 选择值：“value”。默认"text"
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心(默认):"center"  左上角:"topLeft"  右上角:"topRight"  左下角:"bottomLeft"  右下角:"bottomRight"
+    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
     :param cursorOffsetX: [可选参数]横坐标偏移。默认0
     :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
-    :param simulateType: [可选参数]鼠标点击选中项时的模式。模拟操作(默认):"simulate"   消息操作:"message"
+    :param simulateType: [可选参数]鼠标点击选中项时的模式。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
     :return: None
     '''
-def GetValue(target: str | uia.Control, getMethod: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str:
+def getValue(target: str | uia.Control, getMethod: str = 'auto', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str:
     '''
     获取元素文本
 
-    WinElement.GetValue(element, "auto", 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getValue(target, getMethod="auto", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param getMethod: [必选参数]获取方式。自动方式："auto"  搜元素Name方式："name"  搜元素Value方式："value"。建议使用自动方式
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param getMethod: [可选参数]获取方式。自动方式："auto" 搜元素Name方式："name" 搜元素Value方式："value"。默认"auto"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: 元素文本
     '''
-def SetValue(target: str | uia.Control, value: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def setValue(target: str | uia.Control, value: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
     '''
     设置元素文本
 
-    WinElement.SetValue(element, "", 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.setValue(target, "", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param value: [必选参数]待写入UI界面元素的文本内容
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     '''
-def GetRect(target: str | uia.Control, relativeType: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> dict:
+def getRect(target: str | uia.Control, relativeType: str = 'parent', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> dict:
     '''
     获取元素区域
 
-    WinElement.GetRect(element, "parent", 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.getRect(target, relativeType="parent", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param relativeType: [必选参数]返回元素位置是相对于哪一个坐标而言的。  相对父元素:"parent"  相对窗口客户区:"root"  相对屏幕坐标:"screen"
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param relativeType: [可选参数]返回元素位置是相对于哪一个坐标而言的。 相对父元素:"parent" 相对窗口客户区:"root" 相对屏幕坐标:"screen"。默认"parent"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: {"height" : int, "width" : int, "x" : int, "y" : int}
     '''
-def ScreenCapture(target: str | uia.Control, filePath: str, rect: dict, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+def screenCapture(target: str | uia.Control, filePath: str, rect: dict = None, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
     '''
     元素截图
 
-    WinElement.ScreenCapture(element, \'D:/1.jpg\', {"x":0, "y":0, "width":0, "height":0}, 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.screenCapture(target, \'D:/1.png\', rect=None, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param filePath: [必选参数]图片存储的绝对路径。如 \'D:/1.png\'(支持图片保存格式：bmp、jpg、jpeg、png、gif、tif、tiff)
-    :param rect: [必选参数]对指定界面元素截图的范围，如果范围传递为 {"x":0,"y":0,"width":0,"height":0}，则截取该元素的全区域，否则以该元素的左上角为坐标原点，根据高宽进行截图
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param rect: [可选参数]对指定界面元素截图的范围，若传None，则截取该元素的全区域。若传{"x":int,"y":int,"width":int,"height":int}，则以该元素左上角位置偏移x,y的坐标为原点，根据高宽进行截图。默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: bool(截图成功返回True，否则返回假)
     '''
-def Wait(target: str | uia.Control, waitType: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def wait(target: str | uia.Control, waitType: str = 'show', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
     '''
     等待元素（等待元素显示或消失）
 
-    WinElement.Wait(element, \'show\', 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+    winElement.wait(target, waitType=\'show\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param waitType: [必选参数]等待方式。 等待显示："show"  等待消失:"hide"
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param waitType: [可选参数]等待方式。 等待显示："show" 等待消失:"hide"。默认"show"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     '''
```

## Comparing `tdrpa/tdworker/WinKeyboard.pyi` & `tdrpa/tdworker/winKeyboard.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 import uiautomation as uia
 
-def InputText(target: str | uia.Control, inputText: str, clearOldText: bool, inputInterval: int, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, simulateType: str = 'simulate', validate: bool = False, clickBeforeInput: bool = False) -> uia.Control:
+def inputText(target: str | uia.Control, content: str, clearOldText: bool = True, inputInterval: int = 10, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, simulateType: str = 'message', validate: bool = False, clickBeforeInput: bool = False) -> uia.Control:
     '''
     在目标中输入
 
-    WinKeyboard.InputText(element, \'\', True, 10, 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, simulateType=\'message\', validate=False, clickBeforeInput=False)
+    winKeyboard.inputText(target, \'\', clearOldText=True, inputInterval=10, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, simulateType=\'message\', validate=False, clickBeforeInput=False)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param inputText: [必选参数]写入文本
-    :param clearOldText: [必选参数]清空原内容
-    :param inputInterval: [必选参数]键入间隔(毫秒)
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param content: [必选参数]写入文本
+    :param clearOldText: [可选参数]是否清空原内容。默认True
+    :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :param setForeground: [可选参数]激活窗口。默认True
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate"   消息操作:"message"(默认)
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
     :param validate: [可选参数]验证写入文本。默认False
     :param clickBeforeInput: [可选参数]输入前点击。默认False
     :return: 目标元素对象
     '''
-def PressKey(target: str | uia.Control, button: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, keyModifiers: list = None, simulateType: str = 'message', clickBeforeInput: bool = False) -> uia.Control:
+def pressKey(target: str | uia.Control, button: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, keyModifiers: list = None, simulateType: str = 'message', clickBeforeInput: bool = False) -> uia.Control:
     '''
     在目标中按键
 
-    WinKeyboard.PressKey(element, "Enter", 10000, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, keyModifiers=None, simulateType=\'message\', clickBeforeInput=False)
+    winKeyboard.pressKey(target, "Enter", searchDelay=10000, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, keyModifiers=None, simulateType=\'message\', clickBeforeInput=False)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param button: [必选参数]键盘按键上的符号，如“Enter”
-    :param searchDelay: [必选参数]超时时间(毫秒)。
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param button: [必选参数]键盘按键上的符号。如"Enter"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :param setForeground: [可选参数]激活窗口。默认True
-    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate"   消息操作(默认):"message"
+    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选。默认None
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
     :param clickBeforeInput: [可选参数]输入前点击。默认False
     :return: 目标元素对象
     '''
-def Input(inputText: str, inputInterval: int, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
+def inputAct(content: str, inputInterval: int = 10, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
     '''
     输入文本
 
-    WinKeyboard.Input(\'\', 10, delayAfter=100, delayBefore=100, simulateType=\'message\')
+    winKeyboard.inputAct(\'\', inputInterval=10, delayAfter=100, delayBefore=100, simulateType=\'message\')
 
-    :param inputText: [必选参数]输入内容
-    :param inputInterval: [必选参数]键入间隔(毫秒)
+    :param content: [必选参数]输入内容
+    :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate"   消息操作(默认):"message"
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
     :return: None
     '''
-def Press(button: str, pressType: str, keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
+def pressAct(button: str, pressType: str = 'press', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
     '''
     模拟按键
 
-    WinKeyboard.Press(\'Enter\', \'press\', None, delayAfter=100, delayBefore=100, simulateType=\'message\')
+    winKeyboard.pressAct(\'Enter\', pressType=\'press\', keyModifiers=None, delayAfter=100, delayBefore=100, simulateType=\'message\')
 
     :param button: [必选参数]键盘按键上的符号，如“Enter”
-    :param pressType: [必选参数]点击类型。单击:"press" 按下:"down" 弹起:"up"
-    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
+    :param pressType: [可选参数]点击类型。单击:"press" 按下:"down" 弹起:"up"。默认"press"
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate"   消息操作(默认):"message"
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
     :return: None
     '''
```

## Comparing `tdrpa/tdworker/WinMouse.pyi` & `tdrpa/tdworker/winMouse.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 import uiautomation as uia
 
-def Action(target: str | uia.Control, button: str, clickType: str, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = False) -> uia.Control:
+def action(target: str | uia.Control, button: str = 'left', clickType: str = 'click', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = False) -> uia.Control:
     '''
     点击目标元素
 
-    WinMouse.Action(element, \'left\', \'click\', 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
+    winMouse.action(target, button="left", clickType="click", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param button: [必选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"
-    :param clickType: [必选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"
-    :param searchDelay: [必选参数]超时时间(毫秒)。
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+    :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心(默认):"center"  左上角:"topLeft"  右上角:"topRight"  左下角:"bottomLeft"  右下角:"bottomRight"
+    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
     :param cursorOffsetX: [可选参数]横坐标偏移。默认0
     :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
-    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
-    :param simulateType: [可选参数]操作类型。模拟操作(默认):"simulate"   消息操作:"message"
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
     :param moveSmoothly: [可选参数]平滑移动。默认False
     :return:目标元素对象
     '''
-def Hover(target: str | uia.Control, searchDelay: int, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = True) -> uia.Control:
+def hover(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = True) -> uia.Control:
     '''
     移动到目标上
 
-    WinMouse.Hover(element, 10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
+    winMouse.hover(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [必选参数]超时时间(毫秒)
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）默认None
+    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
     :param continueOnError: [可选参数]错误继续执行。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心(默认):"center"  左上角:"topLeft"  右上角:"topRight"  左下角:"bottomLeft"  右下角:"bottomRight"
+    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
     :param cursorOffsetX: [可选参数]横坐标偏移。默认0
-    :param cursorOffsetY: [可选参数]纵坐标偏移。默认None
-    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
-    :param simulateType: [可选参数]操作类型。模拟操作(默认):"simulate"   消息操作:"message"
-    :param moveSmoothly: [可选参数]平滑移动。默认False
+    :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
+    :param moveSmoothly: [可选参数]平滑移动。默认True
     :return:目标元素对象
     '''
-def Click(button: str, clickType: str, keyModifiers: list, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def click(button: str = 'left', clickType: str = 'click', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
     '''
     模拟点击
 
-    WinMouse.Click("left", "click", [], delayAfter=100, delayBefore=100)
+    winMouse.click(button="left", clickType="click", keyModifiers=None, delayAfter=100, delayBefore=100)
 
-    :param button: [必选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"
-    :param clickType: [必选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"
-    :param keyModifiers: [必选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认空
+    :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+    :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     '''
-def Move(x: int, y: int, isRelativeMove: bool, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def move(x: int, y: int, isRelativeMove: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
     """
     # 模拟移动
 
-    WinMouse.Move(0, 0, False, delayAfter=100, delayBefore=100)
+    winMouse.move(0, 0, isRelativeMove=False, delayAfter=100, delayBefore=100)
 
     :param x: [必选参数]横坐标
     :param y: [必选参数]纵坐标
-    :param isRelativeMove: [必选参数]是否相对移动
+    :param isRelativeMove: [可选参数]是否相对目前位置移动。默认False
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     """
-def GetPos() -> tuple[int, int]:
+def getPos() -> tuple[int, int]:
     """
     获取鼠标位置
 
-    WinMouse.GetPos()
+    winMouse.getPos()
 
     :return:pointX, pointY
     """
-def Drag(x1: int, y1: int, x2: int, y2: int, button: str, keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def drag(x1: int, y1: int, x2: int, y2: int, button: str = 'left', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
     '''
     模拟拖动
 
-    WinMouse.Drag(0, 0, 0, 0, \'left\', None, delayAfter=100, delayBefore=100)
+    winMouse.drag(0, 0, 0, 0, button=\'left\', keyModifiers=None, delayAfter=100, delayBefore=100)
 
     :param x1: [必选参数]起始横坐标
     :param y1: [必选参数]起始纵坐标
     :param x2: [必选参数]结束横坐标
     :param y2: [必选参数]结束纵坐标
-    :param button: [必选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"
-    :param keyModifiers: [必选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
+    :param button: [可选参数]鼠标按键。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     '''
-def Wheel(scrollNum: int, scrollDirection: str, keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
+def wheel(scrollNum: int, scrollDirection: str = 'down', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
     '''
     模拟滚轮
 
-    WinMouse.Wheel(0, "down", None, delayAfter=100, delayBefore=100)
+    winMouse.wheel(1, scrollDirection="down", keyModifiers=None, delayAfter=100, delayBefore=100)
 
     :param scrollNum: [必选参数]滚动次数
-    :param scrollDirection: [必选参数]滚动方向
-    :param keyModifiers: [必选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选，默认None
+    :param scrollDirection: [可选参数]滚动方向。向上:"up" 向下:"down"。默认"down"
+    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
     :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
     :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
     :return: None
     '''
```

## Comparing `tdrpa/tdworker/WinWindow.pyi` & `tdrpa/tdworker/window.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 import uiautomation as uia
 
-def Close(target: str | uia.Control) -> None:
+def close(target: str | uia.Control) -> None:
     """
-    # 关闭窗口
+    关闭窗口
 
-    WinWindow.Close(element)
+    window.close(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
     :return: None
     """
-def GetActive() -> uia.Control:
+def getActive() -> uia.Control:
     """
-    # 获取活动窗口
+    获取活动窗口
 
-    WinWindow.GetActive()
+    window.getActive()
 
     :return:control
     """
-def SetActive(target: str | uia.Control) -> bool:
+def setActive(target: str | uia.Control) -> bool:
     """
     设置活动窗口
 
-    WinWindow.SetActive(element)
+    window.setActive(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: bool。激活成功返回True，否则返回False
     """
-def Show(target: str | uia.Control, showStatus: str) -> bool:
+def show(target: str | uia.Control, showStatus: str) -> bool:
     '''
     更改窗口显示状态
 
-    WinWindow.Show(element, "show")
+    window.show(target, "show")
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param showStatus: [必选参数] 显示：\'show\' 隐藏：\'hide\' 最大化：\'max\' 最小化：\'min\' 还原：\'restore\'
     :return: bool。执行成功返回True，否则返回False
     '''
-def Exists(target: str | uia.Control) -> bool:
+def exists(target: str | uia.Control) -> bool:
     """
     判断窗口是否存在
 
-    WinWindow.Exists(element)
+    window.exists(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: bool。窗口存在返回True,否则返回False
     """
-def GetSize(target: str | uia.Control) -> dict:
+def getSize(target: str | uia.Control) -> dict:
     '''
     获取窗口大小
 
-    WinWindow.GetSize(element)
+    window.getSize(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: {"height":int, "width":int, "x":int, "y":int}
     '''
-def SetSize(target: str | uia.Control, width: int, height: int) -> None:
+def setSize(target: str | uia.Control, width: int, height: int) -> None:
     """
     改变窗口大小
 
-    WinWindow.SetSize(element, 800, 600)
+    window.setSize(target, 800, 600)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param width: [必选参数]窗口宽度
     :param height: [必选参数]窗口高度
     :return: None
     """
-def Move(target: str | uia.Control, x: int, y: int) -> None:
+def move(target: str | uia.Control, x: int, y: int) -> None:
     """
     移动窗口位置
 
-    WinWindow.Move(element, 0, 0)
+    window.move(target, 0, 0)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :param x: [必选参数]移动到新位置的横坐标
     :param y: [必选参数]移动到新位置的纵坐标
     :return: None
     """
-def TopMost(target: str | uia.Control, topMost: bool) -> None:
+def topMost(target: str | uia.Control, isTopMost: bool = True) -> None:
     """
     窗口置顶
 
-    WinWindow.TopMost(element, True)
+    window.topMost(target, isTopMost=True)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param topMost: [必选参数]是否使窗口置顶，窗口置顶:true 窗口取消置顶:false
+    :param isTopMost: [可选参数]是否使窗口置顶，窗口置顶:true 窗口取消置顶:false。默认True
     :return: None
     """
-def GetClass(target: str | uia.Control) -> str:
+def getClass(target: str | uia.Control) -> str:
     """
     获取窗口类名
 
-    WinWindow.GetClass(element)
+    window.getClass(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: 窗口的类名称
     """
-def GetPath(target: str | uia.Control) -> str:
+def getPath(target: str | uia.Control) -> str:
     """
     获取窗口程序的文件路径
 
-    WinWindow.GetPath(element)
+    window.getPath(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: 文件绝对路径
     """
-def GetPID(target: str | uia.Control) -> int:
+def getPID(target: str | uia.Control) -> int:
     """
     获取进程PID
 
-    WinWindow.GetPID(element)
+    window.getPID(target)
 
     :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
     :return: PID
     """
```

## Comparing `tdrpa.tdworker-1.1.4.6.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.6
+Version: 1.1.4.7
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
```

## Comparing `tdrpa.tdworker-1.1.4.6.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp38-win_amd64.pyd,sha256=PvfPPm2QuIf7n0HsRFXGmfEm9TEmBeSNqERMbMkTvBE,1178112
-tdrpa/tdworker/WinElement.pyi,sha256=Y6OBYXLr3w1xmRnnVGvbWtlX46v5d87NiOBkq-01O4s,15621
-tdrpa/tdworker/WinKeyboard.pyi,sha256=bRdaR6rM4FNzbIATUXRmt36fm3BhFarzpKruAJHklME,4815
-tdrpa/tdworker/WinMouse.pyi,sha256=H_59kcbqkJwoSfGQxte2Uo_f7J7n1ys2p9MKeZ1tnhU,6966
-tdrpa/tdworker/WinWindow.pyi,sha256=8X9FLtPKbw2rK2Wgc9z2ZmmWUAbogbNK6lmYhQ84dHU,3672
-tdrpa/tdworker/__init__.pyi,sha256=p5gNrSuSvmBtCSEM133tD7XSlW_2LyUB4svpQTlndv8,60
-tdrpa.tdworker-1.1.4.6.dist-info/METADATA,sha256=zOFWOE-y8VBu--6UjS173HWDA4_y4hTDXu0qs0PwjPc,663
-tdrpa.tdworker-1.1.4.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.6.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.6.dist-info/RECORD,,
+tdrpa/tdworker.cp38-win_amd64.pyd,sha256=5U6Xou_qyKd9ObbdidPLTgjfIRVaDouIAzyOVG78Sto,1181696
+tdrpa/tdworker/__init__.pyi,sha256=shtXcGhKTE0C1_MGmin9uKGT_HVSryEfM5KefQ1gucU,57
+tdrpa/tdworker/winElement.pyi,sha256=B4B-ThcOer6rwlJGfzEhibY9hYnhlamW50xL_feHA5c,16314
+tdrpa/tdworker/winKeyboard.pyi,sha256=veEChbM_Zp_AIBKF33TLp3KTPPhD3U9UYwJihUQFocQ,5063
+tdrpa/tdworker/winMouse.pyi,sha256=ZgNQH4Bab7CzXFPqaU3t8Lwg280wuc2FHsGS0bXaRKg,7386
+tdrpa/tdworker/window.pyi,sha256=tFxdjk9BGqS_d9NWv_3qhLoTmBAs1yIa4eSXII_wqVc,3655
+tdrpa.tdworker-1.1.4.7.dist-info/METADATA,sha256=KrgRUDcBO0XJ57E_YUJeBw1y-dnzZyP3fOgRRHzXh38,663
+tdrpa.tdworker-1.1.4.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.7.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.7.dist-info/RECORD,,
```

