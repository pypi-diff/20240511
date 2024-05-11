# Comparing `tmp/spnkr-0.7.0.tar.gz` & `tmp/spnkr-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spnkr-0.7.0.tar", last modified: Fri Apr 26 03:20:46 2024, max compression
+gzip compressed data, was "spnkr-0.8.0.tar", last modified: Sat May 11 19:12:05 2024, max compression
```

## Comparing `spnkr-0.7.0.tar` & `spnkr-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.545469 spnkr-0.7.0/
--rw-rw-rw-   0        0        0     1056 2023-08-17 20:38:12.000000 spnkr-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     3684 2024-04-26 03:20:46.544482 spnkr-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-12-07 02:48:08.000000 spnkr-0.7.0/README.md
--rw-rw-rw-   0        0        0     1023 2024-04-26 03:00:59.000000 spnkr-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 03:20:46.545469 spnkr-0.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.327065 spnkr-0.7.0/spnkr/
--rw-rw-rw-   0        0        0       64 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.417865 spnkr-0.7.0/spnkr/auth/
--rw-rw-rw-   0        0        0      389 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/__init__.py
--rw-rw-rw-   0        0        0      714 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/app.py
--rw-rw-rw-   0        0        0     2771 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/core.py
--rw-rw-rw-   0        0        0     2772 2023-12-01 18:09:06.000000 spnkr-0.7.0/spnkr/auth/halo.py
--rw-rw-rw-   0        0        0     3279 2024-04-26 03:13:49.000000 spnkr-0.7.0/spnkr/auth/oauth.py
--rw-rw-rw-   0        0        0     1051 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/player.py
--rw-rw-rw-   0        0        0     3446 2023-08-24 18:33:58.000000 spnkr-0.7.0/spnkr/auth/xbox.py
--rw-rw-rw-   0        0        0     2637 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/client.py
--rw-rw-rw-   0        0        0      450 2024-04-26 02:56:28.000000 spnkr-0.7.0/spnkr/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.484225 spnkr-0.7.0/spnkr/models/
--rw-rw-rw-   0        0        0       56 2023-12-07 02:48:08.000000 spnkr-0.7.0/spnkr/models/__init__.py
--rw-rw-rw-   0        0        0      908 2023-12-15 14:00:09.000000 spnkr-0.7.0/spnkr/models/base.py
--rw-rw-rw-   0        0        0    15383 2023-12-17 19:54:08.000000 spnkr-0.7.0/spnkr/models/discovery_ugc.py
--rw-rw-rw-   0        0        0     9696 2023-12-17 19:55:04.000000 spnkr-0.7.0/spnkr/models/gamecms_hacs.py
--rw-rw-rw-   0        0        0      711 2023-12-15 14:02:33.000000 spnkr-0.7.0/spnkr/models/profile.py
--rw-rw-rw-   0        0        0    10730 2024-04-26 02:31:17.000000 spnkr-0.7.0/spnkr/models/refdata.py
--rw-rw-rw-   0        0        0     5529 2024-02-23 18:26:14.000000 spnkr-0.7.0/spnkr/models/skill.py
--rw-rw-rw-   0        0        0    26305 2024-02-23 18:26:14.000000 spnkr-0.7.0/spnkr/models/stats.py
--rw-rw-rw-   0        0        0      932 2023-12-17 19:53:12.000000 spnkr-0.7.0/spnkr/models/types.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.540465 spnkr-0.7.0/spnkr/services/
--rw-rw-rw-   0        0        0      499 2023-12-04 03:29:58.000000 spnkr-0.7.0/spnkr/services/__init__.py
--rw-rw-rw-   0        0        0     2213 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/services/base.py
--rw-rw-rw-   0        0        0     7711 2023-12-27 20:34:37.000000 spnkr-0.7.0/spnkr/services/discovery_ugc.py
--rw-rw-rw-   0        0        0     2455 2023-12-21 01:58:28.000000 spnkr-0.7.0/spnkr/services/gamecms_hacs.py
--rw-rw-rw-   0        0        0     1944 2023-12-21 01:58:28.000000 spnkr-0.7.0/spnkr/services/profile.py
--rw-rw-rw-   0        0        0     3099 2023-12-21 19:48:37.000000 spnkr-0.7.0/spnkr/services/skill.py
--rw-rw-rw-   0        0        0     6856 2023-12-21 19:48:37.000000 spnkr-0.7.0/spnkr/services/stats.py
--rw-rw-rw-   0        0        0      942 2024-01-03 04:20:45.000000 spnkr-0.7.0/spnkr/session.py
--rw-rw-rw-   0        0        0     5335 2023-12-07 02:48:08.000000 spnkr-0.7.0/spnkr/tools.py
--rw-rw-rw-   0        0        0     2434 2023-12-01 03:28:26.000000 spnkr-0.7.0/spnkr/xuid.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:20:46.542463 spnkr-0.7.0/spnkr.egg-info/
--rw-rw-rw-   0        0        0     3684 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 03:20:46.000000 spnkr-0.7.0/spnkr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.460912 spnkr-0.8.0/
+-rw-rw-rw-   0        0        0     1056 2023-08-17 20:38:12.000000 spnkr-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3684 2024-05-11 19:12:05.459913 spnkr-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-12-07 02:48:08.000000 spnkr-0.8.0/README.md
+-rw-rw-rw-   0        0        0     1023 2024-05-11 19:09:33.000000 spnkr-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 19:12:05.460912 spnkr-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.408458 spnkr-0.8.0/spnkr/
+-rw-rw-rw-   0        0        0      308 2024-05-11 18:46:00.000000 spnkr-0.8.0/spnkr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.439544 spnkr-0.8.0/spnkr/auth/
+-rw-rw-rw-   0        0        0      429 2024-05-03 02:47:07.000000 spnkr-0.8.0/spnkr/auth/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-08-24 18:33:58.000000 spnkr-0.8.0/spnkr/auth/app.py
+-rw-rw-rw-   0        0        0     2780 2024-05-03 02:47:22.000000 spnkr-0.8.0/spnkr/auth/core.py
+-rw-rw-rw-   0        0        0     2772 2023-12-01 18:09:06.000000 spnkr-0.8.0/spnkr/auth/halo.py
+-rw-rw-rw-   0        0        0     3279 2024-04-26 03:13:49.000000 spnkr-0.8.0/spnkr/auth/oauth.py
+-rw-rw-rw-   0        0        0     1061 2024-05-03 02:47:36.000000 spnkr-0.8.0/spnkr/auth/player.py
+-rw-rw-rw-   0        0        0     3450 2024-05-03 02:47:48.000000 spnkr-0.8.0/spnkr/auth/xbox.py
+-rw-rw-rw-   0        0        0     3508 2024-05-10 17:49:53.000000 spnkr-0.8.0/spnkr/client.py
+-rw-rw-rw-   0        0        0      450 2024-04-26 02:56:28.000000 spnkr-0.8.0/spnkr/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.449544 spnkr-0.8.0/spnkr/models/
+-rw-rw-rw-   0        0        0       56 2023-12-07 02:48:08.000000 spnkr-0.8.0/spnkr/models/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-12-15 14:00:09.000000 spnkr-0.8.0/spnkr/models/base.py
+-rw-rw-rw-   0        0        0    15419 2024-05-03 02:48:19.000000 spnkr-0.8.0/spnkr/models/discovery_ugc.py
+-rw-rw-rw-   0        0        0     3994 2024-05-03 02:55:26.000000 spnkr-0.8.0/spnkr/models/economy.py
+-rw-rw-rw-   0        0        0     9732 2024-05-03 02:48:48.000000 spnkr-0.8.0/spnkr/models/gamecms_hacs.py
+-rw-rw-rw-   0        0        0      711 2023-12-15 14:02:33.000000 spnkr-0.8.0/spnkr/models/profile.py
+-rw-rw-rw-   0        0        0    10730 2024-04-26 02:31:17.000000 spnkr-0.8.0/spnkr/models/refdata.py
+-rw-rw-rw-   0        0        0     5565 2024-05-03 02:49:06.000000 spnkr-0.8.0/spnkr/models/skill.py
+-rw-rw-rw-   0        0        0    26329 2024-05-03 02:49:17.000000 spnkr-0.8.0/spnkr/models/stats.py
+-rw-rw-rw-   0        0        0      932 2023-12-17 19:53:12.000000 spnkr-0.8.0/spnkr/models/types.py
+-rw-rw-rw-   0        0        0     1559 2024-05-11 19:06:53.000000 spnkr-0.8.0/spnkr/responses.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.456544 spnkr-0.8.0/spnkr/services/
+-rw-rw-rw-   0        0        0      643 2024-05-03 02:49:35.000000 spnkr-0.8.0/spnkr/services/__init__.py
+-rw-rw-rw-   0        0        0     1888 2024-05-03 04:52:18.000000 spnkr-0.8.0/spnkr/services/base.py
+-rw-rw-rw-   0        0        0     8073 2024-05-03 04:21:09.000000 spnkr-0.8.0/spnkr/services/discovery_ugc.py
+-rw-rw-rw-   0        0        0     1352 2024-05-03 04:32:29.000000 spnkr-0.8.0/spnkr/services/economy.py
+-rw-rw-rw-   0        0        0     2799 2024-05-03 04:39:19.000000 spnkr-0.8.0/spnkr/services/gamecms_hacs.py
+-rw-rw-rw-   0        0        0     2125 2024-05-03 04:45:54.000000 spnkr-0.8.0/spnkr/services/profile.py
+-rw-rw-rw-   0        0        0     3289 2024-05-03 04:48:29.000000 spnkr-0.8.0/spnkr/services/skill.py
+-rw-rw-rw-   0        0        0     7234 2024-05-03 04:51:52.000000 spnkr-0.8.0/spnkr/services/stats.py
+-rw-rw-rw-   0        0        0     5345 2024-05-03 02:52:24.000000 spnkr-0.8.0/spnkr/tools.py
+-rw-rw-rw-   0        0        0     2439 2024-05-03 02:52:29.000000 spnkr-0.8.0/spnkr/xuid.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:12:05.458599 spnkr-0.8.0/spnkr.egg-info/
+-rw-rw-rw-   0        0        0     3684 2024-05-11 19:12:05.000000 spnkr-0.8.0/spnkr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-11 19:12:05.000000 spnkr-0.8.0/spnkr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 19:12:05.000000 spnkr-0.8.0/spnkr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-05-11 19:12:05.000000 spnkr-0.8.0/spnkr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 19:12:05.000000 spnkr-0.8.0/spnkr.egg-info/top_level.txt
```

### Comparing `spnkr-0.7.0/LICENSE` & `spnkr-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/PKG-INFO` & `spnkr-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spnkr
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API for retrieving Halo Infinite multiplayer data.
 Author: Andy Curtis
 License: Copyright 2022 Andy Curtis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `spnkr-0.7.0/README.md` & `spnkr-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/pyproject.toml` & `spnkr-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'spnkr'
-version = '0.7.0'
+version = '0.8.0'
 description = 'Python API for retrieving Halo Infinite multiplayer data.'
 readme = 'README.md'
 authors = [{ name = 'Andy Curtis' }]
 license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
```

### Comparing `spnkr-0.7.0/spnkr/auth/app.py` & `spnkr-0.8.0/spnkr/auth/app.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/auth/core.py` & `spnkr-0.8.0/spnkr/auth/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Authenticate with services necessary for Halo Infinite API access."""
 
 from aiohttp import ClientSession
 
-from . import app, halo, oauth, player, xbox
+from spnkr.auth import app, halo, oauth, player, xbox
 
 XSTS_V3_XBOX_AUDIENCE = "http://xboxlive.com"
 XSTS_V3_HALO_AUDIENCE = "https://prod.xsts.halowaypoint.com/"
 
 
 async def authenticate_player(session: ClientSession, app: app.AzureApp) -> str:
     """Initial authentication of the `app` with Windows Live and Xbox Live.
```

### Comparing `spnkr-0.7.0/spnkr/auth/halo.py` & `spnkr-0.8.0/spnkr/auth/halo.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/auth/oauth.py` & `spnkr-0.8.0/spnkr/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/auth/player.py` & `spnkr-0.8.0/spnkr/auth/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Information about an authenticated player."""
 
 import datetime as dt
 from dataclasses import dataclass
 
-from .halo import ClearanceToken, SpartanToken
+from spnkr.auth.halo import ClearanceToken, SpartanToken
 
 
 @dataclass(frozen=True)
 class AuthenticatedPlayer:
     """Information about an authenticated player.
 
     Attributes:
```

### Comparing `spnkr-0.7.0/spnkr/auth/xbox.py` & `spnkr-0.8.0/spnkr/auth/xbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Xbox Live authentication."""
 
 from dataclasses import dataclass
 from typing import Any
 
 from aiohttp import ClientSession
 
-from ..xuid import wrap_xuid
+from spnkr.xuid import wrap_xuid
 
 
 @dataclass(frozen=True)
 class XAUResponse:
     """Represents the response from an Xbox user request.
 
     Attributes:
```

### Comparing `spnkr-0.7.0/spnkr/client.py` & `spnkr-0.8.0/spnkr/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 """Provides a client for the Halo Infinite API."""
 
 from functools import cached_property
+from typing import TYPE_CHECKING
 
-from .services import (
+if TYPE_CHECKING:
+    from aiohttp import ClientSession
+    from aiohttp_client_cache.session import CachedSession
+
+from spnkr.services import (
     DiscoveryUgcService,
+    EconomyService,
     GameCmsHacsService,
     ProfileService,
     SkillService,
     StatsService,
 )
-from .session import Session
 
 __all__ = ["HaloInfiniteClient"]
 
 
 class HaloInfiniteClient:
     """A client for the Halo Infinite API."""
 
     def __init__(
         self,
-        session: Session,
+        session: "ClientSession | CachedSession",
         spartan_token: str,
         clearance_token: str,
         requests_per_second: int | None = 5,
     ) -> None:
         """Initialize a client for the Halo Infinite API.
 
         Args:
             session: The `aiohttp.ClientSession` to use. Support for caching is
                 available via a `CachedSession` from `aiohttp-client-cache`.
             spartan_token: The spartan token used to authenticate with the API.
-            clearance_token: The clearance token used to authenticate with the
-                API.
+            clearance_token: The clearance token used to authenticate with the API.
             requests_per_second: The rate limit to use. Note that this rate
                 limit is enforced per service, not globally. Defaults to 5
                 requests per second. Set to None to disable rate limiting.
         """
-        session.headers.clear()
-        session.headers["Accept"] = "application/json"
-        session.headers["x-343-authorization-spartan"] = spartan_token
-        session.headers["343-clearance"] = clearance_token
         self._session = session
         self._requests_per_second = requests_per_second
+        self.set_tokens(spartan_token, clearance_token)
+
+    def set_tokens(self, spartan_token: str, clearance_token: str) -> None:
+        """Update the tokens used for authentication.
+
+        This method is called during initialization, but can be used after
+        initialization to replace expiring tokens.
+
+        Args:
+            spartan_token: The spartan token used to authenticate with the API.
+            clearance_token: The clearance token used to authenticate with the API.
+        """
+        update = {
+            "Accept": "application/json",
+            "x-343-authorization-spartan": spartan_token,
+            "343-clearance": clearance_token,
+        }
+        self._session.headers.update(update)
 
     @cached_property
     def profile(self) -> ProfileService:
         """Profile data service. Get user data, such as XUIDs/gamertags."""
         return ProfileService(self._session, self._requests_per_second)
 
     @cached_property
@@ -63,7 +81,12 @@
         """Stats data service. Retrieve match history and match stats."""
         return StatsService(self._session, self._requests_per_second)
 
     @cached_property
     def discovery_ugc(self) -> DiscoveryUgcService:
         """User-generated content discovery data service (maps, modes, etc.)."""
         return DiscoveryUgcService(self._session, self._requests_per_second)
+
+    @cached_property
+    def economy(self) -> EconomyService:
+        """Store and customization data service."""
+        return EconomyService(self._session, self._requests_per_second)
```

### Comparing `spnkr-0.7.0/spnkr/models/base.py` & `spnkr-0.8.0/spnkr/models/base.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/models/discovery_ugc.py` & `spnkr-0.8.0/spnkr/models/discovery_ugc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import datetime as dt
 import urllib.parse
 from typing import Any
 from uuid import UUID
 
 from pydantic import Field
 
-from .base import PascalCaseModel
-from .refdata import (
+from spnkr.models.base import PascalCaseModel
+from spnkr.models.refdata import (
     AssetHome,
     AssetKind,
     CloneBehavior,
     FilmChunkType,
     FilmStatus,
     InspectionResult,
     PlaylistBotDifficulty,
     PlaylistDeviceInput,
     PlaylistEntrySelectionStrategy,
 )
-from .types import ReadOnlyDict
+from spnkr.models.types import ReadOnlyDict
 
 
 class OnlineUriReference(PascalCaseModel, frozen=True):
     """A reference to an online resource.
 
     Attributes:
         authority_id: The ID of the authority that hosts the resource.
```

### Comparing `spnkr-0.7.0/spnkr/models/gamecms_hacs.py` & `spnkr-0.8.0/spnkr/models/gamecms_hacs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Models for the "gamecms_hacs" authority."""
 
 import datetime as dt
 
 from pydantic import Field
 
-from .base import CamelCaseModel, PascalCaseModel
-from .refdata import MedalDifficulty, MedalType
-from .types import ReadOnlyDict
+from spnkr.models.base import CamelCaseModel, PascalCaseModel
+from spnkr.models.refdata import MedalDifficulty, MedalType
+from spnkr.models.types import ReadOnlyDict
 
 
 class TranslatableString(CamelCaseModel, frozen=True):
     """A string value accompanied by a dictionary of translations.
 
     Attributes:
         value: The string value.
```

### Comparing `spnkr-0.7.0/spnkr/models/profile.py` & `spnkr-0.8.0/spnkr/models/profile.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/models/refdata.py` & `spnkr-0.8.0/spnkr/models/refdata.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/models/skill.py` & `spnkr-0.8.0/spnkr/models/skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Models for the "skill" authority."""
 
 from uuid import UUID
 
-from .base import PascalCaseModel
-from .refdata import SkillResultCode, SubTier, Tier
-from .types import ReadOnlyDict
+from spnkr.models.base import PascalCaseModel
+from spnkr.models.refdata import SkillResultCode, SubTier, Tier
+from spnkr.models.types import ReadOnlyDict
 
 
 class CsrContainer(PascalCaseModel, frozen=True):
     """Container for a player's CSR info.
 
     Attributes:
         value: The player's CSR value.
```

### Comparing `spnkr-0.7.0/spnkr/models/stats.py` & `spnkr-0.8.0/spnkr/models/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Models for the stats authority."""
 
 import datetime as dt
 from uuid import UUID
 
 from pydantic import Field
 
-from .base import PascalCaseModel
-from .refdata import (
+from spnkr.models.base import PascalCaseModel
+from spnkr.models.refdata import (
     AssetKind,
     BotDifficulty,
     GameVariantCategory,
     LifecycleMode,
     Outcome,
     PlayerType,
     PlaylistExperience,
```

### Comparing `spnkr-0.7.0/spnkr/models/types.py` & `spnkr-0.8.0/spnkr/models/types.py`

 * *Files identical despite different names*

### Comparing `spnkr-0.7.0/spnkr/services/base.py` & `spnkr-0.8.0/spnkr/services/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Base service class."""
 
-from typing import Any
+from typing import TYPE_CHECKING, TypeAlias
 
 from aiolimiter import AsyncLimiter
 
-try:
+if TYPE_CHECKING:
+    from aiohttp import ClientResponse, ClientSession
     from aiohttp_client_cache.response import CachedResponse
-except ImportError:
-    CachedResponse = None
+    from aiohttp_client_cache.session import CachedSession
 
-from ..session import Response, Session
+Response: TypeAlias = "ClientResponse | CachedResponse"
+Session: TypeAlias = "ClientSession | CachedSession"
 
 
 def _create_limiter(rate_per_second: int) -> AsyncLimiter:
     """Return an AsyncLimiter with the given rate per second."""
     # Setting the max rate to 1 disallows bursts.
     return AsyncLimiter(1, 1 / rate_per_second)
 
 
 def _is_cached_response(response: Response) -> bool:
     """Return `True` if the response is a cached response."""
-    return CachedResponse is not None and isinstance(response, CachedResponse)
+    return hasattr(response, "from_cache")
 
 
 class BaseService:
     """Base service class. Handles initialization and rate limiting requests."""
 
     def __init__(
         self, session: Session, requests_per_second: int | None = 5
@@ -45,17 +46,7 @@
         """Make a GET request to `url` and return the response."""
         response = await self._session.get(url, **kwargs)
         if not _is_cached_response(response) and self._rate_limiter is not None:
             # Only rate limit non-cached responses.
             await self._rate_limiter.acquire()
         response.raise_for_status()
         return response
-
-    async def _get_json(self, url: str, **kwargs) -> Any:
-        """Make a GET request to `url` and return the decoded JSON response."""
-        response = await self._get(url, **kwargs)
-        return await response.json()
-
-    async def _get_bytes(self, url: str, **kwargs) -> bytes:
-        """Make a GET request to `url` and return the response content."""
-        response = await self._get(url, **kwargs)
-        return await response.read()
```

### Comparing `spnkr-0.7.0/spnkr/services/discovery_ugc.py` & `spnkr-0.8.0/spnkr/services/discovery_ugc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """User-generated content discovery data services."""
 
 import datetime as dt
-from typing import Any, Iterable, Literal
+from typing import Iterable, Literal
 from uuid import UUID
 
-from ..models.discovery_ugc import (
+from spnkr.models.discovery_ugc import (
     AssetSearchPage,
     Film,
     Map,
     MapModePair,
     Playlist,
     UgcGameVariant,
 )
-from .base import BaseService
+from spnkr.responses import JsonResponse
+from spnkr.services.base import BaseService
 
 _HOST = "https://discovery-infiniteugc.svc.halowaypoint.com:443"
 _SortProperty = Literal[
     "name",
     "likes",
     "bookmarks",
     "plays_recent",
@@ -32,77 +33,77 @@
 
 
 class DiscoveryUgcService(BaseService):
     """User-generated content discovery data services."""
 
     async def _get_asset(
         self, asset_type: str, asset_id: str | UUID, version_id: str | UUID
-    ) -> dict[str, Any]:
+    ):
         url = f"{_HOST}/hi/{asset_type}/{asset_id}/versions/{version_id}"
-        return await self._get_json(url)
+        return await self._get(url)
 
     async def get_ugc_game_variant(
         self, asset_id: str | UUID, version_id: str | UUID
-    ) -> UgcGameVariant:
+    ) -> JsonResponse[UgcGameVariant]:
         """Get details about a game mode.
 
         Args:
             asset_id: The asset ID of the game variant.
             version_id: The version ID of the game variant.
 
         Returns:
             The game variant details.
         """
-        data = await self._get_asset("ugcGameVariants", asset_id, version_id)
-        return UgcGameVariant(**data)
+        resp = await self._get_asset("ugcGameVariants", asset_id, version_id)
+        return JsonResponse(resp, lambda data: UgcGameVariant(**data))
 
     async def get_map_mode_pair(
         self, asset_id: str | UUID, version_id: str | UUID
-    ) -> MapModePair:
+    ) -> JsonResponse[MapModePair]:
         """Get details about a map mode pair.
 
         Args:
             asset_id: The asset ID of the map mode pair.
             version_id: The version ID of the map mode pair.
 
         Returns:
             The map mode pair details.
         """
-        data = await self._get_asset("mapModePairs", asset_id, version_id)
-        return MapModePair(**data)
+        resp = await self._get_asset("mapModePairs", asset_id, version_id)
+        return JsonResponse(resp, lambda data: MapModePair(**data))
 
     async def get_map(
         self, asset_id: str | UUID, version_id: str | UUID
-    ) -> Map:
+    ) -> JsonResponse[Map]:
         """Get details about a map.
 
         Args:
             asset_id: The asset ID of the map.
             version_id: The version ID of the map.
 
         Returns:
             The map details.
         """
-        data = await self._get_asset("maps", asset_id, version_id)
-        return Map(**data)
+        resp = await self._get_asset("maps", asset_id, version_id)
+        return JsonResponse(resp, lambda data: Map(**data))
 
     async def get_playlist(
         self, asset_id: str | UUID, version_id: str | UUID
-    ) -> Playlist:
+    ) -> JsonResponse[Playlist]:
         """Get details about a playlist.
 
         Args:
             asset_id: The asset ID of the playlist.
             version_id: The version ID of the playlist.
 
         Returns:
             The playlist details.
         """
-        data = await self._get_asset("playlists", asset_id, version_id)
-        return Playlist(**data)
+        resp = await self._get_asset("playlists", asset_id, version_id)
+        return JsonResponse(resp, lambda data: Playlist(**data))
 
     async def search_assets(
         self,
         start: int = 0,
         count: int = 25,
         sort: _SortProperty = "plays_recent",
         order: Literal["asc", "desc"] = "desc",
@@ -113,15 +114,15 @@
         average_rating_min: float | None = None,
         from_date_created_utc: dt.datetime | dt.date | None = None,
         to_date_created_utc: dt.datetime | dt.date | None = None,
         from_date_modified_utc: dt.datetime | dt.date | None = None,
         to_date_modified_utc: dt.datetime | dt.date | None = None,
         from_date_published_utc: dt.datetime | dt.date | None = None,
         to_date_published_utc: dt.datetime | dt.date | None = None,
-    ) -> AssetSearchPage:
+    ) -> JsonResponse[AssetSearchPage]:
         """Search for map, mode, and prefab assets.
 
         Args:
             start: Index of the first result to return, starting at 0.
             count: Count of results to return. Must be between 1 and 101.
             sort: Property by which to sort the results. Must be one of the
                 following: "name", "likes", "bookmarks", "plays_recent",
@@ -179,20 +180,24 @@
             params["fromDateModifiedUtc"] = from_date_modified_utc.isoformat()
         if to_date_modified_utc is not None:
             params["toDateModifiedUtc"] = to_date_modified_utc.isoformat()
         if from_date_published_utc is not None:
             params["fromDatePublishedUtc"] = from_date_published_utc.isoformat()
         if to_date_published_utc is not None:
             params["toDatePublishedUtc"] = to_date_published_utc.isoformat()
-        return AssetSearchPage(**await self._get_json(url, params=params))
+        resp = await self._get(url, params=params)
+        return JsonResponse(resp, lambda data: AssetSearchPage(**data))
 
-    async def get_film_by_match_id(self, match_id: str | UUID) -> Film:
+    async def get_film_by_match_id(
+        self, match_id: str | UUID
+    ) -> JsonResponse[Film]:
         """Get metadata and download information for a film.
 
         Args:
             match_id: The match ID of the film.
 
         Returns:
             The film details.
         """
         url = f"{_HOST}/hi/films/matches/{match_id}/spectate"
-        return Film(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: Film(**data))
```

### Comparing `spnkr-0.7.0/spnkr/services/gamecms_hacs.py` & `spnkr-0.8.0/spnkr/services/gamecms_hacs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 """Game content management data services."""
 
-from ..models.gamecms_hacs import (
+from spnkr.models.gamecms_hacs import (
     CareerRewardTrack,
     CsrSeasonCalendar,
     MedalMetadata,
     SeasonCalendar,
 )
-from .base import BaseService
+from spnkr.responses import ImageResponse, JsonResponse
+from spnkr.services.base import BaseService
 
 _HOST = "https://gamecms-hacs.svc.halowaypoint.com"
 
 
 class GameCmsHacsService(BaseService):
     """Game content management data services."""
 
-    async def get_medal_metadata(self) -> MedalMetadata:
+    async def get_medal_metadata(self) -> JsonResponse[MedalMetadata]:
         """Get details for all medals obtainable in the game.
 
         Returns:
             The medal metadata.
         """
         url = f"{_HOST}/hi/Waypoint/file/medals/metadata.json"
-        return MedalMetadata(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: MedalMetadata(**data))
 
-    async def get_csr_season_calendar(self) -> CsrSeasonCalendar:
+    async def get_csr_season_calendar(self) -> JsonResponse[CsrSeasonCalendar]:
         """Get IDs and dates for past and current CSR seasons.
 
         CSR seasons represent the time periods between CSR resets.
 
         Returns:
             The CSR season calendar.
         """
         url = (
             f"{_HOST}/hi/Progression/file/Csr/Calendars/CsrSeasonCalendar.json"
         )
-        return CsrSeasonCalendar(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: CsrSeasonCalendar(**data))
 
-    async def get_season_calendar(self) -> SeasonCalendar:
+    async def get_season_calendar(self) -> JsonResponse[SeasonCalendar]:
         """Get IDs and dates for past/current reward track events/operations.
 
         Reward tracks are the progression systems that allow players to earn
         rewards from the XP earned by playing the game.
 
         Returns:
             The calendar of reward tracks.
         """
         url = (
             f"{_HOST}/hi/progression/file/calendars/seasons/seasoncalendar.json"
         )
-        return SeasonCalendar(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: SeasonCalendar(**data))
 
-    async def get_career_reward_track(self) -> CareerRewardTrack:
+    async def get_career_reward_track(self) -> JsonResponse[CareerRewardTrack]:
         """Get details for the career rank progression reward track.
 
         Returns:
             The career rank reward track.
         """
         url = f"{_HOST}/hi/Progression/file/RewardTracks/CareerRanks/careerRank1.json"
-        return CareerRewardTrack(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: CareerRewardTrack(**data))
 
-    async def get_image(self, relative_path: str) -> bytes:
+    async def get_image(self, relative_path: str) -> ImageResponse:
         """Get an image from the game content management service.
 
         Args:
             relative_path: The relative path to the image, such as
                 "career_rank/ProgressWidget/272_Hero.png".
 
         Returns:
             The image data.
         """
         url = f"{_HOST}/hi/images/file/{relative_path.lstrip('/')}"
-        return await self._get_bytes(url)
+        return ImageResponse(await self._get(url))
```

### Comparing `spnkr-0.7.0/spnkr/services/skill.py` & `spnkr-0.8.0/spnkr/services/skill.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Skill data services."""
 
 from pathlib import Path
 from typing import Iterable
 from uuid import UUID
 
-from ..models.skill import MatchSkill, PlaylistCsr
-from ..xuid import wrap_xuid
-from .base import BaseService
+from spnkr.models.skill import MatchSkill, PlaylistCsr
+from spnkr.responses import JsonResponse
+from spnkr.services.base import BaseService
+from spnkr.xuid import wrap_xuid
 
 _HOST = "https://skill.svc.halowaypoint.com:443"
 
 
 class SkillService(BaseService):
     """Skill data services."""
 
     async def get_match_skill(
         self, match_id: str | UUID, xuids: Iterable[str | int]
-    ) -> MatchSkill:
+    ) -> JsonResponse[MatchSkill]:
         """Get player CSR and team MMR values for a given match and player list.
 
         Args:
             match_id: Halo Infinite match ID.
             xuids: The Xbox Live IDs of the match's players. Only
                 players in this list will have their skill data returned.
 
@@ -33,22 +34,23 @@
         """
         if isinstance(xuids, str):
             raise TypeError("`xuids` must be an iterable of XUIDs, got `str`")
         if not xuids:
             raise ValueError("`xuids` cannot be empty")
         url = f"{_HOST}/hi/matches/{match_id}/skill"
         params = {"players": [wrap_xuid(x) for x in xuids]}
-        return MatchSkill(**await self._get_json(url, params=params))
+        resp = await self._get(url, params=params)
+        return JsonResponse(resp, lambda data: MatchSkill(**data))
 
     async def get_playlist_csr(
         self,
         playlist_id: str | UUID,
         xuids: Iterable[str | int],
         season_id: str | None = None,
-    ) -> PlaylistCsr:
+    ) -> JsonResponse[PlaylistCsr]:
         """Get player CSR values for a given playlist and player list.
 
         Args:
             playlist_id: Halo Infinite playlist asset ID.
             xuids: The Xbox Live IDs of the players.
             season_id: Halo Infinite season ID. If not provided, the
                 current season will be used. Value can be provided as a path,
@@ -67,15 +69,16 @@
             raise TypeError("`xuids` must be an iterable of XUIDs, got `str`")
         if not xuids:
             raise ValueError("`xuids` cannot be empty")
         url = f"{_HOST}/hi/playlist/{playlist_id}/csrs"
         params: dict = {"players": [wrap_xuid(x) for x in xuids]}
         if season_id:
             params["season"] = _clean_season_id(season_id)
-        return PlaylistCsr(**await self._get_json(url, params=params))
+        resp = await self._get(url, params=params)
+        return JsonResponse(resp, lambda data: PlaylistCsr(**data))
 
 
 def _clean_season_id(season_id: str) -> str:
     """Remove the path prefix and ".json" extension from a season ID.
 
     For example, season "Csr/Seasons/CsrSeason5-1.json" is cleaned to
     "CsrSeason5-1".
```

### Comparing `spnkr-0.7.0/spnkr/services/stats.py` & `spnkr-0.8.0/spnkr/services/stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """Stats data services."""
 
 import warnings
 from typing import Literal
 from uuid import UUID
 
-from ..models.refdata import GameVariantCategory
-from ..models.stats import MatchCount, MatchHistory, MatchStats, ServiceRecord
-from ..xuid import wrap_xuid_or_gamertag
-from .base import BaseService
+from spnkr.models.refdata import GameVariantCategory
+from spnkr.models.stats import (
+    MatchCount,
+    MatchHistory,
+    MatchStats,
+    ServiceRecord,
+)
+from spnkr.responses import JsonResponse
+from spnkr.services.base import BaseService
+from spnkr.xuid import wrap_xuid_or_gamertag
 
 _HOST = "https://halostats.svc.halowaypoint.com:443"
 _VALID_SERVICE_RECORD_FILTER_SETS = [
     {"season_id"},
     {"season_id", "game_variant_category"},
     {"season_id", "game_variant_category", "playlist_asset_id"},
     {"season_id", "game_variant_category", "is_ranked"},
@@ -20,15 +26,17 @@
     {"game_variant_category", "is_ranked"},
 ]
 
 
 class StatsService(BaseService):
     """Stats data services."""
 
-    async def get_match_count(self, player: str | int) -> MatchCount:
+    async def get_match_count(
+        self, player: str | int
+    ) -> JsonResponse[MatchCount]:
         """Get match counts across different game experiences for a player.
 
         The counts returned are for custom matches, matchmade matches, local
         matches, and total matches.
 
         Args:
             player: Xbox Live ID or gamertag of the player to get counts for.
@@ -36,25 +44,26 @@
                 "1234567890123456", 1234567890123456, and "MyGamertag".
 
         Returns:
             The match counts.
         """
         xuid_or_gamertag = wrap_xuid_or_gamertag(player)
         url = f"{_HOST}/hi/players/{xuid_or_gamertag}/matches/count"
-        return MatchCount(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: MatchCount(**data))
 
     async def get_service_record(
         self,
         player: str | int,
         match_type: Literal["matchmade", "custom", "local"] = "matchmade",
         season_id: str | None = None,
         game_variant_category: GameVariantCategory | int | None = None,
         is_ranked: bool | None = None,
         playlist_asset_id: str | UUID | None = None,
-    ) -> ServiceRecord:
+    ) -> JsonResponse[ServiceRecord]:
         """Get a service record for a player. Summarizes player stats.
 
         Note that filters (`season_id`, `game_variant_category`, `is_ranked`,
         and `playlist_asset_id`) are only applicable to "matchmade"
         `match_type`. A warning is issued and the filters are ignored if they
         are provided for a non-matchmade `match_type`.
 
@@ -111,23 +120,24 @@
             filters = {}
         if filters and set(filters) not in _VALID_SERVICE_RECORD_FILTER_SETS:
             valid = "\n".join(str(s) for s in _VALID_SERVICE_RECORD_FILTER_SETS)
             raise ValueError(
                 f"Invalid filter combination: {filters}. Options:\n{valid}"
             )
         params = {k.replace("_", ""): str(v) for k, v in filters.items()}
-        return ServiceRecord(**await self._get_json(url, params=params))
+        resp = await self._get(url, params=params)
+        return JsonResponse(resp, lambda data: ServiceRecord(**data))
 
     async def get_match_history(
         self,
         player: str | int,
         start: int = 0,
         count: int = 25,
         match_type: Literal["all", "matchmaking", "custom", "local"] = "all",
-    ) -> MatchHistory:
+    ) -> JsonResponse[MatchHistory]:
         """Request a batch of matches from a player's match history.
 
         Args:
             player: Xbox Live ID or gamertag of the player to get counts for.
                 Examples of valid inputs include "xuid(1234567890123456)",
                 "1234567890123456", 1234567890123456, and "MyGamertag".
             start: Index of the first match to request, starting at 0.
@@ -138,20 +148,24 @@
 
         Returns:
             The requested match history "page" of results.
         """
         xuid_or_gamertag = wrap_xuid_or_gamertag(player)
         url = f"{_HOST}/hi/players/{xuid_or_gamertag}/matches"
         params = {"start": start, "count": count, "type": match_type}
-        return MatchHistory(**await self._get_json(url, params=params))
+        resp = await self._get(url, params=params)
+        return JsonResponse(resp, lambda data: MatchHistory(**data))
 
-    async def get_match_stats(self, match_id: str | UUID) -> MatchStats:
+    async def get_match_stats(
+        self, match_id: str | UUID
+    ) -> JsonResponse[MatchStats]:
         """Request match details using the Halo Infinite match GUID.
 
         Args:
             match_id: Halo Infinite GUID identifying the match.
 
         Returns:
             The match details.
         """
         url = f"{_HOST}/hi/matches/{match_id}/stats"
-        return MatchStats(**await self._get_json(url))
+        resp = await self._get(url)
+        return JsonResponse(resp, lambda data: MatchStats(**data))
```

### Comparing `spnkr-0.7.0/spnkr/tools.py` & `spnkr-0.8.0/spnkr/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Tools for Halo Infinite data analysis."""
 
 import math
 from enum import IntEnum
 from typing import NamedTuple
 
-from .models.refdata import (
+from spnkr.models.refdata import (
     BotDifficulty,
     GameVariantCategory,
     LifecycleMode,
     MedalDifficulty,
     MedalType,
     Outcome,
     PlayerType,
     PlaylistExperience,
     SubTier,
     Tier,
 )
-from .xuid import unwrap_xuid, wrap_xuid
+from spnkr.xuid import unwrap_xuid, wrap_xuid
 
 __all__ = [
     "wrap_xuid",
     "unwrap_xuid",
     "BOT_DIFFICULTY_MAP",
     "BOT_MAP",
     "GAME_CATEGORY_MAP",
```

### Comparing `spnkr-0.7.0/spnkr/xuid.py` & `spnkr-0.8.0/spnkr/xuid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Convert Xbox Live IDs (XUID) to and from strings and integers."""
 
 import math
 import re
 
-from .errors import InvalidXuidError
+from spnkr.errors import InvalidXuidError
 
 _XUID_PATTERN = re.compile(r"^xuid\((\d{16})\)$")
 
 
 def wrap_xuid(xuid: str | int) -> str:
     """Wrap an Xbox Live ID in the "xuid()" format.
```

### Comparing `spnkr-0.7.0/spnkr.egg-info/PKG-INFO` & `spnkr-0.8.0/spnkr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spnkr
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API for retrieving Halo Infinite multiplayer data.
 Author: Andy Curtis
 License: Copyright 2022 Andy Curtis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `spnkr-0.7.0/spnkr.egg-info/SOURCES.txt` & `spnkr-0.8.0/spnkr.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 spnkr/__init__.py
 spnkr/client.py
 spnkr/errors.py
-spnkr/session.py
+spnkr/responses.py
 spnkr/tools.py
 spnkr/xuid.py
 spnkr.egg-info/PKG-INFO
 spnkr.egg-info/SOURCES.txt
 spnkr.egg-info/dependency_links.txt
 spnkr.egg-info/requires.txt
 spnkr.egg-info/top_level.txt
@@ -18,20 +18,22 @@
 spnkr/auth/halo.py
 spnkr/auth/oauth.py
 spnkr/auth/player.py
 spnkr/auth/xbox.py
 spnkr/models/__init__.py
 spnkr/models/base.py
 spnkr/models/discovery_ugc.py
+spnkr/models/economy.py
 spnkr/models/gamecms_hacs.py
 spnkr/models/profile.py
 spnkr/models/refdata.py
 spnkr/models/skill.py
 spnkr/models/stats.py
 spnkr/models/types.py
 spnkr/services/__init__.py
 spnkr/services/base.py
 spnkr/services/discovery_ugc.py
+spnkr/services/economy.py
 spnkr/services/gamecms_hacs.py
 spnkr/services/profile.py
 spnkr/services/skill.py
 spnkr/services/stats.py
```

