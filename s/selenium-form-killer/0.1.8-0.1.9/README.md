# Comparing `tmp/selenium_form_killer-0.1.8.tar.gz` & `tmp/selenium_form_killer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_form_killer-0.1.8.tar", max compression
+gzip compressed data, was "selenium_form_killer-0.1.9.tar", max compression
```

## Comparing `selenium_form_killer-0.1.8.tar` & `selenium_form_killer-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1351 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/README.md
--rw-r--r--   0        0        0      709 2024-04-29 19:05:43.564414 selenium_form_killer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       65 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/__init__.py
--rw-r--r--   0        0        0       37 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/anti_captcha/__init__.py
--rw-r--r--   0        0        0     3402 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/anti_captcha/anti_captcha.py
--rw-r--r--   0        0        0       43 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/capmonster/__init__.py
--rw-r--r--   0        0        0      648 2024-04-29 17:29:32.209655 selenium_form_killer-0.1.8/selenium_form_killer/capmonster/captcha_breaker.py
--rw-r--r--   0        0        0      330 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/forms.py
--rw-r--r--   0        0        0    15803 2024-04-29 19:03:05.946653 selenium_form_killer-0.1.8/selenium_form_killer/killer.py
--rw-r--r--   0        0        0      748 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.8/selenium_form_killer/log/logger.py
--rw-r--r--   0        0        0        0 2024-04-29 14:48:53.342634 selenium_form_killer-0.1.8/selenium_form_killer/util/__init__.py
--rw-r--r--   0        0        0      221 2024-04-29 14:48:53.342634 selenium_form_killer-0.1.8/selenium_form_killer/util/util.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 selenium_form_killer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.9/README.md
+-rw-r--r--   0        0        0      787 2024-05-14 14:38:10.004014 selenium_form_killer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-29 14:48:53.338634 selenium_form_killer-0.1.9/selenium_form_killer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:06.682000 selenium_form_killer-0.1.9/selenium_form_killer/anti_captcha/__init__.py
+-rw-r--r--   0        0        0     3403 2024-04-30 17:46:42.106305 selenium_form_killer-0.1.9/selenium_form_killer/anti_captcha/anti_captcha.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:47:06.682000 selenium_form_killer-0.1.9/selenium_form_killer/capmonster/__init__.py
+-rw-r--r--   0        0        0      646 2024-04-30 17:46:42.110305 selenium_form_killer-0.1.9/selenium_form_killer/capmonster/captcha_breaker.py
+-rw-r--r--   0        0        0     4751 2024-04-30 18:32:20.242566 selenium_form_killer-0.1.9/selenium_form_killer/forms.py
+-rw-r--r--   0        0        0    16167 2024-05-12 18:14:04.123437 selenium_form_killer-0.1.9/selenium_form_killer/killer.py
+-rw-r--r--   0        0        0      673 2024-04-30 17:46:36.642373 selenium_form_killer-0.1.9/selenium_form_killer/log/logger.py
+-rw-r--r--   0        0        0      147 2024-04-30 19:16:09.812204 selenium_form_killer-0.1.9/selenium_form_killer/types/generic_types.py
+-rw-r--r--   0        0        0     6231 2024-05-12 18:02:48.096729 selenium_form_killer-0.1.9/selenium_form_killer/types/selenium_types.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:48:53.342634 selenium_form_killer-0.1.9/selenium_form_killer/util/__init__.py
+-rw-r--r--   0        0        0      224 2024-04-30 17:46:42.102305 selenium_form_killer-0.1.9/selenium_form_killer/util/util.py
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 selenium_form_killer-0.1.9/PKG-INFO
```

### Comparing `selenium_form_killer-0.1.8/README.md` & `selenium_form_killer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `selenium_form_killer-0.1.8/pyproject.toml` & `selenium_form_killer-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selenium-form-killer"
-version = "0.1.8"
+version = "0.1.9"
 license = "MIT"
 description = ""
 authors = ["Rodrigoneal <rodrigho2006@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,14 +13,18 @@
 bs4 = "^0.0.2"
 capmonstercloudclient = "^1.3.4"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
 pytest-asyncio = "^0.23.5"
 chardet = "^5.2.0"
 loguru = "^0.7.2"
+respx = "^0.21.1"
+coverage = "^7.5.0"
+mypy = "^1.10.0"
+playwright = "^1.43.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
 
 
 [tool.poetry.group.linter.dependencies]
```

### Comparing `selenium_form_killer-0.1.8/selenium_form_killer/anti_captcha/anti_captcha.py` & `selenium_form_killer-0.1.9/selenium_form_killer/anti_captcha/anti_captcha.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+
 import httpx
 
 
 class AntiCaptcha:
     def __init__(self, api_key: str):
         self.__api_key = api_key
```

### Comparing `selenium_form_killer-0.1.8/selenium_form_killer/capmonster/captcha_breaker.py` & `selenium_form_killer-0.1.9/selenium_form_killer/capmonster/captcha_breaker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from capmonstercloudclient import CapMonsterClient, ClientOptions
-
 from capmonstercloudclient.requests.baseRequest import BaseRequest
 
-
 from selenium_form_killer.log.logger import get_logger
 
 logger = get_logger()
 
 
 async def captcha_token(
     request_captcha: BaseRequest, api_key: str, client_timeout: int = 30
```

### Comparing `selenium_form_killer-0.1.8/selenium_form_killer/killer.py` & `selenium_form_killer-0.1.9/selenium_form_killer/killer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 import asyncio
-from typing import Annotated, Literal, Optional
+import os
+from tempfile import NamedTemporaryFile, TemporaryFile
+from typing import Literal, Optional, Sequence
 from urllib.parse import urlencode
-from typing_extensions import Doc
-from bs4 import BeautifulSoup
-import httpx
-import chardet
+import warnings
+import webbrowser
 
+import chardet
+import httpx
 import requests
-from selenium_form_killer.log.logger import get_logger
+from bs4 import BeautifulSoup
+from typing_extensions import override, Self
 
+from selenium_form_killer.forms import Form, FormInput
+from selenium_form_killer.types.generic_types import ActionTypes
+from selenium_form_killer.types.selenium_types import (
+    FormInputABC,
+    SeleniumKillerABC,
+)
 from selenium_form_killer.util.util import get_base_url, join_url_action
+from playwright.async_api import async_playwright
 
 
-class SeleniumKiller:
+class SeleniumKiller(SeleniumKillerABC):
     def __init__(self, headers: dict[str, str] = {}, verbose: bool = False) -> None:
-        self.url_base: str = None
-        self.headers: Annotated[
-            Optional[dict[str, str]], Doc("Cabecalhos da requisição")
-        ] = headers or {}
-        self.data: Annotated[Optional[str], Doc("Dados da requisição")] = None
-        self.cookies: Annotated[Optional[str], Doc("Cookies da requisição")] = None
-        self._response = None
-        self._forms: list[Form] = None
-        self.status_code: Annotated[
-            Optional[int], Doc("Status code da requisição")
-        ] = None
-        self.session = httpx.AsyncClient(
-            headers=headers,
-        )
-        self.logger = get_logger(verbose)
+        super().__init__(headers=headers, verbose=verbose)
 
     @classmethod
     def from_auth_data(
         cls, url: str, payload: dict, key_token: Optional[str] = None
     ) -> "SeleniumKiller":
+        """
+        Faz uma solicitação POST para o URL fornecido com o payload e retorna uma nova instância de SeleniumKiller com o cabeçalho Authorization definido.
+
+        Se o key_token não for fornecido, ele será padrão para "access_token".
+
+        :param url: URL do endpoint
+        :param payload: dados a serem enviados
+        :param key_token: chave no JSON de resposta que contém o access_token
+
+        """
         payload_data = urlencode(payload)
         key_token = key_token if key_token else "access_token"
-        with httpx.Client() as client:
+        with httpx.Client() as client:  # Achei melhor não usar o proprio request do objeto para não sujar os cookies e etc.
             response = client.post(url, data=payload_data)
+            response.raise_for_status()
+            token = response.json()[key_token]
+            headers = {"Authorization": f"Bearer {token}"}
+            return cls(headers=headers, verbose=True)
 
-            if response.status_code == 200:
-                token = response.json()["access_token"]
-                headers = {"Authorization": f"Bearer {token}"}
-            return cls(headers=headers, verbose=False)
-
-    def __call__(self, *args, **kwargs):
-        return self.__class__(*args, **kwargs)
-
-    def __soup(self, html: Optional[str] = None) -> BeautifulSoup:
-        html = html or self._response.text
-        soup = BeautifulSoup(html, "html.parser")
-        return soup
-
-    def find(self, *args, html: Optional[str] = None, **kwargs):
+    def find(self, *args, html: Optional[str] = None, **kwargs) -> BeautifulSoup:
         self.logger.info(f"find element with args: {args}, kwargs: {kwargs}")
-        soup = self.__soup(html)
+        soup = self.soup(html)
         return soup.find(*args, **kwargs)
 
-    def find_all(self, *args, html: Optional[str] = None, **kwargs):
+    def find_all(
+        self, *args, html: Optional[str] = None, **kwargs
+    ) -> list[BeautifulSoup]:
         self.logger.info(f"find elements with args: {args}, kwargs: {kwargs}")
-        soup = self.__soup(html)
+        soup = self.soup(html)
         return soup.find_all(*args, **kwargs)
 
-    def soup(self, html: Optional[str] = None):
+    def soup(self, html: Optional[str] = None) -> BeautifulSoup:
         html_text = html or self._response.text
-        return self.__soup(html_text)
+        soup = BeautifulSoup(html_text, "html.parser")
+        return soup
 
     async def __aenter__(self):
         self.logger.info("Entering async context")
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if not exc_type:
@@ -76,18 +76,20 @@
         else:
             self.logger.critical(
                 f"Exiting async context with exc_type:{exc_type}, exc_val:{exc_val}, exc_tb:{exc_tb}"
             )
         await self.session.aclose()
         self.logger.info("Session closed")
 
-    def _forms_soup(self, html: Optional[str] = None) -> BeautifulSoup:
-        html = html or self._response.text
-        soup = BeautifulSoup(html, "html.parser")
-        return soup.find_all("form")
+    async def close(self):
+        """
+        Fecha a sessão do httpx.
+        """
+        self.logger.info("Session closed")
+        await self.session.aclose()
 
     @property
     def forms(self) -> list["Form"]:
         return self._forms
 
     @forms.setter
     def forms(self, value: str) -> None:
@@ -96,37 +98,40 @@
 
     async def _requests(self, **kwargs) -> requests.Response:
         self.logger.info(
             f"Making request with kwargs: {kwargs}",
         )
         return await self.session.request(**kwargs)
 
-    async def send_request(
-        self, method: Literal["GET", "POST"], url: str, **kwargs
-    ) -> requests.Response:
-        response = await self._requests(method=method, url=url, **kwargs)
+    async def __handle_response(self, response: requests.Response) -> None:
         encoding = chardet.detect(response.content)["encoding"]
         response.encoding = encoding
         self.headers = response.headers
         self.cookies = response.cookies
         self.status_code = response.status_code
         self.response = response
         self.forms = self.extract_forms()
         self.url_base = get_base_url(str(response.url))
         return self
 
+    async def send_request(
+        self, method: Literal["GET", "POST"], url: str, **kwargs
+    ) -> requests.Response:
+        response = await self._requests(method=method, url=url, **kwargs)
+        return await self.__handle_response(response)
+
     async def get(
         self,
         url: str,
         headers: Optional[dict] = dict(),
         cookies: Optional[dict] = dict(),
         params: Optional[dict] = dict(),
         use_referer: bool = True,
         **kwargs,
-    ) -> requests.Response:
+    ) -> Self:
         self.logger.info(
             f"Making get request with url: {url}, headers:{headers}, cookies:{cookies}, params: {params}, use_referer: {use_referer}, kwargs: {kwargs}"
         )
         await self.make_request(
             method="GET",
             url=url,
             headers=headers,
@@ -136,15 +141,15 @@
             **kwargs,
         )
 
         return self
 
     def _prepare_form_to_request(
         self, form: "Form", fields_delete: Optional[list["FormInput"]]
-    ) -> None:
+    ) -> dict[str, str]:
         self.logger.info(
             f"Preparing form to request with form: {form}, fields_delete: {fields_delete}",
         )
         data = {"data": {}}
         data["method"] = form.method.upper()
         if form.url_base:
             data["url"] = join_url_action(form.url_base, form.action)
@@ -153,60 +158,144 @@
         for input_form in form.inputs:
             for field in fields_delete or []:
                 if input_form.name == field.name:
                     continue
             data["data"][input_form.name] = input_form.value
         return data
 
-    def post(
+    async def post(
         self,
         url: Optional[str] = None,
         headers: Optional[dict[str, str]] = {},
         cookies: Optional[dict[str, str]] = {},
         data: Optional[dict[str, str]] = {},
         params: Optional[dict[str, str]] = {},
         use_referer: bool = True,
         inputs: Optional[list["FormInput"] | dict[str, str]] = None,
         token: Optional[dict] = {},
-        form: Optional["Form"] = False,
+        form: Optional["Form"] = None,
         exclude_forms: Optional[list["FormInput"]] = None,
         **kwargs,
-    ):
+    ) -> Self:
         self.logger.info(f"Making post request with url: {url} e kwargs: {kwargs}")
 
-        return self.make_request(
+        return await self.make_request(
             method="POST",
             url=url,
             headers=headers,
             cookies=cookies,
             data=data,
             params=params,
             use_referer=use_referer,
             inputs=inputs,
             token=token,
             form=form,
             exclude_forms=exclude_forms,
             **kwargs,
         )
 
+    async def render(self, timeout: int = 5, debug: bool = False) -> Self:
+        """Renderiza a pagina que precisa de javascript para funcionar.
+        Quando o modo debug for True o navegador vai desabilitar o headless.
+
+        Keyword Arguments:
+            timeout -- Tempo para aguardar a pagina a renderizar em segundos (default: {5})
+            debug -- Habilita o modo debug (default: {False})
+
+        Returns:
+            self
+        """
+        _timeout = timeout * 1000
+        self.logger.info(f"Renderizando a pagina com timeout: {timeout}")
+        os_name = os.name
+        if os_name == "nt":
+            warnings.warn("A renderização no windows está muito lenta")
+        async with async_playwright() as p:
+            browser = await p.chromium.launch(
+                headless=True if not debug else False,
+                args=["--disable-web-security"],
+                ignore_default_args=[
+                    "--disable-extensions",
+                    "--disable-default-apps",
+                    "--disable-component-extensions-with-background-pages",
+                ],
+            )
+            context = await browser.new_context(
+                bypass_csp=True,
+                java_script_enabled=True,
+                user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 16_0 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/105.0.5195.100 Mobile/15E148 Safari/604.1",
+            )
+            page = await context.new_page()
+            if os_name == "nt":
+                await page.set_content(
+                    self.response.content.decode("utf-8"), wait_until="domcontentloaded"
+                )
+            else:
+                await page.set_content(self.response.content.decode("utf-8"))
+            await page.wait_for_timeout(_timeout)
+            html = await page.content()
+            await browser.close()
+            self._response = httpx.Response(
+                content=html.encode("utf-8"), status_code=self.status_code, text=html
+            )
+            return self
+
+    async def click_by_browser(
+        self, element_click: str, timeout: int = 5, debug: bool = False
+    ) -> Self:
+        _timeout = timeout * 1000
+        self.logger.info(f"Renderizando a pagina com timeout: {timeout}")
+        os_name = os.name
+        if os_name == "nt":
+            warnings.warn("A renderização no windows está muito lenta")
+        async with async_playwright() as p:
+            browser = await p.chromium.launch(
+                headless=True if not debug else False,
+                args=["--disable-web-security"],
+                ignore_default_args=[
+                    "--disable-extensions",
+                    "--disable-default-apps",
+                    "--disable-component-extensions-with-background-pages",
+                ],
+            )
+            context = await browser.new_context(
+                bypass_csp=True,
+                java_script_enabled=True,
+                user_agent="Mozilla/5.0 (iPhone; CPU iPhone OS 16_0 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/105.0.5195.100 Mobile/15E148 Safari/604.1",
+            )
+            page = await context.new_page()
+            if os_name == "nt":
+                await page.set_content(
+                    self.response.content.decode("utf-8"), wait_until="domcontentloaded"
+                )
+            else:
+                await page.set_content(self.response.content.decode("utf-8"))
+            await page.wait_for_timeout(_timeout)
+            html = await page.content()
+            await browser.close()
+            self._response = httpx.Response(
+                content=html.encode("utf-8"), status_code=self.status_code, text=html
+            )
+            return self
+
     async def make_request(
         self,
         method: Literal["GET", "POST"],
         url: Optional[str] = None,
         headers: Optional[dict[str, str]] = {},
         cookies: Optional[dict[str, str]] = {},
         data: Optional[dict[str, str]] = {},
         params: Optional[dict[str, str]] = {},
         use_referer: bool = True,
         inputs: Optional[list["FormInput"] | dict[str, str]] = None,
         token: Optional[dict] = {},
         form: Optional["Form"] = False,
         exclude_forms: Optional[list["FormInput"]] = None,
         **httpx_options: dict[str, str],
-    ) -> requests.Response:
+    ) -> Self:
         if use_referer and self.response:
             self.logger.info(f"Using referer:{str(self.response.url)}")
             self.response.headers["Referer"] = str(self.response.url)
         if inputs:
             if not isinstance(inputs, list):
                 inputs = [FormInput(**input) for input in inputs.items()]
             for input in inputs:
@@ -227,60 +316,81 @@
             cookies=cookies,
             data=data,
             params=params,
             **httpx_options,
         )
         return self
 
-    def extract_inputs(self, formulario: BeautifulSoup) -> list["FormInput"]:
+    def open_response_in_browser(self) -> bool:
+        """
+        Abre a resposta da requisição no browser.
+        Isso é muito util quando está automatizando um formulario para saber se os dados foram preenchidos corretamente.
+
+        Returns:
+            bool: Retorna True se o browser foi aberto com sucesso.
+        """
+        with NamedTemporaryFile(suffix=".html", delete=False) as f:
+            self.logger.info(f"Abrindo a resposta em um browser em: {f.name}")
+            f.write(self.response.content)
+            return webbrowser.open(f.name, 2, False)
+
+    def extract_inputs(self, formulario: BeautifulSoup) -> list[FormInputABC]:
         inputs = formulario.find_all(["input", "textarea"])
         _inputs = []
         for input_tag in inputs:
             nome = input_tag.get("name")
             valor = input_tag.get("value", "")
             if input_tag.get("type"):
                 _type = input_tag.get("type")
             else:
                 _type = "text"
             form_input = FormInput(name=nome, value=valor, type=_type)
             self.logger.info(f"Extracting inputs: {form_input}")
             _inputs.append(form_input)
         return _inputs
 
-    def extract_actions(self, formulario: BeautifulSoup) -> list[str]:
-        form_action = {"action": None, "id": None, "name": None, "method": None}
+    def extract_actions(self, formulario: BeautifulSoup) -> ActionTypes:
+        form_action: ActionTypes = {
+            "action": None,
+            "id": None,
+            "name": None,
+            "method": None,
+        }
         form_action["action"] = formulario.get("action")
         form_action["id"] = formulario.get("id")
         form_action["name"] = formulario.get("name")
         form_action["method"] = formulario.get("method")
         self.logger.info(f"Extracting actions from form:{form_action}")
         return form_action
 
-    def extract_captcha(self, formulario: BeautifulSoup) -> str:
+    def extract_captcha(self, formulario: BeautifulSoup) -> str | None:
         captchas = formulario.find_all(
             class_=lambda value: value and "captcha" in value
         )
         for captcha in captchas:
             if data_site := captcha.get("data-sitekey"):
                 self.logger.info(
                     f"Extracting captcha from form: {captcha} data-sitekey: {data_site}"
                 )
                 return data_site
             else:
                 self.logger.error(
                     f"Extracting captcha from form: {captcha} not found data-sitekey"
                 )
+        return None
 
-    def extract_forms(self, html: Optional[str] = None) -> list["Form"]:
+    @override
+    def extract_forms(self, html: Optional[str] = None) -> Sequence["Form"]:
         self.logger.info("Extracting forms")
         forms = []
-        for formulario in self._forms_soup(html):
+        for formulario in self.find_all("form", html=html):
             _captcha = self.extract_captcha(formulario)
             extract_actions = self.extract_actions(formulario)
             _inputs = self.extract_inputs(formulario)
+
             forms.append(
                 Form(
                     killer=self,
                     inputs=_inputs,
                     captcha=_captcha,
                     button=None,
                     url_base=str(self.response.url),
@@ -313,129 +423,7 @@
 
     def __repr__(self) -> str:
         if self.response:
             return str(
                 f"<SeleniumKiller: url={str(self.response.url)} status={self.response} >"
             )
         return str("<SeleniumKiller: None>")
-
-
-class Form:
-    def __init__(
-        self,
-        killer: SeleniumKiller,
-        inputs: list["FormInput"],
-        action: str,
-        method: str,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        captcha: Optional[str] = None,
-        button: Optional[dict[str, str]] = None,
-        url_base: Optional[str] = None,
-    ) -> None:
-        self.inputs = inputs
-        self.action = action
-        self.method = method
-        self.id = id
-        self.name = name
-        self.button = button
-        self.captcha = captcha
-        self.url_base = url_base
-        self.__killer = killer
-
-    def pretty_print(self) -> None:
-        for index, input in enumerate(self.inputs):
-            print(f"{index}: {input}")
-
-    def __repr__(self) -> str:
-        if self.inputs:
-            if len(self.inputs) > 9:
-                str_inputs = ", ".join(
-                    [
-                        str(index) + ": " + str(input)
-                        for index, input in enumerate(self.inputs[:9])
-                    ]
-                )
-                str_inputs += ", ..."
-                return str(f"<Form: {self.id=}, {str_inputs=}>")
-            else:
-                str_inputs = ", ".join(
-                    [
-                        str(index) + ": " + str(input)
-                        for index, input in enumerate(self.inputs)
-                    ]
-                )
-                return str(f"<Form: {self.id=}, {str_inputs=}>")
-        return str(f"<Form: {self.id=}>")
-
-    def add_input(self, name: str, value: str, type: str = "text") -> None:
-        self.inputs.append(FormInput(name=name, value=value, type=type))
-
-    def delete_input(self, name: str) -> None:
-        self.inputs = [input for input in self.inputs if input.name != name]
-
-    def total_inputs(self) -> int:
-        return len(self.inputs)
-
-    def get_input(self, name: str) -> "FormInput":
-        for input in self.inputs:
-            if input.name == name:
-                return input
-
-    async def submit(
-        self,
-        url: Optional[str] = None,
-        token: Optional[dict[str, str]] = {},
-        method: str = None,
-        input_data: str | list["FormInput"] | list[int] | None = "all",
-        input_query_params: str | list["FormInput"] | list[int] | None = None,
-        **kwargs,
-    ) -> SeleniumKiller:
-        self.__killer.logger.info(f"Submitting form: {self}")
-        if not self.method and not method:
-            raise ValueError(
-                "method is required" + "Form: " + str(self) + "Not have method"
-            )
-        elif method:
-            self.method = method
-        if input_query_params == "all":
-            params = {input.name: input.value for input in self.inputs}
-            kwargs["params"] = params
-        elif isinstance(input_query_params, list):
-            if isinstance(input_query_params[0], int):
-                inputs = [self.inputs[indice] for indice in input_query_params]
-                params = {input.name: input.value for input in inputs}
-                kwargs["params"] = params
-            elif isinstance(input_data[0], FormInput):
-                kwargs["params"] = {input.name: input.value for input in self.inputs}
-
-        if input_data == "all":
-            pass
-        elif isinstance(input_data, list):
-            if isinstance(input_data[0], int):
-                self.inputs = [self.inputs[indice] for indice in input_data]
-            elif isinstance(input_data[0], FormInput):
-                self.inputs = input_data
-        elif not input_data:
-            self.inputs = []
-        kwargs["data"] = {input.name: input.value for input in self.inputs}
-
-        if token:
-            kwargs["data"].update(token)
-
-        if not url:
-            url = join_url_action(self.url_base, self.action)
-        await self.__killer.send_request(method=self.method, url=url, **kwargs)
-        return self.__killer
-
-
-class FormInput:
-    def __init__(self, name: str, value: str, type: str = "text") -> None:
-        self.type = type
-        self.name = name
-        self.value = value
-
-    def __repr__(self) -> str:
-        return str(f"<FormInput: name:{self.name} type:{self.type} value:{self.value}>")
-
-    def to_dict(self) -> dict:
-        return {self.name: self.value}
```

### Comparing `selenium_form_killer-0.1.8/PKG-INFO` & `selenium_form_killer-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: selenium-form-killer
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: Rodrigoneal
 Author-email: rodrigho2006@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: capmonstercloudclient (>=1.3.4,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
+Requires-Dist: coverage (>=7.5.0,<8.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: mypy (>=1.10.0,<2.0.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.5,<0.24.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: respx (>=0.21.1,<0.22.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Selenium Killer
 
 ## Introdução
```

