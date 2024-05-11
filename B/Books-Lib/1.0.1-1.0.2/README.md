# Comparing `tmp/books_lib-1.0.1.tar.gz` & `tmp/books_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_lib-1.0.1.tar", last modified: Sat May 11 19:44:54 2024, max compression
+gzip compressed data, was "books_lib-1.0.2.tar", last modified: Sat May 11 20:53:15 2024, max compression
```

## Comparing `books_lib-1.0.1.tar` & `books_lib-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 19:44:54.202645 books_lib-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-11 19:44:52.201592 books_lib-1.0.1/Books_Lib/
--rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.1/Books_Lib/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.1/Books_Lib/books.csv
--rw-rw-rw-   0        0        0     1217 2024-05-11 19:43:08.000000 books_lib-1.0.1/Books_Lib/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-11 19:44:54.057881 books_lib-1.0.1/Books_Lib.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-11 19:44:34.000000 books_lib-1.0.1/Books_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 19:44:35.000000 books_lib-1.0.1/Books_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 19:44:34.000000 books_lib-1.0.1/Books_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-11 19:44:34.000000 books_lib-1.0.1/Books_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 19:44:34.000000 books_lib-1.0.1/Books_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-11 19:44:54.199714 books_lib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      843 2024-05-11 19:40:16.000000 books_lib-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 19:44:54.202645 books_lib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-11 19:04:50.000000 books_lib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:53:15.709821 books_lib-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-11 20:53:15.525816 books_lib-1.0.2/Books_Lib/
+-rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.2/Books_Lib/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.2/Books_Lib/books.csv
+-rw-rw-rw-   0        0        0     1012 2024-05-11 20:52:46.000000 books_lib-1.0.2/Books_Lib/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:53:15.688313 books_lib-1.0.2/Books_Lib.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-11 20:53:14.000000 books_lib-1.0.2/Books_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-11 20:53:14.000000 books_lib-1.0.2/Books_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:53:14.000000 books_lib-1.0.2/Books_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-11 20:53:14.000000 books_lib-1.0.2/Books_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 20:53:14.000000 books_lib-1.0.2/Books_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-11 20:53:15.691240 books_lib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:53:15.710793 books_lib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-11 20:52:46.000000 books_lib-1.0.2/setup.py
```

### Comparing `books_lib-1.0.1/Books_Lib/books.csv` & `books_lib-1.0.2/Books_Lib/books.csv`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.1/Books_Lib/random_books.py` & `books_lib-1.0.2/Books_Lib/random_books.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,34 +8,32 @@
         self._file = pd.read_csv(SelectBooks.FILE_PATH)
         self._title = None
         self._author = None
         self._genre = None
         self._height = None
         self._publisher = None
 
-    def gen_books(self):
-        self._books = self._file.sample()
-        self._title = self._books["Title"].values[0]
-        self._author = self._books["Author"].values[0]
-        self._genre = self._books["Genre"].values[0]
-        self._height = self._books["Height"].values[0]
-        self._publisher = self._books["Publisher"].values[0]
-
-
-    def getAuthor(_autor):
+    def buscar_Author(author):
         file = "books.csv"
-        dat = pd.read_csv(file)
-        bus = dat[dat["Author"] == _autor]
-        if bus.size == 0:
+        datos = pd.read_csv(file)
+        buscar = datos[datos["Author"] == author]
+        if buscar.size == 0:
             return "No se encontro el autor"
         else:
-            return bus
+            return buscar
 
-    def getTitle(_title):
+    def buscar_Title(title):
         file = "books.csv"
-        dat = pd.read_csv(file)
-        bus = dat[dat["Title"] == _title]
-        if bus.size == 0:
+        datos = pd.read_csv(file)
+        buscar = datos[datos["Title"] == title]
+        if buscar.size == 0:
             return "No se encontro el titulo "
         else:
-            return bus
+            return buscar
+
+
+    def getAuthor(self):
+        return self._author
+
+    def getTitle(self):
+        return self._title
```

### Comparing `books_lib-1.0.1/README.md` & `books_lib-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Puedes instalar la biblioteca usando `pip install Books_Lib`
 ## Uso
 Aquí hay un ejemplo de cómo puedes usar la biblioteca para obtener información sobre Pokémon aleatorios:
 ```python
 from Books_Lib import SelectBooks
 # Crear una instancia de SelectBooks
 _author = input("ingresa el nombre a buscar ")
-resultado = get_Author(_author)
+resultado = getAuthor(_author)
 print(resultado)
 
 ```
 ## Archivo CSV de Pokémon
 La biblioteca utiliza un archivo CSV llamado books.csv que contiene datos de Pokémon. Este archivo se incluye 
 en el paquete y se utiliza para generar los datos de los libros. Si
 necesitas acceder al archivo books.csv directamente, puedes encontrarlo en el directorio SelectBooks.
```

### Comparing `books_lib-1.0.1/setup.py` & `books_lib-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_Lib',
-   version='1.0.1',
+   version='1.0.2',
    author= 'Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_Lib'],
    package_data={'Books_Lib': ['books.csv']},
    install_requires=['pandas',
                      'twine',
```

