# Comparing `tmp/wolf_comm-0.0.7.tar.gz` & `tmp/wolf_comm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolf_comm-0.0.7.tar", last modified: Thu Apr 18 17:57:11 2024, max compression
+gzip compressed data, was "wolf_comm-0.0.8.tar", last modified: Fri May 10 22:59:41 2024, max compression
```

## Comparing `wolf_comm-0.0.7.tar` & `wolf_comm-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.916415 wolf_comm-0.0.7/
--rw-r--r--   0 i037503    (501) staff       (20)    11357 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/LICENSE.txt
--rw-r--r--   0 i037503    (501) staff       (20)      831 2024-04-18 17:57:11.916075 wolf_comm-0.0.7/PKG-INFO
--rw-r--r--   0 i037503    (501) staff       (20)      410 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/README.md
--rw-r--r--   0 i037503    (501) staff       (20)       38 2024-04-18 17:57:11.916499 wolf_comm-0.0.7/setup.cfg
--rw-r--r--   0 i037503    (501) staff       (20)      766 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/setup.py
-drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.905183 wolf_comm-0.0.7/wolf_comm/
--rw-r--r--   0 i037503    (501) staff       (20)       67 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/__init__.py
--rw-r--r--   0 i037503    (501) staff       (20)     1108 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/constants.py
--rw-r--r--   0 i037503    (501) staff       (20)     1091 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/create_session.py
--rw-r--r--   0 i037503    (501) staff       (20)       79 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/helpers.py
--rw-r--r--   0 i037503    (501) staff       (20)     5713 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/models.py
--rw-r--r--   0 i037503    (501) staff       (20)     4646 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/token_auth.py
--rw-r--r--   0 i037503    (501) staff       (20)     8539 2024-04-18 17:55:30.000000 wolf_comm-0.0.7/wolf_comm/wolf_client.py
-drwxr-xr-x   0 i037503    (501) staff       (20)        0 2024-04-18 17:57:11.915663 wolf_comm-0.0.7/wolf_comm.egg-info/
--rw-r--r--   0 i037503    (501) staff       (20)      831 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/PKG-INFO
--rw-r--r--   0 i037503    (501) staff       (20)      357 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/SOURCES.txt
--rw-r--r--   0 i037503    (501) staff       (20)        1 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/dependency_links.txt
--rw-r--r--   0 i037503    (501) staff       (20)       26 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/requires.txt
--rw-r--r--   0 i037503    (501) staff       (20)       10 2024-04-18 17:57:11.000000 wolf_comm-0.0.7/wolf_comm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 22:59:41.102870 wolf_comm-0.0.8/
+-rw-rw-rw-   0        0        0    11357 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      909 2024-05-10 22:59:41.101870 wolf_comm-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 22:59:41.102870 wolf_comm-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-10 22:59:37.000000 wolf_comm-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 22:59:41.092918 wolf_comm-0.0.8/wolf_comm/
+-rw-rw-rw-   0        0        0       67 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/__init__.py
+-rw-rw-rw-   0        0        0     1108 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/constants.py
+-rw-rw-rw-   0        0        0     1091 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/create_session.py
+-rw-rw-rw-   0        0        0       79 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/helpers.py
+-rw-rw-rw-   0        0        0     5713 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/models.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/py.typed
+-rw-rw-rw-   0        0        0     4842 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/token_auth.py
+-rw-rw-rw-   0        0        0     8890 2024-05-10 22:47:13.000000 wolf_comm-0.0.8/wolf_comm/wolf_client.py
+drwxrwxrwx   0        0        0        0 2024-05-10 22:59:41.101870 wolf_comm-0.0.8/wolf_comm.egg-info/
+-rw-rw-rw-   0        0        0      909 2024-05-10 22:59:41.000000 wolf_comm-0.0.8/wolf_comm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-10 22:59:41.000000 wolf_comm-0.0.8/wolf_comm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 22:59:41.000000 wolf_comm-0.0.8/wolf_comm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 22:59:41.000000 wolf_comm-0.0.8/wolf_comm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 22:59:41.000000 wolf_comm-0.0.8/wolf_comm.egg-info/top_level.txt
```

### Comparing `wolf_comm-0.0.7/LICENSE.txt` & `wolf_comm-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolf_comm-0.0.7/setup.py` & `wolf_comm-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='wolf_comm',
-    version='0.0.7',
+    version='0.0.8',
     author="Jan Rothkegel",
     author_email="jan.rothkegel@web.de",
     description="A package to communicate with Wolf SmartSet Cloud",
     long_description=long_description,
     package_data={"wolf_comm": ["py.typed"]},
     long_description_content_type="text/markdown",
     url="https://github.com/janrothkegel/wolf-comm",
```

### Comparing `wolf_comm-0.0.7/wolf_comm/constants.py` & `wolf_comm-0.0.8/wolf_comm/constants.py`

 * *Files identical despite different names*

### Comparing `wolf_comm-0.0.7/wolf_comm/create_session.py` & `wolf_comm-0.0.8/wolf_comm/create_session.py`

 * *Files identical despite different names*

### Comparing `wolf_comm-0.0.7/wolf_comm/models.py` & `wolf_comm-0.0.8/wolf_comm/models.py`

 * *Files identical despite different names*

### Comparing `wolf_comm-0.0.7/wolf_comm/token_auth.py` & `wolf_comm-0.0.8/wolf_comm/token_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Tokens:
-    """Has two tokens: access and refresh"""
+    """Has only one token: access"""
 
-    def __init__(self, access_token: str, refresh_token: str, expires_in: int):
+    def __init__(self, access_token: str, expires_in: int):
         self.access_token = access_token
-        self.refresh_token = refresh_token
         self.expire_date = datetime.datetime.now() + datetime.timedelta(seconds=expires_in)
 
     def is_expired(self) -> bool:
         return self.expire_date < datetime.datetime.now()
 
 
 class TokenAuth:
@@ -44,72 +43,77 @@
             r = await client.get(constants.AUTHENTICATION_BASE_URL + '/Account/Login?ReturnUrl=/idsrv/connect/authorize/callback?client_id={}&redirect_uri={}/signin-callback.html&response_type=code&scope=openid%2520profile api role&state={}&code_challenge={}&code_challenge_method=S256&response_mode=query&lang=de-DE'.format(constants.AUTHENTICATION_CLIENT, constants.BASE_URL,state, code_challenge))
 
             _LOGGER.debug('Verification code response: %s', r.content)
 
             tree = html.document_fromstring(r.text)
             elements = tree.xpath('//form/input/@value')
 
-            verification_token = elements[0] # __RequestVerificationToken
+            if elements:
 
-            # Get code
-            login_data = {
-                "Input.Username": self.username,
-                "Input.Password": self.password,
-                "__RequestVerificationToken": verification_token
-            }
-
-            r = await client.post(
-                constants.AUTHENTICATION_BASE_URL + "/Account/Login",
-                params={
-                    "ReturnUrl": constants.AUTHENTICATION_URL + "/connect/authorize/callback?client_id={}&redirect_uri={}/signin-callback.html&response_type=code&scope=openid profile api role&state={}&code_challenge={}&code_challenge_method=S256&response_mode=query&lang=de-DE".format(constants.AUTHENTICATION_CLIENT, constants.BASE_URL, state,code_challenge)
-                },
-                headers={
+                _LOGGER.debug('Verification token: %s', elements[0])
+
+                verification_token = elements[0] # __RequestVerificationToken
+
+                # Get code
+                login_data = {
+                    "Input.Username": self.username,
+                    "Input.Password": self.password,
+                    "__RequestVerificationToken": verification_token
+                }
+
+                r = await client.post(
+                    constants.AUTHENTICATION_BASE_URL + "/Account/Login",
+                    params={
+                        "ReturnUrl": constants.AUTHENTICATION_URL + "/connect/authorize/callback?client_id={}&redirect_uri={}/signin-callback.html&response_type=code&scope=openid profile api role&state={}&code_challenge={}&code_challenge_method=S256&response_mode=query&lang=de-DE".format(constants.AUTHENTICATION_CLIENT, constants.BASE_URL, state,code_challenge)
+                    },
+                    headers={
+                        "Sec-Fetch-Dest": "document",
+                        "Sec-Fetch-Mode": "navigate",
+                    },
+                    data=login_data,
+                    cookies = r.cookies,
+                    follow_redirects=True
+                )
+                
+                _LOGGER.debug('Code response: %s', r.content)
+                code = r.url.params['code']
+                
+
+                headers = {
+                    "Cache-control": "no-cache",
+                    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0",
+                    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+                    "Accept-Language": "de-DE,de;q=0.8,en-US;q=0.5,en;q=0.3",
+                    "Referer": constants.BASE_URL + "/",
                     "Sec-Fetch-Dest": "document",
                     "Sec-Fetch-Mode": "navigate",
-                },
-                data=login_data,
-                cookies = r.cookies,
-                follow_redirects=True
-            )
-            
-            _LOGGER.debug('Code response: %s', r.content)
-            code = r.url.params['code']
-            
-
-            headers = {
-                "Cache-control": "no-cache",
-                "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0",
-                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-                "Accept-Language": "de-DE,de;q=0.8,en-US;q=0.5,en;q=0.3",
-                "Referer": constants.BASE_URL + "/",
-                "Sec-Fetch-Dest": "document",
-                "Sec-Fetch-Mode": "navigate",
-                "Sec-Fetch-Site": "same-origin",
-                "TE": "trailers"
-            }
-
-            # Get token
-            r = await client.post(
-                constants.AUTHENTICATION_BASE_URL + "/connect/token",
-                headers=headers,
-                data={
-                    "client_id": "smartset.web",
-                    "code": code,
-                    "redirect_uri": constants.BASE_URL + "/signin-callback.html",
-                    "code_verifier": code_verifier,
-                    "grant_type": "authorization_code",
-                },
-            )
-                    
-            json = r.json()
-            _LOGGER.debug('Token response: %s', json)
-            if "error" in json:
+                    "Sec-Fetch-Site": "same-origin",
+                    "TE": "trailers"
+                }
+
+                # Get token
+                r = await client.post(
+                    constants.AUTHENTICATION_BASE_URL + "/connect/token",
+                    headers=headers,
+                    data={
+                        "client_id": "smartset.web",
+                        "code": code,
+                        "redirect_uri": constants.BASE_URL + "/signin-callback.html",
+                        "code_verifier": code_verifier,
+                        "grant_type": "authorization_code",
+                    },
+                )
+                        
+                json = r.json()
+                _LOGGER.debug('Token response: %s', json)
+                if "error" in json:
+                    raise InvalidAuth
+                _LOGGER.info('Successfully authenticated')
+                return Tokens(json.get("access_token"), json.get("expires_in"))
+            else:
                 raise InvalidAuth
-            # TODO: response doesn't actually include a refresh_token
-            _LOGGER.info('Successfully authenticated')
-            return Tokens(json.get("access_token"), json.get("refresh_token"), json.get("expires_in"))
         except:
             raise InvalidAuth
 
 class InvalidAuth(Exception):
     """Please check whether you entered an invalid username or password. If everything looks fine then probably there is an issue with Wolf SmartSet servers."""
     pass
```

### Comparing `wolf_comm-0.0.7/wolf_comm/wolf_client.py` & `wolf_comm-0.0.8/wolf_comm/wolf_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 class WolfClient:
     session_id: int or None
     tokens: Tokens or None
     last_access: datetime or None
     last_failed: bool
+    last_session_refesh: datetime or None
     
     
     @property
     def client(self):
         if hasattr(self, '_client') and self._client != None:
             return self._client
         elif hasattr(self, '_client_lambda') and self._client_lambda != None:
@@ -46,27 +47,31 @@
             self._client = httpx.AsyncClient()
         
         self.tokens = None
         self.token_auth = TokenAuth(username, password)
         self.session_id = None
         self.last_access = None
         self.last_failed = False
+        self.last_session_refesh = None
 
     async def __request(self, method: str, path: str, **kwargs) -> Union[dict, list]:
         if self.tokens is None or self.tokens.is_expired():
             await self.__authorize_and_session()
 
         headers = kwargs.get('headers')
 
         if headers is None:
             headers = bearer_header(self.tokens.access_token)
         else:
             headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
 
-        await update_session(self.client, self.tokens.access_token, self.session_id)
+        if self.last_session_refesh is None or self.last_session_refesh <= datetime.datetime.now():
+            await update_session(self.client, self.tokens.access_token, self.session_id)
+            self.last_session_refesh = datetime.datetime.now() + datetime.timedelta(seconds=60)
+            _LOGGER.debug('Sessionid: %s extented', self.session_id)
         
         resp = await self.__execute(headers, kwargs, method, path)
         if resp.status_code == 401 or resp.status_code == 500:
             _LOGGER.info('Retrying failed request (status code %d)',
                          resp.status_code)
             await self.__authorize_and_session()
             headers = {**bearer_header(self.tokens.access_token), **dict(headers)}
```

### Comparing `wolf_comm-0.0.7/wolf_comm.egg-info/PKG-INFO` & `wolf_comm-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: wolf-comm
-Version: 0.0.7
-Summary: A package to communicate with Wolf SmartSet Cloud
-Home-page: https://github.com/janrothkegel/wolf-comm
-Author: Jan Rothkegel
-Author-email: jan.rothkegel@web.de
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-## Library to handle Wolf SmartSet communication.
-
-### Features:
-- Built-in authentication
-- Session creation
-- Fetch all devices you have
-- Fetch all parameters description
-- Fetch value for specific parameter
-
-### Parameter descriptions
-Parameters verified only for FGB-28 system.
-Other should work.
-Keep in mind that core implementation of fetching parameters is removing duplications by value_id and name.
-
-
+Metadata-Version: 2.1
+Name: wolf_comm
+Version: 0.0.8
+Summary: A package to communicate with Wolf SmartSet Cloud
+Home-page: https://github.com/janrothkegel/wolf-comm
+Author: Jan Rothkegel
+Author-email: jan.rothkegel@web.de
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: httpx
+Requires-Dist: lxml
+Requires-Dist: pkce
+Requires-Dist: shortuuid
+
+## Library to handle Wolf SmartSet communication.
+
+### Features:
+- Built-in authentication
+- Session creation
+- Fetch all devices you have
+- Fetch all parameters description
+- Fetch value for specific parameter
+
+### Parameter descriptions
+Parameters verified only for FGB-28 system.
+Other should work.
+Keep in mind that core implementation of fetching parameters is removing duplications by value_id and name.
```

