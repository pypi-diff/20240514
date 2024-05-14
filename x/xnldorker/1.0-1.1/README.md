# Comparing `tmp/xnldorker-1.0.tar.gz` & `tmp/xnldorker-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnldorker-1.0.tar", last modified: Tue Apr 30 20:51:35 2024, max compression
+gzip compressed data, was "xnldorker-1.1.tar", last modified: Tue May 14 15:11:08 2024, max compression
```

## Comparing `xnldorker-1.0.tar` & `xnldorker-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.955378 xnldorker-1.0/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11035 2024-04-30 20:51:35.941330 xnldorker-1.0/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    10801 2024-04-30 20:50:30.000000 xnldorker-1.0/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-30 20:51:35.957911 xnldorker-1.0/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      671 2024-04-30 20:50:36.000000 xnldorker-1.0/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.640299 xnldorker-1.0/xnldorker/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       18 2024-04-30 20:50:34.000000 xnldorker-1.0/xnldorker/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47493 2024-04-30 20:49:44.000000 xnldorker-1.0/xnldorker/xnldorker.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-30 20:51:35.920228 xnldorker-1.0/xnldorker.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11035 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      295 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       55 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 20:02:25.000000 xnldorker-1.0/xnldorker.egg-info/not-zip-safe
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       64 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       10 2024-04-30 20:51:35.000000 xnldorker-1.0/xnldorker.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 15:11:08.890246 xnldorker-1.1/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11433 2024-05-14 15:11:08.877214 xnldorker-1.1/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11200 2024-05-14 15:06:33.000000 xnldorker-1.1/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-14 15:11:08.892252 xnldorker-1.1/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      671 2024-05-01 11:05:37.000000 xnldorker-1.1/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 15:11:08.547782 xnldorker-1.1/xnldorker/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       18 2024-05-14 14:49:43.000000 xnldorker-1.1/xnldorker/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    56629 2024-05-14 14:57:29.000000 xnldorker-1.1/xnldorker/xnldorker.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 15:11:08.850999 xnldorker-1.1/xnldorker.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    11433 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      295 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       55 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-06 12:38:52.000000 xnldorker-1.1/xnldorker.egg-info/not-zip-safe
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       64 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       10 2024-05-14 15:11:08.000000 xnldorker-1.1/xnldorker.egg-info/top_level.txt
```

### Comparing `xnldorker-1.0/PKG-INFO` & `xnldorker-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: xnldorker
-Version: 1.0
+Version: 1.1
 Summary: Run a dork on different search sites
 Home-page: https://github.com/xnl-h4ck3r/xnldorker
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 Requires-Dist: termcolor
 Requires-Dist: requests
 Requires-Dist: asyncio
 Requires-Dist: beautifulsoup4
 Requires-Dist: playwright
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
 
-## About - v1.0
+## About - v1.1
 
 This is a tool used to run a dork on different search sites.
-The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
+The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google, Yandex**
 
-**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` (and/or `--exclude-source`) argument to specify the appropriate sources.**
 
 **WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
 
 ## Installation
 
 `xnldorker` supports **Python 3**.
 
@@ -63,15 +63,15 @@
 | -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
 | -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
 | -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
 | -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
 | -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
 | -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
 | -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
-| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
+| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 90). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
 |          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
 | -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
 |          | --version            | Show current version number.                                                                                                                                                                                                                      |
 | -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
 | -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
 
 ## Examples
@@ -101,22 +101,23 @@
 The output can also be piped to another command.
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
 
 ## Recommendations
 
 - Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
-- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you do not need to run silently in the background, **I would recommend using the `-sb`/`--show-browser` argument** because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you show the browsers and you get an anti-bot page shown, the process will be paused and wait for the number of seconds specified by `-abt`/`--antobit_timeout` (default 90 seconds). However, it you manually respond to the check and want it to resume quicker, you can enter the name of the source (in lowercase) and press ENTER to resume again.
 - The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
 - You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
 - Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
 - If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
 
 ```sh
-xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+xnldorker -i "example.com" -v -t 120 -sb -rwos -o example.com_xnldorker.txt
 ```
 
 - After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
 
 ## Issues
 
 If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
```

### Comparing `xnldorker-1.0/README.md` & `xnldorker-1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
 
-## About - v1.0
+## About - v1.1
 
 This is a tool used to run a dork on different search sites.
-The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
+The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google, Yandex**
 
-**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` (and/or `--exclude-source`) argument to specify the appropriate sources.**
 
 **WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
 
 ## Installation
 
 `xnldorker` supports **Python 3**.
 
@@ -49,15 +49,15 @@
 | -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
 | -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
 | -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
 | -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
 | -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
 | -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
 | -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
-| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
+| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 90). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
 |          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
 | -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
 |          | --version            | Show current version number.                                                                                                                                                                                                                      |
 | -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
 | -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
 
 ## Examples
@@ -87,22 +87,23 @@
 The output can also be piped to another command.
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
 
 ## Recommendations
 
 - Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
-- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you do not need to run silently in the background, **I would recommend using the `-sb`/`--show-browser` argument** because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you show the browsers and you get an anti-bot page shown, the process will be paused and wait for the number of seconds specified by `-abt`/`--antobit_timeout` (default 90 seconds). However, it you manually respond to the check and want it to resume quicker, you can enter the name of the source (in lowercase) and press ENTER to resume again.
 - The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
 - You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
 - Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
 - If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
 
 ```sh
-xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+xnldorker -i "example.com" -v -t 120 -sb -rwos -o example.com_xnldorker.txt
 ```
 
 - After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
 
 ## Issues
 
 If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
```

### Comparing `xnldorker-1.0/setup.py` & `xnldorker-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `xnldorker-1.0/xnldorker/xnldorker.py` & `xnldorker-1.1/xnldorker/xnldorker.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 import tldextract
 try:
     from . import __version__
 except:
     pass
 
 # Available sources to search
-SOURCES = ['duckduckgo','bing','startpage','yahoo', 'google']
+SOURCES = ['duckduckgo','bing','startpage','yahoo', 'google', 'yandex']
 
 DEFAULT_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36'
 
 # Global variables
 args = None
 browser = None
 stopProgram = False
 stopProgramCount = 0
 inputDork = ''
 duckduckgoEndpoints = set()
 bingEndpoints = set()
 yahooEndpoints = set()
 googleEndpoints = set()
 startpageEndpoints = set()
+yandexEndpoints = set()
 allSubs = set()
 sourcesToProcess = []
 
 # Functions used when printing messages dependant on verbose options
 def verbose():
     return args.verbose or args.vverbose
 def vverbose():
@@ -64,15 +65,15 @@
 
 def showVersion():
     try:
         try:
             resp = requests.get('https://raw.githubusercontent.com/xnl-h4ck3r/xnldorker/main/xnldorker/__init__.py',timeout=3)
         except:
             write('Current xnldorker version '+__version__+' (unable to check if latest)\n')
-        if __version__ == resp.text.split('=')[1].replace('"',''):
+        if __version__ == resp.text.split('=')[1].replace('"','').strip():
             write('Current xnldorker version '+__version__+' ('+colored('latest','green')+')\n')
         else:
             write('Current xnldorker version '+__version__+' ('+colored('outdated','red')+')\n')
     except:
         pass
       
 def showBanner():
@@ -110,15 +111,36 @@
 def getSubdomain(url):
     try:
         # Just get the hostname of the url 
         tldExtract = tldextract.extract(url)
         return tldExtract.subdomain
     except Exception as e:
         writerr(colored('ERROR getSubdomain 1: ' + str(e), 'red')) 
-        
+
+async def wait_for_word_or_sleep(word, timeout):
+    """
+    Called when an antibot screen is detected on a source. It will resume again when the timeout is reached, or if the passed word is typed and ENTER pressed
+    """
+    loop = asyncio.get_event_loop()
+    word_entered = asyncio.Event()
+
+    def on_input_received():
+        input_text = sys.stdin.readline().strip()
+        if input_text == word:
+            word_entered.set()
+
+    loop.add_reader(sys.stdin.fileno(), on_input_received)
+
+    try:
+        await asyncio.wait_for(word_entered.wait(), timeout=timeout)
+    except asyncio.TimeoutError:
+        pass  # Timeout reached, continue with the script
+    finally:
+        loop.remove_reader(sys.stdin.fileno())
+              
 async def getResultsDuckDuckGo(page, endpoints):
     global allSubs
     try:
         content = await page.content()
         soup = BeautifulSoup(content, 'html.parser')
         div_content = soup.find('div', id='web_content_wrapper')
         if div_content:
@@ -150,20 +172,32 @@
         await page.goto(f'https://duckduckgo.com/?kc=-1&ia=web&q={dork}', timeout=args.timeout*1000)
         pageNo = 1
         
         # If captcha is shown then allow time to submit it
         captcha = await page.query_selector('#anomaly-modal__modal.anomaly-modal__modal')
         if captcha:
             if args.show_browser:
-                writerr(colored(f'[ Google ] reCAPTCHA needs responding to. Process will resume in {arg.antibot_timeout} seconds...','yellow')) 
-                await asyncio.sleep(args.antibot_timeout)
+                writerr(colored(f'[ DuckDuckGo ] reCAPTCHA needs responding to. Process will resume in {arg.antibot_timeout} seconds, or when you type "duckduckgo" and press ENTER...','yellow')) 
+                await wait_for_word_or_sleep("duckduckgo", args.antibot_timeout)
+                writerr(colored(f'[ DuckDuckGo ] Resuming...', 'green'))
             else:
-                writerr(colored('[ Google ] reCAPTCHA needed responding to. Consider using option -vb / --view-browser','red'))
+                writerr(colored('[ DuckDuckGo ] reCAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
                 return set(endpoints)
-            
+        
+        try:
+            # Wait for the search results to be fully loaded and have links
+            await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+        except:
+            pass
+
+        captcha = await page.query_selector('#anomaly-modal__modal.anomaly-modal__modal')
+        if captcha:
+            writerr(colored('[ DuckDuckGo ] Failed to complete reCAPTCHA','red'))
+            return set(endpoints)
+               
         # Function to check if the button is disabled and enable it if necessary
         async def enable_more_results():
             more_results_button = await page.query_selector('#more-results')
             if more_results_button:
                 is_disabled = await more_results_button.evaluate('(element) => element.disabled')
                 if is_disabled:
                     await page.evaluate('(element) => element.disabled = false', more_results_button)
@@ -327,23 +361,38 @@
         page = await browser.new_page(user_agent=DEFAULT_USER_AGENT)
         
         if verbose():
             writerr(colored('[ Startpage ] Starting...', 'green'))
             
         await page.goto(f'https://www.startpage.com/', timeout=args.timeout*1000)
         
+        # Wait for the search results to be fully loaded
+        await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+        
         # Check if bot detection is shown
         if '/sp/captcha' in page.url:
             if args.show_browser:
-                writerr(colored(f'[ Startpage ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds...','yellow')) 
-                await asyncio.sleep(args.antibot_timeout)
+                writerr(colored(f'[ Startpage ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds, or when you type "startpage" and press ENTER...','yellow')) 
+                await wait_for_word_or_sleep("startpage", args.antibot_timeout)
+                writerr(colored(f'[ Startpage ] Resuming...', 'green'))
             else:
-                writerr(colored('[ Startpage ] CAPTCHA needed responding to. Consider using option -vb / --view-browser','red'))
+                writerr(colored('[ Startpage ] CAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
                 return set(endpoints)
-                
+
+        try:
+            # Wait for the search results to be fully loaded and have links
+            await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+        except:
+            pass
+
+        # Check if bot detection is still shown
+        if '/sp/captcha' in page.url:
+            writerr(colored('[ Startpage ] Failed to complete CAPTCHA','red'))
+            return set(endpoints)
+        
         await page.fill('input[title="Search"]', dork)
         await page.click('button.search-btn')
         
         # Wait for the search results to be fully loaded
         await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
         
         # Check if any '.result-link' exists
@@ -366,20 +415,32 @@
         # Loop until there is no submit button in the last form with action="/sp/search"
         while True:
             if stopProgram:
                 break
             # Check if bot detection is shown
             if '/sp/captcha' in page.url:
                 if args.show_browser:
-                    writerr(colored(f'[ Startpage ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds...','yellow')) 
-                    await asyncio.sleep(args.antibot_timeout)
+                    writerr(colored(f'[ Startpage ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds, or when you type "startpage" and press ENTER...','yellow')) 
+                    await wait_for_word_or_sleep("startpage", args.antibot_timeout)
+                    writerr(colored(f'[ Startpage ] Resuming...', 'green'))
                 else:
-                    writerr(colored('[ Startpage ] CAPTCHA needed responding to. Consider using option -vb / --view-browser','red'))
+                    writerr(colored('[ Startpage ] CAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
                     return set(endpoints)
             
+            try:
+                # Wait for the search results to be fully loaded and have links
+                await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+            except:
+                pass
+
+            # Check if bot detection is still shown
+            if '/sp/captcha' in page.url:
+                writerr(colored('[ Startpage ] Failed to complete CAPTCHA','red'))
+                return set(endpoints)
+        
             # Locate all forms with action="/sp/search" on the page
             forms = await page.query_selector_all('form[action="/sp/search"]')
             last_form = forms[-1]  # Get the last form
             
             # Get the current value of the "page" input field
             try:
                 curr_page_value = await last_form.evaluate('(form) => form.querySelector("input[name=\'page\']").value')
@@ -595,20 +656,33 @@
         
         pageNo = 1
         
         # If captcha is shown then allow time to submit it
         captcha = await page.query_selector('form#captcha-form')
         if captcha:
             if args.show_browser:
-                writerr(colored(f'[ Google ] reCAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds...','yellow')) 
-                await asyncio.sleep(args.antibot_timeout)
+                writerr(colored(f'[ Google ] reCAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds, or when you type "google" and press ENTER...','yellow')) 
+                await wait_for_word_or_sleep("google", args.antibot_timeout)
+                writerr(colored(f'[ Google ] Resuming...', 'green'))
             else:
-                writerr(colored('[ Google ] reCAPTCHA needed responding to. Consider using option -vb / --view-browser','red'))
+                writerr(colored('[ Google ] reCAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
                 return set(endpoints)
         
+        try:
+            # Wait for the search results to be fully loaded and have links
+            await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+        except:
+            pass
+
+        # Check if bot detection is still shown
+        captcha = await page.query_selector('form#captcha-form')
+        if captcha:
+            writerr(colored('[ Google ] Failed to complete reCAPTCHA','red'))
+            return set(endpoints)
+        
         # If the cookies notice is shown, accept it
         cookieAccept = await page.query_selector('button:has-text("Accept all")')
         if cookieAccept:
             await cookieAccept.click()
         
         # If the dialog box asking if you want location specific search, say Not now
         locationSpecific = await page.query_selector('g-raised-button:has-text("Not now")')
@@ -675,14 +749,151 @@
     finally:
         try:
             await page.close()
             semaphore.release()
         except:
             pass
 
+def extractYandexEndpoints(soup):
+    global allSubs
+    try:
+        endpoints = []
+        result_links = soup.find_all('a', class_=re.compile('.*organic__url.*'))
+        for link in result_links:
+            href = link.get('href')
+            if href and href.startswith('http') and not re.match(r'^https?:\/\/([\w-]+\.)*yandex\.[^\/\.]{2,}', href):
+                endpoints.append(href.strip())
+                # If the same search is going to be resubmitted without subs, get the subdomain
+                if args.resubmit_without_subs:
+                    allSubs.add(getSubdomain(href.strip()))
+        return endpoints
+    except Exception as e:
+        writerr(colored('ERROR extractYandexEndpoints 1: ' + str(e), 'red')) 
+        
+async def getYandex(browser, dork, semaphore):
+    try:
+        endpoints = []
+        page = None
+        await semaphore.acquire()
+        # Set the gdpr cookie to reduce the chances of getting Captcha page a bit
+        context = await browser.new_context(
+            storage_state={
+                'cookies': [{
+                    'name': 'gdpr',
+                    'value': '0',
+                    'domain': '.yandex.com',
+                    'path': '/'
+                }]
+            }
+        )
+        page = await context.new_page()
+    
+        if verbose():
+            writerr(colored('[ Yandex ] Starting...', 'green'))
+        
+        await page.goto(f'https://yandex.com/search/?text={dork}', timeout=args.timeout*1000)
+    
+        # Check if bot detection is shown
+        if '/showcaptcha' in page.url:
+            if args.show_browser:
+                writerr(colored(f'[ Yandex ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds, or when you type "yandex" and press ENTER...','yellow')) 
+                await wait_for_word_or_sleep("yandex", args.antibot_timeout)
+                writerr(colored(f'[ Yandex ] Resuming...', 'green'))
+            else:
+                writerr(colored('[ Yandex ] CAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
+                return set(endpoints)
+        try:
+            await page.wait_for_load_state('networkidle', timeout=1000)
+        except:
+            pass
+
+        # If still on Captcha page, then exit
+        if '/showcaptcha' in page.url:
+            writerr(colored('[ Yandex ] Failed to complete CAPTCHA','red'))
+            return set(endpoints)
+        
+        # Collect endpoints from the initial page
+        if vverbose():
+            writerr(colored('[ Yandex ] Getting endpoints from page 1', 'green', attrs=['dark'])) 
+        content = await page.content()
+        soup = BeautifulSoup(content, 'html.parser')
+        pageNo = 1
+        endpoints = extractYandexEndpoints(soup)
+
+        # Loop until there is no submit button in the last form with action="/sp/search"
+        while True:
+            if stopProgram:
+                break
+
+            # Click the Next button
+            await page.click('a[aria-label="Next page"]')
+            pageNo += 1
+            
+            # Check if bot detection is shown
+            if '/showcaptcha' in page.url:
+                if args.show_browser:
+                    writerr(colored(f'[ Yandex ] CAPTCHA needs responding to. Process will resume in {args.antibot_timeout} seconds, or when you type "yandex" and press ENTER...','yellow')) 
+                    await wait_for_word_or_sleep("yandex", args.antibot_timeout)
+                    writerr(colored(f'[ Yandex ] Resuming...', 'green'))
+                else:
+                    writerr(colored('[ Yandex ] CAPTCHA needed responding to. Consider using option -sb / --show-browser','red'))
+                    return set(endpoints)
+
+            try:
+                # Wait for the search results to be fully loaded and have links
+                await page.wait_for_load_state('networkidle', timeout=args.timeout*1000)
+            except:
+                pass
+
+            # If still on Captcha page, then exit
+            if '/showcaptcha' in page.url:
+                writerr(colored('[ Yandex ] Failed to complete CAPTCHA','red'))
+                return set(endpoints)
+
+            # Check if any classes containing organic__url exist
+            try:
+                await page.wait_for_selector('.organic__url', timeout=1000)
+            except:
+                break  # Break the loop if no '.organic__url' found
+        
+            if vverbose():
+                writerr(colored('[ Yandex ] Getting endpoints from page '+str(pageNo), 'green', attrs=['dark'])) 
+            
+            # Collect endpoints from the current page
+            content = await page.content()
+            soup = BeautifulSoup(content, 'html.parser')
+            endpoints += extractYandexEndpoints(soup)
+
+        await page.close()
+
+        setEndpoints = set(endpoints)
+        if verbose():
+            noOfEndpoints = len(setEndpoints)
+            writerr(colored(f'[ Yandex ] Complete! {str(noOfEndpoints)} endpoints found', 'green')) 
+        return setEndpoints
+    
+    except Exception as e:
+        noOfEndpoints  = len(set(endpoints))
+        if 'net::ERR_TIMED_OUT' in str(e) or 'Timeout' in str(e):
+            writerr(colored(f'[ Yandex ] Page timed out - got {str(noOfEndpoints)} results', 'red'))
+        elif 'net::ERR_ABORTED' in str(e) or 'Target page, context or browser has been closed' in str(e):
+            writerr(colored(f'[ Yandex ] Search aborted - got {str(noOfEndpoints)} results', 'red')) 
+        else:
+            writerr(colored('[ Yandex ] ERROR getYandex1: ' + str(e), 'red')) 
+        # If debug mode then save a copy of the page
+        if args.debug and page is not None:
+            await savePageContents('Yandex',page)
+        return set(endpoints)
+    finally:
+        try:
+            await page.close()
+            semaphore.release()
+        except:
+            pass
+        
 async def savePageContents(source, page):
     try:
         # Press the "Escape" key to stop page loading
         await page.keyboard.press("Escape")
 
         # Wait for a short duration to ensure the page loading is stopped
         await asyncio.sleep(2000)
@@ -696,15 +907,15 @@
             with open(filename, "w", encoding="utf-8") as file:
                 file.write(content)
             writerr(colored(f'[ {source} ] Saved HTML content to {filename}', 'cyan')) 
     except Exception as e:
         writerr(colored(f'[ {source} ] Unable to save page contents: {str(e)}', 'cyan')) 
 
 async def processInput(dork):
-    global browser, sourcesToProcess, duckduckgoEndpoints, bingEndpoints, startpageEndpoints, yahooEndpoints, googleEndpoints
+    global browser, sourcesToProcess, duckduckgoEndpoints, bingEndpoints, startpageEndpoints, yahooEndpoints, googleEndpoints, yandexEndpoints
     try:
         
         # Create a single browser instance
         async with async_playwright() as p:
             if args.show_browser:
                 browser = await p.chromium.launch(headless=False)
             else:
@@ -718,43 +929,34 @@
             if concurrentSources == 0 or concurrentSources > len(sourcesToProcess):
                 concurrentSources = len(sourcesToProcess)
             semaphore = asyncio.Semaphore(concurrentSources)
             
             # Define a list to hold the sources included in the gather call
             includedSources = []
             
-            # Check and add coroutines for DuckDuckGo and Bing if required
+            # Check and add coroutines for any required sources
             try:
                 if 'duckduckgo' in sourcesToProcess:
                     includedSources.append(getDuckDuckGo(browser, dork, semaphore))
                 if 'bing' in sourcesToProcess:
                     includedSources.append(getBing(browser, dork, semaphore))
                 if 'startpage' in sourcesToProcess:
                     includedSources.append(getStartpage(browser, dork, semaphore))
                 if 'yahoo' in sourcesToProcess:
                     includedSources.append(getYahoo(browser, dork, semaphore))
                 if 'google' in sourcesToProcess:
                     includedSources.append(getGoogle(browser, dork, semaphore))
+                if 'yandex' in sourcesToProcess:
+                    includedSources.append(getYandex(browser, dork, semaphore))
             except:
                 pass
             
             # Run all searches concurrently using the same browser instance
             results = await asyncio.gather(*includedSources)
             
-            # Populate the results dictionary
-            #for source, result in zip(sourcesToProcess, results):
-            #    resultsDict[source] = result
-            
-            # Access the results using the source names
-            #duckduckgoEndpoints = resultsDict.get('duckduckgo', [])
-            #bingEndpoints = resultsDict.get('bing', [])
-            #startpageEndpoints = resultsDict.get('startpage', [])
-            #yahooEndpoints = resultsDict.get('yahoo', [])
-            #googleEndpoints = resultsDict.get('google', [])
-            
             # Populate the results dictionary and endpoint lists
             for source, result in zip(sourcesToProcess, results):
                 if source not in resultsDict:  # Check if the source is not already in the resultsDict
                     resultsDict[source] = result  # If not, add it
                 else:
                     # If the source is already in the resultsDict, append new data to existing data
                     resultsDict[source].update(result)
@@ -766,14 +968,16 @@
                     bingEndpoints.update(result)
                 elif source == 'startpage':
                     startpageEndpoints.update(result)
                 elif source == 'yahoo':
                     yahooEndpoints.update(result)
                 elif source == 'google':
                     googleEndpoints.update(result)
+                elif source == 'yandex':
+                    yandexEndpoints.update(result)
         
             # Close the browser instance once all searches are done
             try:
                 await browser.close()
             except:
                 pass
         
@@ -782,15 +986,15 @@
     finally:
         try:
             await browser.close()
         except:
             pass
     
 async def processOutput():
-    global duckduckgoEndpoints, bingEndpoints, startpageEndpoints, yahooEndpoints, googleEndpoints, sourcesToProcess
+    global duckduckgoEndpoints, bingEndpoints, startpageEndpoints, yahooEndpoints, googleEndpoints, yandexEndpoints, sourcesToProcess
     try:
         allEndpoints = set()
 
         # If --output-sources was passed, then keep the source in the endpoint, otherwise we need a unique set without source
         if args.output_sources:
             if duckduckgoEndpoints:
                 allEndpoints.update(f'[ DuckDuckGo ] {endpoint}' for endpoint in duckduckgoEndpoints)
@@ -798,25 +1002,29 @@
                 allEndpoints.update(f'[ Bing ] {endpoint}' for endpoint in bingEndpoints)
             if startpageEndpoints:
                 allEndpoints.update(f'[ StartPage ] {endpoint}' for endpoint in startpageEndpoints)
             if yahooEndpoints:
                 allEndpoints.update(f'[ Yahoo ] {endpoint}' for endpoint in yahooEndpoints)
             if googleEndpoints:
                 allEndpoints.update(f'[ Google ] {endpoint}' for endpoint in googleEndpoints)
+            if yandexEndpoints:
+                allEndpoints.update(f'[ Yandex ] {endpoint}' for endpoint in yandexEndpoints)
         else:
             if duckduckgoEndpoints:
                 allEndpoints |= duckduckgoEndpoints
             if bingEndpoints:
                 allEndpoints |= bingEndpoints
             if startpageEndpoints:
                 allEndpoints |= startpageEndpoints
             if yahooEndpoints:
                 allEndpoints |= yahooEndpoints
             if googleEndpoints:
                 allEndpoints |= googleEndpoints
+            if yandexEndpoints:
+                allEndpoints |= yandexEndpoints
 
         if verbose() and sys.stdin.isatty():
             writerr(colored('\nTotal endpoints found: '+str(len(allEndpoints))+' 🤘  ', 'cyan')+str(sourcesToProcess))
             
         # If the -ow / --output_overwrite argument was passed and the file exists already, get the contents of the file to include
         appendedResults = False
         if args.output and not args.output_overwrite:
@@ -985,15 +1193,15 @@
     )
     parser.add_argument(
         '-sb',
         '--show-browser',
         action='store_true',
         help='View the browser instead of using headless browser.',
     )
-    default_abt = 30
+    default_abt = 90
     parser.add_argument(
         "-abt",
         "--antibot-timeout",
         help="How many seconds to wait when the -sb option was used and a known anti-bot mechanism is encountered. This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.",
         default=default_abt,
         type=int,
         metavar="<seconds>",
@@ -1055,16 +1263,16 @@
                 showBanner()
             if verbose():
                 showOptionsAndConfig()
             
         # Process the input given on -i (--input), or <stdin>
         await processInput(inputDork)
 
-        # Process the input given on -i (--input), or <stdin>
-        if args.resubmit_without_subs:
+        # If there were some subs found, and the --resubmit-without-subs was passed, then run again with subdomains removed
+        if len(allSubs) > 0 and args.resubmit_without_subs:
             inputDork = inputDork + ' ' + ' '.join(['-{}'.format(sub) for sub in allSubs if sub])
             write(colored('\nResubmitting again for input: ', 'magenta')+colored(inputDork,'white'))
             await processInput(inputDork)
         
         # Output the saved urls with parameters
         await processOutput()
```

### Comparing `xnldorker-1.0/xnldorker.egg-info/PKG-INFO` & `xnldorker-1.1/xnldorker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: xnldorker
-Version: 1.0
+Version: 1.1
 Summary: Run a dork on different search sites
 Home-page: https://github.com/xnl-h4ck3r/xnldorker
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 Requires-Dist: termcolor
 Requires-Dist: requests
 Requires-Dist: asyncio
 Requires-Dist: beautifulsoup4
 Requires-Dist: playwright
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/title.png"></center>
 
-## About - v1.0
+## About - v1.1
 
 This is a tool used to run a dork on different search sites.
-The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google**
+The available sources are currently: **DuckDuckGo, Bing, Startpage, Yahoo, Google, Yandex**
 
-**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` argument to specify the appropriate sources.**
+**IMPORTANT: If you use advanced search operators, be aware that operators that work on some of the sources may not work on others. You may need to use the `--sources` (and/or `--exclude-source`) argument to specify the appropriate sources.**
 
 **WARNING: If you use this tool a lot, then I guess there is the potential to get blocked on these source sites, so use sensibly. Using a VPN will help.**
 
 ## Installation
 
 `xnldorker` supports **Python 3**.
 
@@ -63,15 +63,15 @@
 | -os      | --output-sources     | Show the source of each endpoint in the output. Each endpoint will be prefixed, e.g. `[ Bing ] https://example.com`.                                                                                                                              |
 | -s       | --sources            | Specific sources to use when searching (e.g. `-s duckduckgo,bing`). Use `-ls` to display all available sources.                                                                                                                                   |
 | -es      | --exclude-sources    | Specific sources to exclude searching (`-s google,startpage`). Use `-ls` to display all available sources.                                                                                                                                        |
 | -cs      | --concurrent-sources | The number of sources to search at the same time (default: `2`). Passing `0` will run **ALL** specified sources at the same time (this could be very resource intensive and negatively affect results).                                           |
 | -ls      | --list-sources       | List all available sources.                                                                                                                                                                                                                       |
 | -t       | --timeout            | How many seconds to wait for the source to respond (default: 30 seconds)                                                                                                                                                                          |
 | -sb      | --show-browser       | View the browser instead of using a headless browser. This has an advantage because if there is a known anti-bot mechanism, then it will pause for a set time (determined by `-abt`) so you can manually resolve it before `xnldorker` continues. |
-| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 30). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
+| -abt     | --antibot-timeout    | How many seconds to wait when the `-sb` option was used and a known anti-bot mechanism is encountered (default: 90). This is the time you have to manually respond to the anti-bot mechanism before it tries to continue.                         |
 |          | --debug              | Save page contents on error.                                                                                                                                                                                                                      |
 | -nb      | --no-banner          | Hides the tool banner (it is hidden by default if you pipe input to 'xnldorker') output.                                                                                                                                                          |
 |          | --version            | Show current version number.                                                                                                                                                                                                                      |
 | -v       | --verbose            | Verbose output                                                                                                                                                                                                                                    |
 | -vv      | --vverbose           | Increased verbose output                                                                                                                                                                                                                          |
 
 ## Examples
@@ -101,22 +101,23 @@
 The output can also be piped to another command.
 
 <center><img src="https://github.com/xnl-h4ck3r/xnldorker/blob/main/xnldorker/images/example1.png"></center>
 
 ## Recommendations
 
 - Using `-v`/`--verbose` is always a good idea when you first start using a tool. It will help you understand what the tool is doing and highlight any potential problems too.
-- If you do mpt need to run silently in the background, I would recommend using the `-sb`/`--show-browser` option because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you do not need to run silently in the background, **I would recommend using the `-sb`/`--show-browser` argument** because you can see what `xnldorker` is doing (and if it seems to be working ok), plus if there is any known ant-bot detection recognised (currently not for all sources) then you will be notified and have the option to resolve this before `xnldorker` continues.
+- If you show the browsers and you get an anti-bot page shown, the process will be paused and wait for the number of seconds specified by `-abt`/`--antobit_timeout` (default 90 seconds). However, it you manually respond to the check and want it to resume quicker, you can enter the name of the source (in lowercase) and press ENTER to resume again.
 - The number of concurrent sources processed defaults to 2. This can be changed with `-cs`/`--concurrent-sources`. If you are running `xnldorker` on a low spec VPS, it could be worth setting `-cs 1`. The higher the value of `-cs` the quicker the tool will be, but may affect the quality and quantity of results.
 - You may want to run different dorks but write to the same output file. If you use the same output file in `-o`/`--output` then any results will be appended to that file automatically (and de-duplicated). But if you want to overwrite it every time, you can use the `-ow`/`--overwrite-output` argument.
 - Use the `--resubmit-without-subs` option to resubmit the same search, but with all previously found subs removed from the search (where possible, dependant on the source).
 - If I was looking at a new target, `example.com` I would start with running the command below. I would use `-v` to have more insight into what is happening, `-sb` to show the browsers so that I could respond to ant-bot mechanism if shown, `-rwos` to resubmit the same search but excluding the subdomains found in the first search, and `-o` to specify the output file to save the results:
 
 ```sh
-xnldorker -i "example.com" -v -sb -rwos -o example.com_xnldorker.txt
+xnldorker -i "example.com" -v -t 120 -sb -rwos -o example.com_xnldorker.txt
 ```
 
 - After the previous point, I would consider changing my VPN to s different region and re-run to potentially get different results.
 
 ## Issues
 
 If you come across any problems at all, or have ideas for improvements, please feel free to raise an issue on Github. If there is a problem, it will be useful if you can provide the exact command you ran and a detailed description of the problem. If possible, run with `-v` to reproduce the problem and let me know about any error messages that are given.
```

