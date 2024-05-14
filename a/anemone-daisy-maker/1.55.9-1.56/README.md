# Comparing `tmp/anemone_daisy_maker-1.55.9.tar.gz` & `tmp/anemone_daisy_maker-1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.9.tar", last modified: Mon May 13 14:58:33 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.56.tar", last modified: Tue May 14 06:57:25 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.9.tar` & `anemone_daisy_maker-1.56.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.894920 anemone_daisy_maker-1.55.9/
--rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 14:58:33.894419 anemone_daisy_maker-1.55.9/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.890592 anemone_daisy_maker-1.55.9/anemone/
--rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-13 14:58:33.893784 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)     6838 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      308 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/requires.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-13 14:58:33.895054 anemone_daisy_maker-1.55.9/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)     7086 2024-05-13 14:58:33.000000 anemone_daisy_maker-1.55.9/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 06:45:18.000000 anemone_daisy_maker-1.56/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6889 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    10238 2024-05-14 06:45:20.000000 anemone_daisy_maker-1.56/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6889 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      326 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6987 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/setup.py
```

### Comparing `anemone_daisy_maker-1.55.9/PKG-INFO` & `anemone_daisy_maker-1.56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.55.9
+Version: 1.56
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
+Home-page: UNKNOWN
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: mutagen
-
+License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
 `anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
@@ -62,7 +64,8 @@
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
 * Windows is a registered trademark of Microsoft Corp.
 
 * Any other trademarks I mentioned without realising are trademarks of their respective holders.
+
```

### Comparing `anemone_daisy_maker-1.55.9/anemone/__init__.py` & `anemone_daisy_maker-1.56/anemone/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Anemone 1.55 (http://ssb22.user.srcf.net/anemone)
+Anemone 1.56 (http://ssb22.user.srcf.net/anemone)
 (c) 2023-24 Silas S. Brown.  License: Apache 2
 
 To use this module, either run it from the command
 line, or import it and use the anemone() function.
 """
 
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -22,15 +22,15 @@
 # Where to find history:
 # on GitHub at https://github.com/ssb22/indexer
 # and on GitLab at https://gitlab.com/ssb22/indexer
 # and on BitBucket https://bitbucket.org/ssb22/indexer
 # and at https://gitlab.developers.cam.ac.uk/ssb22/indexer
 # and in China: https://gitee.com/ssb22/indexer
 
-def anemone(*files,**options):
+def anemone(*files,**options) -> list[str]:
     """This function can be called by scripts that
     import anemone: simply put the equivalent of
     the command line into 'files' and 'options'.
     You can also specify a JSON dictionary instead
     of the name of a JSON file, and/or an HTML
     string instead of the name of an HTML file
     (this can also be done on the command line
@@ -40,20 +40,26 @@
     Return value is a list of warnings, if any.
 
     Other functions below are generally for
     internal use and are of interest only if you
     want to maintain Anemone, although you might
     find {fetch(), deBlank(), version} useful."""
     
-    R=Run(*[(json.dumps(f) if isinstance(f,dict) else f) for f in files],**options)
-    if R.mp3_recode or any(f.strip().lower().endswith(f"{os.extsep}wav") for f in files if isinstance(f,str)): check_we_got_LAME()
+    R=Run(*[(json.dumps(f) if isinstance(f,dict)
+             else f) for f in files],**options)
+    if R.mp3_recode or any(f.strip().lower().
+                           endswith(
+                               f"{os.extsep}wav")
+                           for f in files
+                           if isinstance(f,str)):
+        check_we_got_LAME()
     write_all(R,get_texts(R))
     return R.warnings
 
-def populate_argument_parser(args):
+def populate_argument_parser(args) -> None:
     """Calls add_argument on args, with the names
     of all Anemone command-line options, which are
     also options for anemone(), and help text.
     This is also used for runtime module help."""
     
     args.add_argument("files",metavar="file",
                       nargs="+",help="""
@@ -178,15 +184,18 @@
 
 generator=__doc__.strip().split('\n')[0] # string we use to identify ourselves in HTTP requests and in Daisy files
 
 def get_argument_parser():
     "populates an ArgumentParser for Anemone"
     
     from argparse import ArgumentParser
-    args = ArgumentParser(prog="anemone",description=generator,fromfile_prefix_chars='@')
+    args = ArgumentParser(
+        prog="anemone",
+        description=generator,
+        fromfile_prefix_chars='@')
     populate_argument_parser(args)
     return args
 
 import time, sys, os, re, json
 import textwrap
 from collections import namedtuple as NT
 from functools import reduce
@@ -201,18 +210,20 @@
 from pathlib import Path # Python 3.5+
 from shutil import which
 
 class DocUpdater:
     def __init__(self,p):
         self.p = p
         self.p.__doc__ += "\nOptions when run as a command-line utility:\n"
-    def add_argument(self,*args,**kwargs): self.p.__doc__ += f"\n* {(chr(10)+'  ').join(textwrap.wrap((args[0]+': ' if args[0].startswith('--') else '')+re.sub(chr(10)+' *',' ',kwargs['help']).strip(),50))}\n"
-populate_argument_parser(DocUpdater(sys.modules[__name__])) ; del DocUpdater
+    def add_argument(self,*args,**kwargs):
+        self.p.__doc__ += f"\n* {(chr(10)+'  ').join(textwrap.wrap((args[0]+': ' if args[0].startswith('--') else '')+re.sub(chr(10)+' *',' ',kwargs['help']).strip(),50))}\n"
+populate_argument_parser(DocUpdater(
+    sys.modules[__name__])) ; del DocUpdater
 
-def error(m):
+def error(m) -> None:
     """Anemone error handler.  If running as an
     application, print message and error-exit.  If
     running as a module, raise an AnemoneError."""
     
     if __name__=="__main__": sys.stderr.write(f"Error: {m}\n"),sys.exit(1)
     else: raise AnemoneError(str(m))
 class AnemoneError(Exception): pass
@@ -221,26 +232,35 @@
 except ImportError: error("Anemone needs the Mutagen library to determine play lengths.\nPlease do: pip install mutagen")
 from io import BytesIO
 
 class Run():
   """The parameters we need for an Anemone run.
   Constructor can either parse args from the
   command line, or from anemone() caller."""
-  def __init__(R,*inFiles,**kwargs):
-    # I know the convention is "self" but I am
-    # working in giant print so my screen area
-    # is important, so 1 letter please...
+  def __init__(self,*inFiles,**kwargs):
+    R = self
     R.audioData,R.filenameTitles = [],[]
     R.jsonData = []
     R.textData,R.htmlData = [],[]
     R.imageFiles,R.outputFile = [],None
     R.warnings = []
-    if inFiles: R.__dict__.update(get_argument_parser().parse_args(list(inFiles)+[a for k,v in kwargs.items() for a in ['--'+k.replace('_','-'),str(v)] if type(v) in [str,int]]).__dict__) # module
-    else: R.__dict__.update(get_argument_parser().parse_args().__dict__) # command line
-    R.__dict__.update((k,v) for k,v in kwargs.items() if type(v) not in [str,int,type(None)]) # (None means keep the default from parse_args; boolean and bytes we might as well handle directly; list e.g. merge_books should bypass parser; ditto session object for cache, a type we can't even name here if requests_cache is not installed)
+    if inFiles: # being called as a module
+        R.__dict__.update(
+            get_argument_parser().parse_args(
+                list(inFiles)+
+                [a for k,v in kwargs.items()
+                 for a in
+                 ['--'+k.replace('_','-'),str(v)]
+                 if type(v) in [str,int]])
+            .__dict__)
+    else: # being called from the command line
+        R.__dict__.update(get_argument_parser().parse_args().__dict__)
+    R.__dict__.update((k,v)
+                      for k,v in kwargs.items()
+                      if type(v) not in [str,int,type(None)]) # (None means keep the default from parse_args; boolean and bytes we might as well handle directly; list e.g. merge_books should bypass parser; ditto session object for cache, a type we can't even name here if requests_cache is not installed)
     for k in ['merge_books','chapter_titles']:
         if not isinstance(R.__dict__[k],list): R.__dict__[k]=R.__dict__[k].split(',') # comma-separate if coming from the command line, but allow lists to be passed in to the module
     for f in R.files:
         fOrig = f
         if f.lower().endswith(f"{os.extsep}zip"):
             if R.outputFile: error(f"Only one {os.extsep}zip output file may be specified")
             R.outputFile = f ; continue
@@ -264,47 +284,59 @@
     if not R.audioData: error("Creating DAISY files without audio is not yet implemented")
     if R.htmlData and not R.jsonData: error("Full text without time markers is not yet implemented")
     if R.jsonData and not R.htmlData: error("Time markers without full text is not implemented")
     if R.htmlData and R.textData: error("Combining full text with title-only text files is not yet implemented.  Please specify full text for everything or just titles for everything, not both.")
     if R.jsonData and not len(R.audioData)==len(R.jsonData): error(f"If JSON marker files are specified, there must be exactly one JSON file for each recording file.  We got f{len(R.jsonData)} JSON files and f{len(R.audioData)} recording files.")
     if R.textData and not len(R.audioData)==len(R.textData): error(f"If text files are specified, there must be exactly one text file for each recording file.  We got f{len(R.textData)} text files and f{len(R.audioData)} recording files.")
     if R.htmlData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
-    if not R.outputFile: R.outputFile=f"output_daisy{os.extsep}zip"
+    if not R.outputFile:
+        R.outputFile=f"output_daisy{os.extsep}zip"
     if not R.title: R.title=R.outputFile.replace(f"{os.extsep}zip","").replace("_daisy","")
-  def warning(R,warningText):
-      R.warnings.append(warningText) ; sys.stderr.write(f"WARNING: {warningText}\n")
+  def warning(self,warningText):
+    self.warnings.append(warningText)
+    sys.stderr.write(f"WARNING: {warningText}\n")
 
-def delimited(s,start,end):
+def delimited(s,start:int,end:int) -> bool:
     """Checks to see if a string or binary data
     is delimited by start and end, converting as
     needed, after stripping"""
     if isinstance(s,bytes):
         s = s.replace(b"\xEF\xBB\xBF",b"").strip() # just in case somebody's using UTF-8 BOMs
         return s.startswith(start.encode('latin1')) and s.endswith(end.encode('latin1'))
     else: # string; assume no BOM to skip
         s = s.strip()
         return s.startswith(start) and s.endswith(end)
 
-def check_for_JSON_transcript(R):
+def check_for_JSON_transcript(R) -> None:
     """Checks to see if the last thing added to
     the Run object is a JSON podcast transcript,
     and converts it to HTML + time markers"""
     
-    if isinstance(R.jsonData[-1].get("segments",None),list) and all(isinstance(s,dict) and "startTime" in s and "body" in s for s in R.jsonData[-1]["segments"]): # looks like JSON transcript format instead of markers format
+    if isinstance(R.jsonData[-1].get(
+            "segments",None),list) and all(
+                isinstance(s,dict) and
+                "startTime" in s and "body" in s
+                for s in R.jsonData[-1]["segments"]): # looks like JSON transcript format instead of markers format
         curSpeaker=None ; bodyList = []
         for s in R.jsonData[-1]["segments"]:
             bodyList.append(s["body"])
             s=s.get("speaker",curSpeaker)
             if not s==curSpeaker:
                 curSpeaker,bodyList[-1] = s,f"[{s}] {bodyList[-1]}"
-                if len(bodyList)>1: bodyList[-2] += "<br>"
-        R.htmlData.append(' '.join(f'<span {R.marker_attribute}="{i}">{c}</span>' for i,c in enumerate(bodyList) if c))
-        R.jsonData[-1]={"markers":[{"id":f"{i}","time":t} for i,t in enumerate(s["startTime"] for s in R.jsonData[-1]["segments"]) if bodyList[i]]}
+                if len(bodyList)>1:
+                    bodyList[-2] += "<br>"
+        R.htmlData.append(' '.join(
+            f'<span {R.marker_attribute}="{i}">{c}</span>' for i,c in enumerate(bodyList) if c))
+        R.jsonData[-1]={"markers":[
+            {"id":f"{i}","time":t}
+            for i,t in enumerate(
+                    s["startTime"] for s in R.jsonData[-1]["segments"])
+            if bodyList[i]]}
 
-def check_we_got_LAME():
+def check_we_got_LAME() -> None:
     """Complains if a LAME binary is not
     available on this system.  Makes a little
     extra effort to find one on Windows."""
     
     if which('lame'): return
     if sys.platform=='win32':
         os.environ["PATH"] += r";C:\Program Files (x86)\Lame for Audacity;C:\Program Files\Lame for Audacity"
@@ -314,15 +346,15 @@
 PageInfo = NT('PageInfo',['duringId','pageNo'])
 TagAndText = NT('TagAndText',['tag','text'])
 TextsAndTimesWithPages = NT('TextsAndTimesWithPages',['textsAndTimes','pageInfos'])
 ChapterTOCInfo = NT('ChapterTOCInfo',['hTag','hLine','itemNo'])
 BookTOCInfo = NT('BookTOCInfo',['hTag','hLine','recNo','itemNo'])
 del NT
 
-def get_texts(R):
+def get_texts(R) -> list:
     """Gets the text markup required for the run,
     extracting it from HTML (guided by JSON IDs)
     if we need to do that."""
     
     if R.textData: return R.textData # section titles only, from text files
     elif not R.htmlData: return R.filenameTitles # section titles only, from sound filenames
     recordingTexts = []
@@ -342,15 +374,20 @@
                 self.imgsMaybeAddTo = None
                 self.pageNoGoesAfter = 0
                 self.theStartTag = None
             def handle_starttag(self,tag,attrs):
                 tag = tagRewrite.get(tag,tag)
                 attrs = dict(attrs)
                 imgURL = attrs.get(R.image_attribute,None)
-                if imgURL and (re.match("https?://.*[.][^/]*$",imgURL) or os.path.isfile(imgURL)) and not (self.addTo is None and self.imgsMaybeAdd is None):
+                if imgURL and (re.match(
+                        "https?://.*[.][^/]*$",
+                        imgURL) or os.path.isfile(
+                            imgURL)) and not (
+                                self.addTo is None
+                                and self.imgsMaybeAdd is None):
                     # TODO: might want to check attrs.get("alt",""), but DAISY3 standard does not list alt as a valid attribute for img, so we'd have to put it after with br etc (changing text_htm) and we don't know if it's in the audio or not: probably best just to leave it and rely on there being a separate caption with ID if it's in the audio
                     img = f'<img src="{(R.imageFiles.index(imgURL) if imgURL in R.imageFiles else len(R.imageFiles))+1}{imgURL[imgURL.rindex("."):]}" {f"""id="i{R.imageFiles.index(imgURL) if imgURL in R.imageFiles else len(R.imageFiles)}" """ if R.daisy3 else ""}/>' # will be moved after paragraph by text_htm
                     if imgURL not in R.imageFiles:
                         R.imageFiles.append(imgURL)
                     if self.addTo is None: self.imgsMaybeAdd.append(img)
                     else: self.addTo.append(img)
                 if attrs.get(R.marker_attribute,None) in want_pids:
@@ -366,15 +403,16 @@
                 elif self.addTo is not None and tag in allowedInlineTags: self.addTo.append(f'<{allowedInlineTags[tag]}>')
                 elif self.addTo is not None and tag=='a': self.lastAStart = len(self.addTo)
                 elif tag=='rt': self.suppress += 1
                 pageNo = attrs.get(R.page_attribute,None)
                 if pageNo: pageNos.append(PageInfo(self.pageNoGoesAfter,pageNo))
             def handle_endtag(self,tag):
                 tag = tagRewrite.get(tag,tag)
-                if self.suppress and tag=='rt': self.suppress -= 1
+                if self.suppress and tag=='rt':
+                    self.suppress -= 1
                 elif self.addTo is not None:
                     if tag==self.theStartTag and self.tagDepth == 0:
                         self.highestImage,self.imgsMaybeAddTo, self.imgsMaybeAdd = len(R.imageFiles),self.addTo,[] # if we find any images (not in an id'd element) after the end of the id'd element, we might want to add them in with any inside it, but only if there's another id'd element after them i.e. not if they're just random decoration at the bottom of the page
                         self.addTo = None
                     elif tag in allowedInlineTags: self.addTo.append(f'</{allowedInlineTags[tag]}>')
                     elif tag=="a" and re.match('[!-.:-~]$',"".join(self.addTo[self.lastAStart:]).strip()): del self.addTo[self.lastAStart:] # remove single-character link, probably to footnote (we won't know if it's in the audio or not, we're not supporting jumps and the symbols might need normalising) but do allow numbers (might be paragraph numbers etc) and non-ASCII (might be single-character CJK word)
                     if tag==self.theStartTag and self.tagDepth: self.tagDepth -= 1
@@ -392,104 +430,125 @@
             if want_pids[i] in id_to_content:
                 tag,content = id_to_content[want_pids[i]]
                 content = ''.join(content).strip()
                 rTxt.append(TagAndText(tag,content_fixes(content)))
             else:
                 R.warning(f"JSON {len(recordingTexts)+1} marker {i+1} marks paragraph ID {want_pids[i]} which is not present in HTML {len(recordingTexts)+1}.  Anemone will make this a blank paragraph.")
                 rTxt.append(TagAndText('p',''))
-        recordingTexts.append(TextsAndTimesWithPages(rTxt,pageNos))
+        recordingTexts.append(
+            TextsAndTimesWithPages(rTxt,pageNos))
     return recordingTexts
 
 tagRewrite = { # used by get_texts
     'legend':'h3', # used in fieldset
 }
 
-def content_fixes(content):
+def content_fixes(content:str) -> str:
     """Miscellaneous fixes for final XML/XHTML
     to work around some issues with readers"""
     content = easyReader_em_fix(content)
     content = re.sub('( *</?br> *)+',' <br />',content) # allow line breaks inside paragraphs, in case any in mid-"sentence", but collapse them because readers typically add extra space to each, plus add a space beforehand in case any reader doesn't render the linebreak (e.g. EasyReader 10 in a sentence span)
     return content
 
-def easyReader_em_fix(content):
+def easyReader_em_fix(content:str) -> str:
     """EasyReader 10 workaround: it does not show
     strong or em, which is OK but it puts space
     around it: no good if it happened after a "("
     or similar, so delete those occurrences"""
     while True:
-        c2 = re.sub(r"<(?P<tag>(strong|em))>(.*?)</(?P=tag)>",lambda m:easyReader_em_fix(m.group(3)) if m.start() and content[m.start()-1] not in ' >' or m.end()<len(content) and content[m.end()] not in ' <' else f"<{m.group(1)}>{easyReader_em_fix(m.group(3))}</{m.group(1)}>",content)
+        c2 = re.sub(
+            r"<(?P<tag>(strong|em))>(.*?)</(?P=tag)>",
+            lambda m:easyReader_em_fix(m.group(3))
+            if m.start() and
+            content[m.start()-1] not in ' >'
+            or m.end()<len(content) and
+            content[m.end()] not in ' <'
+            else f"<{m.group(1)}>{easyReader_em_fix(m.group(3))}</{m.group(1)}>",
+            string = content)
         if c2==content: break
         content = c2 # and re-check
     return content
 
-def jsonAttr(d,suffix):
+def jsonAttr(d:dict,suffix:str) -> str:
     """Returns the value of a dictionary key whose
     name ends with the given lower-case suffix
     (after converting names to lower case), after
     checking exactly one key does this.  Used for
     checking JSON for things like paragraphId if
     you know only that it ends with 'Id'"""
     
     keys = [k for k in d.keys() if k.lower().endswith(suffix)]
     if not keys: error(f"No *{suffix} in {repr(keys)}")
     if len(keys)>1: error(f"More than one *{suffix} in {repr(keys)}")
     return str(d[keys[0]])
 
-def parseTime(t):
+def parseTime(t:str) -> float:
     """Parses a string containing seconds,
     minutes:seconds or hours:minutes:seconds
     (decimal fractions of seconds allowed),
     and returns floating-point seconds"""
     
     tot = 0.0 ; mul = 1
     for u in reversed(t.split(':')):
         tot += float(u)*mul ; mul *= 60
     return tot
 
-def write_all(R,recordingTexts):
+def write_all(R:Run,recordingTexts) -> None:
     """Writes the DAISY zip and everything in it.
     Each item of recordingTexts is either 1 text
     for section title of whole recording, or a
     TextsAndTimesWithPages i.e. ([TagAndText,time,
     TagAndText,time,TagAndText],[PageInfo,...])"""
     
     assert len(R.audioData) == len(recordingTexts)
     headings = getHeadings(R,recordingTexts)
     if R.dry_run: return sys.stderr.write(f"Dry run: {len(R.warnings) if R.warnings else 'no'} warning{'' if len(R.warnings)==1 else 's'} for {R.outputFile}\n")
     merge0lenSpans(recordingTexts,headings)
-    if R.mp3_recode or any('audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData): # parallelise lame if possible
-        if not __name__=="__main__": sys.stderr.write(f"Making {R.outputFile}...\n"),sys.stderr.flush() # especially if repeatedly called, print which outputFile we're working on BEFORE the mp3s also
-        executor = ThreadPoolExecutor(max_workers=cpu_count())
-        recordingTasks=[executor.submit((recodeMP3 if R.mp3_recode or 'audio/mp3' not in mutagen.File(BytesIO(dat)).mime else lambda x:x),dat) for dat in R.audioData]
+    if R.mp3_recode or any(
+            'audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData): # parallelise lame if possible
+        if not __name__=="__main__":
+            sys.stderr.write(f"Making {R.outputFile}...\n"),sys.stderr.flush() # especially if repeatedly called, print which outputFile we're working on BEFORE the mp3s also
+        executor = ThreadPoolExecutor(
+            max_workers=cpu_count())
+        recordingTasks=[executor.submit(
+            (recodeMP3 if
+             R.mp3_recode or
+             'audio/mp3' not in mutagen.File(BytesIO(dat)).mime
+             else lambda x:x),
+            dat) for dat in R.audioData]
     else: executor,recordingTasks = None,None
-    try: _write0(R,recordingTexts,headings,recordingTasks)
+    try: write_all0(R,recordingTexts,headings,recordingTasks)
     except: # unhandled exception: clean up
         try: executor.shutdown(wait=False,cancel_futures=False) # (cancel_futures is Python 3.9+)
         except: pass # (no executor / can't do it) # noqa: E722
         try: os.remove(R.outputFile) # incomplete
         except: pass # noqa: E722
         raise
-def _write0(R,recordingTexts,headings,recordingTasks):
-    if os.sep in R.outputFile: Path(R.outputFile[:R.outputFile.rindex(os.sep)]).mkdir(parents=True,exist_ok=True)
+def write_all0(R:Run,recordingTexts,headings,recordingTasks) -> None:
+    "Service function for write_all"
+    if os.sep in R.outputFile:
+        Path(R.outputFile[:R.outputFile.rindex(os.sep)]).mkdir(parents=True,exist_ok=True)
     z = ZipFile(R.outputFile,"w",ZIP_DEFLATED,True)
     R.dataSectors = R.catalogueEntries = 0
     def writestr(n,s):
         if isinstance(s,bytes): L = len(s)
         else: L = len(s.encode('utf-8'))
         R.dataSectors += (L+2047)//2048 # ISO 9660 sectors on a CD-ROM
         R.catalogueEntries += 1
         # Assume roughly 64 entries per catalogue sector (TODO check), *3 for RockRidge/Joliet
         # Also 16 sectors are unused before start
         # 333,000 sectors on original 650M CD-ROM, TODO: we can probably increase that if 650M CDs are not in use, but some non-CD readers can still go wrong when files greatly exceed this size
-        if 3*((R.catalogueEntries+63)//64) + R.dataSectors + 16 > 333000 and not hasattr(R,"warnedFull"):
+        if 3*((R.catalogueEntries+63)//64) + R.dataSectors + 16 > 333000 \
+           and not hasattr(R,"warnedFull"):
             R.warnedFull = True
             R.warning(f"{R.outputFile} is too big for some DAISY readers")
         z.writestr(n,s)
     def D(s): return s.replace("\n","\r\n") # in case old readers require DOS line endings
-    hasFullText = any(isinstance(t,TextsAndTimesWithPages) for t in recordingTexts)
+    hasFullText = any(isinstance(t,TextsAndTimesWithPages)
+                      for t in recordingTexts)
     if hasFullText: writestr("0000.txt",D(f"""
     If you're reading this, it likely means your
     operating system has unpacked the ZIP file
     and is showing you its contents.  While it
     is possible to extract recordings and text
     this way, it is better to send the whole ZIP
     to a DAISY reader so that its recordings and
@@ -502,42 +561,79 @@
     instead, or at the whole directory/folder.
 """)) # TODO: message in other languages?
     # (it's iOS users that need the above, apparently.  Can't DAISY have a non-ZIP extension so Apple systems don't automatically unpack it?  but we do need to manually unpack if writing to a CD-ROM for old devices.  Can't Apple look at some kind of embedded "don't auto-unpack this zip" request?)
     secsSoFar = 0
     durations = [] ; curP = 1
     for recNo in range(1,len(recordingTexts)+1):
         rTxt = recordingTexts[recNo-1]
-        secsThisRecording = mutagen.File(BytesIO(R.audioData[recNo-1])).info.length
+        secsThisRecording = mutagen.File(
+            BytesIO(R.audioData[recNo-1])
+        ).info.length
         if secsThisRecording > 3600: R.warning(f"Recording {recNo} is long enough to cause ~{secsThisRecording*.0001:.1f}sec synchronisation error on some readers") # seems lame v3.100 can result in timestamps being effectively multiplied by ~1.0001 on some players but not all, causing slight de-sync on 1h+ recordings (bladeenc may avoid this but be lower quality overall; better to keep the recordings shorter if possible)
         durations.append(secsThisRecording)
-        if recordingTasks is not None: sys.stderr.write(f"Adding {recNo:04d}.mp3..."),sys.stderr.flush()
-        writestr(f"{recNo:04d}.mp3",R.audioData[recNo-1] if recordingTasks is None else recordingTasks[recNo-1].result())
-        if recordingTasks is not None: sys.stderr.write(" done\n")
-        writestr(f'{recNo:04d}.smil',D(section_smil(R,recNo,secsSoFar,secsThisRecording,curP,rTxt.textsAndTimes if isinstance(rTxt,TextsAndTimesWithPages) else rTxt)))
-        writestr(f'{recNo:04d}.{"xml" if R.daisy3 else "htm"}',D(text_htm(R,(rTxt.textsAndTimes[(1 if isinstance(rTxt.textsAndTimes[0],float) else 0)::2] if isinstance(rTxt,TextsAndTimesWithPages) else [TagAndText('h1',rTxt)]),curP)))
+        if recordingTasks is not None:
+            sys.stderr.write(f"Adding {recNo:04d}.mp3..."),sys.stderr.flush()
+        writestr(f"{recNo:04d}.mp3",
+                 R.audioData[recNo-1]
+                 if recordingTasks is None
+                 else recordingTasks[recNo-1].result())
+        if recordingTasks is not None:
+            sys.stderr.write(" done\n")
+        writestr(f'{recNo:04d}.smil',D(
+            section_smil(R,recNo,secsSoFar,
+                         secsThisRecording,curP,
+                         rTxt.textsAndTimes if isinstance(rTxt,TextsAndTimesWithPages) else rTxt)))
+        writestr(f'{recNo:04d}.{"xml" if R.daisy3 else "htm"}',
+                 D(text_htm(
+                     R,
+                     (rTxt.textsAndTimes[
+                         (1 if isinstance(rTxt.textsAndTimes[0],float) else 0)
+                         ::2]
+                      if isinstance(rTxt,TextsAndTimesWithPages)
+                      else [TagAndText('h1',rTxt)]),
+                     curP)))
         secsSoFar += secsThisRecording
         curP += (1+len(rTxt.textsAndTimes)//2 if isinstance(rTxt,TextsAndTimesWithPages) else 1)
-    for n,u in enumerate(R.imageFiles): writestr(f'{n+1}{u[u.rindex("."):]}',fetch(u,R.cache,R.refresh,R.refetch,R.delay,R.user_agent) if re.match("https?://",u) else open(u,'rb').read())
+    for n,u in enumerate(R.imageFiles):
+        writestr(f'{n+1}{u[u.rindex("."):]}',
+                 fetch(u,R.cache,R.refresh,R.refetch,R.delay,R.user_agent) if re.match("https?://",u) else open(u,'rb').read())
     if not R.date: R.date = "%d-%02d-%02d" % time.localtime()[:3]
     if R.daisy3:
         writestr('dtbook.2005.basic.css',D(d3css))
-        writestr('package.opf',D(package_opf(R,hasFullText,len(recordingTexts),secsSoFar)))
+        writestr('package.opf',D(package_opf(
+            R, hasFullText, len(recordingTexts),
+            secsSoFar)))
         writestr('text.res',D(textres))
     else: writestr('master.smil',D(master_smil(R,headings,secsSoFar)))
-    writestr('navigation.ncx' if R.daisy3 else 'ncc.html',D(ncc_html(R,headings,hasFullText,secsSoFar,[timeAdjust(t.textsAndTimes if isinstance(t,TextsAndTimesWithPages) else t, durations[i]) for i,t in enumerate(recordingTexts)],[(t.pageInfos if isinstance(t,TextsAndTimesWithPages) else []) for t in recordingTexts])))
+    writestr(
+        'navigation.ncx' if R.daisy3
+        else 'ncc.html',
+        D(ncc_html(
+            R,headings,hasFullText,secsSoFar,
+            [timeAdjust(
+                t.textsAndTimes if isinstance(t,TextsAndTimesWithPages) else t,
+                durations[i])
+             for i,t in enumerate(recordingTexts)],
+            [(t.pageInfos if isinstance(t,TextsAndTimesWithPages) else [])
+             for t in recordingTexts])))
     if not R.daisy3: writestr('er_book_info.xml',D(er_book_info(durations))) # not DAISY standard but EasyReader can use this
     z.close()
     sys.stderr.write(f"Wrote {R.outputFile}\n")
 
-def getHeadings(R,recordingTexts):
+def getHeadings(R:Run,recordingTexts) -> list:
     """Gets headings from recordingTexts for the
     DAISY's NCC / OPF data"""
     
     ret = [] ; cvChaps = [] ; chapNo = 0
-    try: bookTitlesAndNumChaps = [(n,int(v)) for n,v in [(b if isinstance(b,tuple) else b.split('/')) for b in R.merge_books if b]]
+    try: bookTitlesAndNumChaps = [
+            (n,int(v))
+            for n,v in [
+                    (b if isinstance(b,tuple)
+                     else b.split('/'))
+                    for b in R.merge_books if b]]
     except: error(f"Unable to parse merge-books={R.merge_books}") # noqa: E722
     for t in recordingTexts:
         chapNo += 1
         if bookTitlesAndNumChaps and chapNo==bookTitlesAndNumChaps[0][1]+1:
             del bookTitlesAndNumChaps[0]
             if not bookTitlesAndNumChaps: error("merge-books did not account for all files (check the counts)")
             chapNo = 1
@@ -565,44 +661,92 @@
             else:
                 R.warning(f"Chapter {chapNo} is completely blank!  (Is {'--marker-attribute' if __name__=='__main__' else 'marker_attribute'} set correctly?)")
                 nums = [] ; first = 0 ; textsAndTimes.append(TagAndText('p',''))
             chapterNumberTextFull = chapterNumberText = nums[0] if len(nums)==1 and not nums[0]=="1" else str(chapNo)
             if R.chapter_titles:
                 if len(R.chapter_titles)>1: chapterNumberTextFull,R.chapter_titles = R.chapter_titles[0],R.chapter_titles[1:]
                 else: chapterNumberTextFull,R.chapter_titles = R.chapter_titles[0], []
-                if chapterNumberText not in chapterNumberTextFull: R.warning(f"Title for chapter {chapNo} is '{chapterNumberTextFull}' which does not contain the expected '{chapterNumberText}'")
+                if chapterNumberText not in chapterNumberTextFull:
+                    R.warning(f"Title for chapter {chapNo} is '{chapterNumberTextFull}' which does not contain the expected '{chapterNumberText}'")
             # In EasyReader 10 on Android, unless there is at least one HEADING (not just div), navigation display is non-functional.  And every heading must point to a 'real' heading in the text, otherwise EasyReader 10 will delete all the text in Daisy 2, or promote something to a heading in Daisy 3 (this is not done by Thorium Reader)
             # (EasyReader 10 on Android also inserts a newline after every span class=sentence if it's a SMIL item, even if there's no navigation pointing to it)
             # So let's add a "real" start-of-chapter heading before the text, with time 0.001 second if we don't know the time from the first time marker (don't set it to 0 or Thorium can have issues)
-            if first==1 and textsAndTimes[0]: first = 0 # for the insert below: put it before the non-zero opening time marker
+            if first==1 and textsAndTimes[0]:
+                first = 0 # for the insert below: put it before the non-zero opening time marker
             else: textsAndTimes.insert(first,(textsAndTimes[first-1] if first else 0)+0.001)
-            textsAndTimes.insert(first,TagAndText(f'h{R.chapter_heading_level}',chapterNumberTextFull)) # we'll ref this
-            chapHeadings=[ChapterTOCInfo(f'h{R.chapter_heading_level}',chapterNumberTextFull,first//2)] # points to our extra heading
-            if textsAndTimes[first+2].text.startswith(chapterNumberText): textsAndTimes[first+2]=TagAndText(textsAndTimes[first+2].tag,textsAndTimes[first+2].text[len(chapterNumberText):].strip()) # because we just had the number as a heading, so we don't also need it repeated as 1st thing in text
+            textsAndTimes.insert(first,TagAndText(
+                f'h{R.chapter_heading_level}',
+                chapterNumberTextFull)) # we'll ref this
+            chapHeadings=[ChapterTOCInfo(
+                f'h{R.chapter_heading_level}',
+                chapterNumberTextFull,
+                first//2)] # points to our extra heading
+            if textsAndTimes[first+2].text.startswith(chapterNumberText):
+                textsAndTimes[first+2]=TagAndText(
+                    textsAndTimes[first+2].tag,
+                    textsAndTimes[first+2].text[len(chapterNumberText):].strip()) # because we just had the number as a heading, so we don't also need it repeated as 1st thing in text
             first += 2 # past the heading we added
             if first+2<len(textsAndTimes) and re.search("[1-9][0-9]*",textsAndTimes[first+2].text):
-              v2 = int(re.findall("[1-9][0-9]*",textsAndTimes[first+2].text)[0]) # might not start at 2, might start at 13 or something, but does it then increase incrementally:
-              if [re.findall("[1-9][0-9]*",textsAndTimes[f].text)[:1] for f in range(first+4,len(textsAndTimes),2) if textsAndTimes[f].text]==[[str(n)] for n in range(v2+1,v2+(len(textsAndTimes)-first)//2-sum(1 for f in range(first+4,len(textsAndTimes),2) if not textsAndTimes[f].text))]: # looks like we're dealing with consecutive chapter and verse numbers with no other headings, so index the verse numbers (this is resilient to blank paragraphs due to an extra timing marker somewhere, but might cause incorrect numbering if that extra timing marker is not at the end)
+              v2 = int(re.findall(
+                  "[1-9][0-9]*",
+                  textsAndTimes[first+2].text)[0]) # might not start at 2, might start at 13 or something, but does it then increase incrementally:
+              if [re.findall(
+                      "[1-9][0-9]*",
+                      textsAndTimes[f].text)[:1]
+                  for f in range(
+                          first+4,
+                          len(textsAndTimes),2)
+                  if textsAndTimes[f].text]==[
+                          [str(n)]
+                          for n in range(
+                                  v2+1,
+                                  v2+(len(textsAndTimes)-first)//2
+                                  -sum(1 for f in range(
+                                      first+4,
+                                      len(textsAndTimes),
+                                      2)
+                                       if not textsAndTimes[f].text))]: # looks like we're dealing with consecutive chapter and verse numbers with no other headings, so index the verse numbers (this is resilient to blank paragraphs due to an extra timing marker somewhere, but might cause incorrect numbering if that extra timing marker is not at the end)
                 v = 1
                 while v < (len(textsAndTimes)-first)//2+2:
                     lastV = v
-                    while lastV < (len(textsAndTimes)-first)//2+1 and (0 if v==1 else textsAndTimes[first+2*v-3])==textsAndTimes[first+2*lastV-1]: lastV += 1 # check for a span of them sharing a time
-                    if any(textsAndTimes[first+2*vv-2].text for vv in range(v,lastV+1)): chapHeadings.append(ChapterTOCInfo('div' if R.daisy3 or R.strict_ncc_divs else f'h{R.chapter_heading_level+1}',f"{chapterNumberText}:{v}{'' if v==lastV else f'-{lastV}'}",first//2+v-1))
+                    while lastV < (len(textsAndTimes)-first)//2+1 and \
+                          (0 if v==1 else textsAndTimes[first+2*v-3])==textsAndTimes[first+2*lastV-1]: lastV += 1 # check for a span of them sharing a time
+                    if any(textsAndTimes
+                           [first+2*vv-2].text
+                           for vv in range(
+                                   v,lastV+1)):
+                        chapHeadings.append(
+                            ChapterTOCInfo(
+                                'div' if R.daisy3 or R.strict_ncc_divs
+                                else f'h{R.chapter_heading_level+1}',
+                                f"{chapterNumberText}:{v}{'' if v==lastV else f'-{lastV}'}",
+                                first//2+v-1))
                     v = lastV + 1
                 cvChaps.append(len(ret)+1)
         if bookTitlesAndNumChaps:
-            chapHeadings=[ChapterTOCInfo(f'h{int(i.hTag[1:])+1}' if i.hTag.startswith('h') else i.hTag,i.hLine,i.itemNo) for i in chapHeadings] # add 1 to each heading level
-            if chapNo==1: chapHeadings.insert(0,ChapterTOCInfo('h1',bookTitlesAndNumChaps[0][0],chapHeadings[0].itemNo)) # the book title (must point to a real heading for similar reason as above, TODO: if there's substantial text before 1st heading, we'll need to insert a heading in the text with 0.001s audio or something instead of doing this; may also need to in-place change recordingTexts adding 1 to all headings: don't do this unless inserting h1)
+            chapHeadings=[
+                ChapterTOCInfo(
+                    f'h{int(i.hTag[1:])+1}' # add 1 to each heading level
+                    if i.hTag.startswith('h')
+                    else i.hTag,
+                    i.hLine,i.itemNo)
+                for i in chapHeadings]
+            if chapNo==1: chapHeadings.insert(
+                    0,
+                    ChapterTOCInfo(
+                        'h1',
+                        bookTitlesAndNumChaps[0][0], # the book title (must point to a real heading for similar reason as above, TODO: if there's substantial text before 1st heading, we'll need to insert a heading in the text with 0.001s audio or something instead of doing this; may also need to in-place change recordingTexts adding 1 to all headings: don't do this unless inserting h1)
+                        chapHeadings[0].itemNo))
         ret.append(chapHeadings)
     if len(bookTitlesAndNumChaps)>1 or bookTitlesAndNumChaps and not chapNo==bookTitlesAndNumChaps[0][1]: R.warning("merge-books specified more files than given")
     if len(cvChaps) not in [0,len(ret)]: R.warning(f"Verse-indexed only {len(cvChaps)} of {len(ret)} chapters.  Missing: {', '.join(str(i) for i in range(1,len(ret)+1) if i not in cvChaps)}")
     if cvChaps and not R.daisy3 and not R.strict_ncc_divs: R.warning("Verse-indexing in Daisy 2 can prevent EasyReader 10 from displaying the text: try Daisy 3 instead") # (and with strict_ncc_divs, verses are not shown in Book navigation in Daisy 2)
     return ret
 
-def merge0lenSpans(recordingTexts,headings):
+def merge0lenSpans(recordingTexts,headings)->None:
     """Finds spans in the text that are marked as
     zero length in the audio, and merges them into
     their neighbours if possible.  This is so that
     the resulting DAISY file can still be
     navigable if some of the time markers are
     somehow missing in the input JSON, i.e. we
     don't know when item 1 becomes item 2, but we
@@ -611,24 +755,28 @@
     a combined item for both 1 and 2."""
     
     for cT,cH in zip(recordingTexts,headings):
         if not isinstance(cT,TextsAndTimesWithPages): continue
         textsAndTimes,pages = cT
         i=0
         while i < len(textsAndTimes)-2:
-            while i < len(textsAndTimes)-2 and isinstance(textsAndTimes[i],TagAndText) and (0 if i==0 else textsAndTimes[i-1])==textsAndTimes[i+1] and textsAndTimes[i].tag==textsAndTimes[i+2].tag: # tag identical and 0-length
+            while i < len(textsAndTimes)-2 and \
+                  isinstance(textsAndTimes[i],TagAndText) and \
+            (0 if i==0 else textsAndTimes[i-1])==\
+            textsAndTimes[i+1] and \
+            textsAndTimes[i].tag==textsAndTimes[i+2].tag: # tag identical and 0-length
                 textsAndTimes[i] = TagAndText(textsAndTimes[i].tag, f"{textsAndTimes[i].text}{' ' if textsAndTimes[i].tag=='span' else '<br>'}{textsAndTimes[i+2].text}") # new combined item
                 del textsAndTimes[i+1:i+3] # old
                 for hI,hV in enumerate(cH):
                     if hV.itemNo > i//2: cH[hI]=ChapterTOCInfo(hV.hTag,hV.hLine,hV.itemNo-1)
                 for pI,pInfo in enumerate(pages):
                     if pInfo.duringId > i//2: pages[pI]=PageInfo(pInfo.duringId-1,pInfo.pageNo)
             i += 1
 
-def recodeMP3(dat):
+def recodeMP3(dat:bytes) -> bytes:
     """Takes MP3 or WAV data, re-codes it
     as suitable for DAISY, and returns the bytes
     of new MP3 data for putting into DAISY ZIP"""
 
     # It seems broken players like FSReader can get timing wrong if mp3 contains
     # too many tags at the start (e.g. images).
     # eyed3 clear() won't help: it zeros out bytes without changing indices.
@@ -638,20 +786,20 @@
     # with AIFF files too, but we say MP3 or WAV.
     # Some LAME versions can't take WAV from stdin
     # only raw when encoding, but ok if --decode)
     m = re.search(b'(?s)([0-9.]+) kHz, ([0-9]+).*?([0-9]+) bit',decodeJob.stderr) # hope nobody disabled --decode when building LAME (is OK on lame.buanzo.org EXEs)
     if not m: error("lame did not give expected format for frequency, channels and bits output")
     return run(["lame","--quiet","-r","-s",m.group(1).decode('latin1')]+(['-a'] if m.group(2)==b'2' else [])+['-m','m','--bitwidth',m.group(3).decode('latin1'),"-","--resample","44.1","-b","64","-q","0","-o","-"],input=decodeJob.stdout,check=True,stdout=PIPE).stdout
 
-def fetch(url,
-          cache = "cache",
-          refresh = False,
-          refetch = False,
-          delay = 0,
-          user_agent = None):
+def fetch(url:str,
+          cache = "cache", # not necessarily str
+          refresh:bool = False,
+          refetch:bool = False,
+          delay:int = 0,
+          user_agent = None) -> bytes:
     """Fetches a URL, with delay and/or cache.
     
     cache: the cache directory (None = don't save)
     or a requests_cache session object to do it
     (delay option is ignored when using session)
 
     refresh: if True, send an If-Modified-Since
@@ -669,26 +817,36 @@
     user_agent: the User-Agent string to use, if
     not using Python's default User-Agent"""
     
     ifModSince = None
     if hasattr(cache,"get"):
         # if we're given a requests_cache session,
         # use that instead of our own caching code
-        r = cache.request('GET',url,headers = {"User-Agent":user_agent} if user_agent else {},refresh=refresh,force_refresh=refetch)
+        r = cache.request('GET',url,
+                          headers = {
+                              "User-Agent":
+                              user_agent}
+                          if user_agent else {},
+                          refresh=refresh,
+                          force_refresh=refetch)
         if r.status_code == 200: return r.content
         else: raise HTTPError("",r.status_code,"unexpected HTTP code",{},None)
 
     # Fallback to our own filesystem-based code
     # for quick command-line use if you want to
     # manually manage the cache (delete parts of
     # it by directory etc) :
     if cache:
-      fn = re.sub('[%&?@*#{}<>!:+`=|$]','',cache+os.sep+unquote(re.sub('.*?://','',url)).replace('/',os.sep)) # these characters need to be removed on Windows's filesystem; TODO: store original URL somewhere just in case some misguided webmaster puts two identical URLs modulo those characters??
+      fn = re.sub('[%&?@*#{}<>!:+`=|$]', # these characters need to be removed on Windows's filesystem
+                  '', # TODO: store original URL somewhere just in case some misguided webmaster puts two identical URLs modulo those characters??
+                  cache+os.sep+unquote(re.sub('.*?://','',url))
+                  .replace('/',os.sep))
       if fn.endswith(os.sep): fn += "index.html"
-      fn = os.sep.join(f.replace('.',os.extsep) for f in fn.split(os.sep)) # just in case we're on RISC OS (not tested)
+      fn = os.sep.join(f.replace('.',os.extsep)
+                       for f in fn.split(os.sep)) # just in case we're on RISC OS (not tested)
       fnExc = fn+os.extsep+"exception"
       if os.path.exists(fn):
         if refetch: pass # ignore already dl'd
         elif refresh:
             ifModSince=os.stat(fn).st_mtime
         else: return open(fn,'rb').read()
       elif os.path.exists(fnExc) and not refetch and not refresh: raise HTTPError("",int(open(fnExc).read()),"HTTP error on last fetch",{},None) # useful especially if a wrapper script is using our fetch() for multiple chapters and stopping on a 404
@@ -707,40 +865,47 @@
     except HTTPError as e:
         _last_urlopen_time = time.time()
         if e.getcode()==304 and cache:
             sys.stderr.write(" no new data\n")
             return open(fn,'rb').read()
         else:
             sys.stderr.write(f"error {e.getcode()}\n")
-            if cache: open(fnExc,"w").write(str(e.getcode()))
+            if cache: open(fnExc,"w").write(
+                    str(e.getcode()))
             raise
     _last_urlopen_time = time.time()
     if cache:
         open(fn,'wb').write(dat)
         sys.stderr.write(" saved\n")
     else: sys.stderr.write(" fetched\n")
     return dat
 
-def ncc_html(R, headings = [],
-             hasFullText = False,
+def ncc_html(R:Run, headings = [],
+             hasFullText:bool = False,
              totalSecs = 0,
              recTimeTxts = [],
-             pageNos=[]):
+             pageNos=[]) -> str:
     """Returns the Navigation Control Centre (NCC)
     recTimeTxts includes 0 and total
     pageNos is [[PageInfo,...],...]"""
     
     numPages = sum(len(L) for L in pageNos)
-    maxPageNo = max((max((int(i.pageNo) for i in PNs),default=0) for PNs in pageNos),default=0)
+    maxPageNo = max((
+        max(
+            (int(i.pageNo) for i in PNs),
+            default=0)
+        for PNs in pageNos),default=0)
     # TODO: we assume all pages are 'normal' pages
     # (not 'front' pages in Roman letters etc)
     headingsR = normaliseDepth(R,hReduce(headings)) # (hType,hText,recNo,textNo)
     return deBlank(f"""<?xml version="1.0" encoding="utf-8"?>
 {'<!DOCTYPE ncx PUBLIC "-//NISO//DTD ncx 2005-1//EN" "http://www.daisy.org/z3986/2005/ncx-2005-1.dtd">' if R.daisy3 else '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">'}
-<{'ncx xmlns="http://www.daisy.org/z3986/2005/ncx/" version="2005-1"' if R.daisy3 else f'html lang="{R.lang}" xmlns="http://www.w3.org/1999/xhtml"'} xml:lang="{R.lang}">
+<{'ncx xmlns="http://www.daisy.org/z3986/2005/ncx/" version="2005-1"'
+    if R.daisy3
+    else f'html lang="{R.lang}" xmlns="http://www.w3.org/1999/xhtml"'} xml:lang="{R.lang}">
   <head>
     {'<meta name="dtb:uid" content=""/>' if R.daisy3 else '<meta content="text/html; charset=utf-8" http-equiv="Content-type" />'}
     {f'<meta name="dtb:totalPageCount" content="{numPages}" />' if R.daisy3 else ''}
     {f'<meta name="dtb:maxPageNumber" content="{maxPageNo}" />' if R.daisy3 else ''}
     {'' if R.daisy3 else f'<title>{R.title}</title>'}
     <meta name="dc:creator" content="{R.creator}" />
     <meta name="dc:date" content="{R.date}" scheme="yyyy-mm-dd" />
@@ -760,16 +925,18 @@
     <meta name="ncc:pageSpecial" content="0" />
     <meta name="ncc:tocItems" content="{len(headingsR)+sum(len(PNs) for PNs in pageNos)}" />
     <meta name="ncc:totalTime" content="{hmsTime(totalSecs)}" />
     <meta name="ncc:multimediaType" content="{"audioFullText" if hasFullText else "audioNcc"}" />
     <meta name="{'dtb' if R.daisy3 else 'ncc'}:depth" content="{max(int(h.hTag[1:]) for h in headingsR if h.hTag.startswith('h'))+(1 if any(h.hTag=='div' for h in headingsR) else 0)}" />
     <meta name="ncc:files" content="{2+len(headings)*(3 if hasFullText else 2)+len(R.imageFiles)}" />
   </head>
-  {f'<docTitle><text>{R.title}</text></docTitle>' if R.daisy3 else ''}
-  {f'<docAuthor><text>{R.creator}</text></docAuthor>' if R.daisy3 else ''}
+  {f'<docTitle><text>{R.title}</text></docTitle>'
+    if R.daisy3 else ''}
+  {f'<docAuthor><text>{R.creator}</text></docAuthor>'
+    if R.daisy3 else ''}
   <{'navMap id="navMap"' if R.daisy3 else 'body'}>"""+''.join((f"""
     <navPoint id="s{s+1}" class="{t.hTag}" playOrder="{s+1}">
       <navLabel><text>{t.hLine}</text>{'' if recTimeTxts[t.recNo][2*t.itemNo]==recTimeTxts[t.recNo][2*t.itemNo+2] else f'''<audio src="{t.recNo+1:04d}.mp3" clipBegin="{hmsTime(recTimeTxts[t.recNo][2*t.itemNo])}" clipEnd="{hmsTime(recTimeTxts[t.recNo][2*t.itemNo+2])}"/>'''}</navLabel>
       <content src="{t.recNo+1:04d}.smil#pr{t.recNo+1}.{t.itemNo}"/>
     {'</navPoint>'*numDaisy3NavpointsToClose(s,headingsR)}""" if R.daisy3 else ''.join(f"""
     <span class="page-normal" id="page{N}"><a href="{r+1:04d}.smil#t{r+1}.{after}">{N}</a></span>""" for r,PNs in enumerate(pageNos) for (PO,(after,N)) in enumerate(PNs) if (r,after)<=t[2:4] and (not s or (r,after)>headingsR[s-1][2:4]))+f"""
     <{t.hTag} class="{'section' if s or R.allow_jumps else 'title'}" id="s{s+1}">
@@ -780,41 +947,80 @@
       <content src="{r+1:04d}.smil#pr{r+1}.{after}"/>
     </pageTarget>""" for r,PNs in enumerate(pageNos) for (PO,(after,N)) in enumerate(PNs))+"""
   </pageList>
 </ncx>""" if R.daisy3 else """
   </body>
 </html>"""))
 
-def addPbeforeTag(tag,num,paras):
+def addPbeforeTag(tag:str, num:int, paras:list) -> bool:
     "Decides whether a <p> should be added before the current tag"
-    return tag=='span' and (num==0 or not paras[num-1].tag=="span" or paras[num-1].text.endswith("<br />"))
-def closePafterTag(tag,text,num,paras):
+    return tag=='span' and (
+        num==0
+        or not paras[num-1].tag=="span"
+        or paras[num-1].text.endswith("<br />"))
+def closePafterTag(tag:str, text:str, num:int, paras:list) -> bool:
     "Decides whether a </p> should be added after closing the current tag"
-    return tag=='span' and (text.endswith("<br />") or num+1==len(paras) or not paras[num+1].tag=='span')
+    return tag=='span' and (
+        text.endswith("<br />")
+        or num+1==len(paras)
+        or not paras[num+1].tag=='span')
 
-def removeImages(text):
+def removeImages(text:str) -> str:
     "Removes our normalised <img> markup from text"
     return re.sub('<img src="[^"]*" [^/]*/>','',text)
-def imageParagraph(R,text):
+def imageParagraph(R:Run,text:str) -> str:
     "Pulls out our normalised <img> markup for use after the paragraph"
     return f"""{'<p><imggroup>' if R.daisy3 and re.search('<img src="',text) else ''}{''.join(re.findall('<img src="[^"]*" [^/]*/>',text))}{'</imggroup></p>' if R.daisy3 and re.search('<img src="',text) else ''}"""
 
-def daisy3OpenLevelTags(R,tag,num,paras):
+def daisy3OpenLevelTags(R:Run, tag:str, num:int, paras:list[TagAndText]) -> str:
     "Gives the <levelN> tags that should be placed before the current point in the DAISY 3 format"
     if not R.daisy3: return ''
     elif not tag.startswith('h'):
         if num: return '' # will have been started
         else: return '<level1>'
-    return ''.join(f'<level{n}>' for n in range(min(int(tag[1:]),next(int(paras[p].tag[1:]) for p in range(num-1,-1,-1) if paras[p].tag.startswith('h'))+1) if any(paras[P].tag.startswith('h') for P in range(num-1,-1,-1)) else 1,int(tag[1:])+1))
-def daisy3CloseLevelTags(R,tag,num,paras):
+    return ''.join(
+        f'<level{n}>'
+        for n in range(
+                min(
+                    int(tag[1:]),
+                    1+next(
+                        int(paras[p].tag[1:])
+                        for p in range(
+                                num-1,-1,-1)
+                        if paras[p].tag
+                        .startswith('h')))
+                if any(
+                        paras[p].tag
+                        .startswith('h')
+                        for p in range(
+                                num-1,-1,-1))
+                else 1,
+                int(tag[1:])+1))
+def daisy3CloseLevelTags(R:Run, tag:str, num:int, paras:list[TagAndText]) -> str:
     "Gives the </levelN> tags that should be placed before the current point in the DAISY 3 format"
-    if not R.daisy3 or not num+1==len(paras) and not paras[num+1].tag.startswith('h'): return ''
-    return ''.join(f'</level{n}>' for n in range(next(int(paras[p].tag[1:]) for p in range(num,-1,-1) if paras[p].tag.startswith('h')) if any(paras[P].tag.startswith('h') for P in range(num,-1,-1)) else 1,0 if num+1==len(paras) else int(paras[num+1].tag[1:])-1,-1))
+    if not R.daisy3 or not num+1==len(paras) \
+       and not paras[num+1].tag.startswith('h'):
+        return ''
+    return ''.join(
+        f'</level{n}>'
+        for n in range(
+                next(
+                    int(paras[p].tag[1:])
+                    for p in range(num,-1,-1)
+                    if paras[p].tag
+                    .startswith('h')
+                ) if any(
+                    paras[p].tag.startswith('h')
+                    for p in range(num,-1,-1)
+                ) else 1,
+                0 if num+1==len(paras)
+                else int(paras[num+1].tag[1:])-1,
+                -1))
 
-def numDaisy3NavpointsToClose(s,headingsR):
+def numDaisy3NavpointsToClose(s:int, headingsR:list[BookTOCInfo]) -> int:
     """Calculates the number of DAISY 3 navigation
     points that need closing after index s"""
     
     thisTag = headingsR[s]
     if thisTag.hTag.startswith('h'):
         thisDepth = int(thisTag.hTag[1])
     else: thisDepth = None # a div navpoint
@@ -822,44 +1028,60 @@
     else:
         nextTag = headingsR[s+1]
         if nextTag.hTag.startswith('h'):
             nextDepth = int(nextTag.hTag[1])
         else: nextDepth = None # another div
     if thisDepth == nextDepth: return 1 # e.g. this is div and next is div, or same heading level
     elif nextDepth is None: return 0 # never close if it's heading followed by div
-    headingNums_closed = ''.join(('' if not i.hTag.startswith('h') else i.hTag[1] if int(i.hTag[1])>=nextDepth else '0') for i in reversed(headingsR[:s+1])).split('0',1)[0]
+    headingNums_closed = ''.join(
+        ('' if not i.hTag.startswith('h')
+         else i.hTag[1]
+         if int(i.hTag[1])>=nextDepth
+         else '0')
+        for i in reversed(headingsR[:s+1])
+    ).split('0',1)[0]
     if thisDepth: D=thisDepth
     else: D=int(headingNums_closed[0]) # the heading before this div (TODO: this code assumes there will be one, which is currently true as these divs are generated only by verse numbering)
-    N = sum(1 for j in range(nextDepth,D+1) if str(j) in headingNums_closed)
+    N = sum(1 for j in range(nextDepth,D+1)
+            if str(j) in headingNums_closed)
     return N+(1 if thisDepth is None else 0)
 
-def hReduce(headings):
+def hReduce(headings:list) -> list[BookTOCInfo]:
     """convert a list of ChapterTOCInfo lists (or
     text strings for unstructured chapters) into a
     single BookTOCInfo list"""
-    return reduce(lambda a,b:a+b,[([BookTOCInfo(hType,hText,recNo,textNo) for (hType,hText,textNo) in i] if isinstance(i,list) else [BookTOCInfo('h1',i,recNo,0)]) for recNo,i in enumerate(headings)],[])
+    return reduce(lambda a,b:a+b,[
+        ([BookTOCInfo(hType,hText,recNo,textNo)
+          for (hType,hText,textNo) in i]
+         if isinstance(i,list) else
+         [BookTOCInfo('h1',i,recNo,0)])
+        for recNo,i in enumerate(headings)],[])
 
-def normaliseDepth(R,items):
+def normaliseDepth(R:Run, items:list) -> list:
     """Ensure that heading items' depth conforms
     to DAISY standard, in a BookTOCInfo list"""
     
     if R.allow_jumps: return items
     curDepth = 0
     for i in range(len(items)):
       ii = items[i] # TagAndText or BookTOCInfo
       if ii[0].lower().startswith('h'):
         depth = int(ii[0][1:])
         if depth > curDepth+1:
-            if isinstance(ii,BookTOCInfo): items[i]=BookTOCInfo(f'h{curDepth+1}',ii.hLine,ii.recNo,ii.itemNo)
-            else: items[i]=TagAndText(f'h{curDepth+1}',ii.text)
+            if isinstance(ii,BookTOCInfo):
+                items[i]=BookTOCInfo(
+                    f'h{curDepth+1}',ii.hLine,
+                    ii.recNo,ii.itemNo)
+            else: items[i]=TagAndText(
+                    f'h{curDepth+1}',ii.text)
             curDepth += 1
         else: curDepth = depth
     return items
 
-def master_smil(R,headings = [],
+def master_smil(R:Run,headings = [],
                 totalSecs = 0):
     "Compile the master smil for a DAISY file"
     headings = hReduce(headings)
     return f"""<?xml version="1.0"?>
 <!DOCTYPE smil PUBLIC "-//W3C//DTD SMIL 1.0//EN" "http://www.w3.org/TR/REC-smil/SMIL10.dtd">
 <smil>
   <head>
@@ -868,88 +1090,136 @@
     <meta name="ncc:generator" content="{generator}" />
     <meta name="ncc:timeInThisSmil" content="{hmsTime(totalSecs)}" />
     <layout>
       <region id="textView" />
     </layout>
   </head>
   <body>"""+''.join(f"""
-    <ref title="{deHTML(t.hLine)}" src="{t.recNo+1:04d}.smil#t{t.recNo+1}.{t.itemNo}" id="ms_{s+1:04d}" />""" for s,t in enumerate(headings))+"""
+    <ref title="{deHTML(t.hLine)}" src="{
+  t.recNo+1:04d}.smil#t{t.recNo+1}.{t.itemNo
+  }" id="ms_{s+1:04d}" />"""
+                    for s,t in
+                    enumerate(headings))+"""
   </body>
 </smil>
 """
 
-def timeAdjust(textsAndTimes,secsThisRecording):
+def timeAdjust(textsAndTimes,secsThisRecording:float) -> None:
     """Ensure textsAndTimes starts at the
     beginning of the recording, and ends at the
     end.  Necessary for some players to play all
     of the audio."""
-    if not isinstance(textsAndTimes,list): textsAndTimes=[textsAndTimes]
-    return [0.0]+textsAndTimes[(1 if isinstance(textsAndTimes[0],float) else 0):(-1 if isinstance(textsAndTimes[-1],float) else len(textsAndTimes))]+[secsThisRecording]
-
-def section_smil(R, recNo=1,
-                 totalSecsSoFar=0,
-                 secsThisRecording=0,
-                 startP=0,
-                 textsAndTimes=[]):
+    if not isinstance(textsAndTimes,list):
+        textsAndTimes=[textsAndTimes]
+    return [0.0]+textsAndTimes[
+        (1 if isinstance(textsAndTimes[0],float)
+         else 0) :
+        (-1 if isinstance(textsAndTimes[-1],float)
+         else len(textsAndTimes))
+    ] + [secsThisRecording]
+
+def section_smil(R:Run, recNo:int = 1,
+                 totalSecsSoFar:float = 0,
+                 secsThisRecording:float = 0,
+                 startP:int = 0,
+                 textsAndTimes = []) -> str:
     "Compile a section SMIL for a DAISY file"
-    textsAndTimes = timeAdjust(textsAndTimes,secsThisRecording)
+    textsAndTimes = timeAdjust(textsAndTimes,
+                               secsThisRecording)
     return deBlank(f"""<?xml version="1.0" encoding="utf-8"?>
-{'<!DOCTYPE smil PUBLIC "-//NISO//DTD dtbsmil 2005-2//EN" "http://www.daisy.org/z3986/2005/dtbsmil-2005-2.dtd">' if R.daisy3 else '<!DOCTYPE smil PUBLIC "-//W3C//DTD SMIL 1.0//EN" "http://www.w3.org/TR/REC-smil/SMIL10.dtd">'}
-{'<smil xmlns="http://www.w3.org/2001/SMIL20/">' if R.daisy3 else '<smil>'}
+{'<!DOCTYPE smil PUBLIC "-//NISO//DTD dtbsmil 2005-2//EN" "http://www.daisy.org/z3986/2005/dtbsmil-2005-2.dtd">'
+    if R.daisy3
+    else '<!DOCTYPE smil PUBLIC "-//W3C//DTD SMIL 1.0//EN" "http://www.w3.org/TR/REC-smil/SMIL10.dtd">'}
+{'<smil xmlns="http://www.w3.org/2001/SMIL20/">'
+    if R.daisy3
+    else '<smil>'}
   <head>
-    {'<meta name="dtb:uid" content=""/>' if R.daisy3 else '<meta name="dc:format" content="Daisy 2.02" />'}
-    <meta name="{'dtb' if R.daisy3 else 'ncc'}:generator" content="{generator}" />
-    <meta name="{'dtb' if R.daisy3 else 'ncc'}:totalElapsedTime" content="{hmsTime(totalSecsSoFar)}" />""" + ("" if R.daisy3 else f"""
-    <meta name="ncc:timeInThisSmil" content="{hmsTime(secsThisRecording)}" />
-    <meta name="title" content="{deHTML(textsAndTimes[1][1])}" />
-    <meta name="dc:title" content="{deHTML(textsAndTimes[1][1])}" />
+    {'<meta name="dtb:uid" content=""/>'
+    if R.daisy3
+    else '<meta name="dc:format" content="Daisy 2.02" />'}
+    <meta name="{'dtb' if R.daisy3
+    else 'ncc'}:generator" content="{generator}" />
+    <meta name="{'dtb' if R.daisy3
+    else 'ncc'}:totalElapsedTime" content="{
+    hmsTime(totalSecsSoFar)}" />""" + (
+        "" if R.daisy3 else f"""
+    <meta name="ncc:timeInThisSmil" content="{
+        hmsTime(secsThisRecording)}" />
+    <meta name="title" content="{
+        deHTML(textsAndTimes[1][1])}" />
+    <meta name="dc:title" content="{
+        deHTML(textsAndTimes[1][1])}" />
     <layout>
       <region id="textView" />
     </layout>""")+f"""
   </head>
   <body>
-    <seq id="sq{recNo}" dur="{hmsTime(secsThisRecording) if R.daisy3 else f'{secsThisRecording:.3f}s'}" fill="remove">"""+"".join(f"""
-      <par {'' if R.daisy3 else 'endsync="last" '}id="pr{recNo}.{i//2}">
-        <text id="t{recNo}.{i//2}" src="{recNo:04d}.{'xml' if R.daisy3 else 'htm'}#p{startP+i//2}" />
-        {'' if R.daisy3 or textsAndTimes[i-1]==textsAndTimes[i+1] else f'<seq id="sq{recNo}.{i//2}a">'}
-          {'' if textsAndTimes[i-1]==textsAndTimes[i+1] else f'''<audio src="{recNo:04d}.mp3" clip{'B' if R.daisy3 else '-b'}egin="{hmsTime(textsAndTimes[i-1]) if R.daisy3 else f'npt={textsAndTimes[i-1]:.3f}s'}" clip{'E' if R.daisy3 else '-e'}nd="{hmsTime(textsAndTimes[i+1]) if R.daisy3 else f'npt={textsAndTimes[i+1]:.3f}s'}" id="aud{recNo}.{i//2}" />'''}
-        {'' if R.daisy3 or textsAndTimes[i-1]==textsAndTimes[i+1] else '</seq>'}
-      </par>{''.join(f'<par><text id="t{recNo}.{i//2}.{j}" src="{recNo:04d}.xml#{re.sub(".*"+chr(34)+" id=.","",imageID)}"/></par>' for j,imageID in enumerate(re.findall('<img src="[^"]*" id="[^"]*',textsAndTimes[i][1]))) if R.daisy3 else ''}""" for i in range(1,len(textsAndTimes),2))+"""
+    <seq id="sq{recNo}" dur="{
+    hmsTime(secsThisRecording) if R.daisy3
+    else f'{secsThisRecording:.3f}s'}" fill="remove">"""+"".join(f"""
+      <par {'' if R.daisy3
+    else 'endsync="last" '}id="pr{recNo}.{i//2}">
+        <text id="t{recNo}.{i//2}" src="{
+    recNo:04d}.{'xml' if R.daisy3 else 'htm'
+    }#p{startP+i//2}" />
+        {'' if R.daisy3
+    or textsAndTimes[i-1]==textsAndTimes[i+1]
+    else f'<seq id="sq{recNo}.{i//2}a">'}
+          {'' if
+    textsAndTimes[i-1]==textsAndTimes[i+1]
+    else f'''<audio src="{recNo:04d}.mp3" clip{
+    'B' if R.daisy3 else '-b'}egin="{
+    hmsTime(textsAndTimes[i-1]) if R.daisy3 else
+    f'npt={textsAndTimes[i-1]:.3f}s'}" clip{
+    'E' if R.daisy3 else '-e'}nd="{
+    hmsTime(textsAndTimes[i+1]) if R.daisy3 else
+    f'npt={textsAndTimes[i+1]:.3f}s'}" id="aud{
+    recNo}.{i//2}" />'''}
+        {'' if R.daisy3 or
+    textsAndTimes[i-1]==textsAndTimes[i+1]
+    else '</seq>'}
+      </par>{''.join(f'<par><text id="t{recNo}.{i//2}.{j}" src="{recNo:04d}.xml#{re.sub(".*"+chr(34)+" id=.","",imageID)}"/></par>'
+    for j,imageID in enumerate(re.findall(
+    '<img src="[^"]*" id="[^"]*',
+    textsAndTimes[i][1]))) if R.daisy3 else ''
+    }""" for i in range(1,len(textsAndTimes),2))+"""
     </seq>
   </body>
 </smil>
 """)
 # (do not omit text with 0-length audio altogether, even in Daisy 2: unlike image tags after paragraphs, it might end up not being displayed by EasyReader etc.  Omitting audio does NOT save being stopped at the beginning of the chapter when rewinding by paragraph: is this a bug or a feature?)
 
-def deBlank(s):
+def deBlank(s:str) -> str:
     """Remove blank lines from s
     (does not currently remove the first line if
     blank).  Used so that optional items can be
     placed on their own lines in our format-string
     templates for DAISY markup.
     """
     return re.sub("\n( *\n)+","\n",s)
 
-def hmsTime(secs):
+def hmsTime(secs:float) -> str:
     """Formats a floating-point number of seconds
     into the DAISY standard hours:minutes:seconds
     with fractions to 3 decimal places.  (Some
     old DAISY readers can crash if more than 3
     decimals are used, so we must stick to 3)"""
     
     return f"{int(secs/3600)}:{int(secs/60)%60:02d}:{secs%60:06.3f}"
 
-def deHTML(t):
+def deHTML(t:str) -> str:
     """Remove HTML tags from t, collapse
     whitespace and escape quotes so it can be
     included in an XML attribute"""
     
     return re.sub(r'\s+',' ',re.sub('<[^>]*>','',t)).replace('"','&quot;').strip()
 
-def package_opf(R,hasFullText,numRecs,totalSecs):
+def package_opf(R:Run, hasFullText:bool,
+                numRecs:int,
+                totalSecs:float) -> str:
     "Make the package OPF for a DAISY 3 file"
     return f"""<?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE package
   PUBLIC "+//ISBN 0-9673008-1-9//DTD OEB 1.2 Package//EN" "http://openebook.org/dtds/oeb-1.2/oebpkg12.dtd">
 <package xmlns="http://openebook.org/namespaces/oeb-package/1.0/" unique-identifier="{R.url}">
    <metadata>
       <dc-metadata xmlns:dc="http://purl.org/dc/elements/1.1/">
@@ -968,55 +1238,78 @@
          <meta name="dtb:multimediaContent" content="audio,text{',image' if R.imageFiles else ''}"/>
          <meta name="dtb:narrator" content="{deHTML(R.reader)}"/>
          <meta name="dtb:producedDate" content="{R.date}"/>
       </x-metadata>
    </metadata>
    <manifest>
       <item href="package.opf" id="opf" media-type="text/xml"/>"""+''.join(f"""
-      <item href="{i:04d}.mp3" id="opf-{i}" media-type="audio/mpeg"/>""" for i in range(1,numRecs+1))+''.join(f"""
-      <item href="{i+1}{u[u.rindex("."):]}" id="opf-{i+numRecs+1}" media-type="image/{u[u.rindex(".")+1:].lower().replace("jpg","jpeg")}"/>""" for i,u in enumerate(R.imageFiles))+f"""
-      <item href="dtbook.2005.basic.css" id="opf-{len(R.imageFiles)+numRecs+1}" media-type="text/css"/>"""+''.join(f"""
-      <item href="{i:04d}.xml" id="opf-{i+len(R.imageFiles)+numRecs+1}" media-type="application/x-dtbook+xml"/>""" for i in range(1,numRecs+1))+''.join(f"""
-      <item href="{i:04d}.smil" id="{i:04d}" media-type="application/smil+xml"/>""" for i in range(1,numRecs+1))+"""
+      <item href="{i:04d}.mp3" id="opf-{i
+      }" media-type="audio/mpeg"/>""" for i in range(1,numRecs+1))+''.join(f"""
+      <item href="{i+1}{u[u.rindex("."):]
+      }" id="opf-{i+numRecs+1
+      }" media-type="image/{u[u.rindex(".")+1:]
+      .lower().replace("jpg","jpeg")}"/>""" for i,u in enumerate(R.imageFiles))+f"""
+      <item href="dtbook.2005.basic.css" id="opf-{
+      len(R.imageFiles)+numRecs+1}" media-type="text/css"/>"""+''.join(f"""
+      <item href="{i:04d}.xml" id="opf-{i+len(
+      R.imageFiles)+numRecs+1}" media-type="application/x-dtbook+xml"/>""" for i in range(1,numRecs+1))+''.join(f"""
+      <item href="{i:04d}.smil" id="{i
+      :04d}" media-type="application/smil+xml"/>""" for i in range(1,numRecs+1))+"""
       <item href="navigation.ncx" id="ncx" media-type="application/x-dtbncx+xml"/>
       <item href="text.res" id="resource" media-type="application/x-dtbresource+xml"/>
    </manifest>
    <spine>"""+"".join(f"""
       <itemref idref="{i:04d}"/>""" for i in range(1,numRecs+1))+"""
    </spine>
 </package>
 """
 
-def text_htm(R,paras,offset=0):
+def text_htm(R:Run, paras:list[TagAndText], offset:int=0) -> str:
     """Format the text, as htm for DAISY 2 or xml
     for DAISY 3.
     paras = TagAndText list, text is xhtml i.e. & use &amp; etc."""
     
-    return deBlank(f"""<?xml version="1.0"{' encoding="utf-8"' if R.daisy3 else ''}?>{'<?xml-stylesheet type="text/css" href="dtbook.2005.basic.css"?>' if R.daisy3 else ''}
-{'<!DOCTYPE dtbook PUBLIC "-//NISO//DTD dtbook 2005-3//EN" "http://www.daisy.org/z3986/2005/dtbook-2005-3.dtd">' if R.daisy3 else '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">'}
-<{'dtbook xmlns="http://www.daisy.org/z3986/2005/dtbook/" version="2005-2"' if R.daisy3 else f'html lang="{R.lang}" xmlns="http://www.w3.org/1999/xhtml"'} xml:lang="{R.lang}">
+    return deBlank(f"""<?xml version="1.0"{
+    ' encoding="utf-8"' if R.daisy3 else ''
+    }?>{'<?xml-stylesheet type="text/css" href="dtbook.2005.basic.css"?>' if R.daisy3 else ''}
+{'<!DOCTYPE dtbook PUBLIC "-//NISO//DTD dtbook 2005-3//EN" "http://www.daisy.org/z3986/2005/dtbook-2005-3.dtd">'
+    if R.daisy3
+    else '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">'}
+<{'dtbook xmlns="http://www.daisy.org/z3986/2005/dtbook/" version="2005-2"'
+    if R.daisy3
+    else f'html lang="{R.lang}" xmlns="http://www.w3.org/1999/xhtml"'} xml:lang="{R.lang}">
     <head>
         {'<meta name="dt:version" content="1.0" />' if R.daisy3 else ''}
-        {f'<meta name="dc:Title" content="{deHTML(R.title)}"/>' if R.daisy3 else f'<title>{R.title}</title>'}
+        {f'<meta name="dc:Title" content="{deHTML(R.title)}"/>'
+    if R.daisy3 else f'<title>{R.title}</title>'}
         {f'<meta name="dc:Creator" content="{deHTML(R.creator)}"/>' if R.daisy3 else ''}
         {f'<meta name="dc:Publisher" content="{deHTML(R.publisher)}"/>' if R.daisy3 else ''}
         {f'<meta name="dc:Date" content="{R.date}"/>' if R.daisy3 else ''}
         {f'<meta name="dc:Language" content="{R.lang}" />' if R.daisy3 else ''}
         {f'<meta name="dc:identifier" content="{R.url}" />' if R.daisy3 else ''}
         {f'<meta name="dtb:uid" content="{R.url}"/>' if R.daisy3 else '<meta content="text/html; charset=utf-8" http-equiv="content-type"/>'}
         <meta name="generator" content="{generator}"/>
     </head>
     <{'book' if R.daisy3 else 'body'}>
         {f'<frontmatter><doctitle>{R.title}</doctitle><docauthor>{R.creator}</docauthor></frontmatter><bodymatter>' if R.daisy3 else ''}
-"""+"\n".join(f"""{daisy3OpenLevelTags(R,tag,num,paras)}{'<p>' if addPbeforeTag(tag,num,paras) else ''}<{tag} id=\"p{num+offset}\"{(' class="word"' if len(text.split())==1 else ' class="sentence"') if tag=='span' else ''}>{re.sub(" *<br />$","",removeImages(text))}</{tag}>{'</p>' if closePafterTag(tag,text,num,paras) else ''}{imageParagraph(R,text)}{daisy3CloseLevelTags(R,tag,num,paras)}""" for num,(tag,text) in enumerate(normaliseDepth(R,paras)))+f"""
+"""+"\n".join(f"""{
+daisy3OpenLevelTags(R,tag,num,paras)}{
+'<p>' if addPbeforeTag(tag,num,paras) else ''
+}<{tag} id=\"p{num+offset}\"{
+(' class="word"' if len(text.split())==1 else
+' class="sentence"') if tag=='span' else ''}>{
+re.sub(" *<br />$","",removeImages(text))}</{tag
+}>{'</p>' if closePafterTag(tag,text,num,paras)
+else ''}{imageParagraph(R,text)}{
+daisy3CloseLevelTags(R,tag,num,paras)}""" for num,(tag,text) in enumerate(normaliseDepth(R,paras)))+f"""
     </{'bodymatter></book' if R.daisy3 else 'body'}>
 </{'dtbook' if R.daisy3 else 'html'}>
 """)
 
-def er_book_info(durations):
+def er_book_info(durations:list[float]) -> str:
     """Return the EasyReader book info.
     durations = list of secsThisRecording"""
     
     return """<?xml version="1.0" encoding="utf-8"?>
 <book_info>
     <smil_info>"""+"".join(f"""
         <smil nr="{s}" Name="{s+1:04d}.smil" dur="{d:f}"/>""" for s,d in enumerate(durations))+"""
```

### Comparing `anemone_daisy_maker-1.55.9/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: anemone_daisy_maker
-Version: 1.55.9
+Name: anemone-daisy-maker
+Version: 1.56
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
+Home-page: UNKNOWN
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: mutagen
-
+License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
 `anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
@@ -62,7 +64,8 @@
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
 * Windows is a registered trademark of Microsoft Corp.
 
 * Any other trademarks I mentioned without realising are trademarks of their respective holders.
+
```

### Comparing `anemone_daisy_maker-1.55.9/setup.py` & `anemone_daisy_maker-1.56/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-from setuptools import setup, find_packages
-setup(
-    name='anemone_daisy_maker',
-    version='1.55.9',
-    entry_points={"console_scripts":["anemone=anemone.__init__:anemone"]},
-    author='Silas S. Brown',
-    author_email='ssb22@cam.ac.uk',
-    description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',
-    long_description="""
-Anemone DAISY maker
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.56',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
 `anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
@@ -56,19 +47,8 @@
 
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
 * Windows is a registered trademark of Microsoft Corp.
 
-* Any other trademarks I mentioned without realising are trademarks of their respective holders.
-""",
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.7',
-    install_requires=["mutagen"],
-)
+* Any other trademarks I mentioned without realising are trademarks of their respective holders.''',long_description_content_type='text/markdown',packages=find_packages(),classifiers=['Programming Language :: Python :: 3','License :: OSI Approved :: Apache Software License','Operating System :: OS Independent'],python_requires='>=3.7',install_requires=['mutagen'])
```

