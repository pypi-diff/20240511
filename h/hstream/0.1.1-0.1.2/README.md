# Comparing `tmp/hstream-0.1.1.tar.gz` & `tmp/hstream-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.1.tar", max compression
+gzip compressed data, was "hstream-0.1.2.tar", max compression
```

## Comparing `hstream-0.1.1.tar` & `hstream-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,25 @@
--rw-r--r--   0        0        0     3245 2024-05-10 00:18:54.732784 hstream-0.1.1/README.md
--rw-r--r--   0        0        0     6874 2024-05-09 13:05:58.281051 hstream-0.1.1/hstream/HSServer.py
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.1/hstream/__init__.py
--rw-r--r--   0        0        0      142 2024-05-09 13:05:58.281937 hstream-0.1.1/hstream/__main__.py
--rw-r--r--   0        0        0     1030 2024-05-09 13:05:58.282242 hstream-0.1.1/hstream/cli.py
--rw-r--r--   0        0        0    16658 2024-05-10 00:19:41.083664 hstream-0.1.1/hstream/components/components.py
--rw-r--r--   0        0        0     4633 2024-05-09 13:05:58.283127 hstream-0.1.1/hstream/components/styling_components.py
--rw-r--r--   0        0        0      766 2024-05-09 13:05:58.283401 hstream-0.1.1/hstream/hs.py
--rw-r--r--   0        0        0      761 2024-05-09 13:05:58.283588 hstream-0.1.1/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.1/hstream/template.py
--rw-r--r--   0        0        0      161 2024-05-09 13:05:58.284121 hstream-0.1.1/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2453 2024-05-09 13:05:58.284396 hstream-0.1.1/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2659 2024-05-09 13:05:58.284676 hstream-0.1.1/hstream/utils.py
--rw-r--r--   0        0        0      526 2024-05-10 00:24:39.178080 hstream-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 hstream-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4318 2024-05-11 12:21:43.141596 hstream-0.1.2/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.2/hstream/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-09 13:05:58.281937 hstream-0.1.2/hstream/__main__.py
+-rw-r--r--   0        0        0     2377 2024-05-11 13:19:26.505499 hstream-0.1.2/hstream/cli.py
+-rw-r--r--   0        0        0    16829 2024-05-11 11:38:42.857136 hstream-0.1.2/hstream/components/components.py
+-rw-r--r--   0        0        0     4633 2024-05-09 13:05:58.283127 hstream-0.1.2/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-11 01:21:34.641755 hstream-0.1.2/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-11 01:21:34.644340 hstream-0.1.2/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      757 2024-05-11 03:52:48.159049 hstream-0.1.2/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      368 2024-05-11 04:02:12.326494 hstream-0.1.2/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7232 2024-05-11 12:14:46.432202 hstream-0.1.2/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      660 2024-05-11 01:21:34.646023 hstream-0.1.2/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-11 01:21:34.646562 hstream-0.1.2/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649048 hstream-0.1.2/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3215 2024-05-11 04:07:02.605594 hstream-0.1.2/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      800 2024-05-11 01:21:34.649589 hstream-0.1.2/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-11 01:21:34.649841 hstream-0.1.2/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      705 2024-05-11 12:14:20.156589 hstream-0.1.2/hstream/hs.py
+-rw-r--r--   0        0        0      391 2024-05-11 11:50:20.040099 hstream-0.1.2/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.2/hstream/template.py
+-rw-r--r--   0        0        0      161 2024-05-09 13:05:58.284121 hstream-0.1.2/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2453 2024-05-09 13:05:58.284396 hstream-0.1.2/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2465 2024-05-11 12:13:40.726351 hstream-0.1.2/hstream/utils.py
+-rw-r--r--   0        0        0      523 2024-05-11 13:19:34.965468 hstream-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 hstream-0.1.2/PKG-INFO
```

### Comparing `hstream-0.1.1/README.md` & `hstream-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # HStream
 
-Easiest interactive python web app using htmx and semantic html
+Convert your script to interactive python web app `user_said = hs.text_input("What would you like to say:")`
+
+Powered by htmx enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
 
 # Usage
 
 `pip install hstream`
 
 `hstream init`
 
@@ -33,25 +35,39 @@
 ```
 
 And as you can see we get a fully interactive web app - ready for deployment!
 
 ![hstream demo](./demo/example_demo.gif)
 
 
+# Ejection to a Django app
+
+One of the key features of HStream is not having to start over when your project outgrows the linear script structure of HStream. This out growing could be due to needing to implement more complex authentication, more custom user flows or any number of other issues I have faced in building real world PoC's with Streamlit in the past.
+
+Whatever it may be, when you do (hopefully) reach that point just run:
+
+`hstream eject`
+
+`python manage.py runserver` <- this is now running a full fledge Django instance you can edit as you please :)
+
+We'll put your current working app in your directory as a traditional Django app for you to add more routes onto the working HStream endpoint. 
+
+*Caveat:* the HStream part of the server won't follow a typical Django web app structure, but you can go ahead and develop the rest of your service in traditional Django fashion.
+
 # [Examples]((./demo))
 
 # Motivation
 
 Love Streamlit but:
 
 - impossible to customise beyond PoC phase
 - hard to reason about when extending and deploying
 - non-standard approach doesn't play nicely with existing ecosystems
 
-H-(html)-Stream is built with semantic html, FastApi and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
+H-(html)-Stream is built with semantic html, CherryPy and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
 
 ## Components
 
 `hs.markdown`
 
 `hs.text_input`
 
@@ -99,17 +115,15 @@
 
 Big thanks to the following libraries in particular
 
 - Streamlit
 - htmx
 - Yattag
 - pico css
-- MVP.css
-- FastAPI
-- uvicorn
+- CherryPy
 
 
 # Features (WIP)
 
 - [x] live server reload on file change (through univorn)
 - [x] semantic html and basic html manipulation from within script
 - [x] basic components - see below
```

### Comparing `hstream-0.1.1/hstream/HSServer.py` & `hstream-0.1.2/hstream/django_server/hs/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,166 @@
-import traceback
-from hstream.template import format_html, error_html
-import cherrypy
-from hstream.utils import set_session_var, split_code_into_blocks, pick_a_strategy
 from pathlib import Path
+from django.http import HttpResponse, HttpRequest
 from time import sleep
+from hstream.hs import hs as hs_type
+from hstream.template import format_html, error_html
+from hstream.utils import split_code_into_blocks, pick_a_strategy
+from .session_utils import get_session_var, set_session_var
 
-
-def request_server_stop_running_user_script(wait=True):
+def request_server_stop_running_user_script(request,wait=True):
     if wait:
-        while cherrypy.session.get("hs_script_running", False):
-            set_session_var("hs_script_should_stop", True)
+        while get_session_var(request, "hs_script_running", False):
+            set_session_var(request, "hs_script_should_stop", True)
             sleep(0.1)
     else:
-        set_session_var("hs_script_should_stop", True)
-    set_session_var("hs_html", "")
+        set_session_var(request, "hs_script_should_stop", True)
+    set_session_var(request, "hs_html", "")
+
+def index(request: HttpRequest):
+    request_server_stop_running_user_script(request, wait=True)
+    set_session_var(request, "hs_html_last_sent", "")
+    return HttpResponse(format_html())
+
+def run_hs(request):
+    if get_session_var(request, "hs_script_running", False):
+        HttpResponse(f"already running")
+    set_session_var(request, "hs_script_running", True)
+    try:
+        import os
+        # TODO: I'm sure theres a way to pass this filename from django through the cli :thinking
+        print(os.environ["HS_FILE_TO_RUN"])
+        hs: hs_type = run_user_code_and_return_hs_instance(os.environ["HS_FILE_TO_RUN"], request)
+    except Exception as e:
+        set_session_var(request, "hs_script_running", False)
+        set_session_var(
+            request,
+            "hs_html",
+            get_session_var(request, "hs_html", "") + error_html.format(error=e),
+        )
+        return HttpResponse(f"error: {e}")
+    set_session_var(request, "hs_script_running", False)
+    response = HttpResponse(hs.doc.getvalue())
+    hs.clear() # we should always clear the hs element otherwise we get ghost elements on next run
+    response["HX-Trigger"] = "update_content_event"
+    return response
+
+def partial_or_full_html_content(request):
+    """
+    Decides wether to send
+    1. full html content and replace existing content
+    2. nothing
+    3. partial html content and replace existing content partially
+    4. partial html content and append to existing content
+
+    We aim to balance simplicity, user interactivity, minimal updates to frontend
+    (so user doesn't see weird behaviour)
+
+    Decision is based on internal conditions of what was last sent, current html
+    content and if the script is running - see: contribution_docs/update_strategies.md
+    """
+    from hstream.utils import (
+        check_duplicate_ids_is_present,
+        get_hs_ids_with_content,
+    )
+
+    html = get_session_var(request, "hs_html", "")
+    prev_html = get_session_var(request, "hs_html_last_sent", None)
+
+    if check_duplicate_ids_is_present(html):
+        html += error_html.format(
+            error=f"Duplicate ids found in the html: {check_duplicate_ids_is_present(html)}"
+        )
+
+    update_strategy = pick_a_strategy(
+        prev_html, html, get_session_var(request,"hs_script_running", False)
+    )
+    # print(f"update strategy: {update_strategy}")
+    response = HttpResponse()
+    if get_session_var(request,"hs_script_running", False):
+        response.headers["HX-Trigger"] = "update_content_event"
+
+    if update_strategy == "1_full_replace":
+        set_session_var(request, "hs_html_partial_keys_updated", [])
+        set_session_var(request, "hs_html_last_sent", html)
+        response.content = html
+        return response
+    elif update_strategy == "2_nothing":
+        response.headers["HX-Reswap"] = "none"
+        response.headers["HX-Target"] = "none"
+        return response
+    elif update_strategy == "3_partial_replace":
+        current_hs_ids_and_content = get_hs_ids_with_content(html)
+        prev_hs_ids_and_content = get_hs_ids_with_content(prev_html)
+        for old_key, old_value in prev_hs_ids_and_content.items():
+            if old_key in get_session_var(request, "hs_html_partial_keys_updated", []):
+                break
+            new_value = current_hs_ids_and_content.get(old_key, False)
+            if new_value:
+                if old_value != new_value:
+                    set_session_var(
+                        "hs_html_partial_keys_updated",
+                        get_session_var(request,"hs_html_partial_keys_updated", [])
+                        + [old_key],
+                    )
+                    response.headers["HX-Target"] = f"#{old_key}"
+                    response.headers["HX-Reswap"] = "innerHTML"
+                    print("partial html sent")
+                    return new_value
+        # if we reach here we swap to full replacement strategy
+        response.headers["HX-Reswap"] = "none"
+        response.headers["HX-Target"] = "none"
+        return response
+    elif update_strategy == "4_partial_append":
+        # handle the case where script is running for the first time so current is more complete than old
+        # and we want to append the new content to the old content
+        set_session_var(request, "hs_html_partial_keys_updated", [])
+        set_session_var(request, "hs_html_last_sent", html)
+        response.headers["HX-Reswap"] = "beforeend"
+        response.content = html.replace(prev_html, "")
+        return response
+    else:
+        raise ValueError(f"Unknown update strategy: {update_strategy}")
 
 
-def run_user_code_and_return_hs_instance(file: Path):
+def run_user_code_and_return_hs_instance(file: Path, request: HttpRequest) -> hs_type:
     users_hs_instance = None
-    namespace = {}
+    moneky_pathed__builtins__ = __builtins__
+    moneky_pathed__builtins__['_hs_session'] = request.session
+    namespace = {"__builtins__": moneky_pathed__builtins__}
     try:
         code = open(file).read()
         for line, block in enumerate(split_code_into_blocks(code)):
-            if cherrypy.session.get("hs_script_should_stop", False):
+            if get_session_var(request, "hs_script_should_stop", False):
                 break
             compiled_code = compile(block, f"HS_STREAM_USER_FILE_LINE_{line}", "exec")
-            exec(compiled_code, namespace)
+            exec(compiled_code, namespace, )
+            try:
+                for var_name, var_value in namespace.items():
+                    if var_value.__class__.__name__ == "hs":
+                        users_hs_instance = var_value
+                html = users_hs_instance.doc.getvalue()
+                # TODO: if the script sets component values we should honour these as well
+                # for example a button reverting itself back to false after being clicked
+                # request.session = namespace['_hs_session'] 
+                set_session_var(request, "hs_html", html)
+            except:
+                pass
     except Exception as e:
         e.args = (f"Line: {line}, code: {block}", *e.args)
         raise e
     finally:
-        set_session_var("hs_script_should_stop", False)
-        for var_name, var_value in namespace.items():
-            if var_value.__class__.__name__ == "hs":
-                users_hs_instance = var_value
-                # we should always clear the hs element otherwise we get ghost elements on next run
-                users_hs_instance.clear()
-                # users_hs_instance.doc, users_hs_instance.tag, users_hs_instance.text = Doc().tagtext()
+        set_session_var(request, "hs_script_should_stop", False)
     return users_hs_instance
 
 
-class RootServerPathWorld(object):
-    def __init__(self, file: Path):
-        self.file = file
-
-    @cherrypy.expose
-    def index(self):
-        request_server_stop_running_user_script(wait=True)
-        cherrypy.session.acquire_lock()
-        cherrypy.session.clear()
-        cherrypy.session.release_lock()
-        set_session_var("hs_html_last_sent", "")
-        return format_html()
-
-    @cherrypy.expose
-    def run_hs(self):
-        # cherrypy.response.status = 204
-        if cherrypy.session.get("hs_script_running", False):
-            return "already running"
-        set_session_var("hs_script_running", True)
-        try:
-            hs = run_user_code_and_return_hs_instance(self.file)
-        except Exception as e:
-            set_session_var("hs_script_running", False)
-            set_session_var(
-                "hs_html",
-                cherrypy.session.get("hs_html", "") + error_html.format(error=e),
-            )
-            print(e)
-            return "error"
-        set_session_var("hs_script_running", False)
-        cherrypy.response.headers["HX-Trigger"] = "update_content_event"
-        return "suc"
-
-    @cherrypy.expose
-    def partial_or_full_html_content(self):
-        """
-        Decides wether to send
-        1. full html content and replace existing content
-        2. nothing
-        3. partial html content and replace existing content partially
-        4. partial html content and append to existing content
-
-        We aim to balance simplicity, user interactivity, minimal updates to frontend
-        (so user doesn't see weird behaviour)
-
-        Decision is based on internal conditions of what was last sent, current html
-        content and if the script is running - see: contribution_docs/update_strategies.md
-        """
-        from hstream.utils import (
-            check_duplicate_ids_is_present,
-            get_hs_ids_with_content,
-        )
-
-        html = cherrypy.session.get("hs_html", "")
-        prev_html = cherrypy.session.get("hs_html_last_sent", None)
-
-        if check_duplicate_ids_is_present(html):
-            html += error_html.format(
-                error=f"Duplicate ids found in the html: {check_duplicate_ids_is_present(html)}"
-            )
-
-        update_strategy = pick_a_strategy(
-            prev_html, html, cherrypy.session.get("hs_script_running", False)
-        )
-        # print(f"update strategy: {update_strategy}")
-
-        if cherrypy.session.get("hs_script_running", False):
-            cherrypy.response.headers["HX-Trigger"] = "update_content_event"
-
-        if update_strategy == "1_full_replace":
-            set_session_var("hs_html_partial_keys_updated", [])
-            set_session_var("hs_html_last_sent", html)
-            return html
-        elif update_strategy == "2_nothing":
-            cherrypy.response.headers["HX-Reswap"] = "none"
-            cherrypy.response.headers["HX-Target"] = "none"
-            return ""
-        elif update_strategy == "3_partial_replace":
-            current_hs_ids_and_content = get_hs_ids_with_content(html)
-            prev_hs_ids_and_content = get_hs_ids_with_content(prev_html)
-            for old_key, old_value in prev_hs_ids_and_content.items():
-                if old_key in cherrypy.session.get("hs_html_partial_keys_updated", []):
-                    break
-                new_value = current_hs_ids_and_content.get(old_key, False)
-                if new_value:
-                    if old_value != new_value:
-                        set_session_var(
-                            "hs_html_partial_keys_updated",
-                            cherrypy.session.get("hs_html_partial_keys_updated", [])
-                            + [old_key],
-                        )
-                        cherrypy.response.headers["HX-Target"] = f"#{old_key}"
-                        cherrypy.response.headers["HX-Reswap"] = "innerHTML"
-                        print("partial html sent")
-                        return new_value
-            # if we reach here we swap to full replacement strategy
-            cherrypy.response.headers["HX-Reswap"] = "none"
-            cherrypy.response.headers["HX-Target"] = "none"
-            return ""
-        elif update_strategy == "4_partial_append":
-            # handle the case where script is running for the first time so current is more complete than old
-            # and we want to append the new content to the old content
-            set_session_var("hs_html_partial_keys_updated", [])
-            set_session_var("hs_html_last_sent", html)
-            cherrypy.response.headers["HX-Reswap"] = "beforeend"
-            return html.replace(prev_html, "")
-        else:
-            raise ValueError(f"Unknown update strategy: {update_strategy}")
-        # panic and just send the new html
-        set_session_var("hs_html_last_sent", html)
-        set_session_var("hs_html_partial_keys_updated", [])
-        return html
-
-    @cherrypy.expose
-    def set_component_value(self, component_id, new_value=None, *args, **kwargs):
-        request_server_stop_running_user_script(wait=True)
-        if new_value == None:
-            new_value = kwargs
-        set_session_var(component_id, new_value)
-        cherrypy.response.headers["HX-Trigger"] = "trigger_run_hs_event"
-        return f"suc: {cherrypy.session[component_id]}"
+def set_component_value(request: HttpRequest,):
+    # import ipdb; ipdb.set_trace()
+    component_id = request.GET.get("component_id")
+    new_value = request.POST.get("new_value")
+    
+    request_server_stop_running_user_script(request, wait=True)
+    if new_value == None:
+        new_value = request.GET.get("new_value")
+    set_session_var(request, component_id, new_value)
+    response = HttpResponse(f"suc: {request.session[component_id]}")
+    response.headers["HX-Trigger"] = "trigger_run_hs_event"
+    return response
```

### Comparing `hstream-0.1.1/hstream/components/components.py` & `hstream-0.1.2/hstream/components/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Literal, Tuple
 from functools import wraps
 from pathlib import Path
 from inspect import getframeinfo, stack
-import cherrypy
 
 
 def component_wrapper(component_fucntion):
     @wraps(component_fucntion)
     def wrapped_component_function(self, *method_args, **method_kwargs):
         # if we arn't provided a key let make one
         key = method_kwargs.get("key", False)
@@ -55,21 +54,23 @@
                 call_signiture = (
                     f"{Path(inspect_caller.filename).stem}, {inspect_caller.lineno}"
                 )
                 key = "".join(x for x in call_signiture if x.isalpha() or x.isnumeric())
                 return key
 
     def component_value(self, default_value=None, key=None, **kwargs):
-        """Writes a component to the SH front end
+        """Writes a component to the HS front end
 
         Args:
             label (_type_, optional): Must be unique within the app. Content to write to the web front end. Defaults to None.
             default_value (_type_, optional): default value the component returns before use enters value - will always be null for text or component where user doesn't input. Defaults to None.
         """
-        return cherrypy.session.get(key, default_value)
+        # `_hs_session` is injected by the django view - it contains values the user has inputted and sent to 
+        #  the django server
+        return _hs_session.get(key, default_value)
 
 
 class Components(ComponentsGeneric):
     @component_wrapper
     def markdown(self, text: str, key: str = False, **kwargs) -> None:
         import markdown
 
@@ -422,19 +423,20 @@
     ) -> bool:
         """ """
         with self.tag(
             "button",
             ("id", key),
             ("type", "submit") if full_width else ("type", "button"),
             ("hx-trigger", "click"),
-            ("hx-post", f"/set_component_value/?component_id={key}&new_value=true"),
+            ("hx-post", f"/set_component_value?component_id={key}&new_value=true"),
             ("hx-swap", "none"),
         ):
             self.text(label)
-        cherrypy.session[key] = False
+
+        _hs_session[key] = False # set the button back to false after it has been clicked
         return lambda s: True if s in ["True", "true", True] else False
 
     def grid(self, *args, **kwargs):
         return self.tag("div", ("class", "grid"), *args, **kwargs)
 
     def write_dataframe(self, df, key, striped=False, **kwargs) -> None:
         """Writes a dataframe to the
```

### Comparing `hstream-0.1.1/hstream/components/styling_components.py` & `hstream-0.1.2/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.1/hstream/hs.py` & `hstream-0.1.2/hstream/hs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from yattag import Doc, indent
 import yattag
 
 # from hstream.components.text_input import text_input
 from hstream.components.components import Components
 from hstream.components.styling_components import StyledComponents
-from hstream.utils import set_session_var
 
 
 class HSDoc(Doc):
     class Tag(Doc.Tag):
         def __exit__(self, tpe, value, traceback):
             res = super().__exit__(tpe, value, traceback)
-            set_session_var("hs_html", indent(self.doc.getvalue()))
+            # set_session_var("hs_html", indent(self.doc.getvalue()))
             return res
 
 
 class hs(Components, StyledComponents):
-    def __init__(self) -> (yattag.SimpleDoc, yattag.Doc.tag, yattag.Doc.text):
+    def __init__(self) -> (HSDoc, HSDoc.tag, HSDoc.text):
         self.doc, self.tag, self.text = HSDoc().tagtext()
 
     def clear(self):
         self.doc, self.tag, self.text = HSDoc().tagtext()
```

### Comparing `hstream-0.1.1/hstream/templates/format_html.html` & `hstream-0.1.2/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.1/hstream/utils.py` & `hstream-0.1.2/hstream/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-import cherrypy
 import ast
 import bs4
 import collections
 from typing import Literal
 
 
-def set_session_var(component_id, new_value):
-    cherrypy.session.acquire_lock()
-    cherrypy.session[component_id] = new_value
-    cherrypy.session.release_lock()
-    return
-
-
 def check_duplicate_ids_is_present(html):
     soup = bs4.BeautifulSoup(html, features="html.parser")
     ids = [a.attrs["id"] for a in soup.find_all(attrs={"id": True})]
     ids = collections.Counter(ids)
     dups = [key for key, value in ids.items() if value > 1]
 
     return dups if len(dups) > 0 else False
```

### Comparing `hstream-0.1.1/pyproject.toml` & `hstream-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-CherryPy = "^18.9.0"
 click = "^8.1.7"
 yattag = "^1.15.2"
 ipdb = "^0.13.13"
 markdown = "^3.6"
 beautifulsoup4 = "^4.12"
+django = "^5.0.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 ipykernel = "^6.29.4"
 pandas = "^2.2.2"
 
 [build-system]
```

### Comparing `hstream-0.1.1/PKG-INFO` & `hstream-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: CherryPy (>=18.9.0,<19.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12,<5.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: django (>=5.0.6,<6.0.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: markdown (>=3.6,<4.0)
 Requires-Dist: yattag (>=1.15.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # HStream
 
-Easiest interactive python web app using htmx and semantic html
+Convert your script to interactive python web app `user_said = hs.text_input("What would you like to say:")`
+
+Powered by htmx enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
 
 # Usage
 
 `pip install hstream`
 
 `hstream init`
 
@@ -52,25 +54,39 @@
 ```
 
 And as you can see we get a fully interactive web app - ready for deployment!
 
 ![hstream demo](./demo/example_demo.gif)
 
 
+# Ejection to a Django app
+
+One of the key features of HStream is not having to start over when your project outgrows the linear script structure of HStream. This out growing could be due to needing to implement more complex authentication, more custom user flows or any number of other issues I have faced in building real world PoC's with Streamlit in the past.
+
+Whatever it may be, when you do (hopefully) reach that point just run:
+
+`hstream eject`
+
+`python manage.py runserver` <- this is now running a full fledge Django instance you can edit as you please :)
+
+We'll put your current working app in your directory as a traditional Django app for you to add more routes onto the working HStream endpoint. 
+
+*Caveat:* the HStream part of the server won't follow a typical Django web app structure, but you can go ahead and develop the rest of your service in traditional Django fashion.
+
 # [Examples]((./demo))
 
 # Motivation
 
 Love Streamlit but:
 
 - impossible to customise beyond PoC phase
 - hard to reason about when extending and deploying
 - non-standard approach doesn't play nicely with existing ecosystems
 
-H-(html)-Stream is built with semantic html, FastApi and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
+H-(html)-Stream is built with semantic html, CherryPy and htmx to provide a fast and simple framework for rapid web app development that follows traditional frontend/server architecture (or at least follow it closer than Streamlit).
 
 ## Components
 
 `hs.markdown`
 
 `hs.text_input`
 
@@ -118,17 +134,15 @@
 
 Big thanks to the following libraries in particular
 
 - Streamlit
 - htmx
 - Yattag
 - pico css
-- MVP.css
-- FastAPI
-- uvicorn
+- CherryPy
 
 
 # Features (WIP)
 
 - [x] live server reload on file change (through univorn)
 - [x] semantic html and basic html manipulation from within script
 - [x] basic components - see below
```

