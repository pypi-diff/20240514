# Comparing `tmp/pdocr_rpc-2023.8.23.tar.gz` & `tmp/pdocr_rpc-2024.5.14.tar.gz`

## Comparing `pdocr_rpc-2023.8.23.tar` & `pdocr_rpc-2024.5.14.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     8399 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/pdocr_rpc/server.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/pyproject.toml
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 pdocr_rpc-2023.8.23/PKG-INFO
+-rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/NOTICE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.14/PKG-INFO
```

### Comparing `pdocr_rpc-2023.8.23/pdocr_rpc/__init__.py` & `pdocr_rpc-2024.5.14/pdocr_rpc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,125 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-"""
-@Author: Mikigo
-@Date: 2022/5/25 0:03
-"""
+
+# SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
+
+# SPDX-License-Identifier: Apache Software License
 import json
 import os
-from time import sleep
+import time
 from xmlrpc.client import Binary
 from xmlrpc.client import ServerProxy
 
 from pdocr_rpc.conf import setting
 
 os.environ["DISPLAY"] = ":0"
 
 if setting.IS_LINUX:
     import pyscreenshot as ImageGrab
 elif setting.IS_WINDOWS:
     from PIL import ImageGrab
-    
+
 from funnylog import logger
 
 
+
 class OCR:
-    @staticmethod
-    def _pdocr_client(lang, picture_abspath=None, retry: int = 2):
+
+    @classmethod
+    def server_url(cls):
+        return f"http://{setting.SERVER_IP}:{setting.PORT}"
+
+    @classmethod
+    def server(cls):
+        return ServerProxy(cls.server_url(), allow_none=True)
+
+    @classmethod
+    def check_connected(cls):
+        try:
+            return cls.server().check_connected()
+        except OSError:
+            return False
+
+    @classmethod
+    def _pdocr_client(cls, lang, picture_abspath=None, network_retry: int = 1):
         """
          通过 RPC 协议进行 OCR 识别。
         :return: 返回 PaddleOCR 的原始数据
         """
         if not picture_abspath:
             picture_abspath = setting.SCREEN_CACHE
             if setting.IS_X11:
                 ImageGrab.grab().save(os.path.expanduser(picture_abspath))
             else:
                 picture_abspath = (
                     os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
                     .read()
                     .strip("\n")
                 )
-        server = ServerProxy(
-            f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True
-        )
+
         put_handle = open(os.path.expanduser(picture_abspath), "rb")
-        for _ in range(retry):
+        for _ in range(network_retry + 1):
             try:
                 # 将图片上传到服务端
-                pic_dir = server.image_put(Binary(put_handle.read()))
+                pic_dir = cls.server().image_put(Binary(put_handle.read()))
                 put_handle.close()
                 # 返回识别结果
-                return server.paddle_ocr(pic_dir, lang)
+                pic_path =  cls.server().paddle_ocr(pic_dir, lang)
+                return pic_path
             except OSError:
-                pass
-            raise EnvironmentError(
-                f"RPC服务器链接失败. http://{setting.SERVER_IP}:{setting.PORT}"
-            )
+                continue
+        raise EnvironmentError(
+            f"RPC服务器链接失败: {cls.server_url}"
+        )
 
     @classmethod
     def _ocr(
-        cls,
-        *target_strings,
-        picture_abspath=None,
-        similarity=0.6,
-        return_default=False,
-        return_first=False,
-        lang="ch",
-        retry: int = 2,
+            cls,
+            *target_strings,
+            picture_abspath=None,
+            similarity=0.6,
+            return_default=False,
+            return_first=False,
+            lang="ch",
+            network_retry: int = 1,
     ):
         """
          通过 OCR 进行识别。
         :param target_strings:
             目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
             如果不传参，返回图片中识别到的所有字符串。
         :param picture_abspath: 要识别的图片路径，如果不传默认截取全屏识别。
         :param similarity: 匹配度。
         :param return_default: 返回识别的原生数据。
         :param return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
         :param lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
         :param retry: 连接服务器重试次数
         :return: 返回的坐标是目标字符串所在行的中心坐标。
         """
-        results = cls._pdocr_client(picture_abspath=picture_abspath, lang=lang, retry=retry)
+        results = cls._pdocr_client(picture_abspath=picture_abspath, lang=lang, network_retry=network_retry)
         if return_default:
             return results
         more_map = {}
         if len(target_strings) == 1:
             n = 1
-            for res in results:
-                [
+            for res in results[0]:
+                try:
                     [
-                        [left_top_x, left_top_y],
-                        [right_top_x, right_top_y],
-                        [right_bottom_x, right_bottom_y],
-                        [left_bottom_x, left_bottom_y],
-                    ],
-                    (strings, rate),
-                ] = res
+                        [
+                            [left_top_x, left_top_y],
+                            [right_top_x, right_top_y],
+                            [right_bottom_x, right_bottom_y],
+                            [left_bottom_x, left_bottom_y],
+                        ],
+                        [strings, rate],
+                    ] = res
+                except ValueError as e:
+                    print(res)
+                    raise ValueError(e) from e
                 if target_strings[0] in strings:
                     if rate >= similarity:
                         center_x = (right_top_x + left_top_x) / 2
                         center_y = (right_bottom_y + right_top_y) / 2
                         more_map[
                             target_strings[0]
                             if not more_map.get(target_strings[0])
@@ -113,15 +133,15 @@
                 logger.debug(f"OCR识别到字符 [{target_strings[0]}]—>{center_x, center_y}")
                 return center_x, center_y
             if len(more_map) > 1:
                 logger.debug(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
                 return more_map
 
         elif len(target_strings) == 0:
-            for res in results:
+            for res in results[0]:
                 [
                     [
                         [left_top_x, left_top_y],
                         [right_top_x, right_top_y],
                         [right_bottom_x, right_bottom_y],
                         [left_bottom_x, left_bottom_y],
                     ],
@@ -136,15 +156,15 @@
                 logger.debug(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
                 return more_map
 
         else:
             for target_string in target_strings:
                 n = 1
                 more_map[target_string] = False
-                for res in results:
+                for res in results[0]:
                     [
                         [
                             [left_top_x, left_top_y],
                             [right_top_x, right_top_y],
                             [right_bottom_x, right_bottom_y],
                             [left_bottom_x, left_bottom_y],
                         ],
@@ -163,60 +183,71 @@
                             break
                         n += 1
 
             if more_map:
                 logger.debug(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
                 return more_map
         res_log = []
-        for res in results:
+        for res in results[0]:
             [[*_], [strings, rate]] = res
             res_log.append(strings)
         logger.debug(f"未识别到字符{target_strings}, 识别到的原始内容：{res_log}")
         return False
 
     @classmethod
     def ocr(
             cls,
             *target_strings,
-            picture_abspath=None,
-            similarity=0.6,
-            return_default=False,
-            return_first=False,
-            lang="ch",
-            retry: int = 2,
-            res_retry: int = 2,
+            picture_abspath: str = None,
+            similarity: [int, float] = 0.6,
+            return_default: bool = False,
+            return_first: bool = False,
+            lang: str = "ch",
+            network_retry: int = None,
+            pause: [int, float] = None,
+            timeout: [int, float] = None,
+            max_match_number: int = None,
     ):
         """
         通过 OCR 进行识别。
         :param target_strings:
             目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
             如果不传参，返回图片中识别到的所有字符串。
         :param picture_abspath: 要识别的图片路径，如果不传默认截取全屏识别。
         :param similarity: 匹配度。
         :param return_default: 返回识别的原生数据。
         :param return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
         :param lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
-        :param retry: 连接服务器重试次数
-        :param res_retry: 如果结果返回为 False，重试次数
+        :param network_retry: 连接服务器重试次数
+        :param pause: 重试间隔时间,单位秒
+        :param timeout: 最大匹配超时,单位秒
+        :param max_match_number: 最大匹配次数
         :return: 返回的坐标是目标字符串所在行的中心坐标。
         """
-        for _ in range(res_retry):
+        network_retry = network_retry if network_retry else setting.NETWORK_RETRY
+        pause = pause if pause else setting.PAUSE
+        timeout = timeout if timeout else setting.TIMEOUT
+        max_match_number = max_match_number if max_match_number else setting.MAX_MATCH_NUMBER
+        ignore_time = 0
+        start = time.time()
+        for _ in range(max_match_number):
+            end = time.time()
+            during = end - start - ignore_time
+            if during > timeout:
+                return False
+            _start = time.time()
             res = cls._ocr(
                 *target_strings,
                 picture_abspath=picture_abspath,
                 similarity=similarity,
                 return_default=return_default,
                 return_first=return_first,
                 lang=lang,
-                retry=retry,
+                network_retry=network_retry,
             )
+            _end = time.time()
+            ignore_time += (_end - _start)
             if res is False:
-                sleep(1)
+                time.sleep(pause)
                 continue
             return res
         return False
-
-
-if __name__ == "__main__":
-    from pdocr_rpc.conf import setting
-    setting.SERVER_IP = "youqu-dev.uniontech.com"
-    OCR.ocr("uniontech","youqu")
```

### Comparing `pdocr_rpc-2023.8.23/pdocr_rpc/server.py` & `pdocr_rpc-2024.5.14/pdocr_rpc/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-"""
-:Author: Mikigo
-:Date: 2022/5/25 0:02
-"""
+
+# SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
+
+# SPDX-License-Identifier: Apache Software License
 from os import makedirs
 from os.path import join, dirname, abspath, exists
 from socketserver import ThreadingMixIn
 from time import time
 from typing import TYPE_CHECKING
 from xmlrpc.server import SimpleXMLRPCServer
 
@@ -20,14 +20,18 @@
 class ThreadXMLRPCServer(ThreadingMixIn, SimpleXMLRPCServer):
     pass
 
 
 CURRENT_DIR = dirname(abspath(__file__))
 
 
+def check_connected():
+    return True
+
+
 def image_put(data):
     pic_dir = join(CURRENT_DIR, "pic")
     if not exists(pic_dir):
         makedirs(pic_dir)
 
     pic_path = join(pic_dir, f"pic_{time()}.png")
     handle = open(pic_path, "wb")
@@ -40,22 +44,22 @@
     """
      Paddleocr目前支持的多语言语种可以通过修改lang参数进行切换
      例如`ch`, `en`, `fr`, `german`, `korean`, `japan`
     :param file_name:
     :param lang:
     :return:
     """
-    ocr = PaddleOCR(use_angle_cls=True, lang=lang)
+    ocr = PaddleOCR(use_angle_cls=True, lang=lang, ocr_version="PP-OCRv4")
     result = ocr.ocr(pic_path, cls=True)
     return result
 
 
 def server():
-    """server"""
     server = ThreadXMLRPCServer(("0.0.0.0", setting.PORT), allow_none=True)
+    server.register_function(check_connected, "check_connected")
     server.register_function(image_put, "image_put")
     server.register_function(paddle_ocr, "paddle_ocr")
     print("Listen to client requests ...")
     print(f"Client request: IP:{setting.PORT}")
     server.serve_forever()
```

### Comparing `pdocr_rpc-2023.8.23/LICENSE` & `pdocr_rpc-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2023.8.23/README.md` & `pdocr_rpc-2024.5.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 因为 `PaddleOCR` 安装**太重**了，如果你的使用场景是需要经常安装，那绝对是一个痛苦的事情，你要是知道它每次安装要装多少东西你肯定会忍不住摇头；
 
 而在服务端一次性安装部署之后，客户端就可以零成本的使用，非常的方便。
 
 ---
 
-**Documentation**: <a href="https://funny-dream.github.io/pdocr-rpc" target="_blank">https://funny-dream.github.io/pdocr-rpc</a>
+**Documentation**: <a href="https://linuxdeepin.github.io/pdocr-rpc" target="_blank">https://linuxdeepin.github.io/pdocr-rpc</a>
 
-**Source Code**: <a href="https://github.com/funny-dream/pdocr-rpc" target="_blank">https://github.com/funny-dream/pdocr-rpc</a>
+**Source Code**: <a href="https://github.com/linuxdeepin/pdocr-rpc" target="_blank">https://github.com/linuxdeepin/pdocr-rpc</a>
 
 ---
 
 ## 1、服务端
 
 ### 服务端安装
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # pdocr-rpc åºäº `PaddleOCR` å°è£ç `RPC`
 æå¡ï¼åå«å®¢æ·ç«¯åæå¡ç«¯ã
 å®¢æ·ç«¯æä¾äºä¸ä¸ªç®åæç¨çå½æ°
 `ocr`ï¼éè¿ä¸åçåæ°æ§å¶è¿åä¸åçå¼ã
 **ä¸ºä»ä¹è¦åææå¡ç«¯åå®¢æ·ç«¯ï¼** å ä¸º `PaddleOCR`
 å®è£**å¤ªé**äºï¼å¦æä½ çä½¿ç¨åºæ¯æ¯éè¦ç»å¸¸å®è£ï¼é£ç»å¯¹æ¯ä¸ä¸ªçè¦çäºæï¼ä½ è¦æ¯ç¥éå®æ¯æ¬¡å®è£è¦è£å¤å°ä¸è¥¿ä½ è¯å®ä¼å¿ä¸ä½æå¤´ï¼
 èå¨æå¡ç«¯ä¸æ¬¡æ§å®è£é¨ç½²ä¹åï¼å®¢æ·ç«¯å°±å¯ä»¥é¶ææ¬çä½¿ç¨ï¼éå¸¸çæ¹ä¾¿ã
---- **Documentation**: _h_t_t_p_s_:_/_/_f_u_n_n_y_-_d_r_e_a_m_._g_i_t_h_u_b_._i_o_/_p_d_o_c_r_-_r_p_c **Source Code**:
-_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_f_u_n_n_y_-_d_r_e_a_m_/_p_d_o_c_r_-_r_p_c --- ## 1ãæå¡ç«¯ ###
+--- **Documentation**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_p_d_o_c_r_-_r_p_c **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_p_d_o_c_r_-_r_p_c --- ## 1ãæå¡ç«¯ ###
 æå¡ç«¯å®è£ ```console pip install pdocr-rpc[server] ``` ###
 æå¡ç«¯å¯å¨æå¡
 éææ°å»ºä¸ä¸ª`py`æä»¶ï¼åç§°ä½ å¯ä»¥èªå®ä¹ï¼æ¯å¦ï¼`ocr_server.py`ï¼
 åå¥ä»¥ä¸åå®¹ï¼ ```python # ocr_server.py from pdocr_rpc.server import
 server server() ``` é»è®¤ç«¯å£å·ä¸º `8890` å¦æä½ æ³ä¿®æ¹ç«¯å£ï¼
 ```python from pdocr_rpc.server import server from pdocr_rpc.conf import
 setting setting.PORT = 8888 server() ``` ## 2ãå®¢æ·ç«¯ ### å®¢æ·ç«¯å®è£
```

### Comparing `pdocr_rpc-2023.8.23/pyproject.toml` & `pdocr_rpc-2024.5.14/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -43,9 +43,9 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "/pdocr_rpc",
     "/README.md",
 ]
 
 [project.urls]
-Source = "https://github.com/funny-dream/pdocr-rpc"
-Documentation = "https://funny-dream.github.io/pdocr-rpc"
+Source = "https://github.com/linuxdeepin/pdocr-rpc"
+Documentation = "https://linuxdeepin.github.io/pdocr-rpc"
```

### Comparing `pdocr_rpc-2023.8.23/PKG-INFO` & `pdocr_rpc-2024.5.14/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2023.8.23
+Version: 2024.5.14
 Summary: PaddleOCR-RPC
-Project-URL: Source, https://github.com/funny-dream/pdocr-rpc
-Project-URL: Documentation, https://funny-dream.github.io/pdocr-rpc
+Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc
+Project-URL: Documentation, https://linuxdeepin.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
+License-File: NOTICE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: funnylog
 Requires-Dist: pillow; sys_platform == 'win32'
 Requires-Dist: pyscreenshot; sys_platform == 'linux'
@@ -32,17 +33,17 @@
 
 因为 `PaddleOCR` 安装**太重**了，如果你的使用场景是需要经常安装，那绝对是一个痛苦的事情，你要是知道它每次安装要装多少东西你肯定会忍不住摇头；
 
 而在服务端一次性安装部署之后，客户端就可以零成本的使用，非常的方便。
 
 ---
 
-**Documentation**: <a href="https://funny-dream.github.io/pdocr-rpc" target="_blank">https://funny-dream.github.io/pdocr-rpc</a>
+**Documentation**: <a href="https://linuxdeepin.github.io/pdocr-rpc" target="_blank">https://linuxdeepin.github.io/pdocr-rpc</a>
 
-**Source Code**: <a href="https://github.com/funny-dream/pdocr-rpc" target="_blank">https://github.com/funny-dream/pdocr-rpc</a>
+**Source Code**: <a href="https://github.com/linuxdeepin/pdocr-rpc" target="_blank">https://github.com/linuxdeepin/pdocr-rpc</a>
 
 ---
 
 ## 1、服务端
 
 ### 服务端安装
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2023.8.23 Summary: PaddleOCR-RPC
-Project-URL: Source, https://github.com/funny-dream/pdocr-rpc Project-URL:
-Documentation, https://funny-dream.github.io/pdocr-rpc Author-email: mikigo
-<1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
-Requires-Dist: funnylog Requires-Dist: pillow; sys_platform == 'win32'
-Requires-Dist: pyscreenshot; sys_platform == 'linux' Provides-Extra: doc
-Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: server Requires-
-Dist: paddleocr>=2.0.1; extra == 'server' Requires-Dist: paddlepaddle; extra ==
-'server' Provides-Extra: test Requires-Dist: pytest; extra == 'test'
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.14 Summary: PaddleOCR-RPC
+Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc Project-URL:
+Documentation, https://linuxdeepin.github.io/pdocr-rpc Author-email: mikigo
+<1964191531@qq.com> License-File: LICENSE License-File: NOTICE Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
+Python: >=3.7 Requires-Dist: funnylog Requires-Dist: pillow; sys_platform ==
+'win32' Requires-Dist: pyscreenshot; sys_platform == 'linux' Provides-Extra:
+doc Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: server
+Requires-Dist: paddleocr>=2.0.1; extra == 'server' Requires-Dist: paddlepaddle;
+extra == 'server' Provides-Extra: test Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown # pdocr-rpc åºäº `PaddleOCR`
 å°è£ç `RPC` æå¡ï¼åå«å®¢æ·ç«¯åæå¡ç«¯ã
 å®¢æ·ç«¯æä¾äºä¸ä¸ªç®åæç¨çå½æ°
 `ocr`ï¼éè¿ä¸åçåæ°æ§å¶è¿åä¸åçå¼ã
 **ä¸ºä»ä¹è¦åææå¡ç«¯åå®¢æ·ç«¯ï¼** å ä¸º `PaddleOCR`
 å®è£**å¤ªé**äºï¼å¦æä½ çä½¿ç¨åºæ¯æ¯éè¦ç»å¸¸å®è£ï¼é£ç»å¯¹æ¯ä¸ä¸ªçè¦çäºæï¼ä½ è¦æ¯ç¥éå®æ¯æ¬¡å®è£è¦è£å¤å°ä¸è¥¿ä½ è¯å®ä¼å¿ä¸ä½æå¤´ï¼
 èå¨æå¡ç«¯ä¸æ¬¡æ§å®è£é¨ç½²ä¹åï¼å®¢æ·ç«¯å°±å¯ä»¥é¶ææ¬çä½¿ç¨ï¼éå¸¸çæ¹ä¾¿ã
---- **Documentation**: _h_t_t_p_s_:_/_/_f_u_n_n_y_-_d_r_e_a_m_._g_i_t_h_u_b_._i_o_/_p_d_o_c_r_-_r_p_c **Source Code**:
-_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_f_u_n_n_y_-_d_r_e_a_m_/_p_d_o_c_r_-_r_p_c --- ## 1ãæå¡ç«¯ ###
+--- **Documentation**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_p_d_o_c_r_-_r_p_c **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_p_d_o_c_r_-_r_p_c --- ## 1ãæå¡ç«¯ ###
 æå¡ç«¯å®è£ ```console pip install pdocr-rpc[server] ``` ###
 æå¡ç«¯å¯å¨æå¡
 éææ°å»ºä¸ä¸ª`py`æä»¶ï¼åç§°ä½ å¯ä»¥èªå®ä¹ï¼æ¯å¦ï¼`ocr_server.py`ï¼
 åå¥ä»¥ä¸åå®¹ï¼ ```python # ocr_server.py from pdocr_rpc.server import
 server server() ``` é»è®¤ç«¯å£å·ä¸º `8890` å¦æä½ æ³ä¿®æ¹ç«¯å£ï¼
 ```python from pdocr_rpc.server import server from pdocr_rpc.conf import
 setting setting.PORT = 8888 server() ``` ## 2ãå®¢æ·ç«¯ ### å®¢æ·ç«¯å®è£
```

