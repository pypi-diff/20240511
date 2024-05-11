# Comparing `tmp/protein_design_tools-0.1.8.tar.gz` & `tmp/protein_design_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_design_tools-0.1.8.tar", last modified: Thu May  9 21:07:46 2024, max compression
+gzip compressed data, was "protein_design_tools-0.1.9.tar", last modified: Thu May  9 22:03:36 2024, max compression
```

## Comparing `protein_design_tools-0.1.8.tar` & `protein_design_tools-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.514261 protein_design_tools-0.1.8/
--rw-rw-r--   0 schaubaj (755442540) 1360859114     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.8/LICENSE
--rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 21:07:46.513208 protein_design_tools-0.1.8/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) 1360859114      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.8/README.md
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.496703 protein_design_tools-0.1.8/protein_design_tools/
--rw-rw-r--   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:51:26.000000 protein_design_tools-0.1.8/protein_design_tools/__init__.py
--rw-r--r--   0 schaubaj (755442540) 1360859114     7083 2024-05-09 21:07:08.000000 protein_design_tools-0.1.8/protein_design_tools/protein_structure.py
--rw-r--r--   0 schaubaj (755442540) 1360859114    18866 2024-05-09 21:06:44.000000 protein_design_tools-0.1.8/protein_design_tools/protein_structure_utils.py
--rw-r--r--   0 schaubaj (755442540) 1360859114     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.8/protein_design_tools/test.py
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.512150 protein_design_tools-0.1.8/protein_design_tools.egg-info/
--rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) 1360859114      435 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114        1 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114        6 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/requires.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114       21 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/top_level.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114       38 2024-05-09 21:07:46.514327 protein_design_tools-0.1.8/setup.cfg
--rw-rw-r--   0 schaubaj (755442540) 1360859114      899 2024-05-09 21:07:28.000000 protein_design_tools-0.1.8/setup.py
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.506117 protein_design_tools-0.1.8/tests/
--rw-r--r--   0 schaubaj (755442540) 1360859114     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.8/tests/test_protein_structure_utils.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 22:03:36.024838 protein_design_tools-0.1.9/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.9/LICENSE
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1653 2024-05-09 22:03:36.024177 protein_design_tools-0.1.9/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114     1044 2024-05-09 21:16:39.000000 protein_design_tools-0.1.9/README.md
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 22:03:36.009729 protein_design_tools-0.1.9/protein_design_tools/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:51:26.000000 protein_design_tools-0.1.9/protein_design_tools/__init__.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     7083 2024-05-09 21:07:08.000000 protein_design_tools-0.1.9/protein_design_tools/protein_structure.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114    18951 2024-05-09 22:02:57.000000 protein_design_tools-0.1.9/protein_design_tools/protein_structure_utils.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.9/protein_design_tools/test.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 22:03:36.023491 protein_design_tools-0.1.9/protein_design_tools.egg-info/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1653 2024-05-09 22:03:35.000000 protein_design_tools-0.1.9/protein_design_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      435 2024-05-09 22:03:35.000000 protein_design_tools-0.1.9/protein_design_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        1 2024-05-09 22:03:35.000000 protein_design_tools-0.1.9/protein_design_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        6 2024-05-09 22:03:35.000000 protein_design_tools-0.1.9/protein_design_tools.egg-info/requires.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       21 2024-05-09 22:03:35.000000 protein_design_tools-0.1.9/protein_design_tools.egg-info/top_level.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       38 2024-05-09 22:03:36.025002 protein_design_tools-0.1.9/setup.cfg
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      899 2024-05-09 22:03:13.000000 protein_design_tools-0.1.9/setup.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 22:03:36.022423 protein_design_tools-0.1.9/tests/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.9/tests/test_protein_structure_utils.py
```

### Comparing `protein_design_tools-0.1.8/LICENSE` & `protein_design_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.8/PKG-INFO` & `protein_design_tools-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -33,18 +33,27 @@
 
 ## Usage
 Provide some examples of how to use your package. For example:
 
 ### Calculate the radius of gyration of a protein structure's backbone
 
 ```python
-protein_structure = ProteinStructure()
-protein_structure.read_pdb("your.pdb")
-radgyr = get_radgy(protein_structure, atom_type="backbone")
+from protein_design_tools import protein_structure, protein_structure_utils
 
+protein = protein_structure.ProteinStructure()
+protein.read_pdb("example.pdb")
+
+# Get the sequence of each chain in the protein
+sequence_dict = protein.get_sequence()
+for chain_id, sequence in sequence_dict.items():
+    print(f"Chain {chain_id}: {sequence}")
+
+# Calculate the radius of gyration
+rg = protein_structure_utils.get_radgy(protein)
+print(f"The radius of gyration of the protein structure is : {rg}")
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Include information about the license. For example:
```

### Comparing `protein_design_tools-0.1.8/protein_design_tools/protein_structure.py` & `protein_design_tools-0.1.9/protein_design_tools/protein_structure.py`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.8/protein_design_tools/protein_structure_utils.py` & `protein_design_tools-0.1.9/protein_design_tools/protein_structure_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                     masses.append(atom.mass)
                 elif atom_type == "sidechain" and atom.atom_name not in ["N", "CA", "C", "O"]:
                     masses.append(atom.mass)
 
     return masses
 
 
-def get_radgy(structure, atom_type="backbone", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
+def get_radgyr(structure, atom_type="backbone", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
     """
     Calculate the radius of gyration of a protein structure.
 
     Parameters:
     structure (ProteinStructure): The protein structure to calculate the radius of gyration for.
     atom_type (str, optional): The type of atoms to calculate the radius of gyration for. Can be "all", "backbone", or "sidechain". Defaults to "backbone".
     chains (list of str, optional): A list of chain names to calculate the radius of gyration for. If None, calculate the radius of gyration for all chains. Defaults to None.
@@ -127,15 +127,15 @@
     # Calculate the radius of gyration
     radius_of_gyration = np.sqrt(np.average(distances**2, weights=masses))
 
     return radius_of_gyration
 
 # get radius of gyration for all alanine helices of different lengths
 # structure, atom_type="all", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
-def get_radgy_alanine_helix(sequence_length, atom_type="backbone"):
+def get_radgyr_alanine_helix(sequence_length, atom_type="backbone"):
     """
     Retrieve the radius of gyration of an ideal alanine helix.
 
     Parameters:
     sequence_length (int): The length of the alanine helix. The length should be between 11 and 200.
     atom_type (str, optional): The type of atoms to calculate the radius of gyration for. Can be "all" or "backbone". Defaults to "backbone".
 
@@ -143,34 +143,35 @@
     float: The radius of gyration of the alanine helix.
     """
     if atom_type == "all":
         try:
             radius_of_gyration = ALANINE_HELIX_RADGYR_ALLHEAVY[sequence_length]
         except KeyError:
             # Program should break here with error message
+            print(f'KeyError: sequence length of {sequence_length} not found.')
             print('Unable to lookup radgyr for the alanine helix. The sequence length must be between 11 and 200.')
             raise
     elif atom_type == "backbone":
         try:
             radius_of_gyration = ALANINE_HELIX_RADGYR_BACKBONE[sequence_length]
         except KeyError:
             # Program should break here with error message
             print('Unable to lookup radgyr for the alanine helix. The sequence length must be between 11 and 200.')
             raise
     else:
         raise ValueError("Invalid atom type. Atom type must be 'all' or 'backbone'.")
     
     return radius_of_gyration
 
-def get_radgy_ratio(structure, atom_type="backbone", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
+def get_radgyr_ratio(structure, atom_type="backbone", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
 
     # Get the radius of gyration
-    structure_radius_of_gyration = get_radgy(structure, atom_type=atom_type, chains=chains, residue_numbers=residue_numbers, residue_indices=residue_indices, residue_ids=residue_ids)
+    structure_radius_of_gyration = get_radgyr(structure, atom_type=atom_type, chains=chains, residue_numbers=residue_numbers, residue_indices=residue_indices, residue_ids=residue_ids)
 
     # Get the radius of gyration of an ideal alanine helix of the same length. structure.get_sequences will return the sequendes of each chain of the protein, so these need to be summed
     structure_seq_len = sum([len(sequence) for sequence in structure.get_sequence_dict()])
-    alanine_radius_of_gyration = get_radgy_alanine_helix(structure_seq_len, atom_type=atom_type)
+    alanine_radius_of_gyration = get_radgyr_alanine_helix(structure_seq_len, atom_type=atom_type)
 
     # Calculate the radius of gyration ratio
     radius_of_gyration_ratio = structure_radius_of_gyration / alanine_radius_of_gyration
 
     return radius_of_gyration_ratio
```

### Comparing `protein_design_tools-0.1.8/protein_design_tools/test.py` & `protein_design_tools-0.1.9/protein_design_tools/test.py`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.8/protein_design_tools.egg-info/PKG-INFO` & `protein_design_tools-0.1.9/protein_design_tools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -33,18 +33,27 @@
 
 ## Usage
 Provide some examples of how to use your package. For example:
 
 ### Calculate the radius of gyration of a protein structure's backbone
 
 ```python
-protein_structure = ProteinStructure()
-protein_structure.read_pdb("your.pdb")
-radgyr = get_radgy(protein_structure, atom_type="backbone")
+from protein_design_tools import protein_structure, protein_structure_utils
 
+protein = protein_structure.ProteinStructure()
+protein.read_pdb("example.pdb")
+
+# Get the sequence of each chain in the protein
+sequence_dict = protein.get_sequence()
+for chain_id, sequence in sequence_dict.items():
+    print(f"Chain {chain_id}: {sequence}")
+
+# Calculate the radius of gyration
+rg = protein_structure_utils.get_radgy(protein)
+print(f"The radius of gyration of the protein structure is : {rg}")
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 Include information about the license. For example:
```

### Comparing `protein_design_tools-0.1.8/setup.py` & `protein_design_tools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='protein-design-tools',
-    version='0.1.8',
+    version='0.1.9',
     author='Andrew Schaub',
     author_email='andrew.schaub@protonmail.com',
     description='A library of tools for protein design.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/drewschaub/protein-design-tools',
     license=' MIT License',
```

### Comparing `protein_design_tools-0.1.8/tests/test_protein_structure_utils.py` & `protein_design_tools-0.1.9/tests/test_protein_structure_utils.py`

 * *Files identical despite different names*

