# Comparing `tmp/carbon-registry-indexer-0.1.5.tar.gz` & `tmp/carbon-registry-indexer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon-registry-indexer-0.1.5.tar", last modified: Sat May 11 06:37:25 2024, max compression
+gzip compressed data, was "carbon-registry-indexer-0.1.6.tar", last modified: Sat May 11 06:43:06 2024, max compression
```

## Comparing `carbon-registry-indexer-0.1.5.tar` & `carbon-registry-indexer-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.607214 carbon-registry-indexer-0.1.5/
--rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1397 2024-05-11 06:37:25.607214 carbon-registry-indexer-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.591149 carbon-registry-indexer-0.1.5/carbon_registry_indexer/
--rw-rw-rw-   0        0        0    16921 2024-05-10 16:36:49.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.604207 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/
--rw-rw-rw-   0        0        0      467 2024-05-10 11:35:06.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/__init__.py
--rw-rw-rw-   0        0        0    10104 2024-05-10 11:09:42.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/constants.py
--rw-rw-rw-   0        0        0    15848 2024-05-10 15:23:00.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_acr.py
--rw-rw-rw-   0        0        0     4056 2024-05-10 11:33:26.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_cadt.py
--rw-rw-rw-   0        0        0    17876 2024-05-10 15:22:50.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_car.py
--rw-rw-rw-   0        0        0    10328 2024-05-09 09:57:43.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_gs.py
--rw-rw-rw-   0        0        0    18116 2024-05-10 12:19:26.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.606212 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/
--rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/__init__.py
--rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/enums.py
--rw-rw-rw-   0        0        0     8063 2024-05-08 09:13:55.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/target.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.606212 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/
--rw-rw-rw-   0        0        0     1397 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-11 06:37:25.608212 carbon-registry-indexer-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-05-11 06:37:23.000000 carbon-registry-indexer-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:43:06.729660 carbon-registry-indexer-0.1.6/
+-rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1397 2024-05-11 06:43:06.728663 carbon-registry-indexer-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 06:43:06.680215 carbon-registry-indexer-0.1.6/carbon_registry_indexer/
+-rw-rw-rw-   0        0        0    16969 2024-05-11 06:41:08.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:43:06.721149 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/
+-rw-rw-rw-   0        0        0      467 2024-05-10 11:35:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/__init__.py
+-rw-rw-rw-   0        0        0    10128 2024-05-11 06:42:12.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/constants.py
+-rw-rw-rw-   0        0        0    15872 2024-05-11 06:42:20.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_acr.py
+-rw-rw-rw-   0        0        0     4080 2024-05-11 06:42:28.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_cadt.py
+-rw-rw-rw-   0        0        0    17900 2024-05-11 06:42:31.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_car.py
+-rw-rw-rw-   0        0        0    10352 2024-05-11 06:42:33.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_gs.py
+-rw-rw-rw-   0        0        0    18140 2024-05-11 06:42:37.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:43:06.727659 carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/
+-rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/__init__.py
+-rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/enums.py
+-rw-rw-rw-   0        0        0     8079 2024-05-11 06:41:51.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/target.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:43:06.728663 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/
+-rw-rw-rw-   0        0        0     1397 2024-05-11 06:43:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2024-05-11 06:43:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:43:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-11 06:43:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 06:43:06.000000 carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-11 06:43:06.732661 carbon-registry-indexer-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-11 06:42:47.000000 carbon-registry-indexer-0.1.6/setup.py
```

### Comparing `carbon-registry-indexer-0.1.5/LICENSE` & `carbon-registry-indexer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.5/PKG-INFO` & `carbon-registry-indexer-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/__init__.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import json
 import os
 from typing import List
 
 import integrations as sync
-from integrations import constants
-from models import enums
+from carbon_registry_indexer.integrations import constants
+from carbon_registry_indexer.models import enums
 
 import pandas as pd
 from azure.storage.blob import BlobServiceClient
 
 class CarbonRegistryIndexer:
     """
     This class is the main entry point for the Carbon Registry Indexer.
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/constants.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from models import enums
+from carbon_registry_indexer.models import enums
 
 CADT_FILE_NAME = "/cadt.xlsx"
 GS_FILE_NAME = "/gs.xlsx"
 
 PROJECTS_STORAGE_FILE_NAME = "projects"
 ISSUANCES_STORAGE_FILE_NAME = "issuances"
 PROJECT_LOCATIONS_STORAGE_FILE_NAME = "project_location"
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_acr.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_acr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 import uuid
 
-from models import enums, target
+from carbon_registry_indexer.models import enums, target
 from . import utils, constants
 
 import pandas as pd
 
 def acr_projects_upsert(df, data_dir, table_name, project_locations_file_name, labels_file_name, co_benefits_file_name, estimations_file_name):
     """
     Upserts ACR projects.
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_cadt.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_cadt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import uuid
 
-from models import target
+from carbon_registry_indexer.models import target
 from . import utils
 
 import pandas as pd
 
 project_id_mapping = {}
 
 def cadt_project_upsert(df, data_dir, table_name):
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_car.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_car.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 import uuid
 
-from models import enums, target
+from carbon_registry_indexer.models import enums, target
 from . import utils, constants
 
 import pandas as pd
 
 def car_projects_upsert(df, data_dir, table_name, project_locations_file_name, labels_file_name, co_benefits_file_name, estimations_file_name):
     """
     Process CAR projects data and save to csv.
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_gs.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/sync_gs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import uuid
 from datetime import datetime
 
-from models import enums, target
+from carbon_registry_indexer.models import enums, target
 from . import utils, constants
 
 import pandas as pd
 
 def gs_projects_upsert(df, data_dir, table_name, co_benefits_file_name, estimations_file_name):
     """
     Process Gold Standard projects data and save to csv.
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/utils.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/integrations/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 
 import pandas as pd
 
 from . import constants
-from models import enums
+from carbon_registry_indexer.models import enums
 
 
 def update_csv(data, csv_path, schema=None, check_schema=False):
     """
     Updates a CSV file with new data or creates a new file if it does not exist.
 
     Parameters:
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/enums.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/enums.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/target.py` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer/models/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # models/target.py
 from sqlalchemy import Column, Integer, String, Date, Float, ForeignKey, Boolean, Enum, DateTime, func, BigInteger
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.orm import relationship
 from sqlalchemy.schema import MetaData
 from sqlalchemy.ext.declarative import declarative_base
 
-from app.api.models.enums import CorrespondingAdjustmentDeclaration, CorrespondingAdjustmentStatus, Countries, CoveredByNDC, LabelType, Methodology, ProjectSector, ProjectStatusValues, ProjectType, Registries, SustainableDevelopmentGoals, UnitMetric, UnitStatus
+from carbon_registry_indexer.models.enums import CorrespondingAdjustmentDeclaration, CorrespondingAdjustmentStatus, Countries, CoveredByNDC, LabelType, Methodology, ProjectSector, ProjectStatusValues, ProjectType, Registries, SustainableDevelopmentGoals, UnitMetric, UnitStatus
 
 # Define your schema name here
 
 Base = declarative_base()
 
 # Project Location
 class ProjectLocation(Base):
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/PKG-INFO` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/SOURCES.txt` & `carbon-registry-indexer-0.1.6/carbon_registry_indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.5/setup.py` & `carbon-registry-indexer-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name='carbon-registry-indexer',
-    version='0.1.5',
+    version='0.1.6',
     license='MIT',
     description='A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer', 
     download_url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz',
     author='Gautam P',
```

