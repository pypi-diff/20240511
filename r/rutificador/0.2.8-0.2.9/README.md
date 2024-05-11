# Comparing `tmp/rutificador-0.2.8.tar.gz` & `tmp/rutificador-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.8.tar", max compression
+gzip compressed data, was "rutificador-0.2.9.tar", max compression
```

## Comparing `rutificador-0.2.8.tar` & `rutificador-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-05 19:03:15.301237 rutificador-0.2.8/LICENSE
--rw-r--r--   0        0        0     4616 2024-05-05 19:03:15.301237 rutificador-0.2.8/README.md
--rw-r--r--   0        0        0     1147 2024-05-05 19:03:15.301237 rutificador-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      101 2024-05-05 19:03:15.301237 rutificador-0.2.8/rutificador/__init__.py
--rw-r--r--   0        0        0     9142 2024-05-05 19:03:15.301237 rutificador-0.2.8/rutificador/main.py
--rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 rutificador-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-07 01:31:36.044314 rutificador-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4991 2024-05-07 01:31:36.044314 rutificador-0.2.9/README.md
+-rw-r--r--   0        0        0     1147 2024-05-07 01:31:36.044314 rutificador-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-07 01:31:36.044314 rutificador-0.2.9/rutificador/__init__.py
+-rw-r--r--   0        0        0     7899 2024-05-07 01:31:36.044314 rutificador-0.2.9/rutificador/main.py
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 rutificador-0.2.9/PKG-INFO
```

### Comparing `rutificador-0.2.8/LICENSE` & `rutificador-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.8/README.md` & `rutificador-0.2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,26 +67,29 @@
 # Formato predeterminado (Rut con dígito verificador = 'k')
 print(rut2.formatear())  # Salida: 12345670-k
 
 # Con separador de miles y en mayúsculas
 print(rut2.formatear(separador_miles=True, mayusculas=True))  # Salida: 12.345.670-K
 ```
 
-### Validar y Formatear una lista de RUTs con y sin formato
+### Validar y Formatear una lista de RUTs en diversos formatos
+
+Al igual que con los RUTs individuales, al utilizar el método `formatear_lista_ruts` la validación se hace de forma automática cuando se trata de listas de RUTs, la diferencia es que en vez de mostrar una excepción `RunInvalidoError` separará los RUTs válidos de los inválidos. Veamos algunos ejemplos:
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
-ruts_validos = Rut.validar_lista_ruts(ruts)
-print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
+print(Rut.formatear_lista_ruts(ruts, separador_miles=True, mayusculas=True, formato=None))
 # Salida:
 RUTs válidos:
 12.345.678-5
 12.345.670-K
-98.765.432-1
+
+RUTs inválidos:
+98765432-1 - El dígito verificador '1' no coincide con el dígito verificador calculado '5'.
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
```

### Comparing `rutificador-0.2.8/pyproject.toml` & `rutificador-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.8"
+version = "0.2.9"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://pypi.org/project/rutificador/"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo", "librería", "id", "rutificador", "rut-chile"]
 classifiers = [
```

### Comparing `rutificador-0.2.8/rutificador/main.py` & `rutificador-0.2.9/rutificador/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,14 @@
     """Lanzada cuando el RUT ingresado es inválido."""
 
 
 class RutBase:
     """Representa el número base de un RUT chileno."""
 
     def __init__(self, base: str):
-        """
-        Inicializa la instancia de RutBase.
-
-        Args:
-            base (str): El número base del RUT.
-        """
         self.rut_original: str = base
         self.base: str = self.validar_y_normalizar_base(base)
 
     def validar_y_normalizar_base(self, base: str) -> str:
         """
         Valida y normaliza el número base.
 
@@ -52,20 +46,14 @@
         return self.base
 
 
 class RutDigitoVerificador(RutBase):
     """Calcula y representa el dígito verificador de un RUT chileno."""
 
     def __init__(self, base: str):
-        """
-        Inicializa la instancia de RutDigitoVerificador.
-
-        Args:
-            base (str): El número base del RUT.
-        """
         super().__init__(base)
         self.digito_verificador: str = self.calcular_digito_verificador()
 
     def calcular_digito_verificador(self) -> str:
         """
         Calcula el dígito verificador del RUT.
 
@@ -92,48 +80,35 @@
     Atributos:
         rut_string (str): El RUT en formato string.
         base (RutBase): El número base del RUT.
         digito_verificador (RutDigitoVerificador): El dígito verificador del RUT.
 
     Métodos:
         formatear: Formatea el RUT según las opciones especificadas.
-        validar_lista_ruts: Valida una lista de RUTs.
         formatear_lista_ruts: Formatea una lista de RUTs según las opciones especificadas.
     """
 
     PATRON_RUT = re.compile(RUT_REGEX)
 
     def __init__(self, rut: str):
-        """
-        Inicializa la instancia de Rut.
-
-        Args:
-            rut (str): El RUT en formato string.
-        """
         self.rut_string: str = str(rut).strip()
         self._validar_formato_rut()
         self._validar_digito_verificador()
         self.base = RutBase(self.base_string)
         self.digito_verificador = RutDigitoVerificador(self.base_string)
 
     def _validar_formato_rut(self) -> None:
-        """
-        Valida el formato del RUT.
-        """
         match = Rut.PATRON_RUT.fullmatch(self.rut_string)
         if not match:
             raise RutInvalidoError(
                 f"El formato del RUT '{self.rut_string}' es inválido."
             )
         self.base_string: str = match.group(1)
 
     def _validar_digito_verificador(self) -> None:
-        """
-        Valida el dígito verificador del RUT.
-        """
         match = Rut.PATRON_RUT.fullmatch(self.rut_string)
         digito_verificador_input = match.group(3).lower() if match.group(3) else None
         digito_verificador_calculado = RutDigitoVerificador(
             self.base_string
         ).digito_verificador
 
         if (
@@ -170,37 +145,18 @@
         if mayusculas:
             rut = rut.upper()
 
         return rut
 
     @staticmethod
     def _agregar_separador_miles(numero: str) -> str:
-        """
-        Agrega separadores de miles (puntos) a un número.
-
-        Args:
-            numero (str): El número sin separadores de miles.
-
-        Returns:
-            str: El número con separadores de miles.
-        """
         return f"{int(numero):,}".replace(",", ".")
 
     @staticmethod
-    def validar_lista_ruts(ruts: list[str]) -> dict[str, list[str]]:
-        """
-        Valida una lista de RUTs.
-
-        Args:
-            ruts (list[str]): Una lista de RUTs en formato string o numérico.
-
-        Returns:
-            dict[str, list[str]]: Un diccionario con dos claves: 'validos' e 'invalidos',
-                  cada una conteniendo una lista de RUTs válidos e inválidos respectivamente.
-        """
+    def _validar_lista_ruts(ruts: list[str]) -> dict[str, list[str]]:
         validos: list[str] = []
         invalidos: list[tuple[str, str]] = []
         for rut in ruts:
             try:
                 rut_valido: str = str(Rut(rut))
                 validos.append(rut_valido)
             except RutInvalidoError as e:
@@ -233,41 +189,40 @@
         formato=None,
     ) -> str:
         """
         Formatea una lista de RUTs según las opciones especificadas.
 
         Args:
             ruts (list[str]): Una lista de RUTs en formato string o numérico.
-            separador_miles (bool, optional): Si se deben agregar separadores de miles (puntos).
-            mayusculas (bool, optional): Si los RUTs deben estar en mayúsculas.
-            formato (str, optional): El formato de salida deseado (csv, json, xml, None).
+            separador_miles (bool, opcional): Si se deben agregar separadores de miles (puntos).
+            mayusculas (bool, opcional): Si los RUTs deben estar en mayúsculas.
+            formato (str, opcional): El formato de salida deseado (csv, json, xml, None).
 
         Returns:
             str: Una cadena con los RUTs válidos e inválidos formateados según las opciones
                 especificadas.
         """
         formato_salida: dict[str, callable] = {
             "csv": Rut._formatear_csv,
             "xml": Rut._formatear_xml,
             "json": Rut._formatear_json,
         }
-        ruts_validos_invalidos: dict[str, list[str]] = Rut.validar_lista_ruts(ruts)
+        ruts_validos_invalidos: dict[str, list[str]] = Rut._validar_lista_ruts(ruts)
         ruts_validos: list[str] = ruts_validos_invalidos["validos"]
         ruts_invalidos: list[tuple[str, str]] = ruts_validos_invalidos["invalidos"]
 
         resultado: str = ""
         if ruts_validos:
             ruts_validos_formateados: list[str] = [
                 Rut(rut).formatear(separador_miles, mayusculas) for rut in ruts_validos
             ]
             resultado += "RUTs válidos:\n"
             if formato in ("csv", "xml", "json"):
                 resultado += formato_salida[formato](ruts_validos_formateados)
             else:
-                # resultado += '\n'.join(ruts_validos_formateados)
                 resultado += "\n".join(ruts_validos_formateados)
             resultado += "\n\n"
 
         if ruts_invalidos:
             resultado += "RUTs inválidos:\n"
             for rut, error in ruts_invalidos:
                 resultado += f"{rut} - {error}\n"
```

### Comparing `rutificador-0.2.8/PKG-INFO` & `rutificador-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.8
+Version: 0.2.9
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://pypi.org/project/rutificador/
 License: MIT
 Keywords: RUT,Chile,validación,formateo,librería,id,rutificador,rut-chile
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -89,26 +89,29 @@
 # Formato predeterminado (Rut con dígito verificador = 'k')
 print(rut2.formatear())  # Salida: 12345670-k
 
 # Con separador de miles y en mayúsculas
 print(rut2.formatear(separador_miles=True, mayusculas=True))  # Salida: 12.345.670-K
 ```
 
-### Validar y Formatear una lista de RUTs con y sin formato
+### Validar y Formatear una lista de RUTs en diversos formatos
+
+Al igual que con los RUTs individuales, al utilizar el método `formatear_lista_ruts` la validación se hace de forma automática cuando se trata de listas de RUTs, la diferencia es que en vez de mostrar una excepción `RunInvalidoError` separará los RUTs válidos de los inválidos. Veamos algunos ejemplos:
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
-ruts_validos = Rut.validar_lista_ruts(ruts)
-print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
+print(Rut.formatear_lista_ruts(ruts, separador_miles=True, mayusculas=True, formato=None))
 # Salida:
 RUTs válidos:
 12.345.678-5
 12.345.670-K
-98.765.432-1
+
+RUTs inválidos:
+98765432-1 - El dígito verificador '1' no coincide con el dígito verificador calculado '5'.
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
```

