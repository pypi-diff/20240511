# Comparing `tmp/moschitta_routing-0.1.0.tar.gz` & `tmp/moschitta_routing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moschitta_routing-0.1.0.tar", max compression
+gzip compressed data, was "moschitta_routing-0.1.1.tar", max compression
```

## Comparing `moschitta_routing-0.1.0.tar` & `moschitta_routing-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2024-05-10 01:44:52.605241 moschitta_routing-0.1.0/LICENSE
--rw-r--r--   0        0        0     3068 2024-05-10 01:35:01.599128 moschitta_routing-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 05:10:30.083706 moschitta_routing-0.1.0/moschitta_routing/__init__.py
--rw-r--r--   0        0        0     1150 2024-05-09 23:35:15.333893 moschitta_routing-0.1.0/moschitta_routing/router.py
--rw-r--r--   0        0        0     2843 2024-05-09 23:39:12.424720 moschitta_routing-0.1.0/moschitta_routing/routing.py
--rw-r--r--   0        0        0      495 2024-05-08 05:23:43.274968 moschitta_routing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 moschitta_routing-0.1.0/setup.py
--rw-r--r--   0        0        0     3370 1970-01-01 00:00:00.000000 moschitta_routing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-10 01:44:52.605241 moschitta_routing-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3007 2024-05-11 17:52:14.130681 moschitta_routing-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 05:10:30.083706 moschitta_routing-0.1.1/moschitta_routing/__init__.py
+-rw-r--r--   0        0        0     1150 2024-05-09 23:35:15.333893 moschitta_routing-0.1.1/moschitta_routing/router.py
+-rw-r--r--   0        0        0     2843 2024-05-09 23:39:12.424720 moschitta_routing-0.1.1/moschitta_routing/routing.py
+-rw-r--r--   0        0        0      496 2024-05-11 18:01:16.522173 moschitta_routing-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 moschitta_routing-0.1.1/setup.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 moschitta_routing-0.1.1/PKG-INFO
```

### Comparing `moschitta_routing-0.1.0/LICENSE` & `moschitta_routing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moschitta_routing-0.1.0/README.md` & `moschitta_routing-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Certainly! Below is a template for documentation for the `moschitta-routing` package:
-
----
-
 # Moschitta Routing Documentation
 
 The `moschitta-routing` package provides a simple and flexible routing system for the Moschitta Framework, allowing developers to define and handle HTTP routes easily.
 
 ## Installation
 
 You can install `moschitta-routing` via pip:
 
 ```bash
 pip install moschitta-routing
 ```
 
+Or use it with Poetry:
+
+```bash
+poetry add moschitta-routing
+```
+
 ## Usage
 
 ### Creating Routes
 
 Routes are created using the provided decorators (`@GET`, `@POST`, `@PUT`, `@PATCH`, `@DELETE`, `@OPTIONS`, `@HEAD`, `@CONNECT`, `@TRACE`) and registered with the router.
 
 ```python
@@ -83,10 +85,10 @@
 
 ## Contributing
 
 Contributions to `moschitta-routing` are welcome! You can contribute by opening issues for bugs or feature requests, submitting pull requests, or helping improve the documentation.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the [MIT LICENSE](LICENSE).
```

### Comparing `moschitta_routing-0.1.0/moschitta_routing/router.py` & `moschitta_routing-0.1.1/moschitta_routing/router.py`

 * *Files identical despite different names*

### Comparing `moschitta_routing-0.1.0/moschitta_routing/routing.py` & `moschitta_routing-0.1.1/moschitta_routing/routing.py`

 * *Files identical despite different names*

### Comparing `moschitta_routing-0.1.0/setup.py` & `moschitta_routing-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['moschitta_routing']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'moschitta-routing',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': 'Certainly! Below is a template for documentation for the `moschitta-routing` package:\n\n---\n\n# Moschitta Routing Documentation\n\nThe `moschitta-routing` package provides a simple and flexible routing system for the Moschitta Framework, allowing developers to define and handle HTTP routes easily.\n\n## Installation\n\nYou can install `moschitta-routing` via pip:\n\n```bash\npip install moschitta-routing\n```\n\n## Usage\n\n### Creating Routes\n\nRoutes are created using the provided decorators (`@GET`, `@POST`, `@PUT`, `@PATCH`, `@DELETE`, `@OPTIONS`, `@HEAD`, `@CONNECT`, `@TRACE`) and registered with the router.\n\n```python\nfrom moschitta_routing import GET, POST\n\n@GET(\'/users\')\ndef get_users(request):\n    # Handler logic to retrieve users\n    return [{"id": 1, "name": "John"}, {"id": 2, "name": "Alice"}]\n\n@POST(\'/users\')\ndef create_user(request):\n    # Handler logic to create a new user\n    return {"message": "User created successfully"}\n```\n\n### Handling Requests\n\nHandlers are simple functions that take a request object as input and return a JSON response. You can access request parameters within the handler function.\n\n```python\ndef get_users(request):\n    # Handler logic to retrieve users\n    return [{"id": 1, "name": "John"}, {"id": 2, "name": "Alice"}]\n```\n\n### Running the Router\n\nAfter defining routes and handlers, you can run the router to handle incoming HTTP requests.\n\n```python\nfrom moschitta_routing.router import Router\n\nrouter = Router()\n\n# Add routes here using the provided decorators\n\nif __name__ == "__main__":\n    # Run the router\n    router.run(host=\'0.0.0.0\', port=8000)\n```\n\n## API Reference\n\n### `moschitta_routing.router.Router`\n\n- `add_route(path: str, method: str, handler: Callable[[Any], Any]) -> None`: Adds a new route to the router.\n- `get(path: str, method: str = \'GET\') -> Optional[Callable[[Any], Any]]`: Retrieves the handler function associated with a specific route.\n- `__len__() -> int`: Returns the total number of routes currently defined in the router.\n- `__iter__()`: Allows iterating over all registered route paths in the router.\n\n### Decorators\n\n- `@GET(path: str) -> Callable`: Decorator for handling GET requests.\n- `@POST(path: str) -> Callable`: Decorator for handling POST requests.\n- `@PUT(path: str) -> Callable`: Decorator for handling PUT requests.\n- `@PATCH(path: str) -> Callable`: Decorator for handling PATCH requests.\n- `@DELETE(path: str) -> Callable`: Decorator for handling DELETE requests.\n- `@OPTIONS(path: str) -> Callable`: Decorator for handling OPTIONS requests.\n- `@HEAD(path: str) -> Callable`: Decorator for handling HEAD requests.\n- `@CONNECT(path: str) -> Callable`: Decorator for handling CONNECT requests.\n- `@TRACE(path: str) -> Callable`: Decorator for handling TRACE requests.\n\n## Contributing\n\nContributions to `moschitta-routing` are welcome! You can contribute by opening issues for bugs or feature requests, submitting pull requests, or helping improve the documentation.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.\n\n\n',
+    'long_description': '# Moschitta Routing Documentation\n\nThe `moschitta-routing` package provides a simple and flexible routing system for the Moschitta Framework, allowing developers to define and handle HTTP routes easily.\n\n## Installation\n\nYou can install `moschitta-routing` via pip:\n\n```bash\npip install moschitta-routing\n```\n\nOr use it with Poetry:\n\n```bash\npoetry add moschitta-routing\n```\n\n## Usage\n\n### Creating Routes\n\nRoutes are created using the provided decorators (`@GET`, `@POST`, `@PUT`, `@PATCH`, `@DELETE`, `@OPTIONS`, `@HEAD`, `@CONNECT`, `@TRACE`) and registered with the router.\n\n```python\nfrom moschitta_routing import GET, POST\n\n@GET(\'/users\')\ndef get_users(request):\n    # Handler logic to retrieve users\n    return [{"id": 1, "name": "John"}, {"id": 2, "name": "Alice"}]\n\n@POST(\'/users\')\ndef create_user(request):\n    # Handler logic to create a new user\n    return {"message": "User created successfully"}\n```\n\n### Handling Requests\n\nHandlers are simple functions that take a request object as input and return a JSON response. You can access request parameters within the handler function.\n\n```python\ndef get_users(request):\n    # Handler logic to retrieve users\n    return [{"id": 1, "name": "John"}, {"id": 2, "name": "Alice"}]\n```\n\n### Running the Router\n\nAfter defining routes and handlers, you can run the router to handle incoming HTTP requests.\n\n```python\nfrom moschitta_routing.router import Router\n\nrouter = Router()\n\n# Add routes here using the provided decorators\n\nif __name__ == "__main__":\n    # Run the router\n    router.run(host=\'0.0.0.0\', port=8000)\n```\n\n## API Reference\n\n### `moschitta_routing.router.Router`\n\n- `add_route(path: str, method: str, handler: Callable[[Any], Any]) -> None`: Adds a new route to the router.\n- `get(path: str, method: str = \'GET\') -> Optional[Callable[[Any], Any]]`: Retrieves the handler function associated with a specific route.\n- `__len__() -> int`: Returns the total number of routes currently defined in the router.\n- `__iter__()`: Allows iterating over all registered route paths in the router.\n\n### Decorators\n\n- `@GET(path: str) -> Callable`: Decorator for handling GET requests.\n- `@POST(path: str) -> Callable`: Decorator for handling POST requests.\n- `@PUT(path: str) -> Callable`: Decorator for handling PUT requests.\n- `@PATCH(path: str) -> Callable`: Decorator for handling PATCH requests.\n- `@DELETE(path: str) -> Callable`: Decorator for handling DELETE requests.\n- `@OPTIONS(path: str) -> Callable`: Decorator for handling OPTIONS requests.\n- `@HEAD(path: str) -> Callable`: Decorator for handling HEAD requests.\n- `@CONNECT(path: str) -> Callable`: Decorator for handling CONNECT requests.\n- `@TRACE(path: str) -> Callable`: Decorator for handling TRACE requests.\n\n## Contributing\n\nContributions to `moschitta-routing` are welcome! You can contribute by opening issues for bugs or feature requests, submitting pull requests, or helping improve the documentation.\n\n## License\n\nThis project is licensed under the [MIT LICENSE](LICENSE).\n\n\n',
     'author': 'Skyler Saville',
     'author_email': 'skylersaville@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `moschitta_routing-0.1.0/PKG-INFO` & `moschitta_routing-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: moschitta-routing
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Skyler Saville
 Author-email: skylersaville@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-Certainly! Below is a template for documentation for the `moschitta-routing` package:
-
----
-
 # Moschitta Routing Documentation
 
 The `moschitta-routing` package provides a simple and flexible routing system for the Moschitta Framework, allowing developers to define and handle HTTP routes easily.
 
 ## Installation
 
 You can install `moschitta-routing` via pip:
 
 ```bash
 pip install moschitta-routing
 ```
 
+Or use it with Poetry:
+
+```bash
+poetry add moschitta-routing
+```
+
 ## Usage
 
 ### Creating Routes
 
 Routes are created using the provided decorators (`@GET`, `@POST`, `@PUT`, `@PATCH`, `@DELETE`, `@OPTIONS`, `@HEAD`, `@CONNECT`, `@TRACE`) and registered with the router.
 
 ```python
@@ -94,11 +96,11 @@
 
 ## Contributing
 
 Contributions to `moschitta-routing` are welcome! You can contribute by opening issues for bugs or feature requests, submitting pull requests, or helping improve the documentation.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the [MIT LICENSE](LICENSE).
```

