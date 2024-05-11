# Comparing `tmp/jenkins_pysdk-1.3.2.tar.gz` & `tmp/jenkins_pysdk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_pysdk-1.3.2.tar", last modified: Wed May  8 19:42:51 2024, max compression
+gzip compressed data, was "jenkins_pysdk-1.3.5.tar", last modified: Fri May 10 22:14:26 2024, max compression
```

## Comparing `jenkins_pysdk-1.3.2.tar` & `jenkins_pysdk-1.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.797618 jenkins_pysdk-1.3.2/
--rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     3475 2024-05-08 19:42:51.796424 jenkins_pysdk-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2666 2024-04-21 17:59:25.000000 jenkins_pysdk-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.788344 jenkins_pysdk-1.3.2/jenkins_pysdk/
--rw-rw-rw-   0        0        0        2 2024-04-14 12:07:11.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/__init__.py
--rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/_logger.py
--rw-rw-rw-   0        0        0     5431 2024-04-18 19:59:55.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/builders.py
--rw-rw-rw-   0        0        0    15758 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/builds.py
--rw-rw-rw-   0        0        0     4242 2024-05-08 18:20:46.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/consts.py
--rw-rw-rw-   0        0        0     7701 2024-05-08 19:41:50.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/core.py
--rw-rw-rw-   0        0        0    13349 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/credentials.py
--rw-rw-rw-   0        0        0     1869 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/exceptions.py
--rw-rw-rw-   0        0        0    24815 2024-05-08 19:42:43.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/jenkins.py
--rw-rw-rw-   0        0        0    30659 2024-04-21 14:56:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/jobs.py
--rw-rw-rw-   0        0        0    11239 2024-04-21 09:31:25.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/nodes.py
--rw-rw-rw-   0        0        0     2581 2024-04-19 19:23:22.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/objects.py
--rw-rw-rw-   0        0        0    24085 2024-05-08 19:19:52.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/plugins.py
--rw-rw-rw-   0        0        0     6843 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/queues.py
--rw-rw-rw-   0        0        0     9797 2024-04-21 09:41:26.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/users.py
--rw-rw-rw-   0        0        0     4813 2024-05-08 19:25:02.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/utils.py
--rw-rw-rw-   0        0        0       90 2024-05-08 19:35:28.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/version.py
--rw-rw-rw-   0        0        0    12073 2024-04-21 14:55:11.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/views.py
--rw-rw-rw-   0        0        0     3405 2024-04-21 11:21:38.000000 jenkins_pysdk-1.3.2/jenkins_pysdk/workspace.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:42:51.795924 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/
--rw-rw-rw-   0        0        0     3475 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      679 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 19:42:51.000000 jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 19:42:51.797618 jenkins_pysdk-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-08 19:35:28.000000 jenkins_pysdk-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 22:14:26.059475 jenkins_pysdk-1.3.5/
+-rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0     3814 2024-05-10 22:14:26.058470 jenkins_pysdk-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2901 2024-05-10 17:53:19.000000 jenkins_pysdk-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 22:14:26.051844 jenkins_pysdk-1.3.5/jenkins_pysdk/
+-rw-rw-rw-   0        0        0        2 2024-04-14 12:07:11.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/_logger.py
+-rw-rw-rw-   0        0        0     5433 2024-05-10 18:20:36.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/builders.py
+-rw-rw-rw-   0        0        0    15742 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/builds.py
+-rw-rw-rw-   0        0        0     4408 2024-05-10 17:07:56.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/consts.py
+-rw-rw-rw-   0        0        0     7694 2024-05-10 18:20:36.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/core.py
+-rw-rw-rw-   0        0        0    13345 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/credentials.py
+-rw-rw-rw-   0        0        0     1869 2024-04-21 14:28:35.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    26561 2024-05-10 18:14:15.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/jenkins.py
+-rw-rw-rw-   0        0        0    31240 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/jobs.py
+-rw-rw-rw-   0        0        0    11223 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/nodes.py
+-rw-rw-rw-   0        0        0     2620 2024-05-10 18:20:36.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/objects.py
+-rw-rw-rw-   0        0        0    24025 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/plugins.py
+-rw-rw-rw-   0        0        0     6827 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/queues.py
+-rw-rw-rw-   0        0        0     9592 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/users.py
+-rw-rw-rw-   0        0        0     4813 2024-05-08 19:25:02.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/utils.py
+-rw-rw-rw-   0        0        0       90 2024-05-10 19:53:40.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/version.py
+-rw-rw-rw-   0        0        0    12081 2024-05-10 22:13:49.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/views.py
+-rw-rw-rw-   0        0        0     3398 2024-05-10 16:39:59.000000 jenkins_pysdk-1.3.5/jenkins_pysdk/workspace.py
+drwxrwxrwx   0        0        0        0 2024-05-10 22:14:26.057459 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/
+-rw-rw-rw-   0        0        0     3814 2024-05-10 22:14:25.000000 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2024-05-10 22:14:25.000000 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 22:14:25.000000 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-10 22:14:25.000000 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 22:14:25.000000 jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 22:14:26.059975 jenkins_pysdk-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2024-05-10 19:53:40.000000 jenkins_pysdk-1.3.5/setup.py
```

### Comparing `jenkins_pysdk-1.3.2/LICENSE` & `jenkins_pysdk-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3.2/PKG-INFO` & `jenkins_pysdk-1.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: jenkins_pysdk
-Version: 1.3.2
+Version: 1.3.5
 Summary: 2024 Python SDK for Jenkins
 Home-page: https://github.com/KnownZero/JenkinsPythonSDK
 Author: KnownZero
 Author-email: gihjeefs@protonmail.com
 License: MIT
 Keywords: python,Jenkins,SDK,API,REST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: pydantic
 Requires-Dist: urllib3
@@ -48,24 +50,31 @@
 jenkins = Jenkins(
     host="<host>", 
     username="<username>", 
     passw="<passw>"
 )
 ```
 #### OR
+
 ```python
 from jenkins_pysdk.jenkins import Jenkins
 jenkins = Jenkins(
     host="<host>", 
     username="<username>",
     token="<token>"
 )
 ```
+#### Why is the token parameter different?
+```
+Using an API token removes the need for Crumbs in your requests. 
+
+Of course, the SDK handles crumbs for you, but it will reduce the number of requests. 
+```
 
-#### See [docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html) for full documentation.
+### See [[JenkinsPythonSDK Docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html)] for full documentation.
 
 ## Contributing
 
 Feel free to create pull requests.
 
 For major changes, please open an issue first
 to discuss what you would like to change.
@@ -94,12 +103,12 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
-This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
+### This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
 
 ## Contributors
 KnownZero
```

### Comparing `jenkins_pysdk-1.3.2/README.md` & `jenkins_pysdk-1.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,31 @@
 jenkins = Jenkins(
     host="<host>", 
     username="<username>", 
     passw="<passw>"
 )
 ```
 #### OR
+
 ```python
 from jenkins_pysdk.jenkins import Jenkins
 jenkins = Jenkins(
     host="<host>", 
     username="<username>",
     token="<token>"
 )
 ```
+#### Why is the token parameter different?
+```
+Using an API token removes the need for Crumbs in your requests. 
+
+Of course, the SDK handles crumbs for you, but it will reduce the number of requests. 
+```
 
-#### See [docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html) for full documentation.
+### See [[JenkinsPythonSDK Docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html)] for full documentation.
 
 ## Contributing
 
 Feel free to create pull requests.
 
 For major changes, please open an issue first
 to discuss what you would like to change.
@@ -70,12 +77,12 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
-This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
+### This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
 
 ## Contributors
 KnownZero
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/_logger.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/_logger.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/builders.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 __all__ = ["Builder"]
 
 
 class Builder:
     """
     Easy builder if you don't like XML... like me ;)
     """
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/builds.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/builds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
-from collections.abc import Generator
-from typing import List, Optional
-import orjson
+from typing import List, Optional, Generator
 
+import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound
 from jenkins_pysdk.consts import Endpoints, FORM_HEADER_DEFAULT
 
 
@@ -266,15 +265,15 @@
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code != 200:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Failed to fetch job information.")
 
         data = orjson.loads(resp_obj.content)
         return len(data.get('builds', []))
 
-    def iter(self) -> Generator[Build]:
+    def iter(self) -> Generator[Build, None, None]:
         """
         Iterate over builds in the build history of the job.
 
         :yield: A Build object representing each build in the build history.
         :rtype: Generator[:class:`jenkins_pysdk.builds.Build`]
         :raises JenkinsGeneralException: If a general exception occurs.
         """
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/consts.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,19 +113,16 @@
         Delete = "doDelete"
         Disable = "toggleOffline"
         Create = "doCreateItem"
 
 
 class Class:
     Folder = "com.cloudbees.hudson.plugins.folder.Folder"
+    OrganizationFolder = "jenkins.branch.OrganizationFolder"
     Freestyle = "hudson.model.FreeStyleProject"
+    Pipeline = "org.jenkinsci.plugins.workflow.job.WorkflowJob"
+    MultiConfigurationProject = "hudson.matrix.MatrixProject"
+    MultiBranchPipeline = "org.jenkinsci.plugins.workflow.multibranch.WorkflowMultiBranchProject"
     JenkinsFile = ""
     ListView = "hudson.model.ListView"
     MyView = "hudson.model.MyView"
     Dashboard = "hudson.plugins.view.dashboard.Dashboard"
-    UsernamePassword = ""
-
-
-# class References:
-#     class Jobs:
-#         JOBS = "jobs"
-#         VIEWS = "views"
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/core.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Tuple, Any
+from typing import Tuple, Any
 
 import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.consts import Endpoints
 from jenkins_pysdk.utils import interact_http, interact_http_session
 from jenkins_pysdk.consts import HTTP_HEADER_DEFAULT
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/credentials.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from collections.abc import Generator
-from typing import List, Optional
-import orjson
+from typing import List, Optional, Generator
 
+import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound, JenkinsAlreadyExists
 from jenkins_pysdk.consts import Endpoints, XML_HEADER_DEFAULT, XML_POST_HEADER, FORM_HEADER_DEFAULT
 from jenkins_pysdk.builders import Builder
 
@@ -167,15 +166,15 @@
         """
         for cred in self.iter():
             if cred.id == cred_id:
                 return cred
         else:
             raise JenkinsNotFound(f"Credential ({cred_id}) was not found in domain ({self.name}).")
 
-    def iter(self) -> Generator[Credential]:
+    def iter(self) -> Generator[Credential, None, None]:
         """
         Iterate over credentials within the domain.
 
         :return: A generator yielding credentials within the specified domain.
         :rtype: Generator[:class:`jenkins_pysdk.credentials.Credential`]
         :raises JenkinsGeneralException: If a general exception occurs.
         """
@@ -247,15 +246,15 @@
             domain = "_"
         url = self._jenkins._build_url(Endpoints.Credentials.Domain.format(domain=domain))
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code == 404:
             raise JenkinsGeneralException(f"Couldn't find {domain} or you don't have permission to view it.")
         return Domain(jenkins=self._jenkins, url=url)
 
-    def iter_domains(self) -> Generator[Domain]:
+    def iter_domains(self) -> Generator[Domain, None, None]:
         """
         Iterate over domains on the Jenkins instance.
 
         :return: A generator yielding Domain objects.
         :rtype: Generator[:class:`jenkins_pysdk.credentials.Domain`]
         :raises JenkinsGeneralException: If a general exception occurs.
         """
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/exceptions.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/jenkins.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/jenkins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
-
-import os, sys
-project_root = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-sys.path.insert(0, project_root)
-
 import re
 import time
-
 import threading
 from typing import Optional
 
+import orjson
+
+import os, sys
+project_root = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+sys.path.insert(0, project_root)
+
 from jenkins_pysdk.core import Core
 from jenkins_pysdk.consts import Endpoints, FORM_HEADER_DEFAULT, Class
 from jenkins_pysdk.exceptions import JenkinsConnectionException, JenkinsUnauthorisedException, \
     JenkinsRestartFailed, JenkinsActionFailed, JenkinsGeneralException
-from jenkins_pysdk.objects import JenkinsConnectObject, JenkinsActionObject, Views as r_views, Jobs as r_jobs
+from jenkins_pysdk.objects import JenkinsConnectObject, JenkinsActionObject
+from jenkins_pysdk.objects import Views as r_views, Jobs as r_jobs, Folders as r_folders
 from jenkins_pysdk.jobs import Jobs, Folders
 from jenkins_pysdk.views import Views
 from jenkins_pysdk.users import Users, User
 from jenkins_pysdk.credentials import Credentials
 from jenkins_pysdk.plugins import Plugins
 from jenkins_pysdk.nodes import Nodes
 from jenkins_pysdk.queues import Queue
 
-import orjson
-
 
 __all__ = ["Jenkins"]
 
 
 class Jenkins(Core):
     """
     This is the main class for interacting with your Jenkins instance.
@@ -159,14 +158,64 @@
         Flag used to create FreeStyle jobs in Jobs.create() method.
 
         :return: Flag for creating FreeStyle jobs
         :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
         """
         return r_jobs(value=Class.Freestyle)
 
+    @property
+    def Pipeline(self) -> r_jobs:
+        """
+        Flag used to create Pipeline jobs in Jobs.create() method.
+
+        :return: Flag for creating Pipeline jobs
+        :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
+        """
+        return r_jobs(value=Class.Pipeline)
+
+    @property
+    def MultiBranchPipeline(self) -> r_jobs:
+        """
+        Flag used to create MultiBranchPipeline jobs in Jobs.create() method.
+
+        :return: Flag for creating MultiBranchPipeline jobs
+        :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
+        """
+        return r_jobs(value=Class.MultiBranchPipeline)
+
+    @property
+    def MultiConfigurationProject(self) -> r_jobs:
+        """
+        Flag used to create multi-configuration project jobs in Jobs.create() method.
+
+        :return: Flag for creating multi-configuration project jobs
+        :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
+        """
+        return r_jobs(value=Class.MultiConfigurationProject)
+
+    @property
+    def Folder(self) -> r_folders:
+        """
+        Flag used to create Folder in Folders.create() or Folder.create() method.
+
+        :return: Flag for creating Folder
+        :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
+        """
+        return r_folders(value=Class.Folder)
+
+    @property
+    def OrganizationFolder(self) -> r_folders:
+        """
+        Flag used to create OrganizationFolder in Folders.create() or Folder.create() method.
+
+        :return: Flag for creating OrganizationFolder
+        :rtype: :class:`jenkins_pysdk.objects.Flags.Jobs`
+        """
+        return r_folders(value=Class.OrganizationFolder)
+
     # @property
     # def enable_logging(self):
     #     """
     #     Get the logging level.
     #     """
     #     return self.Enable_Logging
     #
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/jobs.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from collections.abc import Generator
-from typing import List
+from typing import List, Generator
 
 import orjson
 from pydantic import HttpUrl
 
-from jenkins_pysdk.objects import JenkinsValidateJob, JenkinsActionObject, Jobs as r_jobs
+from jenkins_pysdk.objects import JenkinsValidateJob, JenkinsActionObject
+from jenkins_pysdk.objects import Jobs as r_jobs, Folders as r_folders
 from jenkins_pysdk.exceptions import JenkinsNotFound, JenkinsGeneralException
 from jenkins_pysdk.consts import Endpoints, Class, XML_HEADER_DEFAULT, XML_POST_HEADER
 from jenkins_pysdk.builders import Builder
 from jenkins_pysdk.builds import Builds
 from jenkins_pysdk.workspace import Workspace
 
 __all__ = ["Jobs", "Folders", "Job", "Folder"]
@@ -192,24 +192,23 @@
         :type path: str
         :return: True if the path corresponds to a job, False otherwise.
         :rtype: bool
         :raises JenkinsGeneralException: If a general exception occurs.
         :raises JenkinsNotFound: If the job is not found.
         """
         built = self._jenkins._build_job_http_path(path)
-        endpoint = f"{built}/{Endpoints.Instance.Standard}"
-        url = self._jenkins._build_url(endpoint)
+        url = self._jenkins._build_url(built, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code == 404:
             raise JenkinsNotFound(f"[{resp_obj.status_code}] {path} not found.")
         else:
             data = orjson.loads(resp_obj.content)
-            if data['_class'] != Class.Folder:
+            if data['_class'] not in [Class.Folder, Class.OrganizationFolder]:
                 return True
             return False
 
     def _validate_job(self, job_path: str) -> JenkinsValidateJob:
         # TODO: Review mess
         job = self._jenkins._build_job_http_path(job_path)
         url = self._jenkins._build_url(job)
@@ -223,15 +222,15 @@
         if not self.is_job(job_path):
             raise JenkinsGeneralException(f"{job_path} is a folder. Please use folders.")
 
         obj = JenkinsValidateJob(url=url, is_valid=validated)
         obj._raw = resp_obj
         return obj
 
-    def _create_job(self, job_name: str, xml, mode: r_jobs, folder_path: HttpUrl = None) \
+    def _create_job(self, job_name: str, xml, mode: str, folder_path: HttpUrl = None) \
             -> JenkinsActionObject or JenkinsNotFound:
         create_endpoint = Endpoints.Jobs.Create
         endpoint = f"{folder_path}/{create_endpoint}" if folder_path else create_endpoint
         url = self._jenkins._build_url(endpoint)
         params = {"name": job_name, "mode": mode}
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_HEADER_DEFAULT,
                                                      params=params, data=xml)
@@ -241,42 +240,41 @@
             msg = f"[{resp_obj.status_code}] Successfully created {job_name}."
         else:
             msg = f"[{resp_obj.status_code}] Failed to create job {job_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, job_path: str, xml: str, *args: r_jobs) -> JenkinsActionObject:
+    def create(self, job_path: str, xml: str, job_type: r_jobs) -> JenkinsActionObject:
         """
         Create a job on the Jenkins instance.
 
         :param job_path: The path where the job should be created.
         :type job_path: str
         :param xml: XML configuration for the job.
         :type xml: str
-        :param args: Additional parameters for job creation.
-        :type args: :class:`jenkins_pysdk.objects.Jobs` (Default: Freestyle)
+        :param job_type: Additional parameters for job creation.
+        :type job_type: :class:`jenkins_pysdk.objects.Jobs`
         :return: Object representing the result of the creation action.
         :rtype: :class:`jenkins_pysdk.objects.JenkinsActionObject`
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         try:
             self.is_job(job_path)
             raise JenkinsGeneralException(f"{job_path} already exists.")
         except JenkinsNotFound:
             pass
 
-        # TODO: Add all other jobs types
-        mode = args[0].value if args else Class.Freestyle
+        mode = job_type.value
         job_name, job_parent = self._jenkins._get_folder_parent(job_path)
         built = self._jenkins._build_job_http_path(job_parent)
         created = self._create_job(job_name, xml, mode, built)
         return created
 
-    def iter(self, folder=None, _paginate=0) -> Generator[Job]:
+    def iter(self, folder=None, _paginate=0) -> Generator[Job, None, None]:
         """
         Iterate through jobs in the Jenkins instance.
 
         :param folder: The folder to iterate through. If None, iterate through all jobs.
         :type folder: str, optional
         :param _paginate: Pagination flag. Defaults to 0 (disabled).
         :type _paginate: int, optional
@@ -317,15 +315,15 @@
                     break
 
                 if _paginate > 0:
                     start += _paginate + 1
                 elif _paginate == 0:
                     break
 
-    def _fetch_job_iter(self, job_url) -> Generator[Job]:
+    def _fetch_job_iter(self, job_url) -> Generator[Job, None, None]:
         # Pagination not needed here because function repeats itself if needed
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
 
         try:
@@ -333,15 +331,15 @@
                 yield Job(jenkins=self._jenkins, job_path=data['fullName'], job_url=data['url'])
             elif data['_class'] == Class.Folder:
                 for item in data.get('jobs', []):
                     yield from self._fetch_job_iter(item['url'])
         except Exception as error:
             print(error)
 
-    def _fetch_job(self, job_url) -> Generator[Job]:
+    def _fetch_job(self, job_url) -> Generator[Job, None, None]:
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         yield Job(jenkins=self._jenkins, job_path=data['fullName'], job_url=data['url'])
 
     def list(self, folder=None, _paginate=0) -> List[Job]:
@@ -445,15 +443,15 @@
         params = {"name": new_job_name, "mode": "copy", "from": copy_job_name}
         url = self._jenkins._build_url(Endpoints.Jobs.Create, prefix=self._folder_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, params=params)
         msg = f"[{resp_obj.status_code}] Successfully copied {copy_job_name} to {new_job_name}."
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code == 400:
-            if re.search(r"A job already exists with the name", str(resp_obj.content)):  # TODO: This is method unreliable
+            if re.search(r"A job already exists with the name", str(resp_obj.content)):  # TODO: This method doesn't seem reliable
                 raise JenkinsGeneralException(f"{new_job_name} already exists.")
             msg = f"[{resp_obj.status_code}] Failed to copy folder."
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to copy folder."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
@@ -473,27 +471,31 @@
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 204:
             msg = f"[{resp_obj.status_code}] Failed to delete folder."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, folder_name: str, xml: str or Builder.Folder) -> JenkinsActionObject:
+    def create(self, folder_name: str, xml: str or Builder.Folder,
+               folder_type: r_folders = Class.Folder) -> JenkinsActionObject:
         """
         Creates sub-folders in the current path.
 
         :param folder_name: The name of the folder to create.
         :type folder_name: str
         :param xml: The XML configuration for the folder. Can be a string or a Builder.Folder object.
         :type xml: str or Builder.Folder
+        :param folder_type: (Optional) The type of folder to create
+        :type folder_type: :class:`jenkins_pysdk.objects.Folders`
         :return: The result of the action.
         :rtype: :class:`jenkins_pysdk.objects.JenkinsActionObject`
         :raises JenkinsGeneralException: If a general exception occurs.
         """
-        return Folders(self._jenkins)._create_folder(folder_name, xml, self.path)
+        mode = folder_type.value if isinstance(folder_type, r_folders) else folder_type
+        return Folders(self._jenkins)._create_folder(folder_name, xml, self.path, mode)
 
     @property
     def config(self) -> str:
         """
         Get the XML configuration of the folder.
 
         :return: The XML configuration of the folder.
@@ -565,42 +567,45 @@
         url = self._jenkins._build_url(built, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 200:
             raise JenkinsNotFound(f"{path} not found.")
         data = orjson.loads(resp_obj.content)
-        if data['_class'] == Class.Folder:
+        if data['_class'] in [Class.Folder, Class.OrganizationFolder]:
             return True
         return False
 
-    def _create_folder(self, folder_name: str, xml, folder_path: str = None) -> JenkinsActionObject:
+    def _create_folder(self, folder_name: str, xml, mode: str, folder_path: str = None) -> JenkinsActionObject:
         endpoint = self._jenkins._build_job_http_path(folder_path)
         url = self._jenkins._build_url(endpoint, suffix=Endpoints.Jobs.Create)
-        params = {"name": folder_name, "mode": Class.Folder}
+        params = {"name": folder_name, "mode": mode}
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_HEADER_DEFAULT,
                                                      params=params, data=xml)
         if resp_obj.status_code == 404:
             raise JenkinsNotFound(f"Parent path {str(folder_path)} not found.")
         elif resp_obj.status_code == 200:
             msg = f"[{resp_obj.status_code}] Successfully created {folder_name}."
         else:
             msg = f"[{resp_obj.status_code}] Failed to create folder {folder_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, folder_path: str, xml: str or Builder.Folder) -> JenkinsActionObject:
+    def create(self, folder_path: str, xml: str or Builder.Folder,
+               folder_type: r_folders = Class.Folder) -> JenkinsActionObject:
         """
         Creates a folder at the specified path with the given XML configuration.
 
         :param folder_path: The path where the folder will be created.
         :type folder_path: str
         :param xml: The XML configuration for the folder.
         :type xml: str or Builder.Folder
+        :param folder_type: (Optional) The type of folder to create
+        :type folder_type: :class:`jenkins_pysdk.objects.Folders`
         :return: The result of the folder creation operation.
         :rtype: :class:`jenkins_pysdk.objects.JenkinsActionObject`
         :raises JenkinsNotFound: If the folder was not found.
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         folder_name, folder_parent = self._jenkins._get_folder_parent(folder_path)
 
@@ -609,21 +614,22 @@
             self.search(built_path)
             raise JenkinsGeneralException(f"{folder_path} already exists.")
         except JenkinsNotFound:
             pass
 
         try:
             built_path = self._jenkins._build_job_http_path(folder_parent)
-            return self._create_folder(folder_name, xml, built_path)
+            mode = folder_type.value
+            return self._create_folder(folder_name, xml, mode, built_path)
         except JenkinsNotFound as error:
             if not self.is_folder(folder_parent):
                 raise JenkinsNotFound(f"Failed to create folder because parent path not found: {folder_parent}.")
             raise error
 
-    def iter(self, folder: str = None, _paginate: int = 0) -> Generator[Folder]:
+    def iter(self, folder: str = None, _paginate: int = 0) -> Generator[Folder, None, None]:
         """
         Iterate over folders within the specified folder.
 
         :param folder: The path of the parent folder. If None, iterate over all folders.
         :type folder: str, optional
         :param _paginate: Number of items to paginate. Default is 0 (no pagination).
         :type _paginate: int, optional
@@ -662,28 +668,28 @@
                     break
 
                 if _paginate > 0:
                     start += _paginate + 1
                 elif _paginate == 0:
                     break
 
-    def _fetch_folder_iter(self, folder_url) -> Generator[Folder]:
+    def _fetch_folder_iter(self, folder_url) -> Generator[Folder, None, None]:
         json_url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=folder_url)
         req_obj, resp_obj = self._jenkins._send_http(url=json_url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
 
         if data['_class'] == Class.Folder:
             folders = data.get('jobs', [])
             for item in folders:
                 yield from self._fetch_folder_iter(item['url'])
             if not folders:
                 yield from self._fetch_folder(data['url'])
 
-    def _fetch_folder(self, folder_url) -> Generator[Folder]:
+    def _fetch_folder(self, folder_url) -> Generator[Folder, None, None]:
         json_url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=folder_url)
         req_obj, resp_obj = self._jenkins._send_http(url=json_url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         yield Folder(jenkins=self._jenkins, folder_path=data['fullName'], folder_url=data['url'])
 
     def list(self, folder=None, _paginate=0) -> List[Folder]:
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/nodes.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from collections.abc import Generator
-from typing import List
+from typing import List, Generator
 
 import orjson
 
 from jenkins_pysdk.consts import Endpoints, XML_HEADER_DEFAULT, XML_POST_HEADER
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound
 from jenkins_pysdk.builders import Builder
@@ -224,15 +223,15 @@
             msg = f"[{resp_obj.status_code}] Bad request for node ({name})."
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to create node ({name})."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def iter(self) -> Generator[Node]:
+    def iter(self) -> Generator[Node, None, None]:
         """
         Iterate over the nodes.
 
         :return: A generator yielding Node objects.
         :rtype: Generator[:class:`jenkins_pysdk.nodes.Node`]
         :raises JenkinsGeneralException: If a general exception occurs.
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/objects.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-
 from typing import Any, Optional
 from pydantic import BaseModel, HttpUrl, PrivateAttr
 
 
 __all__ = ["HTTPRequestObject", "JenkinsConnectObject", "HTTPResponseObject", "JenkinsActionObject", "Parameter",
            "Filter", "Flags", "Setting", "HTTPSessionResponseObject", "HTTPSessionRequestObject", "JenkinsValidateJob",
            "Views", "Jobs"]
@@ -91,14 +90,17 @@
 class Views(Flags):
     value: str
 
 
 class Jobs(Flags):
     value: str
 
+class Folders(Flags):
+    value: str
+
 
 class Parameter(Flags):
     value: str
 
 
 class BaseParameter(Flags):
     value: str
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/plugins.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from collections.abc import Generator
-from typing import List, Union, Dict, BinaryIO
+from typing import List, Union, Dict, BinaryIO, Generator
 
 import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound
 from jenkins_pysdk.consts import Endpoints, XML_POST_HEADER
@@ -125,15 +124,15 @@
         """
         for site in self.iter():
             if name == site.id:
                 return site
         else:
             raise JenkinsNotFound(f"Site ({name}) was not found.")
 
-    def iter(self) -> Generator[Site]:
+    def iter(self) -> Generator[Site, None, None]:
         """
         Iterate over the sites in the update center.
 
         :return: A generator yielding Site objects.
         :rtype: Generator[:class:`jenkins_pysdk.plugins.Site`]
         :raises JenkinsGeneralException: If a general exception occurs.
         """
@@ -327,15 +326,15 @@
         """
         Disable the installed plugin.
 
         :return: JenkinsActionObject representing the disable action.
         :rtype: jenkins_pysdk.objects.JenkinsActionObject
         :raises JenkinsGeneralException: If a general exception occurs.
         """
-        # TODO: Add restart param
+
         url = self._jenkins._build_url(Endpoints.Plugins.PluginManager,
                                        suffix=Endpoints.Plugins.Disable.format(plugin=self.name))
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url)
         if resp_obj.status_code != 200:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Failed to disable plugin ({self.name}).")
 
         msg = f"[{resp_obj.status_code}] Successfully disabled plugin ({self.name})."
@@ -409,15 +408,14 @@
         """
         Delete the plugin from the Jenkins instance.
 
         :return: JenkinsActionObject representing the delete action.
         :rtype: jenkins_pysdk.objects.JenkinsActionObject
         :raises JenkinsGeneralException: If a general exception occurs.
         """
-        # TODO: Add restart param
         url = self._jenkins._build_url(Endpoints.Plugins.PluginManager,
                                        suffix=Endpoints.Plugins.Uninstall.format(plugin=self.name))
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url)
         if resp_obj.status_code != 200:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Failed to uninstall plugin ({self.name}).")
         msg = f"[{resp_obj.status_code}] Successfully uninstalled plugin ({self.name})."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
@@ -454,15 +452,15 @@
         """
         for plugin in self.iter(site=site, _paginate=_paginate):
             if plugin.name == id:
                 return plugin
         else:
             raise JenkinsNotFound(f"Plugin ({id}) was not found in {self.type}.")
 
-    def iter(self, site: str = "default", _paginate: int = 0) -> Generator[Union[Plugin, Installed]]:
+    def iter(self, site: str = "default", _paginate: int = 0) -> Generator[Union[Plugin, Installed], None, None]:
         """
         Iterate over the plugins or installed plugins within the plugin group.
 
         :param site: The site to iterate over. Default is "default".
         :type site: str, optional
         :param _paginate: The number of items to paginate. Default is 0.
         :type _paginate: int, optional
@@ -564,15 +562,15 @@
     def upload(self, filename: str, file_content: BinaryIO or bytes) -> JenkinsActionObject:
         """
         Uploads a plugin to Jenkins.
 
         :param filename: The name of the plugin file.
         :type filename: str
         :param file_content: The content of the plugin file as bytes.
-        :type file_content: bytes
+        :type file_content: bytes or BinaryIO
         :return: A JenkinsActionObject representing the upload action.
         :rtype: jenkins_pysdk.objects.JenkinsActionObject
         :raises JenkinsGeneralException: If a general exception occurs.
         """
         # Solution: https://issues.jenkins.io/browse/JENKINS-68443
         # Make it a form submission ^
         if isinstance(file_content, BinaryIO):
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/queues.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/queues.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from collections.abc import Generator
-from typing import List
+from typing import List, Generator
 
 import orjson
 
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsEmptyQueue
 from jenkins_pysdk.consts import Endpoints
 from jenkins_pysdk.jobs import Job
 from jenkins_pysdk.builds import Build
@@ -127,15 +126,15 @@
 
     :param jenkins: The Jenkins instance.
     :type jenkins: :class:`jenkins_pysdk.jenkins.Jenkins`
     """
     def __init__(self, jenkins):
         self._jenkins = jenkins
 
-    def iter(self, _paginate=0) -> Generator[QueueItem]:
+    def iter(self, _paginate=0) -> Generator[QueueItem, None, None]:
         """
         Iterates over the items in the Jenkins queue.
 
         :param _paginate: The number of items to fetch per page (default is 0, meaning all items).
         :type _paginate: int
         :return: A generator yielding QueueItem objects representing items in the queue.
         :rtype: Generator[:class:`jenkins_pysdk.queues.QueueItem`]
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/users.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from collections.abc import Generator
-from typing import List
-import orjson
+from typing import List, Generator
 
+import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsGeneralException, JenkinsNotFound
 from jenkins_pysdk.consts import Endpoints, FORM_HEADER_DEFAULT
 from jenkins_pysdk.objects import Builder
 from jenkins_pysdk.views import View as v_view
@@ -64,15 +63,15 @@
         :return: The name of the user.
         :rtype: str
         """
         return str(self._raw['fullName'])
 
     def credentials(self, domain="_") -> c_domain:
         """
-        Search the user's personal credential safe.
+        Search the users' personal credential safe.
 
         :param domain: The domain to search for credentials (default is "_").
         :type domain: str, optional
         :return: A domain object representing the user's personal credential safe.
         :rtype: :class:`jenkins_pysdk.credentials.Domain`
         :raises: JenkinsNotFound: If the users credentials were not found.
         """
@@ -107,18 +106,14 @@
         """
         Get a list of builds associated with the user.
 
         :return: A list of build objects associated with the user.
         :rtype: List[jenkins_pysdk.builds.Build]
         :raises JenkinsGeneralException: If a general exception occurs.
         """
-        import time
-        # TODO: Something about this...
-        print(Warning("No REST endpoint available... returning HTML response for the moment..."))
-        time.sleep(1)
         url = self._jenkins._build_url(Endpoints.User.Builds, prefix=self._user_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         code = resp_obj.status_code
         if code != 200:
             raise JenkinsGeneralException(f"[{code}] Failed to get users' builds.")
         return resp_obj.content
 
@@ -142,15 +137,15 @@
             msg = f"[400] Failed to delete user ({self.name})."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     def logout(self) -> JenkinsActionObject:
         """
-        Terminate all the users' sessions.
+        Terminate the user's session.
 
         :return: Result of the logout request
         :rtype: :class:`jenkins_pysdk.objects.JenkinsActionObject`
         """
         url = self._jenkins._build_url(Endpoints.User.Boot.format(user=self.name))
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url)
         if resp_obj.status_code == 200:
@@ -189,15 +184,15 @@
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code == 404:
             raise JenkinsGeneralException(f"User {username} was not found.")
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         return User(self._jenkins, data.get('absoluteUrl', url))
 
-    def iter(self) -> Generator[User]:
+    def iter(self) -> Generator[User, None, None]:
         """
         Iterate over all users.
 
         :return: Generator yielding User objects.
         :rtype: Generator[:class:`jenkins_pysdk.usersUser`]
         """
         url = self._jenkins._build_url(Endpoints.Users.List, suffix=Endpoints.Instance.Standard)
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/utils.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/utils.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/views.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from collections.abc import Generator
-from typing import List
-import orjson
+from typing import List, Generator
 
+import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.objects import JenkinsValidateJob, JenkinsActionObject
 from jenkins_pysdk.exceptions import JenkinsNotFound, JenkinsGeneralException
 from jenkins_pysdk.consts import Endpoints, XML_HEADER_DEFAULT, XML_POST_HEADER
 from jenkins_pysdk.builders import Builder
 
@@ -200,15 +199,15 @@
             raise JenkinsGeneralException(f"{name} already exists.")
         except JenkinsNotFound:
             pass
 
         created = self._create_view(name, xml)
         return created
 
-    def iter(self, folder: str = None, _paginate=0) -> Generator[View]:
+    def iter(self, folder: str = None, _paginate=0) -> Generator[View, None, None]:
         """
         Iterate through views.
 
         :param folder: Check if folder is in a view. Default is None.
         :type folder: str, optional
         :param _paginate: Pagination option. Default is 0 (no pagination).
         :type _paginate: int, optional
@@ -245,29 +244,29 @@
                     yield View(jenkins=self._jenkins, name=item['name'], url=item['url'])
 
                 if _paginate > 0:
                     start += _paginate + 1
                 elif _paginate == 0:
                     break
 
-    def _fetch_view_iter(self, job_url) -> Generator[View]:
+    def _fetch_view_iter(self, job_url) -> Generator[View, None, None]:
         # Pagination not needed here because function repeats itself if needed
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
 
         views = data.get('views', [])
         if not views:
             return
 
         for item in views:
             yield View(jenkins=self._jenkins, name=item['name'], url=item['url'])
 
-    def _fetch_view(self, view_url) -> Generator[View]:
+    def _fetch_view(self, view_url) -> Generator[View, None, None]:
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=view_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         yield View(jenkins=self._jenkins, name=data['name'], url=data['url'])
 
     def list(self, folder: str = None, _paginate=0) -> List[View]:
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk/workspace.py` & `jenkins_pysdk-1.3.5/jenkins_pysdk/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, jenkins, job_name: str, job_url: HttpUrl):
         self._jenkins = jenkins
         self._job_name = job_name
         self._job_url = job_url
 
     def download(self, path: str or Path, workspace_file: str = None) -> JenkinsActionObject:
         """
-        Download workspace files for the Jenkins job.
+        Download workspace files from the job.
 
         :param path: The directory where the workspace files will be saved.
         :type path: str
         :param workspace_file: (Optional) Download a specific file in the workspace
         :type workspace_file: str, optional
         :return: An object representing the action performed in Jenkins.
         :rtype: :class:`jenkins_pysdk.objects.JenkinsActionObject`
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/PKG-INFO` & `jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: jenkins_pysdk
-Version: 1.3.2
+Version: 1.3.5
 Summary: 2024 Python SDK for Jenkins
 Home-page: https://github.com/KnownZero/JenkinsPythonSDK
 Author: KnownZero
 Author-email: gihjeefs@protonmail.com
 License: MIT
 Keywords: python,Jenkins,SDK,API,REST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: pydantic
 Requires-Dist: urllib3
@@ -48,24 +50,31 @@
 jenkins = Jenkins(
     host="<host>", 
     username="<username>", 
     passw="<passw>"
 )
 ```
 #### OR
+
 ```python
 from jenkins_pysdk.jenkins import Jenkins
 jenkins = Jenkins(
     host="<host>", 
     username="<username>",
     token="<token>"
 )
 ```
+#### Why is the token parameter different?
+```
+Using an API token removes the need for Crumbs in your requests. 
+
+Of course, the SDK handles crumbs for you, but it will reduce the number of requests. 
+```
 
-#### See [docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html) for full documentation.
+### See [[JenkinsPythonSDK Docs](https://jenkinspythonsdk.readthedocs.io/en/latest/index.html)] for full documentation.
 
 ## Contributing
 
 Feel free to create pull requests.
 
 For major changes, please open an issue first
 to discuss what you would like to change.
@@ -94,12 +103,12 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
-This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
+### This code is free to use, and I will not take ANY responsibility for any damage that you create yourself.
 
 ## Contributors
 KnownZero
```

### Comparing `jenkins_pysdk-1.3.2/jenkins_pysdk.egg-info/SOURCES.txt` & `jenkins_pysdk-1.3.5/jenkins_pysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-1.3.2/setup.py` & `jenkins_pysdk-1.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name='jenkins_pysdk',
-    version='1.3.2',  # Don't forget to update version.py & conf.py :)
+    version='1.3.5',  # Don't forget to update version.py & conf.py :)
     packages=find_packages(),
     install_requires=[
         'httpx',
         'orjson',
         'pydantic',
         'urllib3',
     ],
@@ -25,10 +25,12 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
     ],
     keywords=['python', 'Jenkins', 'SDK', 'API', 'REST']
 )
```

