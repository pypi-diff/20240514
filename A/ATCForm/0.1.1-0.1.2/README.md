# Comparing `tmp/atcform-0.1.1.tar.gz` & `tmp/atcform-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atcform-0.1.1.tar", last modified: Tue May 14 15:03:07 2024, max compression
+gzip compressed data, was "atcform-0.1.2.tar", last modified: Tue May 14 16:11:58 2024, max compression
```

## Comparing `atcform-0.1.1.tar` & `atcform-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 15:03:07.733956 atcform-0.1.1/
--rw-rw-rw-   0        0        0        0 2024-05-14 14:31:10.000000 atcform-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      821 2024-05-14 15:03:07.732957 atcform-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-14 11:13:13.000000 atcform-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 15:03:07.733956 atcform-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      981 2024-05-14 15:01:26.000000 atcform-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:03:07.713901 atcform-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 15:03:07.731951 atcform-0.1.1/src/ATCForm.egg-info/
--rw-rw-rw-   0        0        0      821 2024-05-14 15:03:07.000000 atcform-0.1.1/src/ATCForm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-14 15:03:07.000000 atcform-0.1.1/src/ATCForm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 15:03:07.000000 atcform-0.1.1/src/ATCForm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 15:03:07.000000 atcform-0.1.1/src/ATCForm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 15:03:07.000000 atcform-0.1.1/src/ATCForm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 15:03:07.730022 atcform-0.1.1/src/ATCFrom/
--rw-rw-rw-   0        0        0    24115 2024-05-14 10:39:09.000000 atcform-0.1.1/src/ATCFrom/AUTO_VOLUNTEER.py
--rw-rw-rw-   0        0        0      151 2024-05-14 11:30:00.000000 atcform-0.1.1/src/ATCFrom/__init__.py
--rw-rw-rw-   0        0        0     1964 2024-05-14 10:46:08.000000 atcform-0.1.1/src/ATCFrom/examlpe.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.781194 atcform-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 15:47:09.000000 atcform-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1565 2024-05-14 16:11:58.779191 atcform-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2024-05-14 16:07:04.000000 atcform-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 11:46:25.000000 atcform-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 16:11:58.781194 atcform-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-05-14 16:11:41.000000 atcform-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.759962 atcform-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.778190 atcform-0.1.2/src/ATCForm.egg-info/
+-rw-rw-rw-   0        0        0     1565 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 16:11:58.000000 atcform-0.1.2/src/ATCForm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 16:11:58.776184 atcform-0.1.2/src/ATCFrom/
+-rw-rw-rw-   0        0        0    24411 2024-05-14 16:04:01.000000 atcform-0.1.2/src/ATCFrom/AUTO_FROM.py
+-rw-rw-rw-   0        0        0      140 2024-05-14 16:08:36.000000 atcform-0.1.2/src/ATCFrom/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-05-14 16:04:29.000000 atcform-0.1.2/src/ATCFrom/examlpe.py
```

### Comparing `atcform-0.1.1/setup.py` & `atcform-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ATCForm",
-    version="0.1.1",
+    version="0.1.2",
     description="ATCFrom - Automatically fill in the collection form 自动化表单填写工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YKONGCO/ATCForm",
     author="YKONGCO",
     author_email="1570585752@qq.com",
-    license=" MIT License",
+    maintainer="YKONGCO",
+    maintainer_email="1570585752@qq.com",
+    license="MIT License",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `atcform-0.1.1/src/ATCFrom/AUTO_VOLUNTEER.py` & `atcform-0.1.2/src/ATCFrom/AUTO_FROM.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,31 @@
         os.remove(file_path)
     download_driver_path = EdgeChromiumDriverManager().install()
     print(download_driver_path)
     shutil.move(download_driver_path, folder_path)
 
 
 
-class AUTO_JSJ_VOLUNTEER:
+class AUTO_JSJ_FROM:
     info_data={}
     select_list=[]
     wait_time :str 
     answer_list=[]
     
     def __init__(self,url : str ):
         options = webdriver.EdgeOptions()
-        # 处理SSL证书错误问题
         options.add_argument('--ignore-certificate-errors')
         options.add_argument('--ignore-ssl-errors')
         options.add_argument("--guest")
-        # 忽略无用的日志
         options.add_experimental_option("excludeSwitches", ['enable-automation', 'enable-logging'])
         try:
             self.driver=webdriver.Edge(options)
         except:
             download_driver()
-            self.driver=webdriver.Edge(options)
-        # self.driver.minimize_window() 
+            self.driver=webdriver.Edge(options) 
         self.actions = ActionChains(self.driver)
         try:
             self.driver.get(url)
         except:
             print("打开网页失败")
     
     
@@ -259,15 +256,15 @@
         except Exception as e:
             print(e)
             
 
     def __del__(self):
         self.driver.quit()
 
-class AUTO_TX_VOLUNTEER:
+class AUTO_TX_FROM:
     info_data={}
     select_list=[]
     wait_time :str 
     answer_list=[]
     
     def __init__(self,url : str ):
         options = webdriver.EdgeOptions()
@@ -556,14 +553,26 @@
 
         Args:
             url (str): 收集表地址
             data_path (str): 数据地址
             start_time (str): 开始时间 格式为202405121200 年月日时分(注意补零).
             is_enable (bool, optional): 是否提前输入需要选择内容 Defaults to True.
             SELECT_LIST (list, optional): 需要选择的内容. Defaults to [] 如["1","2"].
+            
+            
+            1.data.txt 格式要求
+            {
+                    "学号姓名":"",
+                    "手机号":"",
+                    "邮箱":"",
+                    "班级":"",
+                    "学院":"",
+                    "name":"value"
+            }        
+            
         """
         self.url=url
         self.data_path=data_path
         self.start_time=start_time
         self.is_enable=is_enable
         if(is_enable==False):
             self.SELECT_LIST=SELECT_LIST
@@ -571,18 +580,15 @@
     def run(self):
         self.AT1.wait_for_time()
         self.AT1.auto_input()
         self.AT1.auto_click_button()
         self.AT1.auto_submit_click_tx()
         
     def init(self):
-        #收集表链接
-        # url="https://docs.qq.com/form/page/DVUF0aEhvQWZUV3BW"
-        #开抢时间
-        self.AT1=AUTO_TX_VOLUNTEER(self.url)
+        self.AT1=AUTO_TX_FROM(self.url)
         self.AT1.set_wait_time(input_time=self.start_time)
         self.AT1.wait_for_login()
         self.AT1.set_base_data(self.data_path)
         if(self.is_enable==False):
             self.AT1.select_list+=self.SELECT_LIST
         self.AT1.display_all_qus()
         self.AT1.Initializes_the_answer_list()
@@ -595,60 +601,72 @@
         print("任务初始化完成")
         if(current_timestamp < start_timestamp-8):
             print("---------------------")
             print("进入等待时间(5s)，请确认输入结果")
             print("input信息：",self.AT1.answer_list)
             print("select信息：",self.AT1.select_list)
             time.sleep(5)
+            
+    def start(self):
+        self.init()
+        self.run()        
+    
+    
+    
+    
                
 class AuTotask_JSJ: 
     """
 
     """
     def __init__(self,url :str,data_path :str,start_time: str,is_enable=True,SELECT_LIST=[]) -> None:
         """初始化
-
         Args:
             url (str): 收集表地址
             data_path (str): 数据地址
             start_time (str): 开始时间 格式为202405121200 年月日时分(注意补零).
             is_enable (bool, optional): 是否提前输入需要选择内容 Defaults to True.
             SELECT_LIST (list, optional): 需要选择的内容. Defaults to [] 如["1","2"].
+            
+            1.data.txt 格式要求
+            {
+                    "学号姓名":"",
+                    "手机号":"",
+                    "邮箱":"",
+                    "班级":"",
+                    "学院":"",
+                    "name":"value"
+            }    
+            
         """
         self.url=url
         self.data_path=data_path
         self.start_time=start_time
         self.is_enable=is_enable
         if(is_enable==False):
             self.SELECT_LIST=SELECT_LIST
     def run(self):
         self.AJ1.wait_for_time()
         self.AJ1.auto_input()
         self.AJ1.auto_click_button()
         self.AJ1.auto_submit_click_JSJ()
         
     def init(self):
-        #收集表链接
-        # url="https://docs.qq.com/form/page/DVUF0aEhvQWZUV3BW"
-        #开抢时间
-        self.AJ1=AUTO_JSJ_VOLUNTEER(self.url)
+        self.AJ1=AUTO_JSJ_FROM(self.url)
         time.sleep(1)
         self.AJ1.set_wait_time(input_time=self.start_time)
-        # self.AJ1.wait_for_login()
         self.AJ1.set_base_data(self.data_path)
         if(self.is_enable==False):
             self.AJ1.select_list+=self.SELECT_LIST
         self.AJ1.display_all_qus()
         self.AJ1.Initializes_the_answer_list()
         if(self.AJ1.get_questions_select()!=[] and self.is_enable):
             self.AJ1.set_select_list()
-            
         current_timestamp = time.time()
         time_tuple = time.strptime(self.start_time, "%Y%m%d%H%M")
-        # 将时间元组转换为时间戳
         start_timestamp  = time.mktime(time_tuple)
         print("任务初始化完成")
         if(current_timestamp < start_timestamp-8):
             print("---------------------")
             print("进入等待时间(5s)，请确认输入结果")
             print("input信息：",self.AJ1.answer_list)
             print("select信息：",self.AJ1.select_list)
```

### Comparing `atcform-0.1.1/src/ATCFrom/examlpe.py` & `atcform-0.1.2/src/ATCFrom/examlpe.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 #     url (str): 收集表地址
 #     data_path (str): 数据地址
 #     start_time (str): 开始时间 格式为202405121200 年月日时分(注意补零).
 #     is_enable (bool, optional): 是否提前输入需要选择内容 Defaults to True.
 #     SELECT_LIST (list, optional): 需要选择的内容. Defaults to [] 如["1","2"].
 
 
-#金数据任务
-task1 = AT.AuTotask_JSJ(url="https://jinshuju.net/f/ddC0yC",
+#金
+task1 = AT.AuTotask_JSJ(url="https://...", #会自动解析选项稍后会在终端要求输入
                             data_path="./data.txt",
                             start_time="202405141734",
-                            is_enable=False,
-                            SELECT_LIST=["a"]
+                            # is_enable=False,
+                            # SELECT_LIST=["a"]
                             )
 
     
-task2 = AT.AuTotask_JSJ(url="https://jinshuju.net/f/bsHEay?submit_link_generated_from=poster",
+task2 = AT.AuTotask_JSJ(url="https://...",
                             data_path="./data.txt",
                             start_time="202405141200",
                             is_enable=False,
                             SELECT_LIST=["拍摄照片视频"]
                             )
     
-task3 = AT.AuTotask_JSJ(url="https://jinshuju.net/f/SnaRxI?submit_link_generated_from=poster",
+task3 = AT.AuTotask_JSJ(url="https://....",
                             data_path="./data.txt",
                             start_time="202405141230",
                             is_enable=False,
                             SELECT_LIST=["拍照摄影"]
                             )
 
 
-#腾讯文档任务
+#腾
 task3=AT.AuTotask_TX(url="https://......",
                            data_path="./data.txt",
                             start_time="202405141230",
                             is_enable=False,
                             SELECT_LIST=["拍照摄影"]
                            )
```

