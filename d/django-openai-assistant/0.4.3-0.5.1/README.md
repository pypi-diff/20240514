# Comparing `tmp/django_openai_assistant-0.4.3.tar.gz` & `tmp/django_openai_assistant-0.5.1.tar.gz`

## Comparing `django_openai_assistant-0.4.3.tar` & `django_openai_assistant-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/apps.py
--rw-r--r--   0        0        0    17800 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/assistant.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/models.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/src/django_openai_assistant/migrations/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/LICENSE
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 django_openai_assistant-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/apps.py
+-rw-r--r--   0        0        0    18196 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/assistant.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/models.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/src/django_openai_assistant/migrations/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/README.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.1/PKG-INFO
```

### Comparing `django_openai_assistant-0.4.3/src/django_openai_assistant/assistant.py` & `django_openai_assistant-0.5.1/src/django_openai_assistant/assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 import json
 import markdown
 from openai import OpenAI
 import importlib
 from .models import OpenaiTask
 
-_client = OpenAI( api_key=settings.OPENAI_API_KEY)
-
-
 def asmarkdown(text, replaceThis=None, withThis=None):
     ret = None
     if text != None:
         extension_configs = {
         'markdown_link_attr_modifier': {
         'new_tab': 'on',
         'no_referrer': 'external_only',
@@ -24,33 +21,29 @@
         if replaceThis != None and withThis != None:
             ret = markdown.markdown(text,extensions=['tables','markdown_link_attr_modifier'],extension_configs=extension_configs).replace(replaceThis,withThis)
         else:
             ret =markdown.markdown(text,extensions=['tables','markdown_link_attr_modifier'],extension_configs=extension_configs)
     return ret
 
 
-def getOpenaiClient():
-    return _client
-
-
 def createAssistant(name,instructions,model, tools):
     ''' Create an OpenAI Assistant programmatically
     parameters:
         name - name of the assistant 
         instructions - instructions for the assistant
         model - the model to use
         tools - an array of tools to use. They way we do it here is that we assume that the name of the function corresponds 
         to the name of the tool. So if you have a function called 'webscrape' it will be added to the tools array
         as a tool called 'webscrape'. When running an Assistant we will call the function 'webscrape' 
      
         Only use to create new Assistants in OpenAI!
         
     returns: the assistant object as created.  Assistant.id is the unique key that was assigned to the assistant.
     '''
-    client = getOpenaiClient()
+    client = OpenAI( api_key=settings.OPENAI_API_KEY)
     assistant = client.beta.assistants.create(
         name=name,
         instructions=instructions,
         tools=getTools(tools),
         model=model)
     return assistant
         
@@ -66,22 +59,22 @@
         id / assistant_id - the id of the assistant
         
         when called with no parameters it will return a list of all assistants
         
         returns: the OpenAI assistant object
         
     '''
-    client = getOpenaiClient()
+    client = OpenAI( api_key=settings.OPENAI_API_KEY)
     if len(kwargs.items())==0:
-        return client.beta.assistants.list()
+        return client.beta.assistants.list(limit=100)
 
     for key, value in kwargs.items():
         if key == 'name' or key == 'Name' or key == 'assistantName':
             Name = value
-            aa = client.beta.assistants.list()
+            aa = client.beta.assistants.list(limit=100)
             assistant = None
             for a in aa.data:
                 if a.name == Name:
                     assistant = a
                     break
         elif key == 'assistant_id' or key=="id":
             assistant = client.beta.assistants.retrieve(assistant_id=value)  
@@ -177,15 +170,15 @@
     
     fromTools is the array of outputs from each function
     
     After submitting we schedule the next status check to see if the run completed. 
     '''
     run_id = comboId.split(',')[0]
     thread_id = comboId.split(',')[1]
-    client = getOpenaiClient()
+    client = OpenAI( api_key=settings.OPENAI_API_KEY)
     print("Submit tool outputs "+run_id)
     output = []
     for o in fromTools:
         output.append( o["output"])
     try:
         run = client.beta.threads.runs.submit_tool_outputs(
         thread_id=thread_id,
@@ -208,15 +201,15 @@
         comboId - a runId,threadId combo in a string
         we use this because of the celery parameter passing simplicity
         
     '''
     run_id = comboId.split(',')[0]
     thread_id = comboId.split(',')[1]
     # Expects a  runid,threadid combo in a string
-    client = getOpenaiClient()
+    client = OpenAI( api_key=settings.OPENAI_API_KEY)
     run = client.beta.threads.runs.retrieve(thread_id=thread_id, run_id=run_id)
     if run.status == 'completed' or run.status == 'requires_action':
         # only then do we need the object to do something with. 
         task = OpenaiTask.objects.get(runId=run_id)
         if task==None:
             raise Exception('Run '+run_id+' not found in task table')
     
@@ -303,32 +296,33 @@
     
     @metadata.setter
     def metadata(self, value):
         self._metadata = value
         
     @prompt.setter
     def prompt(self, message):
+        att = [ {'file-id': id, 'tools': [{ "type": "file_search" },{ "type": "code_interpreter" }] } for id in self._fileids]
         self._startPrompt = message
         self.threadObject = self.client.beta.threads.create(messages=[] )
         self._message_id = self.client.beta.threads.messages.create(
         thread_id=self.thread_id,
         content=message,
-        file_ids=self._fileids,
+        attachments= att,
         role="user"
             )
     
     def __init__(self, **kwargs ):
         ''' Create an assistant task
         
         Two modes: create a new task or retrieve an existing (probably completed) task from the database
         
         if run_id is provided it will retrieve the task from the database. If not it will create a new task.
         
         '''
-        self.client = getOpenaiClient()
+        self.client = OpenAI( api_key=settings.OPENAI_API_KEY)
         self._fileids = []
         self._startPrompt = None
         self._message_id = None
         self.threadObject = None
         self.runObject = None
         self.messages = None
         self.status = None
@@ -415,32 +409,36 @@
         
     def markdownResponse(self, replaceThis=None, withThis=None):
         ''' returns the response with markdown formatting - convient for rendering in chat like responses
         '''
         return asmarkdown(self.response,replaceThis,withThis)
         
         
-    def uploadFile(self,file=None,fileContent=None,addToAssistant=True,filename=None):
+    def uploadFile(self,file=None,fileContent=None,filename=None,**kwargs):
         ''' Upload a file to openAI either for the Assistant or for the Thread.
         
         parameters:
             file - a file object
             fileContent - the content of the file
+            
             addToAssistant - if true will add the file to the assistant. If false will add it to the thread
+            *** Note addToAssistant is not currently supported due to the V2 changes. 
+            
             filename - the name of the file. If not provided will use the name of the file object
+            All uploaded files will automatically be provided in the message to the assistant with both search and code interpreter enabled.
         '''
         if fileContent == None:
             fileContent = file.read()
         uploadFile = self.client.files.create( file=(filename,fileContent),purpose='assistants')
-        if addToAssistant:
-            af = self.client.beta.assistants.files.create(assistant_id=self.assistant_id, file_id=uploadFile.id)
-            return af.id
-        else:
-            self._fileids.append(uploadFile.id)
-            return uploadFile.id
+        #if addToAssistant:
+        #    af = self.client.beta.assistants.files.create(assistant_id=self.assistant_id, file_id=uploadFile.id)
+        #    return af.id
+        #else:
+        self._fileids.append(uploadFile.id)
+        return uploadFile.id
         
     def getlastresponse(self):
         ''' Get the last response from the assistant, returns the data[] portion of the response
         '''
         messages = self.client.beta.threads.messages.list( thread_id=self.thread_id)
         return messages.data[0]
```

### Comparing `django_openai_assistant-0.4.3/src/django_openai_assistant/models.py` & `django_openai_assistant-0.5.1/src/django_openai_assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.4.3/src/django_openai_assistant/migrations/0001_initial.py` & `django_openai_assistant-0.5.1/src/django_openai_assistant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.4.3/LICENSE` & `django_openai_assistant-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.4.3/README.md` & `django_openai_assistant-0.5.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         print(task.markdownresponse())
     else:
         print('run failed')
 ```
 See https://medium.com/@jlvalorvc/building-a-scalable-openai-assistant-processor-in-django-with-celery-a61a1af722e0
 
 ## Version history:
+0.5.1
+- - Remove getopenaiclient() instead use OpenAI() everywhere
+- - Fix getAssistant() that could fail if retrieving an Assistant by name from an org with more than 20 Assistants.
+0.5.0
+- - Added support for Assistants 2.0. For now all files are added to a thread with support for both search and code completion. For now no support to upload files to a vectorstore to an Assistant. 
 0.4.3
 - - Added optional parameter temperature createRun() default is 1, like the OpenAI default
 
 0.4.2
 - Added optional parameter temperature createRun() default is 1, like the OpenAI default
 
 0.4.1
```

### Comparing `django_openai_assistant-0.4.3/pyproject.toml` & `django_openai_assistant-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-openai-assistant"
-version = "0.4.3"
+version = "0.5.1"
 dependencies = ["openai", "markdown"]
 readme = "README.md"
 authors = [{name = "Jean-Luc Vanhulst", email = "jl@valor.vc"}]
 maintainers = [{name = "Jean-Luc Vanhulst", email = "jl@valor.vc"}]
 classifiers = ["License :: OSI Approved :: MIT License"]
 urls = {Homepage = "https://github.com/jlvanhulst/django-openai"}
 keywords = ["django", "celery", "openai", "assistants"]
```

### Comparing `django_openai_assistant-0.4.3/PKG-INFO` & `django_openai_assistant-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-openai-assistant
-Version: 0.4.3
+Version: 0.5.1
 Summary: Django OpenAI Assistant
 Project-URL: Homepage, https://github.com/jlvanhulst/django-openai
 Author-email: Jean-Luc Vanhulst <jl@valor.vc>
 Maintainer-email: Jean-Luc Vanhulst <jl@valor.vc>
 License-File: LICENSE
 Keywords: assistants,celery,django,openai
 Classifier: License :: OSI Approved :: MIT License
@@ -56,14 +56,19 @@
         print(task.markdownresponse())
     else:
         print('run failed')
 ```
 See https://medium.com/@jlvalorvc/building-a-scalable-openai-assistant-processor-in-django-with-celery-a61a1af722e0
 
 ## Version history:
+0.5.1
+- - Remove getopenaiclient() instead use OpenAI() everywhere
+- - Fix getAssistant() that could fail if retrieving an Assistant by name from an org with more than 20 Assistants.
+0.5.0
+- - Added support for Assistants 2.0. For now all files are added to a thread with support for both search and code completion. For now no support to upload files to a vectorstore to an Assistant. 
 0.4.3
 - - Added optional parameter temperature createRun() default is 1, like the OpenAI default
 
 0.4.2
 - Added optional parameter temperature createRun() default is 1, like the OpenAI default
 
 0.4.1
```

