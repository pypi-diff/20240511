# Comparing `tmp/openpolicedata-0.6.tar.gz` & `tmp/openpolicedata-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.6.tar", last modified: Fri Feb 16 21:59:18 2024, max compression
+gzip compressed data, was "openpolicedata-0.7.tar", last modified: Fri May 10 23:49:27 2024, max compression
```

## Comparing `openpolicedata-0.6.tar` & `openpolicedata-0.7.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 21:59:18.500346 openpolicedata-0.6/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.6/LICENSE
--rw-rw-rw-   0        0        0     8585 2024-02-16 21:59:18.500346 openpolicedata-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4886 2024-02-16 21:57:25.000000 openpolicedata-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 21:59:18.483345 openpolicedata-0.6/openpolicedata/
--rw-rw-rw-   0        0        0      223 2024-01-15 13:28:42.000000 openpolicedata-0.6/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0    51725 2024-02-03 19:05:07.000000 openpolicedata-0.6/openpolicedata/_converters.py
--rw-rw-rw-   0        0        0     7327 2023-12-05 23:00:30.000000 openpolicedata-0.6/openpolicedata/_preproc_utils.py
--rw-rw-rw-   0        0        0      144 2023-09-26 23:30:53.000000 openpolicedata-0.6/openpolicedata/_version.py
--rw-rw-rw-   0        0        0        3 2024-02-09 00:33:17.000000 openpolicedata-0.6/openpolicedata/_version.txt
--rw-rw-rw-   0        0        0    69164 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/data.py
--rw-rw-rw-   0        0        0   101257 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    13006 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0    23297 2024-02-05 02:37:16.000000 openpolicedata-0.6/openpolicedata/datetime_parser.py
--rw-rw-rw-   0        0        0    19094 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/defs.py
-drwxrwxrwx   0        0        0        0 2024-02-16 21:59:18.483345 openpolicedata-0.6/openpolicedata/deprecated/
--rw-rw-rw-   0        0        0        0 2024-02-15 00:43:13.000000 openpolicedata-0.6/openpolicedata/deprecated/__init__.py
--rw-rw-rw-   0        0        0     4395 2024-01-18 23:54:06.000000 openpolicedata-0.6/openpolicedata/deprecated/_decorators.py
--rw-rw-rw-   0        0        0     2429 2023-09-14 23:36:09.000000 openpolicedata-0.6/openpolicedata/deprecated/_pandas.py
--rw-rw-rw-   0        0        0      455 2024-02-15 00:43:45.000000 openpolicedata-0.6/openpolicedata/deprecated/datasetsCompat.py
--rw-rw-rw-   0        0        0      479 2023-09-14 23:36:09.000000 openpolicedata-0.6/openpolicedata/deprecated/messages.py
--rw-rw-rw-   0        0        0     2246 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/deprecated/source_table_compat.py
--rw-rw-rw-   0        0        0     1831 2024-02-16 21:57:25.000000 openpolicedata-0.6/openpolicedata/exceptions.py
--rw-rw-rw-   0        0        0   119068 2024-02-03 18:08:18.000000 openpolicedata-0.6/openpolicedata/preproc.py
--rw-rw-rw-   0        0        0     1049 2023-12-08 00:58:21.000000 openpolicedata-0.6/openpolicedata/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-16 21:59:18.500346 openpolicedata-0.6/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0     8585 2024-02-16 21:59:18.000000 openpolicedata-0.6/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2024-02-16 21:59:18.000000 openpolicedata-0.6/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 21:59:18.000000 openpolicedata-0.6/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-02-16 21:59:18.000000 openpolicedata-0.6/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-16 21:59:18.000000 openpolicedata-0.6/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2825 2024-02-16 21:58:23.000000 openpolicedata-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-16 21:59:18.500346 openpolicedata-0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-16 21:59:18.500346 openpolicedata-0.6/tests/
--rw-rw-rw-   0        0        0    25113 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0    10493 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_datasets.py
--rw-rw-rw-   0        0        0      397 2023-09-14 23:36:09.000000 openpolicedata-0.6/tests/test_defs.py
--rw-rw-rw-   0        0        0    11900 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_deprecated.py
--rw-rw-rw-   0        0        0    14891 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     9592 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    14291 2024-02-16 21:57:25.000000 openpolicedata-0.6/tests/test_opd_data3.py
--rw-rw-rw-   0        0        0    16172 2024-01-15 13:33:38.000000 openpolicedata-0.6/tests/test_preproc.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:49:27.780315 openpolicedata-0.7/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.7/LICENSE
+-rw-rw-rw-   0        0        0     8202 2024-05-10 23:49:27.779317 openpolicedata-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4428 2024-05-10 00:29:14.000000 openpolicedata-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 23:49:27.755312 openpolicedata-0.7/openpolicedata/
+-rw-rw-rw-   0        0        0      223 2024-01-15 13:28:42.000000 openpolicedata-0.7/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0    55679 2024-05-10 23:48:51.000000 openpolicedata-0.7/openpolicedata/_converters.py
+-rw-rw-rw-   0        0        0     7327 2023-12-05 23:00:30.000000 openpolicedata-0.7/openpolicedata/_preproc_utils.py
+-rw-rw-rw-   0        0        0      144 2023-09-26 23:30:53.000000 openpolicedata-0.7/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0        3 2024-04-25 15:48:24.000000 openpolicedata-0.7/openpolicedata/_version.txt
+-rw-rw-rw-   0        0        0    76614 2024-05-10 23:17:18.000000 openpolicedata-0.7/openpolicedata/data.py
+-rw-rw-rw-   0        0        0   128089 2024-05-04 02:35:18.000000 openpolicedata-0.7/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    13352 2024-03-16 22:59:19.000000 openpolicedata-0.7/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0    27960 2024-05-05 19:43:40.000000 openpolicedata-0.7/openpolicedata/datetime_parser.py
+-rw-rw-rw-   0        0        0    20897 2024-05-07 22:28:55.000000 openpolicedata-0.7/openpolicedata/defs.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:49:27.766313 openpolicedata-0.7/openpolicedata/deprecated/
+-rw-rw-rw-   0        0        0        0 2024-02-15 00:43:13.000000 openpolicedata-0.7/openpolicedata/deprecated/__init__.py
+-rw-rw-rw-   0        0        0     4395 2024-01-18 23:54:06.000000 openpolicedata-0.7/openpolicedata/deprecated/_decorators.py
+-rw-rw-rw-   0        0        0     2429 2023-09-14 23:36:09.000000 openpolicedata-0.7/openpolicedata/deprecated/_pandas.py
+-rw-rw-rw-   0        0        0      455 2024-02-15 00:43:45.000000 openpolicedata-0.7/openpolicedata/deprecated/datasetsCompat.py
+-rw-rw-rw-   0        0        0      479 2023-09-14 23:36:09.000000 openpolicedata-0.7/openpolicedata/deprecated/messages.py
+-rw-rw-rw-   0        0        0     2246 2024-02-16 21:57:25.000000 openpolicedata-0.7/openpolicedata/deprecated/source_table_compat.py
+-rw-rw-rw-   0        0        0     1831 2024-02-16 21:57:25.000000 openpolicedata-0.7/openpolicedata/exceptions.py
+-rw-rw-rw-   0        0        0   122942 2024-05-09 22:33:50.000000 openpolicedata-0.7/openpolicedata/preproc.py
+-rw-rw-rw-   0        0        0     1334 2024-04-29 12:05:32.000000 openpolicedata-0.7/openpolicedata/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:49:27.778330 openpolicedata-0.7/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0     8202 2024-05-10 23:49:27.000000 openpolicedata-0.7/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1099 2024-05-10 23:49:27.000000 openpolicedata-0.7/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 23:49:27.000000 openpolicedata-0.7/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-05-10 23:49:27.000000 openpolicedata-0.7/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 23:49:27.000000 openpolicedata-0.7/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3038 2024-05-03 22:07:28.000000 openpolicedata-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 23:49:27.781312 openpolicedata-0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 23:49:27.777310 openpolicedata-0.7/tests/
+-rw-rw-rw-   0        0        0    28956 2024-04-28 23:44:50.000000 openpolicedata-0.7/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9560 2024-04-25 15:48:24.000000 openpolicedata-0.7/tests/test_datasets.py
+-rw-rw-rw-   0        0        0     2013 2024-04-25 15:48:24.000000 openpolicedata-0.7/tests/test_datasets_fixture.py
+-rw-rw-rw-   0        0        0      325 2024-03-10 15:50:52.000000 openpolicedata-0.7/tests/test_defs.py
+-rw-rw-rw-   0        0        0     9917 2024-03-10 16:04:02.000000 openpolicedata-0.7/tests/test_deprecated.py
+-rw-rw-rw-   0        0        0    19859 2024-05-10 23:40:02.000000 openpolicedata-0.7/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     9419 2024-05-01 02:02:34.000000 openpolicedata-0.7/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    15110 2024-05-02 23:27:27.000000 openpolicedata-0.7/tests/test_opd_data3.py
+-rw-rw-rw-   0        0        0    14788 2024-05-10 23:15:38.000000 openpolicedata-0.7/tests/test_preproc.py
+-rw-rw-rw-   0        0        0     4284 2024-04-29 01:52:32.000000 openpolicedata-0.7/tests/test_utils.py
```

### Comparing `openpolicedata-0.6/LICENSE` & `openpolicedata-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/PKG-INFO` & `openpolicedata-0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.6
-Summary: The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints.
+Version: 0.7
+Summary: The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints.
 Author-email: Matt Sowd <openpolicedata@gmail.com>, Paul Otto <potto@ieee.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, sowdm
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -58,86 +58,78 @@
 Requires-Dist: sodapy
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Requires-Dist: xlrd
 Provides-Extra: optional
 Requires-Dist: rapidfuzz; extra == "optional"
 Requires-Dist: msoffcrypto-tool; extra == "optional"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
+The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
 
-Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
+Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.). When data is loaded by OPD, the returned data is unmodified (with the exception of formatting known date fields) from what appears on the source's site, and OPD provides links to the original data for transparency.
 
 OpenPoliceData can be installed from the Python Package Index (PyPI):
 ```
 pip install openpolicedata
 ``` 
 
 OpenPoliceData provides access to police data with 2 simple lines of code:
 ```
 > import openpolicedata as opd
 > src = opd.Source("New Orleans")
 > data = src.load(table_type="USE OF FORCE", year=2022)
 ```
 
-> **NEW IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
+> **NEW STARTING IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
 
 - Documentation: https://openpolicedata.readthedocs.io/
 - Source Code: https://github.com/openpolicedata/openpolicedata
 - Bug Tracker: https://github.com/openpolicedata/openpolicedata/issues
 - [Latest Datasets](#latest-datasets-added)
 - [Release Notes](#release-notes-for-version-057-2023-09-05)
 - [Contributing](#contributing)
 
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 ## Latest Datasets Added to OPD
-- Chicago, IL: Traffic Citations
-- Traffic Citations for agencies across New York State
-- Buffalo Crashes and Incidents
-- Massachusetts (All Agencies): Employee and Disciplinary Records data
-- Alameda County, CA: Incidents
-- Marin County, CA: Incidents
-- Riverside, CA: Incidents
-- Albany, NY: Arrests, Calls for Service, Field Contacts, Incidents, Traffic Citations, and Use of Force
-- Chicago, IL: Pedestrian Stops
-- New York City, NY: 2022 Pedestrian Stops
-- Oakland, CA: 2022 Use of Force
-- San Diego, CA: 2022 Complaints
-- Tacoma, WA: Calls for Service, Complaints, Incidents, and Officer-Involved Shootings
+- Asheville, NC arrests, citations, complaints, incidents, pointing weapon, traffic stops, use of force, and 2023 calls for service
+- Sacramento, CA 2024 calls for service, 2021-2024 incidents, and 2023-2024 citations   
+- Albemarle County, VA: Stops
+- Norman, OK: Crashes, incidents, and traffic stops data (new) and most recent arrests, complaints and use of force data
+- Oakland, CA: Stops
+- Washington D.C.: Lawsuits against MPD
+- Bloomington, IN: Use of Force and Citations
+- Wallkill, NY: Employee and Stops
+- Bremerton, WA: Arrests, Citations, and Incidents
+- Phoenix, AZ: Officers Firearm Pointing
+- Phoenix, AZ: 2024 Calls for Service 
+- Boston, MA: Deathes in Custody
+- San Jose, CA: 2024 Calls for Service
+- Portland, OR: 2024 Calls for Service
+- Santa Monica, CA: 2022-2023 Incidents
 
-## Release Notes for Version 0.6 - 2024-02-10
+## v0.6 - 2024-05-10
 ### Added
-- Data standardization: Added function for standardizing some column names and data values
-- Added reload function to datasets module to allow reloading the datasets table (in case of an update) or loading a datasets table from a custom location
-- Added functions for getting race, gender, and age columns after standardization
-- Added merge function for merging 2 table together
-- Added function for finding related tables
-- Added a function for expanding rows that contain information on multiple officers or subjects into multiple row
-- Made opd.defs.TableType and opd.defs.columns available as opd.TableType and opd.Column
-- Added Table.urls to enable quick retrieval of URLs associated with a dataset
-- Added verbose mode to enable transparency when loading data with get_count, load_data_from_url, and load_from_url_gen
-- Added Source.load_iter to be used instead of Source.load_from_url_gen
-- Added Source.load to be used instead of Source.load_from_url
-- Added data loader for CKAN API
+- Added POINTING WEAPON (by officer) table type
+- Added data loader to combine multiple files that span a single year into a single dataset
+- Added support for more text date column formats in Arcgis loader.
+- Added url_contains input to get_count, load_iter, load, and load_from_csv of Source class to distinguish between multiple datasets matching a data request
+- Added datasets input to get_years to allow getting the years in specific datasets.
+- Added [Year Filter Guide](https://openpolicedata.readthedocs.io/en/stable/getting_started/year_filtering.html) to documentation
 ### Changed
-- Inputs to Source.get_count is now (table_type, year, ...) instead of (year, table_type, ...) so inputs go from general to specific. Original input order is deprecated and will be removed in Version 1.0.
-### Deprecated
-- Deprecated Source.load_from_url_gen. Will be removed in Version 1.0
-- Deprecated Source.load_from_url. Will be removed in Version 1.0
-### Removed
-- Removed support for Python 3.7 which has reached end of life: https://www.python.org/downloads/release/python-370/
+- Updates to standardization to handle more datasets
 ### Fixed
-- Improved speed and feedback when reading large CSV files contained in zip files
-- Source.get_agencies with a partial_name is now case-insensitive
+- Fixed year filtering for Tucson OFFICER-INVOLVED SHOOTINGS - INCIDENTS dataset. Datasets is no longer available using OpenPoliceData prior to Version 0.7.
 
 Complete change log available at: https://github.com/openpolicedata/openpolicedata/blob/main/CHANGELOG.md
 
 ## Contributing
-All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](openpolicedata@gmail.com).
+All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](mailto:openpolicedata@gmail.com).
```

### Comparing `openpolicedata-0.6/README.md` & `openpolicedata-0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,66 @@
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
+The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
 
-Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
+Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.). When data is loaded by OPD, the returned data is unmodified (with the exception of formatting known date fields) from what appears on the source's site, and OPD provides links to the original data for transparency.
 
 OpenPoliceData can be installed from the Python Package Index (PyPI):
 ```
 pip install openpolicedata
 ``` 
 
 OpenPoliceData provides access to police data with 2 simple lines of code:
 ```
 > import openpolicedata as opd
 > src = opd.Source("New Orleans")
 > data = src.load(table_type="USE OF FORCE", year=2022)
 ```
 
-> **NEW IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
+> **NEW STARTING IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
 
 - Documentation: https://openpolicedata.readthedocs.io/
 - Source Code: https://github.com/openpolicedata/openpolicedata
 - Bug Tracker: https://github.com/openpolicedata/openpolicedata/issues
 - [Latest Datasets](#latest-datasets-added)
 - [Release Notes](#release-notes-for-version-057-2023-09-05)
 - [Contributing](#contributing)
 
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 ## Latest Datasets Added to OPD
-- Chicago, IL: Traffic Citations
-- Traffic Citations for agencies across New York State
-- Buffalo Crashes and Incidents
-- Massachusetts (All Agencies): Employee and Disciplinary Records data
-- Alameda County, CA: Incidents
-- Marin County, CA: Incidents
-- Riverside, CA: Incidents
-- Albany, NY: Arrests, Calls for Service, Field Contacts, Incidents, Traffic Citations, and Use of Force
-- Chicago, IL: Pedestrian Stops
-- New York City, NY: 2022 Pedestrian Stops
-- Oakland, CA: 2022 Use of Force
-- San Diego, CA: 2022 Complaints
-- Tacoma, WA: Calls for Service, Complaints, Incidents, and Officer-Involved Shootings
+- Asheville, NC arrests, citations, complaints, incidents, pointing weapon, traffic stops, use of force, and 2023 calls for service
+- Sacramento, CA 2024 calls for service, 2021-2024 incidents, and 2023-2024 citations   
+- Albemarle County, VA: Stops
+- Norman, OK: Crashes, incidents, and traffic stops data (new) and most recent arrests, complaints and use of force data
+- Oakland, CA: Stops
+- Washington D.C.: Lawsuits against MPD
+- Bloomington, IN: Use of Force and Citations
+- Wallkill, NY: Employee and Stops
+- Bremerton, WA: Arrests, Citations, and Incidents
+- Phoenix, AZ: Officers Firearm Pointing
+- Phoenix, AZ: 2024 Calls for Service 
+- Boston, MA: Deathes in Custody
+- San Jose, CA: 2024 Calls for Service
+- Portland, OR: 2024 Calls for Service
+- Santa Monica, CA: 2022-2023 Incidents
 
-## Release Notes for Version 0.6 - 2024-02-10
+## v0.6 - 2024-05-10
 ### Added
-- Data standardization: Added function for standardizing some column names and data values
-- Added reload function to datasets module to allow reloading the datasets table (in case of an update) or loading a datasets table from a custom location
-- Added functions for getting race, gender, and age columns after standardization
-- Added merge function for merging 2 table together
-- Added function for finding related tables
-- Added a function for expanding rows that contain information on multiple officers or subjects into multiple row
-- Made opd.defs.TableType and opd.defs.columns available as opd.TableType and opd.Column
-- Added Table.urls to enable quick retrieval of URLs associated with a dataset
-- Added verbose mode to enable transparency when loading data with get_count, load_data_from_url, and load_from_url_gen
-- Added Source.load_iter to be used instead of Source.load_from_url_gen
-- Added Source.load to be used instead of Source.load_from_url
-- Added data loader for CKAN API
+- Added POINTING WEAPON (by officer) table type
+- Added data loader to combine multiple files that span a single year into a single dataset
+- Added support for more text date column formats in Arcgis loader.
+- Added url_contains input to get_count, load_iter, load, and load_from_csv of Source class to distinguish between multiple datasets matching a data request
+- Added datasets input to get_years to allow getting the years in specific datasets.
+- Added [Year Filter Guide](https://openpolicedata.readthedocs.io/en/stable/getting_started/year_filtering.html) to documentation
 ### Changed
-- Inputs to Source.get_count is now (table_type, year, ...) instead of (year, table_type, ...) so inputs go from general to specific. Original input order is deprecated and will be removed in Version 1.0.
-### Deprecated
-- Deprecated Source.load_from_url_gen. Will be removed in Version 1.0
-- Deprecated Source.load_from_url. Will be removed in Version 1.0
-### Removed
-- Removed support for Python 3.7 which has reached end of life: https://www.python.org/downloads/release/python-370/
+- Updates to standardization to handle more datasets
 ### Fixed
-- Improved speed and feedback when reading large CSV files contained in zip files
-- Source.get_agencies with a partial_name is now case-insensitive
+- Fixed year filtering for Tucson OFFICER-INVOLVED SHOOTINGS - INCIDENTS dataset. Datasets is no longer available using OpenPoliceData prior to Version 0.7.
 
 Complete change log available at: https://github.com/openpolicedata/openpolicedata/blob/main/CHANGELOG.md
 
 ## Contributing
-All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](openpolicedata@gmail.com).
+All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](mailto:openpolicedata@gmail.com).
```

### Comparing `openpolicedata-0.6/openpolicedata/_converters.py` & `openpolicedata-0.7/openpolicedata/_converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,40 @@
     (\d+)               # Lower bound of age range. Capture for reuse.
     \s?(-|_|TO)-?\s?          # - or _ between lower and upper bound with optional spaces 
     (\d+)               # Upper bound of age range. Capture for reuse.
     (\s?[-_]\s?\1\s?[-_]\s?\3)?  # Optional mistaken repeat of same pattern. 
     $                   # End of string
     """, re.VERBOSE)
 
+_p_nonlatino = re.compile(r'[\s,]*NON\-?(HISPANIC|LATINO)(\s|$)+')
+
 
 def convert(converter, col, source_name="", cats=None, std_map=None, delim=None, mult_type=None, item_num=None, 
             no_id="keep", agg_cat=False):
     std_map = {} if std_map is None else std_map
     no_id = no_id.lower()
     if no_id not in ["keep", "null", "error","test"]:
         raise ValueError(f"no_id is {no_id}. It should be 'keep', 'null', or 'error'.")
     
+    is_boolean_cols = False
+    if len(col.shape)==2: # More than 1 column was passed in
+        is_boolean_cols = (col.isnull() | col.isin(['True','False','true','false', True, False])).all().all()
+        if is_boolean_cols and mult_type!=MultType.SINGLE:
+            raise NotImplementedError(f"Multi-column input is not possible for {mult_type} case. "+
+                                      "Please submit an issue: https://github.com/openpolicedata/openpolicedata/issues")
+        if not is_boolean_cols:
+            if col.shape[1]==2:
+                # 2 columns are to be merged because 1 or the other is always null
+                col_new = col[col.columns[0]].copy()
+                is_null = col_new.isnull()
+                col_new[is_null] = col[col.columns[1]][is_null]
+                col = col_new
+            else:
+                raise ValueError(f"Unknown multi-column input to convert with columns {col.columns}")
+    
     # value_counts handles more data types when getting unique values than .unique()
     counts = col.value_counts(dropna=False)
     vals = counts.index
     if mult_type == MultType.DICT:
         return std_dict(col, std_map, converter, no_id, source_name, cats, agg_cat)
     elif mult_type == MultType.DEMO_COL:
         return std_demo_col(col, vals, std_map, item_num, converter, no_id, source_name, cats, agg_cat)
@@ -43,32 +61,78 @@
     elif mult_type == MultType.DELIMITED:
         return std_list(col, vals, std_map, delim, converter, no_id, source_name, cats, agg_cat, known_single=True)
     elif mult_type == MultType.WITH_NAME:
         return std_with_names(col, vals, std_map, item_num, converter, no_id, source_name, cats, agg_cat)
     elif mult_type == MultType.WITH_COUNTS:
         return std_with_counts(col, vals, std_map, delim, converter, no_id, source_name, cats, agg_cat)
     else:
+        if is_boolean_cols:
+            # This currently has only been tested on and needed for Bloomington use of force data
+            col_names = col.columns
+            vals = []
+            for c in col_names:
+                words = utils.split_words(c)
+                last = ""
+                v = []
+                for w in words:
+                    w = w.lower()
+                    if last=='non':
+                        last = ''
+                    elif w=='non':
+                        last = w
+                    elif w not in ['suspect', 'race', 'gender']:
+                        v.append(w)
+
+                if len(v)==0:
+                    raise ValueError(f"Unable to parse column name {c}")
+                vals.append(', '.join(v))
+
         for x in vals:
             std_map[x] = converter(x, no_id, source_name, cats, agg_cat)
             if isinstance(std_map[x], list):
                 std_map[x].sort()
                 std_map[x] = ", ".join(std_map[x])
-        return col.map(std_map)
+        
+        if is_boolean_cols:
+            std_map = {c:std_map[v] for c,v in zip(col_names, vals)}
+            def convert_bools(x):
+                out = set()
+                for c in x.index:
+                    if x[c] in ['true','True'] or x[c]==True:
+                        if isinstance(std_map[c],list):
+                            out.update(std_map[c])
+                        else:
+                            out.add(std_map[c])
+
+                out = list(out)
+                if len(out)==1:
+                    return out[0]
+                elif len(out)>1:
+                    if agg_cat and defs.get_race_cats()[defs._race_keys.LATINO] in out:
+                        return defs.get_race_cats()[defs._race_keys.LATINO]
+                    else:
+                        return ", ".join(out)
+                else:
+                    return defs._race_keys.UNSPECIFIED
+
+            return col.apply(convert_bools, axis=1)
+        else:
+            return col.map(std_map)
     
 
 def convert_off_or_civ(x, no_id, *args, **kwargs):
     orig = x
     if isinstance(x,str):
         x = x.upper()
 
     if pd.isnull(x) or x in ["MISSING"]:
         return defs._roles.UNSPECIFIED
     elif x in ["OFFICER"]:
         return defs._roles.OFFICER
-    elif x in ["SUBJECT","CIVILIAN"]:
+    elif x in ["SUBJECT","CIVILIAN",'CITIZEN']:
         return defs._roles.SUBJECT
     elif no_id in ["error","test"]:
         raise ValueError(f"Unknown person type {orig}")
     else:
         return orig if no_id=="keep" else ""
     
 
@@ -92,14 +156,15 @@
     p_above = re.compile(r"(\d+) (AND|&) (ABOVE|OLDER)",re.IGNORECASE)
     p_decade = re.compile(r"^(\d+)s$", re.IGNORECASE)
     p_range = re.compile(r"^(\d+)\s?<(=?)\s?\w+\s?<(=?)\s?(\d+)?$", re.IGNORECASE)
 
     orig=x
     if type(x)==str:
         x = x.upper().strip()
+        x = re.sub(r'[A-Z] \- ','', x)  # Oakland Stops data includes a category label up front such as: 'B - 18-29'. Remove this.
     if isinstance(x,str) and _p_age_range.search(x)!=None:
         return _p_age_range.sub(r"\1-\3", x)
     elif isinstance(x,str) and p_over.search(x)!=None:
         return p_over.sub(r"\2-120", x)
     elif isinstance(x,str) and p_plus.search(x)!=None:
         return p_plus.sub(r"\1-120", x)
     elif isinstance(x,str) and p_plus2.search(x)!=None:
@@ -243,14 +308,89 @@
                 raise KeyError(f"Unknown race value for {source_name} data: {orig}")
             else:
                 return orig if no_id=="keep" else ""
         else:
             # Replace numerical code with default value
             x = map_dict[x]
 
+    if pd.isnull(x):
+        if has_unspecified:
+            return race_cats[defs._race_keys.UNSPECIFIED]
+        elif no_id=="error":
+            raise ValueError(f"Null value found in race column: {orig}")
+        else:
+            # Same result whether no_id is keep or null
+            return ""
+                 
+    x = x.strip().upper()
+
+    if source_name in ["Austin", "Bloomington", "New York City", "St. John", "Louisville", "Charleston", 
+                        "Los Angeles", "Dallas","Chicago"]:
+        # Handling dataset-specific letter codes
+        if source_name=="Austin":
+            # Per email with Kruemcke, Adrian <Adrian.Kruemcke@austintexas.gov> on 2022-06-17
+            map_dict = {"M":"Middle Eastern", "P":"Pacific Islander/Native Hawaiian", "N":"Native American/Alaskan", "O":"Other"}
+        elif source_name=="Bloomington":
+            # https://data.bloomington.in.gov/Police/Citizen-Complaints/kit3-8bua/about_data
+            map_dict = {
+                "A": "Asian/Pacific Island, Non-Hispanic", 
+                "B": "African American, Non-Hispanic", 
+                "C": "Hawaiian/Other Pacific Island, Hispanic", 
+                "H": "Hawaiian/Other Pacific Island, Non-Hispanic", 
+                "I": "Indian/Alaskan Native, Non-Hispanic", 
+                "K": "African American, Hispanic", 
+                "L": "Caucasian, Hispanic", 
+                "N": "Indian/Alaskan Native, Hispanic", 
+                "P": "Asian/Pacific Island, Hispanic", 
+                "S": "Asian, Non-Hispanic", 
+                "T": "Asian, Hispanic", 
+                "U": "Unknown", 
+                "W": "Caucasian, Non-Hispanic"
+            } 
+        elif source_name == "New York City":
+            # https://www.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/SQF-File-Documentation.zip
+            map_dict = {"P":"Black-Hispanic", "Q":"White-Hispanic", "X":"Unknown","Z":"Other"}
+        elif source_name == "St. John":
+            # https://stjohnin.gov/PD/PDI/Warnings/2019Warnings.php
+            map_dict = {"L":"White/Hispanic/Latin","M":"Multiracial","N":"Asian Indian"}
+        elif source_name == "Louisville":
+            map_dict = {"A":"Asian/Pacific Islander", "U":"Undeclared", "IB":"Indian/India/Burmese", "M":"Middle Eastern Descent","AN":"Alaskan Native"}
+        elif source_name=="Charleston":
+            # Based on correspondance with City of Charleston Ombudsman
+            map_dict = {"A":"Asian or Pacific Islander", "AI": "Alaskan or American Indian", "AP":"Asian or Pacific Islander",
+                        "BK":"Black","MR":"Multi-Racial","AO":"Other"}
+        elif source_name=="Los Angeles":
+            # https://data.lacity.org/Public-Safety/Traffic-Collision-Data-from-2010-to-Present/d5tf-ez2w
+            map_dict = {"A":"Other Asian", "B":"Black", "C":"Chinese", "D":"Cambodian", "F":"Filipino", 
+                        "G":"Guamanian", "H":"Hispanic/Latin/Mexican", "I":"American Indian/Alaskan Native", 
+                        "J":"Japanese", "K":"Korean", "L":"Laotian", "O":"Other", "P":"Pacific Islander", 
+                        "S":"Samoan", "U":"Hawaiian", "V":"Vietnamese", "W":"White", "X":"Unknown", "Z":"Asian Indian"}
+        elif source_name=="Dallas":
+            # Based on Bloomington and St. John usage as well as names associated with usage
+            map_dict = {"L":"Caucasian, Hispanic"}
+        elif source_name=="Chicago":
+            # https://home.chicagopolice.org/wp-content/uploads/2020/08/ISR-Data-Dictionary.csv
+            map_dict = {
+                'BLK' : 'BLACK',
+                'WHI' : 'WHITE',
+                'API' : 'ASIAN/PACIFIC ISLANDER',
+                'WBH' : 'BLACK HISPANIC',
+                'WWH' : 'WHITE HISPANIC',
+                'I' : 'AMER IND/ALASKAN NATIVE',
+                'U' : 'UNKNOWN',
+                'P' : 'NATIVE HAWAIIAN OR OTHER PACIFIC ISLANDER',
+                'WHT' : 'WHITE'
+            }
+
+        if x in map_dict:
+            x = map_dict[x].upper()
+
+    if _p_nonlatino.search(x) and len(m:=_p_nonlatino.sub('', x))>0:
+        x = m
+
     if isinstance(x,str):
         # Look for code: {Race_Abbreviation_Initial} {- or =} {Full name}
         abbrev_full_match = re.search(r"^([\w\s/\.]+)\s?[-=]\s?([\w\s/\.]+)$",x)
         if abbrev_full_match and any([len(x)==1 for x in abbrev_full_match.groups()]):
             x = [x for x in abbrev_full_match.groups() if len(x)>1][0].strip()
 
         delims = [" and ", ",",'|','/']
@@ -262,15 +402,15 @@
                                               'asian/pacis','unk/oth','oth/unk', 'black/africanamerican','hispanic/latino',
                                               "americanindian/alaskanative",'a/indian'] and \
             not any([x.lower() in ['unknown','other'] for x in x.split(delim[0])]):
             # Treat this as a list of races
             delim = delim[0]
             race_list = []
             for v in x.split(delim):
-                if (v=="INDIAN" and "BURMESE" in x):
+                if (v=="INDIAN" and "BURMESE" in x) or v=='N':  # N is non-Latino, which can be ignored
                     # Handle special case to prevent setting someone from country of India to Indigenous
                     continue
                 new_val = _create_race_lut(v, no_id, source_name, race_cats, agg_cat, known_single=True)
                 if isinstance(new_val, list):
                     race_list.extend(new_val)
                 else:
                     race_list.append(new_val)
@@ -295,98 +435,43 @@
                 # Simplify to AAPI
                 return race_cats[defs._race_keys.AAPI]
             elif agg_cat and has_latino and race_cats[defs._race_keys.LATINO] in race_list:
                 # Category is Latino of all races
                 return race_cats[defs._race_keys.LATINO]
             else:
                 return race_list
-                 
-        # Clean x
-        x = x.upper().replace("_", " ").replace("*","").replace("-"," ").replace(".","")
-        x = x.strip()
-
-        if source_name in ["Austin", "Bloomington", "New York City", "St. John", "Louisville", "Charleston", 
-                           "Los Angeles", "Dallas","Chicago"]:
-            # Handling dataset-specific letter codes
-            if source_name=="Austin":
-                # Per email with Kruemcke, Adrian <Adrian.Kruemcke@austintexas.gov> on 2022-06-17
-                map_dict = {"M":"Middle Eastern", "P":"Pacific Islander/Native Hawaiian", "N":"Native American/Alaskan", "O":"Other"}
-            elif source_name=="Bloomington":
-                # https://data.bloomington.in.gov/dataset/bloomington-police-department-employee-demographics
-                map_dict = {"K":"African American, Hispanic", "L":"Caucasian, Hispanic", "N":"Indian/Alaskan Native, Hispanic",
-                            "P":"Asian/Pacific Island, Hispanic"}
-            elif source_name == "New York City":
-                # https://www.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/SQF-File-Documentation.zip
-                map_dict = {"P":"Black-Hispanic", "Q":"White-Hispanic", "X":"Unknown","Z":"Other"}
-            elif source_name == "St. John":
-                # https://stjohnin.gov/PD/PDI/Warnings/2019Warnings.php
-                map_dict = {"L":"White/Hispanic/Latin","M":"Multiracial","N":"Asian Indian"}
-            elif source_name == "Louisville":
-                map_dict = {"A":"Asian/Pacific Islander", "U":"Undeclared", "IB":"Indian/India/Burmese", "M":"Middle Eastern Descent","AN":"Alaskan Native"}
-            elif source_name=="Charleston":
-                # Based on correspondance with City of Charleston Ombudsman
-                map_dict = {"A":"Asian or Pacific Islander", "AI": "Alaskan or American Indian", "AP":"Asian or Pacific Islander",
-                            "BK":"Black","MR":"Multi-Racial","AO":"Other"}
-            elif source_name=="Los Angeles":
-                # https://data.lacity.org/Public-Safety/Traffic-Collision-Data-from-2010-to-Present/d5tf-ez2w
-                map_dict = {"A":"Other Asian", "B":"Black", "C":"Chinese", "D":"Cambodian", "F":"Filipino", 
-                            "G":"Guamanian", "H":"Hispanic/Latin/Mexican", "I":"American Indian/Alaskan Native", 
-                            "J":"Japanese", "K":"Korean", "L":"Laotian", "O":"Other", "P":"Pacific Islander", 
-                            "S":"Samoan", "U":"Hawaiian", "V":"Vietnamese", "W":"White", "X":"Unknown", "Z":"Asian Indian"}
-            elif source_name=="Dallas":
-                # Based on Bloomington and St. John usage as well as names associated with usage
-                map_dict = {"L":"Caucasian, Hispanic"}
-            elif source_name=="Chicago":
-                # https://home.chicagopolice.org/wp-content/uploads/2020/08/ISR-Data-Dictionary.csv
-                map_dict = {
-                    'BLK' : 'BLACK',
-                    'WHI' : 'WHITE',
-                    'API' : 'ASIAN/PACIFIC ISLANDER',
-                    'WBH' : 'BLACK HISPANIC',
-                    'WWH' : 'WHITE HISPANIC',
-                    'I' : 'AMER IND/ALASKAN NATIVE',
-                    'U' : 'UNKNOWN',
-                    'P' : 'NATIVE HAWAIIAN OR OTHER PACIFIC ISLANDER',
-                    'WHT' : 'WHITE'
-                }
 
-            if x.upper() in map_dict:
-                x = map_dict[x.upper()].upper()
+    # Clean x
+    x = x.upper().replace("_", " ").replace("*","").replace("-","").replace(".","").strip()
 
     if pd.notnull(x):
         # Check if value is part of race_cats
         # This is particularly necessary for custom race_cats dicts
         for k,v in race_cats.items():
             # Key is always be a string
             if k.upper()==str(orig).upper() or k.upper()==str(x) or str(v)==str(orig).upper() or str(v)==str(x):
                 return v
-    
-    if pd.isnull(x):
-        if has_unspecified:
-            return race_cats[defs._race_keys.UNSPECIFIED]
-        elif no_id=="error":
-            raise ValueError(f"Null value found in race column: {orig}")
-        else:
-            # Same result whether no_id is keep or null
-            return ""
         
     def is_latino(x):
         if isinstance(x,str):
             x = x.upper().replace("-","").replace(" ","")
-            return ("HISPANIC" in x and "NONHISPANIC" not in x) or \
-                ("LATINO" in x and "NONLATINO" not in x)
+            return "HISPANIC" in x or "LATINO" in x
         else:
             return False
 
+    x_no_space = x.replace(" ","")
     if has_unspecified and (x in ["MISSING","NOT SPECIFIED", "", "NOT RECORDED","N/A", "NOT REPORTED", "NONE"] or \
-        (type(x)==str and ("NO DATA" in x or ("NOT APP" in x and x not in ["NOT APPLICABLE (NON-U.S.)",'NOT APPLICABLE (NON US)']) or "NO RACE" in x or "NULL" in x))):
+        (type(x)==str and ("NO DATA" in x or ("NOT APP" in x and x not in ["NOT APPLICABLE (NONUS)",'NOT APPLICABLE (NON US)']) or "NO RACE" in x or "NULL" in x))):
         return race_cats[defs._race_keys.UNSPECIFIED]
-    if has_white and x.replace(" ","") in ["W", "CAUCASIAN", "WN", "WHITE", "WHTE","WHITENONLATINO", "WHITENONHISPANIC", "WHITE,OTHER"]:  # WN = White-Non-Hispanic
+    if has_white and x_no_space in ["W", "CAUCASIAN", "WN", "WHITE", "WHTE", "WHITE,OTHER"]:  # WN = White-Non-Hispanic
         return race_cats[defs._race_keys.WHITE]
-    if has_black and (x in ["B", "AFRICAN AMERICAN", "BLCK", "BLK", "BLACE"] or re.search("BLACK?($|[^A-Za-z])",x)) and not is_latino(x):
+    if has_black and (x in ["B", "AFRICAN AMERICAN", "BLCK", "BLK", "BLACE",'AFR AMERICAN'] or \
+                      x_no_space in ["AFRICANAMERICAN"] or \
+                      re.search("BLACK?($|[^A-Za-z])",x)) \
+                      and not is_latino(x):
         if x.count("BLACK") > 1:
             raise ValueError(f"The value of {x} likely contains the races for multiple people")
         return race_cats[defs._race_keys.BLACK]
     if has_south_asian and ((x in ["SOUTH ASIAN"] or ("ASIAN" in x and "INDIAN" in x)) or \
                             x in ["EAST INDIAN"]):
         if defs._race_keys.SOUTH_ASIAN in race_cats:
              return race_cats[defs._race_keys.SOUTH_ASIAN]
@@ -394,45 +479,46 @@
             return race_cats[defs._race_keys.MIDDLE_EASTERN_SOUTH_ASIAN] 
     if has_me and (x in ["ME","ARABIC"] or "MIDDLE EAST" in x) and "AFRICA" not in x:  # Ignore Middle Eastern or North African
         if "SOUTH ASIAN" in x:
             if has_me_or_sa:
                 return race_cats[defs._race_keys.MIDDLE_EASTERN_SOUTH_ASIAN]
         else:
             return race_cats[defs._race_keys.MIDDLE_EASTERN] if defs._race_keys.MIDDLE_EASTERN in race_cats else race_cats[defs._race_keys.MIDDLE_EASTERN_SOUTH_ASIAN]
-    if (has_asian or has_aapi) and (x in ["A", 'ORIENTAL'] or "ASIAN" in x.replace("CAUCASIAN","")) and x not in ["SOUTHWEST ASIAN"] and "INDIAN" not in x:
+    if (has_asian or has_aapi) and (x in ["A", 'ORIENTAL', 'AA', 'ASN'] or "ASIAN" in x.replace("CAUCASIAN","")) and x not in ["SOUTHWEST ASIAN"] and "INDIAN" not in x:
         if has_aapi and ("PAC" in x or "HAWAI" in x):
             return race_cats[defs._race_keys.AAPI] 
         else:
             return race_cats[defs._race_keys.ASIAN] if has_asian else race_cats[defs._race_keys.AAPI]
-    if (has_pi or has_aapi) and ("HAWAI" in x or "PACIFICIS" in x.replace(" ","").replace("_","") or \
-                                 "PACISL" in x.replace(" ","")):
+    if (has_pi or has_aapi) and ("HAWAI" in x or "PACIFIC" in x_no_space or \
+                                 "PACISL" in x_no_space):
         return race_cats[defs._race_keys.PACIFIC_ISLANDER] if has_pi else race_cats[defs._race_keys.AAPI]
-    if has_latino and x in ["H", "WH", "HISPANIC", "LATINO", "HISPANIC OR LATINO", "LATINO OR HISPANIC", "HISPANIC/LATINO", "LATINO/HISPANIC",'HISPANIC/LATIN/MEXICAN']:
+    if has_latino and x in ["H", "WH", "HISPANIC", "LATINO", "HISPANIC OR LATINO", "LATINO OR HISPANIC", 
+                            "HISPANIC/LATINO", "LATINO/HISPANIC",'HISPANIC/LATIN/MEXICAN','HISP']:
         return race_cats[defs._race_keys.LATINO] 
     if has_indigenous and (x in ["I", "INDIAN", "ALASKAN NATIVE", "AN", "AI", "AL NATIVE","A/INDIAN", "NAT AM"] or "AMERICAN IND" in x.replace("II","I") or \
-        "NATIVE AM" in x or  "AMERIND" in x.replace(" ","") or "ALASK" in x or "AMIND" in x.replace(" ","") or \
+        "NATIVE AM" in x or  "AMERIND" in x_no_space or "ALASK" in x or "AMIND" in x_no_space or \
         "NAT AMER" in x):
         return race_cats[defs._race_keys.INDIGENOUS] 
     if has_multiple and ("OR MORE" in x or "MULTI" in x or \
-        x.replace(" ","") in ["MIXED","BIRACIAL","MIXEDRACE","MORE THAN TWO RACES".replace(" ",""),
+        x_no_space in ["MIXED","BIRACIAL","MIXEDRACE","MORE THAN TWO RACES".replace(" ",""),
                               "MORE THAN 2 RACES".replace(" ","")]):
         return race_cats[defs._race_keys.MULTIPLE]
     if defs._race_keys.OTHER_UNKNOWN in race_cats and "UNK" in x and "OTH" in x:
         return race_cats[defs._race_keys.OTHER_UNKNOWN]
     if defs._race_keys.UNKNOWN in race_cats and  ("UNK" in x or x in ["U", "UK"]):
         return race_cats[defs._race_keys.UNKNOWN]
     if defs._race_keys.OTHER in race_cats and (x in ["O","OTHER","OTH"] or "OTHER UNCLASS" in x or "OTHER RACE" in x):
         return race_cats[defs._race_keys.OTHER]
     
     if agg_cat:
         # This attempts to categorize more cases based on U.S. Census definitions:
         # https://www.census.gov/programs-surveys/decennial-census/decade/2020/planning-management/release/faqs-race-ethnicity.html
         # Cases include here are based on data values that have been observed
-        if has_latino and (("HISP" in x and "NONHISP" not in x.replace(" ","")) or \
-                           ("LATINO" in x and "NONLATINO" not in x.replace(" ","")) or \
+        if has_latino and (("HISP" in x and "NONHISP" not in x_no_space) or \
+                           ("LATIN" in x and "NONLATINO" not in x_no_space) or \
                             x in ["MEXICAN"]):
             # agg_cat forces Latino of all races
             return race_cats[defs._race_keys.LATINO] 
         elif has_black and x in ["EAST AFRICAN"]:
             return race_cats[defs._race_keys.BLACK]
         elif has_white and x in ["BOSNIAN"]:
             return race_cats[defs._race_keys.WHITE]
@@ -447,32 +533,34 @@
             return race_cats[defs._race_keys.ASIAN] if has_asian else race_cats[defs._race_keys.AAPI]
         elif (has_pi or has_aapi) and x in ["POLYNESIAN","SAMOAN","GUAMANIAN"]:
             return race_cats[defs._race_keys.PACIFIC_ISLANDER] if has_pi else race_cats[defs._race_keys.AAPI]
         elif no_id=="error":
             raise ValueError(f"Unknown value in race column: {orig}")
         elif no_id=="test":
             if x in ["MALE","FEMALE","GIVING ANYTHING OF VALUE","REFUSED", "NA","M","F","OTHER/NOT REPORTED", 
-                     'UNOCCUPIED VEHICLE','MIDDLE EASTERN OR NORTH AFRICAN','P','PAKISTANI','DUPLICATE'] or \
+                     'UNOCCUPIED VEHICLE','MIDDLE EASTERN OR NORTH AFRICAN','P','PAKISTANI','DUPLICATE',
+                     'NOT AVAILABLE'] or \
                 (source_name in ["Chapel Hill","Lansing","Fayetteville"] and x in ["S","P"]) or \
                 (source_name=="Burlington" and x in ["EXPUNGED"]) or \
                 (source_name in ["Cincinnati","San Diego"] and x in ["F","S","P"]) or \
                 (source_name in ["Columbia"] and x in ["M","P",'34']) or \
                 (source_name in ["Urbana"] and x in ["BUSINESS OR OTHER"]) or \
                 (source_name in ["Bloomington","Beloit"] and x in ["M"]) or \
                 (source_name in ["Beloit"] and x in ["L"]) or \
                 (source_name in ["St. John"] and x in ["K","P"]) or \
                 (source_name in ["Rutland"] and x in ["M","R"]) or \
                 (source_name in ["Dallas"] and x in ["NA"]) or \
                 (source_name in ["Sacramento"] and x in ["CUBAN","CARRIBEAN"]) or \
                 (source_name in ["New York City"] and x in ["SOUTHWEST"]) or \
-                (source_name in ["New York City"] and x in ["SOUTHWEST"]) or \
+                (source_name in ["Wallkill"] and x in ["IND",'N','M']) or \
                 (x=="UN" and source_name=="State Police") or \
                 (x=="P" and source_name=="Pittsfield") or \
                 (x=="PENDING RELEASE" and source_name=="Portland") or \
                 (x=="IRAK" and source_name=="Chattanooga") or \
+                (x=="N" and source_name=="Bremerton") or \
                 (x=="W\nW" and source_name=="Sparks") or \
                 (x in ['E','P'] and source_name=="Tucson") or \
                 ("DOG" in x) or \
                 (source_name in ["New Orleans"] and "NOT APPLICABLE (NON" in x) or \
                 (source_name in ["Detroit", "Fairfax County"] and x in ["N","SELECT","UNVERIFIED",'240','160','180','P','120']) or \
                 x in ["OTHER / MIXED RACE", "UNDISCLOSED", "OR SPANISH ORIGIN","PREFER NOT TO SAY","OTHERBLEND","UNDECLARED"] or \
                 len(orig)>100:
@@ -570,15 +658,15 @@
     elif defs._gender_keys.OTHER in gender_cats and x in ["OTHER", "O"]:
         return gender_cats[defs._gender_keys.OTHER]
     elif defs._gender_keys.TRANSGENDER in gender_cats and x in ["TRANSGENDER","TRANSGENDERED"]:
         return gender_cats[defs._gender_keys.TRANSGENDER]
     elif defs._gender_keys.GENDER_NONBINARY in gender_cats and x in ["NONBINARY"]:
         return gender_cats[defs._gender_keys.GENDER_NONBINARY]
     elif defs._gender_keys.TRANSGENDER_OR_GENDER_NONCONFORMING in gender_cats and (x in [
-        "Gender Diverse (gender non-conforming and/or transgender)".upper().replace("-","").replace("_","").replace(" ",""),
+        "Gender Diverse (gender non-conforming and/or transgender)".upper().replace("-","").replace(" ",""),
         "GENDERNONCONFORMING"] or "TGNC" in x):
         return gender_cats[defs._gender_keys.TRANSGENDER_OR_GENDER_NONCONFORMING]
     elif defs._gender_keys.TRANSGENDER_MALE in gender_cats and (x in ["TRANSGENDER MALE".replace(" ","")] or \
         "TRANSGENDERMAN" in x or \
         (source_name=="Los Angeles" and x=="T")):
         return gender_cats[defs._gender_keys.TRANSGENDER_MALE]
     elif defs._gender_keys.TRANSGENDER_FEMALE in gender_cats and \
@@ -590,34 +678,38 @@
         return gender_cats[defs._gender_keys.GENDER_NONCONFORMING]
     elif defs._gender_keys.UNKNOWN in gender_cats and \
         (x in ["U","UK", "UNABLE TO DETERMINE".replace(" ","")] or "UNK" in x):
         return gender_cats[defs._gender_keys.UNKNOWN]
     
     if no_id=="test":
         bad_data = ["BLACK","WHITE",'HISPANIC','ASIAN','FEMALE10','DUPLICATE']
-        if "EXEMPT" in x or x in ["DATAPENDING", "NOTAPPLICABLE","N/A",'NA'] or ("BUSINESS" in x and source_name=="Cincinnati"):
+        if "EXEMPT" in x or x in ["DATAPENDING", "NOTAPPLICABLE","N/A",'NA','NOTAVAILABLE'] or ("BUSINESS" in x and source_name=="Cincinnati"):
             return orig
         elif x in bad_data or \
             (source_name=="New York City" and (x=="Z" or x.isdigit())) or \
             (source_name=="New York" and x in ["Organization".upper(), "X"]) or \
             (source_name=="Baltimore" and x in ["Y","Z"]) or \
             (source_name=="Urbana" and x in ["."]) or \
             (source_name=="Greensboro" and x in ["ASIAN"]) or \
             (source_name=="Columbia" and x in ["B"]) or \
             (source_name=="Burlington" and x in ["EXPUNGED"]) or \
             (source_name=="Fairfax County" and x in ["X",'O']) or \
+            (source_name=='Albemarle County' and x in ['N']) or \
             (source_name in ["Seattle","New Orleans","Menlo Park","Rutland"] and x in ["D","N"]) or \
             (source_name=="Los Angeles County" and x=="0") or \
-            (x in ["W","NA"] and source_name in ["Cincinnati","Beloit"]) or \
+            (x in ["W","NA"]) or \
+            (x in ['L'] and source_name=='Bloomington') or \
+            (x in ['GROUP'] and source_name=='Asheville') or \
             (x=="MA" and source_name in ["Lincoln"]) or \
             (x=="P" and source_name=="Fayetteville") or \
             (x=="5" and source_name=="Lincoln") or \
             (x in ["MALE,MALE"] and source_name=="Chattanooga") or \
             (x=="PENDINGRELEASE" and source_name=="Portland") or \
             (x in ["N","H"] and source_name=="Los Angeles") or \
+            (source_name=='Bremerton' and x in ['B', 'W', 'A','I']) or \
             (x=="X" and source_name in ["Sacramento", "State Police", "Washington D.C.","Northampton"]) or \
             "DOG" in x or \
             x in ["UNDISCLOSE","UNDISCLOSED","PREFER TO SELF DESCRIBE".replace(" ",""),'NONBINARY/THIRDGENDER',
                   "PREFER NOT TO SAY".replace(" ",""),"TGNC/OTHER","REFUSED",'UNVERIFIED','NONBINARY/OTHERX','UNOCCUPIEDVEHICLE'] or \
             source_name == "Buffalo":
             return orig
         else:
@@ -634,15 +726,16 @@
     elif isinstance(x,Number) or pd.api.types.is_bool(x) or x.isdigit():  # is_bool handles numpy.bool_ type
         x = int(x)
         if x<0:
             return x
         else:
             return "INJURED" if x>0 else "NO INJURY"
     orig = x
-    x = x.upper().replace('-',' ').replace('*','').strip()
+    x = x.upper().replace('-',' ').replace('*','').replace('SUBJECT','').strip()
+    x = re.sub(r'OF[FI]{2}CER','', x).strip()  # Handle misspelling officer
 
     if len(x)==0:
         return "UNSPECIFIED"
     elif len(words:=x.split('\n'))>1:
         words = [_create_injury_lut(y, no_id, source_name, cats) for y in words]
         for m in ['FATAL','INJURED']:
             if m in words:
@@ -654,25 +747,26 @@
     fatal_words = ["FATAL","KILLED",'DECEASED',"DEATH", 'FATAL INJURY']
     contains_fatal = any([y in x for y in fatal_words])
     is_fatal = contains_yes and contains_fatal and not contains_nonfatal
 
     if is_fatal or x in fatal_words:
         return "FATAL"
     elif x.startswith('NO INJUR') or x.startswith('NONE') or x.startswith('NO COMPLAINT') or\
-        x in ["NOT INJURED",'NEITHER','NO','N', "MISS", 'SHOOT AND MISS','FALSE','NO VISIBLE INJURY','UNINJURED']:
+        x in ["NOT INJURED",'NEITHER','NO','N', "MISS", 'SHOOT AND MISS','FALSE','NO VISIBLE INJURY','UNINJURED', 'SHOW OF FORCE']:
         return "NO INJURY"
     elif contains_yes or x in nonfatal_words or x in ['Y','YES','TRUE'] or \
         any([x.startswith(y) for y in ['COMPLAINED OF','COMPLAINT OF']]) or \
         any([y in x for y in ['WOUND','PAIN', "BLEEDING",'SWELLING','SCRAPE','PUNCTURE','LACERATION','BRUIS',
                               'BROKEN','UNCONSCIOUS', 'FIRST AID', 'SHOT (INJURED ONLY)', 'INJURED   INCIDENTALLY',
                               'DISLOCATED','FRACTURED','ABBRASION','ABRASION','ABRAISON','ABRASSION','BUSTED','PULLED OUT','REDNESS','LOSS','RASH',
                               'SCRATCH','NUMBNESS','BREATHING','CUT','STUN', 'MARKS', 'EYE', 'PEELING', 'HURT', 'ELBOW', 'KNEE',
                               'SOFT TISSUE','BLOOD','HEAD','SORE','SHOULDER', 'MINOR INJUR', 'FINGER', 'IMPACT', 'FACE', 'ARM',
                               'MOUTH', 'BACK','RIB', 'THUMB','SHIN',' EAR', 'ACHILLES', 'STRUCK', 'LEG', 'SERIOUS',
-                              'CONCUSSION','FRACTURE','CANINE BITE', 'MARK','BURN', 'MINOR', 'DISABL', 'PHYSICAL INJURY']]):
+                              'CONCUSSION','FRACTURE','CANINE BITE', 'MARK','BURN', 'MINOR', 'DISABL', 'PHYSICAL INJURY',
+                              'TREATED','TAKEN TO HOSPITAL']]):
         return "INJURED"
     elif 'NALOXONE' in x:
         return orig
     elif x in ['SELF INFLICTED FATAL', 'DECEASED (SELF INFLICTED)','KILLED (SELF INFLICTED)']:
         return 'SELF-INFLICTED FATAL'
     elif x in ['UNKNOWN','UNKNWON']:
         return 'UNKNOWN'
@@ -695,15 +789,15 @@
         x = int(x)
         if x<0:
             return x
         else:
             return "YES" if x>0 else "NO"
     orig = x
     x = x.upper().strip()
-    if x in ["FATAL","YES", "Y"]:
+    if x in ["FATAL","YES", "Y",'DECEASED']:
         return "YES"
     elif x in ["NON-FATAL","NON FATAL", "NO","N",'NO CONTACT']:
         return "NO"
     elif x in ["SELF-INFLICTED"]:
         return "SELF-INFLICTED FATAL"
     elif no_id=='test':
         raise ValueError(f"Unknown value in injury column: {orig}")
```

### Comparing `openpolicedata-0.6/openpolicedata/_preproc_utils.py` & `openpolicedata-0.7/openpolicedata/_preproc_utils.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/openpolicedata/data.py` & `openpolicedata-0.7/openpolicedata/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 from datetime import datetime
 from dateutil.parser._parser import ParserError
 import logging
 from packaging import version
 import re
 from collections.abc import Iterator
+import sys
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 import warnings
 
 from . import data_loaders
@@ -635,14 +636,15 @@
             if verbose:
                 # Set logger to info so log messages in preproc.standardize will be displayed
                 logger.setLevel(logging.INFO)
             try:                    
                 self.table, self.__transforms = preproc.standardize(self.table, self.table_type, self.year,
                     known_cols=known_cols, 
                     source_name=self.source_name,
+                    state=self.state,
                     keep_raw=keep_raw,
                     agg_race_cat=agg_race_cat,
                     race_cats=race_cats,
                     eth_cats=eth_cats,
                     gender_cats=gender_cats,
                     no_id=no_id,
                     race_eth_combo=race_eth_combo,
@@ -712,15 +714,15 @@
         '''
         self.datasets = datasets.query(source_name=source_name, state=state)
 
         # Ensure that all sources are from the same state
         if len(self.datasets) == 0:
             raise ValueError(f"No Sources Found for {source_name}")
         elif self.datasets["State"].nunique() > 1:
-            raise ValueError("Not all sources are from the same state")
+            raise ValueError(f"There are multiple sources matching the source name {source_name}. Please specify the state of the desired location in the 2nd argument.")
 
 
     def __repr__(self) -> str:
         return str(self.datasets)
 
 
     def get_tables_types(self) -> list[str]:
@@ -733,33 +735,36 @@
         '''
         return list(self.datasets["TableType"].unique())
 
 
     def get_years(self, 
         table_type: str | defs.TableType, 
         force: bool = False, 
-        manual: bool = False
+        manual: bool = False,
+        datasets: pd.DataFrame = None
         ) -> list[int]:
         '''Get years available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             Only returns years for requested table type
         force - bool
             (Optional) Some data types such as CSV files require reading the whole file to filter for years. By default, an error will be thrown that indicates running load may be more efficient. For these cases, set force=True to run get_years without error.
         manual - bool
             (Optional) If True, for datasets that contain multiple years, the years will be determined by making requests to the dataset rather than using the years stored in the dataset table. The default is False, which runs faster but may not be up-to-date.
+        datasets - pd.DataFrame
+            (Optional) Only select from datasets in this dataframe instead of self.datasets. datasets should be a subset of the rows in self.datasets.
 
         Returns
         -------
         list
             List of years available for 1 or more datasets
         '''
-        dfs = self.__find_datasets(table_type)
+        dfs = self.__find_datasets(table_type, datasets)
 
         cur_year = datetime.now().year
         all_years = list(dfs["Year"])
         years = {x for x in all_years if isinstance(x,numbers.Number) or x==defs.NA}
         for k in [k for k,x in enumerate(all_years) if x==defs.MULTI]:
             df = dfs.iloc[k]
             try:
@@ -794,45 +799,52 @@
 
         return years
 
 
     def get_agencies(self, 
                      table_type: str | defs.TableType | None = None, 
                      year: str | int | None = None, 
-                     partial_name: str | None = None
+                     partial_name: str | None = None,
+                     url_contains: str | None = None
                      ) -> list[str]:
         '''Get agencies available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             (Optional) If set, only returns agencies for requested table type
         year - int or the strings opd.defs.MULTI or opd.defs.NONE
             (Optional)  If set, only returns agencies for requested year
         table_type - str or TableType enum
             (Optional) If set, only returns agencies for requested table type
         partial_name - str
             (Optional)  If set, only returns agencies containing the substring
             partial_name for datasets that contain multiple agencies
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         list
             List of agencies available for 1 or more datasets
         '''
 
         src = self.__find_datasets(table_type)
 
+        if url_contains:
+            src = src[src['URL'].str.contains(url_contains, regex=False)]
+
         if year != None:
             src = src[src["Year"] == year]
 
         if len(src) == 1:
             src = src.iloc[0]
         else:
-            raise ValueError("table_type and year inputs must filter for a single source")            
+            print(src, file=sys.stderr)
+            raise ValueError("Inputs must filter for a single source")            
 
         # If year is opd.defs.MULTI, need to use self._agencyField to query URL
         # Otherwise return self.agency
         if src["Agency"] == defs.MULTI:
             _check_version(src)
             loader = self.__get_loader(src["DataType"], src["URL"], src['query'], dataset_id=src["dataset_id"], 
                                        date_field=src["date_field"], agency_field=src["agency_field"])
@@ -867,15 +879,16 @@
 
     @input_swap([0,1], ['table_type','year'], [defs.TableType, {'values':[defs.NA, defs.MULTI], 'types':[list, int]}], opt1=None)
     def get_count(self, 
                   table_type: str | defs.TableType | None = None,
                   year: str | int | list[int] | None = None, 
                   agency: str | None = None, 
                   force: bool = False,
-                  verbose: bool | str = False
+                  verbose: bool | str = False,
+                  url_contains: str | None = None
                   ) -> int:
         '''Get number of records for a data request
 
         Parameters
         ----------
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
@@ -887,36 +900,39 @@
         agency - str
             (Optional) If set, for datasets containing multiple agencies, data will
             only be returned for this agency
         force - bool
             (Optional) For file-based data, an exception will be thrown unless force 
             is true. It may be more efficient to load the data and extract the years
             manually
-        verbose : bool | str, optional
+        verbose - bool | str, optional
             If True, details of data loading will be logged. If a filename, details will
             be logged to that file., by default False
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         Table
             Table object containing the requested data
         '''
 
-        return self.__load(table_type, year, agency, True, pbar=False, return_count=True, force=force, verbose=verbose)
+        return self.__load(table_type, year, agency, True, pbar=False, return_count=True, force=force, verbose=verbose, url_contains=url_contains)
     
     @input_swap([0,1], ['table_type','year'], [defs.TableType, {'values':[defs.NA, defs.MULTI], 'types':[list, int]}], error=True, opt1=None)
     def load_iter(self,
                 table_type: str | defs.TableType,
                 year: str | int | list[int],  
                 agency: str | None = None, 
                 pbar: bool = False, 
                 nbatch: int = 10000, 
                 offset: int = 0, 
                 force: bool =False,
-                verbose: bool | str = False
+                verbose: bool | str = False,
+                url_contains: str | None = None
                 ) -> Iterator[Table]:
         '''Get generator to load data from URL in batches
 
         Parameters
         ----------
         table_type - str or TableType enum
             Table type to load
@@ -937,24 +953,27 @@
             to return records starting from the first.
         force - bool
             (Optional) For file-based data, an exception will be thrown unless force 
             is true. It will be more efficient to read the entire dataset all at once
         verbose : bool | str, optional
             If True, details of data loading will be logged. If a filename, details will
             be logged to that file., by default False
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         Table generator
             generates Table objects containing the requested data
         '''
 
-        count = self.get_count(table_type, year, agency, force, verbose=verbose)
+        count = self.get_count(table_type, year, agency, force, verbose=verbose, url_contains=url_contains)
         for k in range(offset, count, nbatch):
-            yield self.__load(table_type, year, agency, True, pbar, nrows=min(nbatch, count-k), offset=k, verbose=verbose)
+            yield self.__load(table_type, year, agency, True, pbar, nrows=min(nbatch, count-k), offset=k, 
+                              verbose=verbose, url_contains=url_contains)
     
     @deprecated("load_from_url_gen is deprecated and will be removed in a future release. Please use load_iter instead. "+
                 "load_iter uses the same inputs except table_type now comes before year.")
     def load_from_url_gen(self, 
                           year: str | int | list[int], 
                           table_type: str | defs.TableType | None = None, 
                           agency: str | None = None, 
@@ -977,15 +996,16 @@
             table_type: str | defs.TableType, 
             year: str | int | list[int], 
             agency: str | None = None,
             pbar: bool = True,
             nrows: int | None = None, 
             offset: int = 0,
             sortby=None,
-            verbose: bool | str = False
+            verbose: bool | str = False,
+            url_contains: str | None = None
             ) -> Table:
         '''Load data from URL
 
         Parameters
         ----------
         table_type - str or TableType enum
             Table type to load
@@ -1003,22 +1023,25 @@
             (Optional) Number of records to read. Default is None for all records.
         offset - int
             (Optional) Number of records to offset from first record. Default is 0 
             to return records starting from the first.
         verbose : bool | str, optional
             If True, details of data loading will be logged. If a filename, details will
             be logged to that file., by default False
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         Table
             Table object containing the requested data
         '''
 
-        return self.__load(table_type, year, agency, True, pbar, nrows=nrows, offset=offset, sortby=sortby, verbose=verbose)
+        return self.__load(table_type, year, agency, True, pbar, nrows=nrows, offset=offset, sortby=sortby, 
+                           verbose=verbose, url_contains=url_contains)
 
     
     @deprecated("load_from_url is deprecated and will be removed in a future release. Please use load instead. "+
                 "load uses the same inputs except table_type now comes before year.")
     def load_from_url(self, 
                       year: str | int | list[int], 
                       table_type: str | defs.TableType | None = None, 
@@ -1030,55 +1053,115 @@
                       verbose: bool | str = False
                       ) -> Table:
         '''load_from_url is deprecated and will be removed in a future release. Please use load instead.
         '''
 
         return self.__load(table_type, year, agency, True, pbar, nrows=nrows, offset=offset, sortby=sortby, verbose=verbose)
 
-    def __find_datasets(self, table_type):
-        src = self.datasets.copy()
+    def __find_datasets(self, table_type, src=None):
+        if src is None:
+            src = self.datasets.copy()
         if table_type != None:
-            src = src[self.datasets["TableType"].str.upper() == str(table_type).upper()]
+            src = src[src["TableType"].str.upper() == str(table_type).upper()]
 
         return src
+    
+    def __filter_for_source(self, table_type, year, url_contains, errors=True):
+        orig_src = self.__find_datasets(table_type)
+        src = orig_src.copy()
 
-
-    def __load(self, table_type, year, agency, load_table, pbar=True, return_count=False, force=False, 
-               nrows=None, offset=0, sortby=None, verbose=False):
+        if isinstance(year, list) and len(year)>2:
+            raise ValueError("year input must either be a single year or a list containing a start and stop year")
         
-        src = self.__find_datasets(table_type)
+        if url_contains:
+            src = src[src['URL'].str.contains(url_contains, regex=False)]
 
-        if isinstance(year, list):
-            matchingYears = src["Year"] == year[0]
-            for y in year[1:]:
-                matchingYears = matchingYears | (src["Year"] == y)
-        else:
-            matchingYears = src["Year"] == year
+        matchingYears = src["Year"]==year if not isinstance(year, list) else pd.Series(False, src.index)
 
-        filter_by_year = not matchingYears.any()
-        if not filter_by_year:
-            # Use source for this specific year if available
+        if (filter_by_year:=not matchingYears.any()):
+            src = src[src["Year"]==defs.MULTI]
+        else:
             src = src[matchingYears]
+
+        if isinstance(year,list):
+            year_filter = []
+            for y in year:
+                if isinstance(y, str) and re.search(r'\d{4}-\d{2}-\d{2}', y):
+                    year_filter.append(int(y[:4]))
+                else:
+                    year_filter.append(y)
         else:
-            # If there are not any years corresponding to this year, check for a table
-            # containing multiple years
-            matchingYears = src["Year"]==defs.MULTI
-            if matchingYears.any():
-                src = src[matchingYears]
-            else:
-                src = src[src["Year"] == defs.MULTI]
+            year_filter = year
 
+        if len(src)>1 and year!=defs.MULTI:
+            # Try to find a single multi-year dataset containing the year
+            contains = pd.Series(False, index=src.index)
+            for k in src.index:
+                ds_years = self.get_years(table_type, datasets=src.loc[[k]])
+                if isinstance(year,list):
+                    if any([x>=year_filter[0] and x<=year_filter[1] for x in ds_years]):
+                        contains[k] = True
+                elif year in ds_years:
+                    contains[k] = True
+            src = src[contains]
+
+        if len(src)>0 and isinstance(year,list) and not url_contains:
+            # Ensure that year range does not also match a single year dataset
+            if (orig_src['Year'].apply(lambda x: x!=defs.MULTI and x>=year_filter[0] and x<=year_filter[1])).any():
+                raise ValueError(f"Year range cannot contain the year corresponding to a single year dataset.\n "
+                                 f"A dataset exists for the year {year}\n "+
+                                 "If the requested year range was correct, the url_contains input can be used to specify a dataset in ambiguous cases "+
+                                 "by setting url_contains to a unique substring of the desired dataset's URL. The URL(s) for the datasets matching "+
+                                 f"the current inputs are {list(src['URL'])}")
+            
         if isinstance(src, pd.core.frame.DataFrame):
             if len(src) == 0:
-                raise ValueError(f"There are no sources matching tableType {table_type} and year {year}")
+                err_msg = f"There are no sources matching {table_type=} and {year=}"
+                if url_contains:
+                    err_msg+=f" and {url_contains=}"
+                raise ValueError(err_msg)
             elif len(src) > 1:
-                raise ValueError(f"There is more than one source matching tableType {table_type} and year {year}")
+                if errors:
+                    err_msg = f"There is more than one source matching {table_type=} and {year=}"
+                    if url_contains:
+                        err_msg+=f" and {url_contains=}"
+                    if isinstance(year, list):
+                        raise ValueError(err_msg+" It is possible that the year range covers more the one dataset." +
+                                        " Set the year input to not contain years for multiple datasets and/or use the url_contains "+
+                                        "input to specify a single dataset "+
+                                        "by setting url_contains to a unique substring of the desired dataset's URL. "
+                                        f"The URL(s) for the datasets matching the current inputs are {list(src['URL'])}")
+                    elif year==defs.MULTI:
+                        raise ValueError(err_msg+f" Therea are multiple multi-year datasets with year={defs.MULTI}." +
+                                        " Use the url_contains "+
+                                        "input to specify a single dataset "+
+                                        "by setting url_contains to a unique substring of the desired dataset's URL. "
+                                        f"The URL(s) for the datasets matching the current inputs are {list(src['URL'])}")
+                    else:
+                        raise ValueError(err_msg+
+                                        " Set the year input to a single year or a year range and/or "+
+                                        "use the url_contains input to specify a single dataset "+
+                                        "by setting url_contains to a unique substring of the desired dataset's URL. "
+                                        f"The URL(s) for the datasets matching the current inputs are {list(src['URL'])}")
+                else:
+                    # This is only for testing
+                    pass
             else:
                 src = src.iloc[0]
 
+        return src, filter_by_year
+
+
+    def __load(self, table_type, year, agency, load_table, pbar=True, return_count=False, force=False, 
+               nrows=None, offset=0, sortby=None, verbose=False, url_contains=None):
+        # Make copy so original isn't changed
+        year = year.copy() if isinstance(year, list) else year
+
+        src, filter_by_year = self.__filter_for_source(table_type, year, url_contains)
+
         # Load data from URL. For year or agency equal to opd.defs.MULTI, filtering can be done
         url = src["URL"]
 
         if filter_by_year:
             year_filter = year
         else:
             year_filter = None
@@ -1168,15 +1251,16 @@
 
 
     def load_from_csv(self, 
                       year: str | int | list[int],
                       output_dir: str | None = None, 
                       table_type: str | defs.TableType | None = None,
                       agency: str | None = None,
-                      zip: bool =False
+                      zip: bool =False,
+                      url_contains: str | None = None
                       ) -> Table:
         '''Load data from previously saved CSV file
         
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
@@ -1188,22 +1272,24 @@
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
         agency - str
             (Optional) If set, for datasets containing multiple agencies, data will
             only be returned for this agency
         zip - bool
             (Optional) Set to true if CSV is in a zip file with the same filename. Default: False
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         Table
             Table object containing the requested data
         '''
 
-        table = self.__load(table_type, year, agency, False)
+        table = self.__load(table_type, year, agency, False, url_contains=url_contains)
 
         filename = table.get_csv_filename()
         if output_dir != None:
             filename = path.join(output_dir, filename)   
 
         if zip:
             filename = filename.replace(".csv",'.zip')  
@@ -1271,15 +1357,16 @@
             return (), ()
 
 
     def get_csv_filename(self, 
                          year: str | int | list[int],
                          output_dir: str | None = None, 
                          table_type: str | defs.TableType | None = None,
-                         agency: str | None = None
+                         agency: str | None = None,
+                         url_contains: str | None = None
                          ) -> str:
         '''Get auto-generated CSV filename
         
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
@@ -1289,50 +1376,61 @@
         output_dir - str
             (Optional) Directory where CSV file is stored
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
         agency - str
             (Optional) If set, for datasets containing multiple agencies, data will
             only be returned for this agency
+        url_contains - str | None
+            (Optional) If set, URL must contain this string. Can be used when multiple datasets match a set of inputs.
 
         Returns
         -------
         str
             Auto-generated CSV filename
         '''
 
-        table = self.__load(table_type, year, agency, False)
+        table = self.__load(table_type, year, agency, False, url_contains=url_contains)
 
         filename = table.get_csv_filename()
         if output_dir != None:
             filename = path.join(output_dir, filename)             
 
         return filename
 
     def __get_loader(self, data_type, url, query, dataset_id=None, date_field=None, agency_field=None):
         if pd.isnull(dataset_id):
             dataset_id = None
         params = (data_type, url, dataset_id, date_field, agency_field)
         if self.__loader is not None and self.__loader[0]==params:
             return self.__loader[1]
-
-        if data_type ==defs.DataType.CSV:
-            loader = data_loaders.Csv(url, date_field=date_field, agency_field=agency_field)
-        elif data_type ==defs.DataType.EXCEL:
-            loader = data_loaders.Excel(url, sheet=dataset_id, date_field=date_field, agency_field=agency_field) 
-        elif data_type ==defs.DataType.ArcGIS:
-            loader = data_loaders.Arcgis(url, date_field=date_field)
-        elif data_type ==defs.DataType.SOCRATA:
-            loader = data_loaders.Socrata(url, dataset_id, date_field=date_field)
-        elif data_type ==defs.DataType.CARTO:
-            loader = data_loaders.Carto(url, dataset_id, date_field=date_field, query=query)
-        elif data_type ==defs.DataType.CKAN:
-            loader = data_loaders.Ckan(url, dataset_id, date_field=date_field, query=query)
+        
+        if dataset_id and ';' in dataset_id:
+            # Multiple dataset IDs
+            if data_type ==defs.DataType.CSV:
+                loader = data_loaders.CombinedDataset(data_loaders.Csv, url, dataset_id, date_field=date_field, agency_field=agency_field)
+            elif data_type ==defs.DataType.EXCEL:
+                loader = data_loaders.CombinedDataset(data_loaders.Excel, url, dataset_id, date_field=date_field, agency_field=agency_field)
+            else:
+                raise ValueError(f"Not supported data type for CombinedDataset: {data_type}")
         else:
-            raise ValueError(f"Unknown data type: {data_type}")
+            if data_type ==defs.DataType.CSV:
+                loader = data_loaders.Csv(url, date_field=date_field, agency_field=agency_field)
+            elif data_type ==defs.DataType.EXCEL:
+                loader = data_loaders.Excel(url, data_set=dataset_id, date_field=date_field, agency_field=agency_field) 
+            elif data_type ==defs.DataType.ArcGIS:
+                loader = data_loaders.Arcgis(url, date_field=date_field)
+            elif data_type ==defs.DataType.SOCRATA:
+                loader = data_loaders.Socrata(url, dataset_id, date_field=date_field)
+            elif data_type ==defs.DataType.CARTO:
+                loader = data_loaders.Carto(url, dataset_id, date_field=date_field, query=query)
+            elif data_type ==defs.DataType.CKAN:
+                loader = data_loaders.Ckan(url, dataset_id, date_field=date_field, query=query)
+            else:
+                raise ValueError(f"Unknown data type: {data_type}")
 
         self.__loader = (params, loader)
 
         return loader
     
     def __fix_date_field(self, table, date_field, loc):
         if date_field != None and table is not None and len(table)>0 and date_field not in table and \
@@ -1344,14 +1442,15 @@
             datasets.datasets.loc[loc, "date_field"] = date_field
 
         return date_field
 
 
 def _check_date(table, date_field):
     logger = logging.getLogger("opd-load")
+    table = table.copy()
     if date_field != None and table is not None and len(table)>0 and date_field in table:
         dts = table[date_field]
         dts = dts[dts.notnull()]
         if len(dts) > 0:
             one_date = dts.iloc[0]  
             if type(one_date) == pd._libs.tslibs.timestamps.Timestamp:
                 if logger:
@@ -1387,34 +1486,46 @@
                 if logger:
                     logger.debug(f"Converting values in column {date_field} to datetime objects")
                 
                 try:
                     # This way is much faster
                     table[date_field] = to_datetime(table[date_field])
                 except ValueError as e:
-                    table[date_field] = table[date_field].apply(to_datetime_local)
+                    if re.search(r'year 20\d{6} is out of range: 20\d{6}.0, at position 0', str(e)):
+                        # Remove decimal value
+                        table[date_field] = to_datetime(table[date_field].apply(lambda x: x[:-2]))
+                    else:
+                        table[date_field] = table[date_field].apply(to_datetime_local)
 
                 if pd.api.types.is_object_dtype(table[date_field]):
                     try:
                         # Attempt to convert
                         table = table.astype({date_field: 'datetime64[ns]'})
+                    except pd._libs.tslibs.parsing.DateParseError as e:
+                        if 'out of range' in str(e):
+                            pass
+                        else:
+                            raise
                     except UnicodeEncodeError:
                         pass
                     except ValueError as e:
                         if len(e.args)>0 and e.args[0].startswith('Cannot mix tz-aware with tz-naive values') and \
                             table[date_field].apply(lambda x: x.hour==0 and x.minute==0).all() and \
-                            len(s:=set([x.tzinfo for x in table[date_field] if x.tzinfo is not None]))==1:
+                            len(set([str(x.tzinfo) for x in table[date_field] if x.tzinfo is not None]))==1:
                             warnings.warn("Some date values have timezone and some do not. Setting timezone unware objects to have the same timezone as the rest.")
-                            tz = s.pop()
+                            tz = [x.tzinfo for x in table[date_field] if x.tzinfo is not None][0]
                             is_not_aware = table[date_field].apply(lambda x: x.tzinfo is None or x.tzinfo.utcoffset(x) is None)
                             table.loc[is_not_aware, date_field] = table.loc[is_not_aware, date_field].apply(lambda x: x.replace(tzinfo=tz))
                             table[date_field] = table[date_field].convert_dtypes()
                         elif 'DateParseError' in str(type(e)) and '-__' in str(e):
                             # Ignore case where month and day are underscores (i.e. 2023-__-__)
                             pass
+                        elif 'ParserError' in str(type(e)) and re.search('Unknown string format: \d+[-/]\d+[-/]\d+,?\s?\d+[-/]\d+[-/]\d+', str(e)):
+                            # Comma separated list of dates cannot be parsed
+                            pass
                         else:
                             raise
                     except TypeError as e:
                         if "Period'> is not convertible to datetime" in str(e):
                             # Mixture of datetimes and periods
                             pass
                         else:
@@ -1429,15 +1540,14 @@
 
                 
             # Replace bad dates with NaT
             if logger:
                 logger.debug(f"Replacing any values of 1900-01-01 00:00:00 in column {date_field} with null")
             table[date_field] = table[date_field].replace(datetime.strptime('1900-01-01 00:00:00', '%Y-%m-%d %H:%M:%S'), pd.NaT)
 
-
     return table
 
 
 def get_csv_filename(
     state: str, 
     source_name: str, 
     agency: str,
```

### Comparing `openpolicedata-0.6/openpolicedata/data_loaders.py` & `openpolicedata-0.7/openpolicedata/data_loaders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from dataclasses import dataclass
 from io import BytesIO
 import json
 import logging
 import numbers
 import os
 import tempfile
-from datetime import date
+from datetime import date, datetime
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from numpy import nan
 import requests
 import urllib
 import urllib3
 from abc import ABC, abstractmethod
 from sodapy import Socrata as SocrataClient
 import warnings
 from time import sleep
 from tqdm import tqdm
+from typing import Optional
 from math import ceil
 import re
 from xlrd.biffh import XLRDError
 from zipfile import ZipFile
 
 try:
     import geopandas as gpd
@@ -28,14 +30,15 @@
     _has_gpd = True
 except:
     _has_gpd = False
 
 try:
     from .datetime_parser import to_datetime
     from .exceptions import OPD_TooManyRequestsError, OPD_DataUnavailableError, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, DateFilterException
+    from .utils import is_str_number
 except:
     from datetime_parser import to_datetime
     from exceptions import OPD_TooManyRequestsError, OPD_DataUnavailableError, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, DateFilterException
 
 logger = logging.getLogger("opd-load")
 
 sleep_time = 0.1
@@ -57,27 +60,28 @@
 # Get a App Token here: http://dev.socrata.com/docs/app-tokens.html
 # Copy the App Token
 # Create an environment variable SODAPY_API_KEY and set it equal to the API key
 # Setting environment variable in Linux: https://phoenixnap.com/kb/linux-set-environment-variable
 # Windows: https://www.wikihow.com/Create-an-Environment-Variable-in-Windows-10
 default_sodapy_key = os.environ.get("SODAPY_API_KEY")
 
-class double_format(object):
+class repeat_format(object):
     def __init__(self, string):
         self.string = string
+        self.repeat = int(string.count('{}')/2)
 
     def __eq__(self, other) -> bool:
-        return isinstance(other, double_format) and self.string == other.string
-        # if isinstance(other, double_format):
-        #     return other.string == self.string
-        # else:
-        #     return False
+        return isinstance(other, repeat_format) and self.string == other.string
 
     def format(self, date_field, year):
-        return self.string.format(date_field, year, date_field, year)
+        args = []
+        for _ in range(self.repeat):
+            args.extend([date_field, year])
+        args = tuple(args)
+        return self.string.format(*args)
     
 # Based on https://stackoverflow.com/a/73519818/9922439
 class CustomHttpAdapter (requests.adapters.HTTPAdapter):
     # "Transport adapter" that allows us to use custom ssl_context.
 
     def __init__(self, ssl_context=None, **kwargs):
         self.ssl_context = ssl_context
@@ -204,14 +208,166 @@
                 if len(check)==0:
                     break
                 while year not in check:
                     year-=1
                 check.remove(year)
 
         return years
+    
+
+class CombinedDataset(Data_Loader):
+    """
+    A class for combining multiple datasets of a single type (Csv, Excel, etc.) into a single data loader
+
+    Parameters
+    ----------
+    data_class: abc.ABCMeta 
+        Data loader class of datasets to be combined
+    loaders: list[Data_Loader]
+        Individual data loader objects
+
+    Methods
+    -------
+    CombinedDataset(data_class, url, datasets, *args, **kwargs)
+        Constructor.
+    load(*args, **kwargs)
+        Load data for query. 
+    get_count(*args, **kwargs)
+        Get number of records/rows generated by query
+    get_years(*args, **kwargs)
+        Get years contained in data set
+    """
+
+    def __init__(self, data_class, url, datasets, *args, **kwargs):
+        """CombinedDataset constructor
+
+        Parameters
+        ----------
+        data_class : abc.ABCMeta 
+            Class of data loader object
+        url : str
+            Base URL of dataset (will be combined with each value in datasets)
+        datasets : str or List[str]
+            Relative dataset URLs (each value will be combined with url). Can be a semi-colon separate string or a list.
+
+        *args and **kwargs will be passed to the constructor of data_class
+        """
+        self.data_class = data_class
+        sheets = None
+        if isinstance(datasets, str):
+            if '|' in datasets:  # dataset names are separated from relative URLs by |
+                datasets = datasets.split('|')
+                assert len(datasets)==2
+                sheets = datasets[0].split(';')   # Different sheet names for each dataset are separated by ;. If multiple sheets for a given dataset, separate by &
+                datasets = datasets[1]
+            datasets = datasets.split(';')         # Multiple relative URLs are separated by ;
+            
+        self.loaders = []
+        url = url[:-1] if url[-1]=='/' else url
+        for k, ds in enumerate(datasets):
+            kwargs = {}
+            if 'raw.githubusercontent.com/openpolicedata/opd-datasets' in ds and ds.endswith('.csv'):
+                self.loaders.append(Csv(ds, *args, **kwargs))
+            else:
+                ds = ds.strip()
+                ds = ds[1:] if ds[0]=='/' else ds
+                ds = url + '/' + ds
+                if sheets:
+                    kwargs['data_set'] = sheets[min(k, len(sheets)-1)]
+                try:
+                    self.loaders.append(data_class(ds, *args, **kwargs))
+                except ValueError as e:
+                    if str(e)=='Excel file format cannot be determined, you must specify an engine manually.':
+                        try:
+                            # This may be a CSV file instead of an Excel file
+                            self.loaders.append(Csv(ds, *args, **kwargs))
+                        except:
+                            raise e
+                        
+                if ds!=datasets[-1]:
+                    sleep(0.5)  # Reduce likelihood of timeout due to repeated requests
+
+
+
+    def isfile(self):
+        '''Returns True to indicate that Csv data is file-based
+
+        Returns
+        -------
+        True
+        '''
+        return True
+    
+    def load(self, **kwargs):
+        """Load data for query. 
+
+        **kwargs will be passed to the load function of the data_class
+        """
+
+        # Handle these here. Less efficient but easier to implement
+        nrows = kwargs.pop('nrows') if 'nrows' in kwargs else None
+        offset = kwargs.pop('offset') if 'offset' in kwargs else None
+
+        dfs = []
+        date_warn = force_subject_warn = force_officer_warn = False
+        for loader in self.loaders:
+            dfs.append(loader.load(**kwargs))
+            if loader!=self.loaders[-1]:
+                sleep(0.5)  # Reduce likelihood of timeout due to repeated requests
+
+            if 'www.albemarle.org' in loader.url:
+                # Renamed
+                if 'Stop Date' in dfs[-1] and 'Date' in dfs[0]: # Column renamed
+                    dfs[-1] = dfs[-1].rename(columns={'Stop Date':'Date'})
+                    if not date_warn:
+                        date_warn = True
+                        warnings.warn("Renaming date column because name of column names changes in some of the monthly data files")
+                if 'Force Used by Subject' in dfs[-1] and 'Physical Force by Subject' in dfs[0]: # Column renamed
+                    dfs[-1] = dfs[-1].rename(columns={'Force Used by Subject':'Physical Force by Subject'})
+                    if not force_subject_warn:
+                        force_subject_warn = True
+                        warnings.warn("Renaming force by subject column because name of column names changes in some of the monthly data files")
+                if 'Force Used by Officer' in dfs[-1] and 'Physical Force by Officer' in dfs[0]: # Column renamed
+                    dfs[-1] = dfs[-1].rename(columns={'Force Used by Officer':'Physical Force by Officer'})
+                    if not force_officer_warn:
+                        force_officer_warn = True
+                        warnings.warn("Renaming force by officer column because name of column names changes in some of the monthly data files")
+
+        df = pd.concat(dfs, ignore_index=True)
+        if offset!=None:
+            df = df.iloc[offset:]
+        if nrows!=None:
+            df = df.head(nrows)
+
+        return df
+        
+    def get_count(self, *args, **kwargs):   
+        """Get number of records/rows generated by query
+
+        *args and **kwargs will be passed to the load function of the data_class
+        """
+
+        count = 0
+        for loader in self.loaders:
+            count+=loader.get_count(*args, **kwargs)
+
+        return count
+    
+    
+    def get_years(self, *args, **kwargs):   
+        """Get years contained in data set
+
+        *args and **kwargs will be passed to the load function of the data_class
+        """
+
+        years = []
+        for loader in self.loaders:
+            years.extend(loader.get_years(*args, **kwargs))
+
+        return years
 
 
 class Csv(Data_Loader):
     """
     A class for accessing data from CSV download URLs
 
     Parameters
@@ -325,14 +481,17 @@
             (Optional) Name of the agency to filter for. None value returns data for all agencies.
             
         Returns
         -------
         pandas DataFrame
             DataFrame containing table imported from CSV
         '''
+
+        if isinstance(nrows, float):
+            nrows = int(nrows)
         
         logger.debug(f"Loading file from {self.url}")
         if ".zip" in self.url:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=pd.errors.DtypeWarning)
                 try:
                     table = read_zipped_csv(self.url, pbar=pbar)
@@ -347,73 +506,96 @@
                             raise
                     else:
                         raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
                 except Exception as e:
                     raise e
         else:
             use_legacy = False
+            headers = None
             try:
                 r = requests.head(self.url)
             except requests.exceptions.SSLError as e:
                 if "[SSL: UNSAFE_LEGACY_RENEGOTIATION_DISABLED] unsafe legacy renegotiation disabled" in str(e.args[0]) or \
                     "[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate" in str(e.args[0]):
                     use_legacy = True
                 else:
                     raise e
+            except requests.exceptions.ConnectionError as e:
+                if 'Max retries exceeded' in str(e):
+                    raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
+                else:
+                    raise e
             except Exception as e:
                 raise
                 
             if not use_legacy:
                 if r.status_code in [400,404]:
                     # Try get instead
                     r = requests.get(self.url)
                 try:
                     r.raise_for_status()
                     r.close()
                 except requests.exceptions.HTTPError as e:
-                    raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
+                    try:
+                        headers = {
+                            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:106.0) Gecko/20100101 Firefox/106.0',
+                            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
+                            'Accept-Language': 'en-US,en;q=0.5',
+                            # 'Accept-Encoding': 'gzip, deflate, br',
+                            'DNT': '1',
+                            'Connection': 'keep-alive',
+                            'Upgrade-Insecure-Requests': '1',
+                            'Sec-Fetch-Dest': 'document',
+                            'Sec-Fetch-Mode': 'navigate',
+                            'Sec-Fetch-Site': 'none',
+                            'Sec-Fetch-User': '?1',
+                        }
+                        r = requests.get(self.url, headers=headers)
+                        r.raise_for_status()
+                        r.close()
+                    except:
+                        raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
                 except Exception as e:
                     raise e
             
-            def get(url, use_legacy):
+            def get(url, use_legacy, headers=None):
                 if use_legacy:
-                    return get_legacy_session().get(url, params=None, stream=True)
+                    return get_legacy_session().get(url, params=None, stream=True, headers=headers)
                 else:
-                    return requests.get(url, params=None, stream=True)
+                    return requests.get(url, params=None, stream=True, headers=headers)
 
-            is_mass_employee = self.url=="https://www.mass.gov/doc/consolidated-list-of-officer-status-csv-file-as-of-october-5-2023/download" 
-            header = None if is_mass_employee else 'infer'   
+            header = 'infer'   
 
-            with get(self.url, use_legacy) as resp:
+            with get(self.url, use_legacy, headers) as resp:
                 try:
                     with warnings.catch_warnings():
                         warnings.filterwarnings("ignore", message=r"Columns \(.+\) have mixed types", category=pd.errors.DtypeWarning)
                         table = pd.read_csv(TqdmReader(resp, pbar=pbar), nrows=offset+nrows if nrows is not None else None, 
                             encoding_errors='surrogateescape', 
                             header=header)
                 except (urllib.error.HTTPError, pd.errors.ParserError) as e:
                     raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
                 except Exception as e:
                     raise e
-
-            if is_mass_employee:
-                table.columns = ['Officer','Agency','Expiration Date', 'Reason','ID','Certification #','Status']
-                logger.debug(f"This file does not contain headers. The following headers will be used {table.columns}")
+                
+        if len(table.columns)==1 and '?xml' in table.columns[0] and len(table)==1 and 'Error' in table.iloc[0,0]:
+            # Read data was not a CSV file. It was an error code where the line breaks were interpreted as single column data by load_csv
+            raise OPD_DataUnavailableError(table.iloc[0,0], _url_error_msg.format(self.url))
+        
+        table = filter_dataframe(table, date_field=self.date_field, year_filter=year, 
+            agency_field=self.agency_field, agency=agency)
 
         if offset>0:
             rows_limit = offset+nrows if nrows is not None and offset+nrows<len(table) else len(table)
             logger.debug(f"Extracting {rows_limit} rows starting at {offset}")
             table = table.iloc[offset:rows_limit].reset_index(drop=True)
         if nrows is not None and len(table)>nrows:
             logger.debug(f"Extracting the first {nrows} rows")
             table = table.head(nrows)
 
-        table = filter_dataframe(table, date_field=self.date_field, year_filter=year, 
-            agency_field=self.agency_field, agency=agency)
-
         return table
 
     def get_years(self, *, force=False, **kwargs):
         '''Get years contained in data set
         
         Parameters
         ----------
@@ -464,33 +646,33 @@
         Load data for query
     get_count(year=None, agency=None, force=False)
         Get number of records/rows generated by query
     get_years(force=False)
         Get years contained in data set
     """
 
-    def __init__(self, url, date_field=None, agency_field=None, sheet=None):
+    def __init__(self, url, data_set=None, date_field=None, agency_field=None):
         '''Create Excel object
 
         Parameters
         ----------
         url : str
             URL for Excel data
         date_field : str
             (Optional) Name of the column that contains the date
         agency_field : str
             (Optional) Name of the column that contains the agency name (i.e. name of the police departments)
-        sheet : str
+        data_set : str
             (Optional) Excel sheet to use. If not provided, an error will be thrown when loading data if there is more than 1 sheet
         '''
         
         self.url = url
         self.date_field = date_field
         self.agency_field = agency_field
-        self.sheet = sheet
+        self.sheet = data_set
 
         if self.sheet is not None and re.match(r'^[“”"].+[“”"]$', self.sheet):
             # Sheet name was put in quotes due to it being a number to prevent Excel from dropping any zeros from the front
             self.sheet = self.sheet[1:-1]
         
         try:
             if ".zip" in self.url:
@@ -506,16 +688,35 @@
             else:
                 self.excel_file = pd.ExcelFile(url)
         except urllib.error.HTTPError as e:
             if str(e) in ["HTTP Error 406: Not Acceptable", 'HTTP Error 403: Forbidden']:
                 # 406 error: https://stackoverflow.com/questions/34832970/http-error-406-not-acceptable-python-urllib2
                 # File-like input for URL: https://stackoverflow.com/questions/57815780/how-can-i-directly-handle-excel-file-link-python/57815864#57815864
                 headers = {'User-agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'}
-                r = requests.get(url, stream=True, headers=headers)
-                r.raise_for_status()
+                headers2 = {
+                    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:106.0) Gecko/20100101 Firefox/106.0',
+                    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
+                    'Accept-Language': 'en-US,en;q=0.5',
+                    # 'Accept-Encoding': 'gzip, deflate, br',
+                    'DNT': '1',
+                    'Connection': 'keep-alive',
+                    'Upgrade-Insecure-Requests': '1',
+                    'Sec-Fetch-Dest': 'document',
+                    'Sec-Fetch-Mode': 'navigate',
+                    'Sec-Fetch-Site': 'none',
+                    'Sec-Fetch-User': '?1',
+                }
+                for k, h in enumerate([headers, headers2]):
+                    r = requests.get(url, stream=True, headers=h)
+                    try:
+                        r.raise_for_status()
+                        break
+                    except:
+                        if k==1:
+                            raise
                 file_like = BytesIO(r.content)
                 self.excel_file = pd.ExcelFile(file_like)
             else:
                 raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
         except urllib.error.URLError as e:
             if "[SSL: UNSAFE_LEGACY_RENEGOTIATION_DISABLED] unsafe legacy renegotiation disabled" in str(e.args[0]):
                 with get_legacy_session() as session:
@@ -685,24 +886,24 @@
                 if year==None:
                     year = list(sheets.keys())
                     year.sort()
                     year = [year[0], year[-1]]
                 if not isinstance(year, list):
                     year = [year, year]
 
-                table = None
+                table = pd.DataFrame()
                 cols_added = 0
                 for y in range(year[0], year[1]+1):
                     if y in sheets:
                         logger.debug(f"Loading data from sheet {sheets[y]}")
                         df = pd.read_excel(self.excel_file, nrows=nrows_read, sheet_name=sheets[y])
 
                         df = self.__clean(df)
 
-                        if isinstance(table, type(None)):
+                        if len(table)==0:
                             table = df
                             col_matches = [[k] for k in range(len(df.columns))]
                         else:
                             if not df.columns.equals(table.columns):
                                 # Conditional for preventing column names from being too different
                                 if len(df.columns)+cols_added == len(table.columns) and \
                                     (df.columns == table.columns[:len(df.columns)]).sum()>=len(df.columns)-3-cols_added:
@@ -714,50 +915,52 @@
                                             try:
                                                 from rapidfuzz import fuzz
                                             except:
                                                 raise ImportError(f"{self.url} requires installation of rapidfuzz " + 
                                                     "(https://pypi.org/project/rapidfuzz/) to load data from multiple years (pip install rapidfuzz)")
 
                                             if fuzz.ratio(table.columns[k], df.columns[m]) > 80:
-                                                print(f"Identified difference in column names when combining sheets {sheets[y-1]} and {sheets[y]}. " + 
+                                                warnings.warn(f"Identified difference in column names when combining sheets {sheets[y-1]} and {sheets[y]}. " + 
                                                     f"Column names are '{table.columns[k]}' and '{df.columns[m]}'. This appears to be a typo. " + 
                                                     f"These columns are assumed to be the same and will be combined as column '{table.columns[k]}'")
                                                 df.columns = [table.columns[k] if j==m else df.columns[j] for j in range(len(df.columns))]
                                                 break
                                         else:
-                                            print(f"Column '{table.columns[m]}' in current DataFrame does not match '{df.columns[m]}' in new DataFrame. "+ 
+                                            warnings.warn(f"Column '{table.columns[m]}' in current DataFrame does not match '{df.columns[m]}' in new DataFrame. "+ 
                                                 "When they are concatenated, both columns will be included.")
                                             col_matches[m].append(len(table.columns))
                                             cols_added+=1
                                             # raise ValueError(f"Column {table.columns[k]} in table does not match {df.columns[k]} in df")
                                 else:
                                     raise ValueError("Columns don't match")
                             logger.debug("Concatenating data from multiple year sheets")
                             table = pd.concat([table, df], ignore_index=True)
 
                         if nrows_read!=None and len(table)>=nrows_read:
                             break
-
-                if isinstance(table, type(None)):
-                    return table
             else:
-                self.__check_sheet(sheets)
-                sheet_name = 0 if self.sheet is None else self.sheet
-                logger.debug(f"Loading sheet: {sheet_name}")
-                table = pd.read_excel(self.excel_file, nrows=nrows_read, sheet_name=sheet_name)
+                sheets_load = self.sheet.split("&") if isinstance(self.sheet,str) else [self.sheet]
+                dfs = []
+                for s in sheets_load:
+                    if isinstance(s,str):
+                        s = s.strip()
+                        if '*' in s:
+                            p = s.replace('*','.*')
+                            s = [x for x in sheets if re.search(p,x)]
+                            assert len(s)==1
+                            s = s[0]
+                    
+                    self.__check_sheet(s, sheets)
+                    sheet_name = 0 if s is None else s
+                    logger.debug(f"Loading sheet: {sheet_name}")
+                    table = pd.read_excel(self.excel_file, nrows=nrows_read, sheet_name=sheet_name)
+                    dfs.append(table)
+                table = pd.concat(dfs, ignore_index=True)
                 table = self.__clean(table)               
 
-        if offset>0:
-            rows_limit = nrows_read if nrows_read is not None and nrows_read<len(table) else len(table)
-            logger.debug(f"Extracting {rows_limit} rows starting at {offset}")
-            table = table.iloc[offset:rows_limit].reset_index(drop=True)
-        if nrows is not None and len(table)>nrows:
-            logger.debug(f"Extracting the first {nrows} rows")
-            table = table.head(nrows)
-
         # Check for empty rows at the bottom
         num_empty = table.isnull().sum(axis=1)
         empty_rows = num_empty==len(table.columns)
         if empty_rows.any():
             # Check if all rows after first empty row are empty or almost empty
             empty_rows = empty_rows[empty_rows]
             num_empty = num_empty.loc[empty_rows.index[0]:]
@@ -766,45 +969,72 @@
                 table = table.head(empty_rows.index[0])
 
         # Clean up column names
         table.columns = [x.strip() if isinstance(x, str) else x for x in table.columns]
 
         table = filter_dataframe(table, date_field=self.date_field, year_filter=year, 
             agency_field=self.agency_field, agency=agency)
+        
+        if offset>0:
+            rows_limit = nrows_read if nrows_read is not None and nrows_read<len(table) else len(table)
+            logger.debug(f"Extracting {rows_limit} rows starting at {offset}")
+            table = table.iloc[offset:rows_limit].reset_index(drop=True)
+        if nrows is not None and len(table)>nrows:
+            logger.debug(f"Extracting the first {nrows} rows")
+            table = table.head(nrows)
 
         return table
 
 
-    def __check_sheet(self, sheets):
-        if self.sheet is None:
+    def __check_sheet(self, cur_sheet, sheets):
+        if cur_sheet is None:
             if not all([re.match(r"Sheet\d+",x) for x in sheets[1:]]):
                 # More than 1 sheet has non-default name so can't assume 1st sheet
                 raise ValueError(f"The Excel file at {self.url} has {len(sheets)} sheets but no dataset id is specified to indicate which to use.")
-        elif self.sheet not in sheets:
-            raise ValueError(f"Sheet {self.sheet} not found in Excel file at {self.url}")
+        elif cur_sheet not in sheets:
+            raise ValueError(f"Sheet {cur_sheet} not found in Excel file at {self.url}")
 
 
     def __clean(self, df):
         # Row names may not be the 1st row in which case columns need to be fixed
         max_drops = 5
         num_drops = 0
         while sum([(pd.isnull(x) or "Unnamed" in x) for x in df.columns]) / len(df.columns) > 0.5:
-            new_cols = [x for x in df.iloc[0]]
-            if all([isinstance(x, str) or pd.isnull(x) for x in new_cols]):
-                logger.debug(f"Detect that first row does not contain column headers: {df.columns}")
-                logger.debug(f"Making the  second row the column headers: {new_cols}")
-                df.columns = new_cols
-                df.drop(index=df.index[0], inplace=True)
-                df.reset_index(drop=True, inplace=True)
-                num_drops+=1
-
-                if len(df)==0 or num_drops>=max_drops:
-                    raise ValueError("Unable to find column names")
-
-        df = df.convert_dtypes()
+            if ((m:=df.isnull().mean())==1).any():
+                keep = []
+                found1 = False
+                num1 = 0
+                max1 = 3
+                for k,v in m.items():
+                    if found1 and v!=1:
+                        raise ValueError(f"Unable to parse Excel table from {self.url}")
+                    elif v==1:
+                        found1 = True
+                        num1+=1
+                        if num1>=max1:
+                            break
+                    else:
+                        keep.append(k)
+                df = df[keep]
+            else:
+                new_cols = [x for x in df.iloc[0]]
+                if all([isinstance(x, str) or pd.isnull(x) for x in new_cols]):
+                    logger.debug(f"Detect that first row does not contain column headers: {df.columns}")
+                    logger.debug(f"Making the  second row the column headers: {new_cols}")
+                    df.columns = new_cols
+                    df.drop(index=df.index[0], inplace=True)
+                    df.reset_index(drop=True, inplace=True)
+                    num_drops+=1
+
+                    if len(df)==0 or num_drops>=max_drops:
+                        raise ValueError("Unable to find column names")
+
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=RuntimeWarning)
+            df = df.convert_dtypes()
 
         # Check for 1st column being row numbers
         if pd.isnull(df.columns[0]) and list(df.iloc[:,0]) in [[k+1 for k in range(0, len(df))], [k for k in range(0, len(df))]]:
             logger.debug("Removing the 1st column which is just the row number")
             df = df.iloc[:, 1:]
 
         return df
@@ -882,14 +1112,15 @@
         ----------
         url : str
             URL for ArcGIS data
         date_field : str
             (Optional) Name of the column that contains the date
         '''
 
+        self._date_type = None
         self._date_format = None
         self.date_field = date_field
         self.verify = False
 
         # Table vs. Layer: https://developers.arcgis.com/rest/services-reference/enterprise/layer-feature-service-.htm
         # The layer resource represents a single feature layer or a nonspatial table in a feature service. 
         # A feature layer is a table or view with at least one spatial column.
@@ -898,14 +1129,17 @@
 
         p = re.search(r"(MapServer|FeatureServer)/\d+", url)
         self.url = url[:p.span()[1]]
 
         # Get metadata
         meta = self.__request()
 
+        if 'type' not in meta and meta['status']=='error':
+            raise OPD_DataUnavailableError(self.url, meta['messages'])
+
         if "maxRecordCount" in meta:
             self.max_record_count = meta["maxRecordCount"] if meta['maxRecordCount']<self.__max_maxRecordCount else self.__max_maxRecordCount
         else:
             self.max_record_count = None
 
         if meta["type"]=="Feature Layer":
             self.is_table = False
@@ -999,14 +1233,22 @@
         
         if self._last_count is not None and self._last_count[0]==(year,where):
             logger.debug("Request matches previous count request. Returning saved count.")
             record_count = self._last_count[1]
             where_query = self._last_count[2]
         elif where==None:
             where_query, record_count = self.__construct_where(year)
+
+            if not self.__accurate_count:
+                raise ValueError(f"Count is not accurate for year input {self.__accurate_count}. "
+                                 "Date field contains data in text format not date format "
+                                 "and the text not formatted in a way that makes getting a count "
+                                 "possible without loading in the data. Either adjust the input to "
+                                 "get_count to get a range of years instead of a range of dates or "
+                                 "load in the data for the current date range")
         else:
             where_query = where
             try:
                 record_count = self.__request(where=where, return_count=True)["count"]
                 if self.verify:
                     record_count_orig = self.__active_layer.query(where=where, return_count_only=True)
                     if record_count_orig!=record_count:
@@ -1083,21 +1325,22 @@
                     v = v[0] if isinstance(v,list) and len(v)==1 else v
                     args += (k,v)
             raise OPD_DataUnavailableError(url, 'Error returned by ArcGIS query', *args)
         
         return result
 
 
-    def __construct_where(self, year=None):
+    def __construct_where(self, year=None, date_range_error=True):
         where_query = ""
+        self.__accurate_count = True
         if self._last_count is not None and self._last_count[0]==(year,None):
             record_count = self._last_count[1]
             where_query = self._last_count[2]
         elif self.date_field!=None and year!=None:
-            where_query, record_count = self._build_date_query(year)
+            where_query, record_count = self._build_date_query(year, date_range_error)
         else:
             where_query = '1=1'
             try:
                 record_count = self.__request(where=where_query, return_count=True)["count"]
                 if self.verify:
                     record_count_orig = self.__active_layer.query(where=where_query, return_count_only=True)
                     if record_count_orig!=record_count:
@@ -1106,20 +1349,170 @@
                 if len(e.args)>0 and "Error Code: 429" in e.args[0]:
                     raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
                 else:
                     raise
             except:
                 raise
 
-        self._last_count = ((year,None), record_count, where_query)
+        if self.__accurate_count:
+            # Count may not be accurate if date ranges are allowed and the date field was a string
+            self._last_count = ((year,None), record_count, where_query)
 
         return where_query, record_count
+    
+    def _build_date_query(self, year, date_range_error):
+        # Determine format by getting some data
+        data = None
+        if not self._date_type:
+            data = self.__request(where='1=1', out_fields=self.date_field, count=1000)
+            self._date_type = data['fields'][0]['type']
+
+        if self._date_type=='esriFieldTypeDate':
+            where_query, record_count = self._build_date_query_date_type(year)
+        elif self._date_type=='esriFieldTypeString':
+            where_query, record_count = self._build_date_query_string_type(year, data, date_range_error)
+        elif self._date_type=='esriFieldTypeInteger' and (self.date_field.lower()=='yr' or 'year' in self.date_field.lower()):
+            where_query, record_count = self._build_date_query_date_type(year, is_numeric_year=True)
+        else:
+            raise NotImplementedError(f"Unknown field {self._date_type}")
+        
+        return where_query, record_count
+
+    def _build_date_query_string_type(self, year, data, date_range_error):
+        if data != None:
+            dates = [x['attributes'][self.date_field] for x in data['features']]
+
+            # [regex for pattern, Arcgis Pattern OR date delimiter (punctuation between numbers), whether to use inquality to do comparison,
+                # OPTIONAL time delimiter]
+            @dataclass
+            class DateParseParams:
+                regex_pattern: re.Pattern
+                arcgis_pattern: Optional[str] = None
+                ineq_comp: bool = False
+                date_delim: str = ""
+                full_date: bool = True
+
+            matches = [
+                DateParseParams(re.compile(r"^(19|20)\d{6}\b"), ineq_comp=True),  # YYYYMMDD
+                DateParseParams(re.compile(r"^(19|20)\d{12}\b"), ineq_comp=True),  # YYYYMMDDHHMMSS
+                DateParseParams(re.compile(r"^(19|20)\d{2}-\d{2}-\d{2}(\b|T)"), ineq_comp=True, date_delim="-"),  # YYYY-MM-DDThh:mm:ss
+                DateParseParams(re.compile(r"^[A-Z][a-z]+ \d{1,2}, (19|20)\d{2}\b"), "{} LIKE '[A-Z]% [0-9][0-9], {}' OR {} LIKE '[A-Z]% [0-9], {}'"),  # Month DD, YYYY
+                DateParseParams(re.compile(r"^\d{1,2}[-/]\d{1,2}[-/](19|20)\d{2}\b"), 
+                    "{} LIKE '%[0-9][0-9][/-][0-9][0-9][/-]{}%' OR {} LIKE '%[0-9][/-][0-9][0-9][/-]{}%' OR " + 
+                    "{} LIKE '%[0-9][/-][0-9][/-]{}%' OR {} LIKE '%[0-9][0-9][/-][0-9][/-]{}%'"),  # mm/dd/yyyy or mm-dd-yyyy
+                DateParseParams(re.compile(r"^\d{4}[-/]\d{1,2}$"), "{} LIKE '{}[-/][0-9][0-9]' OR {} LIKE '{}[-/][0-9]'", full_date=False),  # YYYY-MM or YYYY/M
+                DateParseParams(re.compile(r"^\d{4}$"), "{} = '{}'", full_date=False),  # YYYY
+            ]
+
+            hi = 0.0
+            idx = None
+            for k, m in enumerate(matches):
+                if (new:=sum([isinstance(x,str) and m.regex_pattern.search(x) != None for x in dates])/len(dates)) > hi:
+                    hi = new
+                    idx = k
+
+            if hi < 0.9:
+                raise ValueError("Unable to find date string pattern")
+            
+            self._ineq_comp = matches[idx].ineq_comp
+            if self._ineq_comp:
+                self._date_delim = matches[idx].date_delim
+            else:
+                self._date_format = repeat_format(matches[idx].arcgis_pattern)
+                self._full_date = matches[idx].full_date
+
+        if self._ineq_comp:
+            where_query, record_count = self._build_date_query_date_type(year, self._date_delim, is_date_string=True)
+        else:
+            year = [year] if isinstance(year, numbers.Number) else year.copy()
+            for k,y in enumerate(year):
+                if isinstance(y,str) and re.search(r'^\d{4}-\d{2}-\d{2}', y):
+                    year[k] = y[:4]
+                    self.__accurate_count = False
+                    
+            if (not self._full_date or date_range_error) and any([isinstance(x,str) and len(x)!=4 for x in year]):
+                # Currently can only handle years
+                raise ValueError(f"Date column is a string data type at the source {self.url}. "+
+                                "Currently only able to filter for a single year (2023) or a year range ([2022,2023]) "+
+                                "not a date range ([2022-01-01, 2022-03-01]).")
+            
+            where_query = self._date_format.format(self.date_field, year[0])
+            if len(year)>1:
+                for x in range(int(year[0])+1,int(year[1])+1):
+                    where_query = f"{where_query} or " + self._date_format.format(self.date_field, x)
+
+            record_count = self.__request(where=where_query, return_count=True)["count"]
+
+        return where_query, record_count
+        
+        
+
+    def _build_date_query_date_type(self, year, date_delim='-', is_numeric_year=False, is_date_string=False):
+        # List of error messages that can occur for bad queries as we search for the right query format
+        query_err_msg = ["Unable to complete operation", "Failed to execute query", "Unable to perform query", "Database error has occurred", 
+                         "'where' parameter is invalid", "Parsing error",'Query with count request failed']
+        
+        where_query = ""
+        zero_found = False
+        if self._date_format in [0,1] or self._date_format==None:
+            start_date, stop_date = _process_date(year, force_year=is_numeric_year, is_date_string=is_date_string)
+
+            if date_delim=='':
+                start_date = start_date.replace('-','')
+                stop_date = stop_date.replace('-','')
+            elif date_delim!='-':
+                raise NotImplementedError("Unable to handle this delimiter")
+            
+            for k in range(0,2):
+                if self._date_format is not None and self._date_format!=k:
+                    continue
+                if k==0:
+                    if is_numeric_year:
+                        where_query = f"{self.date_field} >= {start_date} AND  {self.date_field} <= {stop_date}"
+                    else:
+                        where_query = f"{self.date_field} >= '{start_date}' AND  {self.date_field} <= '{stop_date}'"
+                elif is_numeric_year:
+                    break
+                else:
+                    # break
+                    # Dataset (San Jose crash data) that required this does not function well so removing its functionality for now to speed up this function.
+                    # This is the recommended way but it has been found to not work sometimes. One dataset was found that requires this.
+                    # https://gis.stackexchange.com/questions/451107/arcgis-rest-api-unable-to-complete-operation-on-esrifieldtypedate-in-query
+                    stop_date_tmp = stop_date.replace("T"," ")
+                    where_query = f"{self.date_field} >= TIMESTAMP '{start_date}' AND  {self.date_field} < TIMESTAMP '{stop_date_tmp}'"
+            
+                try:
+                    record_count = self.__request(where=where_query, return_count=True)["count"]
+
+                    if self.verify:
+                        record_count_orig = self.__active_layer.query(where=where_query, return_count_only=True)
+                        if record_count_orig!=record_count:
+                            raise ValueError(f"Record count of {record_count} does not equal count from arcgis package of {record_count_orig}")
+                    if self._date_format!=None or record_count>0:
+                        self._date_format = k
+                        return where_query, record_count
+                    else:
+                        zero_found = True
+                except Exception as e:
+                    if len(e.args)>0 and "Error Code: 429" in e.args[0]:
+                        raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
+                    elif len(e.args)>0 and (any([x in e.args[0] for x in query_err_msg]) or any([x in e.args[-1] for x in query_err_msg])):
+                        # This query throws an error for this dataset. Try another one below
+                        pass
+                    else:
+                        raise
+                except:
+                    raise
+
+        if not zero_found:
+            raise AttributeError(f"Unable to find date format for {self.url}")
 
+        return "", 0
     
-    def _build_date_query(self, year):
+    def _build_date_query_old(self, year):
 
         # List of error messages that can occur for bad queries as we search for the right query format
         query_err_msg = ["Unable to complete operation", "Failed to execute query", "Unable to perform query", "Database error has occurred", 
                          "'where' parameter is invalid", "Parsing error",'Query with count request failed']
         
         where_query = ""
         zero_found = False
@@ -1160,21 +1553,25 @@
                     else:
                         raise
                 except:
                     raise
 
 
         where_formats = [
-            "{} LIKE '%[0-9][0-9]/[0-9][0-9]/{}%'",   # mm/dd/yyyy
-            double_format("{} LIKE '{}/[0-9][0-9]' OR {} LIKE '{}/[0-9]'"),                # yyyy/mm
+            "{} LIKE '%[0-9][0-9][/-][0-9][0-9][/-]{}%' OR {} LIKE '%[0-9][/-][0-9][0-9][/-]{}%' OR " + 
+                "{} LIKE '%[0-9][/-][0-9][/-]{}%' OR {} LIKE '%[0-9][0-9][/-][0-9][/-]{}%'",   # mm/dd/yyyy or mm-dd-yyyy
+            "{} LIKE '{}/[0-9][0-9]' OR {} LIKE '{}/[0-9]'",                # yyyy/mm
             "{} = {}",                # yyyy
-            double_format("{} LIKE '[0-9][0-9]-{}' OR {} LIKE '[0-9]-{}'"),   # mm-yyyy or m-yyyy
+            "{} LIKE '[0-9][0-9]-{}' OR {} LIKE '[0-9]-{}'",   # mm-yyyy or m-yyyy
             "{} = '{}'",                # 'yyyy'
-            "{} LIKE '%[0-9][0-9]-[0-9][0-9]-{}%'",   # mm-dd-yyyy
+            "{}>='{}0101' AND {}<='{}1231'",            # yyyymmdd as float
+            "{} LIKE '[A-Z]% [0-9][0-9], {}'"   # {Month Name} dd, yyyy
         ]
+        where_formats = [repeat_format(x) for x in where_formats]
+
         # Make year iterable
         year = [year] if isinstance(year, numbers.Number) else year
 
         if self._date_format not in [None, 0, 1] and any([isinstance(x,str) and len(x)!=4 for x in year]):
             # Currently can only handle years
             raise ValueError("Currently unable to handle non-year inputs")
 
@@ -1229,15 +1626,15 @@
             
         Returns
         -------
         pandas or geopandas DataFrame
             DataFrame containing table imported from ArcGIS
         '''
         
-        where_query, record_count = self.__construct_where(year)
+        where_query, record_count = self.__construct_where(year, date_range_error=False)
         
         # Update record count for request record offset
         record_count-=offset
         if record_count<=0:
             return pd.DataFrame()
 
         batch_size = self.max_record_count or _default_limit
@@ -1315,14 +1712,29 @@
 
         df = pd.DataFrame.from_records([x["attributes"] for x in features])
         for col in date_cols:
             if col in df:
                 logger.debug(f"Column {col} had a data type of esriFieldTypeDate. Converting values to datetime objects.")
                 df[col] = to_datetime(df[col], unit="ms", errors='coerce')
 
+        if not self.__accurate_count:
+            logger.debug(f"User requested filtering by a date range but this was NOT done in the Arcgis query "+
+                         f"due to the date field not being in a date format. Converting {self.date_field} column to "
+                         f"a datetime in order to filter for requested date range {year}")
+            df[self.date_field] = to_datetime(df[self.date_field], errors='coerce')
+            date_range = [str(x) for x in year]
+            if len(date_range[0])==4:
+                date_range[0] = date_range[0]+'-01-01'
+            if len(date_range[1])==4:
+                date_range[1] = date_range[1] + "-12-31T23:59:59.999"
+            else:
+                date_range[1] = date_range[1] + "T23:59:59.999"
+
+            df = df[ (df[self.date_field] >= date_range[0]) & (df[self.date_field] <= date_range[1]) ]
+
         if len(df) > 0:
             has_point_geometry = any("geometry" in x and "x" in x["geometry"] for x in features)
             if not self.is_table and has_point_geometry:
                 if _use_gpd_force is not None:
                     if not _has_gpd and _use_gpd_force:
                         raise ValueError("User cannot force GeoPandas usage when it is not installed")
                     use_gpd = _use_gpd_force
@@ -1427,14 +1839,17 @@
         '''Returns False to indicate that Carto data is not file-based
 
         Returns
         -------
         False
         '''
         return False
+    
+    def get_api_url(self):
+        return f'{self.url}?q=SELECT * FROM {self.data_set}'
 
 
     def get_count(self, year=None, **kwargs):
         '''Get number of records for a data request
         
         Parameters
         ----------
@@ -1505,15 +1920,15 @@
         r = requests.get(self.url, params=params)
 
         try:
             r.raise_for_status()
         except requests.HTTPError as e:
             if len(e.args)>0:
                 if "503 Server Error" in e.args[0]:
-                    raise OPD_DataUnavailableError(self.url, e.args)
+                    raise OPD_DataUnavailableError(self.get_api_url(), e.args, _url_error_msg.format(self.get_api_url()))
                 else:
                     raise
 
             else: raise e
         except: raise
         
         return r.json()
@@ -1585,15 +2000,15 @@
                 if batch==0 and len(features)>0:
                     date_cols = [key for key, x in type_info["fields"].items() if x["type"]=='date']
                     if len(data["features"]) not in [batch_size, nrows]:
                         num_rows = len(data["features"])
                         raise ValueError(f"Number of rows is {num_rows} but is expected to be max rows to read {batch_size} or total number of rows {nrows}")
             except Exception as e:
                 if len(e.args)>0 and "Error Code: 429" in e.args[0]:
-                    raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
+                    raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.get_api_url()))
                 else:
                     raise
             except:
                 raise
 
             if pbar:
                 bar.update(len(data["features"]))
@@ -1711,15 +2126,24 @@
             if not assume_date and len(column)==0:
                 raise ValueError(f"Date field {self.date_field} not found in dataset")
             if filter_year:
                 start_date, stop_date = _process_date(year, date_field=self.date_field, force_year=True)
                 where = ''
                 for y in range(int(start_date),int(stop_date)+1):
                     # %25 is % wildcard symbol
-                    where+=self.date_field + rf" LIKE '%{y}%' OR "
+                    if self.url=='data.bloomington.in.gov' and self.data_set=='gpr2-wqbb':
+                        # This dataset has a text date field and contains YYYY/MM/DD and MM/DD/YY formats
+                        yy = str(y)[2:]
+                        where+=self.date_field + f" LIKE '_/_/{yy}' OR " + \
+                               self.date_field + f" LIKE '_/__/{yy}' OR " + \
+                               self.date_field + f" LIKE '__/_/{yy}' OR " + \
+                               self.date_field + f" LIKE '__/__/{yy}' OR " + \
+                               self.date_field + rf" LIKE '{y}%' OR "
+                    else:
+                        where+=self.date_field + rf" LIKE '%{y}%' OR "
                 where = where[:-4]
             else:
                 start_date, stop_date = _process_date(year, date_field=self.date_field)
                 where = self.date_field + " between '" + start_date + "' and '" + stop_date +"'"
 
         if opt_filter is not None:
             if not isinstance(opt_filter, list):
@@ -1739,14 +2163,19 @@
         '''Returns False to indicate that Socrata data is not file-based
 
         Returns
         -------
         False
         '''
         return False
+    
+    def get_api_url(self):
+        url = self.url[:-1] if self.url.endswith('/') else self.url
+        url = url if url.startswith('http') else 'https://'+url
+        return f"{url}/resource/{self.data_set}.json"
 
 
     def get_count(self, year=None, *,  opt_filter=None, where=None, **kwargs):
         '''Get number of records for a Socrata data request
         
         Parameters
         ----------
@@ -1773,19 +2202,19 @@
         logger.debug(f"Request dataset {self.data_set} from {self.url}")
         logger.debug(f"\twhere={where}")
         logger.debug(f"\tselect=count(*)")
 
         try:
             results = self.client.get(self.data_set, where=where, select="count(*)")
         except (requests.HTTPError, requests.exceptions.ReadTimeout) as e:
-            raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+            raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.get_api_url()))
         except Exception as e: 
             if len(e.args)>0 and (e.args[0]=='Unknown response format: text/html' or \
                 "Read timed out" in e.args[0]):
-                raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+                raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.get_api_url()))
             else:
                 raise e  
             
         try:
             num_rows = float(results[0]["count"])
         except:
             num_rows = float(results[0]["count_1"]) # Value used in VT Shootings data
@@ -1866,15 +2295,15 @@
             logger.debug(f"\tlimit={batch_size}")
             logger.debug(f"\toffset={offset}")
             logger.debug(f"\torder={order}")
             try:
                 results = self.client.get(self.data_set, where=where,
                     limit=batch_size,offset=offset, select=select, order=order)
             except requests.HTTPError as e:
-                raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+                raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.get_api_url()))
             except Exception as e: 
                 arg_str = None
                 err = e
                 while True:
                     if len(err.args):
                         if isinstance(err.args[0],str):
                             arg_str = err.args[0]
@@ -1883,15 +2312,15 @@
                             err = err.args[0]
                         else:
                             break
                     else:
                         break
                 if arg_str and (arg_str=='Unknown response format: text/html' or \
                     "Read timed out" in arg_str):
-                    raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+                    raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.get_api_url()))
                 else:
                     raise e
 
             if use_gpd and output_type==None:
                 # Check for geo info
                 for r in results:
                     if "geolocation" in r or "geocoded_column" in r:
@@ -2028,14 +2457,17 @@
         '''Returns False to indicate that CKAN data is not file-based
 
         Returns
         -------
         False
         '''
         return False
+    
+    def get_api_url(self):
+        return f'{self.url}?sql=SELECT * FROM "{self.data_set}"'
 
 
     def get_count(self, year=None, opt_filter=None, **kwargs):
         '''Get number of records for a data request
         
         Parameters
         ----------
@@ -2064,16 +2496,16 @@
     def __request(self, where=None, return_count=False, out_fields="*", out_type="json", offset=0, count=None, orderby="_id"):
 
         if isinstance(out_fields, list):
             out_fields = '"' + '", "'.join(out_fields) + '"'
         elif not out_fields:
             out_fields = '*'
 
-        orderby = orderby if orderby else "_id"
         orderby = self.date_field if orderby=='date' else orderby
+        orderby = orderby if orderby else "_id"
 
         query = "SELECT "
         params = {}
         if return_count:
             query+="COUNT("+ out_fields + ")"
         else:
             query+=out_fields
@@ -2107,35 +2539,79 @@
 
         params["sql"] = query
 
         logger.debug(f"Request data from {self.url}")
         for k,v in params.items():
             logger.debug(f"\t{k} = {v}")
 
-        r = requests.get(self.url, params=params)
+        try:
+            r = requests.get(self.url, params=params)
+        except requests.exceptions.SSLError as e:
+            raise OPD_DataUnavailableError(self.url, e.args, self.get_api_url())
 
         try:
             r.raise_for_status()
         except requests.HTTPError as e:
             if len(e.args)>0:
                 if "503 Server Error" in e.args[0]:
-                    raise OPD_DataUnavailableError(self.url, e.args)
+                    raise OPD_DataUnavailableError(self.url, e.args, self.get_api_url())
                 else:
                     raise
 
             else: raise e
         except: raise
         
         return r.json()
 
 
-    def __construct_where(self, year=None, opt_filter=None):
+    def __construct_where(self, year=None, opt_filter=None, filter_year=False, sample_data=None):
         if self.date_field!=None and year!=None:
-            start_date, stop_date = _process_date(year, date_field=self.date_field)
-            where = f""""{self.date_field}" >= '{start_date}' AND "{self.date_field}" <= '{stop_date}'"""
+            datetime_format = None
+            if not sample_data:
+                sample_data = self.__request(count=100)
+            
+            date_col_info = [x for x in sample_data['result']["fields"] if x["id"]==self.date_field]
+            if len(date_col_info)==0:
+                raise ValueError(f"Date column {self.date_field} not found")
+            filter_year = date_col_info[0]["type"] not in ['timestamp','date']
+            if filter_year and date_col_info[0]["type"] == 'text':
+                # See if year can be filtered by YYYY-MM-DD 
+                dates = [x[self.date_field] for x in sample_data['result']['records']]
+                p = re.compile(r'^20\d{2}\-\d{2}\-\d{2}')
+                if all([p.search(x) for x in dates]):
+                    filter_year = False
+                    # Identify time format
+                    times = [p.sub('', x) for x in dates]
+                    if len(times[0])>0:
+                        if times[0][0]==' ':
+                            times = [x[1:] for x in times]
+                        else:
+                            raise ValueError(f"Dates in {self.date_field} are text (not date) values and have unknown format (i.e. {dates[0]})")
+                        
+                        if all([re.search(r'^\d{2}:\d{2}:\d{2}$',x) for x in times]):
+                            datetime_format = r'%Y-%m-%d %H:%M:%S'
+                        elif all(m:=[re.search(r'^\d{2}:\d{2}:\d{2}\+(\d{2})$',x) for x in times]):
+                            utc_offsets = [x.groups(1)[0] for x in m]
+                            if all([x==utc_offsets[0] for x in utc_offsets]):
+                                datetime_format = r'%Y-%m-%d %H:%M:%S+' + utc_offsets[0]
+                            else:
+                                raise ValueError(f"Dates in {self.date_field} are text (not date) values and have varying UTC offset")
+                        else:
+                            raise ValueError(f"Dates in {self.date_field} are text (not date) values and have unknown format (i.e. {dates[0]})")
+
+            if filter_year:
+                start_date, stop_date = _process_date(year, date_field=self.date_field, force_year=True)
+                where = ''
+                for y in range(int(start_date),int(stop_date)+1):
+                    # %25 is % wildcard symbol
+                    where+='"' + self.date_field + '"' + rf" LIKE '%{y}%' OR "
+                where = where[:-4]
+            else:
+                start_date, stop_date = _process_date(year, date_field=self.date_field, datetime_format=datetime_format)
+                where = f""""{self.date_field}" >= '{start_date}' AND "{self.date_field}" <= '{stop_date}'"""
         else:
             where = None
 
         if opt_filter:
             where = where if where else ""
             if not isinstance(opt_filter, list):
                 opt_filter = [opt_filter]
@@ -2173,20 +2649,23 @@
             (Optional) Columns to sort by. Default: '_id'
             
         Returns
         -------
         pandas or geopandas DataFrame
             DataFrame containing downloaded
         '''
+
+        data = self.__request(count=100)
+        date_cols = [x['id'] for x in data['result']["fields"] if x["type"] in ['timestamp','date']]
         
         if self._last_count is not None and self._last_count[0]==year and self._last_count[1]==opt_filter:
             record_count = self._last_count[2]
             where_query = self._last_count[3]
         else:
-            where_query = self.__construct_where(year, opt_filter)
+            where_query = self.__construct_where(year, opt_filter, sample_data=data)
             json = self.__request(where=where_query, return_count=True, out_fields=select)
             record_count = json['result']['records'][0]['count']
             self._last_count = (year, opt_filter, record_count, where_query)
 
         record_count-=offset
         if record_count<=0:
             return pd.DataFrame()
@@ -2197,20 +2676,18 @@
         batch_size = nrows if nrows < batch_size else batch_size
         num_batches = ceil(nrows / batch_size)
             
         pbar = pbar and num_batches>1
         if pbar:
             bar = tqdm(desc=self.url, total=nrows, leave=False)
 
-        data = self.__request(count=0)
-        date_cols = [x['id'] for x in data['result']["fields"] if x["type"]=='timestamp']
         if select:
             fields = select
         else:
-            # CKAN includes a large _full_text and _id columns that are not useful and the _full_text is large
+            # CKAN includes a large _full_text and _id columns that are not useful
             # Get info on columns in order to exclude these columns from the returned data
             
             fields = [x['id'] for x in data['result']['fields'] if x['id'] not in ['_id','_full_text']]
             
         features = []
         for batch in range(num_batches):
             bs = batch_size if batch<num_batches-1 else nrows-batch*batch_size
@@ -2220,15 +2697,15 @@
                 features.extend(data['result']['records'])
 
                 if batch==0 and len(features)>0:
                     if len(features) not in [batch_size, nrows]:
                         raise ValueError(f"Number of rows is {len(features)} but is expected to be max rows to read {batch_size} or total number of rows {nrows}")
             except Exception as e:
                 if len(e.args)>0 and "Error Code: 429" in e.args[0]:
-                    raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
+                    raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.get_api_url()))
                 else:
                     raise
             except:
                 raise
 
             if pbar:
                 bar.update(len(data['result']['records']))
@@ -2253,47 +2730,52 @@
 
 
 
 def _check_year(year):
     return isinstance(year, int) or (isinstance(year, str) and len(year)==4 and year.isdigit())
 
 
-def _process_date(date, date_field=None, force_year=False):
+def _process_date(date, date_field=None, force_year=False, datetime_format=None, is_date_string=False):
     if not isinstance(date, list):
         date = [date, date]
 
     if len(date)!=2:
         raise ValueError("date should be a list of length 2: [startYear, stopYear]")
 
     if date[0] > date[1]:
         raise ValueError('date[0] needs to be smaller than or equal to date[1]')
     
     is_year = force_year or (date_field != None and 'year' in date_field.lower())
-    for d in date:
-        if is_year and not _check_year(d):
-            raise DateFilterException(f"Column {date_field} is not a date column. It either contains a year or is a date but in a text format. "+
-                             "Currently, only a year filter is allowed for this case, but the input {d} appears to not be a year.")
-
-    if type(date[0]) == str:
-        # This should already be in date format
-        start_date = date[0]
-    elif is_year:
-        # Assuming this as actually a string or numeric field for the year rather than a datestamp
+    if is_year:
+        for d in date:
+            if not _check_year(d):
+                raise DateFilterException(f"Column {date_field} is not a date column. It either contains a year or is a date but in a text format. "+
+                                "Currently, only a year filter is allowed for this case, but the input {d} appears to not be a year.")
         start_date = str(date[0])
-    else:
-        start_date = str(date[0]) + "-01-01"
-
-    if type(date[1]) == str:
-        # This should already be in date format
-        stop_date = date[1]
-    elif is_year:
-        # Assuming this as actually a string or numeric field for the year rather than a datestamp
         stop_date = str(date[1])
     else:
-        stop_date  = str(date[1]) + "-12-31T23:59:59.999"
+        if isinstance(date[0], str) and re.search(r'^\d{4}-\d{2}-\d{2}$', date[0]):  # YYYY-MM-DD
+            start_date = date[0]
+        elif isinstance(date[0], numbers.Number) or re.search(r'^\d{4}$', date[0]):   # YYYY
+            start_date = str(date[0]) + "-01-01"
+        else:
+            raise ValueError(f"Unknown date input {date[0]}")
+
+        if isinstance(date[1], str) and re.search(r'^\d{4}-\d{2}-\d{2}$', date[1]):  # YYYY-MM-DD
+            # If date date are strings, the ASCII character for z will be greater than all possible values that follow date[1]
+            stop_date  = str(date[1])+'zz' if is_date_string else str(date[1])+"T23:59:59.999"
+        elif isinstance(date[1], numbers.Number) or re.search(r'^\d{4}$', date[1]):   # YYYY
+            # If date date are strings, the ASCII character for z will be greater than all possible values that follow date[1]
+            stop_date  = str(date[1])+'-12-31zz' if is_date_string else str(date[1])+"-12-31T23:59:59.999"
+        else:
+            raise ValueError(f"Unknown date input {date[1]}")
+
+    if datetime_format:
+        start_date = datetime.strftime(pd.to_datetime(start_date), datetime_format)
+        stop_date = datetime.strftime(pd.to_datetime(stop_date), datetime_format)
 
     return start_date, stop_date
 
 
 def filter_dataframe(df, date_field=None, year_filter=None, agency_field=None, agency=None):
     '''Filter dataframe by agency and/or year (range)
     
@@ -2307,15 +2789,15 @@
         (Optional) Either the year or the year range [first_year, last_year] for the data that is being requested.  None value returns data for all years.
     agency_field : str
         (Optional) Name of the column that contains the agency name (i.e. name of the police departments)
     agency : str
         (Optional) Name of the agency to filter for. None value returns data for all agencies.
     '''
 
-    if date_field != None:
+    if pd.notnull(date_field):
         is_year = date_field.lower()=='year'
         if not is_year and pd.api.types.is_integer_dtype(df[date_field]):
             is_year = ((df[date_field] >= 1900) & (df[date_field] <= 2200)).all()
 
         if not is_year and not hasattr(df[date_field], "dt"):
             with warnings.catch_warnings():
                 # Ignore future warning about how this operation will be attempted to be done inplace:
@@ -2326,34 +2808,48 @@
                 try:
                     df[date_field] = to_datetime(df[date_field], ignore_errors=True)
                 except:
                     return df
     
         if year_filter != None:
             if isinstance(year_filter, list):
+                if len(year_filter) != 2:
+                    raise ValueError(f'Format of the input {year_filter} is invalid.'
+                                     'Date/year filters that are lists are expected to be a length 2 list of ' +
+                                     '[startYear, stopYear] or [startDate, stopDate]. Dates should be in '+
+                                     'YYYY-MM-DD format.')
                 if not is_year:
-                    if isinstance(year_filter[0],int):
-                        if len(year_filter)==1:
-                            year_filter.append(f"{year_filter[0]}-12-31")
+                    if isinstance(year_filter[0],int) or is_str_number(year_filter[0]):
                         year_filter[0] = f"{year_filter[0]}-01-01"
-                    if isinstance(year_filter[-1],int):
-                        year_filter[-1] = f"{year_filter[-1]}-12-31"
-                    logger.debug(f"Keeping values of column {date_field} between {year_filter[0]} and {year_filter[-1]}")
-                    df = df[(df[date_field] >= year_filter[0]) & (df[date_field] <= year_filter[-1])]
-                else:
+                    elif not (re.search(r'\d{4}-\d{2}-\d{2}', year_filter[0]) or \
+                              re.search(r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}', year_filter[0])):
+                        raise ValueError(f"{year_filter[0]} must be in YYYY-MM-DD format")
+                    
+                    if isinstance(year_filter[-1],int) or is_str_number(year_filter[0]):
+                        year_filter[-1] = f"{year_filter[-1]}-12-31T23:59:59.999"
+                    elif re.search(r'\d{4}-\d{2}-\d{2}', year_filter[1]):
+                        year_filter[-1] = f"{year_filter[-1]}T23:59:59.999"
+                    elif not re.search(r'\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}', year_filter[1]):
+                        raise ValueError(f"{year_filter[0]} must be in YYYY-MM-DD format")
+                    logger.debug(f"Keeping values of column {date_field} between {year_filter[0]} and {year_filter[1]}")
+                    df = df[(df[date_field] >= year_filter[0]) & (df[date_field] <= year_filter[1])]
+                elif (isinstance(year_filter[0],int) or is_str_number(year_filter[0])) and \
+                     (isinstance(year_filter[1],int) or is_str_number(year_filter[1])):
                     logger.debug(f"Column {date_field} has been identfied as a year column")
-                    logger.debug(f"Keeping values of column {date_field} between {year_filter[0]} and {year_filter[-1]}")
-                    df = df[df[date_field].isin(range(year_filter[0], year_filter[-1]+1))]
+                    logger.debug(f"Keeping values of column {date_field} between {year_filter[0]} and {year_filter[1]}")
+                    df = df[df[date_field].isin(range(year_filter[0], year_filter[1]+1))]
+                else:
+                    raise ValueError(f"Column {date_field} has been identfied as a year column and cannot be filtered by dates: {year_filter}")
             elif not is_year:
                 logger.debug(f"Keeping values of column {date_field} for year={year_filter}")
-                df = df[df[date_field].dt.year == year_filter]
+                df = df[df[date_field].dt.year == int(year_filter)]
             else:
                 logger.debug(f"Column {date_field} has been identfied as a year column")
                 logger.debug(f"Keeping values of column {date_field} for year={year_filter}")
-                df = df[df[date_field] == year_filter]
+                df = df[df[date_field] == int(year_filter)]
 
     if agency != None and agency_field != None:
         logger.debug(f"Keeping values of column {agency_field} that are equal to {agency}")
         df = df.query(agency_field + " = '" + agency + "'")
 
     return df
```

### Comparing `openpolicedata-0.6/openpolicedata/datasets.py` & `openpolicedata-0.7/openpolicedata/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     }
 
 
 def _build(csv_file, error=False):
 
     loaded, df = check_compat_source_table(column_types=_column_types)
 
-    if not loaded:
+    if isinstance(csv_file, pd.DataFrame):
+        df = csv_file.copy()
+    elif not loaded:
         try:
             df = pd.read_csv(csv_file, dtype=_column_types)
         except:
             if error:
                 raise
             warnings.warn(f"Unable to load CSV file from {csv_file}. " +
                 "This may be due to a bad internet connection or bad filename/URL.")
@@ -47,21 +49,21 @@
     if "Jurisdiction" in df:
         df.rename(columns={
             "Jurisdiction" : "Agency",
             "jurisdiction_field" : "agency_field"
         }, inplace=True)
 
     # Convert years to int
-    df["Year"] = [int(x) if x.isdigit() else x for x in df["Year"]]
+    df["Year"] = [int(x) if isinstance(x,str) and x.isdigit() else x for x in df["Year"]]
     df["Year"] = df["Year"].apply(lambda x: defs.MULTI if x=="MULTI" else x)
     df["SourceName"] = df["SourceName"].str.replace("Police Department", "")
     df["Agency"] = df["Agency"].str.replace("Police Department", "").apply(lambda x: defs.MULTI if x=="MULTI" else x)
 
     for col in df.columns:
-        df[col] = [x.strip() if type(x)==str else x for x in df[col]]
+        df[col] = [x.strip() if isinstance(x, str) else x for x in df[col]]
 
     # ArcGIS datasets should have a URL ending in either /FeatureServer/# or /MapServer/#
     # Where # is a layer #
     urls = list(df["URL"])
     p = re.compile(r"(MapServer|FeatureServer)/\d+")
     for i,url in enumerate(urls):
         if df.iloc[i]["DataType"] == defs.DataType.ArcGIS:
@@ -77,30 +79,32 @@
         raise ValueError(f"{len(misspelled)} states are misspelled in the data sources table including {misspelled.iloc[0]} at index {misspelled.index[0]}")
 
     key_vals = ['State', 'SourceName', 'Agency', 'TableType','Year', 'coverage_start', 'coverage_end']
     df.drop_duplicates(subset=key_vals, inplace=True, ignore_index=True)
 
     if "coverage_start" in df:
         p = re.compile(r"\d{1,2}/\d{1,2}/\d{4}")
-        df["coverage_start"] = df["coverage_start"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
-        df["coverage_end"] = df["coverage_end"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
+        df["coverage_start"] = df["coverage_start"].apply(lambda x: pd.to_datetime(x) if \
+                                                          not isinstance(x,pd.Timestamp) and pd.notnull(x) and p.search(x) else x)
+        df["coverage_end"] = df["coverage_end"].apply(lambda x: pd.to_datetime(x) if \
+                                                      not isinstance(x,pd.Timestamp) and pd.notnull(x) and p.search(x) else x)
 
     return DeprecationHandlerDataFrame(df)
 
 
 datasets = _build(csv_file)
 
 
-def reload(csvfile: str = csv_file):
+def reload(csvfile: Union[str,pd.DataFrame] = csv_file):
     """Reload default datasets CSV file or load datasets CSV from local file. Useful if datasets file may have been updated.
 
     Parameters
     ----------
-    csvfile : str, optional
-        OPTIONAL CSV file location, by default the default OPD CSV file will be loaded from GitHub
+    csvfile : str, pd.DataFrame, optional
+        OPTIONAL CSV file location or pandas DataFrame, by default the default OPD CSV file will be loaded from GitHub
     """
 
     from .import datasets
     datasets.datasets = _build(csvfile, error=True)
     
 
 def query(
```

### Comparing `openpolicedata-0.6/openpolicedata/datetime_parser.py` & `openpolicedata-0.7/openpolicedata/datetime_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import datetime
+import math
 import numpy as np
 import pandas as pd
+from pandas .api.types import is_numeric_dtype
 import datetime as dt
 import re
 import warnings
+import numbers
+
+from .utils import is_str_number
 
 def parse_date_to_datetime(date_col):
     if len(date_col.shape)==2:
         if date_col.shape[1] > 1:
             dts = date_col.iloc[:,0][date_col.iloc[:,0].notnull()]
             if hasattr(dts.iloc[0], "year"):
                 if isinstance(dts.dtype, pd.api.types.PeriodDtype):
@@ -15,15 +21,15 @@
                     un_vals = to_datetime(dts.unique())
                 if (un_vals.month != 1).any() or (un_vals.day != 1).any() or (un_vals.hour != 0).any() or \
                     (un_vals.minute != 0).any() or (un_vals.second != 0).any():
                     raise ValueError("Expected year data to not contain any month, day, or time info")
 
                 # Making a copy to avoid warning
                 d = date_col.copy()
-                d.iloc[:,0] = date_col.iloc[:,0].dt.year
+                d[d.columns[0]] = date_col.iloc[:,0].dt.year
 
                 def month_name_to_num(x):
                     month_list = ["jan","feb","mar","apr","may","jun","jul","aug","sep","oct","nov","dec"]
                     if isinstance(x,str) and not x.isdigit():
                         month_num = [k+1 for k,y in enumerate(month_list) if x.lower().startswith(y)]
                         return month_num[0]
                     else:
@@ -39,56 +45,73 @@
                     return to_datetime(d)
         else:
             date_col = date_col.iloc[:,0]
 
     dts = date_col[date_col.notnull()]
 
     if len(dts) > 0:
-        one_date = dts.iloc[0] 
-        if not hasattr(one_date, "year"):
-            is_num = date_col.dtype == np.int64
+        if not hasattr(dts.iloc[0], "year") or (dts.apply(type)==str).any():
+            is_num = is_numeric_dtype(date_col)
             if not is_num:
                 # Try to convert to all numbers
                 with warnings.catch_warnings():
                     warnings.filterwarnings("ignore", category=RuntimeWarning, message="invalid value encountered in cast")
                     new_col = date_col.convert_dtypes()
                 if new_col.dtype in ["object", "string", "string[python]"] and \
-                    new_col.apply(lambda x: pd.isnull(x) or isinstance(x,int) or x.isdigit() or x.strip()=="").all():
-                    date_col = new_col.apply(lambda x: int(x) if (pd.notnull(x) and (isinstance(x,int) or x.isdigit())) else np.nan)
+                    new_col.apply(lambda x: pd.notnull(x) and (isinstance(x, numbers.Number) or \
+                                  (isinstance(x,str) and (x.isdigit() or x.strip()=="")))).sum() > 0 and \
+                    new_col.apply(lambda x: pd.isnull(x) or isinstance(x,(pd.Timestamp,int, dt.datetime)) or \
+                                  isinstance(x, numbers.Number) or \
+                                  (isinstance(x,str) and (x.isdigit() or x.strip()==""))).sum()>=len(new_col)-1:
+                    # Almost all numeric, null, or timestamp values and at least one numeric value
+                    def clean_dates(x):
+                        if pd.notnull(x) and (isinstance(x, numbers.Number) or is_str_number(x)):
+                            return int(x)
+                        elif isinstance(x,str):
+                            return np.nan
+                        else:
+                            return x
+                        
+                    date_col = new_col.apply(clean_dates)
                     dts = date_col[date_col.notnull()]
                     is_num = True
 
             if is_num:
                 # Date as number like MMDDYYYY. Need to determine order
                 # Assuming year is either first or last
                 if (dts < 0).any():
                     raise ValueError("Date values cannot be negative")
 
                 year_last = dts % 10000
                 year_first = np.floor(dts / 10000)
+                year_last_2digit = dts % 100
                 this_year = dt.datetime.now().year
 
                 is_valid_last = (year_last <= this_year).all() and (year_last > 1300).all()
                 is_valid_first = (year_first <= this_year).all() and (year_first > 1300).all()
+                is_valid_last_2digit = (year_last_2digit <= this_year-2000).all() and (year_last_2digit >= 0).all()
 
                 any_valid = True
                 if is_valid_first and is_valid_last:
                     raise ValueError("Error parsing date")
                 elif is_valid_first:
                     year = date_col.apply(lambda x : np.floor(x / 10000) if not pd.isnull(x) else x)
                     month_day = date_col.apply(lambda x : x % 10000 if not pd.isnull(x) else x)
                 elif is_valid_last:
                     year = date_col.apply(lambda x : x % 10000 if not pd.isnull(x) else x)
                     month_day = date_col.apply(lambda x : np.floor(x / 10000) if not pd.isnull(x) else x)
+                elif is_valid_last_2digit:
+                    year = 2000+date_col.apply(lambda x : x % 100 if not pd.isnull(x) else x)
+                    month_day = date_col.apply(lambda x : np.floor(x / 100) if not pd.isnull(x) else x)
                 else:
                     any_valid = False
 
                 if any_valid:
                     # Determine if month is first or last in month_day
-                    first_val = np.floor(month_day / 100)
+                    first_val = month_day.apply(lambda x: np.floor(x/100) if pd.notnull(x) and isinstance(x,numbers.Number) else x)
                     last_val = month_day % 100
 
                     is_valid_month_first = first_val.max() < 13 and last_val.max() < 32
                     is_valid_month_last = last_val.max() < 13 and first_val.max() < 32
                     if is_valid_month_first and is_valid_month_last:
                         raise ValueError("Error parsing month and day")
                     elif is_valid_month_first:
@@ -118,25 +141,29 @@
                     if new_date_col.dt.year.max() < 1980:
                         raise ValueError("All dates are before 1980. This is unlikely to be a date column.")
 
                     return new_date_col
                     
             elif date_col.dtype in ["O", "object", "string", "string[python]"]:
                 new_col = date_col.convert_dtypes()
-                if new_col.dtype in ["string", "string[python]"]:
+                if new_col.dtype in ["string", "string[python]"] or \
+                    str in new_col.apply(type).unique():
                     p = re.compile(r"\d{1,2}[/-]\d{1,2}[/-]\d{2,4}")
                     p2 = re.compile(r"\d{4}[/-]\d{1,2}[/-]\d{1,2}")
                     p3 = re.compile(r"\d{2}-[A-Z][a-z][a-z]-\d{2,4}", re.IGNORECASE)
                     p_not_match = re.compile(r"\d{1,2}[:\.]?\d\d[:\.]?\d?\d?")
                     num_match = 0
                     num_not_match = 0
                     k = 0
                     num_check = min(5, len(new_col))
                     for m in range(len(new_col)):
-                        if pd.notnull(new_col[m]) and len(new_col[m].strip())!=0:
+                        if isinstance(new_col[m], (pd.Timestamp, dt.datetime)):
+                            num_match+=1
+                            k+=1
+                        elif pd.notnull(new_col[m]) and len(new_col[m].strip())!=0:
                             if p.search(new_col[m]) or p2.search(new_col[m]) or p3.search(new_col[m]):
                                 num_match+=1
                             elif p_not_match.match(new_col[m])==None:
                                 pass
                             else:
                                 num_not_match+=1
                             k+=1
@@ -396,14 +423,17 @@
                 x = x.replace(" ","")
                 time_list = x.split(":")
                 if len(time_list)==1 and len(x.split("."))>1:
                     time_list = x.split(".")
                     if len(time_list)!=3:
                         raise NotImplementedError()
 
+                if len(time_list)==1 and len(x)==5 and x[2]==';':
+                    # Accidentally used ; instead of :
+                    time_list = x.split(";")
                 if len(time_list)==1:
                     if x.strip() in ["","-"]:
                         return pd.NaT
                     elif len(x) == 0 or len(x) > 4 or not x.isdigit():
                         if x in ["#NAME?",'#VALUE!', 'TIME','NULL'] or re.search(r'^C\d+',x) or \
                             any([y.search(x) for y in p_date]):  # Date accidently entered in time column
                             # C2 values were observed in 1 dataset
@@ -462,34 +492,79 @@
 
 def to_datetime(col, ignore_errors=False, *args, **kwargs):
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=UserWarning, message="Could not infer format")
         try:
             return pd.to_datetime(col, *args, **kwargs)
         except UnicodeEncodeError as e:
-            if ignore_errors and isinstance(col, pd.Series):
+            if (ignore_errors or 'errors' in kwargs and kwargs['errors']=='coerce') and isinstance(col, pd.Series):
+                coerce = 'errors' in kwargs and kwargs['errors']=='coerce'
                 def to_datetime_local(x, *args, **kwargs):
                     try:
                         return pd.to_datetime(x, *args, **kwargs)
                     except:
-                        return x
+                        return pd.NaT if coerce else x  # Coerce input to pd.to_datetime should return NaT if cannot convert to datetime
                 return col.apply(to_datetime_local)
             else:
                 return col
+        except pd._libs.tslibs.parsing.DateParseError as e:
+            if 'out of range' in str(e) and not isinstance(col, pd.Series) and re.search(r'year 20\d{6} is out of range: 20\d{6}.0, at position 0', str(e)):
+                return to_datetime(col[:-2])
+            elif ignore_errors and 'out of range' in str(e) and not isinstance(col, pd.Series):
+                return col
+            elif ignore_errors and isinstance(col,str) and \
+                ((m:=re.search(r'^(?P<year>\d{4})\-(?P<month>[\d\_]{2})\-\_\_', col)) or \
+                 (m:=re.search(r'^(?P<year>\d{4})\-(?P<month>[\_]{2})\-\d{2}', col))):
+                if m.groupdict()['month'].isdigit():
+                    return pd.Period(freq='M', year=int(m.groupdict()['year']), month=int(m.groupdict()['month']))
+                else:
+                    return pd.Period(freq='Y', year=int(m.groupdict()['year']))
+            else:
+                raise
         except ValueError as e:
             if ignore_errors and "Given date string" in str(e) and "not likely a datetime" in str(e) and \
                 (len(args)>0 or 'errors' not in kwargs or kwargs['errors']!='coerce'):
                 new_kwargs = kwargs.copy()
                 new_kwargs['errors'] = 'coerce'
                 dts = pd.to_datetime(col, *args, **new_kwargs)
                 raise NotImplementedError()
             elif ignore_errors and isinstance(col,str) and \
                 ((m:=re.search(r'^(?P<year>\d{4})\-(?P<month>[\d\_]{2})\-\_\_', col)) or \
                  (m:=re.search(r'^(?P<year>\d{4})\-(?P<month>[\_]{2})\-\d{2}', col))):
                 if m.groupdict()['month'].isdigit():
                     return pd.Period(freq='M', year=int(m.groupdict()['year']), month=int(m.groupdict()['month']))
                 else:
                     return pd.Period(freq='Y', year=int(m.groupdict()['year']))
+            elif 'doesn\'t match format "%Y-%m-%dT%H:%M:%S.%f%z"' in str(e):
+                return pd.to_datetime(col.apply(lambda x: x[:-1] if isinstance(x,str) and x[-1]=='Z' else x), format='mixed')
+            elif ignore_errors and 'is out of range' in str(e) and is_str_number(col):
+                if (dec:=col.find('.'))>0 and int(col[dec+1:])==0:
+                    col = int(col[:dec])
+                    year_first = math.floor(col/10000)
+                    year_last = col % 10000
+
+                    is_year_first = 1980 <= year_first <= datetime.datetime.now().year
+                    is_year_last =  1980 <= year_last <= datetime.datetime.now().year
+                    if is_year_first + is_year_last != 1:
+                        raise e
+                    elif is_year_first:
+                        year = year_first
+                        month_day = col - year*10000
+                        month = math.floor(month_day/100)
+                        day = month_day - month*100
+                    else:
+                        year = year_last
+                        month_day = year_first
+                        month = math.floor(month_day/100)
+                        day = month_day - month*100
+                    if month>12 or day>31:
+                        raise e
+                    return pd.to_datetime(datetime.datetime(year=year, month=month, day=day))
+                else:
+                    raise e
+            elif ignore_errors and re.search(r'Unknown string format: \d+[-/]\d+[-/]\d+,?\s?\d+[-/]\d+[-/]\d+', str(e)):
+                # Comma separated list of dates. Just return value
+                return col
             else:
                 return pd.to_datetime(col, *args, format='mixed', **kwargs)
         except Exception as e:
             raise
```

### Comparing `openpolicedata-0.6/openpolicedata/defs.py` & `openpolicedata-0.7/openpolicedata/defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,21 @@
     CITATIONS = ("CITATIONS","Commonly referred to as tickets, citations indicate a violation of the law and may be given for "+
         "violations such as traffic and civil violations")
     COMPLAINTS = ("COMPLAINTS","Complaints of police misconduct made internally or by the community")
     COMPLAINTS_ALLEGATIONS = ("COMPLAINTS - ALLEGATIONS",
         "Complaint data may be split into several tables. This table contains specific data on the allegations.")
     COMPLAINTS_BACKGROUND = ("COMPLAINTS - BACKGROUND",
         "Complaint data may be split into several tables. This table contains data on the general background of the complaints.")
+    COMPLAINTS_BODY_WORN_CAMERA = ("COMPLAINTS - BODY WORN CAMERA",
+        "Complaint data may be split into several tables. This table contains data on body worn camera details.")
     COMPLAINTS_SUBJECTS = ("COMPLAINTS - SUBJECTS",
         "Complaint data may be split into several tables. This table contains specific data on the involved subjects.")
+    COMPLAINTS_SUBJECTS_OFFICERS = ("COMPLAINTS - SUBJECTS/OFFICERS",
+        "Complaint data may be split into several tables. This table contains data on the involved subjects and officers. "+
+        "A row in the data will indicate whether that row corresponds to an officer or subject.")
     COMPLAINTS_OFFICERS = ("COMPLAINTS - OFFICERS",
         "Complaint data may be split into several tables. This table contains specific data on the involved officers.")
     COMPLAINTS_PENALTIES = ("COMPLAINTS - PENALTIES",
         "Complaint data may be split into several tables. This table contains specific data on any resulting penalties.")
     CRASHES = ("CRASHES", "Traffic crashes")
     CRASHES_SUBJECTS = ("CRASHES - SUBJECTS",
         "Crash data may be split into several tables due to the possibility that multiple "+
@@ -85,32 +90,45 @@
         "subjects and vehicles may be involved in an incident. This table contains data on vehicles.")
     DISCIPLINARY_RECORDS = ("DISCIPLINARY RECORDS",
         "Disciplinary records of officers")
     EMPLOYEE = ("EMPLOYEE","Demographic data of the police workforce")
     DEATHS_IN_CUSTODY = ("DEATHS IN CUSTODY", "Deaths that occur in custody or during the process of arrest")
     FIELD_CONTACTS = ("FIELD CONTACTS", "Consensual contacts between officers and the community.")
     INCIDENTS = ("INCIDENTS", "Crime incident reports")
+    INCIDENTS_INCIDENTS = ("INCIDENTS - INCIDENTS", 
+                          "Incidents data may be split into several tables due to the possibility that multiple "+
+                        "subjects may be involved in an incident. This table contains data on the details of the incident.")
+    INCIDENTS_SUBJECTS = ("INCIDENTS - SUBJECTS", 
+                          "Incidents data may be split into several tables due to the possibility that multiple "+
+                        "subjects may be involved in an incident. This table contains data on subjects.")
     LAWSUITS = ("LAWSUITS", "Lawsuits against a police department")
     PEDESTRIAN = ("PEDESTRIAN STOPS","Stops of pedestrians based on 'reasonable suspicion'. May lead to a frisk.")
     PEDESTRIAN_ARRESTS = ("PEDESTRIAN ARRESTS","Pedestrian stops leading to an arrest")
     PEDESTRIAN_CITATIONS = ("PEDESTRIAN CITATIONS","Pedestrian stops leading to a citation")
     PEDESTRIAN_WARNINGS = ("PEDESTRIAN WARNINGS","Pedestrian stops leading to a warning")
+    POINTING_WEAPON = ('POINTING WEAPON', "Instances of officers pointing a weapon (firearm, Taser, etc.) at individuals.")
     SHOOTINGS = ("OFFICER-INVOLVED SHOOTINGS","Shootings by officers")
     SHOOTINGS_SUBJECTS = ("OFFICER-INVOLVED SHOOTINGS - SUBJECTS",
         "Officer-involved shootings data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on subjects.")
     SHOOTINGS_OFFICERS = ("OFFICER-INVOLVED SHOOTINGS - OFFICERS",
         "Officer-involved shootings data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on officer.")
     SHOOTINGS_INCIDENTS = ("OFFICER-INVOLVED SHOOTINGS - INCIDENTS",
         "Officer-involved shootings data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on the incident.")
     STOPS = ("STOPS","Contains data on both pedestrian and traffic stops.")
     TRAFFIC = ("TRAFFIC STOPS","Traffic stops are stops by police of motor vehicles due to reasonable suspicion " + 
         " or traffic violations.")
+    TRAFFIC_INCIDENTS = ("TRAFFIC STOPS - INCIDENTS",
+        "Traffic stops data may be split into several tables due to the possibility that multiple "+
+        "subjects and officers may be involved in an incident. This table contains data on the incident.")
+    TRAFFIC_SUBJECTS = ("TRAFFIC STOPS - SUBJECTS",
+        "Traffic stops data may be split into several tables due to the possibility that multiple "+
+        "subjects and officers may be involved in an incident. This table contains data on the subjects.")
     TRAFFIC_ARRESTS = ("TRAFFIC ARRESTS","Traffic stops leading to an arrest.")
     TRAFFIC_CITATIONS = ("TRAFFIC CITATIONS","Traffic stops leading to a citation.")
     TRAFFIC_WARNINGS = ("TRAFFIC WARNINGS","Traffic stops leading to a warning.")
     USE_OF_FORCE = ("USE OF FORCE","Documentation of physical force used against subjects.")
     USE_OF_FORCE_SUBJECTS = ("USE OF FORCE - SUBJECTS",
         "Use of force data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on subjects.")
@@ -118,15 +136,16 @@
         "Use of force data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on officer.")
     USE_OF_FORCE_INCIDENTS = ("USE OF FORCE - INCIDENTS",
         "Use of force data may be split into several tables due to the possibility that multiple "+
         "subjects and officers may be involved in an incident. This table contains data on the incident.")
     USE_OF_FORCE_SUBJECTS_OFFICERS = ("USE OF FORCE - SUBJECTS/OFFICERS",
         "Use of force data may be split into several tables due to the possibility that multiple "+
-        "subjects and officers may be involved in an incident. This table contains data on subjects and officers.")
+        "subjects and officers may be involved in an incident. This table contains data on subjects and officers."+
+        "A row in the data will indicate whether that row corresponds to an officer or subject.")
     VEHICLE_PURSUITS = ("VEHICLE PURSUITS","Attempts by officers in vehicles to pursue vehicles where the operator " + 
         "is believed to be aware that they are being signaled to stop but who is fleeing or ignoring the officer's attempt "+
         "to stop them.")
 
 # Constants used in dataset parameters
 MULTI = "MULTIPLE"    # For data sets that put multiple years or agencies in 1 dataset
 NA = "NONE"         # None = not applicable (pandas converts "N/A" to NaN)
```

### Comparing `openpolicedata-0.6/openpolicedata/deprecated/_decorators.py` & `openpolicedata-0.7/openpolicedata/deprecated/_decorators.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/openpolicedata/deprecated/_pandas.py` & `openpolicedata-0.7/openpolicedata/deprecated/_pandas.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/openpolicedata/deprecated/source_table_compat.py` & `openpolicedata-0.7/openpolicedata/deprecated/source_table_compat.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/openpolicedata/exceptions.py` & `openpolicedata-0.7/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.6/openpolicedata/preproc.py` & `openpolicedata-0.7/openpolicedata/preproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import data_loaders
 from . import datetime_parser
 from . import defs
 from . import _converters as convert
 from ._converters import  _p_age_range
 from ._preproc_utils import _MultData, check_column, DataMapping, _case, MultType
 from .exceptions import BadCategoryDict
-from .utils import camel_case_split, split_words
+from .utils import camel_case_split, split_words, is_str_number
 
 _skip_tables = ["calls for service"]
 _OLD_COLUMN_INDICATOR = "RAW"
 
 logger = logging.getLogger("opd-std")
 logger.setLevel(logging.WARNING)
 sh = logging.StreamHandler()
@@ -70,14 +70,15 @@
         self.cur_dict[new_key] = self.cur_dict.pop(old_key)
         self.orig_dict[new_key] = self.orig_dict.pop(old_key)
         
 
 def standardize(df, table_type, year, 
     known_cols={}, 
     source_name=None, 
+    state=None, 
     keep_raw=True,
     agg_race_cat=False,
     race_cats=defs.get_race_cats(),
     eth_cats=defs.get_eth_cats(),
     gender_cats=defs.get_gender_cats(),
     no_id="keep",
     race_eth_combo="merge",
@@ -86,15 +87,15 @@
 
     if table_type.lower() in _skip_tables:
         print(f"Standardization is not currently applied to {table_type} table.")
         return df, None
     
     logger.info(f"Original columns:\n{df.columns}")
     
-    std = Standardizer(df, table_type, year, known_cols, source_name, keep_raw, agg_race_cat, race_cats, eth_cats, gender_cats, no_id)
+    std = Standardizer(df, table_type, year, known_cols, source_name, state, keep_raw, agg_race_cat, race_cats, eth_cats, gender_cats, no_id)
 
     std.id_columns()
     std.standardize_date()
     std.standardize_time()
     if merge_date_time:
         std.merge_date_time(empty_time=empty_time)
     std.standardize_columns(convert.convert_off_or_civ, col_names=defs.columns.SUBJECT_OR_OFFICER)
@@ -140,15 +141,15 @@
 
 
 def find_id_column(df1, df2, std_id, keep_raw):
     df1 = df1.copy()
     df2 = df2.copy()
     default_result = (None, None, df1, df2, None)
 
-    p_inc_id = r'incident(_|\s)?(id|num|number|code)$'
+    p_inc_id = r'(incident|stop)(_|\s)?(id|num|number|code)$'
     inc_id_matches1 = [x for x in df1.columns if re.search('^'+p_inc_id,x, re.IGNORECASE)]
     inc_id_matches1 = inc_id_matches1 if len(inc_id_matches1) else [x for x in df1.columns if re.search(p_inc_id,x, re.IGNORECASE)]
     inc_id_matches2 = [x for x in df2.columns if re.search('^'+p_inc_id,x, re.IGNORECASE)]
     inc_id_matches2 = inc_id_matches2 if len(inc_id_matches2) else [x for x in df2.columns if re.search(p_inc_id,x, re.IGNORECASE)]
 
     if len(inc_id_matches1)>1 or len(inc_id_matches2)>1:
         raise NotImplementedError()
@@ -172,31 +173,36 @@
                 if 'incident'.startswith(words[0]) and words[1] in ['num','id', 'number']:
                     id_col1 = col1
                     id_col2 = col2
                     break
         
         if not id_col1:
             # If not incident ID, check for other types
-            id_words = ['master','crime','complaint','tax','log','collision','report']
+            id_words = ['master','crime','complaint','tax','log','collision','report','case']
             for c in possible_cols:
                 col1 = [x for x in df1.columns if x.lower()==c][0]
                 col2 = [x for x in df2.columns if x.lower()==c][0]
                 words = split_words(c, case='lower')
                 for w in id_words:
                     if c.lower()==w+"id" or c.lower()==w+"_subject_id" or (len(words)==2 and words[0]==w and words[1] in ['num','id', 'number','no']):
                         id_col1 = col1
                         id_col2 = col2
                         break
                 if id_col1:
                     break
 
         if not id_col1:
-            if 'id' in possible_cols:
+            if (c:='id') in possible_cols or (c:='filenum') in possible_cols:
                 id_col1 = [x for x in df1.columns if x.lower()==c][0]
                 id_col2 = [x for x in df2.columns if x.lower()==c][0]
+            elif any([(c1:=x) for x in df1.columns if x.lower() in ['casenumber','accidentnumber']]) and \
+                 any([(c2:=x) for x in df2.columns if x.lower() in ['casenumber','accidentnumber']]) and \
+                 (df2[c2].isin(df1[c1].unique()).mean()>0.98 or df1[c1].isin(df2[c2].unique()).mean()>0.98):  # Norman crashes dataset
+                id_col1 = c1
+                id_col2 = c2
             else:
                 return default_result         
     
     mapping = None
     if std_id:
         # Save column off rather than creating it before cleanup in case original column name matches new column name
         col1 = df1[id_col1]
@@ -256,15 +262,24 @@
     is_exempt = col.apply(lambda x: "Marsy" in x and "Exempt" in x if isinstance(x,str) else False)
     max_num_vals[is_exempt] = np.nan
 
     return max_num_vals, delim, max_count, is_exempt
 
 
 def _find_gender_col_type_advanced(df, source_name, col_names, types, col_map, civilian_col_name, officer_col_name):
-    if ("subject_sex" in col_names or "officer_sex" in col_names) and \
+    if source_name=='Bloomington' and \
+        len(col_names)==2 and \
+        all([x==civilian_col_name] for x in types) and \
+        all([any([y.lower() in x.lower() for y in ['_male','_female'] for x in col_names])]) and \
+        all([x.startswith('suspect_gender') for x in col_names]):
+        # This dataset has separate boolean columns for each race 
+        # Indicate that all columns should be combined into a single column
+        col_names = [col_names]
+        types = [types[0]]
+    elif ("subject_sex" in col_names or "officer_sex" in col_names) and \
         any([x.startswith("raw_") for x in col_names]):
         # Stanford data
         old_col_names = col_names
         old_types = types
         col_names = []
         types = []
         for x,y in zip(old_col_names, old_types):
@@ -276,15 +291,24 @@
     else:
         col_names, types = _set_type_based_on_order(col_names, types, df, source_name, officer_col_name, civilian_col_name)
 
     return col_names, types
 
 
 def _find_race_col_type_advanced(df, source_name, col_names, types, col_map, civilian_col_name, officer_col_name):
-    if ("subject_race" in col_names or "officer_race" in col_names) and \
+    if source_name=='Bloomington' and \
+        len(col_names)>=3 and \
+        all([x==civilian_col_name] for x in types) and \
+        all([any([y.lower() in x.lower() for y in ['white','_aa_','asian','indian'] for x in col_names])]) and \
+        all([x.startswith('suspect_race') for x in col_names]):
+        # This dataset has separate boolean columns for each race 
+        # Indicate that all columns should be combined into a single column
+        col_names = [col_names]
+        types = [types[0]]
+    elif ("subject_race" in col_names or "officer_race" in col_names) and \
         any([x.startswith("raw_") for x in col_names]):
         # Stanford data
         old_col_names = col_names
         old_types = types
         col_names = []
         types = []
         for x,y in zip(old_col_names, old_types):
@@ -360,27 +384,29 @@
     return col_names, types
 
 
 class Standardizer:
     def __init__(self, df, table_type, year, 
             known_cols={}, 
             source_name=None, 
+            state=None,
             keep_raw=True,
             agg_race_cat=False,
             race_cats=defs.get_race_cats(),
             eth_cats=defs.get_eth_cats(),
             gender_cats=defs.get_gender_cats(),
             no_id="keep"
         ) -> None:
 
         self.df = df
         self.table_type = table_type
         self.year = year
         self.known_cols = defaultdict(lambda: None, known_cols)
         self.source_name = source_name
+        self.state = state
         self.keep_raw=keep_raw
         self.agg_race_cat=agg_race_cat
         self.race_cats=race_cats
         self.eth_cats=eth_cats
         self.gender_cats = gender_cats
         self.no_id = no_id
 
@@ -461,37 +487,41 @@
 
         return match_cols_out
 
 
     def _find_col_matches(self, id, match_substr, 
         known_col_names=None, 
         only_table_types=None,
+        required_table_types=[],
         exclude_table_types=[], 
         exclude_col_names=[], 
         secondary_patterns=[], 
         validator=None,
         always_validate=False,
         validate_args=[],
         std_col_name = None,
         search_data=False,
         word_replacements={},
         tables_to_exclude=[]):
 
+        if only_table_types is not None:  # Make sure that the tables can have this column include the tables that must have this column
+            only_table_types.extend(required_table_types)
+
         logger.info(f"Searching for {id} column")
         if self.table_type in exclude_table_types or \
             (only_table_types != None and self.table_type not in only_table_types) or \
             (self.source_name, self.table_type) in tables_to_exclude:
             if std_col_name in self.df.columns:
                 logger.info(f"\tSetting {id} column as {std_col_name}")
                 return [std_col_name]
             else:
                 logger.info(f"\tTable type {self.table_type} is excluded from tables to search for {id} column. Skipping...")
                 return []
 
-        officer_terms = ["officer","deputy", "empl"]
+        officer_terms = ["officer","deputy", "empl", 'personnel']
         if known_col_names != None and (not isinstance(known_col_names, list) or any([x is not None for x in known_col_names])):
             if isinstance(known_col_names,str):
                 known_col_names = [known_col_names]
             else:
                 known_col_names = [x for x in known_col_names if x is not None]
             for n in known_col_names:
                 if n not in self.df.columns:
@@ -573,15 +603,15 @@
                 multi_check = sum([any([y.lower() in x.lower() for y in officer_terms]) for x in match_cols])!=1
 
             if (len(match_cols)>0 and always_validate) or (multi_check and validator != None and len(match_cols) > 1):
                 logger.info(f"Testing data in column(s) {match_cols} as potential {id} column")
                 match_cols = validator(self.df, match_cols, *validate_args)
                 logger.info(f"Validated data in column(s) {match_cols} as potential {id} column")
 
-            if search_data and len(match_cols)==0:
+            if (search_data or self.table_type in required_table_types) and len(match_cols)==0:
                 logger.info(f"Testing data in all columns as potential {id} column")
                 match_cols = validator(self.df, self.df.columns, *validate_args)
                 logger.info(f"Validated data in column(s) {match_cols} as potential {id} column")
                 
             match_cols_out = self._remove_excluded(match_cols, exclude_col_names, match_substr)
             if match_cols_out!=match_cols:
                 logger.info(f"After applying rules {exclude_col_names}, potential {id} columns reduced from {match_cols} to {match_cols_out}")
@@ -709,15 +739,15 @@
         if self.table_type not in [defs.TableType.SHOOTINGS_INCIDENTS, defs.TableType.USE_OF_FORCE_INCIDENTS]:    
             def role_validator(df, match_cols_test):
                 match_cols = []
                 for col_name in match_cols_test:
                     try:
                         col = df[col_name]
                         # Function for validating a column indicates whether the person described is a civilian or officer
-                        new_col = convert.convert(convert.convert_off_or_civ, col)
+                        new_col = convert.convert(convert.convert_off_or_civ, col, no_id='error')
                         vals = new_col.unique()
 
                         if not any([isinstance(x,str) for x in vals]) or (defs._roles.SUBJECT not in vals and defs._roles.OFFICER not in vals):
                             continue
 
                         if defs._roles.SUBJECT not in vals or defs._roles.OFFICER not in vals:
                             # California data, RAE = Race and Ethnicity
@@ -743,15 +773,16 @@
                     except:
                         pass
 
                 return match_cols
 
             match_cols = self._find_col_matches("Is Person Officer or Subject", ["Civilian_Officer","ROLE"], 
                 known_col_names=self.known_cols[defs.columns.SUBJECT_OR_OFFICER],
-                only_table_types = [defs.TableType.USE_OF_FORCE, defs.TableType.USE_OF_FORCE_SUBJECTS_OFFICERS, defs.TableType.SHOOTINGS],
+                only_table_types = [defs.TableType.USE_OF_FORCE, defs.TableType.SHOOTINGS],
+                required_table_types=[defs.TableType.USE_OF_FORCE_SUBJECTS_OFFICERS, defs.TableType.COMPLAINTS_SUBJECTS_OFFICERS],
                 exclude_col_names=[("not equal","SubjectRole")],  # Subject role would be role of subject not whether person is subject or officer
                 validator=role_validator,
                 always_validate=True)
             if len(match_cols) > 1:
                 raise NotImplementedError(f"Multiple columns {match_cols} found for {defs.columns.SUBJECT_OR_OFFICER} column")
             elif len(match_cols) == 1:
                 logger.info(f"Column {match_cols[0]} identified as a {defs.columns.SUBJECT_OR_OFFICER} column")
@@ -850,15 +881,15 @@
                     ],
                 adv_type_match=_find_gender_col_type_advanced)
             
         injury_tables = [defs.TableType.USE_OF_FORCE, defs.TableType.USE_OF_FORCE_OFFICERS, defs.TableType.USE_OF_FORCE_SUBJECTS, 
                         defs.TableType.USE_OF_FORCE_SUBJECTS_OFFICERS, defs.TableType.SHOOTINGS, defs.TableType.SHOOTINGS_OFFICERS, 
                         defs.TableType.SHOOTINGS_SUBJECTS]
         
-        match_cols = self._find_col_matches("fatal", ['fatal','fatality','deceased','died'], 
+        match_cols = self._find_col_matches("fatal", ['fatal','fatality','deceased','died','death'], 
                                             exclude_col_names=[v for k,v in self.col_map.items() if "INJURY" in k],
                                             validator=_fatal_validator,
                                             only_table_types=injury_tables,
                                             tables_to_exclude=[("Los Angeles County",defs.TableType.SHOOTINGS_OFFICERS)],
                                             always_validate=True)
         
         self._id_demographic_column(match_cols,
@@ -888,14 +919,15 @@
             raise NotImplementedError()
         elif len(match_cols) == 1:
             logger.info(f"Column {match_cols[0]} identified as a {defs.columns.AGENCY} column")
             self.col_map[defs.columns.AGENCY] = match_cols[0]
 
         match_cols = self._find_col_matches("zip_code", ['zip','zipcode'],
                                             validator=_zip_code_validator,
+                                            validate_args=[self.state],
                                             always_validate=True)
         if len(match_cols) > 1:
             raise NotImplementedError()
         elif len(match_cols) == 1:
             logger.info(f"Column {match_cols[0]} identified as a {defs.columns.ZIP_CODE} column")
             self.col_map[defs.columns.ZIP_CODE] = match_cols[0]
 
@@ -937,14 +969,15 @@
             validation_types.append(defs.columns.RACE_OFFICER_SUBJECT)
             logger.info(f"Column {eth_cols[0]} associated with {eth_types[0]}")
         else:
             is_officer_table = self.table_type == defs.TableType.EMPLOYEE.value or \
                     ("- OFFICERS" in self.table_type and "SUBJECTS" not in self.table_type)
             for k in range(len(eth_cols)):
                 if "officer" in eth_cols[k].lower() or \
+                   "personnel" in eth_cols[k].lower() or \
                     "offcr" in eth_cols[k].lower() or is_officer_table or \
                     (self.source_name=="Orlando" and self.table_type==defs.TableType.SHOOTINGS and eth_cols[k]=="ethnicity"):
                     eth_types.append(defs.columns.ETHNICITY_OFFICER)
                     validation_types.append(defs.columns.RACE_OFFICER)
                 else:
                     eth_types.append(defs.columns.ETHNICITY_SUBJECT)
                     validation_types.append(defs.columns.RACE_SUBJECT)
@@ -1059,15 +1092,15 @@
             self.col_map[civ_officer_col_name] = col_names[0]
             return col_names, [civ_officer_col_name]
         else:     
             is_officer_table = self.table_type == defs.TableType.EMPLOYEE.value or \
                 ("- OFFICERS" in self.table_type and "SUBJECTS" not in self.table_type)
             is_subject_table = ("- SUBJECTS" in self.table_type and "OFFICERS" not in self.table_type)
             # mos = Member of Service
-            off_words = ["off", "deputy", "employee", "ofc", "empl", 'emp','mos']
+            off_words = ["off", "deputy", "employee", "ofc", "empl", 'emp','mos', 'personnel']
             civilian_terms = ["citizen","subject","suspect","civilian", "cit", "offender",]
             not_off_words = ["offender"]
 
             types = []
             possible_ambiguity = False
             for k in range(len(col_names)):
                 words = split_words(col_names[k],'lower')
@@ -1204,15 +1237,28 @@
             if len(set(types)) != len(types):
                 un_types = list(set(types))
                 new_types = []
                 new_col_names = []
                 for x in un_types:
                     type_cols = [y for t,y in zip(types, col_names) if t==x]
                     if len(type_cols)>1:
-                        warnings.warn(f"Multiple potential {x} columns ({type_cols}) found for {self.source_name} {self.table_type}. None will be standardized.")
+                        if sum(self.df[type_cols].notnull().any())==1:
+                            # Only 1 column isn't all nulls, use that
+                            new_types.append(x)
+                            m = self.df[type_cols].notnull().any()
+                            m = m[m].index[0]
+                            new_col_names.append(m)
+                            warnings.warn(f"Multiple potential {x} columns ({type_cols}) found for {self.source_name} {self.table_type}. {m} will be used because the rest are all null.")
+                        elif len(type_cols)==2 and (self.df[type_cols].isnull().sum(axis=1)>0).all():
+                            new_types.append(x)
+                            new_col_names.append(type_cols)
+                            warnings.warn(f"2 potential {x} columns ({type_cols}) found for {self.source_name} {self.table_type}. For each row, a value of 1 of the columns is always null. "+
+                                          "It appears that data was merged from multiple tables and the name of the column was change. These columns will be merged")
+                        else:
+                            warnings.warn(f"Multiple potential {x} columns ({type_cols}) found for {self.source_name} {self.table_type}. None will be standardized.")
                     else:
                         new_types.append(x)
                         new_col_names.append(type_cols[0])
                 types = new_types
                 col_names = new_col_names
 
             for k in range(len(col_names)):
@@ -1555,15 +1601,15 @@
                 mult_data.item_gender = gen_item
                 mult_data.item_age = age_item
                 # This is a column with all demographics that will be handled by standardize function
                 mult_data.type = MultType.DEMO_COL
                 return
             else:
                 cols = [self.col_map[x] for x in [age_col, race_col, eth_col, gender_col] if x in self.col_map]
-                if len(cols)<2:
+                if len(cols)<2 or any([isinstance(x, list) for x in cols]):
                     return
 
                 all_bad = self.df[cols].isnull().all()
                 cols = [x for x in cols if not all_bad[x]]
 
                 if len(cols)<2:
                     return
@@ -1857,15 +1903,15 @@
                     # Attempt to convert most values to numbers
                     col = pd.to_numeric(self.df[self.col_map[col_name]], errors="coerce", downcast="integer")
                     if pd.isnull(col).all():
                         logger.warn(f"Unable to convert column {self.col_map[col_name]} to an age")
                         self.col_map.pop(col_name)
                         return
 
-                    test = [int(x)==y if ((isinstance(x,Number) and pd.notnull(x)) or (type(x)==str and x.strip().isdigit())) 
+                    test = [int(float(x))==y if ((isinstance(x,Number) and pd.notnull(x)) or is_str_number(x)) 
                             else False for x,y in zip(self.df[self.col_map[col_name]],col)]
                     sum_test = sum(test)
                     if not check_column(self.col_map[col_name], "age") and  sum_test / len(test) < 0.2:
                         logger.warn(f"Not converting {self.col_map[col_name]} to an age. If this is an age column only {sum(test) / len(test)*100:.1f}% of the data has a valid value")
                         self.col_map.pop(col_name)
                         return
                     elif sum_test / len(test) < 0.85 and not (sum_test>1 and len(test)-sum_test==1):
@@ -1873,15 +1919,15 @@
                         if check_column(self.col_map[col_name], "age"):
                             # See if all values are null or acceptable values
                             badvals = 0                        
                             for x in self.df[self.col_map[col_name]].unique():
                                 x = x.lower().strip() if isinstance(x,str) else x
                                 if pd.isnull(x) or (isinstance(x,str) and x in ["na", "unknown"]):
                                     continue
-                                elif isinstance(x,Number) or  (isinstance(x,str) and x.isdigit()):
+                                elif isinstance(x,Number) or is_str_number(x):
                                     x = int(x)
                                     if x<0 or x>max_age:
                                         badvals+=1
                                 else:
                                     badvals+=1
 
                             if badvals<2 or badvals / len(self.df[self.col_map[col_name]].unique())<0.05 or \
@@ -1956,14 +2002,17 @@
         if check_column(col_name, "race"):
             match_cols.append(col_name)
             continue
         
         # Anything checked beyond this point is less likely to be a race column
         col = df[col_name]
         try:
+            if len(col.unique())>100:
+                # There shouldn't be this many race values
+                continue
             if "address" in col_name.lower() or \
                 (search_all and pd.api.types.is_numeric_dtype(col.dtype)):
                 # Addresses are complicated and could trigger false alarms
                 # Don't search numeric codes when searching all columns. Will lead to false matches
                 continue
 
             race_cats = defs.get_race_cats()
@@ -2009,15 +2058,15 @@
                         continue
             elif len(cols_test) > 5 and df[col_name].isin(["A","B"]).all():
                 # Most likely we are searching all columns in the table and this a column that uses
                 # letters to indicate something other than race
                 continue
 
             if col.apply(lambda x: isinstance(x,list)).mean() > 0.95 and \
-                col.apply(lambda x: any([isinstance(y,Number) or (isinstance(y,str) and y.isdigit()) for y in x]) 
+                col.apply(lambda x: any([isinstance(y,Number) or is_str_number(y) for y in x]) 
                           if isinstance(x,list) else False).mean() > 0.95:
                 # Date columns can result in lists that are mostly of numbers
                 continue
 
             match_cols.append(col_name)
         except Exception as e:
             pass
@@ -2141,42 +2190,49 @@
             col = convert.convert(convert._create_firearm_lut, df[col_name], no_id='error')
             match_cols.append(col_name)
         except:
             pass
 
     return match_cols
 
-def _zip_code_validator(df, cols_test):
+def _zip_code_validator(df, cols_test, state):
     match_cols = []
     for col_name in cols_test:
         try:
-            possible_zips = df[col_name].apply(lambda x: isinstance(x, Number) or (isinstance(x,str) and x.isdigit()) and \
-                                               pd.notnull(x) and int(x)>=1e4 and int(x)<1e5)
-            if possible_zips.mean()>0.5:
+            min_zip = 1e3 if state=='Vermont' else 1e4
+            possible_zips = df[col_name].apply(lambda x: (isinstance(x, Number) or is_str_number(x)) and \
+                                               pd.notnull(x) and int(x)>=min_zip and int(x)<1e5)
+            if (m:=possible_zips.mean())>0.5 or \
+                (m>=0.1 and m+df[col_name].apply(lambda x: pd.isnull(x) or (isinstance(x,str) and x.strip().upper() in ['','UNKNOWN'])).mean()>=0.99):
                 match_cols.append(col_name)
             elif (df[col_name]=='UNKNOWN').any() and \
                 len(m:=df[col_name][df[col_name]!='UNKNOWN'])/len(df)>0.3 and \
-                m.apply(lambda x: isinstance(x, Number) or (isinstance(x,str) and x.isdigit()) and \
+                m.apply(lambda x: (isinstance(x, Number) or is_str_number(x)) and \
                                                pd.notnull(x) and int(x)>=1e4 and int(x)<1e5).mean()==1:
                 match_cols.append(col_name)
             else:
                 raise ValueError("Column is not recognized as a zip code column")
         except:
             pass
 
     return match_cols
 
 def cleanup_column(df, col_name, keep_raw):
     if keep_raw:
-        if not col_name.startswith(_OLD_COLUMN_INDICATOR):
-            new_name = _OLD_COLUMN_INDICATOR+"_"+col_name
-            logger.info(f"Renaming raw column {col_name} to {new_name}")
-            df.rename(columns={col_name : new_name}, inplace=True)
-        else:
-            new_name = col_name
+        col_names = col_name if isinstance(col_name, list) else [col_name]
+        new_names = []
+        for col_name in col_names:
+            if not col_name.startswith(_OLD_COLUMN_INDICATOR):
+                new_name = _OLD_COLUMN_INDICATOR+"_"+col_name
+                logger.info(f"Renaming raw column {col_name} to {new_name}")
+                df.rename(columns={col_name : new_name}, inplace=True)
+                new_names.append(new_name)
+            else:
+                new_names.append(col_name)
+        new_name = new_names[0] if len(new_names)==1 else new_names
         return new_name
     else:
         logger.info(f"Removing raw column {col_name}")
         df.drop(col_name, axis=1, inplace=True)
         return None
     
 def california_ori2agency(col, year, unknown='ignore'):
```

### Comparing `openpolicedata-0.6/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.7/openpolicedata.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.6
-Summary: The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints.
+Version: 0.7
+Summary: The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints.
 Author-email: Matt Sowd <openpolicedata@gmail.com>, Paul Otto <potto@ieee.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, sowdm
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -58,86 +58,78 @@
 Requires-Dist: sodapy
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Requires-Dist: xlrd
 Provides-Extra: optional
 Requires-Dist: rapidfuzz; extra == "optional"
 Requires-Dist: msoffcrypto-tool; extra == "optional"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
+The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints. 
 
-Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
+Users request data by department name and type of data, and the data is returned as a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html). There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.). When data is loaded by OPD, the returned data is unmodified (with the exception of formatting known date fields) from what appears on the source's site, and OPD provides links to the original data for transparency.
 
 OpenPoliceData can be installed from the Python Package Index (PyPI):
 ```
 pip install openpolicedata
 ``` 
 
 OpenPoliceData provides access to police data with 2 simple lines of code:
 ```
 > import openpolicedata as opd
 > src = opd.Source("New Orleans")
 > data = src.load(table_type="USE OF FORCE", year=2022)
 ```
 
-> **NEW IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
+> **NEW STARTING IN VERSION 0.6**: OPD now provides tools for automated data standardization. Applying these tools allow you to start your analysis more quickly by replacing column names and data with standard values for some common column types. [Learn how it works and how to use it here.](https://openpolicedata.readthedocs.io/en/stable/getting_started/index.html#Data-Standardization)
 
 - Documentation: https://openpolicedata.readthedocs.io/
 - Source Code: https://github.com/openpolicedata/openpolicedata
 - Bug Tracker: https://github.com/openpolicedata/openpolicedata/issues
 - [Latest Datasets](#latest-datasets-added)
 - [Release Notes](#release-notes-for-version-057-2023-09-05)
 - [Contributing](#contributing)
 
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 ## Latest Datasets Added to OPD
-- Chicago, IL: Traffic Citations
-- Traffic Citations for agencies across New York State
-- Buffalo Crashes and Incidents
-- Massachusetts (All Agencies): Employee and Disciplinary Records data
-- Alameda County, CA: Incidents
-- Marin County, CA: Incidents
-- Riverside, CA: Incidents
-- Albany, NY: Arrests, Calls for Service, Field Contacts, Incidents, Traffic Citations, and Use of Force
-- Chicago, IL: Pedestrian Stops
-- New York City, NY: 2022 Pedestrian Stops
-- Oakland, CA: 2022 Use of Force
-- San Diego, CA: 2022 Complaints
-- Tacoma, WA: Calls for Service, Complaints, Incidents, and Officer-Involved Shootings
+- Asheville, NC arrests, citations, complaints, incidents, pointing weapon, traffic stops, use of force, and 2023 calls for service
+- Sacramento, CA 2024 calls for service, 2021-2024 incidents, and 2023-2024 citations   
+- Albemarle County, VA: Stops
+- Norman, OK: Crashes, incidents, and traffic stops data (new) and most recent arrests, complaints and use of force data
+- Oakland, CA: Stops
+- Washington D.C.: Lawsuits against MPD
+- Bloomington, IN: Use of Force and Citations
+- Wallkill, NY: Employee and Stops
+- Bremerton, WA: Arrests, Citations, and Incidents
+- Phoenix, AZ: Officers Firearm Pointing
+- Phoenix, AZ: 2024 Calls for Service 
+- Boston, MA: Deathes in Custody
+- San Jose, CA: 2024 Calls for Service
+- Portland, OR: 2024 Calls for Service
+- Santa Monica, CA: 2022-2023 Incidents
 
-## Release Notes for Version 0.6 - 2024-02-10
+## v0.6 - 2024-05-10
 ### Added
-- Data standardization: Added function for standardizing some column names and data values
-- Added reload function to datasets module to allow reloading the datasets table (in case of an update) or loading a datasets table from a custom location
-- Added functions for getting race, gender, and age columns after standardization
-- Added merge function for merging 2 table together
-- Added function for finding related tables
-- Added a function for expanding rows that contain information on multiple officers or subjects into multiple row
-- Made opd.defs.TableType and opd.defs.columns available as opd.TableType and opd.Column
-- Added Table.urls to enable quick retrieval of URLs associated with a dataset
-- Added verbose mode to enable transparency when loading data with get_count, load_data_from_url, and load_from_url_gen
-- Added Source.load_iter to be used instead of Source.load_from_url_gen
-- Added Source.load to be used instead of Source.load_from_url
-- Added data loader for CKAN API
+- Added POINTING WEAPON (by officer) table type
+- Added data loader to combine multiple files that span a single year into a single dataset
+- Added support for more text date column formats in Arcgis loader.
+- Added url_contains input to get_count, load_iter, load, and load_from_csv of Source class to distinguish between multiple datasets matching a data request
+- Added datasets input to get_years to allow getting the years in specific datasets.
+- Added [Year Filter Guide](https://openpolicedata.readthedocs.io/en/stable/getting_started/year_filtering.html) to documentation
 ### Changed
-- Inputs to Source.get_count is now (table_type, year, ...) instead of (year, table_type, ...) so inputs go from general to specific. Original input order is deprecated and will be removed in Version 1.0.
-### Deprecated
-- Deprecated Source.load_from_url_gen. Will be removed in Version 1.0
-- Deprecated Source.load_from_url. Will be removed in Version 1.0
-### Removed
-- Removed support for Python 3.7 which has reached end of life: https://www.python.org/downloads/release/python-370/
+- Updates to standardization to handle more datasets
 ### Fixed
-- Improved speed and feedback when reading large CSV files contained in zip files
-- Source.get_agencies with a partial_name is now case-insensitive
+- Fixed year filtering for Tucson OFFICER-INVOLVED SHOOTINGS - INCIDENTS dataset. Datasets is no longer available using OpenPoliceData prior to Version 0.7.
 
 Complete change log available at: https://github.com/openpolicedata/openpolicedata/blob/main/CHANGELOG.md
 
 ## Contributing
-All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](openpolicedata@gmail.com).
+All contributions are welcome including code enhancments, bug fixes, bug reports, documentation updates, and locating new datasets. If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD) or reach out by [email](mailto:openpolicedata@gmail.com).
```

### Comparing `openpolicedata-0.6/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.7/openpolicedata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -24,13 +24,15 @@
 openpolicedata/deprecated/_decorators.py
 openpolicedata/deprecated/_pandas.py
 openpolicedata/deprecated/datasetsCompat.py
 openpolicedata/deprecated/messages.py
 openpolicedata/deprecated/source_table_compat.py
 tests/test_data_loaders.py
 tests/test_datasets.py
+tests/test_datasets_fixture.py
 tests/test_defs.py
 tests/test_deprecated.py
 tests/test_opd_data1.py
 tests/test_opd_data2.py
 tests/test_opd_data3.py
-tests/test_preproc.py
+tests/test_preproc.py
+tests/test_utils.py
```

### Comparing `openpolicedata-0.6/pyproject.toml` & `openpolicedata-0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "openpolicedata"
 dynamic = ["version"]
 authors = [
   { name="Matt Sowd", email="openpolicedata@gmail.com" },
   { name="Paul Otto", email="potto@ieee.org" },
 ]
-description = "The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 395+ incident-level datasets for about 4800 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints."
+description = "The OpenPoliceData (OPD) Python library is the most comprehensive centralized public access point for incident-level police data in the United States. OPD provides easy access to 425+ incident-level datasets for about 4850 police agencies. Types of data include traffic stops, use of force, officer-involved shootings, and complaints."
 readme = "README.md"
 license = {file = 'LICENSE'}
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Science/Research',
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
@@ -54,14 +54,15 @@
 homepage = "https://openpolicedata.readthedocs.io/"
 documentation = "https://openpolicedata.readthedocs.io/en/stable/documentation.html"
 repository = "https://github.com/openpolicedata/openpolicedata"
 tracker = "https://github.com/openpolicedata/openpolicedata/issues"
 
 [project.optional-dependencies]
 optional = ['rapidfuzz', 'msoffcrypto-tool']
+geopandas = ['geopandas']
 test = ['pytest']
 
 [tool.setuptools.dynamic]
 version = {file = ".\\openpolicedata\\_version.txt"}
 # version = {attr = "openpolicedata.__version__"}
 
 # I think this is true by default...
@@ -73,10 +74,12 @@
 namespaces = false
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:datetime.datetime.utcfromtimestamp():DeprecationWarning:tqdm:",
     "ignore:datetime.datetime:DeprecationWarning:.*openpyxl:",
     "ignore:datetime.datetime.utcfromtimestamp():DeprecationWarning:.*tz:",
+    "ignore:Passing a SingleBlockManager to Series.*:DeprecationWarning:geopandas:",
     # "ignore:distutils Version classes are deprecated. Use packaging.version instead.*:DeprecationWarning::",
     # "ignore:An exception was ignored while fetching the attribute `__array_interface__` from an object of type 'Polygon'*:DeprecationWarning:geopandas.*:"
-]
+]
+addopts = "--csvfile='..\\opd-data\\opd_source_table.csv' --runslow --skip 'Sacramento,Beloit' -s"
```

### Comparing `openpolicedata-0.6/tests/test_data_loaders.py` & `openpolicedata-0.7/tests/test_data_loaders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from io import BytesIO
 import pytest
+import re
 import requests
 if __name__ == "__main__":
 	import sys
 	sys.path.append('../openpolicedata')
 from openpolicedata import data_loaders
 import pandas as pd
 try:
@@ -11,616 +12,715 @@
     _has_gpd = True
 except:
     _has_gpd = False
 
 import warnings
 warnings.filterwarnings(action='ignore', module='arcgis')
 
-class TestProduct:
-    def test_process_date_input_empty(self, csvfile, source, last, skip, loghtml):
-        with pytest.raises(ValueError):
-            data_loaders._process_date([])
-        
-    def test_process_date_too_many(self, csvfile, source, last, skip, loghtml):
-        year = [2021, 2022, 2023]
-        with pytest.raises(ValueError):
-            data_loaders._process_date(year)
-
-    def test_process_dates_year_input_wrong_order(self, csvfile, source, last, skip, loghtml):
-        year = [2023, 2021]
-        with pytest.raises(ValueError):
-            data_loaders._process_date(year)
-
-    def test_ckan(self, csvfile, source, last, skip, loghtml):
-        lim = data_loaders._default_limit
-        data_loaders._default_limit = 500
-        url = "https://data.virginia.gov"
-        dataset = "60506bbb-685f-4360-8a8c-30e137ce3615"
-        date_field = "STOP_DATE"
-        agency_field = 'AGENCY NAME'
-        loader = data_loaders.Ckan(url, dataset, date_field)
-
-        assert not loader.isfile()
-
-        count = loader.get_count()
-
-        r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"')
-        r.raise_for_status()
-        assert count==r.json()['result']['records'][0]['count']>0
-
-        year = 2022
-        count = loader.get_count(year=year)
-
-        r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"' + 
-                         f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01'""")
-        r.raise_for_status()
-        assert count==r.json()['result']['records'][0]['count']>0
-
-        agency='William and Mary Police Department'
-        opt_filter = {'=':{agency_field:agency}}
-        opt_filter = 'LOWER("' + agency_field + '")' + " = '" + agency.lower() + "'"
-        count = loader.get_count(year=year, opt_filter=opt_filter)
-
-        r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"' + 
-                         f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01' AND """+
-                         opt_filter)
-        r.raise_for_status()
-        assert count==r.json()['result']['records'][0]['count']>0
+def test_process_date_input_empty():
+    with pytest.raises(ValueError):
+        data_loaders._process_date([])
+    
+def test_process_date_too_many():
+    year = [2021, 2022, 2023]
+    with pytest.raises(ValueError):
+        data_loaders._process_date(year)
+
+def test_process_dates_year_input_wrong_order():
+    year = [2023, 2021]
+    with pytest.raises(ValueError):
+        data_loaders._process_date(year)
+
+@pytest.mark.parametrize("url, dataset", [
+    ("https://wallkillpd.org/document-center/data/vehicle-a-pedestrian-stops/2016-vehicle-a-pedestrian-stops", 
+        "147-2016-2nd-quarter-vehicle-a-pedestrian-stops/file.html; 148-2016-3rd-quarter-vehicle-a-pedestrian-stops/file.html; 167-2016-4th-quarter-vehicle-pedestrian-stops/file.html"), 
+    ("http://www.bremertonwa.gov/DocumentCenter/View", 
+        "*arrest*| 4713/January-2017-XLSX; 4873/February-2017-XLSX; 4872/March-2017-XLSX; https://raw.githubusercontent.com/openpolicedata/opd-datasets/main/data/Washington_Bremerton_ARRESTS_April_2017.csv; 5026/May-2017-XLSX; 5153/June-2017-XLSX; 5440/July-2017-XLSX; 5441/August-2017-XLSX; 5477/September-2017-XLSX; 5548/October-2017-XLSX; 5608/November-2017-XLSX; 5607/December-2017-XLSX"),
+    ("https://mpdc.dc.gov/sites/default/files/dc/sites/mpdc/publication/attachments", 
+        'Open YTD & Closed YTD; New Lawsuits & Closed Lawsuits & New Claims & Closed Claims| New%20and%20Closed%20Lawsuits%20CY%202023%20as%20of%207.20.2023.xlsx; New%20and%20Closed%20Lawsuits%20and%20Claims%202023%20July-December%20External.xlsx')
+    ]
+    )
+def test_combined(url, dataset):
+    loader = data_loaders.CombinedDataset(data_loaders.Excel, url, dataset)
+
+    assert loader.isfile()
+
+    sheets = None
+    if '|' in dataset:
+        dataset = dataset.split('|')
+        assert len(dataset)==2
+        sheets = dataset[0].split(';')
+        dataset = dataset[1]
+
+    dfs = []
+    for k,ds in enumerate(dataset.split(';')):
+        ds = ds.strip()
+        headers = {'User-agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'}
+        for s in sheets[min(k,len(sheets)-1)].split('&') if sheets else [0]:
+            if ds.endswith('.csv'):
+                df = pd.read_csv(ds)
+            else:
+                r = requests.get(url + '/' + ds, stream=True, headers=headers)
+                r.raise_for_status()
+                file_like = BytesIO(r.content)
+                if isinstance(s,str):
+                    s = s.strip()
+                    if '*' in s:
+                        all_sheets = pd.ExcelFile(file_like).sheet_names
+                        p = s.replace('*','.*')
+                        s = [x for x in all_sheets if re.search(p,x)]
+                        assert len(s)==1
+                        s = s[0]
+                df = pd.read_excel(file_like, sheet_name=s)
+            cols = [x for x in df.columns if not x.startswith('Unnamed')]
+            df = df[cols]
+            dfs.append(df)
+    df_true = pd.concat(dfs, ignore_index=True).convert_dtypes()
+
+    count = loader.get_count(force=True)
+
+    assert len(df_true) == count
+
+    df = loader.load().convert_dtypes()
+    pd.testing.assert_frame_equal(df, df_true)
+
+    offset = 3000
+    nrows = 20
+    df = loader.load(offset=offset).convert_dtypes()
+    pd.testing.assert_frame_equal(df, df_true.iloc[offset:].convert_dtypes())
 
-        loader._last_count = None
-        df = loader.load(year=year, pbar=False, opt_filter=opt_filter)
+    df = loader.load(nrows=nrows).convert_dtypes()
+    pd.testing.assert_frame_equal(df, df_true.head(nrows).convert_dtypes())
 
-        assert len(df)==count
+    df = loader.load(offset=offset, nrows=nrows).convert_dtypes()
+    pd.testing.assert_frame_equal(df, df_true.iloc[offset:].head(nrows).convert_dtypes())
+    
 
-        offset = 1
-        nrows = count - 2
-        df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False, opt_filter=opt_filter)
+def test_ckan():
+    lim = data_loaders._default_limit
+    data_loaders._default_limit = 500
+    url = "https://data.virginia.gov"
+    dataset = "60506bbb-685f-4360-8a8c-30e137ce3615"
+    date_field = "STOP_DATE"
+    agency_field = 'AGENCY NAME'
+    loader = data_loaders.Ckan(url, dataset, date_field)
+
+    assert not loader.isfile()
+
+    count = loader.get_count()
+
+    r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"')
+    r.raise_for_status()
+    assert count==r.json()['result']['records'][0]['count']>0
+
+    year = 2022
+    count = loader.get_count(year=year)
+
+    r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"' + 
+                        f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01'""")
+    r.raise_for_status()
+    assert count==r.json()['result']['records'][0]['count']>0
+
+    agency='William and Mary Police Department'
+    opt_filter = {'=':{agency_field:agency}}
+    opt_filter = 'LOWER("' + agency_field + '")' + " = '" + agency.lower() + "'"
+    count = loader.get_count(year=year, opt_filter=opt_filter)
+
+    r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT COUNT(*) FROM "{dataset}"' + 
+                        f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01' AND """+
+                        opt_filter)
+    r.raise_for_status()
+    assert count==r.json()['result']['records'][0]['count']>0
+
+    loader._last_count = None
+    df = loader.load(year=year, pbar=False, opt_filter=opt_filter)
+
+    assert len(df)==count
+
+    offset = 1
+    nrows = count - 2
+    df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False, opt_filter=opt_filter)
+
+    assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
+
+    df_offset = loader.load(year=year, offset=1, pbar=False, opt_filter=opt_filter)
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+
+    r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT * FROM "{dataset}"' + 
+                        f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01' AND """+
+                        opt_filter + " ORDER BY _id")
+    df_comp= pd.DataFrame(r.json()['result']['records'])
+    df_comp[date_field] = pd.to_datetime(df_comp[date_field])
+    df_comp = df_comp.drop(columns=['_id','_full_text'])
+    
+    assert df.equals(df_comp)
 
-        assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
+    data_loaders._default_limit = lim
 
-        df_offset = loader.load(year=year, offset=1, pbar=False, opt_filter=opt_filter)
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
-        r = requests.get(f'https://data.virginia.gov/api/3/action/datastore_search_sql?sql=SELECT * FROM "{dataset}"' + 
-                         f""" WHERE "{date_field}" >= '{year}-01-01' AND "{date_field}" < '{year+1}-01-01' AND """+
-                         opt_filter + " ORDER BY _id")
-        df_comp= pd.DataFrame(r.json()['result']['records'])
-        df_comp[date_field] = pd.to_datetime(df_comp[date_field])
-        df_comp = df_comp.drop(columns=['_id','_full_text'])
-        
-        assert df.equals(df_comp)
+def test_carto():
+    lim = data_loaders._default_limit
+    data_loaders._default_limit = 500
+    url = "phl"
+    dataset = "shootings"
+    date_field = "date_"
+    loader = data_loaders.Carto(url, dataset, date_field)
 
-        data_loaders._default_limit = lim
+    assert not loader.isfile()
 
-    
-    def test_carto(self, csvfile, source, last, skip, loghtml):
-        lim = data_loaders._default_limit
-        data_loaders._default_limit = 500
-        url = "phl"
-        dataset = "shootings"
-        date_field = "date_"
-        loader = data_loaders.Carto(url, dataset, date_field)
+    count = loader.get_count()
 
-        assert not loader.isfile()
+    r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset}")
+    r.raise_for_status()
+    assert count==r.json()["rows"][0]["count"]>0
 
-        count = loader.get_count()
+    year = 2019
+    count = loader.get_count(year=year)
 
-        r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset}")
-        r.raise_for_status()
-        assert count==r.json()["rows"][0]["count"]>0
+    r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
+    r.raise_for_status()
+    assert count==r.json()["rows"][0]["count"]>0
 
-        year = 2019
-        count = loader.get_count(year=year)
+    df = loader.load(year=year, pbar=False)
 
-        r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
-        r.raise_for_status()
-        assert count==r.json()["rows"][0]["count"]>0
+    assert len(df)==count
 
-        df = loader.load(year=year, pbar=False)
+    offset = 1
+    nrows = count - 2
+    df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False)
 
-        assert len(df)==count
+    assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 
-        offset = 1
-        nrows = count - 2
-        df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False)
+    df_offset = loader.load(year=year, offset=1, pbar=False)
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
-        assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
+    r = requests.get(f"https://phl.carto.com/api/v2/sql?format=GeoJSON&q=SELECT * FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
+    features = r.json()["features"]
+    df_comp= pd.DataFrame.from_records([x["properties"] for x in features])
+    df_comp[date_field] = pd.to_datetime(df_comp[date_field])
+    
+    try:
+        import geopandas as gpd
+        from shapely.geometry import Point
+        geometry = []
+        for feat in features:
+            if "geometry" not in feat or feat["geometry"]==None or len(feat["geometry"]["coordinates"])<2:
+                geometry.append(None)
+            else:
+                geometry.append(Point(feat["geometry"]["coordinates"][0], feat["geometry"]["coordinates"][1]))
 
-        df_offset = loader.load(year=year, offset=1, pbar=False)
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+        df_comp = gpd.GeoDataFrame(df_comp, crs=4326, geometry=geometry)
+    except:
+        geometry = [feat["geometry"] if "geometry" in feat else None for feat in features]
+        df_comp["geolocation"] = geometry
+
+    assert df.equals(df_comp)
+
+    data_loaders._default_limit = lim
+
+    if data_loaders._has_gpd:
+        assert type(df) == gpd.GeoDataFrame
+        data_loaders._has_gpd = False
+        df = loader.load(year=year, nrows=nrows, pbar=False)
+        data_loaders._has_gpd = True
+        assert isinstance(df, pd.DataFrame)
+
+    url2 = "https://phl.carto.com/api/v2/sql?"
+    loader2 = data_loaders.Carto(url2, dataset, date_field)
+    assert loader.url==loader2.url
+
+def test_arcgis():
+    lim = data_loaders._default_limit
+    data_loaders._default_limit = 500
+    data_loaders._verify_arcgis = True
+    url = "https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/16"
+    gis = data_loaders.Arcgis(url)
+    assert not gis.isfile()
+    try:
+        # Check if arcgis is installed
+        from arcgis.features import FeatureLayerCollection
+        # Verify that verify is True by getting active layer 
+        _ = gis._Arcgis__active_layer
+        # Load with verification
+        gis.load()
+        gis.get_count()
+    except:
+        pass
+
+    data_loaders._verify_arcgis = False
+
+    # Now load without verification as user would
+    gis = data_loaders.Arcgis(url)
+    # Confirm that verfication is not set
+    with pytest.raises(AttributeError):
+        gis._Arcgis__active_layer
+    df = gis.load()
+    count = gis.get_count()
+
+    assert len(df)==count
+
+    offset = 1
+    nrows = count-offset
+    df_offset = gis.load(nrows=nrows, offset=offset)
+    assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 
-        r = requests.get(f"https://phl.carto.com/api/v2/sql?format=GeoJSON&q=SELECT * FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
-        features = r.json()["features"]
-        df_comp= pd.DataFrame.from_records([x["properties"] for x in features])
-        df_comp[date_field] = pd.to_datetime(df_comp[date_field])
-        
-        try:
-            import geopandas as gpd
-            from shapely.geometry import Point
-            geometry = []
-            for feat in features:
-                if "geometry" not in feat or feat["geometry"]==None or len(feat["geometry"]["coordinates"])<2:
-                    geometry.append(None)
-                else:
-                    geometry.append(Point(feat["geometry"]["coordinates"][0], feat["geometry"]["coordinates"][1]))
-
-            df_comp = gpd.GeoDataFrame(df_comp, crs=4326, geometry=geometry)
-        except:
-            geometry = [feat["geometry"] if "geometry" in feat else None for feat in features]
-            df_comp["geolocation"] = geometry
-
-        assert df.equals(df_comp)
-
-        data_loaders._default_limit = lim
-
-        if data_loaders._has_gpd:
-            assert type(df) == gpd.GeoDataFrame
-            data_loaders._has_gpd = False
-            df = loader.load(year=year, nrows=nrows, pbar=False)
-            data_loaders._has_gpd = True
-            assert isinstance(df, pd.DataFrame)
-
-        url2 = "https://phl.carto.com/api/v2/sql?"
-        loader2 = data_loaders.Carto(url2, dataset, date_field)
-        assert loader.url==loader2.url
-
-    def test_arcgis(self, csvfile, source, last, skip, loghtml):
-        lim = data_loaders._default_limit
-        data_loaders._default_limit = 500
-        data_loaders._verify_arcgis = True
-        url = "https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/16"
-        gis = data_loaders.Arcgis(url)
-        assert not gis.isfile()
-        try:
-            # Check if arcgis is installed
-            from arcgis.features import FeatureLayerCollection
-            # Verify that verify is True by getting active layer 
-            _ = gis._Arcgis__active_layer
-            # Load with verification
-            gis.load()
-            gis.get_count()
-        except:
-            pass
-
-        data_loaders._verify_arcgis = False
-
-        # Now load without verification as user would
-        gis = data_loaders.Arcgis(url)
-        # Confirm that verfication is not set
-        with pytest.raises(AttributeError):
-            gis._Arcgis__active_layer
-        df = gis.load()
-        count = gis.get_count()
-
-        assert len(df)==count
-
-        offset = 1
-        nrows = count-offset
-        df_offset = gis.load(nrows=nrows, offset=offset)
-        assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
+    df_offset = gis.load(offset=offset)
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+    
+    data_loaders._default_limit = lim
 
-        df_offset = gis.load(offset=offset)
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
-        
-        data_loaders._default_limit = lim
+    try:
+        from arcgis.features import FeatureLayerCollection
+        last_slash = url.rindex("/")
+        layer_num = url[last_slash+1:]
+        base_url = url[:last_slash]
+        layer_collection = FeatureLayerCollection(base_url)
+
+        is_table = True
+        active_layer = None
+        for layer in layer_collection.layers:
+            layer_url = layer.url
+            if layer_url[-1] == "/":
+                layer_url = layer_url[:-1]
+            if layer_num == layer_url[last_slash+1:]:
+                active_layer = layer
+                is_table = False
+                break
 
-        try:
-            from arcgis.features import FeatureLayerCollection
-            last_slash = url.rindex("/")
-            layer_num = url[last_slash+1:]
-            base_url = url[:last_slash]
-            layer_collection = FeatureLayerCollection(base_url)
-
-            is_table = True
-            active_layer = None
-            for layer in layer_collection.layers:
+        if is_table:
+            for layer in layer_collection.tables:
                 layer_url = layer.url
                 if layer_url[-1] == "/":
                     layer_url = layer_url[:-1]
                 if layer_num == layer_url[last_slash+1:]:
                     active_layer = layer
-                    is_table = False
                     break
 
-            if is_table:
-                for layer in layer_collection.tables:
-                    layer_url = layer.url
-                    if layer_url[-1] == "/":
-                        layer_url = layer_url[:-1]
-                    if layer_num == layer_url[last_slash+1:]:
-                        active_layer = layer
-                        break
-
-            layer_query_result = active_layer.query(as_df=True)
-        except:
-            url += "/query"
-            params = {}
-            params["where"] = "1=1"
-            params["outFields"] = "*"
-            params["f"] = "json"
+        layer_query_result = active_layer.query(as_df=True)
+    except:
+        url += "/query"
+        params = {}
+        params["where"] = "1=1"
+        params["outFields"] = "*"
+        params["f"] = "json"
 
-            r = requests.get(url, params=params)
-            r.raise_for_status()
+        r = requests.get(url, params=params)
+        r.raise_for_status()
 
-            features = r.json()["features"]
-            params["resultOffset"] = len(features)
-            r = requests.get(url, params=params)
-            r.raise_for_status()
+        features = r.json()["features"]
+        params["resultOffset"] = len(features)
+        r = requests.get(url, params=params)
+        r.raise_for_status()
 
-            features.extend(r.json()["features"])
-            
-            layer_query_result = pd.DataFrame.from_records([x["attributes"] for x in features])
+        features.extend(r.json()["features"])
+        
+        layer_query_result = pd.DataFrame.from_records([x["attributes"] for x in features])
 
-        assert set(df.columns) == set(layer_query_result.columns)
-        assert len(layer_query_result) == count
-        df = df[layer_query_result.columns]
+    assert set(df.columns) == set(layer_query_result.columns)
+    assert len(layer_query_result) == count
+    df = df[layer_query_result.columns]
+
+    assert layer_query_result.equals(df)
+
+# Including all text date datasets for now. May want to include only unique date formats in the future
+@pytest.mark.parametrize('url, year, date_field',[
+    ('https://gis.ashevillenc.gov/server/rest/services/PublicSafety/APDCitations/MapServer/10', 2023, 'citation_date'), # YYYY-MM-DD
+    ('https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/5', None, 'OCCURRED_DT'),# YYYY-MM-DD
+    ('https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/6', None, 'OCCURRED_DT'),# YYYY-MM-DD
+    ('https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/7', 2023, 'OCCURRED_DT'),# YYYY-MM-DD
+    ('https://services.arcgis.com/aJ16ENn1AaqdFlqx/arcgis/rest/services/APDComplaints/FeatureServer/0', None, 'occurred_date'),  # M/D/YYYY
+    ('https://services1.arcgis.com/79kfd2K6fskCAkyg/arcgis/rest/services/LMPD_STOPS_DATA_(2)/FeatureServer/0', 2020, 'ACTIVITY_DATE'),
+    ('https://gis.ashevillenc.gov/server/rest/services/PublicSafety/APDIncidents/MapServer/3', 2023, 'date_occurred'),   # YYYYMMDD
+    ('https://services.arcgis.com/aJ16ENn1AaqdFlqx/arcgis/rest/services/APD_ShowOfForce/FeatureServer/0', None, 'occ_date'),   # YYYYMMDD
+    ("https://services.arcgis.com/aJ16ENn1AaqdFlqx/arcgis/rest/services/APDTrafficStops2020/FeatureServer/0", 2023, 'date_occurred'),    # YYYYMMDDHHMMSS
+    ('https://services.arcgis.com/aJ16ENn1AaqdFlqx/arcgis/rest/services/APD_UseOfForce2021/FeatureServer/0', 2022, 'occurred_date'),  # YYYYMMDD.0
+    ('https://services.arcgis.com/aJ16ENn1AaqdFlqx/arcgis/rest/services/APDUseOfForce/FeatureServer/0', None, 'date_occurred'), # MONTH, D, YYYY
+    ('https://publicgis.tucsonaz.gov/open/rest/services/OpenData/OpenData_PublicSafety/MapServer/34/', None, 'INCI_DATE'),  # YYYY-MM-DDTHH:MM:SS.SSSZ
+    ('https://gis.charlottenc.gov/arcgis/rest/services/ODP/CMPD_Calls_for_Service/MapServer/0', 2022, 'CALENDAR_YEAR'),  # YYYY
+    ('https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/11', None, 'YEAR_MONTH'),      # YYYY-MM
+    ("https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/14", 2020, 'Month_of_Stop'),
+    ('https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/13', None, 'YR'),   # Numeric year
+])
+def test_arcgis_text_date(url, year, date_field):
+    loader = data_loaders.Arcgis(url, date_field=date_field)
+    data = loader.load(year, pbar=False)
+    
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message='Could not infer format.*')
+        if isinstance(data[date_field].iloc[0],str) and data[date_field].iloc[0][-2:]=='.0': # Date is recorded as float
+            dts = data[date_field].apply(lambda x: x[:-2] if isinstance(x,str) else None)
+            dts = pd.to_datetime(dts, errors='coerce')
+        else:
+            dts = pd.to_datetime(data[date_field], errors='coerce', utc=True)
+        if year:
+            assert (dts.dt.year==year).all()
+
+    un_months = dts.dt.month.unique()
+    if len(un_months)==1 and un_months==[1] and (date_field.lower()=='yr' or 'year' in date_field.lower()):
+        pass
+    else:
+        assert all([x in un_months for x in range(1,13)])
+
+# No datasets currently trigger usage of the legacy server code
+# def test_arcgis_legacy_server():
+#     url = "https://egis.baltimorecity.gov/egis/rest/services/GeoSpatialized_Tables/Arrest/FeatureServer/0/" 
+
+#     gis = data_loaders.Arcgis(url)
+#     gis.load(nrows=1)
+
+#     url = "https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/5/" 
+#     gis = data_loaders.Arcgis(url)
+#     gis.load(nrows=1)
+
+
+def test_arcgis_geopandas():
+    if _has_gpd:
+        url = "https://services1.arcgis.com/zdB7qR0BtYrg0Xpl/arcgis/rest/services/ODC_CRIME_STOPS_P/FeatureServer/32/"
+        date_field = "TIME_PHONEPICKUP"
+        year_filter = 2020
+        nrows = 1000
+        df = data_loaders.Arcgis(url, date_field=date_field).load(year=year_filter, nrows=nrows)
 
-        assert layer_query_result.equals(df)
+        assert type(df) == gpd.GeoDataFrame
+    else:
+        pass
+
+def test_arcgis_pandas():
+    data_loaders._use_gpd_force = False
+    url = "https://services1.arcgis.com/wpJGOi6N4Rq5cqFv/arcgis/rest/services/Pursuits_2020_2021/FeatureServer/0/"
+    date_field = "DATE"
+    year_filter = 2020
+    gis = data_loaders.Arcgis(url, date_field=date_field)
+    df = gis.load(year=year_filter)
+    count = gis.get_count(year=year_filter)
+    # Reset
+    data_loaders._use_gpd_force = None
+
+    assert type(df) == pd.DataFrame
+    assert len(df) == count
 
+    count2 = gis.get_count(year=year_filter+1)
 
-    # No datasets currently trigger usage of the legacy server code
-    # def test_arcgis_legacy_server(self, csvfile, source, last, skip, loghtml):
-    #     url = "https://egis.baltimorecity.gov/egis/rest/services/GeoSpatialized_Tables/Arrest/FeatureServer/0/" 
+    # Ensure that count updates properly with different call (most recent count is cached)
+    assert count!=count2
 
-    #     gis = data_loaders.Arcgis(url)
-    #     gis.load(nrows=1)
+def test_socrata_geopandas():
+    if _has_gpd:
+        url = "data.montgomerycountymd.gov"
+        data_set = "4mse-ku6q"
+        date_field = "date_of_stop"
+        year = 2020
+        nrows = 1000
+        df = data_loaders.Socrata(url=url, data_set=data_set, date_field=date_field).load(year=year, nrows=nrows)
 
-    #     url = "https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/5/" 
-    #     gis = data_loaders.Arcgis(url)
-    #     gis.load(nrows=1)
+        assert type(df) == gpd.GeoDataFrame
+    else:
+        pass
+
+def test_socrata_pandas():
+    data_loaders._use_gpd_force = False
+    url = "data.montgomerycountymd.gov"
+    data_set = "usip-62e2"
+    date_field = "created_dt"
+    year = 2020
+    loader = data_loaders.Socrata(url=url, data_set=data_set, date_field=date_field)
+    df = loader.load(year=year, pbar=False)
+    count = loader.get_count(year=year)
+
+    # Reset
+    data_loaders._use_gpd_force = None
+
+    assert type(df) == pd.DataFrame
+    assert len(df) == count
+
+    count2 = loader.get_count(year=year+1)
+
+    # Ensure that count updates properly with different call (most recent count is cached)
+    assert count!=count2
+
+def test_socrata():
+    lim = data_loaders._default_limit
+    data_loaders._default_limit = 500
+    url = "data.austintexas.gov"
+    data_set = "sc8s-w4ka"
+    loader = data_loaders.Socrata(url, data_set)
+    df =loader.load(pbar=False)
+    assert not loader.isfile()
+    count = loader.get_count()
+
+    assert len(df)==count
+
+    offset = 1
+    nrows = len(df)-offset-1
+    df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
+    assert set(df.columns)==set(df_offset.columns)
+    df_offset = df_offset[df.columns]
+    assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
+
+    df_offset = loader.load(offset=offset, pbar=False)
+    assert set(df.columns)==set(df_offset.columns)
+    df_offset = df_offset[df.columns]
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+    
+    data_loaders._default_limit = lim
 
+    client = data_loaders.SocrataClient(url, data_loaders.default_sodapy_key, timeout=60)
+    results = client.get(data_set, order=":id", limit=100000)
+    rows = pd.DataFrame.from_records(results)
+
+    assert len(df) == count
+    assert rows.equals(df)
+
+def test_csv():
+    url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
+    date_field = "INCIDENT_DATE"
+    loader = data_loaders.Csv(url, date_field=date_field)
+    assert loader.isfile()
+    df = loader.load(pbar=False)
+
+    offset = 1
+    nrows = len(df)-offset-1
+    df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
+    assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
+    
+    df_offset = loader.load(offset=offset, pbar=False)
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
-    def test_arcgis_geopandas(self, csvfile, source, last, skip, loghtml):
-        if _has_gpd:
-            url = "https://services1.arcgis.com/zdB7qR0BtYrg0Xpl/arcgis/rest/services/ODC_CRIME_STOPS_P/FeatureServer/32/"
-            date_field = "TIME_PHONEPICKUP"
-            year_filter = 2020
-            nrows = 1000
-            df = data_loaders.Arcgis(url, date_field=date_field).load(year=year_filter, nrows=nrows)
+    df_comp = pd.read_csv(url)
+    df_comp = df_comp.astype({date_field: 'datetime64[ns]'})
+    df = df.astype({date_field: 'datetime64[ns]'})
 
-            assert type(df) == gpd.GeoDataFrame
-        else:
-            pass
+    count = loader.get_count()
+    assert len(df_comp) == count
+    # Test using cached value
+    assert count == loader.get_count()
 
-    def test_arcgis_pandas(self, csvfile, source, last, skip, loghtml):
-        data_loaders._use_gpd_force = False
-        url = "https://services1.arcgis.com/wpJGOi6N4Rq5cqFv/arcgis/rest/services/Pursuits_2020_2021/FeatureServer/0/"
-        date_field = "DATE"
-        year_filter = 2020
-        gis = data_loaders.Arcgis(url, date_field=date_field)
-        df = gis.load(year=year_filter)
-        count = gis.get_count(year=year_filter)
-        # Reset
-        data_loaders._use_gpd_force = None
-
-        assert type(df) == pd.DataFrame
-        assert len(df) == count
-
-        count2 = gis.get_count(year=year_filter+1)
-
-        # Ensure that count updates properly with different call (most recent count is cached)
-        assert count!=count2
-
-    def test_socrata_geopandas(self, csvfile, source, last, skip, loghtml):
-        if _has_gpd:
-            url = "data.montgomerycountymd.gov"
-            data_set = "4mse-ku6q"
-            date_field = "date_of_stop"
-            year = 2020
-            nrows = 1000
-            df = data_loaders.Socrata(url=url, data_set=data_set, date_field=date_field).load(year=year, nrows=nrows)
+    assert df_comp.equals(df)
 
-            assert type(df) == gpd.GeoDataFrame
-        else:
-            pass
+    with pytest.raises(ValueError):
+        loader.get_years()
 
-    def test_socrata_pandas(self, csvfile, source, last, skip, loghtml):
-        data_loaders._use_gpd_force = False
-        url = "data.montgomerycountymd.gov"
-        data_set = "usip-62e2"
-        date_field = "created_dt"
-        year = 2020
-        loader = data_loaders.Socrata(url=url, data_set=data_set, date_field=date_field)
-        df = loader.load(year=year, pbar=False)
-        count = loader.get_count(year=year)
+    years = loader.get_years(force=True)
 
-        # Reset
-        data_loaders._use_gpd_force = None
+    df = df.astype({date_field: 'datetime64[ns]'})
+    assert list(df[date_field].dt.year.sort_values(ascending=True).dropna().unique()) == years
 
-        assert type(df) == pd.DataFrame
-        assert len(df) == count
+    nrows = 7
+    df = data_loaders.Csv(url).load(nrows=nrows)
+    df_comp = pd.read_csv(url, nrows=nrows)
 
-        count2 = loader.get_count(year=year+1)
+    assert df_comp.equals(df)
 
-        # Ensure that count updates properly with different call (most recent count is cached)
-        assert count!=count2
-
-    def test_socrata(self, csvfile, source, last, skip, loghtml):
-        lim = data_loaders._default_limit
-        data_loaders._default_limit = 500
-        url = "data.austintexas.gov"
-        data_set = "sc8s-w4ka"
-        loader = data_loaders.Socrata(url, data_set)
-        df =loader.load(pbar=False)
-        assert not loader.isfile()
-        count = loader.get_count()
 
-        assert len(df)==count
+def test_csv_year_filter():
+    url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
+    loader = data_loaders.Csv(url, date_field="INCIDENT_DATE")
+    year = 2020
+    df = loader.load(year=year, pbar=False)
+    with pytest.raises(ValueError):
+        count = loader.get_count(year=year)
 
-        offset = 1
-        nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
-        assert set(df.columns)==set(df_offset.columns)
-        df_offset = df_offset[df.columns]
-        assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
-
-        df_offset = loader.load(offset=offset, pbar=False)
-        assert set(df.columns)==set(df_offset.columns)
-        df_offset = df_offset[df.columns]
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
-        
-        data_loaders._default_limit = lim
+    count = loader.get_count(year=year, force=True)
+    assert len(df) == count
 
-        client = data_loaders.SocrataClient(url, data_loaders.default_sodapy_key, timeout=60)
-        results = client.get(data_set, order=":id", limit=100000)
-        rows = pd.DataFrame.from_records(results)
-
-        assert len(df) == count
-        assert rows.equals(df)
-
-    def test_csv(self, csvfile, source, last, skip, loghtml):
-        url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
-        date_field = "INCIDENT_DATE"
-        loader = data_loaders.Csv(url, date_field=date_field)
-        assert loader.isfile()
-        df = loader.load(pbar=False)
-
-        offset = 1
-        nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
-        assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
-        
-        df_offset = loader.load(offset=offset, pbar=False)
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+    count2 = loader.get_count(year=year+1, force=True)
 
-        df_comp = pd.read_csv(url)
-        df_comp = df_comp.astype({date_field: 'datetime64[ns]'})
-        df = df.astype({date_field: 'datetime64[ns]'})
+    # Ensure that count updates properly with different call (most recent count is cached)
+    assert count!=count2
 
-        count = loader.get_count()
-        assert len(df_comp) == count
-        # Test using cached value
-        assert count == loader.get_count()
 
-        assert df_comp.equals(df)
+def test_excel():
+    url = "https://www.norristown.org/DocumentCenter/View/1789/2017-2018-Use-of-Force"
+    date_field = "Date"
+    loader = data_loaders.Excel(url, date_field=date_field, data_set='2017-2018')
+    assert loader.isfile()
+    df = loader.load(pbar=False)
 
-        with pytest.raises(ValueError):
-            loader.get_years()
+    offset = 1
+    nrows = len(df)-offset-1
+    df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
+    assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
 
-        years = loader.get_years(force=True)
+    df_offset = loader.load(offset=offset, pbar=False)
+    assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
-        df = df.astype({date_field: 'datetime64[ns]'})
-        assert list(df[date_field].dt.year.sort_values(ascending=True).dropna().unique()) == years
+    df_comp = pd.read_excel(url)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
 
-        nrows = 7
-        df = data_loaders.Csv(url).load(nrows=nrows)
-        df_comp = pd.read_csv(url, nrows=nrows)
+    with pytest.raises(ValueError):
+        count = loader.get_count()
+    count = loader.get_count(force=True)
+    assert len(df_comp) == count
 
-        assert df_comp.equals(df)
+    # Testing 2nd call which should used cached value
+    assert count == loader.get_count(force=True)
 
+    assert df_comp.equals(df)
 
-    def test_csv_year_filter(self, csvfile, source, last, skip, loghtml):
-        url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
-        loader = data_loaders.Csv(url, date_field="INCIDENT_DATE")
-        year = 2020
-        df = loader.load(year=year, pbar=False)
-        with pytest.raises(ValueError):
-            count = loader.get_count(year=year)
+    with pytest.raises(ValueError):
+        loader.get_years()
 
-        count = loader.get_count(year=year, force=True)
-        assert len(df) == count
+    years = loader.get_years(force=True)
 
-        count2 = loader.get_count(year=year+1, force=True)
+    df = df.astype({date_field: 'datetime64[ns]'})
+    assert list(df[date_field].dt.year.sort_values(ascending=True).dropna().unique()) == years
 
-        # Ensure that count updates properly with different call (most recent count is cached)
-        assert count!=count2
+    nrows = 7
+    df = loader.load(nrows=nrows, pbar=False)        
+    df_comp = pd.read_excel(url, nrows=nrows)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    assert df_comp.equals(df)
 
 
-    def test_excel(self, csvfile, source, last, skip, loghtml):
-        url = "https://www.norristown.org/DocumentCenter/View/1789/2017-2018-Use-of-Force"
-        date_field = "Date"
-        loader = data_loaders.Excel(url, date_field=date_field, sheet='2017-2018')
-        assert loader.isfile()
-        df = loader.load(pbar=False)
+def test_excel_year_sheets(skip):
+    if "Northampton" in skip:
+        return
 
-        offset = 1
-        nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
-        assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
+    url = "https://northamptonpd.com/images/ODP%20Spreadsheets/2014-2020_MV_Pursuits_incident_level_data.xlsx"
+    loader = data_loaders.Excel(url, date_field="Date")
 
-        df_offset = loader.load(offset=offset, pbar=False)
-        assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
+    years = loader.get_years()
+    assert years == [x for x in range(2014,2021)]
 
-        df_comp = pd.read_excel(url)
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    df_comp = pd.read_excel(url, sheet_name="2014")
+    df_comp.columns= [x for x in df_comp.iloc[0]]
+    df_comp.drop(index=df_comp.index[0], inplace=True)
+    df_comp.reset_index(drop=True, inplace=True)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    df_comp = df_comp.iloc[:, 1:]
 
-        with pytest.raises(ValueError):
-            count = loader.get_count()
-        count = loader.get_count(force=True)
-        assert len(df_comp) == count
+    # Load all years
+    df_2014 = loader.load(year=2014, pbar=False)
 
-        # Testing 2nd call which should used cached value
-        assert count == loader.get_count(force=True)
+    assert df_comp.equals(df_2014)
 
-        assert df_comp.equals(df)
+    df_comp = pd.read_excel(url, sheet_name="2015")
+    df_comp.columns= [x for x in df_comp.iloc[0]]
+    df_comp.drop(index=df_comp.index[0], inplace=True)
+    df_comp.reset_index(drop=True, inplace=True)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    df_comp = df_comp.iloc[:, 1:]
 
-        with pytest.raises(ValueError):
-            loader.get_years()
+    # Load all years
+    df_2015 = loader.load(year=2015, pbar=False)
 
-        years = loader.get_years(force=True)
+    assert df_comp.equals(df_2015)
 
-        df = df.astype({date_field: 'datetime64[ns]'})
-        assert list(df[date_field].dt.year.sort_values(ascending=True).dropna().unique()) == years
+    # Note: There is no 2013 data
+    df_multi = loader.load(year=[2013,2015], pbar=False)
 
-        nrows = 7
-        df = loader.load(nrows=nrows, pbar=False)        
-        df_comp = pd.read_excel(url, nrows=nrows)
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        assert df_comp.equals(df)
+    assert df_multi.equals(pd.concat([df_2014, df_2015], ignore_index=True))
 
+    df = loader.load(pbar=False)
+    df_last = loader.load(year=years[-1], pbar=False)
 
-    def test_excel_year_sheets(self, csvfile, source, last, skip, loghtml):
-        if skip != None:
-            skip = skip.split(",")
-            skip = [x.strip() for x in skip]
-            if "Northampton" in skip:
-                return
+    assert df.head(len(df_multi)).equals(df_multi)
+    assert df.tail(len(df_last)).reset_index(drop=True).equals(df_last.reset_index(drop=True))
 
-        url = "https://northamptonpd.com/images/ODP%20Spreadsheets/2014-2020_MV_Pursuits_incident_level_data.xlsx"
-        loader = data_loaders.Excel(url, date_field="Date")
+    # Test loading to ensure that channel name changes are handled
+    data_loaders.Excel("https://northamptonpd.com/images/ODP%20Spreadsheets/NPD_Use_of_Force_2014-2020_incident_level_data.xlsx").load()
 
-        years = loader.get_years()
-        assert years == [x for x in range(2014,2021)]
+def test_excel_header():
+    url = "https://cms7files1.revize.com/sparksnv/Document_Center/Sparks%20Police/IA%20Data/2000-2022-SPD-OIS-Incidents%20(3).xlsx"
 
-        df_comp = pd.read_excel(url, sheet_name="2014")
-        df_comp.columns= [x for x in df_comp.iloc[0]]
-        df_comp.drop(index=df_comp.index[0], inplace=True)
-        df_comp.reset_index(drop=True, inplace=True)
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        df_comp = df_comp.iloc[:, 1:]
+    loader = data_loaders.Excel(url)
+    df = loader.load(pbar=False)
 
-        # Load all years
-        df_2014 = loader.load(year=2014, pbar=False)
+    df_comp = pd.read_excel(url)
+    df_comp.columns= [x for x in df_comp.iloc[3]]
+    df_comp.drop(index=df_comp.index[0:4], inplace=True)
+    df_comp.reset_index(drop=True, inplace=True)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    df_comp = df_comp.dropna(thresh=10)
 
-        assert df_comp.equals(df_2014)
+    assert(df_comp.equals(df))
 
-        df_comp = pd.read_excel(url, sheet_name="2015")
-        df_comp.columns= [x for x in df_comp.iloc[0]]
-        df_comp.drop(index=df_comp.index[0], inplace=True)
-        df_comp.reset_index(drop=True, inplace=True)
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        df_comp = df_comp.iloc[:, 1:]
 
-        # Load all years
-        df_2015 = loader.load(year=2015, pbar=False)
+def test_excel_xls():
+    url = r"http://gouda.beloitwi.gov/WebLink/0/edoc/66423/3Use%20of%20Force%202017%20-%20last%20updated%201-12-18.xls"
 
-        assert df_comp.equals(df_2015)
+    try:
+        df_comp = pd.read_excel(url)
+    except Exception as e:
+        if len(e.args) and e.args[0]=='Excel file format cannot be determined, you must specify an engine manually.':
+            r = requests.get(url)
+            r.raise_for_status()
+            text = r.content
+            file_like = BytesIO(text)
+            df_comp = pd.read_excel(file_like)
+        else:
+            raise e
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    df = data_loaders.Excel(url).load()
 
-        # Note: There is no 2013 data
-        df_multi = loader.load(year=[2013,2015], pbar=False)
+    assert df_comp.equals(df)
 
-        assert df_multi.equals(pd.concat([df_2014, df_2015], ignore_index=True))
 
-        df = loader.load(pbar=False)
-        df_last = loader.load(year=years[-1], pbar=False)
+def test_excel_xls_protected():
+    url = "http://www.rutlandcitypolice.com/app/download/5136813/ResponseToResistance+2015-2017.xls"
 
-        assert df.head(len(df_multi)).equals(df_multi)
-        assert df.tail(len(df_last)).reset_index(drop=True).equals(df_last.reset_index(drop=True))
+    r = requests.get(url)
+    r.raise_for_status()
 
-        # Test loading to ensure that channel name changes are handled
-        data_loaders.Excel("https://northamptonpd.com/images/ODP%20Spreadsheets/NPD_Use_of_Force_2014-2020_incident_level_data.xlsx").load()
+    import os
+    import msoffcrypto
+    import tempfile
+    # Create a file path by joining the directory name with the desired file name
+    output_directory = tempfile.gettempdir()
+    file_path = os.path.join(output_directory, 'temp1.xls')
 
-    def test_excel_header(self, csvfile, source, last, skip, loghtml):
-        url = "https://cms7files1.revize.com/sparksnv/Document_Center/Sparks%20Police/IA%20Data/2000-2022-SPD-OIS-Incidents%20(3).xlsx"
+    # Write the file
+    with open(file_path, 'wb') as output:
+        output.write(r.content)
 
-        loader = data_loaders.Excel(url)
-        df = loader.load(pbar=False)
+    file_path_decrypted = os.path.join(output_directory, 'temp2.xls')
+    # Try and unencrypt workbook with magic password
+    fp = open(file_path, 'rb')
+    wb_msoffcrypto_file = msoffcrypto.OfficeFile(fp)
 
-        df_comp = pd.read_excel(url)
-        df_comp.columns= [x for x in df_comp.iloc[3]]
-        df_comp.drop(index=df_comp.index[0:4], inplace=True)
-        df_comp.reset_index(drop=True, inplace=True)
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        df_comp = df_comp.dropna(thresh=10)
-
-        assert(df_comp.equals(df))
-
-
-    def test_excel_xls(self, csvfile, source, last, skip, loghtml):
-        url = r"http://gouda.beloitwi.gov/WebLink/0/edoc/66423/3Use%20of%20Force%202017%20-%20last%20updated%201-12-18.xls"
-
-        try:
-            df_comp = pd.read_excel(url)
-        except Exception as e:
-            if len(e.args) and e.args[0]=='Excel file format cannot be determined, you must specify an engine manually.':
-                r = requests.get(url)
-                r.raise_for_status()
-                text = r.content
-                file_like = BytesIO(text)
-                df_comp = pd.read_excel(file_like)
-            else:
-                raise e
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        df = data_loaders.Excel(url).load()
+    # https://stackoverflow.com/questions/22789951/xlrd-error-workbook-is-encrypted-python-3-2-3
+    # https://nakedsecurity.sophos.com/2013/04/11/password-excel-velvet-sweatshop/
+    wb_msoffcrypto_file.load_key(password='VelvetSweatshop')
+    with open(file_path_decrypted, 'wb') as output:
+        wb_msoffcrypto_file.decrypt(output)
 
-        assert df_comp.equals(df)
+    fp.close()
 
+    df_comp = pd.read_excel(open(file_path_decrypted, 'rb'))
 
-    def test_excel_xls_protected(self, csvfile, source, last, skip, loghtml):
-        url = "http://www.rutlandcitypolice.com/app/download/5136813/ResponseToResistance+2015-2017.xls"
+    os.remove(file_path)
+    os.remove(file_path_decrypted)
 
-        r = requests.get(url)
-        r.raise_for_status()
+    loader = data_loaders.Excel(url)
+    df = loader.load(pbar=False)
 
-        import os
-        import msoffcrypto
-        import tempfile
-        # Create a file path by joining the directory name with the desired file name
-        output_directory = tempfile.gettempdir()
-        file_path = os.path.join(output_directory, 'temp1.xls')
-
-        # Write the file
-        with open(file_path, 'wb') as output:
-            output.write(r.content)
-
-        file_path_decrypted = os.path.join(output_directory, 'temp2.xls')
-        # Try and unencrypt workbook with magic password
-        fp = open(file_path, 'rb')
-        wb_msoffcrypto_file = msoffcrypto.OfficeFile(fp)
-
-        # https://stackoverflow.com/questions/22789951/xlrd-error-workbook-is-encrypted-python-3-2-3
-        # https://nakedsecurity.sophos.com/2013/04/11/password-excel-velvet-sweatshop/
-        wb_msoffcrypto_file.load_key(password='VelvetSweatshop')
-        with open(file_path_decrypted, 'wb') as output:
-            wb_msoffcrypto_file.decrypt(output)
-
-        fp.close()
-
-        df_comp = pd.read_excel(open(file_path_decrypted, 'rb'))
-
-        os.remove(file_path)
-        os.remove(file_path_decrypted)
-
-        loader = data_loaders.Excel(url)
-        df = loader.load(pbar=False)
-
-        df_comp = df_comp.convert_dtypes()
-        df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
-        assert df_comp.equals(df)
+    df_comp = df_comp.convert_dtypes()
+    df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+    assert df_comp.equals(df)
 
 if __name__ == "__main__":
-    tp = TestProduct()
 
-    tp.test_ckan(None,None,None,None,None)
-    # tp.test_carto(None,None,None,None,None)
-    # tp.test_arcgis(None,None,None,None,None)
-    # tp.test_arcgis_geopandas(None,None,None,None,None)
-    # tp.test_arcgis_pandas(None,None,None,None,None)
-    # tp.test_csv(None,None,None,None,None)
-    # tp.test_csv_year_filter(None,None,None,None,None)
-    # tp.test_process_date_input_empty(None,None,None,None,None)
-    # tp.test_process_date_too_many(None,None,None,None,None)
-    # tp.test_process_dates_year_input_wrong_order(None,None,None,None,None)
-    # tp.test_socrata(None,None,None,None,None)
-    # tp.test_socrata_geopandas(None,None,None,None,None)
-    # tp.test_socrata_pandas(None,None,None,None,None)
-    # tp.test_excel(None,None,None,None,None)
-    # tp.test_excel_year_sheets(None,None,None,None,None)
-    # tp.test_excel_header(None,None,None,None,None)
-    tp.test_excel_xls(None,None,None,None,None)
-    tp.test_excel_xls_protected(None,None,None,None,None)
+    test_combined(None, None, None, None, None)
+    # test_ckan(None,None,None,None,None)
+    # test_carto(None,None,None,None,None)
+    # test_arcgis(None,None,None,None,None)
+    # test_arcgis_geopandas(None,None,None,None,None)
+    # test_arcgis_pandas(None,None,None,None,None)
+    # test_csv(None,None,None,None,None)
+    # test_csv_year_filter(None,None,None,None,None)
+    # test_process_date_input_empty(None,None,None,None,None)
+    # test_process_date_too_many(None,None,None,None,None)
+    # test_process_dates_year_input_wrong_order(None,None,None,None,None)
+    # test_socrata(None,None,None,None,None)
+    # test_socrata_geopandas(None,None,None,None,None)
+    # test_socrata_pandas(None,None,None,None,None)
+    # test_excel(None,None,None,None,None)
+    # test_excel_year_sheets(None,None,None,None,None)
+    # test_excel_header(None,None,None,None,None)
+    # test_excel_xls(None,None,None,None,None)
+    # test_excel_xls_protected(None,None,None,None,None)
```

### Comparing `openpolicedata-0.6/tests/test_deprecated.py` & `openpolicedata-0.7/tests/test_deprecated.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,91 +12,83 @@
 import pytest
 
 @pytest.fixture(scope='module')
 def df_compat():
 	compat_versions_file = 'https://github.com/openpolicedata/opd-data/raw/main/compatibility/compat_versions.csv'
 	return pd.read_csv(compat_versions_file, dtype=str)
 
-def get_datasets(csvfile):
-    if csvfile != None:
-        opd.datasets.datasets = opd.datasets._build(csvfile)
-
-    return opd.datasets.datasets
-
 @input_swap([0,1], ['table_type','year'], [TableType, {'values':[opd.defs.NA, opd.defs.MULTI], 'types':[list, int]}], opt1=None)
 def fswap(table_type,year):
 	if table_type:
 		TableType(table_type)
 	assert year in [opd.defs.NA, opd.defs.MULTI] or isinstance(year,int) or isinstance(year,list)
 
 @input_swap([0,1], ['table_type','year'], [TableType, {'values':[opd.defs.NA, opd.defs.MULTI], 'types':[list, int]}], error=True, opt1=None)
 def fswap_error(table_type,year):
 	fswap(table_type,year)
 
 @pytest.mark.parametrize("year", [2019, [2019, 2020], opd.defs.NA, opd.defs.MULTI])
 @pytest.mark.parametrize("table_type", [TableType.ARRESTS, str(TableType.ARRESTS)])
-def test_no_inputswap(csvfile, source, last, skip, loghtml, year, table_type):
+def test_no_inputswap(year, table_type):
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		fswap(table_type, year)
 
 
 @pytest.mark.parametrize("year", [2019, [2019, 2020], opd.defs.NA, opd.defs.MULTI])
 @pytest.mark.parametrize("table_type", [TableType.ARRESTS, str(TableType.ARRESTS)])
-def test_inputswap_warning(csvfile, source, last, skip, loghtml, year, table_type):
+def test_inputswap_warning(year, table_type):
 	with pytest.warns(DeprecationWarning):
 		fswap(year, table_type)
 
 
 @pytest.mark.parametrize("year", [2019, [2019, 2020], opd.defs.NA, opd.defs.MULTI])
 @pytest.mark.parametrize("table_type", [TableType.ARRESTS, str(TableType.ARRESTS)])
-def test_inputswap_keyword_warning(csvfile, source, last, skip, loghtml, year, table_type):
+def test_inputswap_keyword_warning(year, table_type):
 	with pytest.warns(DeprecationWarning):
 		fswap(year, table_type=table_type)
 
 
 @pytest.mark.parametrize("year", [2019, [2019, 2020], opd.defs.NA, opd.defs.MULTI])
 @pytest.mark.parametrize("table_type", [TableType.ARRESTS, str(TableType.ARRESTS)])
-def test_inputswap_singleinput_warning(csvfile, source, last, skip, loghtml, year, table_type):
+def test_inputswap_singleinput_warning(year, table_type):
 	with pytest.warns(DeprecationWarning):
 		fswap(year)
 
 
 @pytest.mark.parametrize("year", [2019, [2019, 2020], opd.defs.NA, opd.defs.MULTI])
 @pytest.mark.parametrize("table_type", [TableType.ARRESTS, str(TableType.ARRESTS)])
-def test_inputswap_error(csvfile, source, last, skip, loghtml, year, table_type):
+def test_inputswap_error(year, table_type):
 	with pytest.raises(ValueError, match='have been swapped'):
 		fswap_error(year, table_type)
 
 
 @deprecated("MSG")
 def fdep():
 	pass
 
 @pytest.mark.parametrize("func", [fdep, datasets_query])
-def test_deprecated_decorator(csvfile, source, last, skip, loghtml, func):
+def test_deprecated_decorator(func):
 	with pytest.warns(DeprecationWarning):
 		func()
 
 
 @pytest.mark.parametrize("type1, type2", [("COMPLAINTS - SUBJECTS", 'COMPLAINTS - CIVILIANS'),
 										  ("USE OF FORCE - SUBJECTS/OFFICERS", 'USE OF FORCE - CIVILIANS/OFFICERS')])
-def test_deprecated_enums(csvfile, source, last, skip, loghtml, type1, type2):
+def test_deprecated_enums(type1, type2):
 	with pytest.warns(DeprecationWarning):
 		assert TableType(type1) == TableType(type2)
 
 
-def test_datasets_no_civilian_tabletypes(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_no_civilian_tabletypes():
 	df = opd.datasets.query()
 	assert not df["TableType"].str.contains("CIVILIAN").any()
 
 
-def test_datasets_equals_civilian(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_equals_civilian():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	s = df["TableType"]
 	assert isinstance(s, DeprecationHandlerSeries)
 	with pytest.warns(DeprecationWarning):
 		t = s == "USE OF FORCE - CIVILIANS/OFFICERS"
@@ -104,217 +96,196 @@
 	assert t.sum()>0
 	s = df["TableType"][t]
 	assert isinstance(s, pd.Series)
 	assert len(s)>0
 	assert len(df[t])>0
 
 
-def test_datasets_equals_subjects(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_equals_subjects():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	s = df["TableType"]
 	assert isinstance(s, DeprecationHandlerSeries)
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		t = s == "USE OF FORCE - SUBJECTS/OFFICERS"
 
 	assert t.sum()>0
 	assert len(df["TableType"][t])>0
 	assert len(df[t])>0
 
 
-def test_datasets_get_datatype(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_get_datatype():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	s = df["DataType"]
 	assert isinstance(s, pd.Series)
 
 
-def test_datasets_iloc_single_table_type(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_iloc_single_table_type():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	k = [j for j,x in enumerate(df.columns) if x=="TableType"][0]
 	assert isinstance(df.iloc[:, k], DeprecationHandlerSeries)
 
-def test_datasets_iloc_single_table_type_subset_no_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_iloc_single_table_type_subset_no_subject():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	k = [j for j,x in enumerate(df.columns) if x=="TableType"][0]
 	s = df.iloc[:2, k]
 	if not s.str.contains("SUBJECT").any():
 		assert isinstance(s, pd.Series)
 
-def test_datasets_iloc_single_table_type_subset_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_iloc_single_table_type_subset_subject():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	k = [j for j,x in enumerate(df.columns) if x=="TableType"][0]
 	s = df.iloc[31:34, k]
 	if s.str.contains("SUBJECT").any():
 		assert isinstance(s, DeprecationHandlerSeries)
 
 
-def test_datasets_iloc_single_not_table_type(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_iloc_single_not_table_type():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	k = [j for j,x in enumerate(df.columns) if x!="TableType"][0]
 	assert isinstance(df.iloc[:, k], pd.Series)
 
-def test_datasets_iloc_single_row(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_iloc_single_row():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	assert isinstance(df.iloc[0], pd.Series)
 
 
-def test_datasets_loc_single_table_type(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_loc_single_table_type():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	assert isinstance(df.loc[:, "TableType"], DeprecationHandlerSeries)
 
-def test_datasets_loc_single_table_type_subset_no_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_loc_single_table_type_subset_no_subject():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	s = df.loc[:2, "TableType"]
 	if not s.str.contains("SUBJECT").any():
 		assert isinstance(s, pd.Series)
 
-def test_datasets_loc_single_table_type_subset_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_loc_single_table_type_subset_subject():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	s = df.loc[31:34, "TableType"]
 	if s.str.contains("SUBJECT").any():
 		assert isinstance(s, DeprecationHandlerSeries)
 
 
-def test_datasets_loc_single_not_table_type(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_loc_single_not_table_type():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	assert isinstance(df.loc[:, "DataType"], pd.Series)
 
-def test_datasets_loc_single_row(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_loc_single_row():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	assert isinstance(df.loc[0], pd.Series)
 
 
-def test_datasets_isin_civilians(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_isin_civilians():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	with pytest.warns(DeprecationWarning):
 		df["TableType"].isin(["ARRESTS", "OFFICER-INVOLVED SHOOTINGS - CIVILIANS"])
 
 
-def test_datasets_isin_subjects(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_isin_subjects():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		df["TableType"].isin(["ARRESTS", "OFFICER-INVOLVED SHOOTINGS - SUBJECTS"])
 
 
-def test_datasets_isin_DataType(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_datasets_isin_DataType():
 	df = opd.datasets.query()
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		df["DataType"].isin(["ARRESTS", "OFFICER-INVOLVED SHOOTINGS - SUBJECTS"])
 
 
-def test_pandas_query_no_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_pandas_query_no_subject():
 	df = opd.datasets.query(state="Virginia")
 	assert isinstance(df, pd.DataFrame)
 
 
-def test_pandas_query_has_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_pandas_query_has_subject():
 	df = opd.datasets.query(state="California")
 	assert isinstance(df, DeprecationHandlerDataFrame)
 
 
-def test_pandas_query_tabletype_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_pandas_query_tabletype_subject():
 	with pytest.warns(DeprecationWarning):
 		df = opd.datasets.query(table_type="COMPLAINTS - CIVILIANS")
 	assert isinstance(df, DeprecationHandlerDataFrame)
 	assert len (df)>0
 
 
-def test_pandas_query_tabletype_no_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_pandas_query_tabletype_no_subject():
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		df = opd.datasets.query(table_type=opd.defs.TableType.COMPLAINTS_SUBJECTS)
 	assert isinstance(df, pd.DataFrame)
 	assert len (df)>0
 
-def test_tabletype_contains_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_tabletype_contains_subject():
 	with pytest.warns(DeprecationWarning):
 		t = opd.datasets.get_table_types(contains="- CIVILIANS")
 	assert len (t)>0
 
 
-def test_tabletype_contains_no_subject(csvfile, source, last, skip, loghtml):
-	get_datasets(csvfile)
+def test_tabletype_contains_no_subject():
 	with warnings.catch_warnings():
 		warnings.simplefilter("error")
 		t = opd.datasets.get_table_types(contains="- SUBJECTS")
 	assert len (t)>0
 
-def test_source_table_not_deprecated(csvfile, source, last, skip, loghtml):
+def test_source_table_not_deprecated():
 	assert not check_compat_source_table(cur_ver='100.0')[0]
 
-def test_source_table_bad_df_compat(csvfile, source, last, skip, loghtml):
+def test_source_table_bad_df_compat():
 	assert not check_compat_source_table(df_compat=1)[0]
 
-def test_source_table_deprecated(csvfile, source, last, skip, loghtml):
+def test_source_table_deprecated():
 	with pytest.warns(DeprecationWarning):
 		loaded, df = check_compat_source_table(cur_ver='0.0')
 	assert loaded
 	assert len(df)==1  # Number of rows in 1st test source table
 
-def test_source_table_fail_not_req(csvfile, source, last, skip, loghtml, df_compat):
+def test_source_table_fail_not_req(df_compat):
 	df_compat = df_compat.copy(deep=True)
 	df_compat.loc[0, 'csv_name'] = '?!~notafile.csv'
 	with pytest.warns(DeprecationWarning):
 		loaded, df = check_compat_source_table(df_compat=df_compat, cur_ver='0.0')
 	assert loaded
 	assert len(df)==2  # Number of rows in 2nd test source table
 
-def test_source_table_fail_req(csvfile, source, last, skip, loghtml, df_compat):
+def test_source_table_fail_req(df_compat):
 	df_compat = df_compat.copy(deep=True)
 	df_compat.loc[1, 'csv_name'] = '?!~notafile.csv'
 	with pytest.raises(opd.exceptions.CompatSourceTableLoadError):
 		check_compat_source_table(df_compat=df_compat, cur_ver='0.0.1')
 
 
 if __name__ == "__main__":
```

### Comparing `openpolicedata-0.6/tests/test_opd_data1.py` & `openpolicedata-0.7/tests/test_opd_data3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,344 +1,415 @@
 import pytest
 
 if __name__ == "__main__":
 	import sys
 	sys.path.append('../openpolicedata')
-from openpolicedata import data, datasets, data_loaders
-from openpolicedata.defs import DataType, TableType
+from openpolicedata import data, data_loaders
+from openpolicedata import datasets
+from openpolicedata.defs import MULTI, DataType
 from openpolicedata.exceptions import OPD_DataUnavailableError, OPD_TooManyRequestsError,  \
-	OPD_MultipleErrors, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError
+	OPD_MultipleErrors, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError, \
+	DateFilterException
+import random
 from datetime import datetime
 import pandas as pd
 from time import sleep
 import warnings
 import os
+import re
 
-sleep_time = 0.1
+from test_utils import check_for_dataset
 
 # Set Arcgis data loader to validate queries with arcgis package if installed
 data_loaders._verify_arcgis = True
 
+sleep_time = 0.1
 log_filename = f"pytest_url_errors_{datetime.now().strftime('%Y%m%d_%H')}.txt"
 log_folder = os.path.join(".","data/test_logs")
 
 outages_file = os.path.join("..","opd-data","outages.csv")
 # if has_outages:=os.path.exists(outages_file):
 has_outages=os.path.exists(outages_file)
 if has_outages:
 	outages = pd.read_csv(outages_file)
 else:
 	try:
 		outages = pd.read_csv('https://raw.githubusercontent.com/openpolicedata/opd-data/main/outages.csv')
 		has_outages = True
 	except:
 		pass
-
-warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
-
-def get_datasets(csvfile):
-	if csvfile is not None and not os.path.exists(csvfile):
-		raise ValueError(f"Unable to find {csvfile}")
-
-	if csvfile != None:
-		datasets.datasets = datasets._build(csvfile)
-
-	return datasets.datasets
-
-def user_request_skip(datasets, i, skip, last, source):
-	# Skip sources that the user requested to skip
-	if skip != None:
-		skip = skip.split(",")
-		skip = [x.strip() for x in skip]
-	if skip != None and datasets.iloc[i]["SourceName"] in skip:
-		return True
-	# User requested only the last values to run
-	if last!=None and i < len(datasets) - last:
-		return True
-	if source != None and datasets.iloc[i]["SourceName"] != source:
-		return True
 	
-	return False
-
-class TestData:
-	def check_table_type_warning(self, csvfile, source, last, skip, loghtml):
-		sources = datasets.query().copy().iloc[0]
-		sources["TableType"] = "TEST"
-		with pytest.warns(UserWarning):
-			data.Table(sources)
-
-	def test_check_version(self, csvfile, source, last, skip, loghtml):
-		ds = get_datasets(csvfile).iloc[0].copy()
-		# Set min_version to create error
-		ds["min_version"] = "-1"
-		with pytest.raises(OPD_FutureError):
-			data._check_version(ds)
-
-		ds["min_version"] = "100000.0"
-		with pytest.raises(OPD_MinVersionError):
-			data._check_version(ds)
-
-		# These should pass
-		ds["min_version"] = "0.0"
-		data._check_version(ds)
-		ds["min_version"] = pd.NA
-		data._check_version(ds)
-
-
-	def test_offsets_and_nrows(self, csvfile, source, last, skip, loghtml):
-		get_datasets(csvfile)
-		src = data.Source("Philadelphia")
-		df = src.load(year=2019, table_type="Officer-Involved Shootings").table
-		offset = 1
-		nrows = len(df)-2
-		df_offset = src.load(year=2019, table_type="Officer-Involved Shootings", offset=offset, nrows=nrows).table
-		assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
-
-	def check_excel_sheets(self, csvfile, source, last, skip, loghtml):
-		datasets = get_datasets(csvfile)
-		for i in range(len(datasets)):
-			if user_request_skip(datasets, i, skip, last, source):
-				continue
+warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
-			if datasets.iloc[i]["DataType"]!=DataType.EXCEL:
+def test_bloomington_citations():
+	if check_for_dataset('Bloomington', 'CITATIONS'):
+		src = data.Source("Bloomington")
+		count = src.get_count('CITATIONS', MULTI)
+
+		match = src.datasets['TableType']=='CITATIONS'
+		assert match.sum()==1
+		dataset = src.datasets[match].iloc[0]
+		loader = data_loaders.Socrata(dataset['URL'], dataset['dataset_id'])
+		df = loader.load()
+		assert len(df) == count
+		dates = df[dataset['date_field']]
+
+		count_by_year = []
+		for y in range(2016, 2021):
+			count_by_year.append(src.get_count('CITATIONS', y))
+			matches_YYYY = dates.str.startswith(f"{y}-")
+			dates = dates.drop(index=matches_YYYY[matches_YYYY].index)
+			matches_YY = dates.str.match(r'\d{1,2}/\d{1,2}/'+str(y)[2:])
+			dates = dates.drop(index=matches_YY[matches_YY].index)
+			assert count_by_year[-1] == matches_YYYY.sum() + matches_YY.sum()
+
+		assert count==sum(count_by_year)
+
+@pytest.mark.slow(reason="This is a slow test that should be run before a major commit.")
+def test_load_year(datasets, source, start_idx, skip, loghtml, query={}):
+	max_count = 1e5
+		
+	caught_exceptions = []
+	caught_exceptions_warn = []
+	already_run = []
+	for i in range(len(datasets)):
+		if skip != None and datasets.iloc[i]["SourceName"] in skip:
+			continue
+		if i < start_idx:
+			continue
+		if source != None and datasets.iloc[i]["SourceName"] != source:
+			continue
+
+		if is_stanford(datasets.iloc[i]["URL"]):
+			# There are a lot of data sets from Stanford, no need to run them all
+			# Just run approximately a small percentage
+			rnd = random.uniform(0,1)
+			if rnd>0.05:
 				continue
 
-			srcName = datasets.iloc[i]["SourceName"]
-			state = datasets.iloc[i]["State"]
-			src = data.Source(srcName, state=state)
+		match = True
+		for k,v in query.items():
+			if datasets.iloc[i][k]!=v:
+				match = False
+				break
+		if not match:
+			continue
+
+		srcName = datasets.iloc[i]["SourceName"]
+		state = datasets.iloc[i]["State"]
+
+		if datasets.iloc[i]["Agency"] == MULTI and \
+			srcName == "Virginia":
+			# Reduce size of data load by filtering by agency
+			agency = "Henrico Police Department"
+		else:
+			agency = None
 
-			table_print = datasets.iloc[i]["TableType"]
-			now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-			print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
+		table_print = datasets.iloc[i]["TableType"]
 
-			excel = src._Source__get_loader(datasets.iloc[i]["DataType"], datasets.iloc[i]["URL"], 
-				   dataset_id=datasets.iloc[i]["dataset_id"])
-			sheets, has_year_sheets = excel._Excel__get_sheets()
-
-			if has_year_sheets:
-				# Ensure that load works
-				src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False)
+		unique_id = [srcName, state, datasets.iloc[i]["Agency"], table_print]
+		if unique_id in already_run:
+			continue
+
+		now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
+		print(f"{now} Testing {i} of {len(datasets)-1}: {srcName} {table_print} table")
+
+		src = data.Source(srcName, state=state)
+
+		# Handle cases where URL is required to disambiguate requested dataset
+		ds_filter, _ = src._Source__filter_for_source(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], None, errors=False)
+		ds_input = datasets.iloc[[i]] if isinstance(ds_filter,pd.DataFrame) and len(ds_filter)>1 else None
+
+		if ds_input is None:
+			already_run.append(unique_id)
+
+		try:
+			try:
+				years = src.get_years(datasets.iloc[i]["TableType"], datasets=ds_input)
+			except ValueError as e:
+				if len(e.args)>0 and "Extracting the years" in e.args[0]:
+					# Just test reading in the table and continue
+					table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], 
+									agency=agency, pbar=False)
+					continue
+				else:
+					raise
+			except:
+				raise
+		except warn_errors as e:
+			e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+			caught_exceptions_warn.append(e)
+			continue
+		except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
+			# Catch exceptions related to URLs not functioning
+			e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+			caught_exceptions.append(e)
+			continue
+		except:
+			raise
+
+		# Adding a pause here to prevent issues with requesting from site too frequently
+		sleep(sleep_time)
+
+		years_orig = years.copy()
+		for y in src.datasets[src.datasets["TableType"] == datasets.iloc[i]["TableType"]]["Year"]:
+			if y != MULTI:
+				years.remove(y)
+
+		if len(years)==0:
+			# Each datasets is annual
+			# Run 1st and last year
+			multi_case = False
+			years = [min(years_orig)]
+			if len(years_orig)>1:
+				years.append(max(years_orig))
+		else:
+			multi_case = True
+			if len(years)>1:
+				# It is preferred to to not use first or last year that start and stop of year are correct
+				years = years[-2:-1]
 			else:
-				excel._Excel__check_sheet(sheets)
+				years = years[:1]
 
-		
-	def test_source_download_limitable(self, csvfile, source, last, skip, loghtml, query={}):
-		datasets = get_datasets(csvfile)
-		num_stanford = 0
-		max_num_stanford = 1  # This data is standardized. Probably no need to test more than 1
-		caught_exceptions = []
-		caught_exceptions_warn = []
-			
-		for i in range(len(datasets)):
-			if user_request_skip(datasets, i, skip, last, source):
+		tables = []
+		future_error = False
+		for year in years:
+			try:
+				table = src.load(datasets.iloc[i]["TableType"], year, 
+										agency=agency, pbar=False, 
+										sortby="date",
+										nrows=max_count if datasets.iloc[i]["DataType"] not in ["CSV","Excel"] else None)
+			except OPD_FutureError as e:
+				future_error = True
+				break
+			except OPD_DataUnavailableError as e:
+				caught_exceptions_warn.append(e)
+				tables.append(None)
 				continue
+			except:
+				raise
 
-			has_date_field = not pd.isnull(datasets.iloc[i]["date_field"])
-			if can_be_limited(datasets.iloc[i]["DataType"], datasets.iloc[i]["URL"]) or has_date_field:
-				if is_stanford(datasets.iloc[i]["URL"]):
-					num_stanford += 1
-					if num_stanford > max_num_stanford:
-						continue
-				match = True
-				for k,v in query.items():
-					if datasets.iloc[i][k]!=v:
-						match = False
-						break
-				if not match:
-					continue
+			sleep(sleep_time)
 
-				srcName = datasets.iloc[i]["SourceName"]
-				state = datasets.iloc[i]["State"]
-				src = data.Source(srcName, state=state)
-
-				table_print = datasets.iloc[i]["TableType"]
-				now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-				print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
-
-				try:
-					table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False, nrows=20)
-				except warn_errors as e:
-					e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"])
-					caught_exceptions_warn.append(e)
-					continue
-				except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
-					# Catch exceptions related to URLs not functioning
-					e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"])
-					caught_exceptions.append(e)
-					continue
-				except:
-					raise
-
-				if len(table.table)==0 and has_outages and \
-					(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
-					caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
-					continue
+			if len(table.table)==0:
+				# Ensure count should have been 0
+				count = src.get_count(datasets.iloc[i]["TableType"], year, agency=agency, force=True)
+				if count!=0:
+					raise ValueError(f"Expected data for year {year} but received none")
+				
+				# There may not be any data for the year requested.
+				for y in years_orig:
+					if y not in years:
+						count = src.get_count(datasets.iloc[i]["TableType"], y, agency=agency, force=True)
+						if count>0:
+							years = [x if x!=year else y for x in years]
+							table = src.load(datasets.iloc[i]["TableType"], y, 
+										agency=agency, pbar=False, 
+										sortby="date",
+										nrows=max_count if datasets.iloc[i]["DataType"] not in ["CSV","Excel"] else None)
+							break
 				else:
-					assert len(table.table)>0
+					if len(table.table)==0 and has_outages and \
+						(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
+						pass
+					else:
+						raise ValueError("Unable to find data for any year")
+
+			tables.append(table)
 
-				if not pd.isnull(datasets.iloc[i]["date_field"]):
-					if datasets.iloc[i]["date_field"] not in table.table:
-						table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False, nrows=2000)
-					assert datasets.iloc[i]["date_field"] in table.table
-					#assuming a Pandas string dtype('O').name = object is okay too
-					assert (table.table[datasets.iloc[i]["date_field"]].dtype.name in ['datetime64[ns]', 'datetime64[ns, UTC]', 
-																		'datetime64[ms]','period[A-DEC]','period[Y-DEC]','period[Q-DEC]',
-																		'period[M]']) or \
-						    table.table[datasets.iloc[i]["date_field"]].apply(lambda x: type(x) in [pd.Timestamp,pd.Period]).all()
-					dts = table.table[datasets.iloc[i]["date_field"]]
-					dts = dts[dts.notnull()]
-					# New Orleans complaints dataset has many empty dates
-					# "Seattle and Minneapolis starts with bad date data"
-					if len(dts)>0 or srcName not in ["Seattle","New Orleans",'Minneapolis'] or \
-						datasets.iloc[i]["TableType"] not in [TableType.COMPLAINTS, TableType.INCIDENTS]:
-						assert len(dts) > 0   # If not, either all dates are bad or number of rows requested needs increased
-						assert dts.iloc[0].year <= datetime.now().year
-				if not pd.isnull(datasets.iloc[i]["agency_field"]):
-					assert datasets.iloc[i]["agency_field"] in table.table
+		if future_error:
+			continue
 
-				# Adding a pause here to prevent issues with requesting from site too frequently
-				sleep(sleep_time)
+		for year in years:
+			print(f"Testing for year {year}")
 
-		if loghtml:
-			log_errors_to_file(caught_exceptions, caught_exceptions_warn)
-		else:
-			if len(caught_exceptions)==1:
-				raise caught_exceptions[0]
-			elif len(caught_exceptions)>0:
-				msg = f"{len(caught_exceptions)} URL errors encountered:\n"
-				for e in caught_exceptions:
-					msg += "\t" + e.args[0] + "\n"
-				raise OPD_MultipleErrors(msg)
-
-			for e in caught_exceptions_warn:
-				warnings.warn(str(e))
-
-	def test_get_count(self, csvfile, source, last, skip, loghtml):
-		get_datasets(csvfile)
-
-		print("Testing Socrata source")
-		src = data.Source("Richmond")
-		loader = data_loaders.Socrata(src.datasets.iloc[0]["URL"], src.datasets.iloc[0]["dataset_id"], date_field=src.datasets.iloc[0]["date_field"])  
-		year = 2021
-		assert loader.get_count(year=year) == src.get_count(year=year, table_type=src.datasets.iloc[0]["TableType"])
-		year = [2020,2022]
-		assert loader.get_count(year=year) == src.get_count(year=year, table_type=src.datasets.iloc[0]["TableType"])
-
-		print("Testing CKAN source")
-		src = data.Source("Virginia")
-		loader = data_loaders.Ckan(src.datasets.iloc[0]["URL"], src.datasets.iloc[0]["dataset_id"], date_field=src.datasets.iloc[0]["date_field"])  
-		year = 2021
-		assert loader.get_count(year=year) == src.get_count(year=year)
-		year = [2020,2022]
-		assert loader.get_count(year=year) == src.get_count(year=year)
-
-		agency = "Arlington County Police Department"
-		opt_filter = '"' + src.datasets.iloc[0]["agency_field"] + '"' + " = '" + agency + "'"
-		year = 2021
-		assert src.get_count(year=year, agency=agency) == loader.get_count(year=year, opt_filter=opt_filter)
-
-		print("Testing ArcGIS source")
-		src = data.Source("Charlotte-Mecklenburg")
-		count = src.get_count(year="NONE", table_type="EMPLOYEE")
-
-		url = "https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/16/"
-		gis = data_loaders.Arcgis(url)
-		assert count == gis.get_count()
+			table = tables[years.index(year)]
+			if table is None: # Data could not be loaded
+				continue
+
+			if len(table.table)==0 and has_outages and \
+				(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
+				caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
+				continue
+			else:
+				assert len(table.table)>0
 
-		print("Testing CSV source")
-		src = data.Source("Denver")
+			if table.date_field == None or datasets.iloc[i]["DataType"]==DataType.EXCEL.value or \
+				table.date_field.lower()=="year":
+				continue
 
-		url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
-		loader = data_loaders.Csv(url, date_field="INCIDENT_DATE")
+			dts = table.table[table.date_field]
+			# Remove all non-datestamps
+			dts = dts[dts.apply(lambda x: isinstance(x,pd.Timestamp) or isinstance(x,pd.Period))].convert_dtypes()
+			try:
+				dts = dts.sort_values(ignore_index=True)
+			except TypeError as e:
+				if re.search(r"not supported between instances of '(Timestamp|Period)' and '(Timestamp|Period)'", str(e)):
+					dts = dts[dts.apply(lambda x: isinstance(x,pd.Timestamp))]
+					dts = dts.sort_values(ignore_index=True)
+				else:
+					raise
 
-		count = src.get_count(table_type="OFFICER-INVOLVED SHOOTINGS", force=True)
+			all_years = dts.dt.year.unique().tolist()
 			
-		assert loader.get_count() == count
+			try:
+				assert len(all_years) == 1
+			except AssertionError as e:
+				# Some datasets filter by local time but return
+				# UTC time
+				# Until this is solved more elegantly, removing years between {year}-01-01 00:00:00
+				# and {year}-01-01 08:00:00
+				dts = dts[(dts < f"{year+1}-01-01 00:00:00") | (dts > f"{year+1}-01-01 08:00:00")]
+				all_years = dts.dt.year.unique().tolist()
+				assert len(all_years) == 1
+			except:
+				raise(e)
+			assert all_years[0] == year
 
-		print("Testing Excel source")
-		src = data.Source("Rutland")
+			if not multi_case:
+				continue
 
-		url = "http://www.rutlandcitypolice.com/app/download/5136813/ResponseToResistance+2015-2017.xls"
-		loader = data_loaders.Excel(url, date_field="Date")
+			if "month" in table.date_field.lower() or "year" in table.date_field.lower() or "yr" in table.date_field.lower():
+				# Cannot currently filter only by month/year
+				continue
+			
+			start_date = str(year-1) + "-12-29"
+			stop_date = datetime.strftime(dts.iloc[0], "%Y-%m-%d")
 
-		count = src.get_count(table_type="USE OF FORCE", force=True)
+			try:
+				table_start = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
+												agency=agency, pbar=False)
+			except ValueError as e:
+				if str(e).startswith('Year range cannot contain the year corresponding to a single year dataset'):
+					start_date  = str(year) + "-01-01"
+					table_start = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
+												agency=agency, pbar=False)
+				else:
+					raise
+			except DateFilterException as e:
+				continue
+
+			sleep(sleep_time)
+			dts_start = table_start.table[table.date_field]
+			dts_start = dts_start[dts_start.apply(lambda x: isinstance(x,pd._libs.tslibs.timestamps.Timestamp))].convert_dtypes()
+			dts_start = dts_start.sort_values(ignore_index=True, na_position="first")
+
+			# If this isn't true then the stop date is too early
+			assert dts_start.iloc[-1].year == year
+
+			# Find first value date in year
+			dts_start = dts_start[dts_start.dt.year == year]
+			try:
+				assert dts.iloc[0] == dts_start.iloc[0]
+			except AssertionError as e:
+				# See comments in above try/except
+				assert dts.iloc[0].tz_localize(None) <= datetime.strptime(f"{year}-01-01 08:00:00", "%Y-%m-%d %H:%M:%S")
+			except:
+				raise(e)
 			
-		assert loader.get_count(force=True) == count
+			if len(table.table) == max_count:
+				# Whole dataset was not read. Don't compare to latest data in the year
+				continue
 
-		print("Testing Carto source")
-		src = data.Source("Philadelphia")
-		url = "phl"
-		dataset = "car_ped_stops"
-		date_field = "datetimeoccur"
-		loader = data_loaders.Carto(url, dataset, date_field)  
-		year = 2021
-		assert loader.get_count(year=year) == src.get_count(year=year, table_type=TableType.STOPS)
-		year = [2020,2022]
-		assert loader.get_count(year=year) == src.get_count(year=year, table_type=TableType.STOPS)
+			start_date = datetime.strftime(dts.iloc[-1], "%Y-%m-%d")
+			stop_date  = str(year+1) + "-01-10"  
 
-	
-	def test_get_years_to_check(self, csvfile, source, last, skip, loghtml):
-		assert data._get_years_to_check([2020], cur_year=2023, force=True, isfile=False) == []
-		assert data._get_years_to_check([2022], cur_year=2023, force=False, isfile=True) == []
-		assert data._get_years_to_check([2022, 2020], cur_year=2023, force=False, isfile=False) == [2023]
-		assert data._get_years_to_check([2020, 2021], cur_year=2023, force=True, isfile=True) == [2022, 2023]
-		assert data._get_years_to_check([2020, 2021], cur_year=2023, force=True, isfile=False) == [2022, 2023]
-	
-	
-	def test_load_gen(self, csvfile, source, last, skip, loghtml):
-		datasets = [
-			("Virginia",2020,"STOPS", 2000, "Fairfax County Police Department"), # CKAN
-			("Philadelphia", 2021, "STOPS", 1000),  # Carto
-			("Richmond","MULTIPLE","OFFICER-INVOLVED SHOOTINGS", 5), # Socrata
-			("Fairfax County",2016,"ARRESTS", 1000),  # ArcGIS
-			("Norristown", 2016, "USE OF FORCE",100), # Excel
-			("Denver", "MULTIPLE", "OFFICER-INVOLVED SHOOTINGS", 50) # CSV
-			] 
-
-		for ds in datasets:
-			src = data.Source(ds[0])
-			agency = ds[4] if len(ds)>4 else None
-			max_iter = 10
-			df = src.load(ds[2], ds[1], agency=agency, nrows=max_iter*ds[3]).table
-			with warnings.catch_warnings():
-				warnings.filterwarnings("ignore",category=RuntimeWarning)
-				df = df.convert_dtypes()
-
-			offset = 0
-			k = 0
-			for t in src.load_iter(ds[2], ds[1], nbatch=ds[3], force=True, agency=agency):
-				df_cur = df.iloc[offset:offset+len(t.table)].reset_index(drop=True)
-				df2 = t.table.copy()
-				if set(df.columns)!=set(df2.columns):
-					# Expecting that a column was not returned because it is empty in the subset requested in this iteration
-					assert len(df2.columns)<len(df.columns)
-					missing_columns = list(set(df.columns).difference(set(df2.columns)))
-					for col in missing_columns:
-						assert df_cur[col].isnull().all()
-						df_cur.drop(columns=col, inplace=True)
-				# Assure columns are in proper order
-				assert set(df_cur.columns)==set(df2.columns)
-				df2 = df2[df_cur.columns]
-				# Ensure that dtypes match
-				df2 = df2.astype(df_cur.dtypes.to_dict())
-				assert df2.equals(df_cur)
-				offset+=len(t.table)
-				k+=1
-				if k>=max_iter:
-					break
+			try:
+				table_stop = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
+												agency=agency, pbar=False)
+			except ValueError as e:
+				if str(e).startswith('Year range cannot contain the year corresponding to a single year dataset'):
+					stop_date  = str(year) + "-12-31"  
+					table_stop = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
+												agency=agency, pbar=False)
+				else:
+					raise
+			sleep(sleep_time)
+			dts_stop = table_stop.table[table.date_field]
 
+			dts_stop = dts_stop[dts_stop.apply(lambda x: not isinstance(x,str))]
+			try:
+				dts_stop = dts_stop.sort_values(ignore_index=True)
+			except TypeError as e:
+				dts_stop = dts_stop[dts_stop.apply(lambda x: isinstance(x,pd.Timestamp))]
+				dts_stop = dts_stop.sort_values(ignore_index=True)
+
+			# If this isn't true then the start date is too late
+			assert dts_stop.iloc[0].year == year
+
+			# Find last value date in year
+			dts_stop = dts_stop[dts_stop.dt.year == year]
+			assert dts.iloc[-1] == dts_stop.iloc[-1]
 
-def can_be_limited(data_type, url):
-	if (data_type == DataType.CSV and ".zip" in url):
-		return False
-	elif data_type in [DataType.ArcGIS, DataType.SOCRATA, DataType.CSV, DataType.EXCEL, DataType.CARTO, DataType.CKAN]:
-		return True
+	if loghtml:
+		log_errors_to_file(caught_exceptions, caught_exceptions_warn)
 	else:
-		raise ValueError("Unknown table type")
-	
+		if len(caught_exceptions)==1:
+			raise caught_exceptions[0]
+		elif len(caught_exceptions)>0:
+			msg = f"{len(caught_exceptions)} URL errors encountered:\n"
+			for e in caught_exceptions:
+				msg += "\t" + e.args[0] + "\n"
+			raise OPD_MultipleErrors(msg)
+
+		for e in caught_exceptions_warn:
+			warnings.warn(str(e))
+
+
+def test_source_download_not_limitable(datasets, source, start_idx, skip, query={}):		
+	for i in range(len(datasets)):
+		if skip != None and datasets.iloc[i]["SourceName"] in skip:
+			continue
+		if i < start_idx:
+			continue
+		if source != None and datasets.iloc[i]["SourceName"] != source:
+			continue
+
+		if datasets.iloc[i]["DataType"] == DataType.CSV and ".zip" in datasets.iloc[i]["URL"]:
+			if is_stanford(datasets.iloc[i]["URL"]):
+				# There are a lot of data sets from Stanford, no need to run them all
+				# Just run approximately 10%
+				rnd = random.uniform(0,1)
+				if rnd>0.05:
+					continue
+
+			match = True
+			for k,v in query.items():
+				if datasets.iloc[i][k]!=v:
+					match = False
+					break
+			if not match:
+				continue
+
+			srcName = datasets.iloc[i]["SourceName"]
+			state = datasets.iloc[i]["State"]
+			src = data.Source(srcName, state=state)
+
+			year = datasets.iloc[i]["Year"]
+			table_type = datasets.iloc[i]["TableType"]
+
+			now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
+			print(f"{now} Testing {i+1} of {len(datasets)}: {srcName}, {state} {table_type} table for {year}")
+			try:
+				table = src.load(table_type, year, pbar=False)
+			except OPD_FutureError:
+				continue
+			except:
+				raise
+
+			sleep(sleep_time)
+
+			assert len(table.table)>1
+			if not pd.isnull(table.date_field):
+				assert table.date_field in table.table
+				#assuming a Pandas string dtype('O').name = object is okay too
+				assert (table.table[table.date_field].dtype.name in ['datetime64[ns]', 'datetime64[ms]'])
+			if not pd.isnull(datasets.iloc[i]["agency_field"]):
+				assert datasets.iloc[i]["agency_field"] in table.table
+
 
 def is_stanford(url):
 	return "stanford.edu" in url
 
 def log_errors_to_file(*args):
 	if not os.path.exists(log_folder):
 		os.mkdir(log_folder)
@@ -362,29 +433,23 @@
 							break
 
 				if not skip:
 					f.write(new_line)
 					f.write("\n")
 
 if __name__ == "__main__":
+	from test_utils import get_datasets
 	# For testing
-	tp = TestData()
-	# (self, csvfile, source, last, skip, loghtml)
+	use_changed_rows = False
 	csvfile = None
-	# csvfile = r"..\opd-data\opd_source_table.csv"
-	last = None
-	# last = 922-634+1
+	csvfile = r"..\opd-data\opd_source_table.csv"
+	start_idx = 52
 	skip = None
-	# skip = "Greensboro"
+	skip = "Sacramento,Beloit,Rutland"
 	source = None
-	# source = "Tucson"
+	# source = "Asheville"
 
-	# tp.check_excel_sheets(csvfile, source, last, skip, None) 
-	# tp.test_get_years_to_check(csvfile, source, last, skip, None) 
-	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
-	# tp.test_check_version(csvfile, None, last, skip, None) #
-	tp.test_source_download_limitable(csvfile, source, last, skip, None, query={'DataType':'CKAN'}) 
-	
-	# tp.test_get_count(csvfile, None, last, skip, None)
-	# tp.test_load_gen(csvfile, source, last, skip, None) 
-	
+	datasets = get_datasets(csvfile, use_changed_rows)
+
+	test_load_year(datasets, source, start_idx, skip, False) 
+	start_idx = 0
+	test_source_download_not_limitable(datasets, source, start_idx, skip)
```

### Comparing `openpolicedata-0.6/tests/test_opd_data2.py` & `openpolicedata-0.7/tests/test_opd_data2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from datetime import datetime
 from time import sleep
 import warnings
 import os
 import pandas as pd
 import pytest
 
+from test_utils import check_for_dataset
+
 sleep_time = 0.1
 log_filename = f"pytest_url_errors_{datetime.now().strftime('%Y%m%d_%H')}.txt"
 log_folder = os.path.join(".","data/test_logs")
 
 # Set Arcgis data loader to validate queries with arcgis package if installed
 opd.data_loaders._verify_arcgis = True
 
@@ -36,188 +38,177 @@
 warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
 multi_states = ['Connecticut','New York','Virginia']
 multi_tables = ['TRAFFIC STOPS','TRAFFIC CITATIONS','STOPS']
 multi_years = [MULTI,MULTI,MULTI]
 multi_partial = ["Hartford",'Buffalo',"Arlington"]
 
-def get_datasets(csvfile):
-    if csvfile != None:
-        datasets.datasets = datasets._build(csvfile)
-
-    return datasets.datasets
-
-class TestData:
-	def test_get_years(self, csvfile, source, last, skip, loghtml, query={}):
-		if last == None:
-			last = float('inf')
-		datasets = get_datasets(csvfile)
-		caught_exceptions = []
-		caught_exceptions_warn = []
-		if skip != None:
-			skip = skip.split(",")
-			skip = [x.strip() for x in skip]
-
-		already_ran = []
-		for i in range(len(datasets)):
-			if source != None and datasets.iloc[i]["SourceName"] != source:
-				continue
-			if skip != None and datasets.iloc[i]["SourceName"] in skip:
+def test_get_years(datasets, source, start_idx, skip, loghtml, query={}):
+	caught_exceptions = []
+	caught_exceptions_warn = []
+
+	already_ran = []
+	for i in range(len(datasets)):
+		if source != None and datasets.iloc[i]["SourceName"] != source:
+			continue
+		if skip != None and datasets.iloc[i]["SourceName"] in skip:
+			continue
+		if i < start_idx:
+			continue
+		if is_filterable(datasets.iloc[i]["DataType"]) or datasets.iloc[i]["Year"] != MULTI or \
+			datasets.iloc[i]["DataType"] == DataType.EXCEL.value:  # If Excel, we can possibly check
+			srcName = datasets.iloc[i]["SourceName"]
+			state = datasets.iloc[i]["State"]
+
+			match = True
+			for k,v in query.items():
+				if datasets.iloc[i][k]!=v:
+					match = False
+					break
+			if not match:
 				continue
-			if i < len(datasets) - last:
+
+			if (srcName, state, datasets.iloc[i]["TableType"]) in already_ran:
 				continue
-			if is_filterable(datasets.iloc[i]["DataType"]) or datasets.iloc[i]["Year"] != MULTI or \
-				datasets.iloc[i]["DataType"] == DataType.EXCEL.value:  # If Excel, we can possibly check
-				srcName = datasets.iloc[i]["SourceName"]
-				state = datasets.iloc[i]["State"]
-
-				match = True
-				for k,v in query.items():
-					if datasets.iloc[i][k]!=v:
-						match = False
-						break
-				if not match:
-					continue
-
-				if (srcName, state, datasets.iloc[i]["TableType"]) in already_ran:
-					continue
-
-				src = data.Source(srcName, state=state)
-
-				table_print = datasets.iloc[i]["TableType"]
-				now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-				print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
 
-				if datasets.iloc[i]["DataType"] == DataType.EXCEL.value:
+			src = data.Source(srcName, state=state)
+
+			table_print = datasets.iloc[i]["TableType"]
+			now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
+			print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
+
+			if datasets.iloc[i]["DataType"] == DataType.EXCEL.value:
+				if pd.notnull(datasets.iloc[i]['dataset_id']) and ';' in datasets.iloc[i]['dataset_id']:
+					# Multi-dataset table
+					if pd.isnull(datasets.iloc[i]['date_field']):
+						continue
+				else:
 					loader = opd.data_loaders.Excel(datasets.iloc[i]["URL"])
 					has_year_sheets = loader._Excel__get_sheets()[1]
 					if not has_year_sheets:
 						continue				
 
-				already_ran.append((srcName, state, datasets.iloc[i]["TableType"]))
+			already_ran.append((srcName, state, datasets.iloc[i]["TableType"]))
 
-				try:
-					years = src.get_years(datasets.iloc[i]["TableType"], force=True)
-				except warn_errors as e:
-					e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
-					caught_exceptions_warn.append(e)
-					continue
-				except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
-					# Catch exceptions related to URLs not functioning
-					e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
-					caught_exceptions.append(e)
-					continue
-				except:
-					raise
+			try:
+				years = src.get_years(datasets.iloc[i]["TableType"], force=True)
+			except warn_errors as e:
+				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+				caught_exceptions_warn.append(e)
+				continue
+			except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
+				# Catch exceptions related to URLs not functioning
+				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+				caught_exceptions.append(e)
+				continue
+			except:
+				raise
 
-				if len(years)==0 and has_outages and \
-					(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
-					caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
-					continue
+			if len(years)==0 and has_outages and \
+				(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
+				caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
+				continue
 
-				if datasets.iloc[i]["Year"] != MULTI:
-					assert datasets.iloc[i]["Year"] in years
-				else:
-					assert len(years) > 0
+			if datasets.iloc[i]["Year"] != MULTI:
+				assert datasets.iloc[i]["Year"] in years
+			else:
+				assert len(years) > 0
 
-				# Adding a pause here to prevent issues with requesting from site too frequently
-				sleep(0.1)
+			# Adding a pause here to prevent issues with requesting from site too frequently
+			sleep(0.1)
 
-		if loghtml:
-			log_errors_to_file(caught_exceptions, caught_exceptions_warn)
-		else:
-			if len(caught_exceptions)==1:
-				raise caught_exceptions[0]
-			elif len(caught_exceptions)>0:
-				msg = f"{len(caught_exceptions)} URL errors encountered:\n"
-				for e in caught_exceptions:
-					msg += "\t" + e.args[0] + "\n"
-				raise OPD_MultipleErrors(msg)
-
-			for e in caught_exceptions_warn:
-				warnings.warn(str(e))
-
-
-	def test_get_agencies(self, csvfile, source, last, skip, loghtml):
-		if last == None:
-			last = float('inf')
-		datasets = get_datasets(csvfile)
-		if skip != None:
-			skip = skip.split(",")
-			skip = [x.strip() for x in skip]
-			
-		for i in range(len(datasets)):
-			if skip != None and datasets.iloc[i]["SourceName"] in skip:
-				continue
-			if i < len(datasets) - last:
-				continue
-			if source != None and datasets.iloc[i]["SourceName"] != source:
-				continue
+	if loghtml:
+		log_errors_to_file(caught_exceptions, caught_exceptions_warn)
+	else:
+		if len(caught_exceptions)==1:
+			raise caught_exceptions[0]
+		elif len(caught_exceptions)>0:
+			msg = f"{len(caught_exceptions)} URL errors encountered:\n"
+			for e in caught_exceptions:
+				msg += "\t" + e.args[0] + "\n"
+			raise OPD_MultipleErrors(msg)
+
+		for e in caught_exceptions_warn:
+			warnings.warn(str(e))
 
-			if is_filterable(datasets.iloc[i]["DataType"]) or datasets.iloc[i]["Agency"] != MULTI:
-				srcName = datasets.iloc[i]["SourceName"]
-				state = datasets.iloc[i]["State"]
-				src = data.Source(srcName, state=state)
-
-				table_print = datasets.iloc[i]["TableType"]
-				now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-				print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
-
-				try:
-					agencies = src.get_agencies(datasets.iloc[i]["TableType"], year=datasets.iloc[i]["Year"])
-				except OPD_MinVersionError: continue
-				except: raise
 
-				if datasets.iloc[i]["Agency"] != MULTI:
-					assert [datasets.iloc[i]["Agency"]] == agencies
+def test_get_agencies(datasets, source, start_idx, skip):
+		
+	for i in range(len(datasets)):
+		if skip != None and datasets.iloc[i]["SourceName"] in skip:
+			continue
+		if i < start_idx:
+			continue
+		if source != None and datasets.iloc[i]["SourceName"] != source:
+			continue
+
+		if is_filterable(datasets.iloc[i]["DataType"]) or datasets.iloc[i]["Agency"] != MULTI:
+			srcName = datasets.iloc[i]["SourceName"]
+			state = datasets.iloc[i]["State"]
+			src = data.Source(srcName, state=state)
+
+			table_print = datasets.iloc[i]["TableType"]
+			now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
+			print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
+
+			try:
+				agencies = src.get_agencies(datasets.iloc[i]["TableType"], year=datasets.iloc[i]["Year"])
+			except ValueError as e:
+				if 'Inputs must filter for a single source' in str(e):
+					agencies = src.get_agencies(datasets.iloc[i]["TableType"], year=datasets.iloc[i]["Year"], url_contains=datasets.iloc[i]["URL"])
 				else:
-					assert len(agencies) > 0
+					raise
+			except OPD_MinVersionError: continue
+			except: raise
+
+			if datasets.iloc[i]["Agency"] != MULTI:
+				assert [datasets.iloc[i]["Agency"]] == agencies
+			else:
+				assert len(agencies) > 0
 
-				# Adding a pause here to prevent issues with requesting from site too frequently
-				sleep(sleep_time)
+			# Adding a pause here to prevent issues with requesting from site too frequently
+			sleep(sleep_time)
 
 
-	def test_multi_agency_list(self, csvfile, source, last, skip, loghtml):
-		datasets = get_datasets(csvfile)
-		for i in range(len(datasets)):
-			if is_filterable(datasets.iloc[i]["DataType"]) and datasets.iloc[i]["Agency"] == MULTI:
-				assert any([datasets.iloc[i]['State']==x and datasets.iloc[i]['TableType']==y and datasets.iloc[i]['Year']==z for 
-							x,y,z in zip(multi_states, multi_tables,multi_years)])
+def test_multi_agency_list(datasets):
+	for i in range(len(datasets)):
+		if is_filterable(datasets.iloc[i]["DataType"]) and datasets.iloc[i]["Agency"] == MULTI:
+			assert any([datasets.iloc[i]['State']==x and datasets.iloc[i]['TableType']==y and datasets.iloc[i]['Year']==z for 
+						x,y,z in zip(multi_states, multi_tables,multi_years)])
 
 
-	@pytest.mark.parametrize('state,table_type,year,partial',[(x,y,z,a) for x,y,z,a in zip(multi_states, multi_tables,multi_years,multi_partial)])
-	def test_get_agencies_name_match(self, csvfile, source, last, skip, loghtml, state, table_type, year, partial):
+@pytest.mark.parametrize('state,table_type,year,partial',[(x,y,z,a) for x,y,z,a in zip(multi_states, multi_tables,multi_years,multi_partial)])
+def test_get_agencies_name_match(state, table_type, year, partial):
+	if check_for_dataset(state, table_type):
 		src = data.Source(state)
 		try:
 			agencies = src.get_agencies(partial_name=partial, table_type=table_type, year=year)
 		except OPD_MinVersionError:
 			return
 		except Exception as e:
 			raise
 
 		assert len(agencies) > 1
-				
-				
-	def test_agency_filter(self, csvfile, source, last, skip, loghtml):
-		if last == None:
-			last = float('inf')
-		get_datasets(csvfile)
+			
+			
+def test_agency_filter():
+	if check_for_dataset('New York', 'TRAFFIC CITATIONS'):
 		src = data.Source("New York")
 		agency="BUFFALO POLICE DEPT"
 		# For speed, set private limit parameter so that only a single entry is requested
 		table = src.load('TRAFFIC CITATIONS', 2021, agency=agency, pbar=False, nrows=100)
 		
 		assert len(table.table)==100
 		assert table.table[table.agency_field].nunique()==1
 		assert table.table.iloc[0][table.agency_field] == agency
 
 
-	def test_to_csv(self, csvfile, source, last, skip, loghtml):
+def test_to_csv():
+	if check_for_dataset('New York', 'TRAFFIC CITATIONS'):
 		src = data.Source("New York")
-		get_datasets(csvfile)
 		agency="BUFFALO POLICE DEPT"
 		year = 2021
 		table = src.load('TRAFFIC CITATIONS', 2021, agency=agency, pbar=False, nrows=100)
 
 		table.to_csv()
 
 		filename = table.get_csv_filename()
@@ -267,23 +258,29 @@
 							break
 
 				if not skip:
 					f.write(new_line)
 					f.write("\n")
 
 if __name__ == "__main__":
+	from test_utils import get_datasets
 	# For testing
-	tp = TestData()
-	# (self, csvfile, source, last, skip, loghtml)
+	# (csvfile, source, last, skip, loghtml)
+
+	use_changed_rows = False
+
 	csvfile = None
-	# csvfile = os.path.join("..","opd-data","opd_source_table.csv")
-	last = None
-	last = 922-896+1
+	csvfile = os.path.join("..","opd-data","opd_source_table.csv")
+	start_idx = 876
 	source = None
-	# source = "Bloomington"
+	# source = "Burlington"
 	skip = None
+	skip = "Sacramento,Beloit,Rutland"
+	
+	datasets = get_datasets(csvfile, use_changed_rows)
+
 	# skip = "Corona"
-	# tp.test_get_agencies(csvfile, None, None, skip, None)
-	# tp.test_get_agencies_name_match(csvfile, None, last, skip, None)
-	# tp.test_agency_filter(csvfile, None, None, skip, None)
-	# tp.test_to_csv(csvfile, None, None, skip, None)
-	tp.test_get_years(csvfile, source, last, skip, None, query={'DataType':'CKAN'})
+	# test_get_agencies(datasets, source, start_idx, skip)
+	# test_get_agencies_name_match(datasets, None, last, skip, None)
+	# test_agency_filter(datasets, None, None, skip, None)
+	# test_to_csv(datasets, None, None, skip, None)
+	test_get_years(datasets, source, start_idx, skip, None)
```

### Comparing `openpolicedata-0.6/tests/test_opd_data3.py` & `openpolicedata-0.7/tests/test_opd_data1.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,396 +1,413 @@
 import pytest
 
 if __name__ == "__main__":
 	import sys
 	sys.path.append('../openpolicedata')
 from openpolicedata import data, data_loaders
-from openpolicedata import datasets
-from openpolicedata.defs import MULTI, DataType
+from openpolicedata.defs import DataType, TableType
 from openpolicedata.exceptions import OPD_DataUnavailableError, OPD_TooManyRequestsError,  \
-	OPD_MultipleErrors, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError, \
-	DateFilterException
-import random
+	OPD_MultipleErrors, OPD_arcgisAuthInfoError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError
+import openpolicedata as opd
 from datetime import datetime
-from datetime import timedelta
 import pandas as pd
 from time import sleep
 import warnings
 import os
-import re
+
+import pathlib
+import sys
+sys.path.append(pathlib.Path(__file__).parent.resolve())
+from test_utils import check_for_dataset
+
+sleep_time = 0.1
 
 # Set Arcgis data loader to validate queries with arcgis package if installed
 data_loaders._verify_arcgis = True
 
-sleep_time = 0.1
 log_filename = f"pytest_url_errors_{datetime.now().strftime('%Y%m%d_%H')}.txt"
 log_folder = os.path.join(".","data/test_logs")
 
 outages_file = os.path.join("..","opd-data","outages.csv")
 # if has_outages:=os.path.exists(outages_file):
 has_outages=os.path.exists(outages_file)
 if has_outages:
 	outages = pd.read_csv(outages_file)
 else:
 	try:
 		outages = pd.read_csv('https://raw.githubusercontent.com/openpolicedata/opd-data/main/outages.csv')
 		has_outages = True
 	except:
 		pass
-	
+
 warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
-def get_datasets(csvfile):
-    if csvfile != None:
-        datasets.datasets = datasets._build(csvfile)
-
-    return datasets.datasets
-
-class TestData:
-	@pytest.mark.slow(reason="This is a slow test that should be run before a major commit.")
-	def test_load_year(self, csvfile, source, last, skip, loghtml, query={}):
-		max_count = 1e5
-		if last == None:
-			last = float('inf')
-		datasets = get_datasets(csvfile)
-		# Test that filtering for a year works at the boundaries
-		if skip != None:
-			skip = skip.split(",")
-			skip = [x.strip() for x in skip]
-			
-		caught_exceptions = []
-		caught_exceptions_warn = []
-		already_run = []
-		for i in range(len(datasets)):
-			if skip != None and datasets.iloc[i]["SourceName"] in skip:
-				continue
-			if i < len(datasets) - last:
-				continue
-			if source != None and datasets.iloc[i]["SourceName"] != source:
-				continue
+def user_request_skip(datasets, i, skip, start_idx, source):
+	# Skip sources that the user requested to skip
+	if skip and datasets.iloc[i]["SourceName"] in skip:
+		return True
+	# User requested to start at start_idx
+	if i<start_idx:
+		return True
+	if source != None and datasets.iloc[i]["SourceName"] != source:
+		return True
+	
+	return False
 
+def check_table_type_warning(all_datasets):
+	sources = all_datasets.copy().iloc[0]
+	sources["TableType"] = "TEST"
+	with pytest.warns(UserWarning):
+		data.Table(sources)
+
+def test_check_version(datasets):
+	ds = datasets.iloc[0].copy()
+	# Set min_version to create error
+	ds["min_version"] = "-1"
+	with pytest.raises(OPD_FutureError):
+		data._check_version(ds)
+
+	ds["min_version"] = "100000.0"
+	with pytest.raises(OPD_MinVersionError):
+		data._check_version(ds)
+
+	# These should pass
+	ds["min_version"] = "0.0"
+	data._check_version(ds)
+	ds["min_version"] = pd.NA
+	data._check_version(ds)
+
+def test_single_year_filter():
+	if check_for_dataset('Phoenix', opd.defs.TableType.CALLS_FOR_SERVICE):
+		src = data.Source('Phoenix')
+		year = 2017
+		dataset, filter_by_year = src._Source__filter_for_source(opd.defs.TableType.CALLS_FOR_SERVICE, year, None)
+		assert not filter_by_year
+		assert dataset['Year']==year
+		assert dataset['TableType']==opd.defs.TableType.CALLS_FOR_SERVICE
+
+def test_single_year_range_filter():
+	if check_for_dataset('Phoenix', opd.defs.TableType.CALLS_FOR_SERVICE):
+		src = data.Source('Phoenix')
+		with pytest.raises(ValueError, match="There are no sources matching"):
+			src._Source__filter_for_source(opd.defs.TableType.CALLS_FOR_SERVICE, [2017,2018], None)
+
+@pytest.mark.parametrize('year, exp_filt_by_year', [(2017,True), (opd.defs.MULTI,False)])
+def test_multi_year_filter(year,exp_filt_by_year):
+	if check_for_dataset('Norristown', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Norristown')
+		dataset, filter_by_year = src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, None)
+		assert filter_by_year == exp_filt_by_year
+		assert dataset['Year']==opd.defs.MULTI
+		assert dataset['TableType']==opd.defs.TableType.USE_OF_FORCE
+
+def test_multi_year_range_filter_includes_single_year():
+	if check_for_dataset('Norristown', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Norristown')
+		year = [2016,2018]
+		with pytest.raises(ValueError, match="Year range cannot contain the year corresponding to a single year"):
+			src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, None)
+
+def test_bad_year_range():
+	if check_for_dataset('Norristown', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Norristown')
+		year = [2016,2018, 2017]
+		with pytest.raises(ValueError, match="year input must either be a single year or a list containing a start and stop year"):
+			src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, None)
+
+@pytest.mark.parametrize('year, url_contains', [(2019, "APDUseOfForce/FeatureServer/0"), 
+												([2018,2019], "APDUseOfForce/FeatureServer/0"), (2021, "APD_UseOfForce2021/FeatureServer/0")])
+def test_multiple_multiple_year_filter(all_datasets, year, url_contains):
+	if check_for_dataset('Asheville', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Asheville')
+		dataset, filter_by_year = src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, None)
+		assert filter_by_year
+		assert dataset['Year']==opd.defs.MULTI
+		assert dataset['TableType']==opd.defs.TableType.USE_OF_FORCE
+		assert url_contains in dataset['URL']
+
+@pytest.mark.parametrize('year, url_contains, url_contains_test', [(2020, None, 'LMPD_STOPS_DATA_(2)'), 
+												(2021, None, 'LMPD_STOP_DATA_2021'),
+												(2021, 'LMPD_STOPS_DATA_(2)', 'LMPD_STOPS_DATA_(2)')])
+def test_overlapping_multi_and_single(all_datasets, year, url_contains, url_contains_test):
+	if check_for_dataset('Louisville', opd.defs.TableType.TRAFFIC):
+		src = data.Source('Louisville')
+		dataset, filter_by_year = src._Source__filter_for_source(opd.defs.TableType.TRAFFIC, year, url_contains)
+		assert url_contains_test in dataset['URL']
+
+@pytest.mark.parametrize('year', [2020, [2020,2021], opd.defs.MULTI])
+def test_multiple_bad_multiple_year_filter(all_datasets, year):
+	if check_for_dataset('Asheville', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Asheville')
+		with pytest.raises(ValueError, match="There is more than one source matching "):
+			src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, None)
+
+@pytest.mark.parametrize('year, exp_filt_by_year', [([2021,2022], True), (opd.defs.MULTI, False)])
+def test_url_contains(all_datasets, year, exp_filt_by_year):
+	if check_for_dataset('Asheville', opd.defs.TableType.USE_OF_FORCE):
+		src = data.Source('Asheville')
+		url_contains = "APDUseOfForce/FeatureServer/0"
+		dataset, filter_by_year = src._Source__filter_for_source(opd.defs.TableType.USE_OF_FORCE, year, url_contains)
+		assert filter_by_year == exp_filt_by_year
+		assert dataset['Year']==opd.defs.MULTI
+		assert dataset['TableType']==opd.defs.TableType.USE_OF_FORCE
+		assert url_contains in dataset['URL']
+
+
+def test_offsets_and_nrows():
+	if check_for_dataset('Philadelphia', opd.defs.TableType.SHOOTINGS):
+		src = data.Source("Philadelphia")
+		df = src.load(year=2019, table_type="Officer-Involved Shootings").table
+		offset = 1
+		nrows = len(df)-2
+		df_offset = src.load(year=2019, table_type="Officer-Involved Shootings", offset=offset, nrows=nrows).table
+		assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
+
+def check_excel_sheets(datasets, source, start_idx, skip):
+	for i in range(len(datasets)):
+		if user_request_skip(datasets, i, skip, start_idx, source):
+			continue
+
+		if datasets.iloc[i]["DataType"]!=DataType.EXCEL:
+			continue
+
+		srcName = datasets.iloc[i]["SourceName"]
+		state = datasets.iloc[i]["State"]
+		src = data.Source(srcName, state=state)
+
+		table_print = datasets.iloc[i]["TableType"]
+		now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
+		print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
+
+		excel = src._Source__get_loader(datasets.iloc[i]["DataType"], datasets.iloc[i]["URL"], datasets.iloc[i]["query"],
+				dataset_id=datasets.iloc[i]["dataset_id"])
+		sheets, has_year_sheets = excel._Excel__get_sheets()
+
+		if has_year_sheets:
+			# Ensure that load works
+			src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False)
+		else:
+			excel._Excel__check_sheet(sheets)
+
+
+def test_source_download_limitable(datasets, source, start_idx, skip, loghtml, query={}):
+	num_stanford = 0
+	max_num_stanford = 1  # This data is standardized. Probably no need to test more than 1
+	caught_exceptions = []
+	caught_exceptions_warn = []
+		
+	for i in range(len(datasets)):
+		if user_request_skip(datasets, i, skip, start_idx, source):
+			continue
+
+		has_date_field = not pd.isnull(datasets.iloc[i]["date_field"])
+		if can_be_limited(datasets.iloc[i]["DataType"], datasets.iloc[i]["URL"]) or has_date_field:
 			if is_stanford(datasets.iloc[i]["URL"]):
-				# There are a lot of data sets from Stanford, no need to run them all
-				# Just run approximately a small percentage
-				rnd = random.uniform(0,1)
-				if rnd>0.05:
+				num_stanford += 1
+				if num_stanford > max_num_stanford:
 					continue
-
 			match = True
 			for k,v in query.items():
 				if datasets.iloc[i][k]!=v:
 					match = False
 					break
 			if not match:
 				continue
 
 			srcName = datasets.iloc[i]["SourceName"]
 			state = datasets.iloc[i]["State"]
-
-			if datasets.iloc[i]["Agency"] == MULTI and \
-				srcName == "Virginia":
-				# Reduce size of data load by filtering by agency
-				agency = "Henrico Police Department"
-			else:
-				agency = None
+			src = data.Source(srcName, state=state)
 
 			table_print = datasets.iloc[i]["TableType"]
-
-			unique_id = [srcName, state, datasets.iloc[i]["Agency"], table_print]
-			if unique_id in already_run:
-				continue
-			already_run.append(unique_id)
-
 			now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-			print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
+			print(f"{now} Testing {i} of {len(datasets)-1}: {srcName} {table_print} table")
 
-			src = data.Source(srcName, state=state)
+			nrows = 20 if datasets.iloc[i]['DataType']!='Excel' else None
+
+			# Handle cases where URL is required to disambiguate requested dataset
+			ds_filter, _ = src._Source__filter_for_source(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], None, errors=False)
+			url_contains = datasets.iloc[i]['URL'] if isinstance(ds_filter,pd.DataFrame) and len(ds_filter)>1 else None
 
 			try:
-				try:
-					years = src.get_years(datasets.iloc[i]["TableType"])
-				except ValueError as e:
-					if len(e.args)>0 and "Extracting the years" in e.args[0]:
-						# Just test reading in the table and continue
-						table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], 
-										agency=agency, pbar=False)
-						continue
-					else:
-						raise
-				except:
-					raise
+				table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False, nrows=nrows, url_contains=url_contains)
 			except warn_errors as e:
-				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"])
 				caught_exceptions_warn.append(e)
 				continue
 			except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
 				# Catch exceptions related to URLs not functioning
-				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
+				e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"])
 				caught_exceptions.append(e)
 				continue
 			except:
 				raise
 
-			# Adding a pause here to prevent issues with requesting from site too frequently
-			sleep(sleep_time)
-
-			years_orig = years.copy()
-			for y in src.datasets[src.datasets["TableType"] == datasets.iloc[i]["TableType"]]["Year"]:
-				if y != MULTI:
-					years.remove(y)
-
-			if len(years)==0:
-				# Each datasets is annual
-				# Run 1st and last year
-				multi_case = False
-				years = [min(years_orig)]
-				if len(years_orig)>1:
-					years.append(max(years_orig))
-			else:
-				multi_case = True
-				if len(years)>1:
-					# It is preferred to to not use first or last year that start and stop of year are correct
-					years = years[-2:-1]
-				else:
-					years = years[:1]
-
-			tables = []
-			future_error = False
-			for year in years:
-				try:
-					table = src.load(datasets.iloc[i]["TableType"], year, 
-											agency=agency, pbar=False, 
-											sortby="date",
-											nrows=max_count if datasets.iloc[i]["DataType"] not in ["CSV","Excel"] else None)
-				except OPD_FutureError as e:
-					future_error = True
-					break
-				except:
-					raise
-
-				sleep(sleep_time)
-
-				if len(table.table)==0:
-					# Ensure count should have been 0
-					count = src.get_count(datasets.iloc[i]["TableType"], year, agency=agency, force=True)
-					if count!=0:
-						raise ValueError(f"Expected data for year {year} but received none")
-					
-					# There may not be any data for the year requested.
-					for y in years_orig:
-						if y not in years:
-							count = src.get_count(datasets.iloc[i]["TableType"], y, agency=agency, force=True)
-							if count>0:
-								years = [x if x!=year else y for x in years]
-								table = src.load(datasets.iloc[i]["TableType"], y, 
-											agency=agency, pbar=False, 
-											sortby="date",
-											nrows=max_count if datasets.iloc[i]["DataType"] not in ["CSV","Excel"] else None)
-								break
-					else:
-						if len(table.table)==0 and has_outages and \
-							(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
-							pass
-						else:
-							raise ValueError("Unable to find data for any year")
-
-				tables.append(table)
-
-			if future_error:
+			if len(table.table)==0 and has_outages and \
+				(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
+				caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
 				continue
+			else:
+				assert len(table.table)>0
 
-			for year in years:
-				print(f"Testing for year {year}")
-
-				table = tables[years.index(year)]
-
-				if len(table.table)==0 and has_outages and \
-					(outages[["State","SourceName","Agency","TableType","Year"]] == datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]]).all(axis=1).any():
-					caught_exceptions_warn.append(f'Outage continues for {str(datasets.iloc[i][["State","SourceName","Agency","TableType","Year"]])}')
-					continue
-				else:
-					assert len(table.table)>0
-
-				if table.date_field == None or datasets.iloc[i]["DataType"]==DataType.EXCEL.value or \
-					table.date_field.lower()=="year":
-					continue
-
-				dts = table.table[table.date_field]
-				# Remove all non-datestamps
-				dts = dts[dts.apply(lambda x: isinstance(x,pd.Timestamp) or isinstance(x,pd.Period))].convert_dtypes()
-				try:
-					dts = dts.sort_values(ignore_index=True)
-				except TypeError as e:
-					if re.search(r"not supported between instances of '(Timestamp|Period)' and '(Timestamp|Period)'", str(e)):
-						dts = dts[dts.apply(lambda x: isinstance(x,pd.Timestamp))]
-						dts = dts.sort_values(ignore_index=True)
-					else:
-						raise
-
-				all_years = dts.dt.year.unique().tolist()
-				
-				try:
-					assert len(all_years) == 1
-				except AssertionError as e:
-					# Some datasets filter by local time but return
-					# UTC time
-					# Until this is solved more elegantly, removing years between {year}-01-01 00:00:00
-					# and {year}-01-01 08:00:00
-					dts = dts[(dts < f"{year+1}-01-01 00:00:00") | (dts > f"{year+1}-01-01 08:00:00")]
-					all_years = dts.dt.year.unique().tolist()
-					assert len(all_years) == 1
-				except:
-					raise(e)
-				assert all_years[0] == year
-
-				if not multi_case:
-					continue
-
-				if "month" in table.date_field.lower() or "year" in table.date_field.lower() or "yr" in table.date_field.lower():
-					# Cannot currently filter only by month/year
-					continue
-				
-				start_date = str(year-1) + "-12-29"
-				stop_date = datetime.strftime(dts.iloc[0]+timedelta(days=1), "%Y-%m-%d")
-
-				try:
-					table_start = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
-													agency=agency, pbar=False)
-				except ValueError as e:
-					if len(e.args)>0 and e.args[0]=="Currently unable to handle non-year inputs":
-						# The format of the date field does not allow for filtering by date
-						continue
-					else:
-						raise
-				except DateFilterException as e:
-					continue
-				except:
-					raise
-
-				sleep(sleep_time)
-				dts_start = table_start.table[table.date_field]
-				dts_start = dts_start[dts_start.apply(lambda x: isinstance(x,pd._libs.tslibs.timestamps.Timestamp))].convert_dtypes()
-				dts_start = dts_start.sort_values(ignore_index=True, na_position="first")
-
-				# If this isn't true then the stop date is too early
-				assert dts_start.iloc[-1].year == year
-
-				# Find first value date in year
-				dts_start = dts_start[dts_start.dt.year == year]
-				try:
-					assert dts.iloc[0] == dts_start.iloc[0]
-				except AssertionError as e:
-					# See comments in above try/except
-					assert dts.iloc[0].tz_localize(None) <= datetime.strptime(f"{year}-01-01 08:00:00", "%Y-%m-%d %H:%M:%S")
-				except:
-					raise(e)
+			if isinstance(datasets.iloc[i]['dataset_id'], str) and ';' in datasets.iloc[i]['dataset_id']:
+				# A year-long dataset is generated from multiple datasets. Check that whole year is covered
+				# Parse dataset ID to get number of datasets IDs
+				sheets = None
+				dataset_list = datasets.iloc[i]['dataset_id']
+				if '|' in dataset_list:  # dataset names are separated from relative URLs by |
+					dataset_list = dataset_list.split('|')
+					assert len(dataset_list)==2
+					sheets = dataset_list[0].split(';')   # Different sheet names for each dataset are separated by ;. If multiple sheets for a given dataset, separate by &
+					dataset_list = dataset_list[1]
+				dataset_list = dataset_list.split(';')  
 				
-				if len(table.table) == max_count:
-					# Whole dataset was not read. Don't compare to latest data in the year
-					continue
+				table.standardize()
 
-				start_date = datetime.strftime(dts.iloc[-1]-timedelta(days=1), "%Y-%m-%d")
-				stop_date  = str(year+1) + "-01-10"  
+				assert opd.defs.columns.DATE in table.table
+				months = table.table[opd.defs.columns.DATE].dt.month.unique()
+				if len(months)!=12:
+					missing_months = [x for x in range(1,13) if x not in months]
+					if srcName=='Wallkill' and datasets.iloc[i]["Year"]==2016:
+						# Only has last 3 quarters of data
+						missing_months = [x for x in missing_months if x not in [1,2,3]]
+					elif srcName=='Albemarle County' and datasets.iloc[i]["Year"]==2021:
+						# August and Sept data does not have date field
+						missing_months = [x for x in missing_months if x not in [8,9]]
+					for m in missing_months:
+						url = datasets.iloc[i]["URL"] + '/' + dataset_list[m-1].strip()
+						cur_sheet = sheets[min(m-1, len(sheets)-1)] if sheets else None
+						loader = data_loaders.Excel(url, cur_sheet, datasets.iloc[i]["date_field"])
+						df_check = loader.load()
+						assert df_check['DATE'].apply(lambda x: (int(x[:2]) if isinstance(x,str) else x.month) !=m).all()
+
+			if not pd.isnull(datasets.iloc[i]["date_field"]):
+				if datasets.iloc[i]["date_field"] not in table.table:
+					table = src.load(datasets.iloc[i]["TableType"], datasets.iloc[i]["Year"], pbar=False, nrows=2000)
+				assert datasets.iloc[i]["date_field"] in table.table
+				#assuming a Pandas string dtype('O').name = object is okay too
+				assert (table.table[datasets.iloc[i]["date_field"]].dtype.name in ['datetime64[ns]', 'datetime64[ns, UTC]', 
+																	'datetime64[ms]', 'period[Y-DEC]','period[Q-DEC]',
+																	'period[M]']) or \
+						table.table[datasets.iloc[i]["date_field"]].apply(lambda x: type(x) in [pd.Timestamp,pd.Period]).mean()>0.9
+				dts = table.table[datasets.iloc[i]["date_field"]]
+				dts = dts[dts.notnull()]
+				# New Orleans complaints dataset has many empty dates
+				# "Seattle and Minneapolis starts with bad date data"
+				if len(dts)>0 or srcName not in ["Seattle","New Orleans",'Minneapolis'] or \
+					datasets.iloc[i]["TableType"] not in [TableType.COMPLAINTS, TableType.INCIDENTS]:
+					assert len(dts) > 0   # If not, either all dates are bad or number of rows requested needs increased
+					assert dts.iloc[0].year <= datetime.now().year if isinstance(dts.iloc[0], (pd.Timestamp,pd.Period)) else \
+						dts.iloc[1].year <= datetime.now().year
+			if not pd.isnull(datasets.iloc[i]["agency_field"]):
+				assert datasets.iloc[i]["agency_field"] in table.table
 
-				table_stop = src.load(datasets.iloc[i]["TableType"], [start_date, stop_date], 
-												agency=agency, pbar=False)
-				sleep(sleep_time)
-				dts_stop = table_stop.table[table.date_field]
-
-				dts_stop = dts_stop[dts_stop.apply(lambda x: not isinstance(x,str))]
-				dts_stop = dts_stop.sort_values(ignore_index=True)
-
-				# If this isn't true then the start date is too late
-				assert dts_stop.iloc[0].year == year
-
-				# Find last value date in year
-				dts_stop = dts_stop[dts_stop.dt.year == year]
-				assert dts.iloc[-1] == dts_stop.iloc[-1]
+			# Adding a pause here to prevent issues with requesting from site too frequently
+			sleep(sleep_time)
 
-		if loghtml:
-			log_errors_to_file(caught_exceptions, caught_exceptions_warn)
+	if loghtml:
+		log_errors_to_file(caught_exceptions, caught_exceptions_warn)
+	else:
+		if len(caught_exceptions)==1:
+			raise caught_exceptions[0]
+		elif len(caught_exceptions)>0:
+			msg = f"{len(caught_exceptions)} URL errors encountered:\n"
+			for e in caught_exceptions:
+				msg += "\t" + e.args[0] + "\n"
+			raise OPD_MultipleErrors(msg)
+
+		for e in caught_exceptions_warn:
+			warnings.warn(str(e))
+
+@pytest.mark.parametrize("loader, source, table_type, agency, years", [
+	(data_loaders.Socrata, 'Richmond', 'CALLS FOR SERVICE', None, [2021, [2020, 2022]]),
+	(data_loaders.Ckan, 'Virginia', 'STOPS', "Arlington County Police Department", [2021, [2020, 2022]]),
+	(data_loaders.Arcgis, "Charlotte-Mecklenburg", 'EMPLOYEE', None, []),
+	(data_loaders.Csv, 'Denver', "OFFICER-INVOLVED SHOOTINGS", None, []),
+	(data_loaders.Excel, 'Rutland', "USE OF FORCE", None, []),
+	(data_loaders.Carto, "Philadelphia", 'STOPS', None, [2021, [2020, 2022]])
+	])
+def test_get_count(loader, source, table_type, agency, years):
+	if check_for_dataset(source, table_type):
+		print(f"Testing {loader} source")
+		src = opd.Source(source)
+		i = src.datasets["TableType"] == table_type
+		i = i[i].index[0]
+		if pd.notnull(src.datasets.loc[i]["dataset_id"]):
+			loader = loader(src.datasets.loc[i]["URL"], src.datasets.loc[i]["dataset_id"], date_field=src.datasets.loc[i]["date_field"])
 		else:
-			if len(caught_exceptions)==1:
-				raise caught_exceptions[0]
-			elif len(caught_exceptions)>0:
-				msg = f"{len(caught_exceptions)} URL errors encountered:\n"
-				for e in caught_exceptions:
-					msg += "\t" + e.args[0] + "\n"
-				raise OPD_MultipleErrors(msg)
-
-			for e in caught_exceptions_warn:
-				warnings.warn(str(e))
-
-
-	def test_source_download_not_limitable(self, csvfile, source, last, skip, loghtml, query={}):
-		if last == None:
-			last = float('inf')
-		datasets = get_datasets(csvfile)
-		if skip != None:
-			skip = skip.split(",")
-			skip = [x.strip() for x in skip]
-			
-		for i in range(len(datasets)):
-			if skip != None and datasets.iloc[i]["SourceName"] in skip:
-				continue
-			if i < len(datasets) - last:
-				continue
-			if source != None and datasets.iloc[i]["SourceName"] != source:
-				continue
-			if not can_be_limited(datasets.iloc[i]["DataType"], datasets.iloc[i]["URL"]):
-				if is_stanford(datasets.iloc[i]["URL"]):
-					# There are a lot of data sets from Stanford, no need to run them all
-					# Just run approximately 10%
-					rnd = random.uniform(0,1)
-					if rnd>0.05:
-						continue
-
-				match = True
-				for k,v in query.items():
-					if datasets.iloc[i][k]!=v:
-						match = False
-						break
-				if not match:
-					continue
-
-				srcName = datasets.iloc[i]["SourceName"]
-				state = datasets.iloc[i]["State"]
-				src = data.Source(srcName, state=state)
-
-				year = datasets.iloc[i]["Year"]
-				table_type = datasets.iloc[i]["TableType"]
-
-				now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-				print(f"{now} Testing {i+1} of {len(datasets)}: {srcName}, {state} {table_type} table for {year}")
-				try:
-					table = src.load(table_type, year, pbar=False)
-				except OPD_FutureError:
-					continue
-				except:
-					raise
-
-				sleep(sleep_time)
+			loader = loader(src.datasets.loc[i]["URL"], date_field=src.datasets.loc[i]["date_field"])
+		if len(years)==0:
+			assert loader.get_count(force=True) == src.get_count(year=src.datasets.loc[i]['Year'], table_type=table_type, force=True)
+		else: 
+			for year in years:
+				assert loader.get_count(year=year, force=True) == src.get_count(year=year, table_type=table_type, force=True)
 
-				assert len(table.table)>1
-				if not pd.isnull(table.date_field):
-					assert table.date_field in table.table
-					#assuming a Pandas string dtype('O').name = object is okay too
-					assert (table.table[table.date_field].dtype.name in ['datetime64[ns]', 'datetime64[ms]'])
-				if not pd.isnull(datasets.iloc[i]["agency_field"]):
-					assert datasets.iloc[i]["agency_field"] in table.table
+		if agency:
+			opt_filter = '"' + src.datasets.loc[i]["agency_field"] + '"' + " = '" + agency + "'"
+			year = years[0]
+			assert src.get_count(year=year, agency=agency, force=True) == loader.get_count(year=year, opt_filter=opt_filter, force=True)
+
+
+def test_get_years_to_check():
+	assert data._get_years_to_check([2020], cur_year=2023, force=True, isfile=False) == []
+	assert data._get_years_to_check([2022], cur_year=2023, force=False, isfile=True) == []
+	assert data._get_years_to_check([2022, 2020], cur_year=2023, force=False, isfile=False) == [2023]
+	assert data._get_years_to_check([2020, 2021], cur_year=2023, force=True, isfile=True) == [2022, 2023]
+	assert data._get_years_to_check([2020, 2021], cur_year=2023, force=True, isfile=False) == [2022, 2023]
+
+
+@pytest.mark.parametrize('source,year,table_type,nrows,agency', [
+	("Virginia",2020,"STOPS", 2000, "Fairfax County Police Department"), # CKAN
+	("Philadelphia", 2021, "STOPS", 1000, None),  # Carto
+	("Richmond","MULTIPLE","OFFICER-INVOLVED SHOOTINGS", 5, None), # Socrata
+	("Fairfax County",2016,"ARRESTS", 1000, None),  # ArcGIS
+	("Norristown", 2016, "USE OF FORCE",100, None), # Excel
+	("Denver", "MULTIPLE", "OFFICER-INVOLVED SHOOTINGS", 50, None) # CSV
+])
+def test_load_gen(source, year, table_type, nrows, agency):
+	if check_for_dataset(source, table_type):
+		src = data.Source(source)
+		max_iter = 10
+		df = src.load(table_type, year, agency=agency, nrows=max_iter*nrows).table
+		with warnings.catch_warnings():
+			warnings.filterwarnings("ignore",category=RuntimeWarning)
+			df = df.convert_dtypes()
+
+		offset = 0
+		k = 0
+		for t in src.load_iter(table_type, year, nbatch=nrows, force=True, agency=agency):
+			df_cur = df.iloc[offset:offset+len(t.table)].reset_index(drop=True)
+			df2 = t.table.copy()
+			if set(df.columns)!=set(df2.columns):
+				# Expecting that a column was not returned because it is empty in the subset requested in this iteration
+				assert len(df2.columns)<len(df.columns)
+				missing_columns = list(set(df.columns).difference(set(df2.columns)))
+				for col in missing_columns:
+					assert df_cur[col].isnull().all()
+					df_cur.drop(columns=col, inplace=True)
+			# Assure columns are in proper order
+			assert set(df_cur.columns)==set(df2.columns)
+			df2 = df2[df_cur.columns]
+			# Ensure that dtypes match
+			df2 = df2.astype(df_cur.dtypes.to_dict())
+			assert df2.equals(df_cur)
+			offset+=len(t.table)
+			k+=1
+			if k>=max_iter:
+				break
 
 
 def can_be_limited(data_type, url):
-	data_type = DataType(data_type)
 	if (data_type == DataType.CSV and ".zip" in url):
 		return False
 	elif data_type in [DataType.ArcGIS, DataType.SOCRATA, DataType.CSV, DataType.EXCEL, DataType.CARTO, DataType.CKAN]:
 		return True
 	else:
 		raise ValueError("Unknown table type")
+	
 
 def is_stanford(url):
 	return "stanford.edu" in url
 
 def log_errors_to_file(*args):
 	if not os.path.exists(log_folder):
 		os.mkdir(log_folder)
@@ -414,21 +431,30 @@
 							break
 
 				if not skip:
 					f.write(new_line)
 					f.write("\n")
 
 if __name__ == "__main__":
+	from test_utils import get_datasets
 	# For testing
-	tp = TestData()
-	# (self, csvfile, source, last, skip, loghtml)
+	use_changed_rows = False
 	csvfile = None
-	# csvfile = r"..\opd-data\opd_source_table.csv"
-	last = None
-	last = 922-896+1
+	# csvfile = os.path.join(r"..",'opd-data','opd_source_table.csv')
+	start_idx = 402
 	skip = None
-	# skip = "Sacramento"
+	skip = "Sacramento,Beloit,Rutland"
 	source = None
-	# source = "New York City"
-	tp.test_load_year(csvfile, source, last, skip, None, query={'DataType':'CKAN'})
-	# last = None
-	tp.test_source_download_not_limitable(csvfile, source, last, skip, None, query={'DataType':'CKAN'})
+	# source = "Bremerton" #"Washington D.C." #"Wallkill"
+
+	datasets = get_datasets(csvfile, use_changed_rows)
+
+	# check_excel_sheets(csvfile, source, last, skip, None) 
+	# test_get_years_to_check(csvfile, source, last, skip, None) 
+	# check_table_type_warning(csvfile, source, last, skip, None) 
+	# test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	# test_check_version(csvfile, None, last, skip, None) #
+	test_source_download_limitable(datasets, source, start_idx, skip, False) 
+	
+	# test_get_count(csvfile, None, last, skip, None)
+	# test_load_gen(csvfile, source, last, skip, None) 
+
```

### Comparing `openpolicedata-0.6/tests/test_preproc.py` & `openpolicedata-0.7/tests/test_preproc.py`

 * *Files 24% similar despite different names*

```diff
@@ -105,91 +105,91 @@
 def log_filename():
     filename = "test.log"
     yield filename
     if os.path.exists(filename):
         os.remove(filename)
 
 
-def test_no_transform_map(csvfile, source, last, skip, loghtml, table):
+def test_no_transform_map(table):
     assert table.get_transform_map() is None
 
 
-def test_transform_map(csvfile, source, last, skip, loghtml, std_table):
+def test_transform_map(std_table):
     assert isinstance(std_table.get_transform_map(), list)
     assert isinstance(std_table.get_transform_map()[0], DataMapping)
 
 
 @pytest.mark.parametrize("col", [Column.DATE, Column.TIME, Column.DATETIME,
                                  Column.RACE_ETHNICITY_SUBJECT, Column.ETHNICITY_SUBJECT,
                                  Column.RACE_SUBJECT, Column.RE_GROUP_SUBJECT, Column.AGE_SUBJECT,
                                  Column.AGE_RANGE_SUBJECT, Column.GENDER_SUBJECT,
                                  Column.AGENCY])
-def test_col_in_table(csvfile, source, last, skip, loghtml, std_table, col):
+def test_col_in_table(std_table, col):
     assert col in std_table.table
 
 
 @pytest.mark.parametrize("col", [Column.RACE_ETHNICITY_OFFICER_SUBJECT, Column.ETHNICITY_OFFICER_SUBJECT,
                                  Column.RACE_OFFICER_SUBJECT, Column.RE_GROUP_OFFICER_SUBJECT, Column.AGE_OFFICER_SUBJECT,
                                  Column.AGE_RANGE_OFFICER_SUBJECT, Column.GENDER_OFFICER_SUBJECT,
                                  Column.SUBJECT_OR_OFFICER])
-def test_col_in_table_w_role(csvfile, source, last, skip, loghtml, std_table_w_role, col):    
+def test_col_in_table_w_role(std_table_w_role, col):    
     assert col in std_table_w_role.table
 
 
-def test_get_race_cats_expand(csvfile, source, last, skip, loghtml):
+def test_get_race_cats_expand():
     assert defs.get_race_cats() != defs.get_race_cats(expand=True)
     
 
-def test_race_cats(csvfile, source, last, skip, loghtml, table, std_table):
+def test_race_cats(table, std_table):
     race_cats = defs.get_race_cats()
     keys = defs.get_race_keys()
     white = race_cats[keys.WHITE]
     race_cats[keys.WHITE] = "TEST"
     table = standardize(table, race_cats=race_cats)
 
     orig = std_table.table[Column.RACE_SUBJECT]
     renamed = table.table[Column.RACE_SUBJECT]
 
     assert ((orig==white) == (renamed=="TEST")).all()
 
 
-def test_race_cats_bad_input(csvfile, source, last, skip, loghtml, table):
+def test_race_cats_bad_input(table):
     cats = defs.get_race_cats()
     cats["BAD"] = 'ERROR'
     with pytest.raises(BadCategoryDict):
         table = standardize(table, race_cats=cats)
 
-def test_eth_cats_bad_input(csvfile, source, last, skip, loghtml, table):
+def test_eth_cats_bad_input(table):
     cats = defs.get_eth_cats()
     cats["BAD"] = 'ERROR'
     with pytest.raises(BadCategoryDict):
         table = standardize(table, eth_cats=cats)
 
 
-def test_gender_cats_bad_input(csvfile, source, last, skip, loghtml, table):
+def test_gender_cats_bad_input(table):
     cats = defs.get_gender_cats()
     cats["BAD"] = 'ERROR'
     with pytest.raises(BadCategoryDict):
         table = standardize(table, gender_cats=cats)
 
 
-def test_eth_cats(csvfile, source, last, skip, loghtml, table, std_table):
+def test_eth_cats(table, std_table):
     eth_cats = defs.get_eth_cats()
     keys = defs.get_race_keys()
     latino = eth_cats[keys.LATINO]
     eth_cats[keys.LATINO] = "TEST"
     table = standardize(table, eth_cats=eth_cats)
 
     orig = std_table.table[Column.ETHNICITY_SUBJECT]
     renamed = table.table[Column.ETHNICITY_SUBJECT]
 
     assert ((orig==latino) == (renamed=="TEST")).all()
 
 
-def test_gender_cats(csvfile, source, last, skip, loghtml, table, std_table):
+def test_gender_cats(table, std_table):
     cats = defs.get_gender_cats()
     keys = defs.get_gender_keys()
     orig_label = cats[keys.MALE]
     cats[keys.MALE] = "TEST"
     table = standardize(table, gender_cats=cats)
 
     orig = std_table.table[Column.GENDER_SUBJECT]
@@ -197,72 +197,70 @@
 
     assert ((orig==orig_label) == (renamed=="TEST")).all()
 
 @pytest.mark.parametrize("old_column, new_column",
                          [(race_col, Column.RACE_OFFICER_SUBJECT),
                           (gender_col, Column.GENDER_OFFICER_SUBJECT),
                           (eth_col, Column.ETHNICITY_OFFICER_SUBJECT),
-                          (role_col, Column.SUBJECT_OR_OFFICER),
                           (age_group_col, Column.AGE_RANGE_OFFICER_SUBJECT)
                           ])
-def test_no_id_keep(csvfile, source, last, skip, loghtml, table_w_role, old_column, new_column):
+def test_no_id_keep(table_w_role, old_column, new_column):
     orig_label = bad_data
     table_w_role.table.loc[:5, old_column] = orig_label
 
     table_w_role = standardize(table_w_role)
 
     assert (table_w_role.table.loc[:5, new_column] == orig_label).all()
 
 @pytest.mark.parametrize("old_column, new_column",
                          [(race_col, Column.RACE_OFFICER_SUBJECT),
                           (gender_col, Column.GENDER_OFFICER_SUBJECT),
                           (eth_col, Column.ETHNICITY_OFFICER_SUBJECT),
-                          (role_col, Column.SUBJECT_OR_OFFICER),
                           (age_group_col, Column.AGE_RANGE_OFFICER_SUBJECT)
                           ])
-def test_no_id_null(csvfile, source, last, skip, loghtml, table_w_role, old_column, new_column):
+def test_no_id_null(table_w_role, old_column, new_column):
     orig_label = bad_data
     table_w_role.table.loc[:5, old_column] = orig_label
 
     table_w_role = standardize(table_w_role, no_id='null')
 
     assert (table_w_role.table.loc[:5, new_column] == "").all()
 
 
 @pytest.mark.parametrize("old_column", [race_col, gender_col, eth_col, role_col, age_group_col])
-def test_no_id_error(csvfile, source, last, skip, loghtml, table_w_role, old_column):
+def test_no_id_error(table_w_role, old_column):
     orig_label = bad_data
     table_w_role.table.loc[:5, old_column] = orig_label
 
     with pytest.raises(ValueError, match="Unknown"):
         table_w_role = standardize(table_w_role, no_id="error")
 
 
-def test_agg_cat(csvfile, source, last, skip, loghtml, table, std_table):
+def test_agg_cat(table, std_table):
     orig_label = "East African"
     table.table.loc[:5, race_col] = orig_label
 
     table = standardize(table, agg_race_cat=True)
 
     assert (table.table.loc[:5, Column.RACE_SUBJECT] == defs.get_race_cats()[defs.get_race_keys().BLACK]).all()
 
-def test_keep_raw(csvfile, source, last, skip, loghtml, std_table):
+def test_keep_raw(std_table):
     assert any([x.startswith(preproc._OLD_COLUMN_INDICATOR+"_") for x in std_table.table.columns])
 
 
-def test_not_keep_raw(csvfile, source, last, skip, loghtml, table):
+def test_not_keep_raw(table):
     table = standardize(table, keep_raw=False)
     assert not any([x.startswith(preproc._OLD_COLUMN_INDICATOR+"_") for x in table.table.columns])
 
 @pytest.mark.parametrize("column", [Column.DATE, Column.RACE_OFFICER])
-def test_known_col_not_in_table(csvfile, source, last, skip, loghtml, table, column):
+def test_known_col_not_in_table(table, column):
     with pytest.raises(ValueError, match="Known column .+ is not in the DataFrame"):
         table = standardize(table, known_cols={column:"TEST"})
 
-def test_known_col_bad_key(csvfile, source, last, skip, loghtml, table):
+def test_known_col_bad_key(table):
     with pytest.raises(BadCategoryDict):
         table = standardize(table, known_cols={"BAD":"TEST"})
 
 @pytest.mark.parametrize("old_column, new_column", 
                          [(date_col, Column.DATE),
                           (race_col, Column.RACE_SUBJECT),
                           (race_col, Column.RACE_OFFICER),
@@ -279,121 +277,121 @@
                           (eth_col, Column.ETHNICITY_SUBJECT),
                           (age_group_col, Column.AGE_RANGE_OFFICER),
                           (age_group_col, Column.AGE_RANGE_OFFICER_SUBJECT),
                           (age_group_col, Column.AGE_RANGE_SUBJECT),
                           (time_col, Column.TIME)
                          ]
                         )
-def test_known_col(csvfile, source, last, skip, loghtml, table, old_column, new_column):
+def test_known_col(table, old_column, new_column):
     assert old_column in table.table
     table.table["TEST"] = table.table[old_column]
     table = standardize(table, known_cols={new_column:"TEST"})
     assert new_column in table.table
     assert "RAW_TEST" in table.table
 
-def test_known_col_role(csvfile, source, last, skip, loghtml, table_w_role):
+def test_known_col_role(table_w_role):
     assert role_col in table_w_role.table
     table_w_role.table["TEST"] = table_w_role.table[role_col]
     table_w_role = standardize(table_w_role, known_cols={Column.SUBJECT_OR_OFFICER:"TEST"})
     assert Column.SUBJECT_OR_OFFICER in table_w_role.table
     assert "RAW_TEST" in table_w_role.table
 
-def test_known_col_exists_multiple(csvfile, source, last, skip, loghtml, table):
+def test_known_col_exists_multiple(table):
     assert race_col in table.table
     table.table["TEST1"] = table.table[race_col].copy()
     table.table["TEST2"] = table.table[race_col].copy()
     table = standardize(table, known_cols={Column.RACE_OFFICER:"TEST1",Column.RACE_SUBJECT:"TEST2"})
     assert Column.RACE_OFFICER in table.table
     assert "RAW_TEST1" in table.table
     assert Column.RACE_SUBJECT in table.table
     assert "RAW_TEST2" in table.table
 
-def test_not_verbose(csvfile, source, last, skip, loghtml, table):
+def test_not_verbose(table):
     # Capture output to ensure that it's printed
     logger = logging.getLogger("opd-std")
     log_stream = StringIO()
     sh = logging.StreamHandler(log_stream)
     logger.addHandler(sh)
     try:
         table = standardize(table)
     except:
         raise
     finally:
         logger.removeHandler(sh)
 
     assert len(log_stream.getvalue()) == 0
 
-def test_verbose(csvfile, source, last, skip, loghtml, table):
+def test_verbose(table):
     # Capture output to ensure that it's printed
     logger = logging.getLogger("opd-std")
     log_stream = StringIO()
     sh = logging.StreamHandler(log_stream)
     logger.addHandler(sh)
     try:
         table = standardize(table, verbose=True)
     except:
         raise
     finally:
         logger.removeHandler(sh)
 
     assert len(log_stream.getvalue()) > 0
 
-def test_verbose_to_file(csvfile, source, last, skip, loghtml, table, log_filename):
+def test_verbose_to_file(table, log_filename):
     table = standardize(table, verbose=log_filename)
 
     assert os.path.exists(log_filename)
     assert os.path.getsize(log_filename) > 100
     # Ensure that file handler was removed
     assert len(logging.getLogger("opd-std").handlers)==1
 
-def test_verbose_to_file_cleanup_with_error(csvfile, source, last, skip, loghtml, table, log_filename):
+def test_verbose_to_file_cleanup_with_error(table, log_filename):
     table.table.loc[:5, gender_col] = "TEST"
 
     with pytest.raises(ValueError, match="Unknown"):
         table = standardize(table, no_id="error", verbose=log_filename)
 
     assert os.path.exists(log_filename)
     assert os.path.getsize(log_filename) > 100
     # Ensure that file handler was removed
     assert len(logging.getLogger("opd-std").handlers)==1
 
 
-def test_race_eth_combo_merge(csvfile, source, last, skip, loghtml, std_table):
+def test_race_eth_combo_merge(std_table):
     assert Column.RACE_SUBJECT in std_table.table
     assert Column.RACE_ETHNICITY_SUBJECT in std_table.table
     assert Column.RE_GROUP_SUBJECT in std_table.table
     assert all([isinstance(x,str) for x in std_table.table[Column.RACE_ETHNICITY_SUBJECT].unique()])
 
-def test_race_eth_combo_concat(csvfile, source, last, skip, loghtml, table):
+def test_race_eth_combo_concat(table):
     table = standardize(table, race_eth_combo="concat")
 
     r = defs.get_race_cats()
     e = defs.get_eth_cats()
 
     assert Column.RACE_SUBJECT in table.table
     assert Column.RACE_ETHNICITY_SUBJECT in table.table
     assert f"{r[defs.get_race_keys().BLACK]} {e[defs.get_eth_keys().LATINO]}" in table.table[Column.RACE_ETHNICITY_SUBJECT].unique()
 
 
-def test_race_eth_combo_false(csvfile, source, last, skip, loghtml, table):
+def test_race_eth_combo_false(table):
     table = standardize(table, race_eth_combo=False)
     assert Column.RACE_ETHNICITY_SUBJECT not in table.table
 
-def test_merge_datetime_true(csvfile, source, last, skip, loghtml, std_table):
+def test_merge_datetime_true(std_table):
     assert Column.DATETIME in std_table.table
 
-def test_merge_datetime_false(csvfile, source, last, skip, loghtml, table):
+def test_merge_datetime_false(table):
     table = standardize(table, merge_date_time=False)
     assert Column.DATETIME not in table.table
 
-def test_empty_time_nat(csvfile, source, last, skip, loghtml, table, std_table):
+def test_empty_time_nat(table, std_table):
     idx = table.table[time_col]==bad_time
     assert idx.sum()>0
     assert Column.DATETIME in std_table.table
     assert std_table.table[Column.DATETIME][idx].isnull().all()
 
-def test_empty_time_ignore(csvfile, source, last, skip, loghtml, table):
+def test_empty_time_ignore(table):
     idx = table.table[time_col]==bad_time
     table = standardize(table, empty_time='ignore')
     assert idx.sum()>0
     assert Column.DATETIME in table.table
     assert (table.table[Column.DATETIME][idx]==table.table[Column.DATE][idx]).all()
```

