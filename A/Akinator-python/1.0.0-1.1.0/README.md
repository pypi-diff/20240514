# Comparing `tmp/Akinator-python-1.0.0.tar.gz` & `tmp/Akinator-python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akinator-python-1.0.0.tar", last modified: Mon May 13 19:03:25 2024, max compression
+gzip compressed data, was "Akinator-python-1.1.0.tar", last modified: Tue May 14 03:03:25 2024, max compression
```

## Comparing `Akinator-python-1.0.0.tar` & `Akinator-python-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:25.694667 Akinator-python-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:25.683830 Akinator-python-1.0.0/Akinator_python.egg-info/
--rw-rw-rw-   0        0        0     2981 2024-05-13 19:03:25.000000 Akinator-python-1.0.0/Akinator_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-13 19:03:25.000000 Akinator-python-1.0.0/Akinator_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:03:25.000000 Akinator-python-1.0.0/Akinator_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 19:03:25.000000 Akinator-python-1.0.0/Akinator_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2981 2024-05-13 19:03:25.694667 Akinator-python-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2024-05-13 19:03:05.000000 Akinator-python-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 19:03:25.692264 Akinator-python-1.0.0/akinator_python/
--rw-rw-rw-   0        0        0      121 2024-05-13 17:46:25.000000 Akinator-python-1.0.0/akinator_python/__init__.py
--rw-rw-rw-   0        0        0     3344 2024-05-13 17:48:13.000000 Akinator-python-1.0.0/akinator_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-13 19:03:25.694667 Akinator-python-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-05-13 17:51:04.000000 Akinator-python-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:03:25.281631 Akinator-python-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-14 03:03:25.276234 Akinator-python-1.1.0/Akinator_python.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-14 03:03:24.000000 Akinator-python-1.1.0/Akinator_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-14 03:03:24.000000 Akinator-python-1.1.0/Akinator_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:03:24.000000 Akinator-python-1.1.0/Akinator_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 03:03:24.000000 Akinator-python-1.1.0/Akinator_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3914 2024-05-14 03:03:25.276234 Akinator-python-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2024-05-14 03:02:57.000000 Akinator-python-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 03:03:25.276234 Akinator-python-1.1.0/akinator_python/
+-rw-rw-rw-   0        0        0      121 2024-05-14 02:40:48.000000 Akinator-python-1.1.0/akinator_python/__init__.py
+-rw-rw-rw-   0        0        0     4304 2024-05-14 02:56:02.000000 Akinator-python-1.1.0/akinator_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:03:25.281631 Akinator-python-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-14 02:41:02.000000 Akinator-python-1.1.0/setup.py
```

### Comparing `Akinator-python-1.0.0/Akinator_python.egg-info/PKG-INFO` & `Akinator-python-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,97 @@
-Metadata-Version: 2.1
-Name: Akinator-python
-Version: 1.0.0
-Summary: A API wrapper for the AkinatorAPI
-Home-page: https://github.com/taka-4602/Akinator-python
-Author: taka4602
-Author-email: shun4602@gmail.com
-Keywords: akinator
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Akinator-python
 A API wrapper for the AkinatorAPI
-### >>```pip install akinator-python```<<
+### >>```pip install akinator-python```<<  
+### 日本語は -> [README_ja](https://github.com/taka-4602/Akinator-python/blob/main/README_ja.md)
+## Requirement
+- requests
+- bs4
 ## Usage
 Install this module, download example.py and run  
 #### example.py
 ```py
 from akinator_python import Akinator
 
 akinator=Akinator(lang="en")
-print(akinator.start_game())
+akinator.start_game()
 while True:
-    ans=input("answer：")
-    if ans=="b":
-        print(akinator.go_back()['question'])
-    else:
-        response=akinator.post_answer(ans)
-        if "id_proposition" in response:
-            print(f"{response['name_proposition']} / {response['description_proposition']}")
-            ans=input("is it correct?：")
-            if ans=="n":
-                print(akinator.exclude()['question'])
-            elif ans=="y":
-                break
+    try:
+        print(akinator.question)
+        ans=input("answer：")
+        if ans=="b":
+            akinator.go_back()
         else:
-            print(response['question'])
+            akinator.post_answer(ans)
+            if akinator.answer_id:
+                print(f"{akinator.name} / {akinator.description}")
+                ans=input("is it correct?：")
+                if ans=="n":
+                    akinator.exclude()
+                elif ans=="y":
+                    break
+                else:
+                    break
+    except Exception as e:
+        print(e)
+        continue
 ```
 I have prepared a super simple example code  
 You can just run and enjoy it in terminal :)  
 ![0](https://raw.githubusercontent.com/taka-4602/Akinator-python/main/images/0.png)  
 ## Know a little more
 ```Akinator()```  
 - You can set language, theme, child mode in arguments  
 - ```language=str```, The endpoint URL is determined based on this argument  
   If nothing is specified, ```lang=jp``` Japanese will be selected  
 - ```theme=str```, ```characters``` or ```objects``` or ```animals```  
   If nothing is specified, ```theme=characters``` characters will be selected
 - ```child_mode=bool```  
   default is ```False```
+
+```Akinator.start_game()```  
+- Start the Akinator game  
+  it will return a first question in str
   
 ```Akinator.post_answer()```  
 - ```answer=str```  
   Answers are Yes : ```y``` No : ```n``` I don't know : ```idk``` probably : ```p``` probably not : ```pn```
-- it will return a dict
-  ```
-  {'completion': 'OK', 'akitude': 'serein.png', 'step': '1', 'progression': '0.00000',
-   'question_id': '464', 'question': 'Is your character a girl?'}
-  ```
   
 ```Akinator.go_back()```  
 - Yes, you can go back to the previous question
 
 ```Akinator.exclude()```  
 - If Akinator's answer is incorrect, you can restart the question
-### When Akinator makes a guess
+
+```Akinator.step```  
+- Always ```int```, you can check the number of questions
+
+```Akinator.progression```  
+- Always ```float```, progress of Akinator's "guess"
+
+```Akinator.question```  
+- Always ```str```, just a question
+
+## When Akinator makes a guess
+```Akinator.name```  
+- Default is ```None```, when it becomes available ```str```, Character name guessed by Akinator
+
+```Akinator.description```  
+- Same as ```.name```, Character description guessed by Akinator
+
+```Akinator.description```  
+- Same as ```.name```, photo URL in ```str``` Character photo guessed by Akinator
+# Supplement
+```.post_ansewer()``` ```.go_back()``` ```.exclude()``` are ruturn a dict  
+#### Question in progress
+```
+{'completion': 'OK', 'akitude': 'serein.png', 'step': '1', 'progression': '0.00000',
+ 'question_id': '464', 'question': 'Is your character a girl?'}
+```
+#### When Akinator makes a guess
 ```
 {'completion': 'OK', 'id_proposition': '309720', 'id_base_proposition': '10657795', 'valide_contrainte': '1',
  'name_proposition': 'Arihara Nanami', 'description_proposition': 'Riddle Joker', 
  'flag_photo': '2', 'photo': 'https://photos.clarinea.fr/BL_2_en/600/partenaire/p/10657795__894179331.png', 'pseudo': 'MrSand', 'nb_elements': 1}
-```
-It will return the character name, image URL and more  
+``` 
 ## Contacts  
 Discord server / https://discord.gg/aSyaAK7Ktm  
 Discord username / .taka.
```

### Comparing `Akinator-python-1.0.0/akinator_python/main.py` & `Akinator-python-1.1.0/akinator_python/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,87 +2,109 @@
 from bs4 import BeautifulSoup
 
 class AkinatorError(Exception):
     pass
 class Akinator():
     def __init__(self,theme:str="characters",lang:str="jp",child_mode:bool=False) -> None:
         self.ENDPOINT=f"https://{lang}.akinator.com/"
+        self.name=None
+        self.description=None
+        self.photo=None
+        self.answer_id=None
         if theme=="characters":
             sid=1
         elif theme=="objects":
             sid=2
         elif theme=="animals":
             sid=14
         else:
-            raise AkinatorError("the theme must be characters / objects / animals")
+            raise AkinatorError("the theme must be 'characters' / 'objects' / 'animals'")
         self.session=requests.session()
-        self.progress={
+        self.json={
             "step":0,
             "progression":0.0,
             "sid":sid,
             "cm":child_mode,
             "answer":0,
         }
 
     def start_game(self):
-        game=self.session.post(f"{self.ENDPOINT}game",json={"sid":self.progress["sid"],"cm":self.progress["cm"]}).text
+        game=self.session.post(f"{self.ENDPOINT}game",json={"sid":self.json["sid"],"cm":self.json["cm"]}).text
         soup = BeautifulSoup(game,"html.parser")
         askSoundlike=soup.find(id="askSoundlike")
         question_label=soup.find(id="question-label").get_text()
         session_id=askSoundlike.find(id="session").get("value")
         signature_id=askSoundlike.find(id="signature").get("value")
-        self.progress["session"]=session_id
-        self.progress["signature"]=signature_id
+        self.json["session"]=session_id
+        self.json["signature"]=signature_id
+        self.step=0
+        self.progression=0.0
+        self.question=question_label
         return question_label
 
     def post_answer(self,answer:str):
         if answer=="y":
-            self.progress["answer"]=0
+            self.json["answer"]=0
         elif answer=="n":
-            self.progress["answer"]=1
+            self.json["answer"]=1
         elif answer=="idk":
-            self.progress["answer"]=2
+            self.json["answer"]=2
         elif answer=="p":
-            self.progress["answer"]=3
+            self.json["answer"]=3
         elif answer=="pn":
-            self.progress["answer"]=4
+            self.json["answer"]=4
         else:
-            raise AkinatorError("the answer must be y / n / idk / p / pn")
+            raise AkinatorError("the answer must be 'y' / 'n' / 'idk' / 'p' / 'pn'")
         try:
-            progression=self.session.post(f"{self.ENDPOINT}answer",json=self.progress)
+            progression=self.session.post(f"{self.ENDPOINT}answer",json=self.json)
             progression=progression.json()
             if progression["completion"]=="KO":
                 raise AkinatorError("completion : KO")
             try:
-                self.progress["step"]=int(progression["step"])
-                self.progress["progression"]=float(progression["progression"])
+                self.json["step"]=int(progression["step"])
+                self.json["progression"]=float(progression["progression"])
+                self.step=int(progression["step"])
+                self.progression=float(progression["progression"])
+                self.question=progression["question"]
+                self.question_id=progression["question_id"]
             except:
-                None
+                self.name=progression["name_proposition"]
+                self.description=progression["description_proposition"]
+                self.photo=["photo"]
+                self.answer_id=progression["id_proposition"]
             return progression
         except:
             raise AkinatorError(progression.text)
 
     def go_back(self):
-        if self.progress["step"]==0:
+        if self.json["step"]==0:
             raise AkinatorError("it's first question")
-        if "answer" in self.progress:
-            del self.progress["answer"]
+        if "answer" in self.json:
+            del self.json["answer"]
         try:
-            goback=self.session.post(f"{self.ENDPOINT}cancel_answer",json=self.progress)
+            goback=self.session.post(f"{self.ENDPOINT}cancel_answer",json=self.json)
             goback=goback.json()
-            self.progress["step"]=int(goback["step"])
-            self.progress["progression"]=float(goback["progression"])
+            self.json["step"]=int(goback["step"])
+            self.json["progression"]=float(goback["progression"])
+            self.step=int(goback["step"])
+            self.progression=float(goback["progression"])
+            self.question=goback["question"]
+            self.question_id=goback["question_id"]
             return goback
         except:
             raise AkinatorError(goback.text)
 
     def exclude(self):
-        if "answer" in self.progress:
-            del self.progress["answer"]
+        if "answer" in self.json:
+            del self.json["answer"]
         try:
-            exclude=self.session.post(f"{self.ENDPOINT}exclude",json=self.progress)
+            exclude=self.session.post(f"{self.ENDPOINT}exclude",json=self.json)
             exclude=exclude.json()
-            self.progress["step"]=int(self.progress["step"])
-            self.progress["progression"]=float(self.progress["progression"])
+            self.json["step"]=int(self.json["step"])
+            self.json["progression"]=float(self.json["progression"])
+            self.step=int(exclude["step"])
+            self.progression=float(exclude["progression"])
+            self.question=exclude["question"]
+            self.question_id=exclude["question_id"]
             return exclude
         except:
             raise AkinatorError(exclude.text)
```

### Comparing `Akinator-python-1.0.0/setup.py` & `Akinator-python-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Akinator-python',
-    version='1.0.0',
+    version='1.1.0',
     keywords = "akinator",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Akinator-python',
     description='A API wrapper for the AkinatorAPI',
```

