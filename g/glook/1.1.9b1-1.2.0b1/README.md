# Comparing `tmp/glook-1.1.9b1.tar.gz` & `tmp/glook-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glook-1.1.9b1.tar", last modified: Sun May  5 19:02:38 2024, max compression
+gzip compressed data, was "glook-1.2.0b1.tar", last modified: Thu May  9 19:02:01 2024, max compression
```

## Comparing `glook-1.1.9b1.tar` & `glook-1.2.0b1.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:02:38.286896 glook-1.1.9b1/
--rw-rw-rw-   0        0        0     7228 2024-05-05 19:02:38.281901 glook-1.1.9b1/PKG-INFO
--rw-rw-rw-   0        0        0     5322 2024-04-27 21:12:46.000000 glook-1.1.9b1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 19:02:38.120657 glook-1.1.9b1/glook/
--rw-rw-rw-   0        0        0     3471 2024-05-05 09:05:48.000000 glook-1.1.9b1/glook/GLook.py
--rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.1.9b1/glook/__init__.py
--rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.1.9b1/glook/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:02:38.276119 glook-1.1.9b1/glook/pages/
--rw-rw-rw-   0        0        0    26240 2024-05-05 06:31:15.000000 glook-1.1.9b1/glook/pages/10_Unsupervised_learning.py
--rw-rw-rw-   0        0        0   107673 2024-05-05 05:42:46.000000 glook-1.1.9b1/glook/pages/11_Custom_Model_Training.py
--rw-rw-rw-   0        0        0    31057 2024-05-05 18:13:44.000000 glook-1.1.9b1/glook/pages/12_Supervised_Deployment_Demo.py
--rw-rw-rw-   0        0        0    33248 2024-05-05 17:56:46.000000 glook-1.1.9b1/glook/pages/13_Unsupervised_Deployment_Demo.py
--rw-rw-rw-   0        0        0     6149 2024-05-05 19:01:39.000000 glook-1.1.9b1/glook/pages/1_General_Data_Insights.py
--rw-rw-rw-   0        0        0    19790 2024-05-05 17:41:55.000000 glook-1.1.9b1/glook/pages/2_Univariate_Analysis.py
--rw-rw-rw-   0        0        0     7813 2024-04-24 16:05:25.000000 glook-1.1.9b1/glook/pages/3_Bivariate_Analysis.py
--rw-rw-rw-   0        0        0     7707 2024-04-28 06:03:29.000000 glook-1.1.9b1/glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-   0        0        0   113975 2024-05-05 18:57:37.000000 glook-1.1.9b1/glook/pages/5_Pre_Processing.py
--rw-rw-rw-   0        0        0     3641 2024-05-05 13:05:24.000000 glook-1.1.9b1/glook/pages/6_Split_Data.py
--rw-rw-rw-   0        0        0     4588 2024-04-11 19:05:58.000000 glook-1.1.9b1/glook/pages/7_Dimensionality_Reduction.py
--rw-rw-rw-   0        0        0    60527 2024-05-05 17:49:18.000000 glook-1.1.9b1/glook/pages/8_Supervised_Learning.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:02:38.207030 glook-1.1.9b1/glook.egg-info/
--rw-rw-rw-   0        0        0     7228 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      211 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-05 19:02:37.000000 glook-1.1.9b1/glook.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 19:02:38.286896 glook-1.1.9b1/setup.cfg
--rw-rw-rw-   0        0        0     2437 2024-05-05 19:02:23.000000 glook-1.1.9b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.258134 glook-1.2.0b1/
+-rw-rw-rw-   0        0        0     7228 2024-05-09 19:02:01.255138 glook-1.2.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     5322 2024-04-27 21:12:46.000000 glook-1.2.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.012161 glook-1.2.0b1/glook/
+-rw-rw-rw-   0        0        0     3502 2024-05-09 16:44:31.000000 glook-1.2.0b1/glook/GLook.py
+-rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.0b1/glook/__init__.py
+-rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.0b1/glook/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.224290 glook-1.2.0b1/glook/pages/
+-rw-rw-rw-   0        0        0    26240 2024-05-05 06:31:15.000000 glook-1.2.0b1/glook/pages/10_Unsupervised_learning.py
+-rw-rw-rw-   0        0        0   107673 2024-05-05 05:42:46.000000 glook-1.2.0b1/glook/pages/11_Custom_Model_Training.py
+-rw-rw-rw-   0        0        0    31057 2024-05-05 18:13:44.000000 glook-1.2.0b1/glook/pages/12_Supervised_Deployment_Demo.py
+-rw-rw-rw-   0        0        0    33654 2024-05-08 18:38:27.000000 glook-1.2.0b1/glook/pages/13_Unsupervised_Deployment_Demo.py
+-rw-rw-rw-   0        0        0     6483 2024-05-09 16:55:20.000000 glook-1.2.0b1/glook/pages/1_General_Data_Insights.py
+-rw-rw-rw-   0        0        0    20207 2024-05-09 18:30:57.000000 glook-1.2.0b1/glook/pages/2_Univariate_Analysis.py
+-rw-rw-rw-   0        0        0     8173 2024-05-09 16:56:35.000000 glook-1.2.0b1/glook/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-   0        0        0     8067 2024-05-09 16:58:02.000000 glook-1.2.0b1/glook/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-   0        0        0   114361 2024-05-09 17:39:14.000000 glook-1.2.0b1/glook/pages/5_Pre_Processing.py
+-rw-rw-rw-   0        0        0     4099 2024-05-09 17:41:15.000000 glook-1.2.0b1/glook/pages/6_Split_Data.py
+-rw-rw-rw-   0        0        0     4588 2024-04-11 19:05:58.000000 glook-1.2.0b1/glook/pages/7_Dimensionality_Reduction.py
+-rw-rw-rw-   0        0        0    60527 2024-05-05 17:49:18.000000 glook-1.2.0b1/glook/pages/8_Supervised_Learning.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.164924 glook-1.2.0b1/glook.egg-info/
+-rw-rw-rw-   0        0        0     7228 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      211 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 19:02:00.000000 glook-1.2.0b1/glook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.234409 glook-1.2.0b1/look/
+-rw-rw-rw-   0        0        0     3228 2024-05-02 17:40:02.000000 glook-1.2.0b1/look/GLook.py
+-rw-rw-rw-   0        0        0       51 2024-03-25 17:39:42.000000 glook-1.2.0b1/look/__init__.py
+-rw-rw-rw-   0        0        0      339 2024-03-25 18:24:01.000000 glook-1.2.0b1/look/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:02:01.248962 glook-1.2.0b1/look/pages/
+-rw-rw-rw-   0        0        0     6157 2024-05-02 17:40:35.000000 glook-1.2.0b1/look/pages/1_General_Data_Insights.py
+-rw-rw-rw-   0        0        0    19802 2024-05-02 17:43:01.000000 glook-1.2.0b1/look/pages/2_Univariate_Analysis.py
+-rw-rw-rw-   0        0        0     7813 2024-05-02 17:43:17.000000 glook-1.2.0b1/look/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-   0        0        0     7707 2024-05-02 17:43:33.000000 glook-1.2.0b1/look/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 19:02:01.258134 glook-1.2.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     2507 2024-05-09 19:01:54.000000 glook-1.2.0b1/setup.py
```

### Comparing `glook-1.1.9b1/PKG-INFO` & `glook-1.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 1.1.9b1
+Version: 1.2.0b1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glook Version: 1.1.9b1 Summary: Auto EDA. Home-
+Metadata-Version: 2.1 Name: glook Version: 1.2.0b1 Summary: Auto EDA. Home-
 page: https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
 gaurang.ingle@gmail.com Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com License: MIT Project-URL: Bug
 Reports, https://github.com/gaurang157/glook/issues Project-URL: Source, https:
 //github.com/gaurang157/glook Project-URL: Documentation, https://github.com/
 gaurang157/glook/blob/main/README.md Project-URL: Say Thanks!, https://
 github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
```

### Comparing `glook-1.1.9b1/README.md` & `glook-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/GLook.py` & `glook-1.2.0b1/glook/GLook.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 		try:
 			# Try reading as Excel
 			df = pd.read_excel(gg, engine='openpyxl')
 		except Exception as e:
 			st.error(f"Error reading file: {e}")
 	# Store the DataFrame in session_state
 	st.session_state.df = df
+	st.session_state.df_pre = df
 	st.session_state.df0 = df
 	st.session_state.drop = 0
 	st.session_state.miss = 0
 	st.session_state.type_ch = 0
 	st.session_state.treat_out = 0
 	st.session_state.tran = 0
 	st.session_state.out_rplac = 0
```

### Comparing `glook-1.1.9b1/glook/pages/10_Unsupervised_learning.py` & `glook-1.2.0b1/glook/pages/10_Unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/11_Custom_Model_Training.py` & `glook-1.2.0b1/glook/pages/11_Custom_Model_Training.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/12_Supervised_Deployment_Demo.py` & `glook-1.2.0b1/glook/pages/12_Supervised_Deployment_Demo.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/13_Unsupervised_Deployment_Demo.py` & `glook-1.2.0b1/glook/pages/13_Unsupervised_Deployment_Demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,35 @@
 import numpy as np
 from scipy.stats.mstats import winsorize
 from scipy.stats import boxcox, yeojohnson
 from sklearn.preprocessing import LabelEncoder, KBinsDiscretizer
 import matplotlib.colors as mcolors
 from sklearn.decomposition import PCA, NMF, FastICA, FactorAnalysis, DictionaryLearning, TruncatedSVD
 
-if "X_test" in st.session_state:
-	X_test0 = st.session_state.X_test0
-	X_test = st.session_state.X_test
-	 
-dfo = X_test0
+if "X_test" in st.session_state or "df" in st.session_state:
+	try:
+		X_test0 = st.session_state.X_test0
+	except:
+		pass
+	try:
+		X_test = st.session_state.X_test
+	except:
+		pass
+	try:
+		df = st.session_state.df
+	except:
+		pass
+	try:
+		df0 = st.session_state.df0
+	except:
+		pass
+try:
+	dfo = X_test0
+except:
+	pass
 # print(X_test0)
 
 
 def apply_pipeline_d_tpye(df, pipeline):
 	try:
 		# Make a copy of the DataFrame to avoid warnings or unintentional changes
 		modified_df = df.copy()
@@ -403,15 +419,15 @@
 					data = pd.read_csv(uploadedFile)
 				except:
 						try:
 							data = pd.read_excel(uploadedFile)
 						except:      
 							data = pd.DataFrame(uploadedFile)
 		elif choice == "Use Validation Data":
-			data = X_test
+			data = df0
 					
 		else:
 			st.sidebar.warning("You need to upload a csv or excel file.")
 	elif type_ == 'Manual Input':
 		print(1)
 		# Analyze each column to determine type and range
 		# Select a random row to use as default values
@@ -844,14 +860,16 @@
 
 				# # Apply the custom color map to the 'Clusters' column
 				# styled_result = styled_result.applymap(lambda val: generate_color(val, max_cluster), subset=["Clusters"])
 
 				# # Display the styled table in Streamlit
 				# st.table(styled_result.format(precision=2))
 	
+				# Change the Pandas option to allow more elements to be styled
+				pd.set_option("styler.render.max_elements", 5000000000000000000000000000)  # Adjust this to a value greater than your cell count
 
 				# Define color maps for the gradients
 				tomato_cm = sns.light_palette("tomato", as_cmap=True)
 				gold_cm = sns.light_palette("gold", as_cmap=True)
 
 				# Function to create a color map for the 'Clusters' column based on its value
 				def generate_color(val, max_cluster):
```

### Comparing `glook-1.1.9b1/glook/pages/1_General_Data_Insights.py` & `glook-1.2.0b1/look/pages/1_General_Data_Insights.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 	
 	# st.dataframe(df)
 	# Exclude non-numeric columns
 	numeric_df = df.select_dtypes(include='number')
 
 	# Convert non-numeric values to NaN
 	numeric_df = numeric_df.apply(pd.to_numeric, errors='coerce')
-	st.header(":green[Correlation Coefficient]")
+	st.header("Correlation Coefficient :green[Heatmap]")
 	# Calculate the correlation matrix
 	correlation_matrix = numeric_df.corr()
 	# Define the list of colorscales
 	# colorscales = ['aggrnyl', 'agsunset', 'algae', 'amp', 'armyrose', 'balance', 'blackbody', 'bluered', 'blues', 'blugrn', 'bluyl', 'brbg', 'brwnyl', 'bugn', 'bupu', 'burg', 'burgyl', 'cividis', 'curl', 'darkmint', 'deep', 'delta', 'dense', 'earth', 'edge', 'electric', 'emrld', 'fall', 'geyser', 'gnbu', 'gray', 'greens', 'greys', 'haline', 'hot', 'hsv', 'ice', 'icefire', 'inferno', 'jet', 'magenta', 'magma', 'matter', 'mint', 'mrybm', 'mygbm', 'oranges', 'orrd', 'oryel', 'oxy', 'peach', 'phase', 'picnic', 'pinkyl', 'piyg', 'plasma', 'plotly3', 'portland', 'prgn', 'pubu', 'pubugn', 'puor', 'purd', 'purp', 'purples', 'purpor', 'rainbow', 'rdbu', 'rdgy', 'rdpu', 'rdylbu', 'rdylgn', 'redor', 'reds', 'solar', 'spectral', 'speed', 'sunset', 'sunsetdark', 'teal', 'tealgrn', 'tealrose', 'tempo', 'temps', 'thermal', 'tropic', 'turbid', 'turbo', 'twilight', 'viridis', 'ylgn', 'ylgnbu', 'ylorbr', 'ylorrd']
 	# Number input for selecting the colorscale index
 	# colorscale_index = st.number_input('Select a colorscale index:', min_value=0, max_value=len(colorscales)-1, value=0)
 	# st.write(colorscales[colorscale_index])
```

### Comparing `glook-1.1.9b1/glook/pages/2_Univariate_Analysis.py` & `glook-1.2.0b1/look/pages/2_Univariate_Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
 					# """ KDE plot """
 					plt.figure(figsize=(10, 6))  # Adjust figure size
 					sns.histplot(df[column], kde=True, color="green")
 					st.pyplot()
 					plt.close()
 	 				# KDE plot using Plotly
 					# fig = px.histogram(df, x=df[column], marginal="rug", nbins=30, histnorm='probability density', 
-				  	#  title="KDE Plot", color_discrete_sequence=['green'])
+                  	#  title="KDE Plot", color_discrete_sequence=['green'])
 					# # Create KDE plot using Plotly
 					# # Show the plot using Streamlit
 					# st.plotly_chart(fig, use_container_width=True)
 						# Create KDE plot using Plotly Express
 					# fig = px.histogram(df, x=df[column], marginal="rug", nbins=30, histnorm='probability density', 
 					# 				title="KDE Plot", color_discrete_sequence=['green'],opacity=0.5)
```

### Comparing `glook-1.1.9b1/glook/pages/3_Bivariate_Analysis.py` & `glook-1.2.0b1/look/pages/3_Bivariate_Analysis.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/4_Trivariate_Analysis.py` & `glook-1.2.0b1/look/pages/4_Trivariate_Analysis.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/5_Pre_Processing.py` & `glook-1.2.0b1/glook/pages/5_Pre_Processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,18 +435,26 @@
 def callback():
 	st.session_state.button_clicked = True
 
 
 st.header(':green[Try Best Pre-Processing Step]')
 print(53)
 try:
-	st.write('Session State:->', st.session_state['shared'])
+	# st.write('Session State:->', st.session_state['shared'])
 	print(54)
-	if 'df' in st.session_state:
-		df = st.session_state.df
+	if 'df_pre' in st.session_state:
+		# oragnial_df = st.session_state.df
+		df_to_pre = st.session_state.df_pre
+		# st.warning("kl")
+		# to_select = st.selectbox("Select Data Frame (Recommended: DF to Pre-Process)", ["oragnial_df", "df_to_pre_process"], index=1)
+		# if to_select == "oragnial_df":
+		# 	df = oragnial_df
+		# elif to_select == "df_to_pre_process":
+		df = df_to_pre
+		
 		print(1)
 		print(55)
 		selected_column = st.selectbox('Select a column', df.columns)
 		print(2)
 		print(56)
 		html_content = (
 			f"<div class='column-header'>Insights for column:<code>{selected_column}</code></div>"
@@ -1052,15 +1060,15 @@
 				st.subheader('⚠️Please upload a file⚠️')
 				print(215)
 				pass
 			confirm_change = st.button('Confirm Change')
 			if confirm_change:
 				if 'type_ch' in st.session_state:
 					type_ch_no = st.session_state.type_ch
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				pipeline = {'column': f'{selected_column}', 'new_dtype':
 					f'{new_dtype}'}
 				with open(f'{type_ch_no}_datatype_pipeline.pkl', 'wb') as f:
 					joblib.dump(pipeline, f)
 					print(216)
 				type_ch_no += 1
 				st.session_state.type_ch = type_ch_no
@@ -1334,15 +1342,15 @@
 			if confirm_change:
 				if 'drop' in st.session_state:
 					drop_no = st.session_state.drop
 				pipeline1 = {'column': f'{selected_column}'}
 				with open(f'{drop_no}_drop_pipeline.pkl', 'wb') as f:
 					joblib.dump(pipeline1, f)
 					print(276)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				drop_no += 1
 				st.session_state.drop = drop_no
 				# modified_df.to_csv("clean.csv", index=False)
 				st.rerun()
 				print(277)
 	elif preprocessing_action == 'Drop Duplicates':
 		if st.button('Apply', on_click=callback
@@ -1356,15 +1364,15 @@
 			print(280)
 			confirm_change = st.button('Confirm Change')
 			if confirm_change:
 				pipeline2 = {'action': 'drop_duplicates'}
 				with open('drop_dup_pipeline.pkl', 'wb') as f:
 					joblib.dump(pipeline2, f)
 					print(281)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				st.rerun()
 				print(282)
 	elif preprocessing_action == 'Treat Outliers':
 		outlier_method = st.radio('Select Outlier Treatment Method', [
 			'Delete Outliers', 'Winsorization'])
 		if st.button('Apply', on_click=callback
 			) or st.session_state.button_clicked:
@@ -1651,15 +1659,15 @@
 					treat_out_no = st.session_state.treat_out
 				pipeline3 = {'method': f'{outlier_method}', 'column':
 					f'{selected_column}', 'lower_limit': f'{lower_limit}',
 					'upper_limit': f'{upper_limit}', 'z_score_threshold': z_score_threshold}
 				with open(f'{treat_out_no}_outliers_for_col_pipeline.pkl', 'wb') as f:
 					joblib.dump(pipeline3, f)
 					print(342)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				treat_out_no += 1
 				st.session_state.treat_out = treat_out_no
 				st.rerun()
 				print(343)
 				
 				
 	elif preprocessing_action == 'Treat Outliers on full DF':
@@ -1685,15 +1693,15 @@
 				upper_limit)
 			st.write('Modified DataFrame:')
 			print(344)
 			st.write(modified_df)
 			print(345)
 			confirm_change = st.button('Confirm Change')
 			if confirm_change:
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				pipeline4 = {'method': f'{method}', 'lower_limit':
 					f'{lower_limit}', 'upper_limit': f'{upper_limit}',
 					'z_score_threshold': f'{z_score_threshold}'}
 				with open('outliers_for_full_df_pipeline.pkl', 'wb') as f:
 					joblib.dump(pipeline4, f)
 					print(346)
 				st.rerun()
@@ -1973,15 +1981,15 @@
 				if 'miss' in st.session_state:
 					miss_no = st.session_state.miss
 				pipeline5 = {'method': f'{missing_method}', 'column':
 					f'{selected_column}'}
 				with open(f'{miss_no}_treat_missing_vaues_for_col.pkl', 'wb') as f:
 					joblib.dump(pipeline5, f)
 					print(407)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				miss_no += 1
 				st.session_state.miss = miss_no
 				st.rerun()
 				print(408)
 
 
 	elif preprocessing_action == 'Traat Missing from full DF':
@@ -2043,15 +2051,15 @@
 				pipeline6 = {'numeric_treatment': f'{numeric_treatment}',
 					'numeric_strategy': f'{numeric_strategy}',
 					'categorical_treatment': f'{categorical_treatment}',
 					'categorical_strategy': f'{categorical_strategy}'}
 				with open('treat_missing_vaues_in_full_df.pkl', 'wb') as f:
 					joblib.dump(pipeline6, f)
 					print(418)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				st.rerun()
 				print(419)
 			
 
 	elif preprocessing_action == 'Apply Transformation':
 		transformation_method = st.selectbox('Select Transformation Technique',
 			['Log Transformation', 'Exponential Transformation',
@@ -2331,15 +2339,15 @@
 					"method": f'{transformation_method}',
 					"column_name": f'{selected_column}',
 				}
 
 				# Save the pipeline to a serialized object
 				with open(f"{tran_no}_apply_transformation_on_col.pkl", "wb") as f:
 					joblib.dump(pipeline7, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 
 				tran_no += 1
 				st.session_state.tran = tran_no
 
 				st.rerun()
 
 
@@ -2615,15 +2623,15 @@
 					"method": f'{encoding_method}',
 					"param": opt
 				}
 
 				# Save the pipeline to a serialized object
 				with open("apply_encoding_on_df.pkl", "wb") as f:
 					joblib.dump(pipeline8, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				st.rerun()
 				print(537)
 
 	elif preprocessing_action == 'Column to Dummy Variable':
 		encoding_method = st.selectbox('Select encoding method', [
 			'One-Hot Encoding', 'Label Encoding'])
 		opt = st.toggle('drop_first')
@@ -2898,15 +2906,15 @@
 					"column_name": f'{selected_column}',
 					"param": opt
 				}
 
 				# Save the pipeline to a serialized object
 				with open(f"{col_dum_no}_apply_encoding_on_col.pkl", "wb") as f:
 					joblib.dump(pipeline9, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				col_dum_no += 1
 				st.session_state.col_dum = col_dum_no
 				st.rerun()
 				print(595)
 
 
 	elif preprocessing_action == 'Apply Scaling':
@@ -2925,15 +2933,15 @@
 				pipeline10 = {
 					"method": f'{scaling_method}',
 				}
 
 				# Save the pipeline to a serialized object
 				with open("apply_scaling_on_df.pkl", "wb") as f:
 					joblib.dump(pipeline10, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				# modified_df.to_csv("clean.csv", index=False)
 				st.rerun()
 				print(598)
 	elif preprocessing_action == 'Discretize Output Variable':
 		bins = st.slider('Select the number of bins', min_value=2,
 			max_value=20, value=5)
 		strategy = st.selectbox('Select the strategy for binning', [
@@ -3211,15 +3219,15 @@
 				pipeline11 = {
 					"column_name": f'{selected_column}',
 					"bins": bins,
 					"strategy": strategy
 				}
 				with open(f"{des_var_no}_discretize_output_col.pkl", "wb") as f:
 					joblib.dump(pipeline11, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				des_var_no += 1
 				st.session_state.des_var = des_var_no
 				st.rerun()
 				print(658)
 
 	elif preprocessing_action == 'Column Unique Value Replacement(for output variable)':
 		print(43)
@@ -3443,15 +3451,15 @@
 					"replacements": replacements,
 					"select": select
 				}
 
 				# Save the pipeline to a serialized object
 				with open(f"{out_rplac_no}_column_unique_value_replacement.pkl", "wb") as f:
 					joblib.dump(pipeline12, f)
-				st.session_state.df = modified_df
+				st.session_state.df_pre = modified_df
 				out_rplac_no += 1
 				st.session_state.out_rplac = out_rplac_no
 				st.rerun()
 				print(729)
 
 
 except Exception as e:
```

### Comparing `glook-1.1.9b1/glook/pages/6_Split_Data.py` & `glook-1.2.0b1/glook/pages/6_Split_Data.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,30 +25,39 @@
 	except Exception as e:
 		st.error(f"Error occurred during data splitting: {e}")
 
 # st.write(modified_df)
 
 
 try:
-	st.write("Session State:->", st.session_state["shared"])
+	# st.write("Session State:->", st.session_state["shared"])
 	# Streamlit UI for data splitting
 	st.title("Data Splitting Page")
 
 	# Display the modified DataFrame
 	st.subheader("Modified DataFrame")
-	if "df" in st.session_state:
-		df = st.session_state.df
+	if "df_pre" in st.session_state:
+		# df = st.session_state.df
 		df0 = st.session_state.df0
+		oragnial_df = st.session_state.df
+		df_to_pre = st.session_state.df_pre
+		# st.warning("kl")
+		# to_select = st.selectbox("Select Data Frame (Recommended: Pre-Processed DF)", ["oragnial_df", "pre_processed_df"], index=1)
+		# if to_select == "oragnial_df":
+		# 	df = oragnial_df
+		# elif to_select == "pre_processed_df":
+		df = df_to_pre
 		# Assuming df is your DataFrame
 		# df.to_csv('your_file.csv', index=False)
 		# Data split options
 		st.write(df)
 		target_column = st.sidebar.selectbox("Select the target column:", df.columns)
 		test_size = st.sidebar.slider("Select the test size:", 0.1, 0.5, step=0.05)
 		random_state = st.sidebar.number_input("Enter the random state:", min_value=0, max_value=10000, value=42)
+		st.sidebar.warning("Note: Split Data Before Moving to Model Building Page ===>")
 	else:
 		pass
 	if (
 		st.button("Apply", on_click=callback)
 			or st.session_state.button_clicked
 			):
 		try:
@@ -87,15 +96,15 @@
 except:
 	pass
 # Undo functionality
 confirm_change = st.button(
 	'Confirm Change and move to Model Building Page', 
 	use_container_width=True
 	)
-gg = st.sidebar.button("Swith to Model Building")
+gg = st.sidebar.button("Confirm Change and Swith to Model Building")
 
 if gg:
 	st.session_state.X_train = X_train
 	st.session_state.X_test = X_test
 	st.session_state.y_train = y_train
 	st.session_state.y_test = y_test
 	st.session_state.X_test0 = X_test0
```

### Comparing `glook-1.1.9b1/glook/pages/7_Dimensionality_Reduction.py` & `glook-1.2.0b1/glook/pages/7_Dimensionality_Reduction.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook/pages/8_Supervised_Learning.py` & `glook-1.2.0b1/glook/pages/8_Supervised_Learning.py`

 * *Files identical despite different names*

### Comparing `glook-1.1.9b1/glook.egg-info/PKG-INFO` & `glook-1.2.0b1/glook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 1.1.9b1
+Version: 1.2.0b1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glook Version: 1.1.9b1 Summary: Auto EDA. Home-
+Metadata-Version: 2.1 Name: glook Version: 1.2.0b1 Summary: Auto EDA. Home-
 page: https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
 gaurang.ingle@gmail.com Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com License: MIT Project-URL: Bug
 Reports, https://github.com/gaurang157/glook/issues Project-URL: Source, https:
 //github.com/gaurang157/glook Project-URL: Documentation, https://github.com/
 gaurang157/glook/blob/main/README.md Project-URL: Say Thanks!, https://
 github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
```

### Comparing `glook-1.1.9b1/glook.egg-info/SOURCES.txt` & `glook-1.2.0b1/glook.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,15 @@
 glook/pages/1_General_Data_Insights.py
 glook/pages/2_Univariate_Analysis.py
 glook/pages/3_Bivariate_Analysis.py
 glook/pages/4_Trivariate_Analysis.py
 glook/pages/5_Pre_Processing.py
 glook/pages/6_Split_Data.py
 glook/pages/7_Dimensionality_Reduction.py
-glook/pages/8_Supervised_Learning.py
+glook/pages/8_Supervised_Learning.py
+look/GLook.py
+look/__init__.py
+look/cli.py
+look/pages/1_General_Data_Insights.py
+look/pages/2_Univariate_Analysis.py
+look/pages/3_Bivariate_Analysis.py
+look/pages/4_Trivariate_Analysis.py
```

### Comparing `glook-1.1.9b1/setup.py` & `glook-1.2.0b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="glook",
-    version="1.1.9b1",
+    version="1.2.0b1",
     author="Gaurang Ingle",
     author_email="gaurang.ingle@gmail.com",
     description="Auto EDA.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaurang157/glook",
     packages=find_packages(),
     include_package_data=True,
-    package_data={'glook': ['cli.py', 'pages/*']},
+    package_data={'glook': ['cli.py', 'pages/*'],
+    'look': ['cli.py', 'pages/*']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
@@ -44,15 +45,16 @@
         "openpyxl==3.1.2",
         "joblib==1.3.2",
         "scikit_learn==1.3.2",
         "xgboost==2.0.3"
     ],
     entry_points={
         "console_scripts": [
-            "glook=glook:main2",
+            "glookml=glook:main2",
+            "glook=look:main2"
         ],
     },
     license="MIT",
     keywords=[
         "AutoEDA", "Exploratory Data Analysis", "Data Visualization", 
         "GUI", "CLI", "Python", "Streamlit", "CLI interface", "UI interface"
     ],
```

