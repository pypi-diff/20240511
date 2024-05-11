# Comparing `tmp/meds_etl_cpp-0.2.0.tar.gz` & `tmp/meds_etl_cpp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl_cpp-0.2.0.tar", last modified: Sat May  4 21:50:42 2024, max compression
+gzip compressed data, was "meds_etl_cpp-0.2.1.tar", last modified: Sat May 11 05:11:13 2024, max compression
```

## Comparing `meds_etl_cpp-0.2.0.tar` & `meds_etl_cpp-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.726822 meds_etl_cpp-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.718821 meds_etl_cpp-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.722821 meds_etl_cpp-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/.github/workflows/python-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-04 21:50:42.726822 meds_etl_cpp-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.726822 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-04 21:50:42.000000 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-04 21:50:42.000000 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:50:42.000000 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:50:42.000000 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 21:50:42.000000 meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.722821 meds_etl_cpp-0.2.0/native/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/.bazelrc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/WORKSPACE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/backupbazelrc
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/meds_etl_cpp.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:50:42.726822 meds_etl_cpp-0.2.0/native/patches/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/patches/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/patches/ThirdpartyToolchain.cmake.patch
--rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/pdqsort.h
--rw-r--r--   0 runner    (1001) docker     (127)    49548 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/perform_etl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/perform_etl.hh
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/native/simple_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:50:42.726822 meds_etl_cpp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-04 21:50:38.000000 meds_etl_cpp-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.740902 meds_etl_cpp-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.740902 meds_etl_cpp-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 05:11:13.000000 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-11 05:11:13.000000 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 05:11:13.000000 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 05:11:13.000000 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 05:11:13.000000 meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/.bazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/WORKSPACE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/backupbazelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/meds_etl_cpp.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/native/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/patches/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/patches/ThirdpartyToolchain.cmake.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/pdqsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48720 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/perform_etl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/perform_etl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/native/simple_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 05:11:13.744902 meds_etl_cpp-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-11 05:11:10.000000 meds_etl_cpp-0.2.1/setup.py
```

### Comparing `meds_etl_cpp-0.2.0/.github/workflows/python-build.yml` & `meds_etl_cpp-0.2.1/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/LICENSE` & `meds_etl_cpp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/meds_etl_cpp.egg-info/SOURCES.txt` & `meds_etl_cpp-0.2.1/meds_etl_cpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/native/BUILD` & `meds_etl_cpp-0.2.1/native/BUILD`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/native/WORKSPACE` & `meds_etl_cpp-0.2.1/native/WORKSPACE`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/native/patches/ThirdpartyToolchain.cmake.patch` & `meds_etl_cpp-0.2.1/native/patches/ThirdpartyToolchain.cmake.patch`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/native/pdqsort.h` & `meds_etl_cpp-0.2.1/native/pdqsort.h`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/native/perform_etl.cc` & `meds_etl_cpp-0.2.1/native/perform_etl.cc`

 * *Files 15% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 }
 
 const std::vector<std::string> known_fields = {
     "patient_id",    "time",           "code",
     "numeric_value", "datetime_value", "text_value"};
 
 std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
-get_metadata_fields(const std::vector<std::string>& files) {
+get_properties_fields(const std::vector<std::string>& files) {
     arrow::MemoryPool* pool = arrow::default_memory_pool();
     std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>> result;
 
     for (const auto& file : files) {
         auto fields = get_fields_for_file(pool, file);
         for (const auto& field : fields) {
             if (field->name() == "value") {
@@ -115,31 +115,31 @@
         }
     }
 
     return result;
 }
 
 std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
-get_metadata_fields_multithreaded(const std::vector<std::string>& files,
-                                  size_t num_threads) {
+get_properties_fields_multithreaded(const std::vector<std::string>& files,
+                                    size_t num_threads) {
     std::vector<std::thread> threads;
     std::vector<
         std::set<std::pair<std::string, std::shared_ptr<arrow::DataType>>>>
         results(num_threads);
 
     size_t files_per_thread = (files.size() + num_threads - 1) / num_threads;
 
     for (size_t i = 0; i < num_threads; i++) {
         threads.emplace_back([&files, i, &results, files_per_thread]() {
             std::vector<std::string> fraction;
             for (size_t j = files_per_thread * i;
                  j < std::min(files.size(), files_per_thread * (i + 1)); j++) {
                 fraction.push_back(files[j]);
             }
-            results[i] = get_metadata_fields(fraction);
+            results[i] = get_properties_fields(fraction);
         });
     }
 
     for (auto& thread : threads) {
         thread.join();
     }
 
@@ -171,15 +171,15 @@
     size_t reader_index, size_t num_shards,
     moodycamel::BlockingConcurrentQueue<absl::optional<std::string>>&
         file_queue,
     std::vector<moodycamel::BlockingConcurrentQueue<QueueItem>>&
         all_write_queues,
     moodycamel::LightweightSemaphore& all_write_semaphore,
     const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
-        metadata_columns) {
+        properties_columns) {
     arrow::MemoryPool* pool = arrow::default_memory_pool();
 
     std::vector<moodycamel::ProducerToken> ptoks;
     for (size_t i = 0; i < num_shards; i++) {
         ptoks.emplace_back(all_write_queues[i]);
     }
 
@@ -216,18 +216,18 @@
             int time_index = -1;
             int code_index = -1;
 
             int numeric_value_index = -1;
             int datetime_value_index = -1;
             int text_value_index = -1;
 
-            std::vector<int> metadata_indices(metadata_columns.size(), -1);
+            std::vector<int> properties_indices(properties_columns.size(), -1);
 
             std::bitset<std::numeric_limits<unsigned long long>::digits>
-                is_text_metadata;
+                is_text_properties;
 
             const auto& manifest = arrow_reader->manifest();
             for (const auto& schema_field : manifest.schema_fields) {
                 if (schema_field.children.size() != 0 ||
                     !schema_field.is_leaf()) {
                     throw std::runtime_error(
                         "For MEDS-Flat fields should not be nested, but we "
@@ -287,50 +287,51 @@
                         throw std::runtime_error(
                             "C++ MEDS-Flat requires Float32 numeric_value but "
                             "found " +
                             schema_field.field->ToString());
                     }
                     text_value_index = schema_field.column_index;
                 } else {
-                    // Must be metadata
+                    // Must be properties
                     auto iter = std::find_if(
-                        std::begin(metadata_columns),
-                        std::end(metadata_columns), [&](const auto& entry) {
+                        std::begin(properties_columns),
+                        std::end(properties_columns), [&](const auto& entry) {
                             return entry.first == schema_field.field->name();
                         });
-                    if (iter == std::end(metadata_columns)) {
+                    if (iter == std::end(properties_columns)) {
                         throw std::runtime_error(
-                            "Had an extra column in the metadata that "
+                            "Had an extra column in the properties that "
                             "shouldn't exist? " +
                             schema_field.field->ToString());
                     }
 
                     if (!schema_field.field->type()->Equals(iter->second)) {
                         throw std::runtime_error(
-                            "C++ MEDS-Flat requires large_string metadata but "
+                            "C++ MEDS-Flat requires large_string properties "
+                            "but "
                             "found " +
                             schema_field.field->ToString());
                     }
 
-                    int offset = (iter - std::begin(metadata_columns));
+                    int offset = (iter - std::begin(properties_columns));
 
                     if (iter->second->Equals(arrow::LargeStringType())) {
-                        is_text_metadata[offset] = true;
+                        is_text_properties[offset] = true;
                     } else {
-                        is_text_metadata[offset] = false;
+                        is_text_properties[offset] = false;
 
                         if (iter->second->byte_width() == -1) {
                             throw std::runtime_error(
-                                "Found non text metadata with unknown byte "
+                                "Found non text properties with unknown byte "
                                 "width? " +
                                 iter->second->ToString());
                         }
                     }
 
-                    metadata_indices[offset] = schema_field.column_index;
+                    properties_indices[offset] = schema_field.column_index;
                 }
             }
 
             if (patient_id_index == -1) {
                 throw std::runtime_error(
                     "Could not find patient_id column index");
             }
@@ -397,52 +398,54 @@
                     std::dynamic_pointer_cast<arrow::LargeStringArray>(
                         record_batch->column(text_value_index));
                 if (!text_value_array) {
                     throw std::runtime_error("Could not cast text_value array");
                 }
 
                 std::vector<std::shared_ptr<arrow::LargeStringArray>>
-                    text_metadata_arrays(metadata_columns.size());
+                    text_properties_arrays(properties_columns.size());
                 std::vector<std::shared_ptr<arrow::FixedSizeBinaryArray>>
-                    primitive_metadata_arrays(metadata_columns.size());
+                    primitive_properties_arrays(properties_columns.size());
 
-                for (size_t i = 0; i < metadata_columns.size(); i++) {
-                    if (metadata_indices[i] == -1) {
+                for (size_t i = 0; i < properties_columns.size(); i++) {
+                    if (properties_indices[i] == -1) {
                         continue;
                     }
 
-                    if (is_text_metadata[i]) {
-                        auto metadata_array =
+                    if (is_text_properties[i]) {
+                        auto properties_array =
                             std::dynamic_pointer_cast<arrow::LargeStringArray>(
-                                record_batch->column(metadata_indices[i]));
-                        if (!metadata_array) {
+                                record_batch->column(properties_indices[i]));
+                        if (!properties_array) {
                             throw std::runtime_error(
-                                "Could not cast metadata array to text" +
-                                metadata_columns[i].first + " " +
-                                metadata_columns[i].second->ToString());
+                                "Could not cast properties array to text" +
+                                properties_columns[i].first + " " +
+                                properties_columns[i].second->ToString());
                         }
-                        text_metadata_arrays[i] = metadata_array;
+                        text_properties_arrays[i] = properties_array;
                     } else {
                         std::shared_ptr<arrow::Array> fixed_size_array;
                         PARQUET_ASSIGN_OR_THROW(
                             fixed_size_array,
-                            record_batch->column(metadata_indices[i])
+                            record_batch->column(properties_indices[i])
                                 ->View(std::make_shared<
                                        arrow::FixedSizeBinaryType>(
-                                    metadata_columns[i].second->byte_width())));
+                                    properties_columns[i]
+                                        .second->byte_width())));
 
-                        auto metadata_array = std::dynamic_pointer_cast<
+                        auto properties_array = std::dynamic_pointer_cast<
                             arrow::FixedSizeBinaryArray>(fixed_size_array);
-                        if (!metadata_array) {
+                        if (!properties_array) {
                             throw std::runtime_error(
-                                "Could not cast metadata array to fixed size " +
-                                metadata_columns[i].first + " " +
-                                metadata_columns[i].second->ToString());
+                                "Could not cast properties array to fixed "
+                                "size " +
+                                properties_columns[i].first + " " +
+                                properties_columns[i].second->ToString());
                         }
-                        primitive_metadata_arrays[i] = metadata_array;
+                        primitive_properties_arrays[i] = properties_array;
                     }
                 }
 
                 for (int64_t i = 0; i < text_value_array->length(); i++) {
                     if (!patient_id_array->IsValid(i)) {
                         throw std::runtime_error(
                             "patient_id incorrectly has null value " + source);
@@ -482,29 +485,29 @@
                     }
 
                     if (text_value_array->IsValid(i)) {
                         non_null[2] = true;
                         add_string_to_vector(data, text_value_array->Value(i));
                     }
 
-                    for (size_t j = 0; j < metadata_columns.size(); j++) {
-                        if (is_text_metadata[j]) {
-                            if (text_metadata_arrays[j] &&
-                                text_metadata_arrays[j]->IsValid(i)) {
+                    for (size_t j = 0; j < properties_columns.size(); j++) {
+                        if (is_text_properties[j]) {
+                            if (text_properties_arrays[j] &&
+                                text_properties_arrays[j]->IsValid(i)) {
                                 non_null[3 + j] = true;
                                 add_string_to_vector(
-                                    data, text_metadata_arrays[j]->Value(i));
+                                    data, text_properties_arrays[j]->Value(i));
                             }
                         } else {
-                            if (primitive_metadata_arrays[j] &&
-                                primitive_metadata_arrays[j]->IsValid(i)) {
+                            if (primitive_properties_arrays[j] &&
+                                primitive_properties_arrays[j]->IsValid(i)) {
                                 non_null[3 + j] = true;
                                 add_string_to_vector(
                                     data,
-                                    primitive_metadata_arrays[j]->GetView(i));
+                                    primitive_properties_arrays[j]->GetView(i));
                             }
                         }
                     }
 
                     add_literal_to_vector(data, non_null.to_ullong());
 
                     size_t index =
@@ -853,47 +856,47 @@
 
     std::vector<std::string> paths;
 
     for (const auto& entry : fs::directory_iterator(source_directory)) {
         paths.push_back(entry.path());
     }
 
-    auto set_metadata_fields =
-        get_metadata_fields_multithreaded(paths, num_shards);
+    auto set_properties_fields =
+        get_properties_fields_multithreaded(paths, num_shards);
 
     std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>
-        metadata_columns(std::begin(set_metadata_fields),
-                         std::end(set_metadata_fields));
-    std::sort(std::begin(metadata_columns), std::end(metadata_columns));
-
-    metadata_columns.erase(
-        std::unique(std::begin(metadata_columns), std::end(metadata_columns),
-                    [](const auto& a, const auto& b) {
-                        return (a.first == b.first) &&
-                               a.second->Equals(b.second);
-                    }),
-        std::end(metadata_columns));
+        properties_columns(std::begin(set_properties_fields),
+                           std::end(set_properties_fields));
+    std::sort(std::begin(properties_columns), std::end(properties_columns));
+
+    properties_columns.erase(std::unique(std::begin(properties_columns),
+                                         std::end(properties_columns),
+                                         [](const auto& a, const auto& b) {
+                                             return (a.first == b.first) &&
+                                                    a.second->Equals(b.second);
+                                         }),
+                             std::end(properties_columns));
 
-    for (ssize_t i = 0; i < static_cast<ssize_t>(metadata_columns.size()) - 1;
+    for (ssize_t i = 0; i < static_cast<ssize_t>(properties_columns.size()) - 1;
          i++) {
-        if (metadata_columns[i].first == metadata_columns[i + 1].first) {
+        if (properties_columns[i].first == properties_columns[i + 1].first) {
             throw std::runtime_error(
                 "Got conflicting types for column " +
-                metadata_columns[i].first +
-                ", types: " + metadata_columns[i].second->ToString() + " vs " +
-                metadata_columns[i + 1].second->ToString());
+                properties_columns[i].first +
+                ", types: " + properties_columns[i].second->ToString() +
+                " vs " + properties_columns[i + 1].second->ToString());
         }
     }
 
-    if (metadata_columns.size() + 3 >
+    if (properties_columns.size() + 3 >
         std::numeric_limits<unsigned long long>::digits) {
         throw std::runtime_error(
             "C++ MEDS-ETL currently only supports at most " +
             std::to_string(std::numeric_limits<unsigned long long>::digits) +
-            " metadata columns");
+            " properties columns");
     }
 
     moodycamel::BlockingConcurrentQueue<absl::optional<std::string>> file_queue;
 
     for (const auto& path : paths) {
         file_queue.enqueue(path);
     }
@@ -910,17 +913,17 @@
     moodycamel::LightweightSemaphore write_semaphore(QUEUE_SIZE * num_shards);
 
     moodycamel::BlockingConcurrentQueue<std::string> sort_queue;
     std::atomic<ssize_t> remaining_live_writers(num_shards);
 
     for (size_t i = 0; i < num_shards; i++) {
         threads.emplace_back([i, &file_queue, &write_queues, &write_semaphore,
-                              num_shards, &metadata_columns]() {
+                              num_shards, &properties_columns]() {
             shard_reader(i, num_shards, file_queue, write_queues,
-                         write_semaphore, metadata_columns);
+                         write_semaphore, properties_columns);
         });
 
         threads.emplace_back([i, &write_queues, &write_semaphore, num_shards,
                               target_directory, &sort_queue,
                               &remaining_live_writers]() {
             shard_writer(i, num_shards, write_queues[i], write_semaphore,
                          target_directory / std::to_string(i), sort_queue,
@@ -941,75 +944,68 @@
     absl::optional<std::string> next_entry;
     if (sort_queue.try_dequeue(next_entry)) {
         // This should not be possible
         throw std::runtime_error(
             "Had excess unsorted items. This should not be possible");
     }
 
-    return metadata_columns;
+    return properties_columns;
 }
 
 void join_and_write_single(
     const std::filesystem::path& source_directory,
     const std::filesystem::path& target_path,
     const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
-        metadata_columns) {
-    arrow::FieldVector metadata_fields;
+        properties_columns) {
+    arrow::FieldVector properties_fields;
     std::bitset<std::numeric_limits<unsigned long long>::digits>
-        is_text_metadata;
-    for (size_t i = 0; i < metadata_columns.size(); i++) {
-        const auto& metadata_column = metadata_columns[i];
-        if (metadata_column.second->Equals(arrow::LargeStringType())) {
-            is_text_metadata[i] = true;
-            metadata_fields.push_back(arrow::field(
-                metadata_column.first, std::make_shared<arrow::StringType>()));
+        is_text_properties;
+    for (size_t i = 0; i < properties_columns.size(); i++) {
+        const auto& properties_column = properties_columns[i];
+        if (properties_column.second->Equals(arrow::LargeStringType())) {
+            is_text_properties[i] = true;
+            properties_fields.push_back(
+                arrow::field(properties_column.first,
+                             std::make_shared<arrow::StringType>()));
         } else {
-            is_text_metadata[i] = false;
-            metadata_fields.push_back(
-                arrow::field(metadata_column.first, metadata_column.second));
+            is_text_properties[i] = false;
+            properties_fields.push_back(arrow::field(properties_column.first,
+                                                     properties_column.second));
         }
     }
 
-    std::shared_ptr<arrow::DataType> metadata_type;
-    if (metadata_columns.size() != 0) {
-        metadata_type = std::make_shared<arrow::StructType>(metadata_fields);
+    std::shared_ptr<arrow::DataType> properties_type;
+    if (properties_columns.size() != 0) {
+        properties_type =
+            std::make_shared<arrow::StructType>(properties_fields);
     } else {
-        metadata_type = std::make_shared<arrow::FloatType>();
+        properties_type = std::make_shared<arrow::FloatType>();
     }
 
     auto timestamp_type =
         std::make_shared<arrow::TimestampType>(arrow::TimeUnit::MICRO);
 
-    auto measurement_type_fields = {
+    auto event_type_fields = {
+        arrow::field("time", std::make_shared<arrow::TimestampType>(
+                                 arrow::TimeUnit::MICRO)),
+
         arrow::field("code", std::make_shared<arrow::StringType>()),
 
         arrow::field("text_value", std::make_shared<arrow::StringType>()),
         arrow::field("numeric_value", std::make_shared<arrow::FloatType>()),
         arrow::field("datetime_value", std::make_shared<arrow::TimestampType>(
                                            arrow::TimeUnit::MICRO)),
 
-        arrow::field("metadata", metadata_type),
-    };
-
-    auto measurement_type =
-        std::make_shared<arrow::StructType>(measurement_type_fields);
-
-    auto event_type_fields = {
-        arrow::field("time", std::make_shared<arrow::TimestampType>(
-                                 arrow::TimeUnit::MICRO)),
-        arrow::field("measurements",
-                     std::make_shared<arrow::ListType>(measurement_type)),
+        arrow::field("properties", properties_type),
     };
     auto event_type = std::make_shared<arrow::StructType>(event_type_fields);
     auto events_type = std::make_shared<arrow::ListType>(event_type);
 
     auto schema_fields = {
         arrow::field("patient_id", std::make_shared<arrow::Int64Type>()),
-        arrow::field("static_measurements",
-                     std::make_shared<arrow::NullType>()),
         arrow::field("events", events_type),
     };
     auto schema = std::make_shared<arrow::Schema>(schema_fields);
 
     using parquet::ArrowWriterProperties;
     using parquet::WriterProperties;
 
@@ -1062,100 +1058,88 @@
 
         queue.push(std::make_tuple(std::get<0>(*next_entry),
                                    std::get<1>(*next_entry), i,
                                    std::get<2>(*next_entry)));
     }
 
     auto patient_id_builder = std::make_shared<arrow::Int64Builder>(pool);
-    auto static_measurements_builder =
-        std::make_shared<arrow::NullBuilder>(pool);
 
     auto code_builder = std::make_shared<arrow::StringBuilder>(pool);
 
     auto text_value_builder = std::make_shared<arrow::StringBuilder>(pool);
     auto numeric_value_builder = std::make_shared<arrow::FloatBuilder>(pool);
     auto datetime_value_builder =
         std::make_shared<arrow::TimestampBuilder>(timestamp_type, pool);
 
-    std::vector<std::shared_ptr<arrow::StringBuilder>> text_metadata_builders(
-        metadata_columns.size());
+    std::vector<std::shared_ptr<arrow::StringBuilder>> text_properties_builders(
+        properties_columns.size());
     std::vector<std::shared_ptr<arrow::FixedSizeBinaryBuilder>>
-        primitive_metadata_builders(metadata_columns.size());
+        primitive_properties_builders(properties_columns.size());
 
-    std::shared_ptr<arrow::StructBuilder> metadata_builder;
-    std::shared_ptr<arrow::FloatBuilder> null_metadata_builder;
-    std::shared_ptr<arrow::ArrayBuilder> metadata_builder_holder;
-
-    if (metadata_columns.size() != 0) {
-        std::vector<std::shared_ptr<arrow::ArrayBuilder>> metadata_builders(
-            metadata_columns.size());
-        for (size_t i = 0; i < metadata_columns.size(); i++) {
-            if (is_text_metadata[i]) {
+    std::shared_ptr<arrow::StructBuilder> properties_builder;
+    std::shared_ptr<arrow::FloatBuilder> null_properties_builder;
+    std::shared_ptr<arrow::ArrayBuilder> properties_builder_holder;
+
+    if (properties_columns.size() != 0) {
+        std::vector<std::shared_ptr<arrow::ArrayBuilder>> properties_builders(
+            properties_columns.size());
+        for (size_t i = 0; i < properties_columns.size(); i++) {
+            if (is_text_properties[i]) {
                 auto builder = std::make_shared<arrow::StringBuilder>(pool);
-                text_metadata_builders[i] = builder;
-                metadata_builders[i] = builder;
+                text_properties_builders[i] = builder;
+                properties_builders[i] = builder;
             } else {
                 auto builder = std::make_shared<arrow::FixedSizeBinaryBuilder>(
                     std::make_shared<arrow::FixedSizeBinaryType>(
-                        metadata_columns[i].second->byte_width()));
-                primitive_metadata_builders[i] = builder;
-                metadata_builders[i] = builder;
+                        properties_columns[i].second->byte_width()));
+                primitive_properties_builders[i] = builder;
+                properties_builders[i] = builder;
             }
         }
 
-        metadata_builder = std::make_shared<arrow::StructBuilder>(
-            metadata_type, pool, metadata_builders);
-        metadata_builder_holder = metadata_builder;
+        properties_builder = std::make_shared<arrow::StructBuilder>(
+            properties_type, pool, properties_builders);
+        properties_builder_holder = properties_builder;
     } else {
-        null_metadata_builder = std::make_shared<arrow::FloatBuilder>(pool);
-        metadata_builder_holder = null_metadata_builder;
+        null_properties_builder = std::make_shared<arrow::FloatBuilder>(pool);
+        properties_builder_holder = null_properties_builder;
     }
 
-    std::vector<std::shared_ptr<arrow::ArrayBuilder>>
-        measurement_builder_fields{
-            code_builder, text_value_builder, numeric_value_builder,
-            datetime_value_builder, metadata_builder_holder};
-
-    auto measurement_builder = std::make_shared<arrow::StructBuilder>(
-        measurement_type, pool, measurement_builder_fields);
-
     auto time_builder =
         std::make_shared<arrow::TimestampBuilder>(timestamp_type, pool);
-    auto measurements_builder =
-        std::make_shared<arrow::ListBuilder>(pool, measurement_builder);
 
     std::vector<std::shared_ptr<arrow::ArrayBuilder>> event_builder_fields{
-        time_builder, measurements_builder};
+        time_builder,           code_builder,
+        text_value_builder,     numeric_value_builder,
+        datetime_value_builder, properties_builder_holder};
+
     auto event_builder = std::make_shared<arrow::StructBuilder>(
         event_type, pool, event_builder_fields);
 
     auto events_builder =
         std::make_shared<arrow::ListBuilder>(pool, event_builder);
 
     auto flush_arrays = [&]() {
-        std::vector<std::shared_ptr<arrow::Array>> columns(3);
+        std::vector<std::shared_ptr<arrow::Array>> columns(2);
         PARQUET_THROW_NOT_OK(patient_id_builder->Finish(columns.data() + 0));
-        PARQUET_THROW_NOT_OK(
-            static_measurements_builder->Finish(columns.data() + 1));
 
         std::shared_ptr<arrow::Array> events_array;
         PARQUET_THROW_NOT_OK(events_builder->Finish(&events_array));
-        PARQUET_ASSIGN_OR_THROW(columns[2], events_array->View(events_type));
+        PARQUET_ASSIGN_OR_THROW(columns[1], events_array->View(events_type));
 
         std::shared_ptr<arrow::Table> table =
             arrow::Table::Make(schema, columns);
 
         PARQUET_THROW_NOT_OK(writer->WriteTable(*table));
 
         amount_written = 0;
     };
 
     bool is_first = true;
     int64_t last_patient_id = -1;
-    int64_t last_time = -1;
 
     while (!queue.empty()) {
         auto next = std::move(queue.top());
         queue.pop();
 
         int64_t patient_id = std::get<0>(next);
         int64_t time = std::get<1>(next);
@@ -1166,32 +1150,22 @@
             is_first = false;
 
             if (amount_written > PARQUET_PIECE_SIZE) {
                 flush_arrays();
             }
 
             last_patient_id = patient_id;
-            last_time = time;
 
             PARQUET_THROW_NOT_OK(patient_id_builder->Append(patient_id));
-            PARQUET_THROW_NOT_OK(static_measurements_builder->AppendNull());
             PARQUET_THROW_NOT_OK(events_builder->Append());
-
-            PARQUET_THROW_NOT_OK(event_builder->Append());
-            PARQUET_THROW_NOT_OK(time_builder->Append(time));
-            PARQUET_THROW_NOT_OK(measurements_builder->Append());
-        } else if (time != last_time) {
-            last_time = time;
-
-            PARQUET_THROW_NOT_OK(event_builder->Append());
-            PARQUET_THROW_NOT_OK(time_builder->Append(time));
-            PARQUET_THROW_NOT_OK(measurements_builder->Append());
         }
 
-        PARQUET_THROW_NOT_OK(measurement_builder->Append());
+        PARQUET_THROW_NOT_OK(event_builder->Append());
+        PARQUET_THROW_NOT_OK(time_builder->Append(time));
+
         std::bitset<std::numeric_limits<unsigned long long>::digits> non_null(
             *reinterpret_cast<const unsigned long long*>(
                 patient_record.data() + patient_record.size() -
                 sizeof(unsigned long long)));
         size_t offset = sizeof(int64_t) * 2;
 
         size_t size = *reinterpret_cast<const size_t*>(
@@ -1226,41 +1200,41 @@
             PARQUET_THROW_NOT_OK(text_value_builder->Append(
                 patient_record.substr(offset, size)));
             offset += size;
         } else {
             PARQUET_THROW_NOT_OK(text_value_builder->AppendNull());
         }
 
-        if (metadata_columns.size() == 0) {
-            PARQUET_THROW_NOT_OK(null_metadata_builder->AppendNull());
+        if (properties_columns.size() == 0) {
+            PARQUET_THROW_NOT_OK(null_properties_builder->AppendNull());
         } else {
-            PARQUET_THROW_NOT_OK(metadata_builder->Append());
+            PARQUET_THROW_NOT_OK(properties_builder->Append());
 
-            for (size_t j = 0; j < metadata_columns.size(); j++) {
+            for (size_t j = 0; j < properties_columns.size(); j++) {
                 if (non_null[3 + j]) {
                     size_t size = *reinterpret_cast<const size_t*>(
                         patient_record.substr(offset).data());
                     offset += sizeof(size);
                     auto entry = patient_record.substr(offset, size);
 
-                    if (is_text_metadata[j]) {
+                    if (is_text_properties[j]) {
                         PARQUET_THROW_NOT_OK(
-                            text_metadata_builders[j]->Append(entry));
+                            text_properties_builders[j]->Append(entry));
                     } else {
                         PARQUET_THROW_NOT_OK(
-                            primitive_metadata_builders[j]->Append(entry));
+                            primitive_properties_builders[j]->Append(entry));
                     }
                     offset += size;
                 } else {
-                    if (is_text_metadata[j]) {
+                    if (is_text_properties[j]) {
                         PARQUET_THROW_NOT_OK(
-                            text_metadata_builders[j]->AppendNull());
+                            text_properties_builders[j]->AppendNull());
                     } else {
                         PARQUET_THROW_NOT_OK(
-                            primitive_metadata_builders[j]->AppendNull());
+                            primitive_properties_builders[j]->AppendNull());
                     }
                 }
             }
         }
 
         size_t file_index = std::get<2>(next);
         auto next_entry = source_files[file_index].get_next();
@@ -1279,32 +1253,32 @@
     PARQUET_THROW_NOT_OK(writer->Close());
 }
 
 void join_and_write(
     const std::filesystem::path& source_directory,
     const std::filesystem::path& target_directory,
     const std::vector<std::pair<std::string, std::shared_ptr<arrow::DataType>>>&
-        metadata_columns) {
+        properties_columns) {
     std::filesystem::create_directory(target_directory);
 
     std::vector<std::string> shards;
 
     for (const auto& entry : fs::directory_iterator(source_directory)) {
         shards.push_back(fs::relative(entry.path(), source_directory));
     }
 
     std::vector<std::thread> threads;
 
     for (const auto& shard : shards) {
-        threads.emplace_back(
-            [shard, &source_directory, &target_directory, &metadata_columns]() {
-                join_and_write_single(source_directory / shard,
-                                      target_directory / (shard + ".parquet"),
-                                      metadata_columns);
-            });
+        threads.emplace_back([shard, &source_directory, &target_directory,
+                              &properties_columns]() {
+            join_and_write_single(source_directory / shard,
+                                  target_directory / (shard + ".parquet"),
+                                  properties_columns);
+        });
     }
 
     for (auto& thread : threads) {
         thread.join();
     }
 }
 
@@ -1319,13 +1293,13 @@
         fs::copy_file(source_path / "metadata.json",
                       target_path / "metadata.json");
     }
 
     std::filesystem::path shard_path = target_path / "shards";
     std::filesystem::path data_path = target_path / "data";
 
-    auto metadata_columns =
+    auto properties_columns =
         sort_and_shard(source_path / "flat_data", shard_path, num_shards);
-    join_and_write(shard_path, data_path, metadata_columns);
+    join_and_write(shard_path, data_path, properties_columns);
 
     fs::remove_all(shard_path);
 }
```

### Comparing `meds_etl_cpp-0.2.0/pyproject.toml` & `meds_etl_cpp-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meds_etl_cpp-0.2.0/setup.py` & `meds_etl_cpp-0.2.1/setup.py`

 * *Files identical despite different names*

