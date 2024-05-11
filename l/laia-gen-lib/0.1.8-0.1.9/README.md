# Comparing `tmp/laia-gen-lib-0.1.8.tar.gz` & `tmp/laia-gen-lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laia-gen-lib-0.1.8.tar", last modified: Tue Mar 19 07:48:05 2024, max compression
+gzip compressed data, was "laia-gen-lib-0.1.9.tar", last modified: Thu Mar 28 18:21:04 2024, max compression
```

## Comparing `laia-gen-lib-0.1.8.tar` & `laia-gen-lib-0.1.9.tar`

### file list

```diff
@@ -1,128 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-19 07:48:05.000000 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-19 07:48:05.000000 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 07:48:05.000000 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-19 07:48:05.000000 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-19 07:48:05.000000 laia-gen-lib-0.1.8/laia_gen_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.690233 laia-gen-lib-0.1.8/laiagenlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.690233 laia-gen-lib-0.1.8/laiagenlib/Application/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CheckAccessRightsOfFields.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CheckAccessRightsOfUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CreateAccessRights.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/GetAllowedFields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/CreateLaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/DeleteLaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/ReadLaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/SearchLaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/UpdateLaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/CreateLaiaUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/CreateRole.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/LoginLaiaUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/RegisterLaiaUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/UpdateLaiaUser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/CreateFlutterApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/CreateRoutes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.694233 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateBaseFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateModelsFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateRoutesFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/DownloadImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/ExtractClassInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/Schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/UpdateFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/ValidateEmail.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/ValidatePassword.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Domain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Domain/AccessRights/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/AccessRights/AccessRights.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/AccessRights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaBaseModel/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaBaseModel/LaiaBaseModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaBaseModel/ModelRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaBaseModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaUser/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaUser/Auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaUser/LaiaUser.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaUser/Role.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.698233 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/FlutterBaseFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/Openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/OpenapiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/OpenapiRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/OpenapiRoute.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/RoutesInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/FieldInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/ImportModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/AccessRights/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/AccessRights/CreateAccessRightsController.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/AccessRights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaBaseModel/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaBaseModel/CRUDLaiaBaseModelController.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaBaseModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/AuthController.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/CRUDLaiaUserController.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/CRUDRoleController.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/Openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/Openapi/OpenapiController.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/Openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/Shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Framework/Shared/Exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/Shared/Exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/AccessRights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/AccessRights/MongoAccessRightsRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/AccessRights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.702233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaBaseModel/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaBaseModel/MongoModelRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaBaseModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaUser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaUser/MongoLaiaUserRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaUser/MongoRoleRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/FastAPIOpenapiRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/LaiaFastApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/LaiaFlutter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Shared/Exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Shared/Exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/Infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/laiagenlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:48:05.706233 laia-gen-lib-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:47:56.000000 laia-gen-lib-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-28 18:21:04.000000 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-03-28 18:21:04.000000 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:21:04.000000 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-28 18:21:04.000000 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 18:21:04.000000 laia-gen-lib-0.1.9/laia_gen_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.798364 laia-gen-lib-0.1.9/laiagenlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.798364 laia-gen-lib-0.1.9/laiagenlib/Application/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.798364 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CheckAccessRightsOfFields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CheckAccessRightsOfUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CreateAccessRights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/GetAllowedFields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.798364 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/CreateLaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/DeleteLaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/ReadLaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/SearchLaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/UpdateLaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/CreateLaiaUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/CreateRole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/LoginLaiaUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/RegisterLaiaUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/UpdateLaiaUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/CreateFlutterApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/CreateRoutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateBaseFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateModelsFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateRoutesFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/DownloadImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/ExtractClassInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/Schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/UpdateFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/ValidateEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/ValidatePassword.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.802364 laia-gen-lib-0.1.9/laiagenlib/Domain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/AccessRights/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/AccessRights/AccessRights.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/AccessRights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/GeoJSON/
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/GeoJSON/Geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/GeoJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaBaseModel/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaBaseModel/LaiaBaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaBaseModel/ModelRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaBaseModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaUser/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaUser/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaUser/LaiaUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaUser/Role.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/FlutterBaseFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/Openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/OpenapiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/OpenapiRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/OpenapiRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/RoutesInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.806364 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/FieldInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/ImportModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/AccessRights/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/AccessRights/CreateAccessRightsController.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/AccessRights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaBaseModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaBaseModel/CRUDLaiaBaseModelController.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaBaseModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/AuthController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/CRUDLaiaUserController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/CRUDRoleController.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/Openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/Openapi/OpenapiController.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/Openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/Shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Framework/Shared/Exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/Shared/Exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/AccessRights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/AccessRights/MongoAccessRightsRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/AccessRights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaBaseModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaBaseModel/MongoModelRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaBaseModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.810364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaUser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaUser/MongoLaiaUserRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaUser/MongoRoleRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/FastAPIOpenapiRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/LaiaFastApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/LaiaFlutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Shared/Exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Shared/Exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/Infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/laiagenlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:21:04.814364 laia-gen-lib-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:20:55.000000 laia-gen-lib-0.1.9/tests/__init__.py
```

### Comparing `laia-gen-lib-0.1.8/README.md` & `laia-gen-lib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laia_gen_lib.egg-info/SOURCES.txt` & `laia-gen-lib-0.1.9/laia_gen_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 laiagenlib/Application/Shared/Utils/UpdateFile.py
 laiagenlib/Application/Shared/Utils/ValidateEmail.py
 laiagenlib/Application/Shared/Utils/ValidatePassword.py
 laiagenlib/Application/Shared/Utils/__init__.py
 laiagenlib/Domain/__init__.py
 laiagenlib/Domain/AccessRights/AccessRights.py
 laiagenlib/Domain/AccessRights/__init__.py
+laiagenlib/Domain/GeoJSON/Geometry.py
+laiagenlib/Domain/GeoJSON/__init__.py
 laiagenlib/Domain/LaiaBaseModel/LaiaBaseModel.py
 laiagenlib/Domain/LaiaBaseModel/ModelRepository.py
 laiagenlib/Domain/LaiaBaseModel/__init__.py
 laiagenlib/Domain/LaiaUser/Auth.py
 laiagenlib/Domain/LaiaUser/LaiaUser.py
 laiagenlib/Domain/LaiaUser/Role.py
 laiagenlib/Domain/LaiaUser/__init__.py
```

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CheckAccessRightsOfFields.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CheckAccessRightsOfFields.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CheckAccessRightsOfUser.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CheckAccessRightsOfUser.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/AccessRights/CreateAccessRights.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/AccessRights/CreateAccessRights.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/CreateLaiaBaseModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/CreateLaiaBaseModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/DeleteLaiaBaseModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/DeleteLaiaBaseModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/ReadLaiaBaseModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/ReadLaiaBaseModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/SearchLaiaBaseModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/SearchLaiaBaseModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaBaseModel/UpdateLaiaBaseModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaBaseModel/UpdateLaiaBaseModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/CreateLaiaUser.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/CreateLaiaUser.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/CreateRole.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/CreateRole.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/LoginLaiaUser.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/LoginLaiaUser.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/RegisterLaiaUser.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/RegisterLaiaUser.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/LaiaUser/UpdateLaiaUser.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/LaiaUser/UpdateLaiaUser.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/CreateFlutterApp.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/CreateFlutterApp.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 import yaml
 import asyncio
 from ...Domain.Openapi.Openapi import OpenAPI
 from ...Domain.AccessRights.AccessRights import AccessRight
 from ...Domain.LaiaUser.Role import Role
 from ...Domain.Shared.Utils.ImportModel import import_model
-from ...Domain.Openapi.FlutterBaseFiles import model_dart, home_dart
+from ...Domain.Openapi.FlutterBaseFiles import model_dart, home_dart, geojson_models_file
 
 async def create_flutter_app(openapi: OpenAPI=None, app_name:str="", app_path: str="", models_path: str=""):
     subprocess.run("flutter create " + app_name, shell=True)
 
     # TODO: change the following local dart libraries to the ones on the marketç
     await asyncio.gather(
         run("flutter pub add laia_annotations -C " + f"./{app_name}"),
@@ -32,14 +32,17 @@
 
     for openapiModel in openapi.models:
         model_module = import_model(models_path)
         model = getattr(model_module, openapiModel.model_name)
         model_file_content = model_dart(openapiModel, app_name, model)
         with open(os.path.join(app_path, 'lib', 'models', f'{model.__name__.lower()}.dart'), 'w') as f:
             f.write(model_file_content)
+    
+    with open(os.path.join(app_path, 'lib', 'models', 'geometry.dart'), 'w') as f:
+        f.write(geojson_models_file())
 
     laia_models = [AccessRight, Role]
     for model in laia_models:
         model_file_content = model_dart(app_name=app_name, model=model)
         with open(os.path.join(app_path, 'lib', 'models', f'{model.__name__.lower()}.dart'), 'w') as f:
             f.write(model_file_content)
```

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Openapi/CreateRoutes.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Openapi/CreateRoutes.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateBaseFiles.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateBaseFiles.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateModelsFile.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateModelsFile.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,43 @@
 import re
 from .ExtractClassInfo import extract_class_info
 from .UpdateFile import update_file
 from ....Domain.Shared.Utils.logger import _logger
 
 T = TypeVar('T', bound='BaseModel')
 
-def create_models_file(input_file="openapi.yaml", output_file="model.py", models: List[any] = []):
+def create_models_file(input_file="openapi.yaml", output_file="model.py", models: List[any] = [], excluded_models: List[str] = []):
     # This function uses the datamodel-code-generator for generating the pydantic models given a openapi.yaml file. 
     # The generated file is modified so that the pydantic models extend the LaiaBaseModel, this is necessary for 
     # using the Laia library
 
-    excluded_models = ["AccessRight", "Auth", "Role", "ValidationError", "HTTPValidationError"]
-
     subprocess.run(["datamodel-codegen", "--input", input_file, "--output", output_file], check=True)
 
     import_statement = """
 # modified by laia-gen-lib:
 
 from pydantic import ConfigDict
 from laiagenlib.Domain.LaiaBaseModel.LaiaBaseModel import LaiaBaseModel
-from laiagenlib.Domain.LaiaUser.LaiaUser import LaiaUser"""
+from laiagenlib.Domain.LaiaUser.LaiaUser import LaiaUser
+from laiagenlib.Domain.GeoJSON.Geometry import Type, Geometry, LineString, MultiLineString, MultiPoint, MultiPolygon, Point, Polygon"""
 
     with open(output_file, 'r') as f:
         model_content = f.read()
 
     lines = model_content.split('\n')
     import_index = next((i for i, line in enumerate(lines) if "from __future__ import annotations" in line), None)
 
     if import_index is not None:
         lines.insert(import_index + 1, import_statement)
 
     modified_content = '\n'.join(lines)
     modified_content = re.sub(r'class\s+(\w+)\(BaseModel\):', r'class \1(LaiaBaseModel):', modified_content)
 
     excluded_models_pattern = "|".join(excluded_models)
-    model_pattern = re.compile(rf'class ({excluded_models_pattern}|BodySearchElement\w+)\(LaiaBaseModel\):.*?(?=class|$)', re.DOTALL)
+    model_pattern = re.compile(rf'class ({excluded_models_pattern}|BodySearchElement\w+)\(.*?\):.*?(?=class|$)', re.DOTALL)
     modified_content = re.sub(model_pattern, '', modified_content)
     
     for model in models:
         if hasattr(model, 'extensions') and model.extensions:
             model_config_line = f"model_config = ConfigDict(json_schema_extra={model.extensions})"
             modified_content = modified_content.replace(f'class {model.model_name}(LaiaBaseModel):',
                                                         f'class {model.model_name}(LaiaBaseModel):\n    {model_config_line}')
```

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/CreateRoutesFile.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/CreateRoutesFile.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/ExtractClassInfo.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/ExtractClassInfo.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Application/Shared/Utils/UpdateFile.py` & `laia-gen-lib-0.1.9/laiagenlib/Application/Shared/Utils/UpdateFile.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/AccessRights/AccessRights.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/AccessRights/AccessRights.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/LaiaBaseModel/ModelRepository.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/LaiaBaseModel/ModelRepository.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/OpenapiModel.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/OpenapiModel.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/OpenapiRepository.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/OpenapiRepository.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/Openapi/RoutesInfo.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/Openapi/RoutesInfo.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Domain/Shared/Utils/logger.py` & `laia-gen-lib-0.1.9/laiagenlib/Domain/Shared/Utils/logger.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Framework/AccessRights/CreateAccessRightsController.py` & `laia-gen-lib-0.1.9/laiagenlib/Framework/AccessRights/CreateAccessRightsController.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaBaseModel/CRUDLaiaBaseModelController.py` & `laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaBaseModel/CRUDLaiaBaseModelController.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/AuthController.py` & `laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/AuthController.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/CRUDLaiaUserController.py` & `laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/CRUDLaiaUserController.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Framework/LaiaUser/CRUDRoleController.py` & `laia-gen-lib-0.1.9/laiagenlib/Framework/LaiaUser/CRUDRoleController.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Infrastructure/LaiaBaseModel/MongoModelRepository.py` & `laia-gen-lib-0.1.9/laiagenlib/Infrastructure/LaiaBaseModel/MongoModelRepository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import TypeVar, Optional, Dict
+from enum import Enum
 from pydantic import BaseModel
 from bson import ObjectId, regex
 from pymongo.collection import ReturnDocument
+import json
 from ...Application.Shared.Utils.Schemas import list_serial, individual_serial
 from ...Domain.LaiaBaseModel.ModelRepository import ModelRepository
 from ...Domain.Shared.Utils.logger import _logger
 
 
 T = TypeVar('T', bound='BaseModel')
 
@@ -45,14 +47,15 @@
         if item:
             return individual_serial(item)
         raise ValueError(f"{model_name} with ID {item_id} not found")
 
     async def post_item(self, model_name: str, item: T):
         collection = self.db[model_name]
         item_dict = dict(item)
+        item_dict = json.loads(json.dumps(item_dict, default=lambda o: o.value if isinstance(o, Enum) else o))
         item_dict.pop('id', None)
         created_result = collection.insert_one(item_dict)
         inserted_id = created_result.inserted_id
         item_dict['id'] = str(inserted_id)
         item_dict.pop('_id', None)
 
         return item_dict
```

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/FastAPIOpenapiRepository.py` & `laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/FastAPIOpenapiRepository.py`

 * *Files identical despite different names*

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/LaiaFastApi.py` & `laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/LaiaFastApi.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,10 +30,10 @@
 
         backend_dir = os.path.join(os.path.dirname(self.openapi_path), backend_folder_name)
         if not os.path.exists(backend_dir):
             os.makedirs(backend_dir)
 
         models_path = os.path.join(backend_dir, "models.py")
         routes_path = os.path.join(backend_dir, "routes.py")
-        create_models_file(self.openapi_path, models_path, self.openapi.models)
+        create_models_file(self.openapi_path, models_path, self.openapi.models, self.openapi.excluded_models)
         create_routes_file(routes_path)
         await create_crud_routes(self.repository_api_instance, self.repository_instance, self.openapi, models_path, routes_path)
```

### Comparing `laia-gen-lib-0.1.8/laiagenlib/Infrastructure/Openapi/LaiaFlutter.py` & `laia-gen-lib-0.1.9/laiagenlib/Infrastructure/Openapi/LaiaFlutter.py`

 * *Files identical despite different names*

