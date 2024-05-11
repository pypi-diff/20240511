# Comparing `tmp/moschitta_serialization-0.1.0.tar.gz` & `tmp/moschitta_serialization-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moschitta_serialization-0.1.0.tar", max compression
+gzip compressed data, was "moschitta_serialization-0.1.1.tar", max compression
```

## Comparing `moschitta_serialization-0.1.0.tar` & `moschitta_serialization-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1096 2024-05-10 04:22:24.916948 moschitta_serialization-0.1.0/LICENSE
--rw-r--r--   0        0        0     3469 2024-05-10 04:21:43.965833 moschitta_serialization-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 05:12:23.246684 moschitta_serialization-0.1.0/moschitta_serialization/__init__.py
--rw-r--r--   0        0        0      735 2024-05-10 02:14:17.999435 moschitta_serialization-0.1.0/moschitta_serialization/base_serializer.py
--rw-r--r--   0        0        0      746 2024-05-10 02:14:17.999435 moschitta_serialization-0.1.0/moschitta_serialization/json_serializer.py
--rw-r--r--   0        0        0      794 2024-05-10 02:22:41.310706 moschitta_serialization-0.1.0/moschitta_serialization/msgpack_serializer.py
--rw-r--r--   0        0        0      994 2024-05-10 02:55:48.317679 moschitta_serialization-0.1.0/moschitta_serialization/protobuf_serializer.py
--rw-r--r--   0        0        0        0 2024-05-10 02:04:29.369562 moschitta_serialization-0.1.0/moschitta_serialization/utils.py
--rw-r--r--   0        0        0      762 2024-05-10 02:17:34.521766 moschitta_serialization-0.1.0/moschitta_serialization/yaml_serializer.py
--rw-r--r--   0        0        0      632 2024-05-10 03:10:59.126132 moschitta_serialization-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 moschitta_serialization-0.1.0/setup.py
--rw-r--r--   0        0        0     3898 1970-01-01 00:00:00.000000 moschitta_serialization-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-10 04:22:24.916948 moschitta_serialization-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3361 2024-05-11 17:54:58.828525 moschitta_serialization-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 05:12:23.246684 moschitta_serialization-0.1.1/moschitta_serialization/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-10 02:14:17.999435 moschitta_serialization-0.1.1/moschitta_serialization/base_serializer.py
+-rw-r--r--   0        0        0      746 2024-05-10 02:14:17.999435 moschitta_serialization-0.1.1/moschitta_serialization/json_serializer.py
+-rw-r--r--   0        0        0      794 2024-05-10 02:22:41.310706 moschitta_serialization-0.1.1/moschitta_serialization/msgpack_serializer.py
+-rw-r--r--   0        0        0      994 2024-05-10 02:55:48.317679 moschitta_serialization-0.1.1/moschitta_serialization/protobuf_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-10 02:04:29.369562 moschitta_serialization-0.1.1/moschitta_serialization/utils.py
+-rw-r--r--   0        0        0      762 2024-05-10 02:17:34.521766 moschitta_serialization-0.1.1/moschitta_serialization/yaml_serializer.py
+-rw-r--r--   0        0        0      633 2024-05-11 18:02:44.691241 moschitta_serialization-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 moschitta_serialization-0.1.1/setup.py
+-rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 moschitta_serialization-0.1.1/PKG-INFO
```

### Comparing `moschitta_serialization-0.1.0/LICENSE` & `moschitta_serialization-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/README.md` & `moschitta_serialization-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-Here's the README for the `moschitta-serialization` package, formatted similarly to the `moschitta-routing` README:
-
----
-
-# Moschitta Serialization
+# Moschitta Serialization Documentation
 
 `moschitta-serialization` is a Python package that provides serializers for converting data to and from various formats, including JSON, MessagePack, YAML, and Protobuf.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
```

### Comparing `moschitta_serialization-0.1.0/moschitta_serialization/base_serializer.py` & `moschitta_serialization-0.1.1/moschitta_serialization/base_serializer.py`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/moschitta_serialization/json_serializer.py` & `moschitta_serialization-0.1.1/moschitta_serialization/json_serializer.py`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/moschitta_serialization/msgpack_serializer.py` & `moschitta_serialization-0.1.1/moschitta_serialization/msgpack_serializer.py`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/moschitta_serialization/protobuf_serializer.py` & `moschitta_serialization-0.1.1/moschitta_serialization/protobuf_serializer.py`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/moschitta_serialization/yaml_serializer.py` & `moschitta_serialization-0.1.1/moschitta_serialization/yaml_serializer.py`

 * *Files identical despite different names*

### Comparing `moschitta_serialization-0.1.0/pyproject.toml` & `moschitta_serialization-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moschitta-serialization"
-version = "0.1.0"
+version = "0.1.01"
 description = ""
 authors = ["Skyler Saville <skylersaville@gmail.com>"]
 readme = "README.md"
 packages = [{include = "moschitta_serialization"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `moschitta_serialization-0.1.0/setup.py` & `moschitta_serialization-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['msgpack>=1.0.8,<2.0.0', 'protobuf>=5.26.1,<6.0.0', 'pyyaml>=6.0.1,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['compile-protos = python compile_protos.py']}
 
 setup_kwargs = {
     'name': 'moschitta-serialization',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': 'Here\'s the README for the `moschitta-serialization` package, formatted similarly to the `moschitta-routing` README:\n\n---\n\n# Moschitta Serialization\n\n`moschitta-serialization` is a Python package that provides serializers for converting data to and from various formats, including JSON, MessagePack, YAML, and Protobuf.\n\n## Table of Contents\n\n- [Installation](#installation)\n- [Usage](#usage)\n- [Protobuf Serialization](#protobuf-serialization)\n- [Testing](#testing)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Installation\n\nTo install `moschitta-serialization`, you\'ll need Python 3.7 or higher, as well as Poetry for dependency management and building the package.\n\n1. **Install Poetry**: If you haven\'t already, install Poetry, a tool for dependency management and building Python packages. You can install it with the following command:\n\n    ```bash\n    curl -sSL https://install.python-poetry.org | python -\n    ```\n\n2. **Install Protobuf Compiler**: The Protobuf compiler (`protoc`) is required for compiling `.proto` files into Python code. You can install it as follows:\n\n    - On Ubuntu/Debian:\n\n        ```bash\n        sudo apt-get install protobuf-compiler\n        ```\n\n    - On macOS:\n\n        ```bash\n        brew install protobuf\n        ```\n\n    - On Windows, download pre-compiled binaries from the [Protocol Buffers GitHub repository](https://github.com/protocolbuffers/protobuf/releases). After downloading and unzipping the archive, add the `bin/` directory to your PATH.\n\n3. **Install the Package**: Navigate to the root directory of the `moschitta-serialization` package and run the following command to install the package and its dependencies:\n\n    ```bash\n    poetry install\n    ```\n\n## Usage\n\nThe `moschitta-serialization` package provides several serializers that you can use in your application. Here\'s an example of how to use the `JSONSerializer`:\n\n```python\nfrom moschitta_serialization.json_serializer import JSONSerializer\n\nserializer = JSONSerializer()\ndata = {"name": "John", "age": 30}\nserialized_data = serializer.serialize(data)\nprint(serialized_data)  # \'{"name": "John", "age": 30}\'\n```\n\nYou can use the other serializers in a similar way.\n\n## Protobuf Serialization\n\nTo use the `ProtobufSerializer`, you\'ll need to define your Protobuf messages in `.proto` files, compile these files into Python code, and import the generated classes in your application.\n\n1. **Define Protobuf Messages**: Create a `.proto` file in the `proto/` directory and define your Protobuf messages in it.\n\n2. **Compile `.proto` Files**: Run the `compile_protos.py` script to compile the `.proto` files into Python code:\n\n    ```bash\n    python compile_protos.py\n    ```\n\n3. **Import Message Types**: In your Python code, import the generated classes from the Python files:\n\n    ```python\n    from proto.person_pb2 import Person\n    ```\n\nYou can then use these classes with the `ProtobufSerializer`.\n\n## Testing\n\nThe `moschitta-serialization` package includes a suite of tests that you can run with pytest. To run the tests, navigate to the root directory of the package and run the following command:\n\n```bash\npoetry run pytest\n```\n\n## Contributing\n\nContributions to the `moschitta-serialization` package are welcome! Please submit a pull request or open an issue on the [GitHub repository](https://github.com/MoschittaFramework/moschitta-serialization).\n\n## License\n\nThis project is licensed under the terms of the [MIT License](LICENSE).\n\n',
+    'long_description': '# Moschitta Serialization Documentation\n\n`moschitta-serialization` is a Python package that provides serializers for converting data to and from various formats, including JSON, MessagePack, YAML, and Protobuf.\n\n## Table of Contents\n\n- [Installation](#installation)\n- [Usage](#usage)\n- [Protobuf Serialization](#protobuf-serialization)\n- [Testing](#testing)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Installation\n\nTo install `moschitta-serialization`, you\'ll need Python 3.7 or higher, as well as Poetry for dependency management and building the package.\n\n1. **Install Poetry**: If you haven\'t already, install Poetry, a tool for dependency management and building Python packages. You can install it with the following command:\n\n    ```bash\n    curl -sSL https://install.python-poetry.org | python -\n    ```\n\n2. **Install Protobuf Compiler**: The Protobuf compiler (`protoc`) is required for compiling `.proto` files into Python code. You can install it as follows:\n\n    - On Ubuntu/Debian:\n\n        ```bash\n        sudo apt-get install protobuf-compiler\n        ```\n\n    - On macOS:\n\n        ```bash\n        brew install protobuf\n        ```\n\n    - On Windows, download pre-compiled binaries from the [Protocol Buffers GitHub repository](https://github.com/protocolbuffers/protobuf/releases). After downloading and unzipping the archive, add the `bin/` directory to your PATH.\n\n3. **Install the Package**: Navigate to the root directory of the `moschitta-serialization` package and run the following command to install the package and its dependencies:\n\n    ```bash\n    poetry install\n    ```\n\n## Usage\n\nThe `moschitta-serialization` package provides several serializers that you can use in your application. Here\'s an example of how to use the `JSONSerializer`:\n\n```python\nfrom moschitta_serialization.json_serializer import JSONSerializer\n\nserializer = JSONSerializer()\ndata = {"name": "John", "age": 30}\nserialized_data = serializer.serialize(data)\nprint(serialized_data)  # \'{"name": "John", "age": 30}\'\n```\n\nYou can use the other serializers in a similar way.\n\n## Protobuf Serialization\n\nTo use the `ProtobufSerializer`, you\'ll need to define your Protobuf messages in `.proto` files, compile these files into Python code, and import the generated classes in your application.\n\n1. **Define Protobuf Messages**: Create a `.proto` file in the `proto/` directory and define your Protobuf messages in it.\n\n2. **Compile `.proto` Files**: Run the `compile_protos.py` script to compile the `.proto` files into Python code:\n\n    ```bash\n    python compile_protos.py\n    ```\n\n3. **Import Message Types**: In your Python code, import the generated classes from the Python files:\n\n    ```python\n    from proto.person_pb2 import Person\n    ```\n\nYou can then use these classes with the `ProtobufSerializer`.\n\n## Testing\n\nThe `moschitta-serialization` package includes a suite of tests that you can run with pytest. To run the tests, navigate to the root directory of the package and run the following command:\n\n```bash\npoetry run pytest\n```\n\n## Contributing\n\nContributions to the `moschitta-serialization` package are welcome! Please submit a pull request or open an issue on the [GitHub repository](https://github.com/MoschittaFramework/moschitta-serialization).\n\n## License\n\nThis project is licensed under the terms of the [MIT License](LICENSE).\n\n',
     'author': 'Skyler Saville',
     'author_email': 'skylersaville@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `moschitta_serialization-0.1.0/PKG-INFO` & `moschitta_serialization-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: moschitta-serialization
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Skyler Saville
 Author-email: skylersaville@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
-Here's the README for the `moschitta-serialization` package, formatted similarly to the `moschitta-routing` README:
-
----
-
-# Moschitta Serialization
+# Moschitta Serialization Documentation
 
 `moschitta-serialization` is a Python package that provides serializers for converting data to and from various formats, including JSON, MessagePack, YAML, and Protobuf.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
```

