# Comparing `tmp/rdf_doctor-1.1.4-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 59875 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 24-May-10 00:14 doctor/__init__.py
--rw-r--r--  2.0 unx     1754 b- defN 24-May-07 05:38 doctor/consts.py
--rw-r--r--  2.0 unx    81134 b- defN 24-May-07 05:38 doctor/doctor.py
+Zip file size: 75912 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       22 b- defN 24-May-10 00:14 dc/__init__.py
+-rw-r--r--  2.0 unx     1754 b- defN 24-May-07 05:38 dc/consts.py
+-rw-r--r--  2.0 unx    81131 b- defN 24-May-11 00:18 dc/doctor.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-11 08:06 doctor/__init__.py
+-rw-r--r--  2.0 unx     2092 b- defN 24-May-11 08:06 doctor/consts.py
+-rw-r--r--  2.0 unx    92088 b- defN 24-May-11 08:06 doctor/doctor.py
 -rw-r--r--  2.0 unx   134314 b- defN 24-May-07 05:38 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-May-07 05:38 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-May-07 05:38 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    10651 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      995 b- defN 24-May-10 00:15 rdf_doctor-1.1.4.dist-info/RECORD
-12 files, 230749 bytes uncompressed, 58195 bytes compressed:  74.8%
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10727 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1204 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/RECORD
+15 files, 325236 bytes uncompressed, 73928 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,7 +1,16 @@
+Filename: dc/__init__.py
+Comment: 
+
+Filename: dc/consts.py
+Comment: 
+
+Filename: dc/doctor.py
+Comment: 
+
 Filename: doctor/__init__.py
 Comment: 
 
 Filename: doctor/consts.py
 Comment: 
 
 Filename: doctor/doctor.py
@@ -12,26 +21,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/LICENSE
+Filename: rdf_doctor-1.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/METADATA
+Filename: rdf_doctor-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/WHEEL
+Filename: rdf_doctor-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.4.dist-info/RECORD
+Filename: rdf_doctor-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.4"
+__version__ = "1.1.5"
```

## doctor/consts.py

```diff
@@ -12,37 +12,45 @@
 EXTENSION_NT = ".nt"
 EXTENSION_TTL = ".ttl"
 EXTENSION_RDF = ".rdf"
 EXTENSION_XML = ".xml"
 EXTENSION_OWL = ".owl"
 EXTENSION_GZ = ".gz"
 EXTENSION_TAR_GZ = ".tar.gz"
+EXTENSION_XZ = ".xz"
+EXTENSION_TAR_XZ = ".tar.xz"
 EXTENSION_ZIP = ".zip"
 
 # Input file type
 FILE_TYPE_TTL = "ttl"
 FILE_TYPE_NT = "nt"
 FILE_TYPE_RDF_XML = "rdf_xml"
 FILE_TYPE_TTL_GZ = "ttl_gz"
 FILE_TYPE_NT_GZ = "nt_gz"
 FILE_TYPE_RDF_XML_GZ = "rdf_xml_gz"
+FILE_TYPE_TTL_XZ = "ttl_xz"
+FILE_TYPE_NT_XZ = "nt_xz"
+FILE_TYPE_RDF_XML_XZ = "rdf_xml_xz"
 FILE_TYPE_TTL_ZIP = "ttl_zip"
 FILE_TYPE_NT_ZIP = "nt_zip"
 FILE_TYPE_RDF_XML_ZIP = "rdf_xml_zip"
 
 FILE_TYPE_ALL = "all"
 
 # Dictionary of file type IDs and names
 FILE_TYPE_DICT = {
     FILE_TYPE_TTL: "Turtle(.ttl)",
     FILE_TYPE_NT: "N-Triples(.nt)",
     FILE_TYPE_RDF_XML: "RDF/XML(.rdf or .xml or .owl)",
     FILE_TYPE_TTL_GZ: "tar compressed Turtle(.ttl.gz)",
     FILE_TYPE_NT_GZ: "tar compressed N-Triples(.nt.gz)",
     FILE_TYPE_RDF_XML_GZ: "tar compressed RDF/XML(.rdf.gz and .xml.gz and .owl.gz)",
+    FILE_TYPE_TTL_XZ: "tar compressed Turtle(.ttl.xz)",
+    FILE_TYPE_NT_XZ: "tar compressed N-Triples(.nt.xz)",
+    FILE_TYPE_RDF_XML_XZ: "tar compressed RDF/XML(.rdf.xz and .xml.xz and .owl.xz)",
     FILE_TYPE_TTL_ZIP: "zip compressed Turtle(.ttl.zip)",
     FILE_TYPE_NT_ZIP: "zip compressed N-Triples(.nt.zip)",
     FILE_TYPE_RDF_XML_ZIP: "zip compressed RDF/XML(.rdf.zip and .xml.zip and .owl.zip)"
 }
 
 # Correct prefix list file path
 PREFIXES_FILE_PATH = "reference/prefixes.tsv"
```

## doctor/doctor.py

```diff
@@ -15,22 +15,24 @@
 import queue
 import shutil
 from unidecode import unidecode
 from collections import defaultdict
 from pathlib import Path
 import tempfile
 import uuid
+import xz
 from doctor.consts import VERSION_FILE, TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, \
                             EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL, EXTENSION_GZ, EXTENSION_ZIP, EXTENSION_TAR_GZ, \
+                            EXTENSION_XZ, EXTENSION_TAR_XZ, FILE_TYPE_TTL_XZ, FILE_TYPE_NT_XZ, FILE_TYPE_RDF_XML_XZ, \
                             PREFIXES_FILE_PATH, REFINE_CLASS_URIS_FILE_PATH, REFINE_PREFIX_URIS_FILE_PATH, HELP_LINK_URL, \
                             FILE_TYPE_TTL, FILE_TYPE_NT, FILE_TYPE_RDF_XML, FILE_TYPE_TTL_GZ, FILE_TYPE_NT_GZ, FILE_TYPE_RDF_XML_GZ, \
                             FILE_TYPE_TTL_ZIP, FILE_TYPE_NT_ZIP, FILE_TYPE_RDF_XML_ZIP, FILE_TYPE_ALL, FILE_TYPE_DICT, TMP_DISK_USAGE_LIMIT_DEFAULT
 
 from shexer.shaper import Shaper
-from shexer.consts import NT, TURTLE, TURTLE_ITER, RDF_XML, GZ, ZIP, MIXED_INSTANCES
+from shexer.consts import NT, TURTLE, TURTLE_ITER, RDF_XML, GZ, ZIP, XZ, MIXED_INSTANCES, ALL_EXAMPLES
 
 is_displaying_spinner = False
 in_progress_rdflib_query = False
 
 # Main processing of rdf-doctor
 def doctor():
     args = get_command_line_args(sys.argv[1:])
@@ -105,14 +107,15 @@
                 else:
                     input_format = input_file_list[2]
 
                 if args.verbose:
                     print_overwrite(get_dt_now() + " -- Start processing [" + ", ".join(str(input_file) for input_file in input_file_list[0]) + "]")
 
                 # Get and output result. If an error occurs, store it in a queue
+                #print_overwrite(get_dt_now() + " -- " + input_format + ":" + compression_mode)
                 executor_calc.submit(get_and_output_result, args, input_file_list[0], input_format, compression_mode, widely_used_prefixes_dict, refine_prefix_uris, refine_class_uris, error_queue)
 
             executor_calc.shutdown()
             if args.verbose:
                 is_displaying_spinner = False
                 executor_spinner.shutdown()
 
@@ -196,15 +199,15 @@
                         required=True,
                         nargs="+",
                         help='input RDF file or directory (Turtle(.ttl), N-Triples(.nt), RDF/XML(.rdf, .xml, .owl) and their compressed versions are supported)',
                         metavar="RDF-FILE or DIRECTORY")
 
     # Input file type (-t、--type)
     parser.add_argument("-t","--type",
-                        help='specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, ttl_gz, nt_gz, rdf_xml_gz, ttl_zip, nt_zip, rdf_xml_zip)')
+                        help='specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, ttl_gz, nt_gz, rdf_xml_gz, ttl_xz, nt_xz, rdf_xml_xz, ttl_zip, nt_zip, rdf_xml_zip)')
 
     # Add report to results (-r、--report)
     parser.add_argument("-r","--report",
                         action="store_true",
                         help="add report to results")
 
     # Output directory (-o、--output [DIRECTORY]、default: Standard output)
@@ -223,21 +226,21 @@
     parser.add_argument("-m","--merge",
                         action="store_true",
                         help="merge results by input file format")
 
     # Temporary directory (--tmp-dir [DIRECTORY]、default: Platform-dependent default temporary directory)
     parser.add_argument("--tmp-dir", type=str,
                         default=None,
-                        help='Temporary directory where the unzipped contents are placed when processing tar.gz or zip (default: Platform-dependent default temporary directory)',
+                        help='Temporary directory where the unzipped contents are placed when processing tar.gz, tar.xz, or zip (default: Platform-dependent default temporary directory)',
                         metavar="DIRECTORY")
 
     # Temporary directory usage upper limit(--tmp-dir-disk-usage-limit [percentage]、default: 95)
     parser.add_argument("--tmp-dir-disk-usage-limit", type=int,
                         default=TMP_DISK_USAGE_LIMIT_DEFAULT,
-                        help='Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zip. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)',
+                        help='Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz, tar.xz, or zip. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)',
                         metavar="PERCENTAGE")
 
     # Prefix URI dictionary file path(--prefix-uri-dict [FILE]、default: reference/refine-prefix-uris.tsv)
     parser.add_argument("--prefix-uri-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)),
                         help='path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)',
                         metavar="FILE")
@@ -280,14 +283,17 @@
 
     input_file_list_ttl = []            # Turtle(.ttl)
     input_file_list_nt = []             # N-Triples(.nt)
     input_file_list_rdf_xml = []        # RDF/XML(.rdf, .xml, .owl)
     input_file_list_ttl_gz = []         # GZ compressed Turtle(.ttl.gz)
     input_file_list_nt_gz = []          # GZ compressed N-Triples(.nt.gz)
     input_file_list_rdf_xml_gz = []     # GZ compressed RDF/XML(.rdf.gz, .xml.gz, .owl.gz)
+    input_file_list_ttl_xz = []         # XZ compressed Turtle(.ttl.xz)
+    input_file_list_nt_xz = []          # XZ compressed N-Triples(.nt.xz)
+    input_file_list_rdf_xml_xz = []     # XZ compressed RDF/XML(.rdf.xz, .xml.xz, .owl.xz)
     input_file_list_ttl_zip = []        # ZIP compressed Turtle(.ttl.zip)
     input_file_list_nt_zip = []         # ZIP compressed N-Triples(.nt.zip)
     input_file_list_rdf_xml_zip = []    # ZIP compressed RDF/XML(.rdf.zip, .xml.zip, .owl.zip)
     input_file_2d_list = []             # For storing final results
     exists_file_types = []
 
     # input_file_list_other = []        # Other than those above
@@ -313,14 +319,25 @@
                             input_file_list_nt_gz.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml_gz.append(file_path)
                         else:
                             # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
                             pass
 
+                    elif compression_mode == XZ:
+                        if input_format == TURTLE:
+                            input_file_list_ttl_xz.append(file_path)
+                        elif input_format == NT:
+                            input_file_list_nt_xz.append(file_path)
+                        elif input_format == RDF_XML:
+                            input_file_list_rdf_xml_xz.append(file_path)
+                        else:
+                            # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                            pass
+
                     elif compression_mode == ZIP:
                         if input_format == TURTLE:
                             input_file_list_ttl_zip.append(file_path)
                         elif input_format == NT:
                             input_file_list_nt_zip.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml_zip.append(file_path)
@@ -377,14 +394,97 @@
                                     elif input_format == NT:
                                         input_file_list_nt_gz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_gz.append(file_path)
                                     else:
                                         # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
                                         pass
+                                if compression_mode == XZ:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt_xz.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml_xz.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        pass
+                                elif compression_mode == ZIP:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl_zip.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt_zip.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml_zip.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        pass
+
+                                elif compression_mode is None:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl
+                                        pass
+                    else:
+                        error_msg = '1:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        return None, None, error_msg
+
+            elif compression_mode == XZ:
+                if input_format == TURTLE:
+                    input_file_list_ttl_xz.append(input_file)
+                elif input_format == NT:
+                    input_file_list_nt_xz.append(input_file)
+                elif input_format == RDF_XML:
+                    input_file_list_rdf_xml_xz.append(input_file)
+                else:
+                    extension = get_extension_before_compression(input_file) + "." + compression_mode
+
+                    if extension == EXTENSION_TAR_XZ:
+                        # Check disk usage percentage
+                        if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                            error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                            return None, None, error_msg
+
+                        extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
+                        # For .tar.xz, expand and process the contents
+                        with tarfile.open(input_file, 'r:xz') as tar:
+                            tar.extractall(extract_path)
+
+                        # Loop by recursively retrieving files in a directory
+                        for root, _, files in os.walk(top=extract_path):
+                            for file in files:
+                                file_path = Path(root) / file
+
+                                compression_mode = get_compression_mode(file_path)
+                                input_format = get_input_format(file_path, compression_mode)
+                                if compression_mode == GZ:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl_gz.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt_gz.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml_gz.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        pass
+                                elif compression_mode == XZ:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt_xz.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml_xz.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        pass
                                 elif compression_mode == ZIP:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_zip.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_zip.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_zip.append(file_path)
@@ -399,15 +499,15 @@
                                         input_file_list_nt.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml.append(file_path)
                                     else:
                                         # No processing except for .ttl, .nt, .rdf, .xml, .owl
                                         pass
                     else:
-                        error_msg = '"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        error_msg = '2:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                         return None, None, error_msg
 
             elif compression_mode == ZIP:
                 if input_format == TURTLE:
                     input_file_list_ttl_zip.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt_zip.append(input_file)
@@ -440,14 +540,25 @@
                                         input_file_list_nt_gz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_gz.append(file_path)
                                     else:
                                         # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
                                         pass
 
+                                elif compression_mode == XZ:
+                                    if input_format == TURTLE:
+                                        input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == NT:
+                                        input_file_list_nt_xz.append(file_path)
+                                    elif input_format == RDF_XML:
+                                        input_file_list_rdf_xml_xz.append(file_path)
+                                    else:
+                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        pass
+
                                 elif compression_mode == ZIP:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_zip.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_zip.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_zip.append(file_path)
@@ -462,26 +573,26 @@
                                         input_file_list_nt.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml.append(file_path)
                                     else:
                                         # No processing except for .ttl, .nt, .rdf, .xml, .owl
                                         pass
                     else:
-                        error_msg = '"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        error_msg = '3:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                         return None, None, error_msg
 
             elif compression_mode is None:
                 if input_format == TURTLE:
                     input_file_list_ttl.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml.append(input_file)
                 else:
-                    error_msg = '"' + get_extension(input_file) + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                    error_msg = '4:"' + get_extension(input_file) + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                     return None, None, error_msg
 
     if len(input_file_list_ttl) != 0:
         # input_file_dict[FILE_TYPE_TTL] = [input_file_list_ttl, None, TURTLE]
         input_file_2d_list.append([input_file_list_ttl, None, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL)
     if len(input_file_list_nt) != 0:
@@ -492,22 +603,34 @@
         # input_file_dict[FILE_TYPE_RDF_XML] = [input_file_list_rdf_xml, None, RDF_XML]
         input_file_2d_list.append([input_file_list_rdf_xml, None, RDF_XML])
         exists_file_types.append(FILE_TYPE_RDF_XML)
     if len(input_file_list_ttl_gz) != 0:
         # input_file_dict[FILE_TYPE_TTL_GZ] = [input_file_list_ttl_gz, GZ, TURTLE]
         input_file_2d_list.append([input_file_list_ttl_gz, GZ, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL_GZ)
+    if len(input_file_list_ttl_xz) != 0:
+        # input_file_dict[FILE_TYPE_TTL_XZ] = [input_file_list_ttl_xz, XZ, TURTLE]
+        input_file_2d_list.append([input_file_list_ttl_xz, XZ, TURTLE])
+        exists_file_types.append(FILE_TYPE_TTL_XZ)
     if len(input_file_list_nt_gz) != 0:
         # input_file_dict[FILE_TYPE_NT_GZ] = [input_file_list_nt_gz, GZ, NT]
         input_file_2d_list.append([input_file_list_nt_gz, GZ, NT])
         exists_file_types.append(FILE_TYPE_NT_GZ)
+    if len(input_file_list_nt_xz) != 0:
+        # input_file_dict[FILE_TYPE_NT_XZ] = [input_file_list_nt_xz, XZ, NT]
+        input_file_2d_list.append([input_file_list_nt_xz, XZ, NT])
+        exists_file_types.append(FILE_TYPE_NT_XZ)
     if len(input_file_list_rdf_xml_gz) != 0:
         # input_file_dict[FILE_TYPE_RDF_XML_GZ] = [input_file_list_rdf_xml_gz, GZ, RDF_XML]
         input_file_2d_list.append([input_file_list_rdf_xml_gz, GZ, RDF_XML])
         exists_file_types.append(FILE_TYPE_RDF_XML_GZ)
+    if len(input_file_list_rdf_xml_xz) != 0:
+        # input_file_dict[FILE_TYPE_RDF_XML_XZ] = [input_file_list_rdf_xml_xz, XZ, RDF_XML]
+        input_file_2d_list.append([input_file_list_rdf_xml_xz, XZ, RDF_XML])
+        exists_file_types.append(FILE_TYPE_RDF_XML_XZ)
     if len(input_file_list_ttl_zip) != 0:
         # input_file_dict[FILE_TYPE_TTL_ZIP] = [input_file_list_ttl_zip, ZIP, TURTLE]
         input_file_2d_list.append([input_file_list_ttl_zip, ZIP, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL_ZIP)
     if len(input_file_list_nt_zip) != 0:
         # input_file_dict[FILE_TYPE_NT_ZIP] = [input_file_list_nt_zip, ZIP, NT]
         input_file_2d_list.append([input_file_list_nt_zip, ZIP, NT])
@@ -598,14 +721,38 @@
                             input_format = get_input_format(file_path, compression_mode)
                             if input_format in (TURTLE, NT, RDF_XML):
                                 input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
                                 # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
                                 pass
 
+                elif extension == EXTENSION_TAR_XZ:
+                    # Check disk usage percentage
+                    if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                        error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                        return None, None, error_msg
+
+                    extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
+                    # For .tar.xz, expand and process the contents
+                    with tarfile.open(input_file, 'r:xz') as tar:
+                        tar.extractall(extract_path)
+
+                    # Loop by recursively retrieving files in a directory
+                    for root, _, files in os.walk(top=extract_path):
+                        for file in files:
+                            file_path = Path(root) / file
+                            # Determine file type and add to array
+                            compression_mode = get_compression_mode(file_path)
+                            input_format = get_input_format(file_path, compression_mode)
+                            if input_format in (TURTLE, NT, RDF_XML):
+                                input_file_2d_list.append([[file_path], compression_mode, input_format])
+                            else:
+                                # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
+                                pass
+
                 elif extension == EXTENSION_ZIP:
                     # Check disk usage percentage
                     if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
                         error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
                         return None, None, error_msg
 
                     extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
@@ -621,15 +768,15 @@
                             input_format = get_input_format(file_path, compression_mode)
                             if input_format in (TURTLE, NT, RDF_XML):
                                 input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
                                 # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
                                 pass
                 else:
-                    error_msg = '"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                    error_msg = '5:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                     return None, None, error_msg
 
     for input_file_list in input_file_2d_list:
         if input_file_list[1] is None:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL)
             elif input_file_list[2] == NT and FILE_TYPE_NT not in exists_file_types:
@@ -639,29 +786,38 @@
         elif input_file_list[1] == GZ:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL_GZ)
             elif input_file_list[2] == NT and FILE_TYPE_NT_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT_GZ)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML_GZ)
+        elif input_file_list[1] == XZ:
+            if input_file_list[2] == TURTLE and FILE_TYPE_TTL_XZ not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_TTL_XZ)
+            elif input_file_list[2] == NT and FILE_TYPE_NT_XZ not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_NT_XZ)
+            elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_XZ not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_RDF_XML_XZ)
         elif input_file_list[1] == ZIP:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL_ZIP)
             elif input_file_list[2] == NT and FILE_TYPE_NT_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT_ZIP)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML_ZIP)
 
     return input_file_2d_list, exists_file_types, None
 
-# Determine if the input file is compressed and get the compression mode ("gz" or None)
+# Determine if the input file is compressed and get the compression mode ("gz", "xz", "zip" or None)
 def get_compression_mode(input_file):
     extension = get_extension(input_file)
     if extension == EXTENSION_GZ:
         return GZ
+    elif extension == EXTENSION_XZ:
+        return XZ
     elif extension == EXTENSION_ZIP:
         return ZIP
     else:
         return None
 
 
 # Return input file format ("nt" or "turtle" or "xml")
@@ -701,24 +857,24 @@
         # Check if the file has read permission
         if os.access(input_file, os.R_OK) == False:
             error_msg = "Input file error: you don't have permission to read the input file."
             return error_msg
 
         # Allow only ".nt", ".ttl", ".rdf", ".xml", ".owl" (and their compressed versions) extensions
         extension = get_extension(input_file)
-        if extension in [EXTENSION_GZ, EXTENSION_ZIP]:
+        if extension in [EXTENSION_GZ, EXTENSION_XZ, EXTENSION_ZIP]:
             org_extension = get_extension_before_compression(input_file)
             # gz
             # if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL and org_extension != EXTENSION_RDF and org_extension != EXTENSION_XML and org_extension != EXTENSION_OWL:
             if org_extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
-                error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                error_msg = '6:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                 return error_msg
         #elif extension != EXTENSION_NT and extension != EXTENSION_TTL and extension != EXTENSION_RDF and extension != EXTENSION_XML and extension != EXTENSION_OWL:
         elif extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
-            error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+            error_msg = '7:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
             return error_msg
 
         if compression_mode == "":
             compression_mode = get_compression_mode(input_file)
         else:
             # This case usually does not occur because input files are classified by compression mode and input format at the start of processing.
             if compression_mode != get_compression_mode(input_file):
@@ -800,15 +956,15 @@
         if FILE_TYPE_ALL in types:
             if len(types) != 1:
                 error_msg = 'Type error: If "all" is specified, other types cannot be specified.'
                 return error_msg
         else:
             for type in types:
                 if type not in FILE_TYPE_DICT:
-                    error_msg = 'Type error: "' + type + '" is an unsupported input file format. "' + FILE_TYPE_TTL + '", "' + FILE_TYPE_NT + '", "' + FILE_TYPE_RDF_XML + '", "' + FILE_TYPE_TTL_GZ + '", "' + FILE_TYPE_NT_GZ + '", "' + FILE_TYPE_RDF_XML_GZ + '", "' + FILE_TYPE_TTL_ZIP + '", "' + FILE_TYPE_NT_ZIP + '" and "' + FILE_TYPE_RDF_XML_ZIP + '" are supported.'
+                    error_msg = 'Type error: "' + type + '" is an unsupported input file format. "' + FILE_TYPE_TTL + '", "' + FILE_TYPE_NT + '", "' + FILE_TYPE_RDF_XML + '", "' + FILE_TYPE_TTL_GZ + '", "' + FILE_TYPE_NT_GZ + '", "' + FILE_TYPE_RDF_XML_GZ + '", "' + FILE_TYPE_TTL_XZ + '", "' + FILE_TYPE_NT_XZ + '", "' + FILE_TYPE_RDF_XML_XZ + '", "' + FILE_TYPE_TTL_ZIP + '", "' + FILE_TYPE_NT_ZIP + '" and "' + FILE_TYPE_RDF_XML_ZIP + '" are supported.'
                     return error_msg
 
     # Check temporary directory
     if args.tmp_dir is not None:
         # Existence check of file temporary directory destination directory
         if Path(args.tmp_dir).is_file():
             error_msg = "Temporary directory error: A directory must be specified as the temporary directory destination. Files cannot be specified."
@@ -1055,15 +1211,16 @@
     shaper = Shaper(graph_list_of_files_input=input_file_list,
                     target_classes=target_classes,
                     all_classes_mode=all_classes_mode,
                     input_format=input_format,
                     namespaces_dict=namespaces_dict,
                     compression_mode=compression_mode,
                     instances_report_mode=MIXED_INSTANCES,
-                    detect_minimal_iri=True)
+                    detect_minimal_iri=True,
+                    examples_mode=ALL_EXAMPLES)
 
     return shaper.shex_graph(string_output=True,
                             verbose=args.verbose,
                             acceptance_threshold=0.05)
 
 
 # Calculates the percentage of prefixes in the input file that exist in the prefix list file prepared in advance,
@@ -1093,14 +1250,18 @@
     for input_file in input_files:
         g = rdflib.Graph()
 
         if compression_mode == GZ:
             with gzip.open(input_file, "rb") as f:
                 data = f.read()
             g.parse(data=data, format=input_format)
+        elif compression_mode == XZ:
+            with xz.open(input_file, "rb") as f:
+                data = f.read()
+            g.parse(data=data, format=input_format)
         elif compression_mode == ZIP:
             with ZipFile(input_file, "r") as f:
                 data = f.read(Path(input_file).name.replace(".zip", "")).decode()
             g.parse(data=data, format=input_format)
         else:
             g.parse(input_file, format=input_format)
 
@@ -1195,14 +1356,17 @@
     input_prefixes = []
     duplicated_namespaces = []
     duplicated_prefixes_dict = defaultdict(list) # Used for processing Namespace collision prevention when generating namespaces_dict to be passed to sheXer. ex. {'foaf:': ['http://xmlns.com/foaf/0.1/', 'http://xmlns.com/foaf/spec/#']}
     for input_file in input_files:
         if compression_mode == GZ:
             with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
                 data = f.read().splitlines()
+        elif compression_mode == XZ:
+            with xz.open(input_file, mode="rt", encoding="utf-8") as f:
+                data = f.read().splitlines()
         elif compression_mode == ZIP:
             with ZipFile(input_file, "r") as f:
                 data = f.read(Path(input_file).name.replace(".zip", "")).decode().splitlines()
         else:
             with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
                 data = f.read().splitlines()
 
@@ -1236,14 +1400,17 @@
     duplicated_namespaces = []
     duplicated_prefixes_dict = defaultdict(list) # Used for processing Namespace collision prevention when generating namespaces_dict to be passed to sheXer. ex. {'foaf:': ['http://xmlns.com/foaf/0.1/', 'http://xmlns.com/foaf/spec/#']}
     entity_namespaces_dict = {}
     for input_file in input_files:
         if compression_mode == GZ:
             with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
                 data = f.read().splitlines()
+        elif compression_mode == XZ:
+            with xz.open(input_file, mode="rt", encoding="utf-8") as f:
+                data = f.read().splitlines()
         elif compression_mode == ZIP:
             with ZipFile(input_file, "r") as f:
                 data = f.read(Path(input_file).name.replace(".zip", "")).decode().splitlines()
         else:
             with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
                 data = f.read().splitlines()
 
@@ -1452,14 +1619,24 @@
                 return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT_GZ in target_file_types:
                 return True
         elif input_file_list[2] == RDF_XML:
             if FILE_TYPE_RDF_XML_GZ in target_file_types:
                 return True
+    elif input_file_list[1] == XZ:
+        if input_file_list[2] == TURTLE:
+            if FILE_TYPE_TTL_XZ in target_file_types:
+                return True
+        elif input_file_list[2] == NT:
+            if FILE_TYPE_NT_XZ in target_file_types:
+                return True
+        elif input_file_list[2] == RDF_XML:
+            if FILE_TYPE_RDF_XML_XZ in target_file_types:
+                return True
     elif input_file_list[1] == ZIP:
         if input_file_list[2] == TURTLE:
             if FILE_TYPE_TTL_ZIP in target_file_types:
                 return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT_ZIP in target_file_types:
                 return True
```

## Comparing `rdf_doctor-1.1.4.dist-info/LICENSE` & `rdf_doctor-1.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.4.dist-info/METADATA` & `rdf_doctor-1.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.4
+Version: 1.1.5
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask >=2.2.5
 Requires-Dist: Flask-Cors >=3.0.9
 Requires-Dist: rdflib >=6.3.1
 Requires-Dist: SPARQLWrapper >=2.0.0
 Requires-Dist: wlighter >=1.0.1
 Requires-Dist: shexer >=2.4.1
 Requires-Dist: unidecode >=1.3.6
+Requires-Dist: python-xz
 
 # rdf-doctor
 [![Pyversions](https://img.shields.io/pypi/pyversions/rdf-doctor.svg)](https://pypi.python.org/pypi/rdf-doctor)
 
 ## Motivation
 DBCLS has conducted to convert various life science databases to RDF and support it. This development will enable us to provide a high-quality dataset that better links existing RDF datasets stored in the RDF portal site and newly developed RDF.
```

