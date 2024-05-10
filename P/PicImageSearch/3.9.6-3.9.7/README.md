# Comparing `tmp/picimagesearch-3.9.6.tar.gz` & `tmp/picimagesearch-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picimagesearch-3.9.6.tar", max compression
+gzip compressed data, was "picimagesearch-3.9.7.tar", max compression
```

## Comparing `picimagesearch-3.9.6.tar` & `picimagesearch-3.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/LICENSE
--rw-r--r--   0        0        0      251 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/__init__.py
--rw-r--r--   0        0        0     3331 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/ascii2d.py
--rw-r--r--   0        0        0     2108 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/baidu.py
--rw-r--r--   0        0        0     2817 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/ehentai.py
--rw-r--r--   0        0        0     3476 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/google.py
--rw-r--r--   0        0        0     2038 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/iqdb.py
--rw-r--r--   0        0        0      397 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/__init__.py
--rw-r--r--   0        0        0     5465 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/ascii2d.py
--rw-r--r--   0        0        0     1622 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/baidu.py
--rw-r--r--   0        0        0     3103 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/ehentai.py
--rw-r--r--   0        0        0     3697 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/google.py
--rw-r--r--   0        0        0     6739 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/iqdb.py
--rw-r--r--   0        0        0     9180 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/saucenao.py
--rw-r--r--   0        0        0     6683 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/tracemoe.py
--rw-r--r--   0        0        0     2480 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/model/yandex.py
--rw-r--r--   0        0        0     9154 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/network.py
--rw-r--r--   0        0        0     3956 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/saucenao.py
--rw-r--r--   0        0        0     2296 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/sync.py
--rw-r--r--   0        0        0     6308 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/tracemoe.py
--rw-r--r--   0        0        0     1834 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/PicImageSearch/yandex.py
--rw-r--r--   0        0        0     2223 2023-11-13 13:20:47.195318 picimagesearch-3.9.6/README.md
--rw-r--r--   0        0        0     1288 2023-11-13 13:20:47.199318 picimagesearch-3.9.6/pyproject.toml
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 picimagesearch-3.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/LICENSE
+-rw-r--r--   0        0        0      251 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/__init__.py
+-rw-r--r--   0        0        0     2372 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/ascii2d.py
+-rw-r--r--   0        0        0     2167 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/baidu.py
+-rw-r--r--   0        0        0     2862 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/ehentai.py
+-rw-r--r--   0        0        0     3709 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/google.py
+-rw-r--r--   0        0        0     2109 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/iqdb.py
+-rw-r--r--   0        0        0      397 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/__init__.py
+-rw-r--r--   0        0        0     5727 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/ascii2d.py
+-rw-r--r--   0        0        0     1589 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/baidu.py
+-rw-r--r--   0        0        0     3175 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/ehentai.py
+-rw-r--r--   0        0        0     3836 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/google.py
+-rw-r--r--   0        0        0     6566 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/iqdb.py
+-rw-r--r--   0        0        0     8320 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/saucenao.py
+-rw-r--r--   0        0        0     5405 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/tracemoe.py
+-rw-r--r--   0        0        0     2463 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/model/yandex.py
+-rw-r--r--   0        0        0     8534 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/network.py
+-rw-r--r--   0        0        0     3884 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/saucenao.py
+-rw-r--r--   0        0        0     2269 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/sync.py
+-rw-r--r--   0        0        0     6271 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/tracemoe.py
+-rw-r--r--   0        0        0     1789 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/PicImageSearch/yandex.py
+-rw-r--r--   0        0        0     2220 2023-12-12 13:02:08.591548 picimagesearch-3.9.7/README.md
+-rw-r--r--   0        0        0     1334 2023-12-12 13:02:08.595548 picimagesearch-3.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 picimagesearch-3.9.7/PKG-INFO
```

### Comparing `picimagesearch-3.9.6/LICENSE` & `picimagesearch-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.6/PicImageSearch/baidu.py` & `picimagesearch-3.9.7/PicImageSearch/baidu.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,56 +6,60 @@
 from .model import BaiDuResponse
 from .network import HandOver
 
 
 class BaiDu(HandOver):
     """API client for the BaiDu image search engine.
 
-    Attributes:
-        url: The URL endpoint for the BaiDu API.
-        params: Query parameters for the BaiDu API.
+    Used for performing reverse image searches using BaiDu service.
     """
 
     def __init__(self, **request_kwargs: Any):
-        """Initializes BaiDu API client with configuration.
+        """Initializes a BaiDu API client with specified configurations.
 
         Args:
-            **request_kwargs: Additional keyword arguments for request configuration.
+            **request_kwargs: Additional arguments for network requests.
         """
         super().__init__(**request_kwargs)
 
     async def search(
         self, url: Optional[str] = None, file: Union[str, bytes, Path, None] = None
     ) -> BaiDuResponse:
-        """Performs a reverse image search on BaiDu using the URL or file of the image.
+        """Performs a reverse image search on BaiDu.
 
-        The user must provide either a URL or a file.
+        Supports searching by image URL or by uploading an image file.
+
+        Requires either 'url' or 'file' to be provided.
 
         Args:
             url: URL of the image to search.
-            file: Image file to search. Can be a file path (str or Path) or raw bytes.
+            file: Local image file (path or bytes) to search.
 
         Returns:
-            An instance of BaiDuResponse containing the search results and additional metadata.
+            BaiDuResponse: Contains search results and additional information.
 
         Raises:
-            ValueError: If neither `url` nor `file` is provided.
+            ValueError: If neither 'url' nor 'file' is provided.
+
+        Note:
+            The search process involves multiple HTTP requests to BaiDu's API.
         """
         params = {"from": "pc"}
         files: Optional[Dict[str, Any]] = None
         if url:
             params["image"] = url
         elif file:
             files = (
                 {"image": file}
                 if isinstance(file, bytes)
                 else {"image": open(file, "rb")}
             )
         else:
-            raise ValueError("url or file is required")
+            raise ValueError("Either 'url' or 'file' must be provided")
+
         resp = await self.post(
             "https://graph.baidu.com/upload", params=params, files=files
         )
         next_url = (json_loads(resp.text))["data"]["url"]
         resp = await self.get(next_url)
         final_url = resp.url
         next_url = (re.search(r'"firstUrl":"([^"]+)"', resp.text)[1]).replace(r"\/", "/")  # type: ignore
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/ehentai.py` & `picimagesearch-3.9.7/PicImageSearch/ehentai.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,77 +4,80 @@
 from .model import EHentaiResponse
 from .network import HandOver
 
 
 class EHentai(HandOver):
     """API client for the EHentai image search engine.
 
+    Used for performing reverse image searches using EHentai service.
+
     Attributes:
-        url: The URL endpoint for the EHentai API.
-        params: Query parameters for the EHentai API.
+        covers: A flag to search only for covers.
+        similar: A flag to enable similarity scanning.
+        exp: A flag to include results from expunged galleries.
     """
 
     def __init__(
         self,
         covers: bool = False,
         similar: bool = True,
         exp: bool = False,
         **request_kwargs: Any
     ):
-        """Initializes EHentai API client with configuration.
+        """Initializes an EHentai API client with specified configurations.
 
         Args:
-            covers: Whether to only search for covers.
-            similar: Whether to use similarity scan to find similar images.
-            exp: Whether to include results from the expunged galleries.
-            **request_kwargs: Additional keyword arguments for request configuration.
+            covers: If True, search only for covers; otherwise, False.
+            similar: If True, enable similarity scanning; otherwise, False.
+            exp: If True, include results from expunged galleries; otherwise, False.
+            **request_kwargs: Additional arguments for network requests.
         """
-
         super().__init__(**request_kwargs)
         self.covers: bool = covers
         self.similar: bool = similar
         self.exp: bool = exp
 
     async def search(
         self,
         url: Optional[str] = None,
         file: Union[str, bytes, Path, None] = None,
         ex: bool = False,
     ) -> EHentaiResponse:
-        """Performs a reverse image search on EHentai using the URL or file of the image.
+        """Performs a reverse image search on EHentai.
 
-        The user must provide either a URL or a file.
+        Supports searching by image URL or by uploading an image file.
 
-        Note:
-            To use `ex` you must be logged in to exhentai.org via the cookies defined in `EHentai.request_kwargs`.
-            We recommend using `ex=bool(cookies)` or something similar to determine whether to use `ex`.
+        Requires either 'url' or 'file' to be provided.
 
         Args:
             url: URL of the image to search.
-            file: Image file to search. Can be a file path (str or Path) or raw bytes.
-            ex: Whether to search on exhentai.org instead of e-hentai.org. Defaults to False.
+            file: Local image file (path or bytes) to search.
+            ex: If True, search on exhentai.org; otherwise, use e-hentai.org.
 
         Returns:
-            An instance of EHentaiResponse containing the search results and additional metadata.
+            EHentaiResponse: Contains search results and additional information.
 
         Raises:
-            ValueError: If neither `url` nor `file` is provided.
+            ValueError: If neither 'url' nor 'file' is provided.
+
+        Note:
+            Searching on exhentai.org requires logged-in status via cookies in `EHentai.request_kwargs`.
         """
         _url: str = (
             "https://exhentai.org/upld/image_lookup.php"
             if ex
             else "https://upld.e-hentai.org/image_lookup.php"
         )
         data: Dict[str, Any] = {"f_sfile": "search"}
         if url:
             files: Dict[str, Any] = {"sfile": await self.download(url)}
         elif file:
             files = {"sfile": file if isinstance(file, bytes) else open(file, "rb")}
         else:
-            raise ValueError("url or file is required")
+            raise ValueError("Either 'url' or 'file' must be provided")
         if self.covers:
             data["fs_covers"] = "on"
         if self.similar:
             data["fs_similar"] = "on"
         if self.exp:
             data["fs_exp"] = "on"
         resp = await self.post(url=_url, data=data, files=files)
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/google.py` & `picimagesearch-3.9.7/PicImageSearch/google.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,96 +4,100 @@
 from .model import GoogleResponse
 from .network import HandOver
 
 
 class Google(HandOver):
     """API client for the Google image search engine.
 
+    Used for performing reverse image searches using Google service.
+
     Attributes:
-        url: The URL endpoint for the Google API.
-        params: Query parameters for the Google API.
+         base_url: The base URL for Google searches, configurable for different regions.
+            Example: `https://www.google.co.jp/searchbyimage` for searches in Japan.
     """
 
-    def __init__(self, **request_kwargs: Any):
-        """Initializes Google API client with configuration.
+    def __init__(
+        self,
+        base_url: str = "https://www.google.com/searchbyimage",
+        **request_kwargs: Any,
+    ):
+        """Initializes a Google API client with specified configurations.
 
         Args:
-            **request_kwargs: Additional keyword arguments for request configuration.
+            base_url: The base URL for Google searcher, defaults to the international version.
+            **request_kwargs: Additional arguments for network requests.
         """
         super().__init__(**request_kwargs)
-        self.url = "https://www.google.com/searchbyimage"
+        self.base_url = base_url
 
     async def _navigate_page(
         self, resp: GoogleResponse, offset: int
     ) -> Optional[GoogleResponse]:
-        """Navigate to the next or previous page of the search results.
+        """Navigates to a specific page in search results based on the given offset.
 
         Args:
-            resp: The response from the previous search.
-            offset: The offset to navigate to. Negative values navigate backwards.
+            resp: The current GoogleResponse instance.
+            offset: Integer for page navigation, positive for forward and negative for backward.
 
         Returns:
-            An instance of GoogleResponse containing the search results and additional metadata.
-            Or None if the offset is out of bounds.
+            GoogleResponse: Updated response after navigating to the specified page, or None if out of range.
         """
-
         index = resp.pages.index(resp.url)
         new_index = index + offset
         if new_index < 0 or new_index >= len(resp.pages):
             return None
         _resp = await self.get(resp.pages[new_index])
         return GoogleResponse(_resp.text, _resp.url)
 
     async def pre_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
-        """Navigate to the previous page of the search results.
+        """Navigates to the previous page in Google search results.
 
         Args:
-            resp: The response from the previous search.
+            resp: The current GoogleResponse instance.
 
         Returns:
-            An instance of GoogleResponse containing the search results and additional metadata.
-            Or None if there is no previous page.
+            GoogleResponse: Updated response after navigating to the previous page, or None if out of range.
         """
-
         return await self._navigate_page(resp, -1)
 
     async def next_page(self, resp: GoogleResponse) -> Optional[GoogleResponse]:
-        """Navigate to the next page of the search results.
+        """Navigates to the next page in Google search results.
 
         Args:
-            resp: The response from the previous search.
+            resp: The current GoogleResponse instance.
 
         Returns:
-            An instance of GoogleResponse containing the search results and additional metadata.
-            Or None if there is no next page.
+            GoogleResponse: Updated response after navigating to the next page, or None if out of range.
         """
         return await self._navigate_page(resp, 1)
 
     async def search(
         self, url: Optional[str] = None, file: Union[str, bytes, Path, None] = None
     ) -> GoogleResponse:
-        """Performs a reverse image search on Google using the URL or file of the image.
+        """Performs a reverse image search on Google.
+
+        Supports searching by image URL or by uploading an image file.
 
-        The user must provide either a URL or a file.
+        Requires either 'url' or 'file' to be provided.
 
         Args:
             url: URL of the image to search.
-            file: Image file to search. Can be a file path (str or Path) or raw bytes.
+            file: Local image file (path or bytes) to search.
 
         Returns:
-            An instance of GoogleResponse containing the search results and additional metadata.
+            GoogleResponse: Contains search results and additional information.
 
         Raises:
-            ValueError: If neither `url` nor `file` is provided.
+            ValueError: If neither 'url' nor 'file' is provided.
         """
         params: Dict[str, Any] = {"sbisrc": 1}
         if url:
             params["image_url"] = url
-            resp = await self.get(self.url, params=params)
+            resp = await self.get(self.base_url, params=params)
         elif file:
             files = {
                 "encoded_image": file if isinstance(file, bytes) else open(file, "rb")
             }
-            resp = await self.post(f"{self.url}/upload", data=params, files=files)
+            resp = await self.post(f"{self.base_url}/upload", data=params, files=files)
         else:
-            raise ValueError("url or file is required")
+            raise ValueError("Either 'url' or 'file' must be provided")
         return GoogleResponse(resp.text, resp.url)
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/iqdb.py` & `picimagesearch-3.9.7/PicImageSearch/iqdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,56 +4,59 @@
 from .model import IqdbResponse
 from .network import HandOver
 
 
 class Iqdb(HandOver):
     """API client for the Iqdb image search engine.
 
-    Attributes:
-        url: The URL endpoint for the Iqdb API.
-        params: Query parameters for the Iqdb API.
+    Used for performing reverse image searches using Iqdb service.
     """
 
     def __init__(self, **request_kwargs: Any):
-        """Initializes Iqdb API client with configuration.
+        """Initializes an Iqdb API client with request configuration.
 
         Args:
-            **request_kwargs: Additional keyword arguments for request configuration.
+            **request_kwargs: Additional arguments for network requests.
         """
         super().__init__(**request_kwargs)
 
     async def search(
         self,
         url: Optional[str] = None,
         file: Union[str, bytes, Path, None] = None,
         force_gray: bool = False,
         is_3d: bool = False,
     ) -> IqdbResponse:
-        """Performs a reverse image search on Iqdb using the URL or file of the image.
+        """Performs a reverse image search on Iqdb.
 
-        The user must provide either a URL or a file.
+        Supports searching by image URL or by uploading an image file.
+
+        Requires either 'url' or 'file' to be provided.
 
         Args:
             url: URL of the image to search.
-            file: Image file to search. Can be a file path (str or Path) or raw bytes.
-            force_gray: Whether to ignore color.
-            is_3d: Whether to search for irl images on none anime related sites. This uses the 3d.iqdb.org endpoint.
+            file: Local image file (path or bytes) to search.
+            force_gray: If True, ignores color information in the image.
+            is_3d: If True, searches on 3d.iqdb.org for real-life images; otherwise, iqdb.org for anime images.
 
         Returns:
-            An instance of IqdbResponse containing the search results and additional metadata.
+            IqdbResponse: Contains search results and additional information.
 
         Raises:
-            ValueError: If neither `url` nor `file` is provided.
+            ValueError: If neither 'url' nor 'file' is provided.
+
+        Note:
+            Search can be tailored for anime or real-life images using `is_3d` parameter.
         """
         iqdb_url = "https://3d.iqdb.org/" if is_3d else "https://iqdb.org/"
         data: Dict[str, Any] = {}
-        if force_gray:  # 忽略颜色
+        if force_gray:
             data["forcegray"] = "on"
         if url:
             data["url"] = url
             resp = await self.post(iqdb_url, data=data)
         elif file:
             files = {"file": file if isinstance(file, bytes) else open(file, "rb")}
             resp = await self.post(iqdb_url, data=data, files=files)
         else:
-            raise ValueError("url or file is required")
+            raise ValueError("Either 'url' or 'file' must be provided")
         return IqdbResponse(resp.text)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/ascii2d.py` & `picimagesearch-3.9.7/PicImageSearch/model/ascii2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,96 +6,96 @@
 
 BASE_URL = "https://ascii2d.net"
 SUPPORTED_SOURCES = ["pixiv", "twitter", "fanbox", "fantia", "ニコニコ静画", "ニジエ"]
 URL = namedtuple("URL", ["href", "text"])
 
 
 class Ascii2DItem:
-    """
-    A single Ascii2D search result item.
-
-    This class encapsulates the details of a single result from an Ascii2D reverse image search.
+    """Represents a single Ascii2D search result item.
 
-    Args:
-        data: The raw data from the search result.
+    Holds details of a result from an Ascii2D reverse image search.
 
     Attributes:
-        origin: The original raw data from the search result.
-        hash: The hash string extracted from the search result.
-        detail: Detailed information such as image dimensions, type, and size.
+        origin: The raw data of the search result item.
+        hash: The hash string from the search result.
+        detail: Image details like dimensions, type, and size.
         thumbnail: URL of the thumbnail image.
-        url: Direct URL of the image source.
-        url_list (List[URL]): List of URLs and their text descriptions.
+        url: URL of the webpage with the image.
+        url_list: List of URLs with text descriptions.
         title: Title of the image or related content.
         author: Author of the image or related content.
         author_url: URL to the author's page or profile.
     """
 
     def __init__(self, data: PyQuery):
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        # 原图长宽，类型，大小 (original image width, height, type, size)
+        """Initializes an Ascii2DItem with data from a search result.
+
+        Args:
+            data: A PyQuery instance containing the search result item's data.
+        """
+        self.origin: PyQuery = data
         self.hash: str = data("div.hash").eq(0).text()
         self.detail: str = data("small").eq(0).text()
         self.thumbnail: str = BASE_URL + data("img").eq(0).attr("src")
         self.url: str = ""
         self.url_list: List[URL] = []
         self.title: str = ""
         self.author: str = ""
         self.author_url: str = ""
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
-        """
-        Organize search result data.
+        """Organize search result data.
 
         Extracts and sets the URL list, title, author, and author URL from the provided data.
 
+        Also normalizes the URL list and sets backup links if necessary.
+
         Args:
-            data: A PyQuery instance containing the search result data.
+            data: A PyQuery instance containing the search result item's data.
         """
         if infos := data.find("div.detail-box.gray-link"):
             links = infos.find("a")
             self.url_list = (
                 [URL(i.attr("href"), i.text()) for i in links.items()] if links else []
             )
             mark = infos("small").eq(-1).text() if links else ""
             self._arrange_links(infos, links, mark)
             self._arrange_title(infos)
         self._normalize_url_list()
         if not self.url_list:
             self._arrange_backup_links(data)
 
     def _arrange_links(self, infos: PyQuery, links: PyQuery, mark: str) -> None:
-        """
-        Extract and set the title for the search result item.
+        """Extract and set the primary and author URLs, along with the title and author name for the search result item.
 
         Args:
-            infos: PyQuery object that may contain the title text.
+            infos: A PyQuery instance containing additional information about the search result.
+            links: A PyQuery instance containing the URL links.
+            mark: A string identifier used to determine the source of the link.
         """
         if links:
             link_items = list(links.items())
             if len(link_items) > 1 and mark in SUPPORTED_SOURCES:
                 self.title, self.url = link_items[0].text(), link_items[0].attr("href")
                 self.author_url, self.author = (
                     link_items[1].attr("href"),
                     link_items[1].text(),
                 )
             elif links.eq(0).parents("small"):
                 infos.remove("small")
                 self.title = infos.text()
 
     def _arrange_title(self, infos: PyQuery) -> None:
-        """
-        Extract text from external link containers.
+        """Extract and refine the title of the search result.
 
-        Args:
-            infos: PyQuery object to extract external text from.
+        The method removes certain predefined keywords from the title if they are present.
 
-        Returns:
-            A string containing the extracted text.
+        Args:
+            infos: A PyQuery instance to extract the title from.
         """
         if not self.title:
             self.title = self._extract_external_text(infos) or infos.find("h6").text()
         if self.title and any(i in self.title for i in {"詳細掲示板のログ", "2ちゃんねるのログ"}):
             self.title = ""
 
     @staticmethod
@@ -108,39 +108,42 @@
         """Normalize the URL list to absolute paths."""
         self.url_list = [
             URL(BASE_URL + url.href, url.text) if url.href.startswith("/") else url
             for url in self.url_list
         ]
 
     def _arrange_backup_links(self, data: PyQuery) -> None:
-        """
-        Set backup links if the main URL list is empty.
+        """Set backup links if the main URL list is empty.
 
         Args:
-            data: PyQuery object to search for backup links.
+            data: A PyQuery instance to search for backup links.
         """
         if links := data.find("div.pull-xs-right > a"):
             self.url = links.eq(0).attr("href")
             self.url_list = [URL(self.url, links.eq(0).text())]
 
 
 class Ascii2DResponse:
-    """
-    Ascii2D reverse image search response.
+    """Encapsulates an Ascii2D reverse image search response.
 
-    This class encapsulates the entire response from an Ascii2D reverse image search operation.
+    Contains the complete response from an Ascii2D reverse image search operation.
 
     Attributes:
-        origin (PyQuery): The original raw data from the response.
-        raw (List[Ascii2DItem]): A list of Ascii2DItem instances representing each search result.
-        url (str): The URL of the response or the search query.
+        origin: The raw response data.
+        raw: List of Ascii2DItem instances for each search result.
+        url: URL to the search result page.
     """
 
     def __init__(self, resp_text: str, resp_url: str):
+        """Initializes with the response text and URL.
+
+        Args:
+            resp_text: The text of the response.
+            resp_url: URL to the search result page.
+        """
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        # 结果返回值 (result returned from source)
+        self.origin: PyQuery = data
         self.raw: List[Ascii2DItem] = [
             Ascii2DItem(i) for i in data.find("div.row.item-box").items()
         ]
         self.url: str = resp_url
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/baidu.py` & `picimagesearch-3.9.7/PicImageSearch/model/baidu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from typing import Any, Dict, List
 
 
 class BaiDuItem:
-    """A single BaiDu search result.
+    """Represents a single BaiDu search result item.
+
+    Holds details of a result from a BaiDu reverse image search.
 
     Attributes:
-        origin: The raw data of the item.
-        thumbnail: URL to the thumbnail image.
-        url: URL to the web page where the image is located.
+        origin: The raw data of the search result item.
+        thumbnail: URL of the thumbnail image.
+        url: URL of the webpage with the image.
     """
 
     def __init__(self, data: Dict[str, Any]):
-        """Initializes with data from a search result.
+        """Initializes with data from a BaiDu search result.
 
         Args:
-            data: Data for the item.
+            data: A dictionary containing the search result data.
         """
-        self.origin: Dict[str, Any] = data  # 原始数据
-        # self.similarity: float = round(float(data["simi"]) * 100, 2)  # deprecated
-        # self.title: str = data["fromPageTitle"]  # 页面标题 deprecated
-        self.thumbnail: str = data["thumbUrl"]  # 图片地址 (thumbnail)
-        self.url: str = data["fromUrl"]  # 图片所在网页地址 (image url)
+        self.origin: Dict[str, Any] = data
+        # deprecated attributes
+        # self.similarity: float = round(float(data["simi"]) * 100, 2)
+        # self.title: str = data["fromPageTitle"]
+        self.thumbnail: str = data["thumbUrl"]
+        self.url: str = data["fromUrl"]
 
 
 class BaiDuResponse:
-    """The response from a BaiDu image search.
+    """Encapsulates a BaiDu reverse image search response.
+
+    Contains the complete response from a BaiDu reverse image search operation.
 
     Attributes:
-        url: URL to the BaiDu search result page.
         origin: The raw response data.
         raw: List of BaiDuItem instances for each search result.
+        url: URL to the search result page.
     """
 
     def __init__(self, resp_json: Dict[str, Any], resp_url: str):
-        """Initializes with the JSON response and result URL.
+        """Initializes with the JSON response and response URL.
 
         Args:
-            resp_json: The response JSON from BaiDu.
-            resp_url: URL of the search result page.
+            resp_json: The response JSON.
+            resp_url: URL to the search result page.
         """
-        self.url: str = resp_url  # 搜索结果地址 (link to search result)
-        self.origin: Dict[str, Any] = resp_json  # 原始数据 (raw data)
-        # 来源结果返回值 (results returned from source)
+        self.origin: Dict[str, Any] = resp_json
         self.raw: List[BaiDuItem] = [BaiDuItem(i) for i in resp_json["data"]["list"]]
+        self.url: str = resp_url
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/ehentai.py` & `picimagesearch-3.9.7/PicImageSearch/model/ehentai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from typing import List
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
 
 class EHentaiItem:
-    """A single e-hentai gallery item.
+    """Represents a single e-hentai gallery item.
+
+    Holds details of a gallery from an e-hentai reverse image search.
 
     Attributes:
-        origin: The raw data of the item.
-        title: The title of the gallery.
-        url: The URL of the gallery.
-        thumbnail: The URL to the thumbnail of the gallery.
-        type: The type or category of the gallery.
-        date: The date when the gallery was posted.
-        tags: A list of tags associated with the gallery.
+        origin: The raw data of the search result item.
+        thumbnail: URL of the gallery's thumbnail.
+        url: URL of the gallery.
+        title: Title of the gallery.
+        type: Category of the gallery.
+        date: Date when the gallery was posted.
+        tags: List of tags associated with the gallery.
     """
 
     def __init__(self, data: PyQuery):
-        """Initializes an EHentaiItem with parsed data from a page element.
+        """Initializes an EHentaiItem with data from a search result.
 
         Args:
-            data: A PyQuery object containing data of the gallery item.
+            data: A PyQuery instance containing the search result item's data.
         """
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        self.title: str = ""
-        self.url: str = ""
+        self.origin: PyQuery = data
         self.thumbnail: str = ""
+        self.url: str = ""
+        self.title: str = ""
         self.type: str = ""
         self.date: str = ""
         self.tags: List[str] = []
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
-        """Arranges data from a PyQuery object into attributes of the gallery item.
+        """Organize gallery data.
+
+        Extracts and sets the gallery's title, URL, thumbnail, type, date and tags.
 
         Args:
-            data: A PyQuery object containing data of the gallery item.
+            data: A PyQuery instance containing the gallery's data.
         """
         glink = data.find(".glink")
         self.title = glink.text()
         if glink.parent("div"):
             self.url = glink.parent("div").parent("a").attr("href")
         else:
             self.url = glink.parent("a").attr("href")
@@ -55,32 +59,34 @@
         self.date = data.find("[id^='posted']").eq(0).text()
         self.tags = [
             i.text() for i in data.find("div[class=gt],div[class=gtl]").items()
         ]
 
 
 class EHentaiResponse:
-    """The response from an e-hentai gallery search.
+    """Encapsulates an e-hentai reverse image search response.
+
+    Contains the complete response from an e-hentai reverse image search operation.
 
     Attributes:
-        origin: The raw data of the response.
-        raw: A list of EHentaiItem instances representing gallery items.
-        url: The URL to the e-hentai search result page.
+        origin: The raw response data.
+        raw: List of EHentaiItem instances for each gallery item.
+        url: URL to the search result page.
     """
 
     def __init__(self, resp_text: str, resp_url: str):
-        """Initializes an EHentaiResponse with the text response and result URL.
+        """Initializes with the response text and URL.
 
         Args:
-            resp_text: The text of the HTTP response.
-            resp_url: The URL of the search result page.
+            resp_text: The text of the response.
+            resp_url: URL to the search result page.
         """
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
-        self.origin: PyQuery = data  # 原始数据 (raw data)
+        self.origin: PyQuery = data
         if "No unfiltered results found." in resp_text:
             self.raw = []
         elif tr_items := data.find(".itg").children("tr").items():
             self.raw = [EHentaiItem(i) for i in tr_items if i.children("td")]
         else:
             gl1t_items = data.find(".itg").children(".gl1t").items()
             self.raw = [EHentaiItem(i) for i in gl1t_items]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/google.py` & `picimagesearch-3.9.7/PicImageSearch/model/google.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 from typing import Dict, List, Optional
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
 
 class GoogleItem:
-    """A single Google search result item.
+    """Represents a single Google search result item.
+
+    Holds details of a result from a Google reverse image search.
 
     Attributes:
-        origin: The raw data of the item.
-        title: The title of the search result.
-        url: The URL of the search result.
-        thumbnail: The optional base64 encoded thumbnail image.
+        origin: The raw data of the search result item.
+        title: Title of the search result.
+        url: URL to the search result.
+        thumbnail: Optional base64 encoded thumbnail image.
     """
 
     def __init__(self, data: PyQuery, thumbnail: Optional[str]):
-        """Initializes a GoogleItem instance.
+        """Initializes a GoogleItem with data from a search result.
 
         Args:
-            data: The PyQuery object containing the item's data.
-            thumbnail: An optional base64 encoded thumbnail image.
+            data: A PyQuery instance containing the search result item's data.
+            thumbnail: Optional base64 encoded thumbnail image.
         """
-        self.origin: PyQuery = data  # 原始数据 (raw data)
+        self.origin: PyQuery = data
         self.title: str = data("h3").text()
         self.url: str = data("a").eq(0).attr("href")
         self.thumbnail: Optional[str] = thumbnail
 
 
 class GoogleResponse:
-    """The response from a Google search query.
+    """Encapsulates a Google reverse image search response.
+
+    Contains the complete response from a Google reverse image search operation.
 
     Attributes:
-        origin: The raw data of the response.
+        origin: The raw response data.
         page_number: The current page number in the search results.
-        url: The URL to the Google search result page.
-        pages: A list of URLs to the pages of search results.
-        raw: A list of GoogleItem instances representing individual search results.
+        url: URL to the search result page.
+        pages: List of URLs to pages of search results.
+        raw: List of GoogleItem instances for each search result.
     """
 
     def __init__(self, resp_text: str, resp_url: str):
-        """Initializes a GoogleResponse instance.
+        """Initializes with the response text and URL.
 
         Args:
-            resp_text: The response text containing the HTML of the search results.
-            resp_url: The URL from which the response was obtained.
+            resp_text: The text of the response.
+            resp_url: URL to the search result page.
         """
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        self.page_number: int = 1  # 当前页 (current page)
+        self.origin: PyQuery = data
+        self.page_number: int = 1
         self.url: str = resp_url
         index = 1
         for i, item in enumerate(
             list(data.find('div[role="navigation"] td').items())[1:-1]
         ):
             if not PyQuery(item).find("a"):
                 index = i + 1
@@ -61,25 +65,26 @@
                 break
         self.pages: List[str] = [
             f'https://www.google.com{i.attr("href")}'
             for i in data.find('a[aria-label~="Page"]').items()
         ]
         self.pages.insert(index - 1, resp_url)
         script_list = list(data.find("script").items())
-        # 结果返回值 (result returned from source)
         thumbnail_dict: Dict[str, str] = self.create_thumbnail_dict(script_list)
         self.raw: List[GoogleItem] = [
             GoogleItem(i, thumbnail_dict.get(i('img[id^="dimg_"]').attr("id")))
             for i in data.find("#search .g").items()
         ]
 
     @staticmethod
     def create_thumbnail_dict(script_list: List[PyQuery]) -> Dict[str, str]:
         """Extracts a dictionary of thumbnail images from the list of script tags.
 
+        Parses script tags to extract a mapping of image IDs to their base64 encoded thumbnails.
+
         Args:
             script_list: A list of PyQuery objects each containing a script element.
 
         Returns:
             A dictionary where keys are image IDs and values are base64 encoded images.
         """
         thumbnail_dict = {}
@@ -87,14 +92,15 @@
         id_regex = compile(r"dimg_\d+")
 
         for script in script_list:
             base_64_match = base_64_regex.findall(script.text())
             if not base_64_match:
                 continue
 
+            # extract and adjust base64 encoded thumbnails
             base64: str = base_64_match[0]
             id_list: List[str] = id_regex.findall(script.text())
 
             for _id in id_list:
                 thumbnail_dict[_id] = base64.replace(r"\x3d", "=")
 
         return thumbnail_dict
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/iqdb.py` & `picimagesearch-3.9.7/PicImageSearch/model/iqdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 from typing import Dict, List
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
 
 class IqdbItem:
-    """A single IQDB search result item.
+    """Represents a single IQDB search result item.
+
+    Holds details of a result from an IQDB reverse image search.
 
     Attributes:
-        origin: The original PyQuery object containing the item data.
+        origin: The raw data of the search result item.
         content: Text content of the result (e.g., 'Best match', 'Additional match').
-        url: URL of the image provided as search result.
-        source: The name of the source platform where the image was found.
-        other_source (list[dict[str, str]]): A list of dictionaries containing 'source' and 'url' for
-         additional sources.
-        thumbnail: URL of the image's thumbnail.
-        size: The dimensions and size of the image found.
-        similarity: The percentage similarity between the search image and the result.
-
+        url: URL of the webpage with the image.
+        source: Name of the source platform where the image was found.
+        other_source: Additional source URLs and their corresponding source names.
+        thumbnail: URL of the thumbnail image.
+        size: Dimensions and size of the image found.
+        similarity: Percentage similarity between the search image and the result.
     """
 
     def __init__(self, data: PyQuery):
-        """Initializes an IqdbItem with data from IQDB search result.
+        """Initializes an IqdbItem with data from a search result.
 
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance containing the search result item's data.
         """
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        self.content: str = ""  # 备注
+        self.origin: PyQuery = data
+        self.content: str = ""
         self.url: str = ""
-        self.source: str = ""  # 来源平台名称 (source platform name)
-        self.other_source: List[Dict[str, str]] = []  # 其他来源数据 (data from other sources)
+        self.source: str = ""
+        self.other_source: List[Dict[str, str]] = []
         self.thumbnail: str = ""
-        self.size: str = ""  # 原图长宽大小 (original image width, height, size)
-        self.similarity: float = 0  # 相似值
+        self.size: str = ""
+        self.similarity: float = 0
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
-        """Arranges the PyQuery data into the object's attributes.
+        """Organize search result data.
+
+        Extracts and sets the content, URL, source, other sources, thumbnail, size,
+         and similarity attributes from the given data.
 
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance containing the search result item's data.
         """
         tr_list = list(data("tr").items())
         if len(tr_list) >= 5:
             self.content = tr_list[0]("th").text()
             if self.content == "No relevant matches":
                 return
             tr_list = tr_list[1:]
@@ -73,52 +76,55 @@
         Returns:
             str: The absolute URL with 'https' prepended if necessary.
         """
         return url if url.startswith("http") else f"https:{url}"
 
 
 class IqdbResponse:
-    """Encapsulates the response from an IQDB image search.
+    """Encapsulates an IQDB reverse image search response.
+
+    Contains the complete response from an IQDB reverse image search operation.
 
     Attributes:
-        origin: The original PyQuery object containing the search result data.
-        raw: A list of IqdbItem objects representing the search results.
-        more: A list of IqdbItem objects representing the additional search results.
+        origin: The raw response data.
+        raw: List of IqdbItem instances for each search result.
+        more: Additional IqdbItem objects for lower similarity results.
         saucenao_url: URL of the search results on SauceNao.
         ascii2d_url: URL of the search results on Ascii2D.
         google_url: URL of the search results on Google Images.
         tineye_url: URL of the search results on TinEye.
-        url: URL of the search results on IQDB.
+        url: URL to the original IQDB search result page.
     """
 
     def __init__(self, resp_text: str):
-        """Initializes an IqdbResponse with data from IQDB search result.
+        """Initializes with the response text.
 
         Args:
-            resp_text: The HTML text of the IQDB search result.
+            resp_text: The text of the response.
         """
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        self.raw: List[IqdbItem] = []  # 结果返回值 (result returned from source)
-        self.more: List[
-            IqdbItem
-        ] = []  # 更多结果返回值 ( 低相似度)  (more results returned from source)
-        self.saucenao_url: str = ""  # SauceNao 搜索链接 (SauceNao search link)
-        self.ascii2d_url: str = ""  # Ascii2d 搜索链接 (Ascii2d search link)
-        self.google_url: str = ""  # Google 搜索链接 (Google search link)
-        self.tineye_url: str = ""  # TinEye 搜索链接 (TinEye search link)
+        self.origin: PyQuery = data
+        self.raw: List[IqdbItem] = []
+        self.more: List[IqdbItem] = []
+        self.saucenao_url: str = ""
+        self.ascii2d_url: str = ""
+        self.google_url: str = ""
+        self.tineye_url: str = ""
         self.url: str = ""
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
         """Arranges the PyQuery data into the object's attributes.
 
+        Extracts and sets the search result URL, primary and additional search results,
+         and URLs for other search engines.
+
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance representing a search result item.
         """
         host = (
             "https://iqdb.org"
             if data('a[href^="//3d.iqdb.org"]')
             else "https://3d.iqdb.org"
         )
         tables = list(data("#pages > div > table").items())
@@ -131,24 +137,29 @@
         else:
             self._get_other_urls(data("#show1 > a"))
         self._get_more(data("#more1 > div.pages > div > table"))
 
     def _get_more(self, data: PyQuery) -> None:
         """Get additional search results with lower similarity.
 
+        Extracts additional search results from the provided data.
+
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance representing the search result item.
         """
         self.more.extend([IqdbItem(i) for i in data.items()])
 
     def _get_other_urls(self, data: PyQuery) -> None:
         """Get URLs for other search engines.
 
+        Extracts and sets the URLs for searches on other platforms like SauceNao, ascii2d.net, Google Images,
+         and TinEye.
+
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance representing the search result item.
         """
         urls_with_name = {
             "SauceNao": ["https:", "saucenao"],
             "ascii2d.net": ["", "ascii2d"],
             "Google Images": ["https:", "google"],
             "TinEye": ["https:", "tineye"],
         }
@@ -158,11 +169,10 @@
             text = link.text()
 
             if href == "#":
                 continue
 
             if text in urls_with_name:
                 prefix, attr_name = urls_with_name[text]
-                # 检查 href 是否已包含 `https:` 前缀
-                # check if the href already contains the `https:` prefix
+                # Check if the href already contains the `https:` prefix
                 full_url = href if href.startswith("https:") else prefix + href
                 setattr(self, f"{attr_name}_url", full_url)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/saucenao.py` & `picimagesearch-3.9.7/PicImageSearch/model/saucenao.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Optional
 
 
 class SauceNAOItem:
-    """A single search result from the SauceNAO image search engine.
+    """Represents a single SauceNAO search result item.
+
+    Holds details of a result from a SauceNAO reverse image search.
 
     Attributes:
-        origin: The original response data for the item.
-        similarity: The similarity score of the search result to the query image.
-        thumbnail: The URL to the thumbnail image of the search result.
-        index_id: The index number of the result source on SauceNAO.
-        index_name: The name of the result source index.
-        hidden: An integer indicating if NSFW content is present and should be hidden (0 or 1).
-        title: The title of the work associated with the image.
-        url: The direct URL to the work (when available).
-        ext_urls: A list of external URLs for additional information or resources related to the image.
-        author: The author/creator/name of the user responsible for the work.
-        author_url: The URL to the profile or page of the author/creator.
-        source: The specific source of the search result, as a string.
+        origin: The raw data of the search result item.
+        similarity: Similarity score of the search result to the query image.
+        thumbnail: URL of the thumbnail image.
+        index_id: Index number of the result source on SauceNAO.
+        index_name: Name of the result source index.
+        hidden: Indicator of NSFW content; non-zero values indicate hidden content.
+        title: Title of the work associated with the image.
+        url: Direct URL to the work, when available.
+        ext_urls: External URLs for additional information or resources related to the image.
+        author: Author/creator/name of the user responsible for the work.
+        author_url: URL to the profile or page of the author/creator.
+        source: Specific source of the search result.
     """
 
     def __init__(self, data: Dict[str, Any]):
-        """Initializes a SauceNAOItem with data parsed from the SauceNAO API response.
+        """Initializes a SauceNAOItem with data from a search result.
 
         Args:
-            data: A dictionary containing the parsed response data for an individual result.
+            data: A dictionary containing the search result data.
         """
         result_header = data["header"]
         result_data = data["data"]
-        self.origin: Dict[str, Any] = data  # 原始数据 (raw data)
+        self.origin: Dict[str, Any] = data
         self.similarity: float = float(result_header["similarity"])
         self.thumbnail: str = result_header["thumbnail"]
-        self.index_id: int = result_header["index_id"]  # 文件 id (file id)
-        self.index_name: str = result_header["index_name"]  # 文件名称 (file name)
-        self.hidden: int = result_header.get(
-            "hidden", 0
-        )  # 是否为搜索引擎参数 hide 对应的 NSFW 内容 (whether to hide NSFW content)
+        self.index_id: int = result_header["index_id"]
+        self.index_name: str = result_header["index_name"]
+        self.hidden: int = result_header.get("hidden", 0)
         self.title: str = self._get_title(result_data)
         self.url: str = self._get_url(result_data)
         self.ext_urls: List[str] = result_data.get("ext_urls", [])
         self.author: str = self._get_author(result_data)
         self.author_url: str = self._get_author_url(result_data)
         self.source: str = result_data.get("source", "")
 
@@ -72,15 +72,15 @@
         )
 
     @staticmethod
     def _get_url(data: Dict[str, Any]) -> str:
         """Constructs the URL to the work using the result data.
 
         Args:
-            data: A dictionary containing the parsed data for an individual result.
+            data: A dictionary containing the search result data.
 
         Returns:
             The URL to the work referenced in the search result.
         """
         if "pixiv_id" in data:
             return f'https://www.pixiv.net/artworks/{data["pixiv_id"]}'
         elif "pawoo_id" in data:
@@ -147,61 +147,55 @@
             return f'https://twitter.com/intent/user?user_id={data["twitter_user_id"]}'
         elif "pawoo_user_acct" in data:
             return f'https://pawoo.net/@{data["pawoo_user_acct"]}'
         return str(data.get("author_url", ""))
 
 
 class SauceNAOResponse:
-    """Encapsulates the overall response from a SauceNAO image search.
+    """Encapsulates a SauceNAO reverse image search response.
+
+    Contains the complete response from a SauceNAO reverse image search operation.
 
     Attributes:
-        status_code: The HTTP status code received from SauceNAO.
-        raw: A list of SauceNAOItem instances representing individual search results.
-        origin: The original response data received from the SauceNAO API.
-        short_remaining: The number of search queries remaining for the short term limit.
-        long_remaining: The number of search queries remaining for the daily limit.
-        user_id: The user ID associated with the SauceNAO API account used.
-        account_type: The type of account associated with the SauceNAO API account used.
-        short_limit: Short term limit for search queries as stated by SauceNAO.
-        long_limit: Daily limit for search queries as stated by SauceNAO.
-        status: An integer status of the search query operation.
-        results_requested: The number of results requested in the search query.
-        search_depth: The number of database indexes searched by SauceNAO.
-        minimum_similarity: The minimum similarity score required for results.
-        results_returned: The number of results actually returned in the search response.
-        url: The URL of the SauceNAO search query.
+        status_code: HTTP status code received from SauceNAO.
+        raw: List of SauceNAOItem instances for each search result.
+        origin: The raw response data.
+        short_remaining: Queries remaining under the 30-second rate limit.
+        long_remaining: Queries remaining under the daily rate limit.
+        user_id: User ID of the SauceNAO API account used for the request, if any.
+        account_type: Account type of the SauceNAO API account used for the request, if any.
+        short_limit: Maximum queries allowed under the 30-second rate limit.
+        long_limit: Maximum queries allowed under the daily rate limit.
+        status: Status of the response, indicating success or error types.
+        results_requested: Number of results requested in the search query.
+        search_depth: Number of database indexes searched by SauceNAO.
+        minimum_similarity: Minimum similarity score required for results.
+        results_returned: Number of results returned in the search response.
+        url: URL to the search result page.
     """
 
     def __init__(self, data: Dict[str, Any]):
-        """Initializes a SauceNAOResponse with data parsed from the SauceNAO API response.
+        """Initializes with the response data.
 
         Args:
             data: A dictionary containing the parsed response data from SauceNAO.
         """
-        # HTTP 状态码 (HTTP status code)
         self.status_code: int = data["status_code"]
         res_header = data["header"]
         res_results = data.get("results", [])
-        # 所有的返回结果 (results returned from source)
         self.raw: List[SauceNAOItem] = [SauceNAOItem(i) for i in res_results]
-        self.origin: Dict[str, Any] = data  # 原始返回结果
-        # 每30秒访问额度 (access limit every 30 seconds)
+        self.origin: Dict[str, Any] = data
         self.short_remaining: Optional[int] = res_header.get("short_remaining")
-        # 每天访问额度 (access limit every day)
         self.long_remaining: Optional[int] = res_header.get("long_remaining")
         self.user_id: Optional[int] = res_header.get("user_id")
         self.account_type: Optional[int] = res_header.get("account_type")
         self.short_limit: Optional[str] = res_header.get("short_limit")
         self.long_limit: Optional[str] = res_header.get("long_limit")
         self.status: Optional[int] = res_header.get("status")
-        # 数据返回值数量 (result returned from source)
         self.results_requested: Optional[int] = res_header.get("results_requested")
-        # 搜索所涉及的数据库数量 (number of searched database indexes)
         self.search_depth: Optional[int] = res_header.get("search_depth")
-        # 最小相似度 (minimum similarity)
         self.minimum_similarity: Optional[float] = res_header.get("minimum_similarity")
-        # 数据返回值数量 (result returned from source)
         self.results_returned: Optional[int] = res_header.get("results_returned")
         self.url: str = (
             f"https://saucenao.com/search.php?url="
             f'https://saucenao.com{res_header.get("query_image_display")}'
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/model/yandex.py` & `picimagesearch-3.9.7/PicImageSearch/model/yandex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from typing import List
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
 
 class YandexItem:
-    """A single Yandex search result item.
+    """Represents a single Yandex search result item.
+
+    Holds details of a result from a Yandex reverse image search.
 
     Attributes:
-        url: Direct URL of the image provided as a search result.
-        title: Title associated with the image search result.
-        thumbnail: URL of the image's thumbnail.
-        source: Name of the source domain where the image was found.
-        content: Description or any additional text content provided with the search result.
-        size: The dimensions and/or size of the image found.
+        url: URL of the webpage with the image.
+        title: Title or caption associated with the image.
+        thumbnail: URL of the thumbnail image.
+        source: Domain name of the website where the image was found.
+        content: Additional text description or content with the image.
+        size: Displayed dimensions or size information of the image.
     """
 
     def __init__(self, data: PyQuery):
-        """Initializes a YandexItem with data from a Yandex search result item.
+        """Initializes a YandexItem with data from a search result.
 
         Args:
-            data: A PyQuery object representing a search result item.
+            data: A PyQuery instance containing the search result item's data.
         """
-        self.origin: PyQuery = data  # 原始数据 (raw data)
+        self.origin: PyQuery = data
         self.url: str = data.find("div.CbirSites-ItemTitle a").attr("href")
         self.title: str = data.find("div.CbirSites-ItemTitle").text()
         self.thumbnail: str = data.find("div.CbirSites-ItemThumb img").attr("src")
         if not self.thumbnail:
             self.thumbnail = data.find("div.CbirSites-ItemThumb a").attr("href")
+        # Add https to thumbnail URL if protocol is missing
         if self.thumbnail and self.thumbnail.startswith("//"):
             self.thumbnail = f"https:{self.thumbnail}"
         self.source: str = data.find("a.CbirSites-ItemDomain").text()
         self.content: str = data.find("div.CbirSites-ItemDescription").text() or ""
         self.size: str = data.find("div.Thumb-Mark").text()
 
 
 class YandexResponse:
-    """Encapsulates the response from a Yandex reverse image search.
+    """Encapsulates a Yandex reverse image search response.
+
+    Contains the complete response from a Yandex reverse image search operation.
 
     Attributes:
-        raw: A list of YandexItem objects representing the search results.
-        url: The URL from which the search results were obtained.
+        raw: List of YandexItem instances for each search result.
+        url: URL to the search results page.
     """
 
     def __init__(self, resp_text: str, resp_url: str):
-        """Initializes a YandexResponse with data from a Yandex search response.
+        """Initializes with the response text and URL.
 
         Args:
-            resp_text: The HTML text of the Yandex search response.
-            resp_url: The URL of the Yandex search page.
+            resp_text: the text of the response.
+            resp_url: URL to the search result page.
         """
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
-        self.origin: PyQuery = data  # 原始数据 (raw data)
-        # 结果返回值 (results returned from source)
+        self.origin: PyQuery = data
         self.raw: List[YandexItem] = [
             YandexItem(i) for i in data.find("li.CbirSites-Item").items()
         ]
         self.url: str = resp_url
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/network.py` & `picimagesearch-3.9.7/PicImageSearch/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,39 +11,40 @@
         "Chrome/99.0.4844.82 Safari/537.36"
     )
 }
 RESP = namedtuple("RESP", ["text", "url", "status_code"])
 
 
 class Network:
-    """Creates and manages the HTTP client used for network operations.
+    """Manages HTTP client for network operations.
 
     Attributes:
-        internal: A flag indicating whether the object should manage its own client lifecycle.
-        cookies: A dictionary that holds parsed cookies if provided in string format on initialization.
+        internal: Indicates if the object manages its own client lifecycle.
+        cookies: Dictionary of parsed cookies, provided in string format upon initialization.
+        client: Instance of an HTTP client.
     """
 
     def __init__(
         self,
         internal: bool = False,
         proxies: Optional[str] = None,
         headers: Optional[Dict[str, str]] = None,
         cookies: Optional[str] = None,
         timeout: float = 30,
         verify_ssl: bool = True,
     ):
-        """Initializes the Network object with configuration for the HTTP client.
+        """Initializes Network with configuration for HTTP requests.
 
         Args:
-            internal: Specifies if the client should be managed internally.
-            proxies: The proxy configuration to be used with the HTTP client.
-            headers: Custom headers to be used with the HTTP client.
-            cookies: Cookies to be used with the HTTP client in a ';' separated string format.
-            timeout: The timeout to use for network operations.
-            verify_ssl: A flag to indicate whether to verify SSL certificates.
+            internal: If True, Network manages its own HTTP client lifecycle.
+            proxies: Proxy settings for the HTTP client.
+            headers: Custom headers for the HTTP client.
+            cookies: Cookies in string format for the HTTP client.
+            timeout: Timeout duration for the HTTP client.
+            verify_ssl: If True, verifies SSL certificates.
         """
         self.internal: bool = internal
         headers = {**DEFAULT_HEADERS, **headers} if headers else DEFAULT_HEADERS
         self.cookies: Dict[str, str] = {}
         if cookies:
             for line in cookies.split(";"):
                 key, value = line.strip().split("=", 1)
@@ -55,140 +56,143 @@
             verify=verify_ssl,
             proxies=proxies,
             timeout=timeout,
             follow_redirects=True,
         )
 
     def start(self) -> AsyncClient:
-        """Starts and returns the internally managed HTTP client.
+        """Initializes and returns the HTTP client.
 
         Returns:
-            The initialized AsyncClient instance.
+            AsyncClient: Initialized HTTP client for network operations.
         """
         return self.client
 
     async def close(self) -> None:
-        """Closes the internally managed HTTP client session."""
+        """Closes the HTTP client session if managed internally."""
         await self.client.aclose()
 
     async def __aenter__(self) -> AsyncClient:
-        """Async context manager entry, initializing or returning the HTTP client.
+        """Async context manager entry for initializing or returning the HTTP client.
 
         Returns:
-            The initialized AsyncClient instance if managed internally, otherwise the predefined client.
+            AsyncClient: The HTTP client instance.
         """
         return self.client
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        """Async context manager exit, closing the HTTP client if it is managed internally."""
+        """Async context manager exit for closing the HTTP client if managed internally."""
         await self.client.aclose()
 
 
 class ClientManager:
-    """Manages an HTTP client for performing network requests, handling the lifecycle if created internally.
+    """Manages an HTTP client for network requests, handling lifecycle if created internally.
 
     Attributes:
-        client: The HTTP client to be managed.
+        client: Managed instance of the HTTP client.
     """
 
     def __init__(
         self,
         client: Optional[AsyncClient] = None,
         proxies: Optional[str] = None,
         headers: Optional[Dict[str, str]] = None,
         cookies: Optional[str] = None,
         timeout: float = 30,
     ):
-        """Initializes the ClientManager with an existing client or new client configuration.
+        """Initializes ClientManager with an existing HTTP client or creates a new one.
 
         Args:
-            client: A pre-configured AsyncClient instance if available, otherwise None.
-            proxies: The proxy configuration for a new client if required.
-            headers: Custom headers for a new client if required.
-            cookies: Cookies in a ';' separated string format for a new client if provided.
-            timeout: Timeout for the new client if created.
+            client: An existing AsyncClient instance or None to create a new one.
+            proxies: Proxy settings for the new client.
+            headers: Custom headers for the new client.
+            cookies: Cookies in ';' separated string format for the new client.
+            timeout: Timeout setting for the new client.
         """
         self.client: Union[Network, AsyncClient] = client or Network(
             internal=True,
             proxies=proxies,
             headers=headers,
             cookies=cookies,
             timeout=timeout,
         )
 
     async def __aenter__(self) -> AsyncClient:
-        """Async context manager entry for performing network operations, starting a new client or using an existing one
+        """Async context manager entry for network operations with new or existing client.
 
         Returns:
-            The instance of AsyncClient ready for use.
+            AsyncClient: The instance ready for use.
         """
         return self.client.start() if isinstance(self.client, Network) else self.client
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        """Async context manager exit, cleaning up the client if it was created internally."""
+        """Async context manager exit, cleans up the client if created internally."""
         if isinstance(self.client, Network) and self.client.internal:
             await self.client.close()
 
 
 class HandOver:
-    """Facilitates network operations like GET, POST, and download, reusing or creating an HTTP client accordingly.
+    """Facilitates network operations like GET, POST, and download, managing an HTTP client.
+
+    Provides methods for HTTP GET, POST requests, and download operations,
+    managing the lifecycle of an HTTP client.
 
     Attributes:
-        client: A pre-configured AsyncClient instance if available, otherwise None.
-        proxies: The proxy configuration for a new client if required.
-        headers: Custom headers for a new client if required.
-        cookies: Cookies in a ';' separated string format for a new client if provided.
-        timeout: Timeout for the new client if created.
+        client: Optional pre-configured AsyncClient instance.
+        proxies: Proxy settings for requests.
+        headers: Custom HTTP headers for requests.
+        cookies: Cookies for requests in string format.
+        timeout: Timeout duration for requests.
     """
 
     def __init__(
         self,
         client: Optional[AsyncClient] = None,
         proxies: Optional[str] = None,
         headers: Optional[Dict[str, str]] = None,
         cookies: Optional[str] = None,
         timeout: float = 30,
     ):
-        """Initializes the HandOver with or without a pre-configured AsyncClient.
+        """Initializes HandOver with an existing AsyncClient or creates a new one.
 
         Args:
-            client: An existing AsyncClient to be reused, otherwise None.
-            proxies: Proxies for a new client if required.
-            headers: Custom headers for a new client if required.
-            cookies: Cookies in a ';' separated string format for a new client if provided.
-            timeout: Timeout for a new client if created.
+            client: An existing AsyncClient or None for a new client.
+            proxies: Proxy settings.
+            headers: Custom headers.
+            cookies: Cookies in ';' separated string format.
+            timeout: Timeout duration.
         """
         self.client: Optional[AsyncClient] = client
         self.proxies: Optional[str] = proxies
         self.headers: Optional[Dict[str, str]] = headers
         self.cookies: Optional[str] = cookies
         self.timeout: float = timeout
 
     async def get(
         self, url: str, params: Optional[Dict[str, str]] = None, **kwargs: Any
     ) -> RESP:
         """Performs an HTTP GET request.
 
         Args:
-            url: The URL to perform the GET request on.
-            params: Optional dictionary of URL parameters to append to the URL.
-            **kwargs: Additional keyword arguments passed to the GET request method.
+            url: URL for the GET request.
+            params: Optional query parameters.
+            **kwargs: Additional arguments for the GET request.
 
         Returns:
-            A namedtuple RESP with response text, response URL, and status code.
+            RESP: Response with text, URL, and status code.
         """
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
             self.timeout,
@@ -204,44 +208,44 @@
         files: Optional[Dict[str, Any]] = None,
         json: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> RESP:
         """Performs an HTTP POST request.
 
         Args:
-            url: The URL to perform the POST request on.
-            params: Optional dictionary or QueryParams object of URL parameters.
-            data: Optional dictionary of form data to send in the body of the request.
-            files: Optional dictionary of file-like objects to send in the multipart request.
-            json: Optional dictionary which if given, will be sent as a JSON payload.
-            **kwargs: Additional keyword arguments passed to the POST request method.
+            url: URL for the POST request.
+            params: Optional query or QueryParams object.
+            data: Optional data for the request body.
+            files: Optional file-like objects for multipart submissions.
+            json: Optional JSON payload for the request body.
+            **kwargs: Additional arguments for the POST request.
 
         Returns:
-            A namedtuple RESP with response text, response URL, and status code.
+            RESP: Response with text, URL, and status code.
         """
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
             self.timeout,
         ) as client:
             resp = await client.post(
                 url, params=params, data=data, files=files, json=json, **kwargs
             )
             return RESP(resp.text, str(resp.url), resp.status_code)
 
     async def download(self, url: str) -> bytes:
-        """Downloads content from a given URL.
+        """Downloads content from a URL.
 
         Args:
-            url: The URL to download content from.
+            url: URL to download content from.
 
         Returns:
-            The content of the response as bytes.
+            bytes: Downloaded content.
         """
         async with ClientManager(
             self.client,
             self.proxies,
             self.headers,
             self.cookies,
             self.timeout,
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/saucenao.py` & `picimagesearch-3.9.7/PicImageSearch/saucenao.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from typing import Any, Dict, List, Optional, Union
 
 from httpx import QueryParams
 
 from .model import SauceNAOResponse
 from .network import HandOver
 
+BASE_URL = "https://saucenao.com/search.php"
+
 
 class SauceNAO(HandOver):
     """API client for the SauceNAO image search engine.
 
+    Used for performing reverse image searches using SauceNAO service.
+
     Attributes:
-        url: The URL endpoint for the SauceNAO API.
-        params: Query parameters for the SauceNAO API.
+        params: The query parameters for SauceNAO search.
     """
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         numres: int = 5,
         hide: int = 0,
@@ -26,38 +29,36 @@
         testmode: int = 0,
         dbmask: Optional[int] = None,
         dbmaski: Optional[int] = None,
         db: int = 999,
         dbs: Optional[List[int]] = None,
         **request_kwargs: Any,
     ):
-        """Initializes SauceNAO API client with configuration.
-
-        Further documentation on the API can be found at on saucenao.com when your account is logged in:
-            https://saucenao.com/user.php?page=search-api
-
-        For more information on `dbmask`, `dbmaski`, `db`, and `dbs` specifically, see:
-            https://saucenao.com/tools/examples/api/index_details.txt
+        """Initializes a SauceNAO API client with specified configurations.
 
         Args:
-            api_key: Access key for SauceNAO.
-            numres: The number of results to return.
-            hide: Control over hiding results based on content rating.
-            minsim: The minimum similarity threshold required for a result.
-            output_type: Specifies the output format (0=html, 1=xml, 2=json).
-            testmode: Enables test mode, which performs a dry-run.
-            dbmask: A bitmask to select specific indices to be enabled.
-            dbmaski: A bitmask to select specific indices to be disabled.
-            db: Specifies individual database indices to search (999 for all).
-            dbs: Specifies multiple database indices to search.
-            **request_kwargs: Additional keyword arguments for request configuration.
+            api_key: API key for SauceNAO API access.
+            numres: Number of results to return from search.
+            hide: Option to hide results based on content rating.
+            minsim: Minimum similarity percentage for results.
+            output_type: Output format of search results.
+            testmode: If 1, performs a dry-run search.
+            dbmask: Bitmask for enabling specific databases.
+            dbmaski: Bitmask for disabling specific databases.
+            db: Specifies database index(es) for search.
+            dbs: List of database indices for search.
+            **request_kwargs: Additional arguments for network requests.
+
+        Note:
+            Detailed API documentation is available at:
+            https://saucenao.com/user.php?page=search-api (requires login).
+            For specific details on `dbmask`, `dbmaski`, `db`, and `dbs`, refer to:
+            https://saucenao.com/tools/examples/api/index_details.txt
         """
-        # minsim 控制最小相似度 (minsim controls the minimum similarity)
         super().__init__(**request_kwargs)
-        self.url = "https://saucenao.com/search.php"
         params: Dict[str, Any] = {
             "testmode": testmode,
             "numres": numres,
             "output_type": output_type,
             "hide": hide,
             "db": db,
             "minsim": minsim,
@@ -73,35 +74,39 @@
             self.params = self.params.remove("db")
             for i in dbs:
                 self.params = self.params.add("dbs[]", i)
 
     async def search(
         self, url: Optional[str] = None, file: Union[str, bytes, Path, None] = None
     ) -> SauceNAOResponse:
-        """Searches for images using the SauceNAO API.
+        """Performs a reverse image search on SauceNAO.
+
+        Supports searching by image URL or by uploading an image file.
+
+        Requires either 'url' or 'file' to be provided.
 
         Args:
-            url: The URL of the image to be searched.
-            file: The local file path or image file bytes to be searched.
+            url: URL of the image to search.
+            file: Local image file (path or bytes) to search.
 
         Returns:
-            SauceNAOResponse: The response containing search results and metadata.
+            SauceNAOResponse: Contains search results and additional information.
 
         Raises:
-            ValueError: If neither a URL nor a file is provided as a search parameter.
+            ValueError: If neither 'url' nor 'file' is provided.
         """
         params = self.params
         files: Optional[Dict[str, Any]] = None
         if url:
             params = params.add("url", url)
         elif file:
             files = (
                 {"file": file}
                 if isinstance(file, bytes)
                 else {"file": open(file, "rb")}
             )
         else:
-            raise ValueError("url or file is required")
-        resp = await self.post(self.url, params=params, files=files)
+            raise ValueError("Either 'url' or 'file' must be provided")
+        resp = await self.post(BASE_URL, params=params, files=files)
         resp_json = json_loads(resp.text)
         resp_json.update({"status_code": resp.status_code})
         return SauceNAOResponse(resp_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/sync.py` & `picimagesearch-3.9.7/PicImageSearch/sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-"""
-From: telethon/sync
-This magical module will rewrite all public methods in the public interface
-of the library so they can run the loop on their own if it's not already
-running. This rewrite may not be desirable if the end user always uses the
-methods they way they should be ran, but it's incredibly useful for quick
-scripts and the runtime overhead is relatively low.
+"""From: telethon/sync
+Rewrites all public asynchronous methods in the library's public interface for synchronous execution.
+Useful for scripts, with low runtime overhead. Ideal for synchronous calls preference over managing an event loop.
+
+Automatically wraps asynchronous methods of specified classes, enabling synchronous calls.
 """
 import asyncio
 import functools
 import inspect
 
 from . import Ascii2D, BaiDu, EHentai, Google, Iqdb, Network, SauceNAO, TraceMoe, Yandex
 
 
-def _syncify_wrap(t, method_name):  # type: ignore
-    """Wrap an asynchronous method to allow synchronous execution.
+def _syncify_wrap(class_type, method_name):  # type: ignore
+    """Wrap an asynchronous method of a class for synchronous calling.
 
-    The wrapper checks if the event loop is already running, and executes the method
-    accordingly. The original asynchronous method is stored as `__tl.sync` attribute.
+    Creates a synchronous version of the specified asynchronous method.
+    Checks if the event loop is running; if not, runs it until method completion.
+    Original asynchronous method remains accessible via `__tl.sync` attribute.
 
     Args:
-        class_type: The class containing the method to wrap.
-        method_name: The name of the method to wrap.
+        class_type: Class with the method to wrap.
+        method_name: Name of the asynchronous method to wrap.
 
     Returns:
-        A wrapped synchronous method which can be called directly.
+        None: Modifies the class method in-place.
     """
-    method = getattr(t, method_name)
+    method = getattr(class_type, method_name)
 
     @functools.wraps(method)
     def syncified(*args, **kwargs):  # type: ignore
         coro = method(*args, **kwargs)
         loop = asyncio.get_event_loop()
         return coro if loop.is_running() else loop.run_until_complete(coro)
 
-    # Save an accessible reference to the original method
     setattr(syncified, "__tl.sync", method)
-    setattr(t, method_name, syncified)
+    setattr(class_type, method_name, syncified)
 
 
-def syncify(*types):  # type: ignore
-    """Decorate all coroutine methods of given classes to enable synchronous calling.
+def syncify(*classes):  # type: ignore
+    """Decorate coroutine methods of classes for synchronous execution.
 
-    This function applies `_syncify_wrap` decorator to all coroutine methods
-    of the passed in classes, allowing those methods to be run synchronously.
+    Iterates over classes, applying `_syncify_wrap` to coroutine methods.
+    Enables methods to be used synchronously without managing an asyncio loop.
 
     Args:
-        classes: A variable number of class objects to syncify.
+        *classes: Classes to modify for synchronous coroutine method use.
     """
-    for t in types:
-        for name in dir(t):
+    for c in classes:
+        for name in dir(c):
             if (
                 not name.startswith("_") or name == "__call__"
-            ) and inspect.iscoroutinefunction(getattr(t, name)):
-                _syncify_wrap(t, name)  # type: ignore
+            ) and inspect.iscoroutinefunction(getattr(c, name)):
+                _syncify_wrap(c, name)  # type: ignore
 
 
 syncify(Ascii2D, BaiDu, EHentai, Google, Iqdb, Network, SauceNAO, TraceMoe, Yandex)  # type: ignore
 
 __all__ = [
     "Ascii2D",
     "BaiDu",
```

### Comparing `picimagesearch-3.9.6/PicImageSearch/tracemoe.py` & `picimagesearch-3.9.7/PicImageSearch/tracemoe.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,107 +35,100 @@
     isAdult
   }
 }
 """
 
 
 class TraceMoe(HandOver):
-    """API Client for the TraceMoe API to search anime by image.
+    """API Client for the TraceMoe image search engine.
 
-    Inherits from HandOver for network operations.
+    Used for performing reverse image searches using TraceMoe service.
 
     Attributes:
-        search_url: A string representing the API endpoint for searching.
-        me_url: A string representing the API endpoint to retrieve user info.
-        size: An optional string indicating the size of the preview (s/m/l).
-        mute: A boolean indicating whether to mute the preview video.
+        search_url: URL for TraceMoe API endpoint for image search.
+        me_url: URL for TraceMoe API endpoint to retrieve user info.
+        size: Optional string indicating preview size ('s', 'm', 'l').
+        mute: A flag to mute preview video in search results.
     """
 
     search_url = "https://api.trace.moe/search"
     me_url = "https://api.trace.moe/me"
 
     def __init__(
         self, mute: bool = False, size: Optional[str] = None, **request_kwargs: Any
     ):
-        """Initializes the TraceMoe client with optional settings.
+        """Initializes a TraceMoe API client with specified configurations.
 
         Args:
-            mute: If True, mutes the preview video. Defaults to False.
-            size: Defines the preview size. Can be 's', 'm', or 'l'.
-            **request_kwargs: Additional keyword arguments for request settings.
+            mute: If True, mutes preview video in search results.
+            size: Specifies preview video size ('s', 'm', 'l').
+            **request_kwargs: Additional arguments for network requests.
         """
         super().__init__(**request_kwargs)
         self.size: Optional[str] = size
         self.mute: bool = mute
 
     async def me(self, key: Optional[str] = None) -> TraceMoeMe:
-        """Retrieves information about the API key usage.
+        """Retrieves information about the user's API key usage from TraceMoe.
 
         Args:
-            key: The API key for authentication.
+            key: Optional API key for authentication.
 
         Returns:
-            An instance of TraceMoeMe containing the user's information.
-
-        Raises:
-            HTTPError: If the request to the API fails.
+            TraceMoeMe: Information about the user's API key usage.
         """
         params = {"key": key} if key else None
         resp = await self.get(self.me_url, params=params)
         return TraceMoeMe(json_loads(resp.text))
 
     @staticmethod
     def set_params(
         url: Optional[str],
         anilist_id: Optional[int],
         cut_borders: bool,
     ) -> Dict[str, Union[bool, int, str]]:
-        """Constructs query parameters for API requests.
+        """Constructs query parameters for TraceMoe API request.
 
         Args:
-            url: The image URL to search for.
-            anilist_id: The Anilist ID to limit the search to.
-            cut_borders: If True, trims the borders of the image.
+            url: URL of the image to search.
+            anilist_id: Anilist ID for specific anime focus.
+            cut_borders: If True, trims image borders during search.
 
         Returns:
-            A dictionary with query parameters for the API request.
+            Dict[str, Union[bool, int, str]]: Query parameters for the API request.
         """
         params: Dict[str, Union[bool, int, str]] = {}
         if cut_borders:
             params["cutBorders"] = "true"
         if anilist_id:
             params["anilistID"] = anilist_id
         if url:
             params["url"] = url
         return params
 
     async def update_anime_info(
         self, item: TraceMoeItem, chinese_title: bool = True
     ) -> None:
-        """Updates the anime information of a search result item.
+        """Updates TraceMoeItem with detailed anime information from TraceMoe API.
 
         Args:
-            item: The TraceMoeItem object to update with additional data.
-            chinese_title: If True, retrieves the Chinese title if available.
-
-        Raises:
-            HTTPError: If the request to the API fails.
+            item: TraceMoeItem to update with anime information.
+            chinese_title: If True, includes Chinese title in item info.
         """
         variables = {"id": item.anilist}
         url = "https://trace.moe/anilist/"
         item.anime_info = json_loads(
             (
                 await self.post(
                     url=url, json={"query": ANIME_INFO_QUERY, "variables": variables}
                 )
             )[0]
         )["data"]["Media"]
-        item.idMal = item.anime_info[
-            "idMal"
-        ]  # 匹配的MyAnimelist ID见https://myanimelist.net/ (matched MyAnimelist ID)
+        # Update item fields with anime information
+        item.idMal = item.anime_info["idMal"]
         item.title = item.anime_info["title"]
         item.title_native = item.anime_info["title"]["native"]
         item.title_romaji = item.anime_info["title"]["romaji"]
         item.title_english = item.anime_info["title"]["english"]
         item.synonyms = item.anime_info["synonyms"]
         item.isAdult = item.anime_info["isAdult"]
         item.type = item.anime_info["type"]
@@ -151,44 +144,47 @@
         url: Optional[str] = None,
         file: Union[str, bytes, Path, None] = None,
         key: Optional[str] = None,
         anilist_id: Optional[int] = None,
         chinese_title: bool = True,
         cut_borders: bool = True,
     ) -> TraceMoeResponse:
-        """Searches for anime using an image or URL.
+        """Performs a reverse image search on TraceMoe.
+
+        Supports searching by image URL or by uploading an image file.
+
+        Requires either 'url' or 'file' to be provided.
 
         Args:
-            url: URL of the image.
-            file: Local image file path or image data.
-            key: API key for authentication.
-            anilist_id: Anilist ID to limit the search.
-            chinese_title: Include Chinese title in the result if available.
-            cut_borders: Trim image borders during search.
+            url: URL of the image to search.
+            file: Local image file (path or bytes) to search.
+            key: Optional API key for authentication.
+            anilist_id: Anilist ID to limit search scope.
+            chinese_title: If True, includes Chinese titles in results.
+            cut_borders: If True, trims image borders for search.
 
         Returns:
-            A TraceMoeResponse object with search results.
+            TraceMoeResponse: Search results and additional metadata.
 
         Raises:
-            ValueError: If neither URL nor file is provided.
-            HTTPError: If the request to the API fails.
+            ValueError: If neither 'url' nor 'file' is provided.
         """
         headers = {"x-trace-key": key} if key else None
         files: Optional[Dict[str, Any]] = None
         if url:
             params = self.set_params(url, anilist_id, cut_borders)
         elif file:
             params = self.set_params(None, anilist_id, cut_borders)
             files = (
                 {"file": file}
                 if isinstance(file, bytes)
                 else {"file": open(file, "rb")}
             )
         else:
-            raise ValueError("url or file is required")
+            raise ValueError("Either 'url' or 'file' must be provided")
         resp = await self.post(
             self.search_url, headers=headers, params=params, files=files
         )
         result = TraceMoeResponse(json_loads(resp.text), self.mute, self.size)
         await asyncio.gather(
             *[self.update_anime_info(item, chinese_title) for item in result.raw]
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picimagesearch-3.9.6/README.md` & `picimagesearch-3.9.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 <div align="center">
 
 # PicImageSearch
 
-✨ 聚合识图引擎 用于以图搜源 ✨ Reverse Image Search Aggregator ✨
+Read this in other languages: [English](README.md), [中文](README.cn.md), [Русский](README.ru.md)
 
-</div>
+✨ Reverse Image Search Aggregator ✨
 
-<p align="center">
-  <a href="https://raw.githubusercontent.com/kitUIN/PicImageSearch/master/LICENSE">
+<a href="https://raw.githubusercontent.com/kitUIN/PicImageSearch/master/LICENSE">
     <img src="https://img.shields.io/github/license/kitUIN/PicImageSearch" alt="license">
-  </a>
-  <a href="https://pypi.python.org/pypi/PicImageSearch">
+</a>
+<a href="https://pypi.python.org/pypi/PicImageSearch">
     <img src="https://img.shields.io/pypi/v/PicImageSearch" alt="pypi">
-  </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
-  <a href="https://github.com/kitUIN/PicImageSearch/releases">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
+<a href="https://github.com/kitUIN/PicImageSearch/releases">
     <img src="https://img.shields.io/github/v/release/kitUIN/PicImageSearch" alt="release">
-  </a>
-  <a href="https://github.com/kitUIN/PicImageSearch/issues">
-    <img src="https://img.shields.io/github/issues/kitUIN/PicImageSearch" alt="release">
-  </a>
- </p>
-<p align="center">
-  <a href="https://pic-image-search.kituin.fun/">📖文档 / Documentation</a>
-  ·
-  <a href="https://github.com/kitUIN/PicImageSearch/issues/new">🐛提交建议 / Submit Suggestions</a>
-</p>
-
-## 简要说明 / Usage
-
-详细见[文档](https://pic-image-search.kituin.fun/) 或者[`demo`](https://github.com/kitUIN/PicImageSearch/tree/main/demo)
-\
-`同步`请使用`from PicImageSearch.sync import ...`导入\
-`异步`请使用`from PicImageSearch import Network,...`导入\
-**推荐使用异步**
-
-For details, see the [Documentation](https://pic-image-search.kituin.fun/) or the
-[`demo`](https://github.com/kitUIN/PicImageSearch/tree/main/demo). \
-For synchronous usage, import with `from PicImageSearch.sync import ...`. \
-For asynchronous usage, import with `from PicImageSearch import Network,...`. \
-**Asynchronous usage is recommended.**
+</a>
+<a href="https://github.com/kitUIN/PicImageSearch/issues">
+    <img src="https://img.shields.io/github/issues/kitUIN/PicImageSearch" alt="issues">
+</a>
+
+<a href="https://pic-image-search.kituin.fun/">📖 Documentation</a>
+·
+<a href="https://github.com/kitUIN/PicImageSearch/issues/new">🐛 Submit Issue</a>
 
-### 安装 / Installation
+</div>
 
-- 此包需要 Python 3.8 或更新版本。
-- `pip install PicImageSearch` 或者
-- `pip install PicImageSearch -i https://pypi.tuna.tsinghua.edu.cn/simple`
+## Support
+
+| Engine   | Website                          |
+|----------|----------------------------------|
+| ASCII2D  | https://ascii2d.net/             |
+| Baidu    | https://graph.baidu.com/         |
+| E-Hentai | https://e-hentai.org/            |
+| ExHentai | https://exhentai.org/            |
+| Google   | https://www.google.com/imghp     |
+| IQDB     | https://iqdb.org/                |
+| SauceNAO | https://saucenao.com/            |
+| TraceMoe | https://trace.moe/               |
+| Yandex   | https://yandex.com/images/search |
+
+## Usage
+
+For details, see the [documentation](https://pic-image-search.kituin.fun/) or the [demo codes](demo/en/).  
+For synchronous usage, import with `from PicImageSearch.sync import ...` .  
+For asynchronous usage, import with `from PicImageSearch import Network,...` .  
+**Asynchronous usage is recommended.**
 
-<!-- Separation -->
+### Installation
 
-- This package requires Python 3.8 or later.
-- `pip install PicImageSearch` or
-- `pip install PicImageSearch -i https://pypi.tuna.tsinghua.edu.cn/simple`
+- Requires Python 3.8 or later.
+- Install: `pip install PicImageSearch`
+- Or use Tsinghua mirror: `pip install PicImageSearch -i https://pypi.tuna.tsinghua.edu.cn/simple`
 
 ## Star History
 
 [![Star History](https://starchart.cc/kitUIN/PicImageSearch.svg)](https://starchart.cc/kitUIN/PicImageSearch)
```

#### html2text {}

```diff
@@ -1,20 +1,18 @@
- # PicImageSearch â¨ èåè¯å¾å¼æ ç¨äºä»¥å¾ææº â¨ Reverse Image
-                             Search Aggregator â¨
-                   _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]_[_r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_]
-      _ð____æ___æ_¡_£_ _/_ _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _ð____æ___ä_º_¤_å_»_º_è_®_®_ _/_ _S_u_b_m_i_t_ _S_u_g_g_e_s_t_i_o_n_s
-## ç®è¦è¯´æ / Usage è¯¦ç»è§[ææ¡£](https://pic-image-search.kituin.fun/
-) æè[`demo`](https://github.com/kitUIN/PicImageSearch/tree/main/demo) \
-`åæ­¥`è¯·ä½¿ç¨`from PicImageSearch.sync import ...`å¯¼å¥\
-`å¼æ­¥`è¯·ä½¿ç¨`from PicImageSearch import Network,...`å¯¼å¥\
-**æ¨èä½¿ç¨å¼æ­¥** For details, see the [Documentation](https://pic-image-
-search.kituin.fun/) or the [`demo`](https://github.com/kitUIN/PicImageSearch/
-tree/main/demo). \ For synchronous usage, import with `from PicImageSearch.sync
-import ...`. \ For asynchronous usage, import with `from PicImageSearch import
-Network,...`. \ **Asynchronous usage is recommended.** ### å®è£ /
-Installation - æ­¤åéè¦ Python 3.8 ææ´æ°çæ¬ã - `pip install
-PicImageSearch` æè - `pip install PicImageSearch -i https://
-pypi.tuna.tsinghua.edu.cn/simple` - This package requires Python 3.8 or later.
-- `pip install PicImageSearch` or - `pip install PicImageSearch -i https://
-pypi.tuna.tsinghua.edu.cn/simple` ## Star History [![Star History](https://
-starchart.cc/kitUIN/PicImageSearch.svg)](https://starchart.cc/kitUIN/
-PicImageSearch)
+ # PicImageSearch Read this in other languages: [English](README.md), [ä¸­æ]
+    (README.cn.md), [Ð ÑÑÑÐºÐ¸Ð¹](README.ru.md) â¨ Reverse Image Search
+ Aggregator â¨ _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]_[_r_e_l_e_a_s_e_]_[_i_s_s_u_e_s_]_ð____ _D_o_c_u_m_e_n_t_a_t_i_o_n Â·
+                               _ð____ _S_u_b_m_i_t_ _I_s_s_u_e
+## Support | Engine | Website | |----------|----------------------------------
+| | ASCII2D | https://ascii2d.net/ | | Baidu | https://graph.baidu.com/ | | E-
+Hentai | https://e-hentai.org/ | | ExHentai | https://exhentai.org/ | | Google
+| https://www.google.com/imghp | | IQDB | https://iqdb.org/ | | SauceNAO |
+https://saucenao.com/ | | TraceMoe | https://trace.moe/ | | Yandex | https://
+yandex.com/images/search | ## Usage For details, see the [documentation](https:
+//pic-image-search.kituin.fun/) or the [demo codes](demo/en/). For synchronous
+usage, import with `from PicImageSearch.sync import ...` . For asynchronous
+usage, import with `from PicImageSearch import Network,...` . **Asynchronous
+usage is recommended.** ### Installation - Requires Python 3.8 or later. -
+Install: `pip install PicImageSearch` - Or use Tsinghua mirror: `pip install
+PicImageSearch -i https://pypi.tuna.tsinghua.edu.cn/simple` ## Star History [!
+[Star History](https://starchart.cc/kitUIN/PicImageSearch.svg)](https://
+starchart.cc/kitUIN/PicImageSearch)
```

### Comparing `picimagesearch-3.9.6/pyproject.toml` & `picimagesearch-3.9.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PicImageSearch"
-version = "3.9.6"
+version = "3.9.7"
 description = "PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "lleans", "chinoll", "NekoAria"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "PicImageSearch" }]
 homepage = "https://github.com/kitUIN/PicImageSearch"
@@ -18,28 +18,28 @@
     "saucenao",
     "tracemoe",
     "yandex",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.25.1"
+httpx = "^0.25.2"
 lxml = "^4.9.3"
 pyquery = "^2.0.0"
 socksio = { version = "^1.0.0", optional = true }
 
 [tool.poetry.extras]
 socks = ["socksio"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.11.0"
 loguru = "^0.7.2"
-mypy = "^1.7.0"
+mypy = "^1.7.1"
 pre-commit = "^3.5.0"
-ruff = "^0.1.5"
+ruff = "^0.1.7"
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 implicit_reexport = true
 pretty = true
 show_error_codes = true
@@ -49,10 +49,13 @@
 select = ["F", "E", "W", "I", "UP"]
 target-version = "py38"
 line-length = 120
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

