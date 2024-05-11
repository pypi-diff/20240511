# Comparing `tmp/arctix-0.0.3a1.tar.gz` & `tmp/arctix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.3a1.tar", max compression
+gzip compressed data, was "arctix-0.0.4.tar", max compression
```

## Comparing `arctix-0.0.3a1.tar` & `arctix-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1501 2024-04-27 06:41:51.236513 arctix-0.0.3a1/LICENSE
--rw-r--r--   0        0        0     4493 2024-04-27 06:41:51.236513 arctix-0.0.3a1/README.md
--rw-r--r--   0        0        0     6569 2024-04-27 06:41:51.240513 arctix-0.0.3a1/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/__init__.py
--rw-r--r--   0        0        0       43 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/__init__.py
--rw-r--r--   0        0        0    16839 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/breakfast.py
--rw-r--r--   0        0        0    22011 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/multithumos.py
--rw-r--r--   0        0        0      247 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/testing/__init__.py
--rw-r--r--   0        0        0      538 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/testing/fixtures.py
--rw-r--r--   0        0        0       29 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/__init__.py
--rw-r--r--   0        0        0     2165 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/__init__.py
--rw-r--r--   0        0        0     6978 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/base.py
--rw-r--r--   0        0        0     3265 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/casting.py
--rw-r--r--   0        0        0     2107 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/function.py
--rw-r--r--   0        0        0     2914 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/replace.py
--rw-r--r--   0        0        0     3809 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/sequential.py
--rw-r--r--   0        0        0     2413 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/sorting.py
--rw-r--r--   0        0        0     3185 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/string.py
--rw-r--r--   0        0        0     4581 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/vocab.py
--rw-r--r--   0        0        0       34 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0      276 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/removing.py
--rw-r--r--   0        0        0     1618 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/vocab.py
--rw-r--r--   0        0        0     3334 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/download.py
--rw-r--r--   0        0        0     7145 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/imports.py
--rw-r--r--   0        0        0      190 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/iter/__init__.py
--rw-r--r--   0        0        0     3543 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/iter/path.py
--rw-r--r--   0        0        0     1324 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/mapping.py
--rw-r--r--   0        0        0     3234 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/masking.py
--rw-r--r--   0        0        0    12749 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/vocab.py
--rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 arctix-0.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-11 19:35:43.976134 arctix-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6556 2024-05-11 19:35:43.976134 arctix-0.0.4/README.md
+-rw-r--r--   0        0        0     6664 2024-05-11 19:35:43.980134 arctix-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/__init__.py
+-rw-r--r--   0        0        0    22996 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/breakfast.py
+-rw-r--r--   0        0        0    23825 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/epic_kitchen_100.py
+-rw-r--r--   0        0        0    27519 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/multithumos.py
+-rw-r--r--   0        0        0      247 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/testing/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/testing/fixtures.py
+-rw-r--r--   0        0        0       29 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/__init__.py
+-rw-r--r--   0        0        0     3095 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/__init__.py
+-rw-r--r--   0        0        0     6978 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/base.py
+-rw-r--r--   0        0        0     6262 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/casting.py
+-rw-r--r--   0        0        0     2107 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/function.py
+-rw-r--r--   0        0        0     4084 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/json.py
+-rw-r--r--   0        0        0     2914 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/replace.py
+-rw-r--r--   0        0        0     3809 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/sequential.py
+-rw-r--r--   0        0        0     4352 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/sorting.py
+-rw-r--r--   0        0        0     3107 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/string.py
+-rw-r--r--   0        0        0     3200 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/time.py
+-rw-r--r--   0        0        0     4581 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/vocab.py
+-rw-r--r--   0        0        0       34 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/removing.py
+-rw-r--r--   0        0        0     1618 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/vocab.py
+-rw-r--r--   0        0        0     3196 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/download.py
+-rw-r--r--   0        0        0     7145 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0      190 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/iter/__init__.py
+-rw-r--r--   0        0        0     3543 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/iter/path.py
+-rw-r--r--   0        0        0     1325 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/mapping.py
+-rw-r--r--   0        0        0     3234 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/masking.py
+-rw-r--r--   0        0        0      596 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/noop.py
+-rw-r--r--   0        0        0    14150 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/vocab.py
+-rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 arctix-0.0.4/PKG-INFO
```

### Comparing `arctix-0.0.3a1/LICENSE` & `arctix-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/pyproject.toml` & `arctix-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.3a1"
+version = "0.0.4"
 description = ""
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
-keywords = []
+keywords = ["asynchronous time-series", "dataset", "preprocessing"]
 license = "BSD-3-Clause"
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
@@ -51,25 +51,25 @@
 jupyterlab = "^4.0"
 seaborn = "^0.13"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mike = "^2.0"
+mike = "^2.1"
 mkdocs-material = "^9.5"
-mkdocstrings = { extras = ["python"], version = "^0.24" }
+mkdocstrings = { extras = ["python"], version = "^0.25" }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=24.4"
 coverage = { extras = ["toml"], version = "^7.5" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.7"
-pygments = "^2.17"
-pytest = "^8.1"
+pygments = "^2.18"
+pytest = "^8.2"
 pytest-cov = "^5.0"
 pytest-timeout = "^2.3"
 ruff = ">=0.4.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
@@ -253,14 +253,17 @@
 [tool.ruff.lint.per-file-ignores]
 # Ignore all directories named `tests`.
 "tests/**" = [
     "D", # pydocstyle
     "PL", # Pylint
     "S101", # flake8-bandit
 ]
+"**.ipynb" = [
+    "T20", # flake8-print
+]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `arctix-0.0.3a1/src/arctix/dataset/multithumos.py` & `arctix-0.0.4/src/arctix/dataset/breakfast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,228 @@
-r"""Contain code to prepare/preprocess the MultiTHUMOS data.
+r"""Contain code to download and prepare the Breakfast data.
 
-Information about the MultiTHUMOS dataset can be found in the following
-paper:
-
-Every Moment Counts: Dense Detailed Labeling of Actions in Complex
-Videos. Yeung S., Russakovsky O., Jin N., Andriluka M., Mori G., Fei-Fei
-L. IJCV 2017 (
-
-http://arxiv.org/pdf/1507.05738)
-
-Project page: http://ai.stanford.edu/~syyeung/everymoment.html
+The following documentation assumes the data are downloaded in the
+directory `/path/to/data/breakfast/`.
 """
 
 from __future__ import annotations
 
 __all__ = [
+    "COOKING_ACTIVITIES",
+    "Column",
+    "DATASET_SPLITS",
+    "MetadataKeys",
+    "NUM_COOKING_ACTIVITIES",
+    "URLS",
     "download_data",
     "fetch_data",
     "filter_by_split",
-    "generate_split_column",
     "group_by_sequence",
-    "is_annotation_path_ready",
     "load_annotation_file",
     "load_data",
     "parse_annotation_lines",
     "prepare_data",
-    "to_array_data",
+    "to_array",
+    "to_list",
 ]
 
 import logging
-import zipfile
+import tarfile
 from functools import partial
 from pathlib import Path
-from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING
 
 import numpy as np
 import polars as pl
 from iden.utils.path import sanitize_path
 
 from arctix.transformer import dataframe as td
 from arctix.utils.dataframe import drop_duplicates, generate_vocabulary
-from arctix.utils.download import download_url_to_file
+from arctix.utils.download import download_drive_file
 from arctix.utils.iter import FileFilter, PathLister
 from arctix.utils.mapping import convert_to_dict_of_flat_lists
 from arctix.utils.masking import convert_sequences_to_array, generate_mask_from_lengths
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 logger = logging.getLogger(__name__)
 
-ANNOTATION_URL = "http://ai.stanford.edu/~syyeung/resources/multithumos.zip"
+URLS = {
+    "segmentation_coarse": "https://drive.google.com/open?id=1R3z_CkO1uIOhu4y2Nh0pCHjQQ2l-Ab9E",
+    "segmentation_fine": "https://drive.google.com/open?id=1Alg_xjefEFOOpO_6_RnelWiNqbJlKhVF",
+}
+COOKING_ACTIVITIES = (
+    "cereals",
+    "coffee",
+    "friedegg",
+    "juice",
+    "milk",
+    "pancake",
+    "salat",
+    "sandwich",
+    "scrambledegg",
+    "tea",
+)
+NUM_COOKING_ACTIVITIES = {
+    "cereals": 214,
+    "coffee": 100,
+    "friedegg": 198,
+    "juice": 187,
+    "milk": 224,
+    "pancake": 173,
+    "salat": 185,
+    "sandwich": 197,
+    "scrambledegg": 188,
+    "tea": 223,
+}
+
+PART1 = tuple(f"P{i:02d}" for i in range(3, 16))
+PART2 = tuple(f"P{i:02d}" for i in range(16, 29))
+PART3 = tuple(f"P{i:02d}" for i in range(29, 42))
+PART4 = tuple(f"P{i:02d}" for i in range(42, 55))
+
+DATASET_SPLITS = {
+    "all": sorted(PART1 + PART2 + PART3 + PART4),
+    "minitrain1": sorted(PART2 + PART3),
+    "minitrain2": sorted(PART3 + PART4),
+    "minitrain3": sorted(PART1 + PART4),
+    "minitrain4": sorted(PART1 + PART2),
+    "minival1": sorted(PART4),
+    "minival2": sorted(PART1),
+    "minival3": sorted(PART2),
+    "minival4": sorted(PART3),
+    "test1": sorted(PART1),
+    "test2": sorted(PART2),
+    "test3": sorted(PART3),
+    "test4": sorted(PART4),
+    "train1": sorted(PART2 + PART3 + PART4),
+    "train2": sorted(PART1 + PART3 + PART4),
+    "train3": sorted(PART1 + PART2 + PART4),
+    "train4": sorted(PART1 + PART2 + PART3),
+}
 
 
 class Column:
+    r"""Indicate the column names."""
+
     ACTION: str = "action"
     ACTION_ID: str = "action_id"
+    COOKING_ACTIVITY: str = "cooking_activity"
+    COOKING_ACTIVITY_ID: str = "cooking_activity_id"
     END_TIME: str = "end_time"
-    SEQUENCE_LENGTH: str = "sequence_length"
-    SPLIT: str = "split"
+    PERSON: str = "person"
+    PERSON_ID: str = "person_id"
     START_TIME: str = "start_time"
-    VIDEO: str = "video"
-    VIDEO_ID: str = "video_id"
+    SEQUENCE_LENGTH: str = "sequence_length"
+
+
+class MetadataKeys:
+    r"""Indicate the metadata keys."""
+
+    VOCAB_ACTION: str = "vocab_action"
+    VOCAB_ACTIVITY: str = "vocab_activity"
+    VOCAB_PERSON: str = "vocab_person"
 
 
 def fetch_data(
-    path: Path, remove_duplicate: bool = True, force_download: bool = False
+    path: Path, name: str, remove_duplicate: bool = True, force_download: bool = False
 ) -> pl.DataFrame:
     r"""Download and load the data for Breakfast dataset.
 
     Args:
         path: The path where to store the downloaded data.
+        name: The name of the dataset. The valid names are
+            ``'segmentation_coarse'`` and ``'segmentation_fine'``.
         remove_duplicate: If ``True``, the duplicate examples are
             removed.
         force_download: If ``True``, the annotations are downloaded
             everytime this function is called. If ``False``,
             the annotations are downloaded only if the
             given path does not contain the annotation data.
 
     Returns:
         The data in a DataFrame
 
+    Raises:
+        RuntimeError: if the name is incorrect
+
     Example usage:
 
     ```pycon
 
     >>> from pathlib import Path
-    >>> from arctix.dataset.multithumos import fetch_data
-    >>> data = fetch_data(Path("/path/to/data/multithumos/"))  # doctest: +SKIP
+    >>> from arctix.dataset.breakfast import fetch_data
+    >>> data = fetch_data(
+    ...     Path("/path/to/data/breakfast/"), "segmentation_coarse"
+    ... )  # doctest: +SKIP
 
     ```
     """
+    if name not in (valid_names := set(URLS.keys())):
+        msg = f"Incorrect name: {name}. Valid names are: {valid_names}"
+        raise RuntimeError(msg)
     path = sanitize_path(path)
     download_data(path, force_download)
-    return load_data(path, remove_duplicate)
+    return load_data(path.joinpath(name), remove_duplicate)
 
 
 def download_data(path: Path, force_download: bool = False) -> None:
-    r"""Download the MultiTHUMOS annotation data.
-
-    Internally, this function downloads the annotations in a temporary
-    directory, then extracts the files from the download zip files in
-    the temporary directory, and finally moves the extracted files to
-    the given path.
+    r"""Download the Breakfast annotations.
 
     Args:
-        path: The path where to store the MultiTHUMOS data.
+        path: The path where to store the downloaded data.
         force_download: If ``True``, the annotations are downloaded
             everytime this function is called. If ``False``,
             the annotations are downloaded only if the
             given path does not contain the annotation data.
 
     Example usage:
 
     ```pycon
 
     >>> from pathlib import Path
-    >>> from arctix.dataset.multithumos import download_data
-    >>> path = Path("/path/to/data")
-    >>> download_data(path)  # doctest: +SKIP
-
-    ```
-    """
-    path = sanitize_path(path)
-    if not is_annotation_path_ready(path) or force_download:
-        with TemporaryDirectory() as tmpdir:
-            tmp_path = Path(tmpdir)
-            zip_file = tmp_path.joinpath("multithumos.zip.tmp")
-            logger.info(f"downloading MultiTHUMOS annotations data in {zip_file}...")
-            download_url_to_file(ANNOTATION_URL, zip_file.as_posix(), progress=True)
-
-            logger.info(f"extracting {zip_file} in {tmp_path}...")
-            with zipfile.ZipFile(zip_file, "r") as zip_ref:
-                zip_ref.extractall(tmp_path)
-
-            logger.info(f"moving extracted files to {path}...")
-            path.mkdir(parents=True, exist_ok=True)
-            tmp_path.joinpath("multithumos/README").rename(path.joinpath("README"))
-            tmp_path.joinpath("multithumos/class_list.txt").rename(path.joinpath("class_list.txt"))
-            tmp_path.joinpath("multithumos/annotations").rename(path.joinpath("annotations"))
-
-    logger.info(f"MultiTHUMOS annotation data are available in {path}")
-
-
-def is_annotation_path_ready(path: Path) -> bool:
-    r"""Indicate if the given path contains the MultiTHUMOS annotation
-    data.
-
-    Args:
-        path: The path to check.
-
-    Returns:
-        ``True`` if the path contains the MultiTHUMOS data,
-            otherwise ``False``.
-
-    Example usage:
-
-    ```pycon
-
-    >>> from pathlib import Path
-    >>> from arctix.dataset.multithumos import is_annotation_path_ready
-    >>> is_annotation_path_ready(Path("/path/to/data/"))
-    False
+    >>> from arctix.dataset.breakfast import download_data
+    >>> download_data(Path("/path/to/data/breakfast/"))  # doctest: +SKIP
 
     ```
     """
     path = sanitize_path(path)
-    if not path.joinpath("README").is_file():
-        return False
-    if not path.joinpath("class_list.txt").is_file():
-        return False
-    if not path.joinpath("annotations").is_dir():
-        return False
-    return len(tuple(path.joinpath("annotations").glob("*.txt"))) == 65
+    logger.info(f"Downloading Breakfast dataset annotations in {path}...")
+    for name, url in URLS.items():
+        if not path.joinpath(name).is_dir() or force_download:
+            tar_file = path.joinpath(f"{name}.tar.gz")
+            download_drive_file(url, tar_file, quiet=False, fuzzy=True)
+            tarfile.open(tar_file).extractall(path)  # noqa: S202
+            tar_file.unlink(missing_ok=True)
 
 
 def load_data(path: Path, remove_duplicate: bool = True) -> pl.DataFrame:
     r"""Load all the annotations in a DataFrame.
 
     Args:
         path: The directory where the dataset annotations are stored.
         remove_duplicate: If ``True``, the duplicate rows are removed.
 
     Returns:
         The annotations in a DataFrame.
     """
-    paths = FileFilter(PathLister([sanitize_path(path)], pattern="annotations/*.txt"))
+    paths = FileFilter(PathLister([sanitize_path(path)], pattern="**/*.txt"))
     annotations = list(map(load_annotation_file, paths))
     data = convert_to_dict_of_flat_lists(annotations)
     data = pl.DataFrame(data)
     if remove_duplicate:
         data = drop_duplicates(data)
-    if data.select(pl.len()).item():
-        data = data.sort(by=[Column.VIDEO, Column.START_TIME])
-    return data
+    transformer = td.Sequential(
+        [
+            td.Sort(columns=[Column.COOKING_ACTIVITY, Column.PERSON, Column.START_TIME]),
+            td.SortColumns(),
+        ]
+    )
+    return transformer.transform(data)
 
 
 def load_annotation_file(path: Path) -> dict[str, list]:
     r"""Load the annotation data from a text file.
 
     Args:
         path: The file path to the annotation data.
@@ -215,184 +239,102 @@
         )
         raise ValueError(msg)
     logger.info(f"Reading {path}...")
     with Path.open(path) as file:
         lines = [x.strip() for x in file.readlines()]
 
     annotation = parse_annotation_lines(lines)
-    annotation[Column.ACTION] = [path.stem] * len(annotation[Column.VIDEO])
+    person_id = path.stem.split("_", maxsplit=1)[0]
+    cooking_activity = path.stem.rsplit("_", maxsplit=1)[-1]
+    annotation[Column.PERSON] = [person_id] * len(lines)
+    annotation[Column.COOKING_ACTIVITY] = [cooking_activity] * len(lines)
     return annotation
 
 
 def parse_annotation_lines(lines: Sequence[str]) -> dict:
     r"""Parse the action annotation lines and returns a dictionary with
     the prepared data.
 
     Args:
         lines: The lines to parse.
 
     Returns:
-        A dictionary with the sequence of video names, the start
+        A dictionary with the sequence of actions, the start
             time and end time of each action.
-
-    Example usage:
-
-    ```pycon
-
-    >>> from arctix.dataset.multithumos import parse_annotation_lines
-    >>> out = parse_annotation_lines(
-    ...     [
-    ...         "video_validation_0000266 72.80 76.40",
-    ...         "video_validation_0000681 44.00 50.90",
-    ...         "video_validation_0000682 1.50 5.40",
-    ...         "video_validation_0000682 79.30 83.90",
-    ...     ]
-    ... )
-    >>> out
-    {'video': ['video_validation_0000266', 'video_validation_0000681', 'video_validation_0000682', 'video_validation_0000682'],
-     'start_time': [72.8, 44.0, 1.5, 79.3],
-     'end_time': [76.4, 50.9, 5.4, 83.9]}
-
-    ```
     """
-    videos = []
+    actions = []
     start_time = []
     end_time = []
-    for line in (item.strip() for item in lines):
-        if not line:
-            continue
-        video, start, end = line.split(" ")
-        videos.append(video)
+    for line in lines:
+        pair_time, action = line.strip().split()
+        actions.append(action)
+        start, end = pair_time.split("-")
         start_time.append(float(start))
         end_time.append(float(end))
-    return {Column.VIDEO: videos, Column.START_TIME: start_time, Column.END_TIME: end_time}
+    return {Column.ACTION: actions, Column.START_TIME: start_time, Column.END_TIME: end_time}
 
 
-def prepare_data(frame: pl.DataFrame, split: str = "all") -> tuple[pl.DataFrame, dict]:
-    r"""Prepare the data.
+def filter_by_split(frame: pl.DataFrame, split: str = "all") -> pl.DataFrame:
+    r"""Filter the DataFrame to keep only the rows associated to a
+    dataset split.
 
     Args:
-        frame: The raw DataFrame.
+        frame: The DataFrame to filter.
         split: The dataset split. By default, the union of all the
             dataset splits is used.
 
     Returns:
-        A tuple containing the prepared data and the metadata.
+        The filtered DataFrame.
+    """
+    persons = DATASET_SPLITS[split]
+    return frame.filter(pl.col(Column.PERSON).is_in(persons))
 
-    Example usage:
 
-    ```pycon
+def prepare_data(frame: pl.DataFrame, split: str = "all") -> tuple[pl.DataFrame, dict]:
+    r"""Prepare the data.
 
-    >>> import polars as pl
-    >>> from arctix.dataset.multithumos import Column, prepare_data
-    >>> frame = pl.DataFrame(
-    ...     {
-    ...         Column.VIDEO: ["video_validation_1", "video_test_2", "video_validation_3", "video_test_4"],
-    ...         Column.START_TIME: [72.80, 44.00, 1.50, 17.57],
-    ...         Column.END_TIME: [76.40, 50.90, 5.40, 18.33],
-    ...         Column.ACTION: ["dribble", "dribble", "dribble", "guard"],
-    ...     }
-    ... )
-    >>> data, metadata = prepare_data(frame)
-    >>> data
-    shape: (4, 6)
-    ┌────────────────────┬────────────┬───────────┬─────────┬───────────┬────────────┐
-    │ video              ┆ start_time ┆ end_time  ┆ action  ┆ action_id ┆ split      │
-    │ ---                ┆ ---        ┆ ---       ┆ ---     ┆ ---       ┆ ---        │
-    │ str                ┆ f32        ┆ f32       ┆ str     ┆ i64       ┆ str        │
-    ╞════════════════════╪════════════╪═══════════╪═════════╪═══════════╪════════════╡
-    │ video_test_2       ┆ 44.0       ┆ 50.900002 ┆ dribble ┆ 0         ┆ test       │
-    │ video_test_4       ┆ 17.57      ┆ 18.33     ┆ guard   ┆ 1         ┆ test       │
-    │ video_validation_1 ┆ 72.800003  ┆ 76.400002 ┆ dribble ┆ 0         ┆ validation │
-    │ video_validation_3 ┆ 1.5        ┆ 5.4       ┆ dribble ┆ 0         ┆ validation │
-    └────────────────────┴────────────┴───────────┴─────────┴───────────┴────────────┘
-    >>> metadata
-    {'vocab_action': Vocabulary(
-      counter=Counter({'dribble': 3, 'guard': 1}),
-      index_to_token=('dribble', 'guard'),
-      token_to_index={'dribble': 0, 'guard': 1},
-    )}
+    Args:
+        frame: The raw DataFrame.
+        split: The dataset split. By default, the union of all the
+            dataset splits is used.
 
-    ```
+    Returns:
+        A tuple containing the prepared data and the metadata.
     """
     vocab_action = generate_vocabulary(frame, col=Column.ACTION).sort_by_count()
+    vocab_person = generate_vocabulary(frame, col=Column.PERSON).sort_by_count()
+    vocab_activity = (
+        generate_vocabulary(frame, col=Column.COOKING_ACTIVITY).sort_by_token().sort_by_count()
+    )
     transformer = td.Sequential(
         [
-            td.Sort(columns=[Column.VIDEO, Column.START_TIME]),
-            td.Cast(columns=[Column.START_TIME, Column.END_TIME], dtype=pl.Float32),
-            td.StripChars(columns=[Column.ACTION, Column.VIDEO]),
+            td.Sort(columns=[Column.COOKING_ACTIVITY, Column.PERSON, Column.START_TIME]),
+            td.Cast(columns=[Column.START_TIME, Column.END_TIME], dtype=pl.Float64),
+            td.StripChars(columns=[Column.ACTION, Column.PERSON, Column.COOKING_ACTIVITY]),
+            td.Function(partial(filter_by_split, split=split)),
             td.TokenToIndex(
                 vocab=vocab_action, token_column=Column.ACTION, index_column=Column.ACTION_ID
             ),
-            td.Function(generate_split_column),
-            td.Function(partial(filter_by_split, split=split)),
+            td.TokenToIndex(
+                vocab=vocab_person, token_column=Column.PERSON, index_column=Column.PERSON_ID
+            ),
+            td.TokenToIndex(
+                vocab=vocab_activity,
+                token_column=Column.COOKING_ACTIVITY,
+                index_column=Column.COOKING_ACTIVITY_ID,
+            ),
+            td.SortColumns(),
         ]
     )
     out = transformer.transform(frame)
-    return out, {"vocab_action": vocab_action}
-
-
-def generate_split_column(frame: pl.DataFrame) -> pl.DataFrame:
-    r"""Generate the split column from the video name column.
-
-    Args:
-        frame: The input DataFrame with the video name column.
-
-    Returns:
-        The output DataFrame with the additional split column.
-
-    Example usage:
-
-    ```pycon
-
-    >>> import polars as pl
-    >>> from arctix.dataset.multithumos import Column, generate_split_column
-    >>> frame = pl.DataFrame(
-    ...     {
-    ...         Column.VIDEO: ["video_validation_1", "video_test_2", "video_validation_3", "video_test_4"],
-    ...         Column.ACTION_ID: [0, 2, 5, 1],
-    ...     }
-    ... )
-    >>> out = generate_split_column(frame)
-    >>> out
-    shape: (4, 3)
-    ┌────────────────────┬───────────┬────────────┐
-    │ video              ┆ action_id ┆ split      │
-    │ ---                ┆ ---       ┆ ---        │
-    │ str                ┆ i64       ┆ str        │
-    ╞════════════════════╪═══════════╪════════════╡
-    │ video_validation_1 ┆ 0         ┆ validation │
-    │ video_test_2       ┆ 2         ┆ test       │
-    │ video_validation_3 ┆ 5         ┆ validation │
-    │ video_test_4       ┆ 1         ┆ test       │
-    └────────────────────┴───────────┴────────────┘
-
-    ```
-    """
-    return frame.with_columns(
-        pl.col(Column.VIDEO).str.split_exact(by="_", n=3).struct[1].alias(Column.SPLIT)
-    )
-
-
-def filter_by_split(frame: pl.DataFrame, split: str = "all") -> pl.DataFrame:
-    r"""Filter the DataFrame to keep only the rows associated to a
-    dataset split.
-
-    Args:
-        frame: The DataFrame to filter.
-        split: The dataset split. By default, the union of all the
-            dataset splits is used.
-
-    Returns:
-        The filtered DataFrame.
-    """
-    splits = {split}
-    if split == "all":
-        splits = {"validation", "test"}
-    return frame.filter(pl.col(Column.SPLIT).is_in(splits))
+    return out, {
+        MetadataKeys.VOCAB_ACTION: vocab_action,
+        MetadataKeys.VOCAB_ACTIVITY: vocab_activity,
+        MetadataKeys.VOCAB_PERSON: vocab_person,
+    }
 
 
 def group_by_sequence(frame: pl.DataFrame) -> pl.DataFrame:
     r"""Group the DataFrame by sequences of actions.
 
     Args:
         frame: The input DataFrame.
@@ -401,198 +343,293 @@
         The DataFrame after the grouping.
 
     Example usage:
 
     ```pycon
 
     >>> import polars as pl
-    >>> from arctix.dataset.multithumos import Column, group_by_sequence
+    >>> from arctix.dataset.breakfast import Column, group_by_sequence
     >>> frame = pl.DataFrame(
     ...     {
-    ...         Column.VIDEO: [
-    ...             "video_validation_1",
-    ...             "video_validation_1",
-    ...             "video_validation_1",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...         ],
-    ...         Column.START_TIME: [1.50, 17.57, 79.30, 2.97, 4.54, 20.22, 27.42],
-    ...         Column.END_TIME: [5.40, 18.33, 83.90, 3.60, 5.07, 20.49, 30.23],
     ...         Column.ACTION: [
-    ...             "dribble",
-    ...             "guard",
-    ...             "dribble",
-    ...             "guard",
-    ...             "guard",
-    ...             "guard",
-    ...             "shoot",
+    ...             "SIL",
+    ...             "take_bowl",
+    ...             "pour_cereals",
+    ...             "pour_milk",
+    ...             "stir_cereals",
+    ...             "SIL",
+    ...             "SIL",
+    ...             "pour_milk",
+    ...             "spoon_powder",
+    ...             "SIL",
     ...         ],
-    ...         Column.ACTION_ID: [1, 0, 1, 0, 0, 0, 2],
-    ...         Column.SPLIT: [
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
+    ...         Column.ACTION_ID: [0, 2, 5, 1, 3, 0, 0, 1, 4, 0],
+    ...         Column.COOKING_ACTIVITY: [
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
     ...         ],
-    ...     },
-    ...     schema={
-    ...         Column.VIDEO: pl.String,
-    ...         Column.START_TIME: pl.Float32,
-    ...         Column.END_TIME: pl.Float32,
-    ...         Column.ACTION: pl.String,
-    ...         Column.ACTION_ID: pl.Int64,
-    ...         Column.SPLIT: pl.String,
-    ...     },
+    ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
+    ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
+    ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...     }
     ... )
     >>> groups = group_by_sequence(frame)
-    >>> groups
-    shape: (2, 6)
-    ┌─────────────────┬────────────┬─────────────┬─────────────────┬─────────────────┬─────────────────┐
-    │ video           ┆ split      ┆ action_id   ┆ start_time      ┆ end_time        ┆ sequence_length │
-    │ ---             ┆ ---        ┆ ---         ┆ ---             ┆ ---             ┆ ---             │
-    │ str             ┆ str        ┆ list[i64]   ┆ list[f32]       ┆ list[f32]       ┆ u32             │
-    ╞═════════════════╪════════════╪═════════════╪═════════════════╪═════════════════╪═════════════════╡
-    │ video_validatio ┆ validation ┆ [1, 0, 1]   ┆ [1.5, 17.57,    ┆ [5.4, 18.33,    ┆ 3               │
-    │ n_1             ┆            ┆             ┆ 79.300003]      ┆ 83.900002]      ┆                 │
-    │ video_validatio ┆ validation ┆ [0, 0, … 2] ┆ [2.97, 4.54, …  ┆ [3.6, 5.07, …   ┆ 4               │
-    │ n_2             ┆            ┆             ┆ 27.42]          ┆ 30.23]          ┆                 │
-    └─────────────────┴────────────┴─────────────┴─────────────────┴─────────────────┴─────────────────┘
+    >>> with pl.Config(tbl_cols=-1):
+    ...     groups
+    shape: (2, 9)
+    ┌───────────┬───────────┬──────────┬──────────┬──────────┬────────┬──────────┬──────────┬──────────┐
+    │ action    ┆ action_id ┆ cooking_ ┆ cooking_ ┆ end_time ┆ person ┆ person_i ┆ sequence ┆ start_ti │
+    │ ---       ┆ ---       ┆ activity ┆ activity ┆ ---      ┆ ---    ┆ d        ┆ _length  ┆ me       │
+    │ list[str] ┆ list[i64] ┆ ---      ┆ _id      ┆ list[f64 ┆ str    ┆ ---      ┆ ---      ┆ ---      │
+    │           ┆           ┆ str      ┆ ---      ┆ ]        ┆        ┆ i64      ┆ u32      ┆ list[f64 │
+    │           ┆           ┆          ┆ i64      ┆          ┆        ┆          ┆          ┆ ]        │
+    ╞═══════════╪═══════════╪══════════╪══════════╪══════════╪════════╪══════════╪══════════╪══════════╡
+    │ ["SIL",   ┆ [0, 2, …  ┆ cereals  ┆ 0        ┆ [30.0,   ┆ P03    ┆ 0        ┆ 6        ┆ [1.0,    │
+    │ "take_bow ┆ 0]        ┆          ┆          ┆ 150.0, … ┆        ┆          ┆          ┆ 31.0, …  │
+    │ l", …     ┆           ┆          ┆          ┆ 836.0]   ┆        ┆          ┆          ┆ 706.0]   │
+    │ "SIL"]    ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
+    │ ["SIL",   ┆ [0, 1, …  ┆ milk     ┆ 1        ┆ [47.0,   ┆ P54    ┆ 1        ┆ 4        ┆ [1.0,    │
+    │ "pour_mil ┆ 0]        ┆          ┆          ┆ 215.0, … ┆        ┆          ┆          ┆ 48.0, …  │
+    │ k", …     ┆           ┆          ┆          ┆ 747.0]   ┆        ┆          ┆          ┆ 566.0]   │
+    │ "SIL"]    ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
+    └───────────┴───────────┴──────────┴──────────┴──────────┴────────┴──────────┴──────────┴──────────┘
 
     ```
     """
-    return (
-        frame.group_by([Column.VIDEO])
-        .agg(
-            pl.first(Column.SPLIT),
-            pl.col(Column.ACTION_ID).alias(Column.ACTION_ID),
-            pl.col(Column.START_TIME).alias(Column.START_TIME),
-            pl.col(Column.END_TIME).alias(Column.END_TIME),
-            pl.len().alias(Column.SEQUENCE_LENGTH),
-        )
-        .sort(by=[Column.VIDEO])
+    data = frame.group_by([Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]).agg(
+        pl.first(Column.COOKING_ACTIVITY),
+        pl.first(Column.PERSON),
+        pl.col(Column.ACTION),
+        pl.col(Column.ACTION_ID),
+        pl.col(Column.START_TIME),
+        pl.col(Column.END_TIME),
+        pl.len().alias(Column.SEQUENCE_LENGTH),
+    )
+    transformer = td.Sequential(
+        [
+            td.Sort(columns=[Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]),
+            td.SortColumns(),
+        ]
     )
+    return transformer.transform(data)
 
 
-def to_array_data(frame: pl.DataFrame) -> dict[str, np.ndarray]:
+def to_array(frame: pl.DataFrame) -> dict[str, np.ndarray]:
     r"""Convert a DataFrame to a dictionary of arrays.
 
     Args:
         frame: The input DataFrame.
 
     Returns:
         The dictionary of arrays.
 
     Example usage:
 
     ```pycon
 
     >>> import polars as pl
-    >>> from arctix.dataset.multithumos import Column, to_array_data
+    >>> from arctix.dataset.breakfast import Column, to_array
     >>> frame = pl.DataFrame(
     ...     {
-    ...         Column.VIDEO: [
-    ...             "video_validation_1",
-    ...             "video_validation_1",
-    ...             "video_validation_1",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...             "video_validation_2",
-    ...         ],
-    ...         Column.START_TIME: [1.0, 17.0, 79.0, 2.0, 4.0, 20.0, 27.0],
-    ...         Column.END_TIME: [5.0, 18.0, 83.0, 3.0, 5.0, 20.0, 30.0],
     ...         Column.ACTION: [
-    ...             "dribble",
-    ...             "guard",
-    ...             "dribble",
-    ...             "guard",
-    ...             "guard",
-    ...             "guard",
-    ...             "shoot",
+    ...             "SIL",
+    ...             "take_bowl",
+    ...             "pour_cereals",
+    ...             "pour_milk",
+    ...             "stir_cereals",
+    ...             "SIL",
+    ...             "SIL",
+    ...             "pour_milk",
+    ...             "spoon_powder",
+    ...             "SIL",
     ...         ],
-    ...         Column.ACTION_ID: [1, 0, 1, 0, 0, 0, 2],
-    ...         Column.SPLIT: [
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
-    ...             "validation",
+    ...         Column.ACTION_ID: [0, 2, 5, 1, 3, 0, 0, 1, 4, 0],
+    ...         Column.COOKING_ACTIVITY: [
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
     ...         ],
-    ...     },
-    ...     schema={
-    ...         Column.VIDEO: pl.String,
-    ...         Column.START_TIME: pl.Float32,
-    ...         Column.END_TIME: pl.Float32,
-    ...         Column.ACTION: pl.String,
-    ...         Column.ACTION_ID: pl.Int64,
-    ...         Column.SPLIT: pl.String,
-    ...     },
+    ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
+    ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
+    ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...     }
     ... )
-    >>> arrays = to_array_data(frame)
+    >>> arrays = to_array(frame)
     >>> arrays
-    {'sequence_length': array([3, 4]),
-     'split': array(['validation', 'validation'], dtype='<U10'),
-     'action_id': masked_array(
-      data=[[1, 0, 1, --],
-            [0, 0, 0, 2]],
-      mask=[[False, False, False,  True],
-            [False, False, False, False]],
+    {'action': masked_array(
+      data=[['SIL', 'take_bowl', 'pour_cereals', 'pour_milk', 'stir_cereals',
+             'SIL'],
+            ['SIL', 'pour_milk', 'spoon_powder', 'SIL', --, --]],
+      mask=[[False, False, False, False, False, False],
+            [False, False, False, False,  True,  True]],
+      fill_value='N/A',
+      dtype='<U12'), 'action_id': masked_array(
+      data=[[0, 2, 5, 1, 3, 0],
+            [0, 1, 4, 0, --, --]],
+      mask=[[False, False, False, False, False, False],
+            [False, False, False, False,  True,  True]],
       fill_value=999999),
-     'start_time': masked_array(
-      data=[[1.0, 17.0, 79.0, --],
-            [2.0, 4.0, 20.0, 27.0]],
-      mask=[[False, False, False,  True],
-            [False, False, False, False]],
-      fill_value=1e+20),
-     'end_time': masked_array(
-      data=[[5.0, 18.0, 83.0, --],
-            [3.0, 5.0, 20.0, 30.0]],
-      mask=[[False, False, False,  True],
-            [False, False, False, False]],
+      'cooking_activity': array(['cereals', 'milk'], dtype='<U7'),
+      'cooking_activity_id': array([0, 1]),
+      'person': array(['P03', 'P54'], dtype='<U3'),
+      'person_id': array([0, 1]),
+      'sequence_length': array([6, 4]),
+      'start_time': masked_array(
+      data=[[1.0, 31.0, 151.0, 429.0, 576.0, 706.0],
+            [1.0, 48.0, 216.0, 566.0, --, --]],
+      mask=[[False, False, False, False, False, False],
+            [False, False, False, False,  True,  True]],
+      fill_value=1e+20), 'end_time': masked_array(
+      data=[[30.0, 150.0, 428.0, 575.0, 705.0, 836.0],
+            [47.0, 215.0, 565.0, 747.0, --, --]],
+      mask=[[False, False, False, False, False, False],
+            [False, False, False, False,  True,  True]],
       fill_value=1e+20)}
 
     ```
     """
     groups = group_by_sequence(frame)
     lengths = groups.get_column(Column.SEQUENCE_LENGTH).to_numpy()
     mask = generate_mask_from_lengths(lengths)
     return {
-        Column.SEQUENCE_LENGTH: lengths.astype(int),
-        Column.SPLIT: groups.get_column(Column.SPLIT).to_numpy().astype(str),
+        Column.ACTION: np.ma.masked_array(
+            data=convert_sequences_to_array(
+                groups.get_column(Column.ACTION).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.object_,
+                padded_value="N/A",
+            ).astype(str),
+            mask=mask,
+        ),
         Column.ACTION_ID: np.ma.masked_array(
             data=convert_sequences_to_array(
-                groups.get_column(Column.ACTION_ID).to_list(), dtype=int, max_len=mask.shape[1]
-            ).astype(int),
+                groups.get_column(Column.ACTION_ID).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.int64,
+                padded_value=-1,
+            ),
             mask=mask,
         ),
+        Column.COOKING_ACTIVITY: groups.get_column(Column.COOKING_ACTIVITY).to_numpy().astype(str),
+        Column.COOKING_ACTIVITY_ID: groups.get_column(Column.COOKING_ACTIVITY_ID)
+        .to_numpy()
+        .astype(np.int64),
+        Column.PERSON: groups.get_column(Column.PERSON).to_numpy().astype(str),
+        Column.PERSON_ID: groups.get_column(Column.PERSON_ID).to_numpy().astype(np.int64),
+        Column.SEQUENCE_LENGTH: lengths.astype(np.int64),
         Column.START_TIME: np.ma.masked_array(
             data=convert_sequences_to_array(
-                groups.get_column(Column.START_TIME).to_list(), dtype=float, max_len=mask.shape[1]
-            ).astype(float),
+                groups.get_column(Column.START_TIME).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.float64,
+                padded_value=-1.0,
+            ),
             mask=mask,
         ),
         Column.END_TIME: np.ma.masked_array(
             data=convert_sequences_to_array(
-                groups.get_column(Column.END_TIME).to_list(), dtype=float, max_len=mask.shape[1]
-            ).astype(float),
+                groups.get_column(Column.END_TIME).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.float64,
+                padded_value=-1.0,
+            ),
             mask=mask,
         ),
     }
 
 
+def to_list(frame: pl.DataFrame) -> dict[str, list]:
+    r"""Convert a DataFrame to a dictionary of lists.
+
+    Args:
+        frame: The input DataFrame.
+
+    Returns:
+        The dictionary of lists.
+
+    Example usage:
+
+    ```pycon
+
+    >>> import polars as pl
+    >>> from arctix.dataset.breakfast import Column, to_list
+    >>> frame = pl.DataFrame(
+    ...     {
+    ...         Column.ACTION: [
+    ...             "SIL",
+    ...             "take_bowl",
+    ...             "pour_cereals",
+    ...             "pour_milk",
+    ...             "stir_cereals",
+    ...             "SIL",
+    ...             "SIL",
+    ...             "pour_milk",
+    ...             "spoon_powder",
+    ...             "SIL",
+    ...         ],
+    ...         Column.ACTION_ID: [0, 2, 5, 1, 3, 0, 0, 1, 4, 0],
+    ...         Column.COOKING_ACTIVITY: [
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...         ],
+    ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
+    ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
+    ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+    ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...     }
+    ... )
+    >>> data_list = to_list(frame)
+    >>> data_list
+    {'action': [['SIL', 'take_bowl', 'pour_cereals', 'pour_milk', 'stir_cereals', 'SIL'], ['SIL', 'pour_milk', 'spoon_powder', 'SIL']],
+     'action_id': [[0, 2, 5, 1, 3, 0], [0, 1, 4, 0]],
+     'cooking_activity': ['cereals', 'milk'],
+     'cooking_activity_id': [0, 1],
+     'end_time': [[30.0, 150.0, 428.0, 575.0, 705.0, 836.0], [47.0, 215.0, 565.0, 747.0]],
+     'person': ['P03', 'P54'],
+     'person_id': [0, 1],
+     'sequence_length': [6, 4],
+     'start_time': [[1.0, 31.0, 151.0, 429.0, 576.0, 706.0], [1.0, 48.0, 216.0, 566.0]]}
+
+    ```
+    """
+    return group_by_sequence(frame).to_dict(as_series=False)
+
+
 if __name__ == "__main__":  # pragma: no cover
     import os
 
     logging.basicConfig(level=logging.DEBUG)
 
-    path = Path(os.environ["ARCTIX_DATA_PATH"]).joinpath("multithumos")
-    raw_data = fetch_data(path)
+    path = Path(os.environ["ARCTIX_DATA_PATH"]).joinpath("breakfast")
+    raw_data = fetch_data(path, name="segmentation_coarse")
+    logger.info(f"data_raw:\n{raw_data}")
     data, metadata = prepare_data(raw_data)
     logger.info(f"data:\n{data}")
     logger.info(f"metadata:\n{metadata}")
```

### Comparing `arctix-0.0.3a1/src/arctix/testing/fixtures.py` & `arctix-0.0.4/src/arctix/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/__init__.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,51 +6,73 @@
     "BaseDataFrameTransformer",
     "Cast",
     "CastDataFrameTransformer",
     "Function",
     "FunctionDataFrameTransformer",
     "IndexToToken",
     "IndexToTokenDataFrameTransformer",
+    "JsonDecode",
+    "JsonDecodeDataFrameTransformer",
     "Replace",
     "ReplaceDataFrameTransformer",
     "Sequential",
     "SequentialDataFrameTransformer",
     "Sort",
+    "SortColumns",
+    "SortColumnsDataFrameTransformer",
     "SortDataFrameTransformer",
     "StripChars",
     "StripCharsDataFrameTransformer",
+    "TimeToSecond",
+    "TimeToSecondDataFrameTransformer",
+    "ToTime",
+    "ToTimeDataFrameTransformer",
     "TokenToIndex",
     "TokenToIndexDataFrameTransformer",
     "is_dataframe_transformer_config",
     "setup_dataframe_transformer",
 ]
 
 from arctix.transformer.dataframe.base import (
     BaseDataFrameTransformer,
     is_dataframe_transformer_config,
     setup_dataframe_transformer,
 )
 from arctix.transformer.dataframe.casting import CastDataFrameTransformer
 from arctix.transformer.dataframe.casting import CastDataFrameTransformer as Cast
+from arctix.transformer.dataframe.casting import ToTimeDataFrameTransformer
+from arctix.transformer.dataframe.casting import ToTimeDataFrameTransformer as ToTime
 from arctix.transformer.dataframe.function import FunctionDataFrameTransformer
 from arctix.transformer.dataframe.function import (
     FunctionDataFrameTransformer as Function,
 )
+from arctix.transformer.dataframe.json import JsonDecodeDataFrameTransformer
+from arctix.transformer.dataframe.json import (
+    JsonDecodeDataFrameTransformer as JsonDecode,
+)
 from arctix.transformer.dataframe.replace import ReplaceDataFrameTransformer
 from arctix.transformer.dataframe.replace import ReplaceDataFrameTransformer as Replace
 from arctix.transformer.dataframe.sequential import SequentialDataFrameTransformer
 from arctix.transformer.dataframe.sequential import (
     SequentialDataFrameTransformer as Sequential,
 )
+from arctix.transformer.dataframe.sorting import SortColumnsDataFrameTransformer
+from arctix.transformer.dataframe.sorting import (
+    SortColumnsDataFrameTransformer as SortColumns,
+)
 from arctix.transformer.dataframe.sorting import SortDataFrameTransformer
 from arctix.transformer.dataframe.sorting import SortDataFrameTransformer as Sort
 from arctix.transformer.dataframe.string import StripCharsDataFrameTransformer
 from arctix.transformer.dataframe.string import (
     StripCharsDataFrameTransformer as StripChars,
 )
+from arctix.transformer.dataframe.time import TimeToSecondDataFrameTransformer
+from arctix.transformer.dataframe.time import (
+    TimeToSecondDataFrameTransformer as TimeToSecond,
+)
 from arctix.transformer.dataframe.vocab import IndexToTokenDataFrameTransformer
 from arctix.transformer.dataframe.vocab import (
     IndexToTokenDataFrameTransformer as IndexToToken,
 )
 from arctix.transformer.dataframe.vocab import TokenToIndexDataFrameTransformer
 from arctix.transformer.dataframe.vocab import (
     TokenToIndexDataFrameTransformer as TokenToIndex,
```

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/base.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/casting.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-r"""Contain ``polars.DataFrame`` transformers to convert some columns to
-a new data type."""
+r"""Contain ``polars.DataFrame`` transformers to process columns with
+time values."""
 
 from __future__ import annotations
 
-__all__ = ["CastDataFrameTransformer"]
+__all__ = ["TimeToSecondDataFrameTransformer"]
 
-from typing import TYPE_CHECKING, Any
 
 import polars as pl
 
 from arctix.transformer.dataframe.base import BaseDataFrameTransformer
-from arctix.utils.imports import is_tqdm_available
 
-if TYPE_CHECKING:
-    from collections.abc import Iterable, Sequence
 
-if is_tqdm_available():
-    from tqdm import tqdm
-else:  # pragma: no cover
-
-    def tqdm(it: Iterable, *args: Any, **kwargs: Any) -> Iterable:  # noqa: ARG001
-        return it
-
-
-class CastDataFrameTransformer(BaseDataFrameTransformer):
-    r"""Implement a transformer to convert some columns to a new data
-    type.
+class TimeToSecondDataFrameTransformer(BaseDataFrameTransformer):
+    r"""Implement a transformer to convert a column with time values to
+    seconds.
 
     Args:
-        columns: The columns to convert.
-        dtype: The target data type.
+        in_col: The input column with the time value to convert.
+        out_col: The output column with the time in seconds.
 
     Example usage:
 
     ```pycon
 
+    >>> import datetime
     >>> import polars as pl
-    >>> from arctix.transformer.dataframe import Cast
-    >>> transformer = Cast(columns=["col1", "col3"], dtype=pl.Int32)
+    >>> from arctix.transformer.dataframe import TimeToSecond
+    >>> transformer = TimeToSecond(in_col="time", out_col="second")
     >>> transformer
-    CastDataFrameTransformer(columns=('col1', 'col3'), dtype=Int32)
+    TimeToSecondDataFrameTransformer(in_col=time, out_col=second)
     >>> frame = pl.DataFrame(
     ...     {
-    ...         "col1": [1, 2, 3, 4, 5],
-    ...         "col2": ["1", "2", "3", "4", "5"],
-    ...         "col3": ["1", "2", "3", "4", "5"],
-    ...         "col4": ["a", "b", "c", "d", "e"],
-    ...     }
+    ...         "time": [
+    ...             datetime.time(0, 0, 1, 890000),
+    ...             datetime.time(0, 1, 1, 890000),
+    ...             datetime.time(1, 1, 1, 890000),
+    ...             datetime.time(0, 19, 19, 890000),
+    ...             datetime.time(19, 19, 19, 890000),
+    ...         ],
+    ...         "col": ["a", "b", "c", "d", "e"],
+    ...     },
+    ...     schema={"time": pl.Time, "col": pl.String},
     ... )
     >>> frame
-    shape: (5, 4)
-    ┌──────┬──────┬──────┬──────┐
-    │ col1 ┆ col2 ┆ col3 ┆ col4 │
-    │ ---  ┆ ---  ┆ ---  ┆ ---  │
-    │ i64  ┆ str  ┆ str  ┆ str  │
-    ╞══════╪══════╪══════╪══════╡
-    │ 1    ┆ 1    ┆ 1    ┆ a    │
-    │ 2    ┆ 2    ┆ 2    ┆ b    │
-    │ 3    ┆ 3    ┆ 3    ┆ c    │
-    │ 4    ┆ 4    ┆ 4    ┆ d    │
-    │ 5    ┆ 5    ┆ 5    ┆ e    │
-    └──────┴──────┴──────┴──────┘
+    shape: (5, 2)
+    ┌──────────────┬─────┐
+    │ time         ┆ col │
+    │ ---          ┆ --- │
+    │ time         ┆ str │
+    ╞══════════════╪═════╡
+    │ 00:00:01.890 ┆ a   │
+    │ 00:01:01.890 ┆ b   │
+    │ 01:01:01.890 ┆ c   │
+    │ 00:19:19.890 ┆ d   │
+    │ 19:19:19.890 ┆ e   │
+    └──────────────┴─────┘
     >>> out = transformer.transform(frame)
     >>> out
-    shape: (5, 4)
-    ┌──────┬──────┬──────┬──────┐
-    │ col1 ┆ col2 ┆ col3 ┆ col4 │
-    │ ---  ┆ ---  ┆ ---  ┆ ---  │
-    │ i32  ┆ str  ┆ i32  ┆ str  │
-    ╞══════╪══════╪══════╪══════╡
-    │ 1    ┆ 1    ┆ 1    ┆ a    │
-    │ 2    ┆ 2    ┆ 2    ┆ b    │
-    │ 3    ┆ 3    ┆ 3    ┆ c    │
-    │ 4    ┆ 4    ┆ 4    ┆ d    │
-    │ 5    ┆ 5    ┆ 5    ┆ e    │
-    └──────┴──────┴──────┴──────┘
+    shape: (5, 3)
+    ┌──────────────┬─────┬──────────┐
+    │ time         ┆ col ┆ second   │
+    │ ---          ┆ --- ┆ ---      │
+    │ time         ┆ str ┆ f64      │
+    ╞══════════════╪═════╪══════════╡
+    │ 00:00:01.890 ┆ a   ┆ 1.89     │
+    │ 00:01:01.890 ┆ b   ┆ 61.89    │
+    │ 01:01:01.890 ┆ c   ┆ 3661.89  │
+    │ 00:19:19.890 ┆ d   ┆ 1159.89  │
+    │ 19:19:19.890 ┆ e   ┆ 69559.89 │
+    └──────────────┴─────┴──────────┘
 
     ```
     """
 
-    def __init__(self, columns: Sequence[str], dtype: type[pl.DataType]) -> None:
-        self._columns = tuple(columns)
-        self._dtype = dtype
+    def __init__(self, in_col: str, out_col: str) -> None:
+        self._in_col = in_col
+        self._out_col = out_col
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__qualname__}(columns={self._columns}, dtype={self._dtype})"
+        return f"{self.__class__.__qualname__}(in_col={self._in_col}, out_col={self._out_col})"
 
     def transform(self, frame: pl.DataFrame) -> pl.DataFrame:
-        for col in tqdm(self._columns, desc=f"converting to {self._dtype}"):
-            frame = frame.with_columns(frame.select(pl.col(col).cast(self._dtype)))
-        return frame
+        return frame.with_columns(
+            frame.select(
+                pl.col(self._in_col)
+                .cast(pl.Duration)
+                .dt.total_microseconds()
+                .truediv(1e6)
+                .alias(self._out_col)
+            )
+        )
```

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/function.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/function.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/replace.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/replace.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/sequential.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/sequential.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/string.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/string.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 r"""Contain ``polars.DataFrame`` transformers to process string
 values."""
 
 from __future__ import annotations
 
 __all__ = ["StripCharsDataFrameTransformer"]
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 import polars as pl
 
 from arctix.transformer.dataframe.base import BaseDataFrameTransformer
 from arctix.utils.imports import is_tqdm_available
 
 if TYPE_CHECKING:
-    from collections.abc import Iterable, Sequence
+    from collections.abc import Sequence
 
 if is_tqdm_available():
     from tqdm import tqdm
 else:  # pragma: no cover
-
-    def tqdm(it: Iterable, *args: Any, **kwargs: Any) -> Iterable:  # noqa: ARG001
-        return it
+    from arctix.utils.noop import tqdm
 
 
 class StripCharsDataFrameTransformer(BaseDataFrameTransformer):
     r"""Implement a transformer to remove leading and trailing
     characters.
 
     Args:
```

### Comparing `arctix-0.0.3a1/src/arctix/transformer/dataframe/vocab.py` & `arctix-0.0.4/src/arctix/transformer/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/dataframe/removing.py` & `arctix-0.0.4/src/arctix/utils/dataframe/removing.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/dataframe/vocab.py` & `arctix-0.0.4/src/arctix/utils/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/download.py` & `arctix-0.0.4/src/arctix/utils/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 r"""Contain utility functions to download data assets."""
 
 from __future__ import annotations
 
 __all__ = ["download_drive_file", "download_url_to_file"]
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import Any
 
 from iden.io.utils import generate_unique_tmp_path
 from iden.utils.path import sanitize_path
 
 from arctix.utils.imports import (
     check_gdown,
     check_requests,
     is_gdown_available,
     is_requests_available,
     is_tqdm_available,
 )
 
-if TYPE_CHECKING:
-    from collections.abc import Iterable
-
 if is_gdown_available():
     import gdown
 else:  # pragma: no cover
     gdown = None
 
 if is_requests_available():
     import requests
 else:  # pragma: no cover
     requests = None
 
 if is_tqdm_available():
     from tqdm import tqdm
 else:  # pragma: no cover
-
-    def tqdm(it: Iterable, *args: Any, **kwargs: Any) -> Iterable:  # noqa: ARG001
-        return it
+    from arctix.utils.noop import tqdm
 
 
 def download_drive_file(url: str, path: Path, *args: Any, **kwargs: Any) -> None:
     r"""Download a file from Google Drive.
 
     Args:
         url: The Google Drive URL.
```

### Comparing `arctix-0.0.3a1/src/arctix/utils/imports.py` & `arctix-0.0.4/src/arctix/utils/imports.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/iter/path.py` & `arctix-0.0.4/src/arctix/utils/iter/path.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/mapping.py` & `arctix-0.0.4/src/arctix/utils/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from coola.nested import convert_to_dict_of_lists
 
 if TYPE_CHECKING:
     from collections.abc import Hashable
 
 
 def convert_to_dict_of_flat_lists(
-    seq_of_mappings: list[dict[Hashable, list]]
+    seq_of_mappings: list[dict[Hashable, list]],
 ) -> dict[Hashable, list]:
     r"""Convert a sequence of mappings to a dictionary of lists.
 
     All the dictionaries should have the same keys. The first
     mapping in the sequence is used to find the keys.
     The lists of lists are converted to flat lists.
```

### Comparing `arctix-0.0.3a1/src/arctix/utils/masking.py` & `arctix-0.0.4/src/arctix/utils/masking.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a1/src/arctix/utils/vocab.py` & `arctix-0.0.4/src/arctix/utils/vocab.py`

 * *Files 6% similar despite different names*

```diff
@@ -418,14 +418,54 @@
         >>> vocab.get_index_to_token()
         ('b', 'c')
 
         ```
         """
         return Vocabulary(Counter(dict(self.counter.most_common(max_num_tokens))))
 
+    @classmethod
+    def from_token_to_index(cls, token_to_index: dict[str, int]) -> Vocabulary:
+        r"""Instantiate a ``Vocabulary`` from a token to index mapping.
+
+        The counter is initialized to 1 for each token.
+
+        Args:
+            token_to_index: The token to index mapping.
+
+        Returns:
+            The instantiated ``Vocabulary``.
+
+        Example usage:
+
+        ```pycon
+
+        >>> from collections import Counter
+        >>> from arctix.utils.vocab import Vocabulary
+        >>> vocab = Vocabulary.from_token_to_index({"grizz": 2, "polar": 0, "bear": 1})
+        >>> vocab
+        Vocabulary(
+          counter=Counter({'polar': 1, 'bear': 1, 'grizz': 1}),
+          index_to_token=('polar', 'bear', 'grizz'),
+          token_to_index={'polar': 0, 'bear': 1, 'grizz': 2},
+        )
+        >>> vocab.get_token_to_index()
+        {'polar': 0, 'bear': 1, 'grizz': 2}
+
+        ```
+        """
+        mapping = dict(sorted(token_to_index.items(), key=lambda item: item[1]))
+        vocab = Vocabulary(Counter({token: 1 for token in mapping}))
+        if not objects_are_equal(vocab.get_token_to_index(), token_to_index):
+            msg = (
+                "token_to_index and the vocabulary token to index mapping do not match:\n"
+                f"{token_to_index}\n{vocab.get_token_to_index()}"
+            )
+            raise RuntimeError(msg)
+        return vocab
+
 
 class VocabularyEqualityComparator(BaseEqualityComparator[Vocabulary]):
     r"""Implement an equality comparator for ``Vocabulary`` objects."""
 
     def __init__(self) -> None:
         self._handler = SameObjectHandler()
         self._handler.chain(SameTypeHandler()).chain(EqualHandler())
```

### Comparing `arctix-0.0.3a1/PKG-INFO` & `arctix-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: arctix
-Version: 0.0.3a1
-Summary: 
-Home-page: https://github.com/durandtibo/arctix
-License: BSD-3-Clause
-Author: Thibaut Durand
-Author-email: durand.tibo+gh@gmail.com
-Requires-Python: >=3.9,<3.13
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Provides-Extra: all
-Requires-Dist: batcharray (>=0.0.2,<0.1)
-Requires-Dist: coola (>=0.6,<1.0)
-Requires-Dist: gdown (>=5.0,<6.0) ; extra == "all"
-Requires-Dist: iden (>=0.0.3,<1.0)
-Requires-Dist: matplotlib (>=3.6,<4.0) ; extra == "all"
-Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: polars (>=0.20.0,<1.0)
-Requires-Dist: requests (>=2.20,<3.0) ; extra == "all"
-Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all"
-Project-URL: Repository, https://github.com/durandtibo/arctix
-Description-Content-Type: text/markdown
-
 # arctix
 
 <p align="center">
     <a href="https://github.com/durandtibo/arctix/actions">
         <img alt="CI" src="https://github.com/durandtibo/arctix/workflows/CI/badge.svg">
     </a>
     <a href="https://github.com/durandtibo/arctix/actions">
@@ -91,26 +58,52 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/arctix/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-TODO
+The `arctix` package consists of functionalities to prepare dataset of asynchronous time series.
+It is design to make dataset preparation reusable and reproducible.
+For each dataset, `arctix` provides 3 main functions:
+
+- `fetch_data` to load the raw data are loaded in
+  a [`polars.DataFrame`](https://docs.pola.rs/py-polars/html/reference/dataframe/index.html). When
+  possible, it downloads automatically the data.
+- `prepare_data` to prepare the data. It outputs the prepared data
+  in [`polars.DataFrame`](https://docs.pola.rs/py-polars/html/reference/dataframe/index.html), and
+  the metadata.
+- `to_array` to convert the prepared data to a dictionary of numpy arrays.
+
+For example, it is possible to use the following lines to download and prepare the MultiTHUMOS data.
+
+```pycon
+
+>>> from pathlib import Path
+>>> from arctix.dataset.multithumos import fetch_data, prepare_data, to_array
+>>> dataset_path = Path("/path/to/dataset/multithumos")
+>>> data_raw = fetch_data(dataset_path)  # doctest: +SKIP
+>>> data, metadata = prepare_data(data_raw)  # doctest: +SKIP
+>>> arrays = to_array(data)  # doctest: +SKIP
+
+```
 
-- [Motivation](#motivation)
 - [Documentation](https://durandtibo.github.io/arctix/)
 - [Installation](#installation)
 - [Contributing](#contributing)
 - [API stability](#api-stability)
 - [License](#license)
 
-## Motivation
+## Documentation
 
-TODO
+- [latest (stable)](https://durandtibo.github.io/arctix/): documentation from the latest stable
+  release.
+- [main (unstable)](https://durandtibo.github.io/arctix/main/): documentation associated to the
+  main branch of the repo. This documentation may contain a lot of work-in-progress/outdated/missing
+  parts.
 
 ## Installation
 
 We highly recommend installing
 a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
 `arctix` can be installed from pip using the following command:
 
@@ -124,14 +117,21 @@
 
 ```shell
 pip install arctix[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/arctix/get_started) to see how to
 install only some specific packages or other alternatives to install the library.
+The following is the corresponding `karbonn` versions and dependencies.
+
+| `batcharray` | `batcharray`   | `coola`      | `iden`           | `numpy`       | `polars`        | `python`      |
+|--------------|----------------|--------------|------------------|---------------|-----------------|---------------|
+| `main`       | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
+| `0.0.4`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
+| `0.0.3`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
 
 ## API stability
 
@@ -141,8 +141,7 @@
 In practice, this means that upgrading `arctix` to a new version will possibly break any code that
 was using the old version of `arctix`.
 
 ## License
 
 `arctix` is licensed under BSD 3-Clause "New" or "Revised" license available in [LICENSE](LICENSE)
 file.
-
```

#### html2text {}

```diff
@@ -1,46 +1,55 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.3a1 Summary: Home-page: https:/
-/github.com/durandtibo/arctix License: BSD-3-Clause Author: Thibaut Durand
-Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Provides-Extra: all Requires-Dist: batcharray
-(>=0.0.2,<0.1) Requires-Dist: coola (>=0.6,<1.0) Requires-Dist: gdown
-(>=5.0,<6.0) ; extra == "all" Requires-Dist: iden (>=0.0.3,<1.0) Requires-Dist:
-matplotlib (>=3.6,<4.0) ; extra == "all" Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: polars (>=0.20.0,<1.0) Requires-Dist: requests (>=2.20,<3.0) ;
-extra == "all" Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all" Project-URL:
-Repository, https://github.com/durandtibo/arctix Description-Content-Type:
-text/markdown # arctix
+# arctix
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_M_o_n_t_h_l_y_ _d_o_w_n_l_o_a_d_s_]
-## Overview TODO - [Motivation](#motivation) - [Documentation](https://
+## Overview The `arctix` package consists of functionalities to prepare dataset
+of asynchronous time series. It is design to make dataset preparation reusable
+and reproducible. For each dataset, `arctix` provides 3 main functions: -
+`fetch_data` to load the raw data are loaded in a [`polars.DataFrame`](https://
+docs.pola.rs/py-polars/html/reference/dataframe/index.html). When possible, it
+downloads automatically the data. - `prepare_data` to prepare the data. It
+outputs the prepared data in [`polars.DataFrame`](https://docs.pola.rs/py-
+polars/html/reference/dataframe/index.html), and the metadata. - `to_array` to
+convert the prepared data to a dictionary of numpy arrays. For example, it is
+possible to use the following lines to download and prepare the MultiTHUMOS
+data. ```pycon >>> from pathlib import Path >>> from arctix.dataset.multithumos
+import fetch_data, prepare_data, to_array >>> dataset_path = Path("/path/to/
+dataset/multithumos") >>> data_raw = fetch_data(dataset_path) # doctest: +SKIP
+>>> data, metadata = prepare_data(data_raw) # doctest: +SKIP >>> arrays =
+to_array(data) # doctest: +SKIP ``` - [Documentation](https://
 durandtibo.github.io/arctix/) - [Installation](#installation) - [Contributing]
 (#contributing) - [API stability](#api-stability) - [License](#license) ##
-Motivation TODO ## Installation We highly recommend installing a [virtual
+Documentation - [latest (stable)](https://durandtibo.github.io/arctix/):
+documentation from the latest stable release. - [main (unstable)](https://
+durandtibo.github.io/arctix/main/): documentation associated to the main branch
+of the repo. This documentation may contain a lot of work-in-progress/outdated/
+missing parts. ## Installation We highly recommend installing a [virtual
 environment](https://packaging.python.org/guides/installing-using-pip-and-
 virtual-environments/). `arctix` can be installed from pip using the following
 command: ```shell pip install arctix ``` To make the package as slim as
 possible, only the minimal packages required to use `arctix` are installed. To
 include all the packages, you can use the following command: ```shell pip
 install arctix[all] ``` Please check the [get started page](https://
 durandtibo.github.io/arctix/get_started) to see how to install only some
-specific packages or other alternatives to install the library. ## Contributing
-Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ##
-API stability :warning: While `arctix` is in development stage, no API is
-guaranteed to be stable from one release to the next. In fact, it is very
-likely that the API will change multiple times before a stable 1.0.0 release.
-In practice, this means that upgrading `arctix` to a new version will possibly
-break any code that was using the old version of `arctix`. ## License `arctix`
-is licensed under BSD 3-Clause "New" or "Revised" license available in
+specific packages or other alternatives to install the library. The following
+is the corresponding `karbonn` versions and dependencies. | `batcharray` |
+`batcharray` | `coola` | `iden` | `numpy` | `polars` | `python` | |------------
+--|----------------|--------------|------------------|---------------|---------
+--------|---------------| | `main` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.4`
+| `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` |
+`>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.3` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | ##
+Contributing Please check the instructions in [CONTRIBUTING.md](.github/
+CONTRIBUTING.md). ## API stability :warning: While `arctix` is in development
+stage, no API is guaranteed to be stable from one release to the next. In fact,
+it is very likely that the API will change multiple times before a stable 1.0.0
+release. In practice, this means that upgrading `arctix` to a new version will
+possibly break any code that was using the old version of `arctix`. ## License
+`arctix` is licensed under BSD 3-Clause "New" or "Revised" license available in
 [LICENSE](LICENSE) file.
```

