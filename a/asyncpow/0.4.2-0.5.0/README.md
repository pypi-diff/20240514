# Comparing `tmp/asyncpow-0.4.2.tar.gz` & `tmp/asyncpow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpow-0.4.2.tar", max compression
+gzip compressed data, was "asyncpow-0.5.0.tar", max compression
```

## Comparing `asyncpow-0.4.2.tar` & `asyncpow-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     6694 2024-04-15 16:21:59.097174 asyncpow-0.4.2/README.md
--rw-r--r--   0        0        0     1215 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/__init__.py
--rw-r--r--   0        0        0     4908 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/media.py
--rw-r--r--   0        0        0     2781 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/movie.py
--rw-r--r--   0        0        0     6053 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/request.py
--rw-r--r--   0        0        0     5290 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/search.py
--rw-r--r--   0        0        0     3006 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/status.py
--rw-r--r--   0        0        0     2848 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/apis/tv.py
--rw-r--r--   0        0        0     1176 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/const.py
--rw-r--r--   0        0        0     1781 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/exceptions.py
--rw-r--r--   0        0        0     4995 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/common.py
--rw-r--r--   0        0        0     4026 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/media.py
--rw-r--r--   0        0        0     3815 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/movie.py
--rw-r--r--   0        0        0     1574 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/request.py
--rw-r--r--   0        0        0     5039 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/search.py
--rw-r--r--   0        0        0     1546 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/status.py
--rw-r--r--   0        0        0     3085 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/models/tv.py
--rw-r--r--   0        0        0     4502 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/overseerr.py
--rw-r--r--   0        0        0        0 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/py.typed
--rw-r--r--   0        0        0     4096 2024-04-15 16:21:59.097174 asyncpow-0.4.2/asyncpow/utils/http.py
--rw-r--r--   0        0        0     2919 2024-04-15 16:22:48.329913 asyncpow-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6837 2024-05-14 10:44:33.631772 asyncpow-0.5.0/README.md
+-rw-r--r--   0        0        0     1215 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/apis/media.py
+-rw-r--r--   0        0        0     2970 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/apis/movie.py
+-rw-r--r--   0        0        0     6214 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/apis/request.py
+-rw-r--r--   0        0        0     5596 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/apis/search.py
+-rw-r--r--   0        0        0     3385 2024-05-14 10:44:33.631772 asyncpow-0.5.0/asyncpow/apis/status.py
+-rw-r--r--   0        0        0     3059 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/apis/tv.py
+-rw-r--r--   0        0        0     5319 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/apis/user.py
+-rw-r--r--   0        0        0     1176 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/const.py
+-rw-r--r--   0        0        0     1781 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/exceptions.py
+-rw-r--r--   0        0        0     4132 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/common.py
+-rw-r--r--   0        0        0     1709 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/issue.py
+-rw-r--r--   0        0        0     4119 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/media.py
+-rw-r--r--   0        0        0     3815 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/movie.py
+-rw-r--r--   0        0        0     1574 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/request.py
+-rw-r--r--   0        0        0     5037 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/search.py
+-rw-r--r--   0        0        0     1546 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/status.py
+-rw-r--r--   0        0        0     3085 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/tv.py
+-rw-r--r--   0        0        0     2998 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/models/user.py
+-rw-r--r--   0        0        0     5224 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/overseerr.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/py.typed
+-rw-r--r--   0        0        0      775 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/utils/api_key.py
+-rw-r--r--   0        0        0     4096 2024-05-14 10:44:33.635772 asyncpow-0.5.0/asyncpow/utils/http.py
+-rw-r--r--   0        0        0     2919 2024-05-14 10:45:23.159721 asyncpow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 asyncpow-0.5.0/PKG-INFO
```

### Comparing `asyncpow-0.4.2/README.md` & `asyncpow-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 This project is a work in progress, the main branch is being developed on live, which may cause breaking changes until the first full release.
 
 The library returns results in JSON format for ease of use, this also reduces the risk of failue when the APIs are updated.
 
-Type hints and type models are in place for all of the APIs, if you notice missing items please create a request to have it fixed.
+Type hints and type models are in place where possible (this API has terrible circular dependencies which breaks python), if you notice missing items please create a request to have it fixed.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Built With
 
 [![python][python]][python-url]
 
@@ -93,15 +93,19 @@
 * Discover - WIP
   * Trending - Completed
 * Media - WIP
   * Get - Completed
   * Update Status - Completed
   * Delete
   * Get Watch Data
-
+* User - WIP
+  * Get - Completed
+  * Bulk Update - Completed
+  * Update
+  * Delete
 
 ## Compatibility
 
 AsyncPOW is built for Python 3.12, and initially the v1 Overseerr API
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -24,26 +24,28 @@
    8. _L_i_c_e_n_s_e
    9. _C_o_n_t_a_c_t
   10. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About The Project This project is a work in progress, the main branch is
 being developed on live, which may cause breaking changes until the first full
 release. The library returns results in JSON format for ease of use, this also
 reduces the risk of failue when the APIs are updated. Type hints and type
-models are in place for all of the APIs, if you notice missing items please
-create a request to have it fixed.
+models are in place where possible (this API has terrible circular dependencies
+which breaks python), if you notice missing items please create a request to
+have it fixed.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With [![python][python]][python-url]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started * [QuickStart Guide](https://docs.totaldebug.uk/asyncpow/
 quickstart.html) * [Full Documentation](https://docs.totaldebug.uk/asyncpow) *
 [Release Notes](https://github.com/totaldebug/asyncpow/releases)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Features * Asynchronous * Type Checking * Status - Completed * Discover -
 WIP * Trending - Completed * Media - WIP * Get - Completed * Update Status -
-Completed * Delete * Get Watch Data ## Compatibility AsyncPOW is built for
+Completed * Delete * Get Watch Data * User - WIP * Get - Completed * Bulk
+Update - Completed * Update * Delete ## Compatibility AsyncPOW is built for
 Python 3.12, and initially the v1 Overseerr API
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Roadmap See the [feature requests](https://github.com/totaldebug/asyncpow/
 labels/type%2Ffeature) for a full list of requested features.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Sponsor My projects arent possible without the support of the community,
 please consider donating a small amount to keep these projects alive. [!
```

### Comparing `asyncpow-0.4.2/asyncpow/__init__.py` & `asyncpow-0.5.0/asyncpow/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/apis/media.py` & `asyncpow-0.5.0/asyncpow/apis/media.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,51 +33,58 @@
 class Media:
     """
     Class to interact with media-related endpoints.
 
     Initialize the Media object with the base URL, API key, and session.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """
         Initialize the MediaAPI object with the base URL and API key.
 
         Args:
             base_url (str): The base URL for the media API.
             api_key (str): The API key for authentication.
             session (ClientSession): HTTP Session
+            raw_response (bool): Return json if True.
 
         Returns:
             None
         """
         self.media_url = base_url.joinpath("media")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
 
     async def async_get_media(
         self,
         take: int = 20,
         skip: int = 0,
         filter: MediaFilterOptions | None = None,
         sort: SortOptions | None = None,
-        raw_response: bool = False,
+        raw_response: bool | None = None,
     ) -> dict | MediaModel:
         """
         Get media items based on specified parameters.
 
         Args:
             take (int): The number of items to retrieve (default is 20).
             skip (int): The number of items to skip (default is 0).
             filter (MediaFilterOptions): The filter option for media items (default is None).
             sort (SortOptions): The sorting option for media items (default is None).
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
 
         Returns:
             dict | MediaModel: The media model object retrieved based on the parameters.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
+
         params: dict = {"take": take, "skip": skip}
         if filter:
             params["filter"] = filter
         if sort:
             params["sort"] = sort
 
         headers = {"X-Api-Key": self.api_key}
@@ -85,28 +92,30 @@
         return response if raw_response else MediaModel(**response)
 
     async def async_post_media_status(
         self,
         mediaId: int,
         status: MediaStatusOptions,
         is4k: Optional[bool] = None,
-        raw_response: bool = False,
+        raw_response: bool | None = None,
     ) -> dict | MediaModel2:
         """
         Update the status of a media item with optional 4k flag.
 
         Args:
             mediaId (int): The ID of the media item.
             status (MediaStatusOptions): The status to set for the media item.
             is4k (Optional[bool]): Optional flag indicating 4k status.
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
 
         Returns:
             dict | MediaModel2: The model object representing the updated media item.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
 
         url = self.media_url.joinpath(str(mediaId), str(status))
         data = {"is4k": is4k} if is4k else {}
         headers = {"X-Api-Key": self.api_key}
         response = await request(
             self.session, url, method=hdrs.METH_POST, data=data, headers=headers
         )
```

### Comparing `asyncpow-0.4.2/asyncpow/apis/movie.py` & `asyncpow-0.5.0/asyncpow/apis/movie.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,44 +27,50 @@
 
 
 class Movie:
     """
     Initialize the Movie object with the base URL and API key.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """
         Initialize the MovieAPI object with the base URL and API key.
 
         Args:
             base_url (str): The base URL for the media API.
             api_key (str): The API key for authentication.
             session (ClientSession): HTTP Session
+            raw_response (bool): Return json if True.
 
         Returns:
             None
         """
         self.media_url = base_url.joinpath("movie")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
 
     async def async_get_movie(
-        self, id: int, lang: str = "en", raw_response: bool = False
+        self, id: int, lang: str = "en", raw_response: bool | None = None
     ) -> dict | MovieDetailsModel:
         """
         Retrieves movie details by ID asynchronously.
 
         Args:
             id (int): The ID of the movie.
             lang (str): The language for the response (default is "en").
-            raw_response (bool): Flag to return raw response or MovieDetailsModel (default is False).
+            raw_response (bool, optional): return raw json. Defaults to None.
 
         Returns:
             dict | MovieDetailsModel: The raw response or MovieDetailsModel object based on the raw_response flag.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
 
         params = {"language": lang}
         url = self.media_url.joinpath(str(id))
 
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, params=params, headers=headers)
         return response if raw_response else MovieDetailsModel(**response)
```

### Comparing `asyncpow-0.4.2/asyncpow/apis/request.py` & `asyncpow-0.5.0/asyncpow/apis/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     """
 
     def __init__(
         self,
         base_url: URL,
         api_key: str,
         session: ClientSession,
+        raw_response: bool,
         tv_instance: Tv,
         movie_instance: Movie,
     ) -> None:
         """Initialize the RequestAPI object with the base URL, API key, and session.
 
         Args:
             base_url (str): The base URL for the media API.
@@ -59,39 +60,42 @@
 
         Returns:
             None
         """
         self.request_url = base_url.joinpath("request")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
         self.tv = tv_instance
         self.movie = movie_instance
 
     async def async_get_requests(
         self,
-        raw_response: bool = False,
+        raw_response: bool | None = None,
         take: int = 20,
         skip: int = 0,
         filter: RequestFilterOptions = "all",
         sort: SortOptions = "added",
         requested_by: int = 1,
     ) -> dict | RequestResultsResponseModel:
         """Get a list of requests
 
         Args:
-            raw_response (bool, optional): Return JSON response. Defaults to False.
+            raw_response (bool, optional): Return JSON response. Defaults to None.
             take (int, optional): Number if pages. Defaults to 20.
             skip (int, optional): Pages to skip. Defaults to 0.
             filter (RequestFilterOptions, optional): Filter requests. Defaults to "all".
             sort (SortOptions, optional): Sort Requests. Defaults to "added".
             requested_by (int, optional): Only requests by user. Defaults to 1.
 
         Returns:
             dict | RequestResultsResponseModel: Returns a request record
         """
+        if raw_response is None:
+            raw_response = self.raw_response
 
         url = self.request_url.with_query(
             {
                 "take": take,
                 "skip": skip,
                 "filter": filter,
                 "sort": sort,
@@ -103,54 +107,55 @@
         return response if raw_response else RequestResultsResponseModel(**response)
 
     async def async_post_request(
         self,
         id: int,
         type: Literal["movie", "tv"],
         series: Literal["all", "latest", "first"] = "all",
-        raw_response: bool = False,
+        raw_response: bool | None = None,
     ) -> dict | MediaRequestModel:
         """Get a list of requests
 
         Args:
             id (int): Movie or TV ID.
             type (str): Type of request movie | tv.
             series (str, optional): What series to request - all | latest | first, only aplies to tv. Defautls to all
-            raw_response (bool, optional): Return JSON response. Defaults to False.
+            raw_response (bool, optional): Return JSON response. Defaults to None.
 
         Returns:
             dict | MediaRequestModel: Returns a request record
         """
+        if raw_response is None:
+            raw_response = self.raw_response
 
         if type == "movie":
             req_data = {
                 "mediaType": "movie",
                 "mediaId": id,
             }
         elif type == "tv":
             data = await self.tv.async_get_tv(id=id)
-            if isinstance(data, TvDetailsModel):
-                if series == "all":
-                    seasons_array = [
-                        season.seasonNumber for season in data.seasons if season.seasonNumber != 0
-                    ]
-                elif series == "first":
-                    seasons_array = [1]
-
-                elif series == "latest":
-                    for season in data.seasons:
-                        seasons_array = [season.seasonNumber]
-                req_data = {
-                    "mediaType": "tv",
-                    "mediaId": id,
-                    "tvdbId": data.externalIds.tvdbId,
-                    "seasons": seasons_array,
-                }
-            else:
+            if not isinstance(data, TvDetailsModel):
                 raise POWException(f"Expecting TvDetailsModel, got {type(data)}")
+            if series == "all":
+                seasons_array = [
+                    season.seasonNumber for season in data.seasons if season.seasonNumber != 0
+                ]
+            elif series == "first":
+                seasons_array = [1]
+
+            elif series == "latest":
+                for season in data.seasons:
+                    seasons_array = [season.seasonNumber]
+            req_data = {
+                "mediaType": "tv",
+                "mediaId": id,
+                "tvdbId": data.externalIds.tvdbId,
+                "seasons": seasons_array,
+            }
         else:
             raise POWMediaTypeException("Unknown media type, use either movie or tv")
 
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         response = await request(
             self.session,
             self.request_url,
```

### Comparing `asyncpow-0.4.2/asyncpow/apis/search.py` & `asyncpow-0.5.0/asyncpow/apis/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,101 +29,115 @@
 class Search:
     """
     Class to interact with search-related endpoints.
 
     Initialize the Search object with the base URL, API key, and session.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """Initialize the SearchAPI object with the base URL, API key, and session.
 
         Args:
             base_url (str): The base URL for the media API.
             api_key (str): The API key for authentication.
-            session (ClientSession): HTTP Session
+            session (ClientSession): HTTP Session.
+            raw_response (bool): Return json if True.
 
         Returns:
             None
         """
         self.search_url = base_url.joinpath("search")
         self.api_key = api_key
         self.session = session
 
     async def async_get_search(
-        self, query: str, raw_response: bool = False, page: int = 1, lang: str = "en"
+        self, query: str, raw_response: bool | None = None, page: int = 1, lang: str = "en"
     ) -> dict | SearchResultModel:
         """Search for Movies, TV or Person
 
         Args:
             query (str):
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
             page (int): The page number for items (default is 1).
             lang (str): The language for items (default is "en").
 
         Returns:
             _type_: _description_
         """
+        if raw_response is None:
+            raw_response = self.raw_response
+
         url = self.search_url.with_query({"query": query, "page": page, "language": lang})
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, headers=headers)
         return response if raw_response else SearchResultModel(**response)
 
 
 class Discover:
     """
     Class to interact with discover-related endpoints.
 
     Initialize the Discover object with the base URL, API key, and session.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """Initialize the DiscoverAPI object with the base URL, API key, and session.
 
         Args:
             base_url (str): The base URL for the media API.
             api_key (str): The API key for authentication.
             session (ClientSession): HTTP Session
+            raw_response (bool): Return json if True.
 
         Returns:
             None
         """
         self.discover_url = base_url.joinpath("discover")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
 
     async def async_get_trending(
-        self, raw_response: bool = False, page: int = 1, lang: str = "en"
+        self, raw_response: bool | None = None, page: int = 1, lang: str = "en"
     ) -> dict | SearchResultModel:
         """
         Get trending items based on specified page and language.
 
         Args:
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
             page (int): The page number for trending items (default is 1).
             lang (str): The language for the trending items (default is "en").
 
         Returns:
             dict | SearchResultModel: The model object containing trending items.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
 
         url = self.discover_url.joinpath("trending").with_query({"page": page, "language": lang})
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, headers=headers)
         return response if raw_response else SearchResultModel(**response)
 
     async def async_get_watchlist(
-        self, raw_response: bool = False, page: int = 1
+        self, raw_response: bool | None = None, page: int = 1
     ) -> dict | DiscoverWatchlistModel:
         """
         Get the watchlist items based on the specified page.
 
         Args:
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
             page (int): The page number for watchlist items (default is 1).
 
         Returns:
             dict | DiscoverWatchlistModel: The model object containing watchlist items.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
         url = self.discover_url.joinpath("watchlist").with_query({"page": page})
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, headers=headers)
         return response if raw_response else DiscoverWatchlistModel(**response)
```

### Comparing `asyncpow-0.4.2/asyncpow/apis/status.py` & `asyncpow-0.5.0/asyncpow/apis/status.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,45 +30,63 @@
 class Status:
     """
     Class to interact with status-related endpoints.
 
     Initialize the Status object with the base URL, API key, and session.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """
         Initialize the Status object with the base URL, API key, and session.
 
+        Args:
+            base_url (str): The base URL for the user API.
+            api_key (str): The API key for authentication.
+            session (ClientSession): HTTP Session.
+            raw_response (bool): Return json if True.
+
         Returns:
             None
         """
 
         self.base_url = base_url.joinpath("status")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
 
-    async def async_get_status(self, raw_response: bool = False) -> dict | StatusModel:
+    async def async_get_status(
+        self,
+        raw_response: bool | None = None,
+    ) -> dict | StatusModel:
         """
         Summary:
             Asynchronously retrieves the status from the server.
 
         Args:
-            raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
 
         Returns:
             dict | StatusModel: The status information as either a dictionary or a StatusModel object.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
+
         response = await request(self.session, self.base_url)
         return response if raw_response else StatusModel(**response)
 
-    async def async_get_appdata(self, raw_response: bool = False) -> dict | StatusAppDataModel:
+    async def async_get_appdata(self, raw_response: bool = None) -> dict | StatusAppDataModel:
         """Retrieves the appdata from the server
 
         Args:
-            raw_response (bool, optional): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
+            raw_response (bool, optional): return raw json. Defaults to None.
 
         Returns:
             dict | StatusAppDataModel: The model object containing appdata items.
         """
+        if raw_response is None:
+            raw_response = self.raw_response
+
         url = self.base_url.joinpath("appdata")
         response = await request(self.session, url)
         return response if raw_response else StatusAppDataModel(**response)
```

### Comparing `asyncpow-0.4.2/asyncpow/apis/tv.py` & `asyncpow-0.5.0/asyncpow/apis/tv.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,46 +28,55 @@
 
 
 class Tv:
     """
     Initialize the Tv object with the base URL and API key.
     """
 
-    def __init__(self, base_url: URL, api_key: str, session: ClientSession) -> None:
+    def __init__(
+        self, base_url: URL, api_key: str, session: ClientSession, raw_response: bool
+    ) -> None:
         """
         Initialize the MovieAPI object with the base URL and API key.
 
         Args:
             base_url (str): The base URL for the media API.
             api_key (str): The API key for authentication.
-            session (ClientSession): HTTP Session
+            session (ClientSession): HTTP Session.
+            raw_response (bool): Return json if True.
 
         Returns:
             None
         """
         self.media_url = base_url.joinpath("tv")
         self.api_key = api_key
         self.session = session
+        self.raw_response = raw_response
 
     async def async_get_tv(
-        self, id: int, lang: str = "en", raw_response: bool = False
+        self,
+        id: int,
+        lang: str = "en",
+        raw_response: bool | None = None,
     ) -> dict | TvDetailsModel:
         """
         Retrieves TV details by ID asynchronously.
 
         Args:
             id (int): The ID of the TV show.
-            lang (str): The language for the response (default is "en").
-            raw_response (bool): Flag to return raw response or TvDetailsModel (default is False).
+            lang (str): The language for the response. Default to "en".
+            raw_response (bool): Flag to return Json. Defaults to None.
 
         Returns:
             dict | TvDetailsModel: The raw response or TvDetailsModel object based on the raw_response flag.
 
         Examples:
             tv_details = await async_get_tv(12345, lang="en", raw_response=False)
         """
+        if raw_response is None:
+            raw_response = self.raw_response
         params = {"language": lang}
         url = self.media_url.joinpath(str(id))
 
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, params=params, headers=headers)
         return response if raw_response else TvDetailsModel(**response)
```

### Comparing `asyncpow-0.4.2/asyncpow/const.py` & `asyncpow-0.5.0/asyncpow/const.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/exceptions.py` & `asyncpow-0.5.0/asyncpow/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/models/common.py` & `asyncpow-0.5.0/asyncpow/models/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,48 +21,18 @@
 
 
 from typing import Literal
 
 from pydantic import BaseModel
 
 SortOptions = Literal["added", "modified", "mediaAdded"]
+UserSortOptions = Literal["created"]
 MediaType = Literal["movie", "tv"]
 
 
-class UserModel(BaseModel):
-    """
-    Data class representing a user model.
-    """
-
-    displayName: str
-    id: int
-    email: str
-    username: str | None = None
-    password: str | None = None
-    resetPasswordGuid: str | None = None
-    recoveryLinkExpirationDate: str | None = None
-    userType: int
-    plexId: int | None = None
-    plexToken: str | None = None
-    plexUsername: str | None = None
-    permissions: int
-    avatar: str
-    createdAt: str
-    updatedAt: str
-    requestCount: int
-    requests: list | None = None  # TODO: Requests
-    movieQuotaLimit: int | None = None
-    movieQuotaDays: int | None = None
-    tvQuotaLimit: int | None = None
-    tvQuotaDays: int | None = None
-    settings: dict | None = None  # TODO: UserSettingsModel
-    pushSubscriptions: list | None = None  # TODO: UserPushSubscriptionModel
-    createdIssues: list | None = None  # TODO: IssueModel
-
-
 class PageInfoModel(BaseModel):
     """
     Data class representing page information.
 
     As per code
     """
```

### Comparing `asyncpow-0.4.2/asyncpow/models/media.py` & `asyncpow-0.5.0/asyncpow/models/media.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from typing import Literal
 
 from pydantic import BaseModel
 
-from asyncpow.models.common import MediaType, PaginatedResponseModel, SeasonModel, UserModel
+from asyncpow.models.common import MediaType, PaginatedResponseModel, SeasonModel
 
 MediaFilterOptions = Literal["all", "available", "partial", "allavailable", "pending", "processing"]
 
 MediaStatusOptions = Literal["available", "partial", "pending", "processing", "unknown"]
 
 
 class MediaRequestModel(BaseModel):
@@ -37,16 +37,16 @@
 
     As per code
     """
 
     id: int
     status: int  # 1 = PENDING APPROVAL, 2 = APPROVED, 3 = DECLINED
     media: "MediaInfoModel"
-    requestedBy: UserModel
-    modifiedBy: UserModel | None = None
+    requestedBy: dict  # TODO: should be user model, circular import
+    modifiedBy: dict | None = None  # TODO: should be user model, circular import
     createdAt: str
     updatedAt: str
     type: MediaType
     is4k: bool
     serverId: int | None = None
     profileId: int | None = None
     rootFolder: str | None = None
@@ -67,15 +67,15 @@
     tmdbId: int
     status: int  # 1 = UNKNOWN, 2 = PENDING, 3 = PROCESSING, 4 = PARTIALLY_AVAILABLE, 5 = AVAILABLE
     status4k: int
 
     createdAt: str
     updatedAt: str
     lastSeasonChange: str
-    issues: dict | None = None  # TODO: Add list of issues model
+    issues: dict | None = None  # TODO: should be issue model, circular import
     mediaAddedAt: str | None = None
     serviceId: int | None = None
     serviceId4k: int | None = None
     externalServiceId: int | None = None
     externalServiceId4k: int | None = None
     externalServiceSlug: str | None = None
     externalServiceSlug4k: str | None = None
@@ -109,15 +109,15 @@
 
 
 class MediaModel(PaginatedResponseModel):
     """
     Data class representing a media model.
     """
 
-    results: MediaInfoModel
+    results: list[MediaInfoModel]
 
 
 class MediaModel2(BaseModel):
     """
     Data class representing a secondary media model.
     """
```

### Comparing `asyncpow-0.4.2/asyncpow/models/movie.py` & `asyncpow-0.5.0/asyncpow/models/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/models/request.py` & `asyncpow-0.5.0/asyncpow/models/request.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/models/search.py` & `asyncpow-0.5.0/asyncpow/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 from asyncpow.exceptions import POWMediaTypeException
 from asyncpow.models.media import MediaInfoModel
 
 
 class MovieResultModel(BaseModel):
     """
@@ -80,15 +80,15 @@
     name: str
     popularity: float
     adult: bool
     mediaType: str
     knownFor: list[MovieResultModel | TvResultModel]
     profilePath: str | None = None
 
-    @validator("knownFor", pre=True)
+    @field_validator("knownFor")
     def validate_knownfor(cls, v):
         """
         Validate the 'knownFor' field by creating and returning a list of validated known for items.
 
         Args:
             v: The value to be validated.
 
@@ -120,15 +120,15 @@
     """
 
     page: int
     totalPages: int
     totalResults: int
     results: list[MovieResultModel | TvResultModel | PersonResultModel]
 
-    @validator("results", pre=True)
+    @field_validator("results")
     def validate_results(cls, v):
         """
         Validate the 'results' field by creating and returning a list of validated result items.
 
         Args:
             v: The value to be validated.
```

### Comparing `asyncpow-0.4.2/asyncpow/models/status.py` & `asyncpow-0.5.0/asyncpow/models/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/models/tv.py` & `asyncpow-0.5.0/asyncpow/models/tv.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/asyncpow/overseerr.py` & `asyncpow-0.5.0/asyncpow/overseerr.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 from asyncpow.apis.media import Media
 from asyncpow.apis.movie import Movie
 from asyncpow.apis.request import Request
 from asyncpow.apis.search import Discover, Search
 from asyncpow.apis.status import Status
 from asyncpow.apis.tv import Tv
+from asyncpow.apis.user import User
 from asyncpow.const import API_URI
+from asyncpow.utils.api_key import is_valid_api_key
 
 VERSION_CACHE: TTLCache[str, str | None] = TTLCache(maxsize=16, ttl=7200)
 
 
 class Overseerr:
     """The Overseerr class provides convenient access to Overseerr's API.
 
@@ -54,14 +56,21 @@
         ) as api:
             # Inside the context, you can use the API wrapper as needed
             status = await api.status.get_status()
             print("Status:", status)
 
     """
 
+    raw_response = False  # Default value for raw_response
+
+    @classmethod
+    def set_raw_response(cls, value: bool):
+        """Set the raw_response attribute globally."""
+        cls.raw_response = value
+
     def __init__(
         self,
         host: str,
         api_key: str,
         port: int | None = None,
         tls: bool = True,
         base_path: str = "",
@@ -82,26 +91,35 @@
         scheme = "https" if tls else "http"
         self.url = URL.build(
             scheme=scheme,
             host=host,
             port=port,
             path=base_path,
         ).joinpath(API_URI)
-        self.api_key = api_key
+        if not api_key:
+            raise ValueError("No API Key provided")
+
+        if is_valid_api_key(api_key):
+            self.api_key = api_key
+        else:
+            raise ValueError("API Key is not valid")
 
         # Initialize a single instance of ClientSession
         self._session = aiohttp.ClientSession()
         # Initialize instances of API classes
-        self.status = Status(self.url, self.api_key, self._session)
-        self.search = Search(self.url, self.api_key, self._session)
-        self.discover = Discover(self.url, self.api_key, self._session)
-        self.media = Media(self.url, self.api_key, self._session)
-        self.movie = Movie(self.url, self.api_key, self._session)
-        self.tv = Tv(self.url, self.api_key, self._session)
-        self.request = Request(self.url, self.api_key, self._session, self.tv, self.movie)
+        self.status = Status(self.url, self.api_key, self._session, self.raw_response)
+        self.search = Search(self.url, self.api_key, self._session, self.raw_response)
+        self.discover = Discover(self.url, self.api_key, self._session, self.raw_response)
+        self.media = Media(self.url, self.api_key, self._session, self.raw_response)
+        self.movie = Movie(self.url, self.api_key, self._session, self.raw_response)
+        self.tv = Tv(self.url, self.api_key, self._session, self.raw_response)
+        self.request = Request(
+            self.url, self.api_key, self._session, self.raw_response, self.tv, self.movie
+        )
+        self.user = User(self.url, self.api_key, self._session, self.raw_response)
 
     async def __aenter__(self):
         """
         Enter method for asynchronous context manager.
 
         Returns:
             self
```

### Comparing `asyncpow-0.4.2/asyncpow/utils/http.py` & `asyncpow-0.5.0/asyncpow/utils/http.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.2/pyproject.toml` & `asyncpow-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpow"
-version = "0.4.2"
+version = "0.5.0"
 description = "Asynchronous Python Overseerr Wrapper"
 authors = ["Steven Marks - TotalDebug"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/totaldebug/asyncpow"
 repository = "https://github.com/totaldebug/asyncpow"
 classifiers = [
```

### Comparing `asyncpow-0.4.2/PKG-INFO` & `asyncpow-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpow
-Version: 0.4.2
+Version: 0.5.0
 Summary: Asynchronous Python Overseerr Wrapper
 Home-page: https://github.com/totaldebug/asyncpow
 License: MIT
 Keywords: wled,api,async,client
 Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug
 Requires-Python: >=3.12,<4.0
@@ -87,15 +87,15 @@
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 This project is a work in progress, the main branch is being developed on live, which may cause breaking changes until the first full release.
 
 The library returns results in JSON format for ease of use, this also reduces the risk of failue when the APIs are updated.
 
-Type hints and type models are in place for all of the APIs, if you notice missing items please create a request to have it fixed.
+Type hints and type models are in place where possible (this API has terrible circular dependencies which breaks python), if you notice missing items please create a request to have it fixed.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Built With
 
 [![python][python]][python-url]
 
@@ -118,15 +118,19 @@
 * Discover - WIP
   * Trending - Completed
 * Media - WIP
   * Get - Completed
   * Update Status - Completed
   * Delete
   * Get Watch Data
-
+* User - WIP
+  * Get - Completed
+  * Bulk Update - Completed
+  * Update
+  * Delete
 
 ## Compatibility
 
 AsyncPOW is built for Python 3.12, and initially the v1 Overseerr API
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncpow Version: 0.4.2 Summary: Asynchronous
+Metadata-Version: 2.1 Name: asyncpow Version: 0.5.0 Summary: Asynchronous
 Python Overseerr Wrapper Home-page: https://github.com/totaldebug/asyncpow
 License: MIT Keywords: wled,api,async,client Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
@@ -36,26 +36,28 @@
    8. _L_i_c_e_n_s_e
    9. _C_o_n_t_a_c_t
   10. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About The Project This project is a work in progress, the main branch is
 being developed on live, which may cause breaking changes until the first full
 release. The library returns results in JSON format for ease of use, this also
 reduces the risk of failue when the APIs are updated. Type hints and type
-models are in place for all of the APIs, if you notice missing items please
-create a request to have it fixed.
+models are in place where possible (this API has terrible circular dependencies
+which breaks python), if you notice missing items please create a request to
+have it fixed.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With [![python][python]][python-url]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started * [QuickStart Guide](https://docs.totaldebug.uk/asyncpow/
 quickstart.html) * [Full Documentation](https://docs.totaldebug.uk/asyncpow) *
 [Release Notes](https://github.com/totaldebug/asyncpow/releases)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Features * Asynchronous * Type Checking * Status - Completed * Discover -
 WIP * Trending - Completed * Media - WIP * Get - Completed * Update Status -
-Completed * Delete * Get Watch Data ## Compatibility AsyncPOW is built for
+Completed * Delete * Get Watch Data * User - WIP * Get - Completed * Bulk
+Update - Completed * Update * Delete ## Compatibility AsyncPOW is built for
 Python 3.12, and initially the v1 Overseerr API
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Roadmap See the [feature requests](https://github.com/totaldebug/asyncpow/
 labels/type%2Ffeature) for a full list of requested features.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Sponsor My projects arent possible without the support of the community,
 please consider donating a small amount to keep these projects alive. [!
```

