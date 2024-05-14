# Comparing `tmp/QEasyWidgets-0.1.7.tar.gz` & `tmp/QEasyWidgets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.1.7.tar", last modified: Thu May  9 05:45:51 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.1.8.tar", last modified: Tue May 14 15:27:43 2024, max compression
```

## Comparing `QEasyWidgets-0.1.7.tar` & `QEasyWidgets-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 05:45:51.676888 QEasyWidgets-0.1.7/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1759 2024-05-09 05:45:51.676888 QEasyWidgets-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 05:45:51.661884 QEasyWidgets-0.1.7/QEasyWidgets/
--rw-rw-rw-   0        0        0    22207 2024-05-09 05:44:53.000000 QEasyWidgets-0.1.7/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0    15173 2024-05-09 05:44:56.000000 QEasyWidgets-0.1.7/QEasyWidgets/QFunctions.py
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.7/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0    70976 2024-05-08 10:24:53.000000 QEasyWidgets-0.1.7/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    29197 2024-05-08 03:09:46.000000 QEasyWidgets-0.1.7/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.1.7/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.7/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 05:45:51.676888 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-05-09 05:45:51.000000 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-09 05:45:51.000000 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 05:45:51.000000 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-09 05:45:51.000000 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-09 05:45:51.000000 QEasyWidgets-0.1.7/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 05:45:51.676888 QEasyWidgets-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1570 2024-05-09 05:44:51.000000 QEasyWidgets-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.100190 QEasyWidgets-0.1.8/QEasyWidgets/
+-rw-rw-rw-   0        0        0    23435 2024-05-14 14:01:25.000000 QEasyWidgets-0.1.8/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0    15667 2024-05-14 09:59:56.000000 QEasyWidgets-0.1.8/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.8/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0    70976 2024-05-08 10:24:53.000000 QEasyWidgets-0.1.8/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    29197 2024-05-08 03:09:46.000000 QEasyWidgets-0.1.8/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.1.8/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.8/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 15:27:43.000000 QEasyWidgets-0.1.8/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 15:27:43.103299 QEasyWidgets-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-05-14 10:04:20.000000 QEasyWidgets-0.1.8/setup.py
```

### Comparing `QEasyWidgets-0.1.7/LICENSE` & `QEasyWidgets-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/PKG-INFO` & `QEasyWidgets-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.1.8/QEasyWidgets/ComponentsCustomizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         super().__init__(parent)
 
         self.setIcon(IconBase.Ellipsis)
 
     def setMenu(self, menu: QMenu) -> None:
         def ShowMenu():
             MenuWidth = menu.sizeHint().width()
-            XPos = MenuWidth - self.width()
+            XPos = self.width() - MenuWidth
             YPos = self.height()
             menu.exec(self.mapToGlobal(QPoint(XPos, YPos)))
         self.clicked.connect(ShowMenu)
 
     def SetMenu(self, ActionEvents: dict) -> None:
         Menu = QMenu(self)
         for Action in ActionEvents.keys():
@@ -448,47 +448,85 @@
             self.removeRow(0)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Table.Deregistrate(self)
 
 ##############################################################################################################################
 
+class LineEdit(QLineEdit):
+    '''
+    '''
+    focusedIn = Signal()
+    focusedOut = Signal()
+
+    def __init__(self, parent: QWidget = None):
+        super().__init__(parent)
+
+    def focusInEvent(self, arg__1: QFocusEvent) -> None:
+        self.focusedIn.emit()
+
+    def focusOutEvent(self, arg__1: QFocusEvent) -> None:
+        self.focusedOut.emit()
+
+
 class LineEditBase(QFrame):
     '''
     '''
     textChanged = Signal(str)
+    cursorPositionChanged = Signal(int, int)
+
+    focusedIn = Signal()
+    focusedOut = Signal()
 
     rectChanged = Signal(QRect)
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
 
-        self.LineEdit = QLineEdit()
-        self.LineEdit.textChanged.connect(self.LineEdit.setStatusTip)
+        self.LineEdit = LineEdit()
         self.LineEdit.textChanged.connect(self.textChanged.emit)
+        #self.LineEdit.cursorPositionChanged.connect(self.cursorPositionChanged.emit)
+        self.LineEdit.focusedIn.connect(self.focusInEvent)
+        self.LineEdit.focusedOut.connect(self.focusOutEvent)
 
         self.Button = ButtonBase()
         self.Button.setIcon(IconBase.OpenedFolder)
 
         HBoxLayout = QHBoxLayout(self)
         HBoxLayout.setSpacing(0)
         HBoxLayout.setContentsMargins(0, 0, 0, 0)
         HBoxLayout.addWidget(self.LineEdit)
         HBoxLayout.addWidget(self.Button, alignment = Qt.AlignRight)
 
+        self.ToolTip = QToolTip()
+        self.IsAlerted = False
+
         StyleSheetBase.Edit.Apply(self)
 
-        self.Mask = QLabel(self)
-        self.rectChanged.connect(self.Mask.setGeometry)
-        self.Mask.setStyleSheet('background-color: rgba(0, 0, 0, 111);')
-        self.Mask.setAlignment(Qt.AlignCenter)
-        self.Mask.hide()
+    def focusInEvent(self) -> None:
+        self.focusedIn.emit()
+
+    def focusOutEvent(self) -> None:
+        self.focusedOut.emit()
+
+    def showToolTip(self, Content: Optional[str] = None) -> None:
+        XPos = 0
+        YPos = 0 - self.height()
+        self.ToolTip.showText(self.mapToGlobal(QPoint(XPos, YPos)), Content) if not self.ToolTip.isVisible() and Content is not None else None
+
+    def hideToolTip(self) -> None:
+        self.ToolTip.hideText() if self.ToolTip.isVisible() else None
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
-        self.Mask.hide()
+        position = event.position()
+        self.cursorPositionChanged.emit(position.x(), position.y())
+        if 0 < position.x() < self.width() and 0 < position.y() < self.height():
+            pass #self.focusInEvent()
+        else:
+            self.focusOutEvent()
 
     def moveEvent(self, event: QMoveEvent) -> None:
         self.rectChanged.emit(self.rect())
 
     def resizeEvent(self, event: QResizeEvent) -> None:
         self.rectChanged.emit(self.rect())
 
@@ -528,19 +566,22 @@
     def RemoveFileDialogButton(self):
         self.Button.deleteLater()
         self.Button.hide()
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Edit.Deregistrate(self)
 
-    def Alert(self, Enable: bool, MaskContent: Optional[str] = None) -> None:
-        AlertStyle = 'LineEditBase {border-color: red;}'
-        self.setStyleSheet((self.styleSheet() + AlertStyle) if Enable else self.styleSheet().replace(AlertStyle, ''))
-        self.Mask.setText(MaskContent) if MaskContent is not None else None
-        self.Mask.show() if Enable else self.Mask.hide()
+    def setStyleSheet(self, styleSheet: str) -> None:
+        AlertStyle = 'LineEditBase {border-color: red;}' if self.IsAlerted else ''
+        super().setStyleSheet(styleSheet + AlertStyle)
+
+    def Alert(self, Enable: bool, Content: Optional[str] = None) -> None:
+        self.IsAlerted = Enable
+        StyleSheetBase.Edit.Apply(self)
+        self.showToolTip(Content) if Enable else self.hideToolTip()
 
 ##############################################################################################################################
 
 class MediaPlayerBase(QWidget):
     '''
     '''
     def __init__(self, parent: QWidget = None):
```

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.1.8/QEasyWidgets/QFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,31 @@
     AnimationGroup.addAnimation(Function_SetAnimation(FrameAnimationMinWidth, CurrentWidth, TargetWidth, Duration)) if TargetWidth is not None else None
     AnimationGroup.addAnimation(Function_SetAnimation(FrameAnimationMaxWidth, CurrentWidth, TargetWidth, Duration)) if TargetWidth is not None else None
     AnimationGroup.addAnimation(Function_SetAnimation(FrameAnimationMinHeight, CurrentHeight, TargetHeight, Duration)) if TargetHeight is not None else None
     AnimationGroup.addAnimation(Function_SetAnimation(FrameAnimationMaxHeight, CurrentHeight, TargetHeight, Duration)) if TargetHeight is not None else None
 
     return AnimationGroup
 
+
+def Function_SetWidgetOpacityAnimation(
+    Widget: QWidget,
+    OriginalOpacity: float,
+    TargetOpacity: float,
+    Duration: int = 99
+):
+    OpacityEffect = QGraphicsOpacityEffect()
+    Widget.setGraphicsEffect(OpacityEffect)
+
+    OriginalOpacity = OriginalOpacity
+    AlteredOpacity = TargetOpacity
+
+    WidgetAnimation = QPropertyAnimation(OpacityEffect, b"opacity", Widget)
+
+    return Function_SetAnimation(WidgetAnimation, OriginalOpacity, AlteredOpacity, Duration)
+
 ##############################################################################################################################
 
 def Function_SetNoContents(
     Widget: QWidget
 ):
     if isinstance(Widget, QStackedWidget):
         while Widget.count():
```

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.1.8/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/Sources.py` & `QEasyWidgets-0.1.8/QEasyWidgets/Sources.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/Utils.py` & `QEasyWidgets-0.1.8/QEasyWidgets/Utils.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.1.8/QEasyWidgets/WindowCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.1.8/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
```

### Comparing `QEasyWidgets-0.1.7/README.md` & `QEasyWidgets-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.7/setup.py` & `QEasyWidgets-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.1.7',
+    version = '0.1.8',
     description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
```

