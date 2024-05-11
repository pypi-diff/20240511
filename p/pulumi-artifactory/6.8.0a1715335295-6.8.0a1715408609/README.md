# Comparing `tmp/pulumi_artifactory-6.8.0a1715335295.tar.gz` & `tmp/pulumi_artifactory-6.8.0a1715408609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-6.8.0a1715335295.tar", last modified: Fri May 10 10:04:06 2024, max compression
+gzip compressed data, was "pulumi_artifactory-6.8.0a1715408609.tar", last modified: Sat May 11 06:27:37 2024, max compression
```

## Comparing `pulumi_artifactory-6.8.0a1715335295.tar` & `pulumi_artifactory-6.8.0a1715408609.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (127)    52175 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   589480 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    36736 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    51222 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    21268 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_property_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    22027 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifactory_release_bundle_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    37133 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/build_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    22064 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    48832 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    55251 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    63807 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    67159 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58684 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58624 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    69277 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    62611 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    68899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58564 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58548 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58264 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    81849 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    64747 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    81669 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    81789 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58324 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    64870 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    63862 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    74217 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    81669 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    59042 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58564 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    20773 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18961 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19175 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19891 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    21424 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19146 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    24081 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20518 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23838 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23742 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23838 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19731 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_file_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    17460 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14938 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    17413 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18575 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23545 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_huggingfaceml_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    21757 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14109 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    39710 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    40035 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    39890 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    36882 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35518 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44626 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    37153 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    36487 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    47038 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    41898 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    46657 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    48350 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35870 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    42269 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    41677 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35179 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35249 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    46657 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    35518 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    37599 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    39897 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16037 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13147 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15924 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/global_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    41861 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    29798 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)    35287 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_group_setting_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    51241 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    48083 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_setting_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    53791 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45157 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45119 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    47872 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45900 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45069 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44891 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    67509 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    51180 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45457 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_huggingfaceml_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    68274 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    67529 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44929 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    51971 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    50587 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44929 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45043 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    23801 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    58014 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    65761 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    68274 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45315 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45289 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45361 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    45081 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    24739 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/mail_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27227 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    43126 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)   543325 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/password_expiration_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    28406 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    46081 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)    20769 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/release_bundle_custom_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    20304 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)   128911 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   137445 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   138727 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128799 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   138052 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   137706 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   131782 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128847 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128781 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128893 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   152049 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128777 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   131621 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128935 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   131613 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   153047 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   143849 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   146226 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   129362 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_huggingfaceml_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   152885 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   155006 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   130853 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   144037 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   145583 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128829 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128725 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128767 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128891 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   137973 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    41818 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)   128741 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   152771 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   128813 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   132496 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)   139285 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26662 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    43483 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    62144 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27814 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/user_lock_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    40717 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    44928 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38224 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34919 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    41183 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38226 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38184 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    50459 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38641 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34745 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34817 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    46176 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    42550 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38508 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_helmoci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    46062 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    48249 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38603 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_oci_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34657 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34703 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34821 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34729 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    46084 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    33871 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    34547 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-10 10:04:06.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-05-10 10:04:06.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:04:06.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 10:04:06.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 10:04:06.000000 pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 10:03:59.000000 pulumi_artifactory-6.8.0a1715335295/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:04:06.180527 pulumi_artifactory-6.8.0a1715335295/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (127)    52175 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   589480 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36736 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51222 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21268 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_property_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22027 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifactory_release_bundle_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37133 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/build_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22064 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48832 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55251 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63807 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67159 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58684 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58624 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69277 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62611 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58564 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58548 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58264 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81849 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64747 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81669 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81789 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58324 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64870 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63862 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74217 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81669 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58444 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59042 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58564 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20773 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18961 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19175 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19891 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21424 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19146 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24081 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20518 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23838 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23742 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23838 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18968 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19731 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17460 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14938 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17413 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18575 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23545 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_huggingfaceml_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23581 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21757 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14109 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39710 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40035 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39890 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36882 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35518 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44626 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37153 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36487 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47038 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41898 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46657 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48350 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35870 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42269 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41677 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35179 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35249 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46657 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35518 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37599 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39897 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16037 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13147 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15924 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/global_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41861 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29798 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35287 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_group_setting_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51241 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48083 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_setting_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53791 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45157 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45119 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47872 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45900 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45069 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44891 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67509 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51180 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45457 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_huggingfaceml_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68274 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67529 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44929 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51971 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50587 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44929 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45043 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44967 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23801 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58014 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65761 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68274 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45005 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45315 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45289 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45361 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45081 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24739 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/mail_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26149 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43126 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)   543325 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/password_expiration_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28406 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46081 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20769 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/release_bundle_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20304 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128911 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137445 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138727 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128799 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138052 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137706 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131782 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128847 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128781 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128893 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152049 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128777 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131621 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128935 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131613 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   153047 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143849 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146226 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129362 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_huggingfaceml_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152885 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155006 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130853 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144037 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145583 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128829 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128725 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128767 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128891 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137973 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41818 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128741 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152771 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128813 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132496 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139285 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26662 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43483 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62144 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27814 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29281 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/user_lock_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40717 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44928 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38224 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34919 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41183 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38226 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38184 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50459 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38641 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34745 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34817 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46176 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42550 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38508 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_helmoci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46062 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48249 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38603 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_oci_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34657 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34703 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34821 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34729 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46084 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33871 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34547 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-11 06:27:37.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-05-11 06:27:37.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 06:27:37.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 06:27:37.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 06:27:37.000000 pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-11 06:27:31.000000 pulumi_artifactory-6.8.0a1715408609/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 06:27:37.707908 pulumi_artifactory-6.8.0a1715408609/setup.cfg
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/PKG-INFO` & `pulumi_artifactory-6.8.0a1715408609/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_artifactory
-Version: 6.8.0a1715335295
+Version: 6.8.0a1715408609
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi,artifactory
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/README.md` & `pulumi_artifactory-6.8.0a1715408609/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/__init__.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/access_token.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/api_key.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_property_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_property_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifactory_release_bundle_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifactory_release_bundle_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/backup.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/build_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/build_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/certificate.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/__init__.pyi` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_public_key.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/general_security.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/general_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,13 +181,13 @@
         __props__ = _GeneralSecurityState.__new__(_GeneralSecurityState)
 
         __props__.__dict__["enable_anonymous_access"] = enable_anonymous_access
         return GeneralSecurity(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="enableAnonymousAccess")
-    def enable_anonymous_access(self) -> pulumi.Output[Optional[bool]]:
+    def enable_anonymous_access(self) -> pulumi.Output[bool]:
         """
         Enable anonymous access.  Default value is `false`.
         """
         return pulumi.get(self, "enable_anonymous_access")
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_file.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_file_list.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_file_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_group.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_huggingfaceml_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_huggingfaceml_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_repositories.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_user.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/global_environment.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/global_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/group.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/keypair.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_group_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_group_setting_v2.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_group_setting_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/ldap_setting_v2.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/ldap_setting_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_huggingfaceml_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_huggingfaceml_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/mail_server.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/mail_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,50 +5,51 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ManagedUserArgs', 'ManagedUser']
+__all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
-class ManagedUserArgs:
+class UserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
-                 password: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a ManagedUser resource.
+        The set of arguments for constructing a User resource.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         pulumi.set(__self__, "email", email)
-        pulumi.set(__self__, "password", password)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
         """
@@ -58,26 +59,14 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
-    def password(self) -> pulumi.Input[str]:
-        """
-        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
-        """
-        return pulumi.get(self, "password")
-
-    @password.setter
-    def password(self, value: pulumi.Input[str]):
-        pulumi.set(self, "password", value)
-
-    @property
-    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
         (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
@@ -129,39 +118,51 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        """
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
         (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
 @pulumi.input_type
-class _ManagedUserState:
+class _UserState:
     def __init__(__self__, *,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering ManagedUser resources.
+        Input properties used for looking up and filtering User resources.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
         :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
@@ -277,49 +278,59 @@
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
-class ManagedUser(pulumi.CustomResource):
+class User(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
+        Provides an Artifactory user resource. This can be used to create and manage Artifactory users.
+        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later. When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
+
+        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        test_user = artifactory.ManagedUser("test-user",
+        test_user = artifactory.User("test-user",
             name="terraform",
             password="my super secret password",
             email="test-user@artifactory-terraform.com",
-            groups=[
-                "readers",
-                "logged-in-users",
-            ])
+            admin=False,
+            profile_updatable=True,
+            disable_ui_access=False,
+            internal_password_disabled=False,
+            groups=["logged-in-users"])
         ```
 
+        ## Managing groups relationship
+
+        See our recommendation on how to manage user-group relationship.
+
         ## Import
 
         ```sh
-        $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
+        $ pulumi import artifactory:index/user:User test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
@@ -329,46 +340,56 @@
         :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ManagedUserArgs,
+                 args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory user resource. This can be used to create and manage Artifactory users.
+        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later. When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
+
+        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        test_user = artifactory.ManagedUser("test-user",
+        test_user = artifactory.User("test-user",
             name="terraform",
             password="my super secret password",
             email="test-user@artifactory-terraform.com",
-            groups=[
-                "readers",
-                "logged-in-users",
-            ])
+            admin=False,
+            profile_updatable=True,
+            disable_ui_access=False,
+            internal_password_disabled=False,
+            groups=["logged-in-users"])
         ```
 
+        ## Managing groups relationship
+
+        See our recommendation on how to manage user-group relationship.
+
         ## Import
 
         ```sh
-        $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
+        $ pulumi import artifactory:index/user:User test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
-        :param ManagedUserArgs args: The arguments to use to populate this resource's properties.
+        :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ManagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -384,32 +405,30 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ManagedUserArgs.__new__(ManagedUserArgs)
+            __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
             __props__.__dict__["name"] = name
-            if password is None and not opts.urn:
-                raise TypeError("Missing required property 'password'")
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ManagedUser, __self__).__init__(
-            'artifactory:index/managedUser:ManagedUser',
+        super(User, __self__).__init__(
+            'artifactory:index/user:User',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -417,17 +436,17 @@
             admin: Optional[pulumi.Input[bool]] = None,
             disable_ui_access: Optional[pulumi.Input[bool]] = None,
             email: Optional[pulumi.Input[str]] = None,
             groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             internal_password_disabled: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             password: Optional[pulumi.Input[str]] = None,
-            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'ManagedUser':
+            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'User':
         """
-        Get an existing ManagedUser resource's state with the given name, id, and optional extra
+        Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
@@ -436,25 +455,25 @@
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
         :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ManagedUserState.__new__(_ManagedUserState)
+        __props__ = _UserState.__new__(_UserState)
 
         __props__.__dict__["admin"] = admin
         __props__.__dict__["disable_ui_access"] = disable_ui_access
         __props__.__dict__["email"] = email
         __props__.__dict__["groups"] = groups
         __props__.__dict__["internal_password_disabled"] = internal_password_disabled
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
         __props__.__dict__["profile_updatable"] = profile_updatable
-        return ManagedUser(resource_name, opts=opts, __props__=__props__)
+        return User(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def admin(self) -> pulumi.Output[bool]:
         """
         (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/outputs.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/password_expiration_policy.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/password_expiration_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/property_set.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/property_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/provider.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/proxy.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/release_bundle_custom_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/release_bundle_custom_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_huggingfaceml_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_huggingfaceml_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/repository_layout.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/scoped_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/unmanaged_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/user.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/managed_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,51 +5,50 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['UserArgs', 'User']
+__all__ = ['ManagedUserArgs', 'ManagedUser']
 
 @pulumi.input_type
-class UserArgs:
+class ManagedUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
+                 password: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a User resource.
+        The set of arguments for constructing a ManagedUser resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
-        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "password", password)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
         """
@@ -59,14 +58,26 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        """
+        (Optional, Sensitive) Password for the user.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
         (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
@@ -118,58 +129,46 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        """
-        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
-        """
-        return pulumi.get(self, "password")
-
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
-
-    @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
         (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
 @pulumi.input_type
-class _UserState:
+class _ManagedUserState:
     def __init__(__self__, *,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering User resources.
+        Input properties used for looking up and filtering ManagedUser resources.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
-        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user.
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if email is not None:
@@ -257,15 +256,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        (Optional, Sensitive) Password for the user.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -278,118 +277,98 @@
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
-class User(pulumi.CustomResource):
+class ManagedUser(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Provides an Artifactory user resource. This can be used to create and manage Artifactory users.
-        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later. When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
-
-        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        test_user = artifactory.User("test-user",
+        test_user = artifactory.ManagedUser("test-user",
             name="terraform",
             password="my super secret password",
             email="test-user@artifactory-terraform.com",
-            admin=False,
-            profile_updatable=True,
-            disable_ui_access=False,
-            internal_password_disabled=False,
-            groups=["logged-in-users"])
+            groups=[
+                "readers",
+                "logged-in-users",
+            ])
         ```
 
-        ## Managing groups relationship
-
-        See our recommendation on how to manage user-group relationship.
-
         ## Import
 
         ```sh
-        $ pulumi import artifactory:index/user:User test-user myusername
+        $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
-        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user.
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UserArgs,
+                 args: ManagedUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides an Artifactory user resource. This can be used to create and manage Artifactory users.
-        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later. When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
-
-        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        test_user = artifactory.User("test-user",
+        test_user = artifactory.ManagedUser("test-user",
             name="terraform",
             password="my super secret password",
             email="test-user@artifactory-terraform.com",
-            admin=False,
-            profile_updatable=True,
-            disable_ui_access=False,
-            internal_password_disabled=False,
-            groups=["logged-in-users"])
+            groups=[
+                "readers",
+                "logged-in-users",
+            ])
         ```
 
-        ## Managing groups relationship
-
-        See our recommendation on how to manage user-group relationship.
-
         ## Import
 
         ```sh
-        $ pulumi import artifactory:index/user:User test-user myusername
+        $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
-        :param UserArgs args: The arguments to use to populate this resource's properties.
+        :param ManagedUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ManagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -405,30 +384,32 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UserArgs.__new__(UserArgs)
+            __props__ = ManagedUserArgs.__new__(ManagedUserArgs)
 
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
             __props__.__dict__["name"] = name
+            if password is None and not opts.urn:
+                raise TypeError("Missing required property 'password'")
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(User, __self__).__init__(
-            'artifactory:index/user:User',
+        super(ManagedUser, __self__).__init__(
+            'artifactory:index/managedUser:ManagedUser',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -436,44 +417,44 @@
             admin: Optional[pulumi.Input[bool]] = None,
             disable_ui_access: Optional[pulumi.Input[bool]] = None,
             email: Optional[pulumi.Input[str]] = None,
             groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             internal_password_disabled: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             password: Optional[pulumi.Input[str]] = None,
-            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'User':
+            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'ManagedUser':
         """
-        Get an existing User resource's state with the given name, id, and optional extra
+        Get an existing ManagedUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user. May contain lowercase letters, numbers and symbols: '.-_@'
-        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user.
         :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UserState.__new__(_UserState)
+        __props__ = _ManagedUserState.__new__(_ManagedUserState)
 
         __props__.__dict__["admin"] = admin
         __props__.__dict__["disable_ui_access"] = disable_ui_access
         __props__.__dict__["email"] = email
         __props__.__dict__["groups"] = groups
         __props__.__dict__["internal_password_disabled"] = internal_password_disabled
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
         __props__.__dict__["profile_updatable"] = profile_updatable
-        return User(resource_name, opts=opts, __props__=__props__)
+        return ManagedUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def admin(self) -> pulumi.Output[bool]:
         """
         (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
@@ -519,15 +500,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
-        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        (Optional, Sensitive) Password for the user.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/user_lock_policy.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/user_lock_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_helmoci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_helmoci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_oci_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_oci_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_artifactory
-Version: 6.8.0a1715335295
+Version: 6.8.0a1715408609
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi,artifactory
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_artifactory-6.8.0a1715335295/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-6.8.0a1715408609/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-6.8.0a1715335295/pyproject.toml` & `pulumi_artifactory-6.8.0a1715408609/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_artifactory"
   description = "A Pulumi package for creating and managing artifactory cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "artifactory"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.8.0a1715335295"
+  version = "6.8.0a1715408609"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-artifactory"
 
 [build-system]
```

