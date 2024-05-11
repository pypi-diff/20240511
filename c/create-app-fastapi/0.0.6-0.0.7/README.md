# Comparing `tmp/create-app-fastapi-0.0.6.tar.gz` & `tmp/create-app-fastapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-app-fastapi-0.0.6.tar", last modified: Fri May  3 09:48:47 2024, max compression
+gzip compressed data, was "create-app-fastapi-0.0.7.tar", last modified: Sat May 11 08:48:14 2024, max compression
```

## Comparing `create-app-fastapi-0.0.6.tar` & `create-app-fastapi-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:48:47.414887 create-app-fastapi-0.0.6/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      673 2024-05-03 09:48:47.414887 create-app-fastapi-0.0.6/PKG-INFO
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:48:47.414887 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      673 2024-05-03 09:48:47.000000 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/PKG-INFO
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-05-03 09:48:47.000000 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-05-03 09:48:47.000000 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-05-03 09:48:47.000000 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/entry_points.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-05-03 09:48:47.000000 create-app-fastapi-0.0.6/create_app_fastapi.egg-info/top_level.txt
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:48:47.414887 create-app-fastapi-0.0.6/projectfastapi/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.6/projectfastapi/__init__.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     3976 2024-05-03 09:48:17.000000 create-app-fastapi-0.0.6/projectfastapi/main.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     2243 2024-05-03 09:47:51.000000 create-app-fastapi-0.0.6/projectfastapi/source.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-05-03 09:48:47.414887 create-app-fastapi-0.0.6/setup.cfg
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      900 2024-05-03 09:48:14.000000 create-app-fastapi-0.0.6/setup.py
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 08:48:14.546987 create-app-fastapi-0.0.7/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1118 2024-05-11 08:48:14.546987 create-app-fastapi-0.0.7/PKG-INFO
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 08:48:14.546987 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1118 2024-05-11 08:48:14.000000 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-05-11 08:48:14.000000 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-05-11 08:48:14.000000 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-05-11 08:48:14.000000 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/entry_points.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-05-11 08:48:14.000000 create-app-fastapi-0.0.7/create_app_fastapi.egg-info/top_level.txt
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 08:48:14.546987 create-app-fastapi-0.0.7/projectfastapi/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.7/projectfastapi/__init__.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     5123 2024-05-11 08:47:48.000000 create-app-fastapi-0.0.7/projectfastapi/main.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     2647 2024-05-11 08:44:02.000000 create-app-fastapi-0.0.7/projectfastapi/source.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-05-11 08:48:14.546987 create-app-fastapi-0.0.7/setup.cfg
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1345 2024-05-11 08:47:53.000000 create-app-fastapi-0.0.7/setup.py
```

### Comparing `create-app-fastapi-0.0.6/projectfastapi/main.py` & `create-app-fastapi-0.0.7/projectfastapi/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,142 @@
 import os, platform, sys, subprocess, threading, time, argparse
-from .source import getFileData
+from source import getFileData
 
 def main():
+    try:
+        parser = argparse.ArgumentParser(prog ='create-app-fastapi', description="Create fastapi project") 
+        parser.add_argument('name', metavar ='NAME', type = str, help ='create a project in this name')
+        parser.add_argument('-v','--version',action='version',
+                        version='%(prog)s 0.0.6', help ="show program's version number and exit")
+        args = parser.parse_args()
+
+        curdir= os.getcwd()
+        platformOS= platform.system()
+        threadStop= False
+
+        # terminal color code
+        RED = "\033[31m"
+        GREEN = "\033[32m"
+        RESET = "\033[0m"
+
+        # Inputs
+        name= args.name
+        virENV= input("Virtual environment name (default 'venv'): ")
+        virENV= virENV if virENV else 'venv'
+        dependencies= ['fastapi[all]','sqlalchemy','pytest']
+
+        # get file data
+        fileData= getFileData(name, virENV)
+
+        # create folders and files
+        def create_dir(folderName, base= False):
+            fullFolderName= folderName if base else os.path.join(name, folderName)
+            files= {'settings':['auth.py','config.py','db.py'], 'models':['model.py'],'schemas':['schema.py'],'APIs':['api.py'],'testcase':['test_main.py']}
+            try:
+                if os.path.exists(fullFolderName):
+                    exit(RED + f"Folder {fullFolderName} already exists" + RESET)
+                os.mkdir(fullFolderName)
+
+                # create files inside folder
+                if files.get(folderName):
+                    for file in files[folderName]:
+                        with open(f"{fullFolderName}/{file}", 'w') as f:
+                            f.writelines(fileData[file])
+                if not base:
+                    with open(fullFolderName+'/__init__.py','w') as f:
+                        pass
+            except Exception as err:
+                exit(err)
+
+        # display loading
+        def loading():
+            load= 0
+            symbol=['*   ',' *  ','  * ','   *']
+            while True:
+                print("\r", end="")
+                print("Setup virtual environment and installing dependencies", end="")
+                print(GREEN,symbol[load],RESET, end="")
+                load +=1
+                time.sleep(0.5)
+                if load >= 3:   load= 0
+                if threadStop:    
+                    print()
+                    break
+
+        # execute system cmd using subprocess
+        def run(cmd):
+            status= subprocess.run(cmd, shell=True,cwd=os.path.join(curdir, name),capture_output=True)
+            if status.returncode != 0:
+                raise Exception(status.stderr.decode('utf-8'))
+        
+        # function to delete project if error
+        def errorExit(error):
+            run(f"rm -rf {os.path.join(curdir, name)}")
+            exit(F"{error}\n")
 
-    parser = argparse.ArgumentParser(prog ='create-app-fastapi', description="Create fastapi project") 
-    parser.add_argument('name', metavar ='NAME', type = str, help ='create a project in this name')
-    parser.add_argument('-v','--version',action='version',
-                    version='%(prog)s 0.0.6', help ="show program's version number and exit")
-    args = parser.parse_args()
-
-    curdir= os.getcwd()
-    platformOS= platform.system()
-    threadStop= False
-
-    # terminal color code
-    RED = "\033[31m"
-    GREEN = "\033[32m"
-    RESET = "\033[0m"
-
-    # Inputs
-    name= args.name
-    virENV= input("Virtual environment name (default 'venv'): ")
-    virENV= virENV if virENV else 'venv'
-
-    # get file data
-    fileData= getFileData(name, virENV)
-
-    # create folders and files
-    def create_dir(folderName, base= False):
-        fullFolderName= folderName if base else os.path.join(name, folderName)
-        files= {'settings':['auth.py','config.py','db.py'], 'models':['model.py'],'schemas':['schema.py'],'APIs':['api.py']}
-        try:
-            if os.path.exists(fullFolderName):
-                exit(RED + f"Folder {fullFolderName} already exists" + RESET)
-            os.mkdir(fullFolderName)
-
-            # create files inside folder
-            if files.get(folderName):
-                for file in files[folderName]:
-                    with open(f"{fullFolderName}/{file}", 'w') as f:
-                        f.writelines(fileData[file])
-            if not base:
-                with open(fullFolderName+'/__init__.py','w') as f:
-                    pass
-        except Exception as err:
-            exit(err)
-
-    # display loading
-    def loading():
-        load= 0
-        symbol=['*   ',' *  ','  * ','   *']
-        while True:
-            print("\r", end="")
-            print("Setup virtual environment and installing dependencies", end="")
-            print(GREEN,symbol[load],RESET, end="")
-            load +=1
-            time.sleep(0.5)
-            if load >= 3:   load= 0
-            if threadStop:    
-                print()
-                break
-
-    # execute system cmd using subprocess
-    def run(cmd):
-        subprocess.run(cmd, shell=True,cwd=os.path.join(curdir, name), stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-
-
-    # thread for display loading same time of execute cmd
-    thread= threading.Thread(target=loading)
-
-    # create project directory
-    create_dir(name, base= True)
+        # thread for display loading same time of execute cmd
+        thread= threading.Thread(target=loading)
 
-    dependencies= ['fastapi[all]','sqlalchemy']
+        # create project directory
+        create_dir(name, base= True)
 
-    try:
+        # Start loading thread for show loading while install dependencies
         thread.start()
-        if platformOS == 'Linux':
-            run(f"{sys.executable} -m venv {virENV}")
-            run(f"{virENV}/bin/pip install {' '.join(dependencies)}")
-            run(f"{virENV}/bin/pip freeze > requirements.txt")
-
-        elif platformOS == 'Windows':
-            run(f"{sys.executable} -m venv {virENV}")
-            run(f"{virENV}\Scripts\pip3.exe install {' '.join(dependencies)}")
-            run(f"{virENV}\Scripts\pip3.exe freeze > requirements.txt")
+        err= False
 
+        try:
+            if platformOS == 'Linux':
+                run(f"{sys.executable} -m venv {virENV}")
+                run(f"{virENV}/bin/pip install {' '.join(dependencies)}")
+                run(f"{virENV}/bin/pip freeze > requirements.txt")
+
+            elif platformOS == 'Windows':
+                run(f"{sys.executable} -m venv {virENV}")
+                run(f"{virENV}\Scripts\pip.exe install {' '.join(dependencies)}")
+                run(f"{virENV}\Scripts\pip3.exe freeze > requirements.txt")
+        except Exception as error:
+            err=error
+
+        # Stop the thread after istall dependencies
+        threadStop= True
+        thread.join()
+        
+        if err:
+            print(RED+'\nError while creating virtual environment'+RESET)
+            errorExit(err)
+
+
+        # project folders
+        project_dirs= ['settings', 'models', 'schemas', 'APIs', 'testcase']
+
+        # loop for creating folders
+        for dir in project_dirs:
+            create_dir(dir)
+
+        # creating base files
+        base_files= ['main.py', '.gitignore','.env']
+        for file in base_files:
+            with open(f'{name}/{file}','w') as f:
+                f.writelines(fileData[file])
+
+
+        print(f"""{GREEN}Project created successfully!{RESET}
+
+        Note: activate virtual environment before run source {GREEN}main.py{RESET}
+        Run API service : fastapi dev main.py
+        Run testcase : pytest -v
+        {GREEN}Have a nice day! {RESET}
+        """)
+
+        openvs= input("Open project in VS Code? (y/n): ")
+        if openvs.lower() == 'y':
+            run("code .")
+        return
+    except KeyboardInterrupt:
+        threadStop= True
+        thread.join()
+        errorExit(RED+"Error: Cancelled by user"+RESET)
+    except Exception as error:
+        print(error)
         threadStop= True
         thread.join()
-    except Exception as err:
-        print(RED+'Error while creating virtual environment'+RESET,err)
-        virENV= False
-
-    # project folders
-    project_dirs= ['settings', 'models', 'schemas', 'APIs', 'testcase']
-
-    # loop for creating folders
-    for dir in project_dirs:
-        create_dir(dir)
-
-    # creating base files
-    base_files= ['main.py', '.gitignore','.env']
-    for file in base_files:
-        with open(f'{name}/{file}','w') as f:
-            f.writelines(fileData[file])
-
-
-    print(f"""{GREEN}Project created successfully!{RESET}
-
-    Note: activate virtual environment before run source {GREEN}main.py{RESET}
-    {GREEN}Have a nice day! {RESET}
-    """)
-
-    openvs= input("Open project in VS Code? (y/n): ")
-    if openvs.lower() == 'y':
-        run("code .")
-    return
+        errorExit(error)
```

### Comparing `create-app-fastapi-0.0.6/projectfastapi/source.py` & `create-app-fastapi-0.0.7/projectfastapi/source.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #jwt token code here
 def genToken():
     pass
 
 def authenticate():
     pass
 
-#user password encrypt decrypt
+#user password encrypt verify
 def encrypt_pwd():
     pass
 
 def verify_pwd():
     pass
 """
 
@@ -105,20 +105,39 @@
     tags=["api"]
 )
 @app.get('/')
 def initial():
     return {"message": "Serive from API routes"}
 """
 
+#api file
+def test_main():
+    return """from fastapi.testclient import TestClient
+from main import app
+
+client = TestClient(app)
+
+# the main service test case
+def test_main():
+    response= client.get('/')
+    assert response.status_code == 200
+
+# the api test case
+def test_api():
+    response= client.get('/api/v1')
+    assert response.status_code == 200
+""" 
+
 def getFileData(name, venv):
     return {
             'auth.py': auth(),
             'config.py': config(),
             'db.py': db(),
             'model.py': model(),
             'schema.py': schema(),
             'api.py': api(),
-            'main.py': main(name), 
+            'main.py': main(name),
+            'test_main.py': test_main(),
             '.gitignore':gitignore(venv),
-            '.env':env()
+            '.env':env(),
             }
```

### Comparing `create-app-fastapi-0.0.6/setup.py` & `create-app-fastapi-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 from setuptools import setup, find_packages
 
 setup( 
 	name="create-app-fastapi", 
-	version="0.0.6", 
+	version="0.0.7", 
 	author="Ravishnu", 
 	author_email="ravishnu60@gmail.com", 
 	packages=find_packages(), 
     url="https://github.com/ravishnu60/create-app-fastapi.git",
 	description="Library for initializing FastAPI projects - create-app-fastapi", 
 	long_description="""A package used to create fastAPI project structure with virtual environment and dependencies.
     Once you install this package use below command to create fastapi project,
     
     create-app-fastapi project-name
     
+    The Project structure will be created in current working directory.
+    The structure will be,
+    
+		root-folder
+		|-APIs
+		|  |-__init__.py
+		|  |-api.py
+		|-models
+		|  |-__init__.py
+		|  |-model.py
+		|-schemas
+		|  |-__init__.py
+		|  |-schema.py
+		|-settings
+		|  |-__init__.py
+		|  |-auth.py
+		|  |-config.py
+		|  |-db.py
+		|-testcase
+		|  |-__init__.py
+		|  |-test_main.py
+		|-venv
+		|-.gitignore
+		|-main.py
+		|-requirements.txt
+    
     """, 
 	long_description_content_type="text/markdown", 
 	python_requires='>=3.9', 
 	install_requires=[],
 	entry_points ={ 
 		'console_scripts': [ 
 			'create-app-fastapi=projectfastapi.main:main'
```

