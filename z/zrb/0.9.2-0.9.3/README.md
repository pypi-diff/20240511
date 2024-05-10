# Comparing `tmp/zrb-0.9.2.tar.gz` & `tmp/zrb-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb-0.9.2.tar", max compression
+gzip compressed data, was "zrb-0.9.3.tar", max compression
```

## Comparing `zrb-0.9.2.tar` & `zrb-0.9.3.tar`

### file list

```diff
@@ -1,1280 +1,1280 @@
--rw-r--r--   0        0        0      728 2023-08-27 04:24:41.005442 zrb-0.9.2/LICENSE
--rw-r--r--   0        0        0    15202 2024-02-25 03:37:59.986130 zrb-0.9.2/README.md
--rw-r--r--   0        0        0     1077 2024-03-10 01:36:55.385095 zrb-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2440 2024-03-10 01:37:06.585159 zrb-0.9.2/src/zrb/__init__.py
--rw-r--r--   0        0        0      314 2024-03-10 01:36:55.385095 zrb-0.9.2/src/zrb/__main__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.009441 zrb-0.9.2/src/zrb/action/__init__.py
--rw-r--r--   0        0        0     4839 2024-03-10 01:36:55.385095 zrb-0.9.2/src/zrb/action/runner.py
--rw-r--r--   0        0        0      548 2024-01-23 09:38:21.729760 zrb-0.9.2/src/zrb/advertisement.py
--rw-r--r--   0        0        0      477 2024-03-10 01:37:06.613159 zrb-0.9.2/src/zrb/builtin/__init__.py
--rw-r--r--   0        0        0     1335 2024-01-23 09:38:21.729760 zrb-0.9.2/src/zrb/builtin/base64.py
--rw-r--r--   0        0        0      613 2024-03-10 01:37:06.617159 zrb-0.9.2/src/zrb/builtin/devtool/__init__.py
--rw-r--r--   0        0        0     1649 2024-03-07 06:21:41.680065 zrb-0.9.2/src/zrb/builtin/devtool/aws/install.sh
--rw-r--r--   0        0        0    15461 2024-02-13 00:58:48.332275 zrb-0.9.2/src/zrb/builtin/devtool/devtool_install.py
--rw-r--r--   0        0        0     3067 2024-03-07 06:21:41.680065 zrb-0.9.2/src/zrb/builtin/devtool/docker/install.sh
--rw-r--r--   0        0        0      531 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/gcloud/install.sh
--rw-r--r--   0        0        0      415 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/gvm/download.sh
--rw-r--r--   0        0        0      538 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/gvm/finalize.sh
--rw-r--r--   0        0        0      253 2024-01-07 03:05:39.354277 zrb-0.9.2/src/zrb/builtin/devtool/gvm/resource/config.sh
--rw-r--r--   0        0        0     1040 2024-02-25 03:37:59.986130 zrb-0.9.2/src/zrb/builtin/devtool/helix/install-language-server.sh
--rw-r--r--   0        0        0     1375 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/helix/install.sh
--rw-r--r--   0        0        0      282 2023-09-14 07:29:41.114392 zrb-0.9.2/src/zrb/builtin/devtool/helix/resource/config.toml
--rw-r--r--   0        0        0       56 2023-08-28 15:53:50.909810 zrb-0.9.2/src/zrb/builtin/devtool/helix/resource/themes/gruvbox_transparent.toml
--rw-r--r--   0        0        0      228 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/helm/install.sh
--rw-r--r--   0        0        0      269 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/kubectl/install.sh
--rw-r--r--   0        0        0      192 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/nvm/download.sh
--rw-r--r--   0        0        0      571 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/nvm/finalize.sh
--rw-r--r--   0        0        0      222 2024-01-07 03:05:39.354277 zrb-0.9.2/src/zrb/builtin/devtool/nvm/resource/config.sh
--rw-r--r--   0        0        0      162 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/pulumi/install.sh
--rw-r--r--   0        0        0       79 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/devtool/pulumi/resource/config.sh
--rw-r--r--   0        0        0     1788 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/pyenv/download.sh
--rw-r--r--   0        0        0      607 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/pyenv/finalize.sh
--rw-r--r--   0        0        0      144 2024-01-07 03:05:39.354277 zrb-0.9.2/src/zrb/builtin/devtool/pyenv/resource/config.sh
--rw-r--r--   0        0        0      160 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/sdkman/download.sh
--rw-r--r--   0        0        0      359 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/sdkman/finalize.sh
--rw-r--r--   0        0        0      173 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/devtool/sdkman/resource/config.sh
--rw-r--r--   0        0        0     1342 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/selenium/install.sh
--rw-r--r--   0        0        0      300 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/terraform/install.sh
--rw-r--r--   0        0        0       84 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/devtool/terraform/resource/config.sh
--rw-r--r--   0        0        0     1229 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/tmux/install.sh
--rw-r--r--   0        0        0      416 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/devtool/tmux/resource/config.sh
--rw-r--r--   0        0        0     1720 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/devtool/zsh/install.sh
--rw-r--r--   0        0        0     5068 2024-02-25 03:37:59.990130 zrb-0.9.2/src/zrb/builtin/devtool/zsh/resource/config.sh
--rw-r--r--   0        0        0      586 2024-02-25 11:35:22.812654 zrb-0.9.2/src/zrb/builtin/docker.py
--rw-r--r--   0        0        0     1134 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/env.py
--rw-r--r--   0        0        0      746 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/eval.py
--rw-r--r--   0        0        0     5353 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/explain.py
--rw-r--r--   0        0        0     1129 2024-03-10 01:37:06.629159 zrb-0.9.2/src/zrb/builtin/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/app_generator/__init__.py
--rw-r--r--   0        0        0     6192 2024-03-10 01:37:06.693159 zrb-0.9.2/src/zrb/builtin/generator/app_generator/add.py
--rw-r--r--   0        0        0     5655 2024-03-10 01:37:06.737160 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/add.py
--rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/__init__.py
--rw-r--r--   0        0        0      353 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_checker.py
--rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py
--rw-r--r--   0        0        0      334 2024-02-25 00:07:25.666566 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/app-activate-venv.sh
--rw-r--r--   0        0        0       15 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/app-start.sh
--rw-r--r--   0        0        0       29 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
--rw-r--r--   0        0        0      126 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
--rw-r--r--   0        0        0       24 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
--rw-r--r--   0        0        0     3843 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py
--rw-r--r--   0        0        0     3500 2024-03-10 01:37:06.765160 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py
--rw-r--r--   0        0        0      311 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py
--rw-r--r--   0        0        0      611 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
--rw-r--r--   0        0        0       31 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/.gitignore
--rw-r--r--   0        0        0       12 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      137 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0     2633 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py
--rw-r--r--   0        0        0       74 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/template.env
--rw-r--r--   0        0        0       83 2023-09-14 07:29:41.114392 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.env
--rw-r--r--   0        0        0      712 2023-10-12 00:54:12.983360 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml
--rw-r--r--   0        0        0     6544 2024-03-10 01:37:06.817160 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/add.py
--rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py
--rw-r--r--   0        0        0     4791 2024-03-10 01:37:06.853160 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py
--rw-r--r--   0        0        0     3829 2024-03-10 01:37:06.885161 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py
--rw-r--r--   0        0        0     2245 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py
--rw-r--r--   0        0        0     1424 2024-03-10 01:37:06.905161 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
--rw-r--r--   0        0        0       60 2023-09-14 07:29:41.114392 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.env
--rw-r--r--   0        0        0      646 2023-10-12 00:54:12.983360 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml
--rw-r--r--   0        0        0       22 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/.dockerignore
--rw-r--r--   0        0        0       39 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/.gitignore
--rw-r--r--   0        0        0      214 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/Dockerfile
--rw-r--r--   0        0        0        7 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/go.work
--rw-r--r--   0        0        0      523 2023-09-02 10:31:35.040307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/main.go
--rw-r--r--   0        0        0       83 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/template.env
--rw-r--r--   0        0        0      481 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/http-port/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_checker.py
--rw-r--r--   0        0        0     1447 2024-03-10 01:37:06.925161 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/http-port-build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
--rw-r--r--   0        0        0      695 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py
--rw-r--r--   0        0        0        0 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/.helmignore
--rw-r--r--   0        0        0     1154 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/Chart.yaml
--rw-r--r--   0        0        0     1791 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/NOTES.txt
--rw-r--r--   0        0        0     1892 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/_helpers.tpl
--rw-r--r--   0        0        0     1915 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/deployment.yaml
--rw-r--r--   0        0        0     1024 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/hpa.yaml
--rw-r--r--   0        0        0     2101 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/ingress.yaml
--rw-r--r--   0        0        0      394 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/service.yaml
--rw-r--r--   0        0        0      342 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      412 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0     1885 2023-09-02 10:31:35.044307 zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/values.yaml
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/cmd_task/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-10 01:37:06.953161 zrb-0.9.2/src/zrb/builtin/generator/cmd_task/add.py
--rw-r--r--   0        0        0      489 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/cmd_task/template/_automate/snake_zrb_task_name.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/common/__init__.py
--rw-r--r--   0        0        0     1899 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/common/helper.py
--rw-r--r--   0        0        0     3272 2024-03-10 01:37:07.089161 zrb-0.9.2/src/zrb/builtin/generator/common/task_factory.py
--rw-r--r--   0        0        0     5190 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/common/task_input.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/__init__.py
--rw-r--r--   0        0        0     2710 2024-03-10 01:37:07.133162 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/add.py
--rw-r--r--   0        0        0     1328 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/_automate/snake_zrb_task_name.py
--rw-r--r--   0        0        0       12 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/.dockerignore
--rw-r--r--   0        0        0       30 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/.gitignore
--rw-r--r--   0        0        0       72 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.env
--rw-r--r--   0        0        0      762 2023-10-12 00:54:12.983360 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.yml
--rw-r--r--   0        0        0      275 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/Dockerfile
--rw-r--r--   0        0        0      511 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/main.py
--rw-r--r--   0        0        0      525 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/__init__.py
--rw-r--r--   0        0        0     7413 2024-03-10 01:37:07.189162 zrb-0.9.2/src/zrb/builtin/generator/fastapp/add.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/__init__.py
--rw-r--r--   0        0        0     2263 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_checker.py
--rw-r--r--   0        0        0     2987 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_config.py
--rw-r--r--   0        0        0     1178 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env.py
--rw-r--r--   0        0        0      602 2024-03-10 01:37:07.197162 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env_file.py
--rw-r--r--   0        0        0     3938 2024-03-10 01:37:07.229162 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_get_start_microservices.py
--rw-r--r--   0        0        0     2631 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_helper.py
--rw-r--r--   0        0        0     1892 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_input.py
--rw-r--r--   0        0        0      334 2024-02-25 00:07:25.666566 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/activate-venv.sh
--rw-r--r--   0        0        0      155 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-build-frontend.sh
--rw-r--r--   0        0        0      377 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-load-test.sh
--rw-r--r--   0        0        0       48 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-prepare-backend.sh
--rw-r--r--   0        0        0       49 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-prepare-load-test.sh
--rw-r--r--   0        0        0       56 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-start.sh
--rw-r--r--   0        0        0      308 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-test.sh
--rw-r--r--   0        0        0       29 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
--rw-r--r--   0        0        0      126 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
--rw-r--r--   0        0        0       24 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
--rw-r--r--   0        0        0       15 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/config/modules.json
--rw-r--r--   0        0        0     4408 2024-03-10 01:37:07.261163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/container.py
--rw-r--r--   0        0        0     2513 2024-03-10 01:37:07.281163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/deployment.py
--rw-r--r--   0        0        0     1878 2024-03-10 01:37:07.297163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/frontend.py
--rw-r--r--   0        0        0     1947 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/image.py
--rw-r--r--   0        0        0     2769 2024-03-10 01:37:07.321163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/load_test.py
--rw-r--r--   0        0        0     6454 2024-03-10 01:37:07.377163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/local.py
--rw-r--r--   0        0        0     2183 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/test.py
--rw-r--r--   0        0        0       53 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/.gitignore
--rw-r--r--   0        0        0    10176 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/README.md
--rw-r--r--   0        0        0       56 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/all-module-disabled.env
--rw-r--r--   0        0        0       54 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/all-module-enabled.env
--rw-r--r--   0        0        0       12 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      137 2023-08-27 04:24:41.013442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0     1139 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/README.md
--rw-r--r--   0        0        0     1519 2024-03-10 01:37:07.393163 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/__main__.py
--rw-r--r--   0        0        0     4943 2024-03-07 06:21:52.652119 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/_common.py
--rw-r--r--   0        0        0     6043 2024-03-10 01:37:07.449164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/app_helper.py
--rw-r--r--   0        0        0      351 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/.helmignore
--rw-r--r--   0        0        0      231 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.lock
--rw-r--r--   0        0        0     1075 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.yaml
--rw-r--r--   0        0        0   185265 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/README.md
--rw-r--r--   0        0        0      360 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/.helmignore
--rw-r--r--   0        0        0      531 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/Chart.yaml
--rw-r--r--   0        0        0     7191 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/README.md
--rw-r--r--   0        0        0     5480 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     7044 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1494 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_compatibility.tpl
--rw-r--r--   0        0        0     1703 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     4071 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2431 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0     2147 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2497 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     1980 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_resources.tpl
--rw-r--r--   0        0        0     7908 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      698 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0     1385 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2599 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0     3449 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2644 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     4059 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4449 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     4003 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5091 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3334 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2526 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      182 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/values.yaml
--rw-r--r--   0        0        0     7987 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/NOTES.txt
--rw-r--r--   0        0        0    14792 2024-03-07 06:21:41.684065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/_helpers.tpl
--rw-r--r--   0        0        0     6066 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/cronjob.yaml
--rw-r--r--   0        0        0     1617 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/pvc.yaml
--rw-r--r--   0        0        0      189 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/extra-list.yaml
--rw-r--r--   0        0        0     1047 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/configmap.yaml
--rw-r--r--   0        0        0      818 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/extended-configmap.yaml
--rw-r--r--   0        0        0      755 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/initialization-configmap.yaml
--rw-r--r--   0        0        0      690 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-configmap.yaml
--rw-r--r--   0        0        0     1418 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-svc.yaml
--rw-r--r--   0        0        0     3247 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/networkpolicy.yaml
--rw-r--r--   0        0        0     2314 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/servicemonitor.yaml
--rw-r--r--   0        0        0    38198 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/statefulset.yaml
--rw-r--r--   0        0        0     1827 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc-headless.yaml
--rw-r--r--   0        0        0     2883 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc.yaml
--rw-r--r--   0        0        0     1043 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1069 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/psp.yaml
--rw-r--r--   0        0        0      829 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/extended-configmap.yaml
--rw-r--r--   0        0        0      734 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-configmap.yaml
--rw-r--r--   0        0        0     1473 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-svc.yaml
--rw-r--r--   0        0        0     3365 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/networkpolicy.yaml
--rw-r--r--   0        0        0     2368 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/servicemonitor.yaml
--rw-r--r--   0        0        0    33309 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/statefulset.yaml
--rw-r--r--   0        0        0     1910 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc-headless.yaml
--rw-r--r--   0        0        0     3078 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc.yaml
--rw-r--r--   0        0        0     1077 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/role.yaml
--rw-r--r--   0        0        0      846 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/rolebinding.yaml
--rw-r--r--   0        0        0     5145 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/secrets.yaml
--rw-r--r--   0        0        0      837 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1963 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/tls-secrets.yaml
--rw-r--r--   0        0        0     4571 2023-08-27 04:24:41.017442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.schema.json
--rw-r--r--   0        0        0    80485 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.yaml
--rw-r--r--   0        0        0      351 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/.helmignore
--rw-r--r--   0        0        0      231 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.lock
--rw-r--r--   0        0        0      907 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.yaml
--rw-r--r--   0        0        0   105669 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/README.md
--rw-r--r--   0        0        0      360 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/.helmignore
--rw-r--r--   0        0        0      531 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/Chart.yaml
--rw-r--r--   0        0        0     7191 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/README.md
--rw-r--r--   0        0        0     5480 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     7044 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1494 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_compatibility.tpl
--rw-r--r--   0        0        0     1703 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     4071 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2431 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0     2147 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2497 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     1980 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_resources.tpl
--rw-r--r--   0        0        0     7908 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      698 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0     1385 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2599 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0     3449 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2644 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     4059 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4449 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     4003 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5091 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3334 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2526 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      182 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/values.yaml
--rw-r--r--   0        0        0     7342 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/NOTES.txt
--rw-r--r--   0        0        0    12599 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/_helpers.tpl
--rw-r--r--   0        0        0     1055 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/config-secret.yaml
--rw-r--r--   0        0        0      189 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/extra-list.yaml
--rw-r--r--   0        0        0     1875 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress-tls-secrets.yaml
--rw-r--r--   0        0        0     3265 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress.yaml
--rw-r--r--   0        0        0      693 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/init-configmap.yaml
--rw-r--r--   0        0        0     3812 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/networkpolicy.yaml
--rw-r--r--   0        0        0     1090 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/pdb.yaml
--rw-r--r--   0        0        0     1114 2024-03-07 06:21:41.688065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/prometheusrule.yaml
--rw-r--r--   0        0        0      776 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/role.yaml
--rw-r--r--   0        0        0      870 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/rolebinding.yaml
--rw-r--r--   0        0        0     2809 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/secrets.yaml
--rw-r--r--   0        0        0      908 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     3142 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    25075 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/statefulset.yaml
--rw-r--r--   0        0        0     1966 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc-headless.yaml
--rw-r--r--   0        0        0     5530 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc.yaml
--rw-r--r--   0        0        0     2021 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/tls-secrets.yaml
--rw-r--r--   0        0        0      116 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/validation.yaml
--rw-r--r--   0        0        0     2815 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.schema.json
--rw-r--r--   0        0        0    65942 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.yaml
--rw-r--r--   0        0        0      366 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/.helmignore
--rw-r--r--   0        0        0      293 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.lock
--rw-r--r--   0        0        0     1158 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.yaml
--rw-r--r--   0        0        0    11357 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/LICENSE
--rw-r--r--   0        0        0    61366 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/README.md
--rw-r--r--   0        0        0      366 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/.helmignore
--rw-r--r--   0        0        0      837 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/Chart.yaml
--rw-r--r--   0        0        0    11357 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/LICENSE
--rw-r--r--   0        0        0    24858 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/README.md
--rw-r--r--   0        0        0     1197 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/01-default-values.yaml
--rw-r--r--   0        0        0     1177 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/02-broker-tls-values.yaml
--rw-r--r--   0        0        0     3898 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/_helpers.tpl
--rw-r--r--   0        0        0    13014 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/deployment.yaml
--rw-r--r--   0        0        0     1432 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/pod-monitor.yaml
--rw-r--r--   0        0        0     1535 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/service.yaml
--rw-r--r--   0        0        0     1160 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     8687 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/tests/01-mm2-values.yaml
--rw-r--r--   0        0        0    12366 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/values.yaml
--rw-r--r--   0        0        0      366 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/.helmignore
--rw-r--r--   0        0        0      728 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/Chart.yaml
--rw-r--r--   0        0        0    13250 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/README.md
--rw-r--r--   0        0        0     3112 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/examples/console-enterprise.yaml
--rw-r--r--   0        0        0     2511 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/NOTES.txt
--rw-r--r--   0        0        0     3199 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/_helpers.tpl
--rw-r--r--   0        0        0     1379 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/configmap.yaml
--rw-r--r--   0        0        0    12390 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/deployment.yaml
--rw-r--r--   0        0        0     1755 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/hpa.yaml
--rw-r--r--   0        0        0     2897 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/ingress.yaml
--rw-r--r--   0        0        0     3615 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/secret.yaml
--rw-r--r--   0        0        0     1406 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/service.yaml
--rw-r--r--   0        0        0     1084 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      570 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0     6149 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.schema.json
--rw-r--r--   0        0        0     7718 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.yaml
--rw-r--r--   0        0        0      832 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/01-default-values.yaml
--rw-r--r--   0        0        0     1258 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/02-one-node-cluster-no-tls-no-sasl-values.yaml
--rw-r--r--   0        0        0     1012 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/03-one-node-cluster-tls-no-sasl-values.yaml
--rw-r--r--   0        0        0     1135 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/04-one-node-cluster-no-tls-sasl-values.yaml
--rw-r--r--   0        0        0     1281 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/05-one-node-cluster-tls-sasl-values.yaml
--rw-r--r--   0        0        0      868 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/06-rack-awareness-values.yaml
--rw-r--r--   0        0        0     1850 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/07-multiple-listeners-values.yaml
--rw-r--r--   0        0        0     1099 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/08-custom-podantiaffinity-values.yaml
--rw-r--r--   0        0        0     2081 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/09-initcontainers-resources-values.yaml
--rw-r--r--   0        0        0     1095 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/10-external-addresses-values.yaml
--rw-r--r--   0        0        0     1293 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/11-update-sasl-users-values.yaml
--rw-r--r--   0        0        0     2608 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/12-external-cert-secrets-values.yaml
--rw-r--r--   0        0        0     1124 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/13-loadbalancer-tls-values.yaml
--rw-r--r--   0        0        0      835 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/14-prometheus-no-tls-values.yaml
--rw-r--r--   0        0        0      834 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/15-prometheus-tls-values.yaml
--rw-r--r--   0        0        0      869 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/16-controller-sidecar-values.yaml
--rw-r--r--   0        0        0      944 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/17-resources-without-unit-values.yaml
--rw-r--r--   0        0        0     1049 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/18-single-external-address-values.yaml
--rw-r--r--   0        0        0     1513 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/21-eks-tiered-storage-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1702 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/22-gke-tiered-storage-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1745 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/23-aks-tiered-storage-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1545 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/24-eks-tiered-storage-persistent-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1734 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/25-gke-tiered-storage-persistent-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1777 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/26-aks-tiered-storage-persistent-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1603 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/27-eks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1792 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/28-gke-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1815 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/29-aks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
--rw-r--r--   0        0        0     1308 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/96-audit-logging-values.yaml.tpl
--rw-r--r--   0        0        0     1131 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/97-license-key-values.yaml.tpl
--rw-r--r--   0        0        0     1166 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/98-license-secret-values.yaml
--rw-r--r--   0        0        0     2363 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/99-none-existent-config-options-with-empty-values.yaml
--rw-r--r--   0        0        0     4551 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/NOTES.txt
--rw-r--r--   0        0        0    31567 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_configmap.tpl
--rw-r--r--   0        0        0     1893 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_example-commands.tpl
--rw-r--r--   0        0        0    36976 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_helpers.tpl
--rw-r--r--   0        0        0     1472 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_job.tpl
--rw-r--r--   0        0        0     5041 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_statefulset.tpl
--rw-r--r--   0        0        0     1118 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2784 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/cert-issuers.yaml
--rw-r--r--   0        0        0     4010 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/certs.yaml
--rw-r--r--   0        0        0     1366 2024-03-07 06:21:41.692065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/configmap.yaml
--rw-r--r--   0        0        0     4825 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/connectors/connectors.yaml
--rw-r--r--   0        0        0    12686 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/console/configmap-and-deployment.yaml
--rw-r--r--   0        0        0     1647 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/poddisruptionbudget.yaml
--rw-r--r--   0        0        0     5811 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-install-upgrade-job.yaml
--rw-r--r--   0        0        0     5551 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-upgrade.yaml
--rw-r--r--   0        0        0     5778 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/rbac.yaml
--rw-r--r--   0        0        0    15622 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/secrets.yaml
--rw-r--r--   0        0        0     1776 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.internal.yaml
--rw-r--r--   0        0        0     4130 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.loadbalancer.yaml
--rw-r--r--   0        0        0     1150 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1936 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/servicemonitor.yaml
--rw-r--r--   0        0        0     2874 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/services.nodeport.yaml
--rw-r--r--   0        0        0    23322 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/statefulset.yaml
--rw-r--r--   0        0        0     2059 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-api-status.yaml
--rw-r--r--   0        0        0     4090 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-auditLogging.yaml
--rw-r--r--   0        0        0     8436 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-connector-via-console.yaml
--rw-r--r--   0        0        0     1988 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-console.yaml
--rw-r--r--   0        0        0     5105 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-internal-external-tls-secrets.yaml
--rw-r--r--   0        0        0     2589 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-internal-tls-status.yaml
--rw-r--r--   0        0        0     4608 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-nodelete.yaml
--rw-r--r--   0        0        0     4010 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-produce-consume.yaml
--rw-r--r--   0        0        0     3144 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-sasl-status.yaml
--rw-r--r--   0        0        0     3036 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-license-with-console.yaml
--rw-r--r--   0        0        0     2620 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-lifecycle-scripts.yaml
--rw-r--r--   0        0        0     6188 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-loadbalancer-tls.yaml
--rw-r--r--   0        0        0     6207 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-nodeport-tls.yaml
--rw-r--r--   0        0        0     3906 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-internal-tls-status.yaml
--rw-r--r--   0        0        0     3338 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-status.yaml
--rw-r--r--   0        0        0     3442 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-prometheus-targets.yaml
--rw-r--r--   0        0        0     2619 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rack-awareness.yaml
--rw-r--r--   0        0        0     3938 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rpk-debug-bundle.yaml
--rw-r--r--   0        0        0     2996 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-sasl-updated.yaml
--rw-r--r--   0        0        0     8953 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-internal-tls-status.yaml
--rw-r--r--   0        0        0     9070 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-status.yaml
--rw-r--r--   0        0        0    44082 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.schema.json
--rw-r--r--   0        0        0    62802 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.yaml
--rw-r--r--   0        0        0      633 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.lock
--rw-r--r--   0        0        0     1335 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.yaml
--rw-r--r--   0        0        0    32538 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/README.md
--rw-r--r--   0        0        0      816 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/Chart.yaml
--rw-r--r--   0        0        0    17134 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/README.md
--rw-r--r--   0        0        0      593 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/NOTES.txt
--rw-r--r--   0        0        0     5361 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/_helpers.tpl
--rw-r--r--   0        0        0     3837 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-deployment.yaml
--rw-r--r--   0        0        0      634 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrole.yaml
--rw-r--r--   0        0        0      760 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1440 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp.yaml
--rw-r--r--   0        0        0     3748 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-rbac.yaml
--rw-r--r--   0        0        0      949 2023-08-27 04:24:41.021442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-serviceaccount.yaml
--rw-r--r--   0        0        0   374997 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/crds.yaml
--rw-r--r--   0        0        0     5687 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/deployment.yaml
--rw-r--r--   0        0        0      594 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrole.yaml
--rw-r--r--   0        0        0      722 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1398 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp.yaml
--rw-r--r--   0        0        0    19514 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/rbac.yaml
--rw-r--r--   0        0        0      972 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/service.yaml
--rw-r--r--   0        0        0      863 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1591 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/servicemonitor.yaml
--rw-r--r--   0        0        0     2845 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-job.yaml
--rw-r--r--   0        0        0      779 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrole.yaml
--rw-r--r--   0        0        0      910 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1520 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp.yaml
--rw-r--r--   0        0        0     1642 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-rbac.yaml
--rw-r--r--   0        0        0      994 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-serviceaccount.yaml
--rw-r--r--   0        0        0      746 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-config.yaml
--rw-r--r--   0        0        0     6309 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-deployment.yaml
--rw-r--r--   0        0        0     1657 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-mutating-webhook.yaml
--rw-r--r--   0        0        0      572 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrole.yaml
--rw-r--r--   0        0        0      694 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1558 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp.yaml
--rw-r--r--   0        0        0     2641 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-rbac.yaml
--rw-r--r--   0        0        0      954 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-service.yaml
--rw-r--r--   0        0        0      877 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-serviceaccount.yaml
--rw-r--r--   0        0        0     1874 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-validating-webhook.yaml
--rw-r--r--   0        0        0    17877 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/values.yaml
--rw-r--r--   0        0        0      349 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/.helmignore
--rw-r--r--   0        0        0      234 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.lock
--rw-r--r--   0        0        0      614 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.yaml
--rw-r--r--   0        0        0      839 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/README.md
--rw-r--r--   0        0        0      333 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/.helmignore
--rw-r--r--   0        0        0      225 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.lock
--rw-r--r--   0        0        0      673 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.yaml
--rw-r--r--   0        0        0    60071 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/README.md
--rw-r--r--   0        0        0      342 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/.helmignore
--rw-r--r--   0        0        0      529 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/Chart.yaml
--rw-r--r--   0        0        0     7114 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/README.md
--rw-r--r--   0        0        0     3723 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     5472 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2587 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2361 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2427 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     7323 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2064 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/values.yaml
--rw-r--r--   0        0        0     3774 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/NOTES.txt
--rw-r--r--   0        0        0    12157 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/_helpers.tpl
--rw-r--r--   0        0        0      726 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/configmap.yaml
--rw-r--r--   0        0        0      117 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/extra-list.yaml
--rw-r--r--   0        0        0     1180 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/metrics-svc.yaml
--rw-r--r--   0        0        0     1606 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/networkpolicy.yaml
--rw-r--r--   0        0        0     1096 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/pdb.yaml
--rw-r--r--   0        0        0     1211 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     5313 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/scripts-configmap.yaml
--rw-r--r--   0        0        0     4077 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/secrets.yaml
--rw-r--r--   0        0        0      944 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2516 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    28701 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/statefulset.yaml
--rw-r--r--   0        0        0     1747 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc-headless.yaml
--rw-r--r--   0        0        0     3297 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc.yaml
--rw-r--r--   0        0        0     3656 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/tls-secrets.yaml
--rw-r--r--   0        0        0    36148 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/values.yaml
--rw-r--r--   0        0        0    77365 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallations.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    77423 2023-08-27 04:24:41.025442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallationtemplates.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    20500 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseoperatorconfigurations.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    10595 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/_helper.tpl
--rw-r--r--   0        0        0    10878 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/clickhouse-instance.yaml
--rw-r--r--   0        0        0      924 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/configmap.yaml
--rw-r--r--   0        0        0      421 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/serviceaccount.yaml
--rw-r--r--   0        0        0      664 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/storage-class.yaml
--rw-r--r--   0        0        0      333 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-confd-files.yaml
--rw-r--r--   0        0        0     8493 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-configd-files.yaml
--rw-r--r--   0        0        0    11736 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-files.yaml
--rw-r--r--   0        0        0     2694 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-templatesd-files.yaml
--rw-r--r--   0        0        0     1681 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-usersd-files.yaml
--rw-r--r--   0        0        0     5371 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/deployment.yaml
--rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/namespace.yaml
--rw-r--r--   0        0        0     2638 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/role.yaml
--rw-r--r--   0        0        0      701 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/rolebinding.yaml
--rw-r--r--   0        0        0      419 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/secret.yaml
--rw-r--r--   0        0        0      600 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/service.yaml
--rw-r--r--   0        0        0      482 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/serviceaccount.yaml
--rw-r--r--   0        0        0    20429 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/values.yaml
--rw-r--r--   0        0        0      342 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/.helmignore
--rw-r--r--   0        0        0    24586 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/CHANGELOG.md
--rw-r--r--   0        0        0     1007 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/Chart.yaml
--rw-r--r--   0        0        0      213 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/OWNERS
--rw-r--r--   0        0        0    36385 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md
--rw-r--r--   0        0        0    10571 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md.gotmpl
--rw-r--r--   0        0        0      171 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/controller-custom-ingressclass-flags.yaml
--rw-r--r--   0        0        0      267 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customconfig-values.yaml
--rw-r--r--   0        0        0      337 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customnodeport-values.yaml
--rw-r--r--   0        0        0      198 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-extra-modules.yaml
--rw-r--r--   0        0        0      280 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-headers-values.yaml
--rw-r--r--   0        0        0      315 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-internal-lb-values.yaml
--rw-r--r--   0        0        0      191 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-nodeport-values.yaml
--rw-r--r--   0        0        0      368 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-podannotations-values.yaml
--rw-r--r--   0        0        0      338 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-configMapNamespace-values.yaml
--rw-r--r--   0        0        0      284 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-portNamePrefix-values.yaml
--rw-r--r--   0        0        0      260 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-values.yaml
--rw-r--r--   0        0        0      254 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-values.yaml
--rw-r--r--   0        0        0      192 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-default-values.yaml
--rw-r--r--   0        0        0      221 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-metrics-values.yaml
--rw-r--r--   0        0        0      228 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-psp-values.yaml
--rw-r--r--   0        0        0      227 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-and-psp-values.yaml
--rw-r--r--   0        0        0      191 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-values.yaml
--rw-r--r--   0        0        0      274 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-behavior-values.yaml
--rw-r--r--   0        0        0      207 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-values.yaml
--rw-r--r--   0        0        0      248 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customconfig-values.yaml
--rw-r--r--   0        0        0      318 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customnodeport-values.yaml
--rw-r--r--   0        0        0      170 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-default-values.yaml
--rw-r--r--   0        0        0      197 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-extra-modules.yaml
--rw-r--r--   0        0        0      262 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-headers-values.yaml
--rw-r--r--   0        0        0      297 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-internal-lb-values.yaml
--rw-r--r--   0        0        0      203 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-metrics-values.yaml
--rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-nodeport-values.yaml
--rw-r--r--   0        0        0      350 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-podannotations-values.yaml
--rw-r--r--   0        0        0      170 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-psp-values.yaml
--rw-r--r--   0        0        0      320 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-configMapNamespace-values.yaml
--rw-r--r--   0        0        0      266 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-portNamePrefix-values.yaml
--rw-r--r--   0        0        0      242 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-values.yaml
--rw-r--r--   0        0        0      196 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-values.yaml
--rw-r--r--   0        0        0      209 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-and-psp-values.yaml
--rw-r--r--   0        0        0      204 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-extraEnvs-values.yaml
--rw-r--r--   0        0        0      425 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-resources-values.yaml
--rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-values.yaml
--rw-r--r--   0        0        0     3498 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/NOTES.txt
--rw-r--r--   0        0        0     5570 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_helpers.tpl
--rw-r--r--   0        0        0     2996 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_params.tpl
--rw-r--r--   0        0        0     1120 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrole.yaml
--rw-r--r--   0        0        0      913 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrolebinding.yaml
--rw-r--r--   0        0        0     3740 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-createSecret.yaml
--rw-r--r--   0        0        0     3783 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-patchWebhook.yaml
--rw-r--r--   0        0        0     1183 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/psp.yaml
--rw-r--r--   0        0        0      769 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/role.yaml
--rw-r--r--   0        0        0      936 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/rolebinding.yaml
--rw-r--r--   0        0        0      650 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/serviceaccount.yaml
--rw-r--r--   0        0        0     1937 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/validating-webhook.yaml
--rw-r--r--   0        0        0     1949 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrole.yaml
--rw-r--r--   0        0        0      612 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0      459 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-addheaders.yaml
--rw-r--r--   0        0        0      693 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-proxyheaders.yaml
--rw-r--r--   0        0        0      547 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-tcp.yaml
--rw-r--r--   0        0        0      547 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-udp.yaml
--rw-r--r--   0        0        0     1162 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap.yaml
--rw-r--r--   0        0        0     9624 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-daemonset.yaml
--rw-r--r--   0        0        0     9990 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-deployment.yaml
--rw-r--r--   0        0        0     1620 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-hpa.yaml
--rw-r--r--   0        0        0      760 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-ingressclass.yaml
--rw-r--r--   0        0        0     1619 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-keda.yaml
--rw-r--r--   0        0        0      877 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-poddisruptionbudget.yaml
--rw-r--r--   0        0        0      961 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-prometheusrules.yaml
--rw-r--r--   0        0        0     2572 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-psp.yaml
--rw-r--r--   0        0        0     2463 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-role.yaml
--rw-r--r--   0        0        0      651 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-rolebinding.yaml
--rw-r--r--   0        0        0     3570 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-internal.yaml
--rw-r--r--   0        0        0     2106 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-metrics.yaml
--rw-r--r--   0        0        0     1670 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-webhook.yaml
--rw-r--r--   0        0        0     4504 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service.yaml
--rw-r--r--   0        0        0      623 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-serviceaccount.yaml
--rw-r--r--   0        0        0     2061 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-servicemonitor.yaml
--rw-r--r--   0        0        0      464 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-wehbooks-networkpolicy.yaml
--rw-r--r--   0        0        0     5476 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-deployment.yaml
--rw-r--r--   0        0        0     1143 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-hpa.yaml
--rw-r--r--   0        0        0      864 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-poddisruptionbudget.yaml
--rw-r--r--   0        0        0      925 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-psp.yaml
--rw-r--r--   0        0        0      806 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-role.yaml
--rw-r--r--   0        0        0      760 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-rolebinding.yaml
--rw-r--r--   0        0        0     1562 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-service.yaml
--rw-r--r--   0        0        0      573 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-serviceaccount.yaml
--rw-r--r--   0        0        0      233 2023-08-27 04:24:41.029442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/dh-param-secret.yaml
--rw-r--r--   0        0        0    31188 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/values.yaml
--rw-r--r--   0        0        0      349 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/.helmignore
--rw-r--r--   0        0        0      556 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/Chart.yaml
--rw-r--r--   0        0        0      276 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/NOTES.txt
--rw-r--r--   0        0        0    17762 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_config.tpl
--rw-r--r--   0        0        0    12793 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_helpers.tpl
--rw-r--r--   0        0        0      442 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/apikey-secret.yaml
--rw-r--r--   0        0        0      172 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/namespace.yaml
--rw-r--r--   0        0        0      448 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrole.yaml
--rw-r--r--   0        0        0      540 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrolebinding.yaml
--rw-r--r--   0        0        0      334 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/configmap.yaml
--rw-r--r--   0        0        0     6500 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/daemonset.yaml
--rw-r--r--   0        0        0     1763 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/ingress.yaml
--rw-r--r--   0        0        0      565 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/service.yaml
--rw-r--r--   0        0        0      471 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/serviceaccount.yaml
--rw-r--r--   0        0        0      513 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/tests/test-connection.yaml
--rw-r--r--   0        0        0      473 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrole.yaml
--rw-r--r--   0        0        0      564 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrolebinding.yaml
--rw-r--r--   0        0        0      359 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/configmap.yaml
--rw-r--r--   0        0        0     5859 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/deployment.yaml
--rw-r--r--   0        0        0     1813 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/ingress.yaml
--rw-r--r--   0        0        0      590 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/service.yaml
--rw-r--r--   0        0        0      501 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/serviceaccount.yaml
--rw-r--r--   0        0        0      599 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/tests/test-connection.yaml
--rw-r--r--   0        0        0      577 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/tls-secret.yaml
--rw-r--r--   0        0        0    28367 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/values.yaml
--rw-r--r--   0        0        0      305 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.lock
--rw-r--r--   0        0        0      872 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.yaml
--rw-r--r--   0        0        0    51454 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/README.md
--rw-r--r--   0        0        0      342 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/.helmignore
--rw-r--r--   0        0        0      569 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/Chart.yaml
--rw-r--r--   0        0        0    25039 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/README.md
--rw-r--r--   0        0        0     3502 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2437 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2314 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2461 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     6183 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2049 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/values.yaml
--rw-r--r--   0        0        0      333 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/.helmignore
--rw-r--r--   0        0        0      219 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.lock
--rw-r--r--   0        0        0      845 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.yaml
--rw-r--r--   0        0        0   101381 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/README.md
--rw-r--r--   0        0        0      342 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/.helmignore
--rw-r--r--   0        0        0      569 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/Chart.yaml
--rw-r--r--   0        0        0    25039 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/README.md
--rw-r--r--   0        0        0     3502 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2437 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2314 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2461 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     6183 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2049 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/values.yaml
--rw-r--r--   0        0        0     5433 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/NOTES.txt
--rw-r--r--   0        0        0    13838 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/_helpers.tpl
--rw-r--r--   0        0        0      117 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/extra-list.yaml
--rw-r--r--   0        0        0     1341 2023-08-27 04:24:41.033442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/networkpolicy-egress.yaml
--rw-r--r--   0        0        0     1072 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/configmap.yaml
--rw-r--r--   0        0        0      842 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/extended-configmap.yaml
--rw-r--r--   0        0        0      782 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/initialization-configmap.yaml
--rw-r--r--   0        0        0      717 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-configmap.yaml
--rw-r--r--   0        0        0     1269 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-svc.yaml
--rw-r--r--   0        0        0     3347 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/networkpolicy.yaml
--rw-r--r--   0        0        0     2390 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/servicemonitor.yaml
--rw-r--r--   0        0        0    34437 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/statefulset.yaml
--rw-r--r--   0        0        0     1452 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc-headless.yaml
--rw-r--r--   0        0        0     2721 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc.yaml
--rw-r--r--   0        0        0     1126 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1162 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/psp.yaml
--rw-r--r--   0        0        0      853 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/extended-configmap.yaml
--rw-r--r--   0        0        0      761 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-configmap.yaml
--rw-r--r--   0        0        0     1319 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-svc.yaml
--rw-r--r--   0        0        0     2225 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/networkpolicy.yaml
--rw-r--r--   0        0        0     2444 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/servicemonitor.yaml
--rw-r--r--   0        0        0    29932 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/statefulset.yaml
--rw-r--r--   0        0        0     1520 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc-headless.yaml
--rw-r--r--   0        0        0     2919 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc.yaml
--rw-r--r--   0        0        0     1172 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/role.yaml
--rw-r--r--   0        0        0      873 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/rolebinding.yaml
--rw-r--r--   0        0        0     1769 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/secrets.yaml
--rw-r--r--   0        0        0      875 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1690 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/tls-secrets.yaml
--rw-r--r--   0        0        0     4571 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.schema.json
--rw-r--r--   0        0        0    63223 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.yaml
--rw-r--r--   0        0        0     5526 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/NOTES.txt
--rw-r--r--   0        0        0     9090 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/_helpers.tpl
--rw-r--r--   0        0        0     1947 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap-env-vars.yaml
--rw-r--r--   0        0        0      743 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap.yaml
--rw-r--r--   0        0        0      117 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/extra-list.yaml
--rw-r--r--   0        0        0     1160 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/headless-service.yaml
--rw-r--r--   0        0        0     1858 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/hpa.yaml
--rw-r--r--   0        0        0     3152 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/ingress.yaml
--rw-r--r--   0        0        0      802 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/init-scripts-configmap.yaml
--rw-r--r--   0        0        0      850 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-configmap.yaml
--rw-r--r--   0        0        0     7172 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-job.yaml
--rw-r--r--   0        0        0     1228 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/metrics-service.yaml
--rw-r--r--   0        0        0     1498 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/networkpolicy.yaml
--rw-r--r--   0        0        0     1023 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/pdb.yaml
--rw-r--r--   0        0        0     1129 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/prometheusrule.yaml
--rw-r--r--   0        0        0      950 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/role.yaml
--rw-r--r--   0        0        0      974 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/rolebinding.yaml
--rw-r--r--   0        0        0     1982 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/secrets.yaml
--rw-r--r--   0        0        0     3171 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/service.yaml
--rw-r--r--   0        0        0     1019 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2655 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    20259 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/statefulset.yaml
--rw-r--r--   0        0        0     3273 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/tls-secret.yaml
--rw-r--r--   0        0        0    40146 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/values.yaml
--rw-r--r--   0        0        0      368 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/.helmignore
--rw-r--r--   0        0        0      359 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/Chart.yaml
--rw-r--r--   0        0        0     9349 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/README.md
--rw-r--r--   0        0        0     2668 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/NOTES.txt
--rw-r--r--   0        0        0     3022 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_bucket.txt
--rw-r--r--   0        0        0     2010 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_policy.txt
--rw-r--r--   0        0        0     3087 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_user.txt
--rw-r--r--   0        0        0     1473 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_custom_command.txt
--rw-r--r--   0        0        0      469 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_policy.tpl
--rw-r--r--   0        0        0     6479 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helpers.tpl
--rw-r--r--   0        0        0      887 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/configmap.yaml
--rw-r--r--   0        0        0     1693 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-ingress.yaml
--rw-r--r--   0        0        0     1558 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-service.yaml
--rw-r--r--   0        0        0     6682 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/deployment.yaml
--rw-r--r--   0        0        0     6449 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/gateway-deployment.yaml
--rw-r--r--   0        0        0     1594 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/ingress.yaml
--rw-r--r--   0        0        0      812 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/networkpolicy.yaml
--rw-r--r--   0        0        0      371 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/poddisruptionbudget.yaml
--rw-r--r--   0        0        0     3130 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-bucket-job.yaml
--rw-r--r--   0        0        0     3135 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-policy-job.yaml
--rw-r--r--   0        0        0     3460 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-user-job.yaml
--rw-r--r--   0        0        0     3190 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-custom-command.yaml
--rw-r--r--   0        0        0     1059 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/pvc.yaml
--rw-r--r--   0        0        0      752 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/secrets.yaml
--rw-r--r--   0        0        0     1117 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/securitycontextconstraints.yaml
--rw-r--r--   0        0        0     1457 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/service.yaml
--rw-r--r--   0        0        0      195 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2036 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/servicemonitor.yaml
--rw-r--r--   0        0        0     8507 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/statefulset.yaml
--rw-r--r--   0        0        0    13974 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/values.yaml
--rw-r--r--   0        0        0     2317 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/NOTES.txt
--rw-r--r--   0        0        0     8852 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_clickhouse.tpl
--rw-r--r--   0        0        0    23248 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_helpers.tpl
--rw-r--r--   0        0        0      460 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/configmap.yaml
--rw-r--r--   0        0        0     1716 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/ingress.yaml
--rw-r--r--   0        0        0      434 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/pdb.yaml
--rw-r--r--   0        0        0      432 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/serviceaccount.yaml
--rw-r--r--   0        0        0     1455 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/services.yaml
--rw-r--r--   0        0        0     8128 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/statefulset.yaml
--rw-r--r--   0        0        0      974 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/cert-issuer.yaml
--rw-r--r--   0        0        0     1792 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/configmap.yaml
--rw-r--r--   0        0        0     3589 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/deployment.yaml
--rw-r--r--   0        0        0     1311 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/hpa.yaml
--rw-r--r--   0        0        0     1647 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/ingress.yaml
--rw-r--r--   0        0        0     1016 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/keda-autoscaler.yaml
--rw-r--r--   0        0        0      542 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/service.yaml
--rw-r--r--   0        0        0      384 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/serviceaccount.yaml
--rw-r--r--   0        0        0      459 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/tests/test-connection.yaml
--rw-r--r--   0        0        0      429 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrole.yaml
--rw-r--r--   0        0        0      519 2023-08-27 04:24:41.037442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrolebinding.yaml
--rw-r--r--   0        0        0      375 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/configmap.yaml
--rw-r--r--   0        0        0     8408 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/deployment.yaml
--rw-r--r--   0        0        0     1361 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/hpa.yaml
--rw-r--r--   0        0        0     1692 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/ingress.yaml
--rw-r--r--   0        0        0     1061 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/keda-autoscaler.yaml
--rw-r--r--   0        0        0      487 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/service.yaml
--rw-r--r--   0        0        0      404 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/serviceaccount.yaml
--rw-r--r--   0        0        0      523 2024-03-07 06:21:41.696065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrole.yaml
--rw-r--r--   0        0        0      759 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrolebinding.yaml
--rw-r--r--   0        0        0      341 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/configmap.yaml
--rw-r--r--   0        0        0     8528 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/deployment.yaml
--rw-r--r--   0        0        0     1795 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/ingress.yaml
--rw-r--r--   0        0        0      577 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/service.yaml
--rw-r--r--   0        0        0      472 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/serviceaccount.yaml
--rw-r--r--   0        0        0     1111 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/configmap.yaml
--rw-r--r--   0        0        0     1683 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/ingress.yaml
--rw-r--r--   0        0        0     1204 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/service.yaml
--rw-r--r--   0        0        0      400 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/serviceaccount.yaml
--rw-r--r--   0        0        0     9499 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/statefulset.yaml
--rw-r--r--   0        0        0      546 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/tests/test-connection.yaml
--rw-r--r--   0        0        0     3044 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-init.yaml
--rw-r--r--   0        0        0     3088 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-upgrade.yaml
--rw-r--r--   0        0        0      273 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/secrets-clickhouse-external.yaml
--rw-r--r--   0        0        0    92137 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/values.yaml
--rw-r--r--   0        0        0      972 2024-03-10 01:37:07.461164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_postgresql_helper.py
--rw-r--r--   0        0        0      755 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_rabbitmq_helper.py
--rw-r--r--   0        0        0     1052 2024-03-10 01:37:07.469164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_redpanda_helper.py
--rw-r--r--   0        0        0      904 2024-03-10 01:37:07.481164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_signoz_helper.py
--rw-r--r--   0        0        0       86 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0      556 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/template.env
--rw-r--r--   0        0        0      330 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose-app.env
--rw-r--r--   0        0        0     1238 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.env
--rw-r--r--   0        0        0    15205 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.yml
--rw-r--r--   0        0        0       68 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/README.md
--rw-r--r--   0        0        0     6411 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/README.md
--rw-r--r--   0        0        0    81204 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-microservices.png
--rw-r--r--   0        0        0    41834 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-monolith.png
--rw-r--r--   0        0        0    40600 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp.png
--rw-r--r--   0        0        0       17 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/.gitignore
--rw-r--r--   0        0        0      870 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/locustfile.py
--rw-r--r--   0        0        0      495 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/pyproject.toml
--rw-r--r--   0        0        0      107 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/template.env
--rw-r--r--   0        0        0     2870 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-cluster.xml
--rw-r--r--   0        0        0    55854 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-config.xml
--rw-r--r--   0        0        0     1754 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-storage.xml
--rw-r--r--   0        0        0     6258 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-users.xml
--rw-r--r--   0        0        0      575 2023-08-27 04:24:41.041442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/custom-function.xml
--rwxr-xr-x   0        0        0  1849156 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile
--rw-r--r--   0        0        0     6986 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile.go
--rw-r--r--   0        0        0     1475 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/frontend/nginx-config.conf
--rw-r--r--   0        0        0     5284 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector/otel-collector-config.yaml
--rw-r--r--   0        0        0     1548 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector-metrics/otel-collector-metrics-config.yaml
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/dashboards/.gitkeep
--rw-r--r--   0        0        0        9 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/data/.gitignore
--rw-r--r--   0        0        0      757 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/prometheus.yml
--rw-r--r--   0        0        0      135 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.dockerignore
--rw-r--r--   0        0        0       53 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.gitignore
--rw-r--r--   0        0        0        7 2023-10-17 11:37:32.073861 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.python-version
--rw-r--r--   0        0        0      555 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/Dockerfile
--rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/__init__.py
--rw-r--r--   0        0        0     1949 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/error.py
--rwxr-xr-x   0        0        0      801 2024-03-10 01:37:07.489164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/__init__.py
--rw-r--r--   0        0        0     6041 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/admin.py
--rwxr-xr-x   0        0        0    10820 2024-03-10 01:37:07.573164 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/consumer.py
--rwxr-xr-x   0        0        0     7090 2024-03-10 01:37:07.697165 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/publisher.py
--rwxr-xr-x   0        0        0     1731 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/messagebus.py
--rw-r--r--   0        0        0     1991 2024-03-10 01:37:07.721165 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/mock.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5121 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/admin.py
--rwxr-xr-x   0        0        0     6750 2024-03-10 01:37:07.781165 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/consumer.py
--rwxr-xr-x   0        0        0     4525 2024-03-10 01:37:07.821166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/publisher.py
--rw-r--r--   0        0        0       67 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/__init__.py
--rw-r--r--   0        0        0     1744 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/repo_model.py
--rw-r--r--   0        0        0      258 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/__init__.py
--rw-r--r--   0        0        0      538 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_entity_mixin.py
--rw-r--r--   0        0        0     9446 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_repo.py
--rw-r--r--   0        0        0      932 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/repo.py
--rw-r--r--   0        0        0      147 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/search_filter.py
--rw-r--r--   0        0        0      244 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/__init__.py
--rw-r--r--   0        0        0     3201 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/caller.py
--rw-r--r--   0        0        0     2197 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/server.py
--rw-r--r--   0        0        0     1625 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/rpc.py
--rw-r--r--   0        0        0      127 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/schema/__init__.py
--rw-r--r--   0        0        0      342 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/schema/base_schema.py
--rw-r--r--   0        0        0      154 2024-03-10 01:37:07.825166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/__init__.py
--rw-r--r--   0        0        0      854 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/serializer.py
--rwxr-xr-x   0        0        0     4380 2024-01-23 09:38:21.733760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/config.py
--rw-r--r--   0        0        0      160 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.eslintignore
--rw-r--r--   0        0        0      494 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      132 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.gitignore
--rw-r--r--   0        0        0       19 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.npmrc
--rw-r--r--   0        0        0      160 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.prettierignore
--rw-r--r--   0        0        0      233 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.prettierrc
--rwxr-xr-x   0        0        0      944 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/README.md
--rwxr-xr-x   0        0        0     1362 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/package.json
--rwxr-xr-x   0        0        0      225 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/playwright.config.ts
--rwxr-xr-x   0        0        0       80 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/postcss.config.js
--rwxr-xr-x   0        0        0       58 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.css
--rwxr-xr-x   0        0        0      241 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.d.ts
--rwxr-xr-x   0        0        0      350 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.html
--rwxr-xr-x   0        0        0      148 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/index.test.ts
--rwxr-xr-x   0        0        0   130279 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/assets/logo.png
--rwxr-xr-x   0        0        0     5281 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/helper.ts
--rwxr-xr-x   0        0        0      125 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/store.ts
--rwxr-xr-x   0        0        0      197 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/type.ts
--rw-r--r--   0        0        0      608 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectDiv.svelte
--rw-r--r--   0        0        0      361 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectUl.svelte
--rw-r--r--   0        0        0     1906 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/input/arrayOfObjectCheckboxes.svelte
--rw-r--r--   0        0        0      281 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/json/jsonView.svelte
--rwxr-xr-x   0        0        0     1675 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Menu.svelte
--rwxr-xr-x   0        0        0     4085 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Navigation.svelte
--rwxr-xr-x   0        0        0      727 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/helper.ts
--rwxr-xr-x   0        0        0      127 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/type.ts
--rwxr-xr-x   0        0        0     1609 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/app.ts
--rwxr-xr-x   0        0        0      648 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/navData.ts
--rwxr-xr-x   0        0        0      350 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/error/helper.ts
--rwxr-xr-x   0        0        0      291 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+error.svelte
--rwxr-xr-x   0        0        0       65 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.js
--rwxr-xr-x   0        0        0      584 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.svelte
--rwxr-xr-x   0        0        0      489 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+page.svelte
--rwxr-xr-x   0        0        0     6285 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/+page.svelte
--rwxr-xr-x   0        0        0     3763 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2968 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     4306 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/new/+page.svelte
--rw-r--r--   0        0        0     5028 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     6051 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/+page.svelte
--rwxr-xr-x   0        0        0     3462 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2662 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     2905 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/new/+page.svelte
--rw-r--r--   0        0        0     3659 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     6622 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/+page.svelte
--rwxr-xr-x   0        0        0     4323 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     3529 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     6049 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/new/+page.svelte
--rw-r--r--   0        0        0     6952 2023-08-27 04:24:41.053442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     5409 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/+page.svelte
--rwxr-xr-x   0        0        0     2941 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     1321 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/favicon.png
--rwxr-xr-x   0        0        0    12221 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/logo.png
--rwxr-xr-x   0        0        0      317 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/svelte.config.js
--rwxr-xr-x   0        0        0      203 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tailwind.config.js
--rwxr-xr-x   0        0        0      224 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tests/test.ts
--rwxr-xr-x   0        0        0      532 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tsconfig.json
--rwxr-xr-x   0        0        0      210 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/vite.config.ts
--rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/__init__.py
--rw-r--r--   0        0        0      490 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/async_task.py
--rwxr-xr-x   0        0        0      763 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/conversion.py
--rw-r--r--   0        0        0     1858 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/migration.py
--rw-r--r--   0        0        0      103 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/value.py
--rwxr-xr-x   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/__init__.py
--rwxr-xr-x   0        0        0     3177 2024-03-10 01:37:07.853166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app.py
--rw-r--r--   0        0        0     1389 2024-03-10 01:37:07.869166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_lifespan.py
--rw-r--r--   0        0        0      870 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_state.py
--rw-r--r--   0        0        0     1062 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/db_connection.py
--rw-r--r--   0        0        0      322 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/frontend_index.py
--rw-r--r--   0        0        0     1838 2024-03-10 01:37:07.881166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/log.py
--rw-r--r--   0        0        0     3460 2024-03-10 01:37:07.925166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/messagebus.py
--rw-r--r--   0        0        0     1410 2024-03-10 01:37:07.941166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/rpc.py
--rwxr-xr-x   0        0        0      280 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/main.py
--rw-r--r--   0        0        0      232 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/migrate.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/__init__.py
--rw-r--r--   0        0        0      978 2024-03-10 01:37:07.953167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/api.py
--rw-r--r--   0        0        0      907 2024-03-10 01:37:07.961166 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/_init_.py
--rw-r--r--   0        0        0     1204 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/scheme.py
--rw-r--r--   0        0        0     2124 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/util.py
--rw-r--r--   0        0        0      354 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/authorizer.py
--rw-r--r--   0        0        0     1178 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/rpc_authorizer.py
--rw-r--r--   0        0        0      446 2024-03-10 01:37:07.965167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/password_hasher/bcrypt_password_hasher.py
--rw-r--r--   0        0        0      258 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/password_hasher/password_hasher.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/_init_.py
--rw-r--r--   0        0        0     1674 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/util.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/__init__.py
--rw-r--r--   0        0        0     4203 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/api.py
--rw-r--r--   0        0        0      280 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/model.py
--rw-r--r--   0        0        0     1283 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/repo.py
--rw-r--r--   0        0        0     2331 2024-03-03 13:54:04.996858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/rpc.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/__init__.py
--rw-r--r--   0        0        0     4425 2024-03-10 01:37:08.009167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/api.py
--rw-r--r--   0        0        0      905 2024-03-10 01:37:08.021167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/model.py
--rw-r--r--   0        0        0     1134 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/repo.py
--rw-r--r--   0        0        0     2554 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/rpc.py
--rw-r--r--   0        0        0      661 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/table.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/__init__.py
--rw-r--r--   0        0        0     6543 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/api.py
--rw-r--r--   0        0        0     6582 2024-03-10 01:37:08.077167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/model.py
--rw-r--r--   0        0        0     3175 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/repo.py
--rw-r--r--   0        0        0     3612 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/rpc.py
--rw-r--r--   0        0        0      279 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/event.py
--rw-r--r--   0        0        0      777 2024-03-10 01:37:08.081167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/__init__.py
--rw-r--r--   0        0        0      570 2024-03-10 01:37:08.089167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_scheme.py
--rw-r--r--   0        0        0      560 2024-03-10 01:37:08.097167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_util.py
--rw-r--r--   0        0        0      316 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/authorizer.py
--rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/base.py
--rw-r--r--   0        0        0      155 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/bearer_token_scheme.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/__init__.py
--rw-r--r--   0        0        0      223 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/group_model.py
--rw-r--r--   0        0        0      263 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/permission_model.py
--rw-r--r--   0        0        0     1010 2024-03-10 01:37:08.105167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/user_model.py
--rw-r--r--   0        0        0      129 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/password_hasher.py
--rw-r--r--   0        0        0      568 2024-03-10 01:37:08.113167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/refresh_token_util.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/__init__.py
--rw-r--r--   0        0        0      212 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/group_repo.py
--rw-r--r--   0        0        0      242 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/permission_repo.py
--rw-r--r--   0        0        0      313 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/user_repo.py
--rw-r--r--   0        0        0      805 2024-03-10 01:37:08.121168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/user.py
--rw-r--r--   0        0        0      576 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/migrate.py
--rw-r--r--   0        0        0     1154 2024-03-10 01:37:08.133168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_module.py
--rw-r--r--   0        0        0     1322 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_permission.py
--rw-r--r--   0        0        0      711 2024-03-10 01:37:08.141167 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/rpc.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/__init__.py
--rw-r--r--   0        0        0      461 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/group.py
--rw-r--r--   0        0        0      337 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/permission.py
--rw-r--r--   0        0        0      190 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/request.py
--rw-r--r--   0        0        0      319 2024-01-23 09:38:21.737760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/token.py
--rw-r--r--   0        0        0      697 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/user.py
--rw-r--r--   0        0        0      518 2024-03-10 01:37:08.149168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/api.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/__init__.py
--rw-r--r--   0        0        0     1612 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/historical_repo_model.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/__init__.py
--rw-r--r--   0        0        0     2151 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/api.py
--rw-r--r--   0        0        0      611 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/event.py
--rw-r--r--   0        0        0      229 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/model.py
--rw-r--r--   0        0        0      621 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/repo.py
--rw-r--r--   0        0        0     2340 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/rpc.py
--rw-r--r--   0        0        0      552 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/table.py
--rw-r--r--   0        0        0      434 2024-03-10 01:37:08.153168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/event.py
--rw-r--r--   0        0        0       58 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/__init__.py
--rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/base.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/model/__init__.py
--rw-r--r--   0        0        0      189 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/model/activity_model.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/repo/__init__.py
--rw-r--r--   0        0        0      229 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/repo/activity_repo.py
--rw-r--r--   0        0        0      429 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/migrate.py
--rw-r--r--   0        0        0     1147 2024-03-10 01:37:08.165168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/register_module.py
--rw-r--r--   0        0        0      445 2024-03-10 01:37:08.169168 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/rpc.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/schema/__init__.py
--rw-r--r--   0        0        0      338 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/schema/activity.py
--rw-r--r--   0        0        0     1000 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/schema/__init__.py
--rw-r--r--   0        0        0      163 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/schema/frontend_config.py
--rwxr-xr-x   0        0        0     1721 2024-02-18 23:16:10.199317 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/start.sh
--rw-r--r--   0        0        0     1608 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/template.env
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/__init__.py
--rw-r--r--   0        0        0     7724 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_group_crud.py
--rw-r--r--   0        0        0     7782 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_permission_crud.py
--rw-r--r--   0        0        0     8005 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_crud.py
--rw-r--r--   0        0        0     8581 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_login.py
--rw-r--r--   0        0        0      314 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/conftest.py
--rw-r--r--   0        0        0      278 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/helper.py
--rw-r--r--   0        0        0     1232 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/test_liveness_and_readiness.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/__init__.py
--rw-r--r--   0        0        0     4870 2024-03-10 01:37:08.229168 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/add.py
--rw-r--r--   0        0        0     4057 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/helper.py
--rw-r--r--   0        0        0       13 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/.gitignore
--rw-r--r--   0        0        0    11259 2023-09-14 07:29:41.118392 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package-lock.json
--rw-r--r--   0        0        0      369 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package.json
--rw-r--r--   0        0        0     1460 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/addNav.ts
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/fastapp/src/frontend/src/lib/config/navData.ts
--rw-r--r--   0        0        0    12289 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/tsconfig.json
--rw-r--r--   0        0        0     1335 2024-03-10 01:37:08.241168 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/task_factory.py
--rwxr-xr-x   0        0        0     6304 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/+page.svelte
--rwxr-xr-x   0        0        0     3517 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2683 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     2911 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/new/+page.svelte
--rw-r--r--   0        0        0     3673 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.ts
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/__init__.py
--rw-r--r--   0        0        0     5305 2024-03-10 01:37:08.285168 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/api.py
--rw-r--r--   0        0        0      478 2024-03-10 01:37:08.289168 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/model.py
--rw-r--r--   0        0        0      780 2024-03-10 01:37:08.297168 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/repo.py
--rw-r--r--   0        0        0     2775 2024-03-10 01:37:08.325169 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/rpc.py
--rw-r--r--   0        0        0      403 2024-03-10 01:37:08.329169 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/model/snake_zrb_entity_name_model.py
--rw-r--r--   0        0        0      336 2024-03-10 01:37:08.333169 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/repo/snake_zrb_entity_name_repo.py
--rw-r--r--   0        0        0      378 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/schema/snake_zrb_entity_name.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/__init__.py
--rw-r--r--   0        0        0     8206 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/test_snake_zrb_entity_name.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_field/__init__.py
--rw-r--r--   0        0        0     6406 2024-03-10 01:37:08.381169 zrb-0.9.2/src/zrb/builtin/generator/fastapp_field/add.py
--rw-r--r--   0        0        0    11031 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/fastapp_field/helper.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/__init__.py
--rw-r--r--   0        0        0     4607 2024-03-10 01:37:08.421169 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/add.py
--rw-r--r--   0        0        0    10945 2024-03-10 01:37:08.525170 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/helper.py
--rw-r--r--   0        0        0      381 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/api.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/component/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/__init__.py
--rw-r--r--   0        0        0      570 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/table.py
--rw-r--r--   0        0        0      296 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/event.py
--rw-r--r--   0        0        0       76 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/__init__.py
--rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/base.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/model/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/repo/__init__.py
--rw-r--r--   0        0        0      537 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/migrate.py
--rw-r--r--   0        0        0     1273 2024-03-10 01:37:08.537170 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/register_module.py
--rw-r--r--   0        0        0      313 2024-03-03 13:54:05.000858 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/rpc.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/schema/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/pip_package/__init__.py
--rw-r--r--   0        0        0     3122 2024-03-10 01:37:08.561170 zrb-0.9.2/src/zrb/builtin/generator/pip_package/add.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/__init__.py
--rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/activate-venv.sh
--rw-r--r--   0        0        0       86 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/build.sh
--rw-r--r--   0        0        0       37 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/install-symlink.sh
--rw-r--r--   0        0        0       38 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/prepare-venv.sh
--rw-r--r--   0        0        0       80 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/publish.sh
--rw-r--r--   0        0        0     3131 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/local.py
--rw-r--r--   0        0        0        6 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/.gitignore
--rw-r--r--   0        0        0     1995 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/README.md
--rw-r--r--   0        0        0      764 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/pyproject.toml
--rw-r--r--   0        0        0       38 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/__init__.py
--rw-r--r--   0        0        0       38 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/__main__.py
--rw-r--r--   0        0        0       60 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/util.py
--rw-r--r--   0        0        0     2351 2024-03-10 01:37:08.581170 zrb-0.9.2/src/zrb/builtin/generator/plugin/create.py
--rw-r--r--   0        0        0     1076 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/.github/workflows/_zrb.yml
--rw-r--r--   0        0        0      218 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/.github/workflows/hello.yml
--rw-r--r--   0        0        0       32 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/.gitignore
--rw-r--r--   0        0        0        7 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/.python-version
--rw-r--r--   0        0        0     2051 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/README.md
--rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/_cmd/activate-venv.sh
--rw-r--r--   0        0        0       86 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/_cmd/build.sh
--rw-r--r--   0        0        0       37 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/_cmd/install-symlink.sh
--rw-r--r--   0        0        0       38 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/_cmd/prepare-venv.sh
--rw-r--r--   0        0        0       64 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/_cmd/publish.sh
--rwxr-xr-x   0        0        0     1938 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/project.sh
--rw-r--r--   0        0        0      763 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/pyproject.toml
--rw-r--r--   0        0        0      130 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/__init__.py
--rw-r--r--   0        0        0      121 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/__main__.py
--rw-r--r--   0        0        0      325 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/task/example_task.py
--rw-r--r--   0        0        0      118 2023-12-25 09:04:52.769412 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/template.env
--rw-r--r--   0        0        0     2459 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/plugin/template/zrb_init.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project/__init__.py
--rw-r--r--   0        0        0     3303 2024-03-10 01:37:08.613170 zrb-0.9.2/src/zrb/builtin/generator/project/create.py
--rw-r--r--   0        0        0       56 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project/template/.flake8
--rw-r--r--   0        0        0     1081 2023-10-18 00:29:25.312347 zrb-0.9.2/src/zrb/builtin/generator/project/template/.github/workflows/_zrb.yml
--rw-r--r--   0        0        0      218 2023-10-18 00:29:25.312347 zrb-0.9.2/src/zrb/builtin/generator/project/template/.github/workflows/hello.yml
--rw-r--r--   0        0        0       27 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project/template/.gitignore
--rw-r--r--   0        0        0        7 2023-10-12 00:54:12.983360 zrb-0.9.2/src/zrb/builtin/generator/project/template/.python-version
--rw-r--r--   0        0        0     2026 2023-12-08 01:44:50.345704 zrb-0.9.2/src/zrb/builtin/generator/project/template/README.md
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project/template/_automate/__init__.py
--rwxr-xr-x   0        0        0     1938 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/project/template/project.sh
--rw-r--r--   0        0        0      520 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/project/template/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project/template/src/.gitkeep
--rw-r--r--   0        0        0       64 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/project/template/template.env
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project/template/zrb_init.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/project_task/__init__.py
--rw-r--r--   0        0        0     6083 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/task_factory.py
--rw-r--r--   0        0        0      644 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/__init__.py
--rw-r--r--   0        0        0      322 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/build_project_images.py
--rw-r--r--   0        0        0      298 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/deploy_project.py
--rw-r--r--   0        0        0      312 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/destroy_project.py
--rw-r--r--   0        0        0      319 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/push_project_images.py
--rw-r--r--   0        0        0      342 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/remove_project_containers.py
--rw-r--r--   0        0        0      294 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project.py
--rw-r--r--   0        0        0      333 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project_containers.py
--rw-r--r--   0        0        0      334 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/stop_project_containers.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.2/src/zrb/builtin/generator/python_task/__init__.py
--rw-r--r--   0        0        0     1848 2024-03-10 01:37:08.629170 zrb-0.9.2/src/zrb/builtin/generator/python_task/add.py
--rw-r--r--   0        0        0      765 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/python_task/template/_automate/snake_zrb_task_name.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/__init__.py
--rw-r--r--   0        0        0     6515 2024-03-10 01:37:08.681171 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/add.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/__init__.py
--rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/_common.py
--rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/app-activate-venv.sh
--rw-r--r--   0        0        0      195 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/app-start.sh
--rw-r--r--   0        0        0       29 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
--rw-r--r--   0        0        0      126 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
--rw-r--r--   0        0        0       24 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
--rw-r--r--   0        0        0     4836 2024-03-10 01:37:08.733171 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/container.py
--rw-r--r--   0        0        0     3841 2024-03-10 01:37:08.761171 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/deployment.py
--rw-r--r--   0        0        0     2235 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/image.py
--rw-r--r--   0        0        0     1388 2024-03-10 01:37:08.777171 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/local.py
--rw-r--r--   0        0        0       31 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/.gitignore
--rw-r--r--   0        0        0       12 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      137 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0     2633 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/__main__.py
--rw-r--r--   0        0        0       74 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0        0 2023-08-28 15:53:50.913810 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/template.env
--rw-r--r--   0        0        0       68 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.env
--rw-r--r--   0        0        0      646 2023-10-12 00:54:12.983360 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.yml
--rw-r--r--   0        0        0       22 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/.dockerignore
--rw-r--r--   0        0        0       23 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/.gitignore
--rw-r--r--   0        0        0      274 2024-02-18 23:16:10.203317 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/Dockerfile
--rw-r--r--   0        0        0      511 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/main.py
--rw-r--r--   0        0        0      568 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/pyproject.toml
--rw-r--r--   0        0        0       87 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/template.env
--rw-r--r--   0        0        0     3016 2024-02-25 11:35:16.468626 zrb-0.9.2/src/zrb/builtin/git.py
--rw-r--r--   0        0        0     1168 2024-02-25 11:35:24.964664 zrb-0.9.2/src/zrb/builtin/group.py
--rw-r--r--   0        0        0        0 2023-12-03 01:12:52.544398 zrb-0.9.2/src/zrb/builtin/helper/__init__.py
--rw-r--r--   0        0        0     1940 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/helper/reccuring_action.py
--rw-r--r--   0        0        0     1235 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/md5.py
--rw-r--r--   0        0        0     1283 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/process.py
--rw-r--r--   0        0        0     1195 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/project.py
--rw-r--r--   0        0        0     3866 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/say.py
--rw-r--r--   0        0        0      989 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/schedule.py
--rw-r--r--   0        0        0     3087 2024-03-10 01:37:08.801171 zrb-0.9.2/src/zrb/builtin/ubuntu.py
--rw-r--r--   0        0        0      397 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/update.py
--rw-r--r--   0        0        0      478 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/version.py
--rw-r--r--   0        0        0     1191 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/builtin/watch_changes.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/config/__init__.py
--rw-r--r--   0        0        0     1170 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/config/config.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/__init__.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/accessories/__init__.py
--rw-r--r--   0        0        0      805 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/helper/accessories/color.py
--rw-r--r--   0        0        0      509 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/helper/accessories/icon.py
--rw-r--r--   0        0        0     2775 2024-01-23 09:38:21.741760 zrb-0.9.2/src/zrb/helper/accessories/name.py
--rw-r--r--   0        0        0      787 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/advertisement.py
--rw-r--r--   0        0        0      231 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/callable.py
--rw-r--r--   0        0        0     2050 2024-03-10 01:37:08.821171 zrb-0.9.2/src/zrb/helper/cli.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/codemod/__init__.py
--rw-r--r--   0        0        0     1252 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_argument_to_function.py
--rw-r--r--   0        0        0      998 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_argument_to_function_call.py
--rw-r--r--   0        0        0      825 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_assert_resource.py
--rw-r--r--   0        0        0     1036 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_function_call.py
--rw-r--r--   0        0        0     3220 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_import_module.py
--rw-r--r--   0        0        0     1583 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_key_value_to_dict.py
--rw-r--r--   0        0        0     2872 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_property_to_class.py
--rw-r--r--   0        0        0     3191 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/add_upstream_to_task.py
--rw-r--r--   0        0        0      933 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/append_code_to_function.py
--rw-r--r--   0        0        0      147 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/codemod/format_code.py
--rw-r--r--   0        0        0     2045 2024-03-10 01:36:55.389095 zrb-0.9.2/src/zrb/helper/default_env.py
--rw-r--r--   0        0        0     2046 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/docker_compose/fetch_external_env.py
--rw-r--r--   0        0        0      686 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/docker_compose/file.py
--rw-r--r--   0        0        0     4815 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/docstring.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/env_map/__init__.py
--rw-r--r--   0        0        0     2177 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/env_map/fetch.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/file/__init__.py
--rw-r--r--   0        0        0     1729 2024-03-10 01:36:55.389095 zrb-0.9.2/src/zrb/helper/file/copy_tree.py
--rw-r--r--   0        0        0      566 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/file/match.py
--rw-r--r--   0        0        0      809 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/file/text.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/git/__init__.py
--rw-r--r--   0        0        0     1150 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/git/detect_changes.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/loader/__init__.py
--rw-r--r--   0        0        0     1757 2024-03-10 01:36:55.389095 zrb-0.9.2/src/zrb/helper/loader/load_module.py
--rw-r--r--   0        0        0      517 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/log.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/map/__init__.py
--rw-r--r--   0        0        0      444 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/map/conversion.py
--rw-r--r--   0        0        0      245 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/python_task.py
--rw-r--r--   0        0        0      679 2024-03-10 01:37:08.849171 zrb-0.9.2/src/zrb/helper/render_data.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/helper/string/__init__.py
--rw-r--r--   0        0        0      112 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/string/constant.py
--rw-r--r--   0        0        0     1431 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/string/conversion.py
--rw-r--r--   0        0        0      330 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/string/jinja.py
--rw-r--r--   0        0        0      144 2023-10-07 04:36:46.239224 zrb-0.9.2/src/zrb/helper/string/modification.py
--rw-r--r--   0        0        0      291 2023-09-07 23:19:19.451089 zrb-0.9.2/src/zrb/helper/string/parse_replacement.py
--rw-r--r--   0        0        0      402 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/typecheck.py
--rw-r--r--   0        0        0      312 2024-03-10 01:37:08.853172 zrb-0.9.2/src/zrb/helper/typing.py
--rw-r--r--   0        0        0     3545 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/helper/util.py
--rw-r--r--   0        0        0      118 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/runner.py
--rw-r--r--   0        0        0      229 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/shell-scripts/_common-util.sh
--rw-r--r--   0        0        0     2999 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/shell-scripts/ensure-docker-is-installed.sh
--rw-r--r--   0        0        0     1146 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/shell-scripts/ensure-rsync-is-installed.sh
--rw-r--r--   0        0        0     2414 2024-03-07 06:21:41.700065 zrb-0.9.2/src/zrb/shell-scripts/ensure-ssh-is-installed.sh
--rw-r--r--   0        0        0      843 2023-12-03 01:12:52.544398 zrb-0.9.2/src/zrb/shell-scripts/notify.ps1
--rw-r--r--   0        0        0      353 2023-11-09 07:37:41.473343 zrb-0.9.2/src/zrb/shell-scripts/rsync-util.sh
--rw-r--r--   0        0        0      401 2023-10-07 04:36:46.239224 zrb-0.9.2/src/zrb/shell-scripts/ssh-util.sh
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/task/__init__.py
--rw-r--r--   0        0        0    36254 2024-03-10 01:37:08.945172 zrb-0.9.2/src/zrb/task/any_task.py
--rw-r--r--   0        0        0      359 2023-10-21 14:01:33.314524 zrb-0.9.2/src/zrb/task/any_task_event_handler.py
--rw-r--r--   0        0        0     9220 2024-03-10 01:37:09.049173 zrb-0.9.2/src/zrb/task/base_remote_cmd_task.py
--rw-r--r--   0        0        0        0 2023-11-30 02:25:11.701393 zrb-0.9.2/src/zrb/task/base_task/__init__.py
--rw-r--r--   0        0        0    17502 2024-03-10 01:37:09.225174 zrb-0.9.2/src/zrb/task/base_task/base_task.py
--rw-r--r--   0        0        0        0 2023-11-30 02:25:11.701393 zrb-0.9.2/src/zrb/task/base_task/component/__init__.py
--rw-r--r--   0        0        0    10300 2024-03-10 01:37:09.321174 zrb-0.9.2/src/zrb/task/base_task/component/base_task_model.py
--rw-r--r--   0        0        0    11275 2024-03-10 01:37:09.453175 zrb-0.9.2/src/zrb/task/base_task/component/common_task_model.py
--rw-r--r--   0        0        0      292 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/task/base_task/component/pid_model.py
--rw-r--r--   0        0        0     4439 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/task/base_task/component/renderer.py
--rw-r--r--   0        0        0     1950 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/task/base_task/component/trackers.py
--rw-r--r--   0        0        0     3117 2024-03-10 01:37:09.485175 zrb-0.9.2/src/zrb/task/checker.py
--rw-r--r--   0        0        0    13890 2024-03-10 01:37:09.617176 zrb-0.9.2/src/zrb/task/cmd_task.py
--rw-r--r--   0        0        0     2887 2024-03-10 01:37:09.641176 zrb-0.9.2/src/zrb/task/decorator.py
--rw-r--r--   0        0        0    14017 2024-03-10 01:37:09.793177 zrb-0.9.2/src/zrb/task/docker_compose_task.py
--rw-r--r--   0        0        0     4639 2024-03-10 01:37:09.837177 zrb-0.9.2/src/zrb/task/flow_task.py
--rw-r--r--   0        0        0     5172 2024-03-10 01:37:09.885177 zrb-0.9.2/src/zrb/task/http_checker.py
--rw-r--r--   0        0        0     5986 2024-03-10 01:37:09.961178 zrb-0.9.2/src/zrb/task/notifier.py
--rw-r--r--   0        0        0     1042 2024-01-23 09:38:21.745760 zrb-0.9.2/src/zrb/task/parallel.py
--rw-r--r--   0        0        0     4153 2024-03-10 01:37:10.005178 zrb-0.9.2/src/zrb/task/path_checker.py
--rw-r--r--   0        0        0     6268 2024-03-10 01:37:10.061178 zrb-0.9.2/src/zrb/task/path_watcher.py
--rw-r--r--   0        0        0     4072 2024-03-10 01:37:10.101179 zrb-0.9.2/src/zrb/task/port_checker.py
--rw-r--r--   0        0        0     7133 2024-03-10 01:37:10.185179 zrb-0.9.2/src/zrb/task/recurring_task.py
--rw-r--r--   0        0        0     3709 2024-03-10 01:37:10.221179 zrb-0.9.2/src/zrb/task/remote_cmd_task.py
--rw-r--r--   0        0        0     6576 2024-03-10 01:37:10.277180 zrb-0.9.2/src/zrb/task/resource_maker.py
--rw-r--r--   0        0        0     3949 2024-03-10 01:37:10.349180 zrb-0.9.2/src/zrb/task/rsync_task.py
--rw-r--r--   0        0        0      182 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task/task.py
--rw-r--r--   0        0        0     3908 2024-03-10 01:37:10.417180 zrb-0.9.2/src/zrb/task/time_watcher.py
--rw-r--r--   0        0        0       44 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_env/constant.py
--rw-r--r--   0        0        0     4766 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_env/env.py
--rw-r--r--   0        0        0     2932 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_env/env_file.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/task_group/__init__.py
--rw-r--r--   0        0        0     5937 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_group/group.py
--rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.2/src/zrb/task_input/__init__.py
--rw-r--r--   0        0        0     1909 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/any_input.py
--rw-r--r--   0        0        0     5484 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/base_input.py
--rw-r--r--   0        0        0     3881 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/bool_input.py
--rw-r--r--   0        0        0     4129 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/choice_input.py
--rw-r--r--   0        0        0       42 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/constant.py
--rw-r--r--   0        0        0     3962 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/float_input.py
--rw-r--r--   0        0        0     4040 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/int_input.py
--rw-r--r--   0        0        0     4029 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/password_input.py
--rw-r--r--   0        0        0     4042 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/str_input.py
--rw-r--r--   0        0        0     2022 2024-01-23 09:38:21.749760 zrb-0.9.2/src/zrb/task_input/task_input.py
--rw-r--r--   0        0        0    16500 1970-01-01 00:00:00.000000 zrb-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      728 2023-08-27 04:24:41.005442 zrb-0.9.3/LICENSE
+-rw-r--r--   0        0        0    15202 2024-02-25 03:37:59.986130 zrb-0.9.3/README.md
+-rw-r--r--   0        0        0     1077 2024-03-12 12:13:16.513037 zrb-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2440 2024-03-12 12:13:46.565177 zrb-0.9.3/src/zrb/__init__.py
+-rw-r--r--   0        0        0      314 2024-03-10 01:36:55.385095 zrb-0.9.3/src/zrb/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.009441 zrb-0.9.3/src/zrb/action/__init__.py
+-rw-r--r--   0        0        0     4839 2024-03-10 01:36:55.385095 zrb-0.9.3/src/zrb/action/runner.py
+-rw-r--r--   0        0        0      548 2024-01-23 09:38:21.729760 zrb-0.9.3/src/zrb/advertisement.py
+-rw-r--r--   0        0        0      477 2024-03-12 12:13:46.589177 zrb-0.9.3/src/zrb/builtin/__init__.py
+-rw-r--r--   0        0        0     1335 2024-01-23 09:38:21.729760 zrb-0.9.3/src/zrb/builtin/base64.py
+-rw-r--r--   0        0        0      613 2024-03-12 12:13:46.601177 zrb-0.9.3/src/zrb/builtin/devtool/__init__.py
+-rw-r--r--   0        0        0     1649 2024-03-07 06:21:41.680065 zrb-0.9.3/src/zrb/builtin/devtool/aws/install.sh
+-rw-r--r--   0        0        0    15461 2024-02-13 00:58:48.332275 zrb-0.9.3/src/zrb/builtin/devtool/devtool_install.py
+-rw-r--r--   0        0        0     3067 2024-03-07 06:21:41.680065 zrb-0.9.3/src/zrb/builtin/devtool/docker/install.sh
+-rw-r--r--   0        0        0      531 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/gcloud/install.sh
+-rw-r--r--   0        0        0      415 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/gvm/download.sh
+-rw-r--r--   0        0        0      538 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/gvm/finalize.sh
+-rw-r--r--   0        0        0      253 2024-01-07 03:05:39.354277 zrb-0.9.3/src/zrb/builtin/devtool/gvm/resource/config.sh
+-rw-r--r--   0        0        0     1040 2024-02-25 03:37:59.986130 zrb-0.9.3/src/zrb/builtin/devtool/helix/install-language-server.sh
+-rw-r--r--   0        0        0     1375 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/helix/install.sh
+-rw-r--r--   0        0        0      282 2023-09-14 07:29:41.114392 zrb-0.9.3/src/zrb/builtin/devtool/helix/resource/config.toml
+-rw-r--r--   0        0        0       56 2023-08-28 15:53:50.909810 zrb-0.9.3/src/zrb/builtin/devtool/helix/resource/themes/gruvbox_transparent.toml
+-rw-r--r--   0        0        0      228 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/helm/install.sh
+-rw-r--r--   0        0        0      269 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/kubectl/install.sh
+-rw-r--r--   0        0        0      192 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/nvm/download.sh
+-rw-r--r--   0        0        0      571 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/nvm/finalize.sh
+-rw-r--r--   0        0        0      222 2024-01-07 03:05:39.354277 zrb-0.9.3/src/zrb/builtin/devtool/nvm/resource/config.sh
+-rw-r--r--   0        0        0      162 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/pulumi/install.sh
+-rw-r--r--   0        0        0       79 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/devtool/pulumi/resource/config.sh
+-rw-r--r--   0        0        0     1788 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/pyenv/download.sh
+-rw-r--r--   0        0        0      607 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/pyenv/finalize.sh
+-rw-r--r--   0        0        0      144 2024-01-07 03:05:39.354277 zrb-0.9.3/src/zrb/builtin/devtool/pyenv/resource/config.sh
+-rw-r--r--   0        0        0      160 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/sdkman/download.sh
+-rw-r--r--   0        0        0      359 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/sdkman/finalize.sh
+-rw-r--r--   0        0        0      173 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/devtool/sdkman/resource/config.sh
+-rw-r--r--   0        0        0     1342 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/selenium/install.sh
+-rw-r--r--   0        0        0      300 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/terraform/install.sh
+-rw-r--r--   0        0        0       84 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/devtool/terraform/resource/config.sh
+-rw-r--r--   0        0        0     1229 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/tmux/install.sh
+-rw-r--r--   0        0        0      416 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/devtool/tmux/resource/config.sh
+-rw-r--r--   0        0        0     1720 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/devtool/zsh/install.sh
+-rw-r--r--   0        0        0     5068 2024-02-25 03:37:59.990130 zrb-0.9.3/src/zrb/builtin/devtool/zsh/resource/config.sh
+-rw-r--r--   0        0        0      586 2024-02-25 11:35:22.812654 zrb-0.9.3/src/zrb/builtin/docker.py
+-rw-r--r--   0        0        0     1134 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/env.py
+-rw-r--r--   0        0        0      746 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/eval.py
+-rw-r--r--   0        0        0     5353 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/explain.py
+-rw-r--r--   0        0        0     1129 2024-03-12 12:13:46.629177 zrb-0.9.3/src/zrb/builtin/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/app_generator/__init__.py
+-rw-r--r--   0        0        0     6192 2024-03-12 12:13:46.693178 zrb-0.9.3/src/zrb/builtin/generator/app_generator/add.py
+-rw-r--r--   0        0        0     5655 2024-03-12 12:13:46.753178 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/add.py
+-rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/__init__.py
+-rw-r--r--   0        0        0      353 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_checker.py
+-rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py
+-rw-r--r--   0        0        0      334 2024-02-25 00:07:25.666566 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/app-activate-venv.sh
+-rw-r--r--   0        0        0       15 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/app-start.sh
+-rw-r--r--   0        0        0       29 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
+-rw-r--r--   0        0        0      126 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
+-rw-r--r--   0        0        0       24 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
+-rw-r--r--   0        0        0     3843 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py
+-rw-r--r--   0        0        0     3500 2024-03-12 12:13:46.785178 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py
+-rw-r--r--   0        0        0      311 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py
+-rw-r--r--   0        0        0      611 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
+-rw-r--r--   0        0        0       31 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/.gitignore
+-rw-r--r--   0        0        0       12 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/.gitignore
+-rw-r--r--   0        0        0      137 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
+-rw-r--r--   0        0        0     2633 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0       74 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/requirements.txt
+-rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
+-rw-r--r--   0        0        0        0 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/template.env
+-rw-r--r--   0        0        0       83 2023-09-14 07:29:41.114392 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0      712 2023-10-12 00:54:12.983360 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0     6544 2024-03-12 12:13:46.861178 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/add.py
+-rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py
+-rw-r--r--   0        0        0     4791 2024-03-12 12:13:46.901179 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py
+-rw-r--r--   0        0        0     3829 2024-03-12 12:13:46.933179 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py
+-rw-r--r--   0        0        0     2245 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py
+-rw-r--r--   0        0        0     1424 2024-03-12 12:13:46.945179 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
+-rw-r--r--   0        0        0       60 2023-09-14 07:29:41.114392 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0      646 2023-10-12 00:54:12.983360 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0       22 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/.dockerignore
+-rw-r--r--   0        0        0       39 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/.gitignore
+-rw-r--r--   0        0        0      214 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/Dockerfile
+-rw-r--r--   0        0        0        7 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/go.work
+-rw-r--r--   0        0        0      523 2023-09-02 10:31:35.040307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/main.go
+-rw-r--r--   0        0        0       83 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/template.env
+-rw-r--r--   0        0        0      481 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/http-port/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_checker.py
+-rw-r--r--   0        0        0     1447 2024-03-12 12:13:46.961179 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/http-port-build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py
+-rw-r--r--   0        0        0      695 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0        0 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/.helmignore
+-rw-r--r--   0        0        0     1154 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/Chart.yaml
+-rw-r--r--   0        0        0     1791 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/NOTES.txt
+-rw-r--r--   0        0        0     1892 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1915 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/deployment.yaml
+-rw-r--r--   0        0        0     1024 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/hpa.yaml
+-rw-r--r--   0        0        0     2101 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/ingress.yaml
+-rw-r--r--   0        0        0      394 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/service.yaml
+-rw-r--r--   0        0        0      342 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      412 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0     1885 2023-09-02 10:31:35.044307 zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/values.yaml
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/cmd_task/__init__.py
+-rw-r--r--   0        0        0     1886 2024-03-12 12:13:46.981179 zrb-0.9.3/src/zrb/builtin/generator/cmd_task/add.py
+-rw-r--r--   0        0        0      489 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/cmd_task/template/_automate/snake_zrb_task_name.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/common/__init__.py
+-rw-r--r--   0        0        0     1899 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/common/helper.py
+-rw-r--r--   0        0        0     3272 2024-03-12 12:13:47.029179 zrb-0.9.3/src/zrb/builtin/generator/common/task_factory.py
+-rw-r--r--   0        0        0     5190 2024-02-18 23:16:10.199317 zrb-0.9.3/src/zrb/builtin/generator/common/task_input.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/__init__.py
+-rw-r--r--   0        0        0     2710 2024-03-12 12:13:47.053179 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/add.py
+-rw-r--r--   0        0        0     1328 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/_automate/snake_zrb_task_name.py
+-rw-r--r--   0        0        0       12 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/.dockerignore
+-rw-r--r--   0        0        0       30 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/.gitignore
+-rw-r--r--   0        0        0       72 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.env
+-rw-r--r--   0        0        0      762 2023-10-12 00:54:12.983360 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.yml
+-rw-r--r--   0        0        0      312 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/Dockerfile
+-rw-r--r--   0        0        0      511 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/main.py
+-rw-r--r--   0        0        0      525 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/__init__.py
+-rw-r--r--   0        0        0     7637 2024-03-12 12:13:47.113180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/add.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/__init__.py
+-rw-r--r--   0        0        0     2263 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_checker.py
+-rw-r--r--   0        0        0     2987 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_config.py
+-rw-r--r--   0        0        0     1178 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env.py
+-rw-r--r--   0        0        0      602 2024-03-12 12:13:47.121180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env_file.py
+-rw-r--r--   0        0        0     3938 2024-03-12 12:13:47.157180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_get_start_microservices.py
+-rw-r--r--   0        0        0     2631 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_helper.py
+-rw-r--r--   0        0        0     1892 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_input.py
+-rw-r--r--   0        0        0      334 2024-02-25 00:07:25.666566 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/activate-venv.sh
+-rw-r--r--   0        0        0      155 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-build-frontend.sh
+-rw-r--r--   0        0        0      377 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-load-test.sh
+-rw-r--r--   0        0        0       48 2024-02-18 23:16:10.199317 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-prepare-backend.sh
+-rw-r--r--   0        0        0       49 2024-02-18 23:16:10.199317 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-prepare-load-test.sh
+-rw-r--r--   0        0        0       56 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-start.sh
+-rw-r--r--   0        0        0      308 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/app-test.sh
+-rw-r--r--   0        0        0       29 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
+-rw-r--r--   0        0        0      126 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
+-rw-r--r--   0        0        0       24 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
+-rw-r--r--   0        0        0       15 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/config/modules.json
+-rw-r--r--   0        0        0     4408 2024-03-12 12:13:47.189180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/container.py
+-rw-r--r--   0        0        0     2513 2024-03-12 12:13:47.209180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/deployment.py
+-rw-r--r--   0        0        0     1878 2024-03-12 12:13:47.229180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/frontend.py
+-rw-r--r--   0        0        0     1947 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/image.py
+-rw-r--r--   0        0        0     2769 2024-03-12 12:13:47.253180 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/load_test.py
+-rw-r--r--   0        0        0     6454 2024-03-12 12:13:47.317181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/local.py
+-rw-r--r--   0        0        0     2183 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/test.py
+-rw-r--r--   0        0        0       53 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/.gitignore
+-rw-r--r--   0        0        0    10176 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/README.md
+-rw-r--r--   0        0        0       56 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/all-module-disabled.env
+-rw-r--r--   0        0        0       54 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/all-module-enabled.env
+-rw-r--r--   0        0        0       12 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/.gitignore
+-rw-r--r--   0        0        0      137 2023-08-27 04:24:41.013442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
+-rw-r--r--   0        0        0     1139 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/README.md
+-rw-r--r--   0        0        0     1519 2024-03-12 12:13:47.333181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0     4943 2024-03-07 06:21:52.652119 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/_common.py
+-rw-r--r--   0        0        0     6043 2024-03-12 12:13:47.389181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/app_helper.py
+-rw-r--r--   0        0        0      351 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/.helmignore
+-rw-r--r--   0        0        0      231 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.lock
+-rw-r--r--   0        0        0     1075 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.yaml
+-rw-r--r--   0        0        0   185265 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/README.md
+-rw-r--r--   0        0        0      360 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/.helmignore
+-rw-r--r--   0        0        0      531 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/Chart.yaml
+-rw-r--r--   0        0        0     7191 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/README.md
+-rw-r--r--   0        0        0     5480 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     7044 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1494 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_compatibility.tpl
+-rw-r--r--   0        0        0     1703 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     4071 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2431 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0     2147 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2497 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     1980 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_resources.tpl
+-rw-r--r--   0        0        0     7908 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      698 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0     1385 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2599 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0     3449 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2644 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     4059 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4449 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     4003 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5091 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3334 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2526 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      182 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/values.yaml
+-rw-r--r--   0        0        0     7987 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/NOTES.txt
+-rw-r--r--   0        0        0    14792 2024-03-07 06:21:41.684065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/_helpers.tpl
+-rw-r--r--   0        0        0     6066 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/cronjob.yaml
+-rw-r--r--   0        0        0     1617 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/pvc.yaml
+-rw-r--r--   0        0        0      189 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1047 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/configmap.yaml
+-rw-r--r--   0        0        0      818 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/extended-configmap.yaml
+-rw-r--r--   0        0        0      755 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/initialization-configmap.yaml
+-rw-r--r--   0        0        0      690 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1418 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-svc.yaml
+-rw-r--r--   0        0        0     3247 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/networkpolicy.yaml
+-rw-r--r--   0        0        0     2314 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/servicemonitor.yaml
+-rw-r--r--   0        0        0    38198 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/statefulset.yaml
+-rw-r--r--   0        0        0     1827 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc-headless.yaml
+-rw-r--r--   0        0        0     2883 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc.yaml
+-rw-r--r--   0        0        0     1043 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1069 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/psp.yaml
+-rw-r--r--   0        0        0      829 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/extended-configmap.yaml
+-rw-r--r--   0        0        0      734 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1473 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-svc.yaml
+-rw-r--r--   0        0        0     3365 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/networkpolicy.yaml
+-rw-r--r--   0        0        0     2368 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/servicemonitor.yaml
+-rw-r--r--   0        0        0    33309 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/statefulset.yaml
+-rw-r--r--   0        0        0     1910 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc-headless.yaml
+-rw-r--r--   0        0        0     3078 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc.yaml
+-rw-r--r--   0        0        0     1077 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/role.yaml
+-rw-r--r--   0        0        0      846 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     5145 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/secrets.yaml
+-rw-r--r--   0        0        0      837 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1963 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0     4571 2023-08-27 04:24:41.017442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.schema.json
+-rw-r--r--   0        0        0    80485 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.yaml
+-rw-r--r--   0        0        0      351 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/.helmignore
+-rw-r--r--   0        0        0      231 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.lock
+-rw-r--r--   0        0        0      907 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.yaml
+-rw-r--r--   0        0        0   105669 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/README.md
+-rw-r--r--   0        0        0      360 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/.helmignore
+-rw-r--r--   0        0        0      531 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/Chart.yaml
+-rw-r--r--   0        0        0     7191 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/README.md
+-rw-r--r--   0        0        0     5480 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     7044 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1494 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_compatibility.tpl
+-rw-r--r--   0        0        0     1703 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     4071 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2431 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0     2147 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2497 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     1980 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_resources.tpl
+-rw-r--r--   0        0        0     7908 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      698 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0     1385 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2599 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0     3449 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2644 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     4059 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4449 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     4003 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5091 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3334 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2526 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      182 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/values.yaml
+-rw-r--r--   0        0        0     7342 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/NOTES.txt
+-rw-r--r--   0        0        0    12599 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1055 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/config-secret.yaml
+-rw-r--r--   0        0        0      189 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1875 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress-tls-secrets.yaml
+-rw-r--r--   0        0        0     3265 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress.yaml
+-rw-r--r--   0        0        0      693 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/init-configmap.yaml
+-rw-r--r--   0        0        0     3812 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/networkpolicy.yaml
+-rw-r--r--   0        0        0     1090 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/pdb.yaml
+-rw-r--r--   0        0        0     1114 2024-03-07 06:21:41.688065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0      776 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/role.yaml
+-rw-r--r--   0        0        0      870 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     2809 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/secrets.yaml
+-rw-r--r--   0        0        0      908 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     3142 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0    25075 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/statefulset.yaml
+-rw-r--r--   0        0        0     1966 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc-headless.yaml
+-rw-r--r--   0        0        0     5530 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc.yaml
+-rw-r--r--   0        0        0     2021 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0      116 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/validation.yaml
+-rw-r--r--   0        0        0     2815 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.schema.json
+-rw-r--r--   0        0        0    65942 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.yaml
+-rw-r--r--   0        0        0      366 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/.helmignore
+-rw-r--r--   0        0        0      293 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.lock
+-rw-r--r--   0        0        0     1158 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.yaml
+-rw-r--r--   0        0        0    11357 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/LICENSE
+-rw-r--r--   0        0        0    61366 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/README.md
+-rw-r--r--   0        0        0      366 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/.helmignore
+-rw-r--r--   0        0        0      837 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/Chart.yaml
+-rw-r--r--   0        0        0    11357 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/LICENSE
+-rw-r--r--   0        0        0    24858 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/README.md
+-rw-r--r--   0        0        0     1197 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/01-default-values.yaml
+-rw-r--r--   0        0        0     1177 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/02-broker-tls-values.yaml
+-rw-r--r--   0        0        0     3898 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/_helpers.tpl
+-rw-r--r--   0        0        0    13014 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/deployment.yaml
+-rw-r--r--   0        0        0     1432 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/pod-monitor.yaml
+-rw-r--r--   0        0        0     1535 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/service.yaml
+-rw-r--r--   0        0        0     1160 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     8687 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/tests/01-mm2-values.yaml
+-rw-r--r--   0        0        0    12366 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/values.yaml
+-rw-r--r--   0        0        0      366 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/.helmignore
+-rw-r--r--   0        0        0      728 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/Chart.yaml
+-rw-r--r--   0        0        0    13250 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/README.md
+-rw-r--r--   0        0        0     3112 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/examples/console-enterprise.yaml
+-rw-r--r--   0        0        0     2511 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/NOTES.txt
+-rw-r--r--   0        0        0     3199 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1379 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/configmap.yaml
+-rw-r--r--   0        0        0    12390 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/deployment.yaml
+-rw-r--r--   0        0        0     1755 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/hpa.yaml
+-rw-r--r--   0        0        0     2897 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/ingress.yaml
+-rw-r--r--   0        0        0     3615 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/secret.yaml
+-rw-r--r--   0        0        0     1406 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/service.yaml
+-rw-r--r--   0        0        0     1084 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      570 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0     6149 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.schema.json
+-rw-r--r--   0        0        0     7718 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.yaml
+-rw-r--r--   0        0        0      832 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/01-default-values.yaml
+-rw-r--r--   0        0        0     1258 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/02-one-node-cluster-no-tls-no-sasl-values.yaml
+-rw-r--r--   0        0        0     1012 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/03-one-node-cluster-tls-no-sasl-values.yaml
+-rw-r--r--   0        0        0     1135 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/04-one-node-cluster-no-tls-sasl-values.yaml
+-rw-r--r--   0        0        0     1281 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/05-one-node-cluster-tls-sasl-values.yaml
+-rw-r--r--   0        0        0      868 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/06-rack-awareness-values.yaml
+-rw-r--r--   0        0        0     1850 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/07-multiple-listeners-values.yaml
+-rw-r--r--   0        0        0     1099 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/08-custom-podantiaffinity-values.yaml
+-rw-r--r--   0        0        0     2081 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/09-initcontainers-resources-values.yaml
+-rw-r--r--   0        0        0     1095 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/10-external-addresses-values.yaml
+-rw-r--r--   0        0        0     1293 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/11-update-sasl-users-values.yaml
+-rw-r--r--   0        0        0     2608 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/12-external-cert-secrets-values.yaml
+-rw-r--r--   0        0        0     1124 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/13-loadbalancer-tls-values.yaml
+-rw-r--r--   0        0        0      835 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/14-prometheus-no-tls-values.yaml
+-rw-r--r--   0        0        0      834 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/15-prometheus-tls-values.yaml
+-rw-r--r--   0        0        0      869 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/16-controller-sidecar-values.yaml
+-rw-r--r--   0        0        0      944 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/17-resources-without-unit-values.yaml
+-rw-r--r--   0        0        0     1049 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/18-single-external-address-values.yaml
+-rw-r--r--   0        0        0     1513 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/21-eks-tiered-storage-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1702 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/22-gke-tiered-storage-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1745 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/23-aks-tiered-storage-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1545 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/24-eks-tiered-storage-persistent-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1734 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/25-gke-tiered-storage-persistent-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1777 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/26-aks-tiered-storage-persistent-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1603 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/27-eks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1792 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/28-gke-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1815 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/29-aks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl
+-rw-r--r--   0        0        0     1308 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/96-audit-logging-values.yaml.tpl
+-rw-r--r--   0        0        0     1131 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/97-license-key-values.yaml.tpl
+-rw-r--r--   0        0        0     1166 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/98-license-secret-values.yaml
+-rw-r--r--   0        0        0     2363 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/99-none-existent-config-options-with-empty-values.yaml
+-rw-r--r--   0        0        0     4551 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/NOTES.txt
+-rw-r--r--   0        0        0    31567 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_configmap.tpl
+-rw-r--r--   0        0        0     1893 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_example-commands.tpl
+-rw-r--r--   0        0        0    36976 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1472 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_job.tpl
+-rw-r--r--   0        0        0     5041 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_statefulset.tpl
+-rw-r--r--   0        0        0     1118 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2784 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/cert-issuers.yaml
+-rw-r--r--   0        0        0     4010 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/certs.yaml
+-rw-r--r--   0        0        0     1366 2024-03-07 06:21:41.692065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/configmap.yaml
+-rw-r--r--   0        0        0     4825 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/connectors/connectors.yaml
+-rw-r--r--   0        0        0    12686 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/console/configmap-and-deployment.yaml
+-rw-r--r--   0        0        0     1647 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     5811 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-install-upgrade-job.yaml
+-rw-r--r--   0        0        0     5551 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-upgrade.yaml
+-rw-r--r--   0        0        0     5778 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/rbac.yaml
+-rw-r--r--   0        0        0    15622 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/secrets.yaml
+-rw-r--r--   0        0        0     1776 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.internal.yaml
+-rw-r--r--   0        0        0     4130 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.loadbalancer.yaml
+-rw-r--r--   0        0        0     1150 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1936 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0     2874 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/services.nodeport.yaml
+-rw-r--r--   0        0        0    23322 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/statefulset.yaml
+-rw-r--r--   0        0        0     2059 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-api-status.yaml
+-rw-r--r--   0        0        0     4090 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-auditLogging.yaml
+-rw-r--r--   0        0        0     8436 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-connector-via-console.yaml
+-rw-r--r--   0        0        0     1988 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-console.yaml
+-rw-r--r--   0        0        0     5105 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-internal-external-tls-secrets.yaml
+-rw-r--r--   0        0        0     2589 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-internal-tls-status.yaml
+-rw-r--r--   0        0        0     4608 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-nodelete.yaml
+-rw-r--r--   0        0        0     4010 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-produce-consume.yaml
+-rw-r--r--   0        0        0     3144 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-sasl-status.yaml
+-rw-r--r--   0        0        0     3036 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-license-with-console.yaml
+-rw-r--r--   0        0        0     2620 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-lifecycle-scripts.yaml
+-rw-r--r--   0        0        0     6188 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-loadbalancer-tls.yaml
+-rw-r--r--   0        0        0     6207 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-nodeport-tls.yaml
+-rw-r--r--   0        0        0     3906 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-internal-tls-status.yaml
+-rw-r--r--   0        0        0     3338 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-status.yaml
+-rw-r--r--   0        0        0     3442 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-prometheus-targets.yaml
+-rw-r--r--   0        0        0     2619 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rack-awareness.yaml
+-rw-r--r--   0        0        0     3938 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rpk-debug-bundle.yaml
+-rw-r--r--   0        0        0     2996 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-sasl-updated.yaml
+-rw-r--r--   0        0        0     8953 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-internal-tls-status.yaml
+-rw-r--r--   0        0        0     9070 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-status.yaml
+-rw-r--r--   0        0        0    44082 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.schema.json
+-rw-r--r--   0        0        0    62802 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.yaml
+-rw-r--r--   0        0        0      633 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.lock
+-rw-r--r--   0        0        0     1335 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.yaml
+-rw-r--r--   0        0        0    32538 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/README.md
+-rw-r--r--   0        0        0      816 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/Chart.yaml
+-rw-r--r--   0        0        0    17134 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/README.md
+-rw-r--r--   0        0        0      593 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/NOTES.txt
+-rw-r--r--   0        0        0     5361 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/_helpers.tpl
+-rw-r--r--   0        0        0     3837 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-deployment.yaml
+-rw-r--r--   0        0        0      634 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrole.yaml
+-rw-r--r--   0        0        0      760 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrolebinding.yaml
+-rw-r--r--   0        0        0     1440 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp.yaml
+-rw-r--r--   0        0        0     3748 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-rbac.yaml
+-rw-r--r--   0        0        0      949 2023-08-27 04:24:41.021442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-serviceaccount.yaml
+-rw-r--r--   0        0        0   374997 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/crds.yaml
+-rw-r--r--   0        0        0     5687 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/deployment.yaml
+-rw-r--r--   0        0        0      594 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrole.yaml
+-rw-r--r--   0        0        0      722 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrolebinding.yaml
+-rw-r--r--   0        0        0     1398 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp.yaml
+-rw-r--r--   0        0        0    19514 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/rbac.yaml
+-rw-r--r--   0        0        0      972 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/service.yaml
+-rw-r--r--   0        0        0      863 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1591 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0     2845 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-job.yaml
+-rw-r--r--   0        0        0      779 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrole.yaml
+-rw-r--r--   0        0        0      910 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrolebinding.yaml
+-rw-r--r--   0        0        0     1520 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp.yaml
+-rw-r--r--   0        0        0     1642 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-rbac.yaml
+-rw-r--r--   0        0        0      994 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-serviceaccount.yaml
+-rw-r--r--   0        0        0      746 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-config.yaml
+-rw-r--r--   0        0        0     6309 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-deployment.yaml
+-rw-r--r--   0        0        0     1657 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-mutating-webhook.yaml
+-rw-r--r--   0        0        0      572 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrole.yaml
+-rw-r--r--   0        0        0      694 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrolebinding.yaml
+-rw-r--r--   0        0        0     1558 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp.yaml
+-rw-r--r--   0        0        0     2641 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-rbac.yaml
+-rw-r--r--   0        0        0      954 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-service.yaml
+-rw-r--r--   0        0        0      877 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-serviceaccount.yaml
+-rw-r--r--   0        0        0     1874 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-validating-webhook.yaml
+-rw-r--r--   0        0        0    17877 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/values.yaml
+-rw-r--r--   0        0        0      349 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/.helmignore
+-rw-r--r--   0        0        0      234 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.lock
+-rw-r--r--   0        0        0      614 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.yaml
+-rw-r--r--   0        0        0      839 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/README.md
+-rw-r--r--   0        0        0      333 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/.helmignore
+-rw-r--r--   0        0        0      225 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.lock
+-rw-r--r--   0        0        0      673 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.yaml
+-rw-r--r--   0        0        0    60071 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/README.md
+-rw-r--r--   0        0        0      342 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/.helmignore
+-rw-r--r--   0        0        0      529 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/Chart.yaml
+-rw-r--r--   0        0        0     7114 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/README.md
+-rw-r--r--   0        0        0     3723 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     5472 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     2587 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2361 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0      586 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2427 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     7323 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      628 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0      391 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2064 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0      580 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      118 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/values.yaml
+-rw-r--r--   0        0        0     3774 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/NOTES.txt
+-rw-r--r--   0        0        0    12157 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/_helpers.tpl
+-rw-r--r--   0        0        0      726 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/configmap.yaml
+-rw-r--r--   0        0        0      117 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1180 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/metrics-svc.yaml
+-rw-r--r--   0        0        0     1606 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/networkpolicy.yaml
+-rw-r--r--   0        0        0     1096 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/pdb.yaml
+-rw-r--r--   0        0        0     1211 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     5313 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/scripts-configmap.yaml
+-rw-r--r--   0        0        0     4077 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/secrets.yaml
+-rw-r--r--   0        0        0      944 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     2516 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0    28701 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/statefulset.yaml
+-rw-r--r--   0        0        0     1747 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc-headless.yaml
+-rw-r--r--   0        0        0     3297 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc.yaml
+-rw-r--r--   0        0        0     3656 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0    36148 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/values.yaml
+-rw-r--r--   0        0        0    77365 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallations.clickhouse.altinity.com.yaml
+-rw-r--r--   0        0        0    77423 2023-08-27 04:24:41.025442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallationtemplates.clickhouse.altinity.com.yaml
+-rw-r--r--   0        0        0    20500 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseoperatorconfigurations.clickhouse.altinity.com.yaml
+-rw-r--r--   0        0        0    10595 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/_helper.tpl
+-rw-r--r--   0        0        0    10878 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/clickhouse-instance.yaml
+-rw-r--r--   0        0        0      924 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/configmap.yaml
+-rw-r--r--   0        0        0      421 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/serviceaccount.yaml
+-rw-r--r--   0        0        0      664 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/storage-class.yaml
+-rw-r--r--   0        0        0      333 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-confd-files.yaml
+-rw-r--r--   0        0        0     8493 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-configd-files.yaml
+-rw-r--r--   0        0        0    11736 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-files.yaml
+-rw-r--r--   0        0        0     2694 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-templatesd-files.yaml
+-rw-r--r--   0        0        0     1681 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-usersd-files.yaml
+-rw-r--r--   0        0        0     5371 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/deployment.yaml
+-rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/namespace.yaml
+-rw-r--r--   0        0        0     2638 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/role.yaml
+-rw-r--r--   0        0        0      701 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/rolebinding.yaml
+-rw-r--r--   0        0        0      419 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/secret.yaml
+-rw-r--r--   0        0        0      600 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/service.yaml
+-rw-r--r--   0        0        0      482 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/serviceaccount.yaml
+-rw-r--r--   0        0        0    20429 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/values.yaml
+-rw-r--r--   0        0        0      342 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/.helmignore
+-rw-r--r--   0        0        0    24586 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/CHANGELOG.md
+-rw-r--r--   0        0        0     1007 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/Chart.yaml
+-rw-r--r--   0        0        0      213 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/OWNERS
+-rw-r--r--   0        0        0    36385 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md
+-rw-r--r--   0        0        0    10571 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md.gotmpl
+-rw-r--r--   0        0        0      171 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/controller-custom-ingressclass-flags.yaml
+-rw-r--r--   0        0        0      267 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customconfig-values.yaml
+-rw-r--r--   0        0        0      337 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customnodeport-values.yaml
+-rw-r--r--   0        0        0      198 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-extra-modules.yaml
+-rw-r--r--   0        0        0      280 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-headers-values.yaml
+-rw-r--r--   0        0        0      315 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-internal-lb-values.yaml
+-rw-r--r--   0        0        0      191 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-nodeport-values.yaml
+-rw-r--r--   0        0        0      368 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-podannotations-values.yaml
+-rw-r--r--   0        0        0      338 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-configMapNamespace-values.yaml
+-rw-r--r--   0        0        0      284 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-portNamePrefix-values.yaml
+-rw-r--r--   0        0        0      260 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-values.yaml
+-rw-r--r--   0        0        0      254 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-values.yaml
+-rw-r--r--   0        0        0      192 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-default-values.yaml
+-rw-r--r--   0        0        0      221 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-metrics-values.yaml
+-rw-r--r--   0        0        0      228 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-psp-values.yaml
+-rw-r--r--   0        0        0      227 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-and-psp-values.yaml
+-rw-r--r--   0        0        0      191 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-values.yaml
+-rw-r--r--   0        0        0      274 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-behavior-values.yaml
+-rw-r--r--   0        0        0      207 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-values.yaml
+-rw-r--r--   0        0        0      248 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customconfig-values.yaml
+-rw-r--r--   0        0        0      318 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customnodeport-values.yaml
+-rw-r--r--   0        0        0      170 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-default-values.yaml
+-rw-r--r--   0        0        0      197 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-extra-modules.yaml
+-rw-r--r--   0        0        0      262 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-headers-values.yaml
+-rw-r--r--   0        0        0      297 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-internal-lb-values.yaml
+-rw-r--r--   0        0        0      203 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-metrics-values.yaml
+-rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-nodeport-values.yaml
+-rw-r--r--   0        0        0      350 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-podannotations-values.yaml
+-rw-r--r--   0        0        0      170 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-psp-values.yaml
+-rw-r--r--   0        0        0      320 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-configMapNamespace-values.yaml
+-rw-r--r--   0        0        0      266 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-portNamePrefix-values.yaml
+-rw-r--r--   0        0        0      242 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-values.yaml
+-rw-r--r--   0        0        0      196 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-values.yaml
+-rw-r--r--   0        0        0      209 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-and-psp-values.yaml
+-rw-r--r--   0        0        0      204 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-extraEnvs-values.yaml
+-rw-r--r--   0        0        0      425 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-resources-values.yaml
+-rw-r--r--   0        0        0      173 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-values.yaml
+-rw-r--r--   0        0        0     3498 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/NOTES.txt
+-rw-r--r--   0        0        0     5570 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2996 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_params.tpl
+-rw-r--r--   0        0        0     1120 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrole.yaml
+-rw-r--r--   0        0        0      913 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrolebinding.yaml
+-rw-r--r--   0        0        0     3740 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-createSecret.yaml
+-rw-r--r--   0        0        0     3783 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-patchWebhook.yaml
+-rw-r--r--   0        0        0     1183 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/psp.yaml
+-rw-r--r--   0        0        0      769 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/role.yaml
+-rw-r--r--   0        0        0      936 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/rolebinding.yaml
+-rw-r--r--   0        0        0      650 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/serviceaccount.yaml
+-rw-r--r--   0        0        0     1937 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/validating-webhook.yaml
+-rw-r--r--   0        0        0     1949 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      612 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0      459 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-addheaders.yaml
+-rw-r--r--   0        0        0      693 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-proxyheaders.yaml
+-rw-r--r--   0        0        0      547 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-tcp.yaml
+-rw-r--r--   0        0        0      547 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-udp.yaml
+-rw-r--r--   0        0        0     1162 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap.yaml
+-rw-r--r--   0        0        0     9624 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-daemonset.yaml
+-rw-r--r--   0        0        0     9990 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-deployment.yaml
+-rw-r--r--   0        0        0     1620 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-hpa.yaml
+-rw-r--r--   0        0        0      760 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-ingressclass.yaml
+-rw-r--r--   0        0        0     1619 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-keda.yaml
+-rw-r--r--   0        0        0      877 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0      961 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-prometheusrules.yaml
+-rw-r--r--   0        0        0     2572 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-psp.yaml
+-rw-r--r--   0        0        0     2463 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-role.yaml
+-rw-r--r--   0        0        0      651 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-rolebinding.yaml
+-rw-r--r--   0        0        0     3570 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-internal.yaml
+-rw-r--r--   0        0        0     2106 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-metrics.yaml
+-rw-r--r--   0        0        0     1670 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-webhook.yaml
+-rw-r--r--   0        0        0     4504 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service.yaml
+-rw-r--r--   0        0        0      623 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-serviceaccount.yaml
+-rw-r--r--   0        0        0     2061 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-servicemonitor.yaml
+-rw-r--r--   0        0        0      464 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-wehbooks-networkpolicy.yaml
+-rw-r--r--   0        0        0     5476 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-deployment.yaml
+-rw-r--r--   0        0        0     1143 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-hpa.yaml
+-rw-r--r--   0        0        0      864 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0      925 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-psp.yaml
+-rw-r--r--   0        0        0      806 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-role.yaml
+-rw-r--r--   0        0        0      760 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-rolebinding.yaml
+-rw-r--r--   0        0        0     1562 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-service.yaml
+-rw-r--r--   0        0        0      573 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-serviceaccount.yaml
+-rw-r--r--   0        0        0      233 2023-08-27 04:24:41.029442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/dh-param-secret.yaml
+-rw-r--r--   0        0        0    31188 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/values.yaml
+-rw-r--r--   0        0        0      349 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/.helmignore
+-rw-r--r--   0        0        0      556 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/Chart.yaml
+-rw-r--r--   0        0        0      276 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/NOTES.txt
+-rw-r--r--   0        0        0    17762 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_config.tpl
+-rw-r--r--   0        0        0    12793 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_helpers.tpl
+-rw-r--r--   0        0        0      442 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/apikey-secret.yaml
+-rw-r--r--   0        0        0      172 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/namespace.yaml
+-rw-r--r--   0        0        0      448 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrole.yaml
+-rw-r--r--   0        0        0      540 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrolebinding.yaml
+-rw-r--r--   0        0        0      334 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/configmap.yaml
+-rw-r--r--   0        0        0     6500 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/daemonset.yaml
+-rw-r--r--   0        0        0     1763 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/ingress.yaml
+-rw-r--r--   0        0        0      565 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/service.yaml
+-rw-r--r--   0        0        0      471 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/serviceaccount.yaml
+-rw-r--r--   0        0        0      513 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/tests/test-connection.yaml
+-rw-r--r--   0        0        0      473 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrole.yaml
+-rw-r--r--   0        0        0      564 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrolebinding.yaml
+-rw-r--r--   0        0        0      359 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/configmap.yaml
+-rw-r--r--   0        0        0     5859 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/deployment.yaml
+-rw-r--r--   0        0        0     1813 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/ingress.yaml
+-rw-r--r--   0        0        0      590 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/service.yaml
+-rw-r--r--   0        0        0      501 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/serviceaccount.yaml
+-rw-r--r--   0        0        0      599 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/tests/test-connection.yaml
+-rw-r--r--   0        0        0      577 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/tls-secret.yaml
+-rw-r--r--   0        0        0    28367 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/values.yaml
+-rw-r--r--   0        0        0      305 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.lock
+-rw-r--r--   0        0        0      872 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.yaml
+-rw-r--r--   0        0        0    51454 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/README.md
+-rw-r--r--   0        0        0      342 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/.helmignore
+-rw-r--r--   0        0        0      569 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/Chart.yaml
+-rw-r--r--   0        0        0    25039 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/README.md
+-rw-r--r--   0        0        0     3502 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     4780 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     2437 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2314 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0      586 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2461 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     6183 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      628 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0      391 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2049 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0      580 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      118 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/values.yaml
+-rw-r--r--   0        0        0      333 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/.helmignore
+-rw-r--r--   0        0        0      219 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.lock
+-rw-r--r--   0        0        0      845 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.yaml
+-rw-r--r--   0        0        0   101381 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/README.md
+-rw-r--r--   0        0        0      342 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/.helmignore
+-rw-r--r--   0        0        0      569 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/Chart.yaml
+-rw-r--r--   0        0        0    25039 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/README.md
+-rw-r--r--   0        0        0     3502 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     4780 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1633 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     2437 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2314 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0      586 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2461 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     6183 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      628 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0      391 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2049 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0      580 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2574 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     3989 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4379 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     3933 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5021 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3264 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2456 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      118 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/values.yaml
+-rw-r--r--   0        0        0     5433 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/NOTES.txt
+-rw-r--r--   0        0        0    13838 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/_helpers.tpl
+-rw-r--r--   0        0        0      117 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1341 2023-08-27 04:24:41.033442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/networkpolicy-egress.yaml
+-rw-r--r--   0        0        0     1072 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/configmap.yaml
+-rw-r--r--   0        0        0      842 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/extended-configmap.yaml
+-rw-r--r--   0        0        0      782 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/initialization-configmap.yaml
+-rw-r--r--   0        0        0      717 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1269 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-svc.yaml
+-rw-r--r--   0        0        0     3347 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/networkpolicy.yaml
+-rw-r--r--   0        0        0     2390 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/servicemonitor.yaml
+-rw-r--r--   0        0        0    34437 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/statefulset.yaml
+-rw-r--r--   0        0        0     1452 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc-headless.yaml
+-rw-r--r--   0        0        0     2721 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc.yaml
+-rw-r--r--   0        0        0     1126 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1162 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/psp.yaml
+-rw-r--r--   0        0        0      853 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/extended-configmap.yaml
+-rw-r--r--   0        0        0      761 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1319 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-svc.yaml
+-rw-r--r--   0        0        0     2225 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/networkpolicy.yaml
+-rw-r--r--   0        0        0     2444 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/servicemonitor.yaml
+-rw-r--r--   0        0        0    29932 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/statefulset.yaml
+-rw-r--r--   0        0        0     1520 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc-headless.yaml
+-rw-r--r--   0        0        0     2919 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc.yaml
+-rw-r--r--   0        0        0     1172 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/role.yaml
+-rw-r--r--   0        0        0      873 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     1769 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/secrets.yaml
+-rw-r--r--   0        0        0      875 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1690 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0     4571 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.schema.json
+-rw-r--r--   0        0        0    63223 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.yaml
+-rw-r--r--   0        0        0     5526 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/NOTES.txt
+-rw-r--r--   0        0        0     9090 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1947 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap-env-vars.yaml
+-rw-r--r--   0        0        0      743 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap.yaml
+-rw-r--r--   0        0        0      117 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1160 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/headless-service.yaml
+-rw-r--r--   0        0        0     1858 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/hpa.yaml
+-rw-r--r--   0        0        0     3152 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/ingress.yaml
+-rw-r--r--   0        0        0      802 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/init-scripts-configmap.yaml
+-rw-r--r--   0        0        0      850 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-configmap.yaml
+-rw-r--r--   0        0        0     7172 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-job.yaml
+-rw-r--r--   0        0        0     1228 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/metrics-service.yaml
+-rw-r--r--   0        0        0     1498 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/networkpolicy.yaml
+-rw-r--r--   0        0        0     1023 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/pdb.yaml
+-rw-r--r--   0        0        0     1129 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0      950 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/role.yaml
+-rw-r--r--   0        0        0      974 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     1982 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/secrets.yaml
+-rw-r--r--   0        0        0     3171 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/service.yaml
+-rw-r--r--   0        0        0     1019 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     2655 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0    20259 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/statefulset.yaml
+-rw-r--r--   0        0        0     3273 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/tls-secret.yaml
+-rw-r--r--   0        0        0    40146 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/values.yaml
+-rw-r--r--   0        0        0      368 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/.helmignore
+-rw-r--r--   0        0        0      359 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/Chart.yaml
+-rw-r--r--   0        0        0     9349 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/README.md
+-rw-r--r--   0        0        0     2668 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/NOTES.txt
+-rw-r--r--   0        0        0     3022 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_bucket.txt
+-rw-r--r--   0        0        0     2010 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_policy.txt
+-rw-r--r--   0        0        0     3087 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_user.txt
+-rw-r--r--   0        0        0     1473 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_custom_command.txt
+-rw-r--r--   0        0        0      469 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_policy.tpl
+-rw-r--r--   0        0        0     6479 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helpers.tpl
+-rw-r--r--   0        0        0      887 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/configmap.yaml
+-rw-r--r--   0        0        0     1693 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-ingress.yaml
+-rw-r--r--   0        0        0     1558 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-service.yaml
+-rw-r--r--   0        0        0     6682 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/deployment.yaml
+-rw-r--r--   0        0        0     6449 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/gateway-deployment.yaml
+-rw-r--r--   0        0        0     1594 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/ingress.yaml
+-rw-r--r--   0        0        0      812 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/networkpolicy.yaml
+-rw-r--r--   0        0        0      371 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     3130 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-bucket-job.yaml
+-rw-r--r--   0        0        0     3135 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-policy-job.yaml
+-rw-r--r--   0        0        0     3460 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-user-job.yaml
+-rw-r--r--   0        0        0     3190 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-custom-command.yaml
+-rw-r--r--   0        0        0     1059 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/pvc.yaml
+-rw-r--r--   0        0        0      752 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/secrets.yaml
+-rw-r--r--   0        0        0     1117 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/securitycontextconstraints.yaml
+-rw-r--r--   0        0        0     1457 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/service.yaml
+-rw-r--r--   0        0        0      195 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     2036 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0     8507 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/statefulset.yaml
+-rw-r--r--   0        0        0    13974 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/values.yaml
+-rw-r--r--   0        0        0     2317 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/NOTES.txt
+-rw-r--r--   0        0        0     8852 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_clickhouse.tpl
+-rw-r--r--   0        0        0    23248 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_helpers.tpl
+-rw-r--r--   0        0        0      460 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/configmap.yaml
+-rw-r--r--   0        0        0     1716 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/ingress.yaml
+-rw-r--r--   0        0        0      434 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/pdb.yaml
+-rw-r--r--   0        0        0      432 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/serviceaccount.yaml
+-rw-r--r--   0        0        0     1455 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/services.yaml
+-rw-r--r--   0        0        0     8128 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/statefulset.yaml
+-rw-r--r--   0        0        0      974 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/cert-issuer.yaml
+-rw-r--r--   0        0        0     1792 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/configmap.yaml
+-rw-r--r--   0        0        0     3589 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/deployment.yaml
+-rw-r--r--   0        0        0     1311 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/hpa.yaml
+-rw-r--r--   0        0        0     1647 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/ingress.yaml
+-rw-r--r--   0        0        0     1016 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/keda-autoscaler.yaml
+-rw-r--r--   0        0        0      542 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/service.yaml
+-rw-r--r--   0        0        0      384 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/serviceaccount.yaml
+-rw-r--r--   0        0        0      459 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/tests/test-connection.yaml
+-rw-r--r--   0        0        0      429 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrole.yaml
+-rw-r--r--   0        0        0      519 2023-08-27 04:24:41.037442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrolebinding.yaml
+-rw-r--r--   0        0        0      375 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/configmap.yaml
+-rw-r--r--   0        0        0     8408 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/deployment.yaml
+-rw-r--r--   0        0        0     1361 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/hpa.yaml
+-rw-r--r--   0        0        0     1692 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/ingress.yaml
+-rw-r--r--   0        0        0     1061 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/keda-autoscaler.yaml
+-rw-r--r--   0        0        0      487 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/service.yaml
+-rw-r--r--   0        0        0      404 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/serviceaccount.yaml
+-rw-r--r--   0        0        0      523 2024-03-07 06:21:41.696065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrole.yaml
+-rw-r--r--   0        0        0      759 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrolebinding.yaml
+-rw-r--r--   0        0        0      341 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/configmap.yaml
+-rw-r--r--   0        0        0     8528 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/deployment.yaml
+-rw-r--r--   0        0        0     1795 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/ingress.yaml
+-rw-r--r--   0        0        0      577 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/service.yaml
+-rw-r--r--   0        0        0      472 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/serviceaccount.yaml
+-rw-r--r--   0        0        0     1111 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/configmap.yaml
+-rw-r--r--   0        0        0     1683 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/ingress.yaml
+-rw-r--r--   0        0        0     1204 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/service.yaml
+-rw-r--r--   0        0        0      400 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/serviceaccount.yaml
+-rw-r--r--   0        0        0     9499 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/statefulset.yaml
+-rw-r--r--   0        0        0      546 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/tests/test-connection.yaml
+-rw-r--r--   0        0        0     3044 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-init.yaml
+-rw-r--r--   0        0        0     3088 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-upgrade.yaml
+-rw-r--r--   0        0        0      273 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/secrets-clickhouse-external.yaml
+-rw-r--r--   0        0        0    92137 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/values.yaml
+-rw-r--r--   0        0        0      972 2024-03-12 12:13:47.401181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_postgresql_helper.py
+-rw-r--r--   0        0        0      755 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_rabbitmq_helper.py
+-rw-r--r--   0        0        0     1052 2024-03-12 12:13:47.409181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_redpanda_helper.py
+-rw-r--r--   0        0        0      904 2024-03-12 12:13:47.421181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_signoz_helper.py
+-rw-r--r--   0        0        0       86 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/requirements.txt
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
+-rw-r--r--   0        0        0      556 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/template.env
+-rw-r--r--   0        0        0      330 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose-app.env
+-rw-r--r--   0        0        0     1238 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0    15205 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0       68 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/README.md
+-rw-r--r--   0        0        0     6411 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/README.md
+-rw-r--r--   0        0        0    81204 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-microservices.png
+-rw-r--r--   0        0        0    41834 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-monolith.png
+-rw-r--r--   0        0        0    40600 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp.png
+-rw-r--r--   0        0        0       17 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/.gitignore
+-rw-r--r--   0        0        0      870 2024-01-23 09:38:21.733760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/locustfile.py
+-rw-r--r--   0        0        0      495 2024-02-18 23:16:10.199317 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/template.env
+-rw-r--r--   0        0        0     2870 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-cluster.xml
+-rw-r--r--   0        0        0    55854 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-config.xml
+-rw-r--r--   0        0        0     1754 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-storage.xml
+-rw-r--r--   0        0        0     6258 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-users.xml
+-rw-r--r--   0        0        0      575 2023-08-27 04:24:41.041442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/custom-function.xml
+-rwxr-xr-x   0        0        0  1849156 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile
+-rw-r--r--   0        0        0     6986 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile.go
+-rw-r--r--   0        0        0     1475 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/frontend/nginx-config.conf
+-rw-r--r--   0        0        0     5284 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector/otel-collector-config.yaml
+-rw-r--r--   0        0        0     1548 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector-metrics/otel-collector-metrics-config.yaml
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/dashboards/.gitkeep
+-rw-r--r--   0        0        0        9 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/data/.gitignore
+-rw-r--r--   0        0        0      757 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/prometheus.yml
+-rw-r--r--   0        0        0      135 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.dockerignore
+-rw-r--r--   0        0        0       53 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.gitignore
+-rw-r--r--   0        0        0        7 2023-10-17 11:37:32.073861 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/.python-version
+-rw-r--r--   0        0        0      592 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/Dockerfile
+-rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.049442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/__init__.py
+-rw-r--r--   0        0        0     1949 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/error.py
+-rwxr-xr-x   0        0        0      801 2024-03-12 12:13:47.429181 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/__init__.py
+-rw-r--r--   0        0        0     6041 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/admin.py
+-rwxr-xr-x   0        0        0    10820 2024-03-12 12:13:47.509182 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/consumer.py
+-rwxr-xr-x   0        0        0     7090 2024-03-12 12:13:47.577182 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/publisher.py
+-rwxr-xr-x   0        0        0     1731 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/messagebus.py
+-rw-r--r--   0        0        0     1991 2024-03-12 12:13:47.597182 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/mock.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     5121 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/admin.py
+-rwxr-xr-x   0        0        0     6750 2024-03-12 12:13:47.657182 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/consumer.py
+-rwxr-xr-x   0        0        0     4525 2024-03-12 12:13:47.697183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/publisher.py
+-rw-r--r--   0        0        0       67 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/__init__.py
+-rw-r--r--   0        0        0     1744 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/repo_model.py
+-rw-r--r--   0        0        0      258 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/__init__.py
+-rw-r--r--   0        0        0      538 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_entity_mixin.py
+-rw-r--r--   0        0        0     9446 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_repo.py
+-rw-r--r--   0        0        0      932 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/repo.py
+-rw-r--r--   0        0        0      147 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/search_filter.py
+-rw-r--r--   0        0        0      244 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/__init__.py
+-rw-r--r--   0        0        0     3201 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/caller.py
+-rw-r--r--   0        0        0     2197 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/server.py
+-rw-r--r--   0        0        0     1625 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/rpc.py
+-rw-r--r--   0        0        0      127 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/schema/__init__.py
+-rw-r--r--   0        0        0      342 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/schema/base_schema.py
+-rw-r--r--   0        0        0      154 2024-03-12 12:13:47.697183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/__init__.py
+-rw-r--r--   0        0        0      854 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/serializer.py
+-rwxr-xr-x   0        0        0     4402 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/config.py
+-rw-r--r--   0        0        0      160 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.eslintignore
+-rw-r--r--   0        0        0      494 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      132 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.gitignore
+-rw-r--r--   0        0        0       19 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.npmrc
+-rw-r--r--   0        0        0      160 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.prettierignore
+-rw-r--r--   0        0        0      233 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/.prettierrc
+-rwxr-xr-x   0        0        0      944 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/README.md
+-rwxr-xr-x   0        0        0     1362 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/package.json
+-rwxr-xr-x   0        0        0      225 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/playwright.config.ts
+-rwxr-xr-x   0        0        0       80 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/postcss.config.js
+-rwxr-xr-x   0        0        0       58 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.css
+-rwxr-xr-x   0        0        0      241 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.d.ts
+-rwxr-xr-x   0        0        0      350 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/app.html
+-rwxr-xr-x   0        0        0      148 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/index.test.ts
+-rwxr-xr-x   0        0        0   130279 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/assets/logo.png
+-rwxr-xr-x   0        0        0     5281 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/helper.ts
+-rwxr-xr-x   0        0        0      125 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/store.ts
+-rwxr-xr-x   0        0        0      197 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/type.ts
+-rw-r--r--   0        0        0      608 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectDiv.svelte
+-rw-r--r--   0        0        0      361 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectUl.svelte
+-rw-r--r--   0        0        0     1906 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/input/arrayOfObjectCheckboxes.svelte
+-rw-r--r--   0        0        0      281 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/json/jsonView.svelte
+-rwxr-xr-x   0        0        0     1675 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Menu.svelte
+-rwxr-xr-x   0        0        0     4085 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Navigation.svelte
+-rwxr-xr-x   0        0        0      727 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/helper.ts
+-rwxr-xr-x   0        0        0      127 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/type.ts
+-rwxr-xr-x   0        0        0     1609 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/app.ts
+-rwxr-xr-x   0        0        0      648 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/navData.ts
+-rwxr-xr-x   0        0        0      350 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/error/helper.ts
+-rwxr-xr-x   0        0        0      291 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+error.svelte
+-rwxr-xr-x   0        0        0       65 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.js
+-rwxr-xr-x   0        0        0      584 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.svelte
+-rwxr-xr-x   0        0        0      489 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+page.svelte
+-rwxr-xr-x   0        0        0     6285 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/+page.svelte
+-rwxr-xr-x   0        0        0     3763 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.ts
+-rwxr-xr-x   0        0        0     2968 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.ts
+-rwxr-xr-x   0        0        0     4306 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/new/+page.svelte
+-rw-r--r--   0        0        0     5028 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.ts
+-rwxr-xr-x   0        0        0     6051 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/+page.svelte
+-rwxr-xr-x   0        0        0     3462 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.ts
+-rwxr-xr-x   0        0        0     2662 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.ts
+-rwxr-xr-x   0        0        0     2905 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/new/+page.svelte
+-rw-r--r--   0        0        0     3659 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.ts
+-rwxr-xr-x   0        0        0     6622 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/+page.svelte
+-rwxr-xr-x   0        0        0     4323 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.ts
+-rwxr-xr-x   0        0        0     3529 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.ts
+-rwxr-xr-x   0        0        0     6049 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/new/+page.svelte
+-rw-r--r--   0        0        0     6952 2023-08-27 04:24:41.053442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.ts
+-rwxr-xr-x   0        0        0     5409 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/+page.svelte
+-rwxr-xr-x   0        0        0     2941 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.ts
+-rwxr-xr-x   0        0        0     1321 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/favicon.png
+-rwxr-xr-x   0        0        0    12221 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/logo.png
+-rwxr-xr-x   0        0        0      317 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/svelte.config.js
+-rwxr-xr-x   0        0        0      203 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tailwind.config.js
+-rwxr-xr-x   0        0        0      224 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tests/test.ts
+-rwxr-xr-x   0        0        0      532 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tsconfig.json
+-rwxr-xr-x   0        0        0      210 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/vite.config.ts
+-rwxr-xr-x   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/__init__.py
+-rw-r--r--   0        0        0      490 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/async_task.py
+-rwxr-xr-x   0        0        0      763 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/conversion.py
+-rw-r--r--   0        0        0     1858 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/migration.py
+-rw-r--r--   0        0        0      103 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/value.py
+-rwxr-xr-x   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/__init__.py
+-rwxr-xr-x   0        0        0     3177 2024-03-12 12:13:47.741183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app.py
+-rw-r--r--   0        0        0     1389 2024-03-12 12:13:47.757183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_lifespan.py
+-rw-r--r--   0        0        0      870 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_state.py
+-rw-r--r--   0        0        0     1062 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/db_connection.py
+-rw-r--r--   0        0        0      322 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/frontend_index.py
+-rw-r--r--   0        0        0     1838 2024-03-12 12:13:47.769183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/log.py
+-rw-r--r--   0        0        0     3460 2024-03-12 12:13:47.813183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/messagebus.py
+-rw-r--r--   0        0        0     1410 2024-03-12 12:13:47.829183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/rpc.py
+-rwxr-xr-x   0        0        0      280 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/main.py
+-rw-r--r--   0        0        0      232 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/migrate.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/__init__.py
+-rw-r--r--   0        0        0      978 2024-03-12 12:13:47.837183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/api.py
+-rw-r--r--   0        0        0      907 2024-03-12 12:13:47.845183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/_init_.py
+-rw-r--r--   0        0        0     1204 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/scheme.py
+-rw-r--r--   0        0        0     2124 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/util.py
+-rw-r--r--   0        0        0      354 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/authorizer.py
+-rw-r--r--   0        0        0     1178 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/rpc_authorizer.py
+-rw-r--r--   0        0        0      446 2024-03-12 12:13:47.849183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/password_hasher/bcrypt_password_hasher.py
+-rw-r--r--   0        0        0      258 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/password_hasher/password_hasher.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/_init_.py
+-rw-r--r--   0        0        0     1674 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/util.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/__init__.py
+-rw-r--r--   0        0        0     5296 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/api.py
+-rw-r--r--   0        0        0      280 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/model.py
+-rw-r--r--   0        0        0     1283 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/repo.py
+-rw-r--r--   0        0        0     2331 2024-03-03 13:54:04.996858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/rpc.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/__init__.py
+-rw-r--r--   0        0        0     5510 2024-03-12 12:13:47.909183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/api.py
+-rw-r--r--   0        0        0      905 2024-03-12 12:13:47.921183 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/model.py
+-rw-r--r--   0        0        0     1134 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/repo.py
+-rw-r--r--   0        0        0     2554 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/rpc.py
+-rw-r--r--   0        0        0      661 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/table.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/__init__.py
+-rw-r--r--   0        0        0     7929 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/api.py
+-rw-r--r--   0        0        0     6582 2024-03-12 12:13:47.997184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/model.py
+-rw-r--r--   0        0        0     3175 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/repo.py
+-rw-r--r--   0        0        0     3612 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/rpc.py
+-rw-r--r--   0        0        0      279 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/event.py
+-rw-r--r--   0        0        0      777 2024-03-12 12:13:48.005184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/__init__.py
+-rw-r--r--   0        0        0      570 2024-03-12 12:13:48.013184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_scheme.py
+-rw-r--r--   0        0        0      560 2024-03-12 12:13:48.017184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_util.py
+-rw-r--r--   0        0        0      316 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/authorizer.py
+-rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/base.py
+-rw-r--r--   0        0        0      155 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/bearer_token_scheme.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/__init__.py
+-rw-r--r--   0        0        0      223 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/group_model.py
+-rw-r--r--   0        0        0      263 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/permission_model.py
+-rw-r--r--   0        0        0     1010 2024-03-12 12:13:48.025184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/user_model.py
+-rw-r--r--   0        0        0      129 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/password_hasher.py
+-rw-r--r--   0        0        0      568 2024-03-12 12:13:48.033184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/refresh_token_util.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/__init__.py
+-rw-r--r--   0        0        0      212 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/group_repo.py
+-rw-r--r--   0        0        0      242 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/permission_repo.py
+-rw-r--r--   0        0        0      313 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/repo/user_repo.py
+-rw-r--r--   0        0        0      805 2024-03-12 12:13:48.041184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/user.py
+-rw-r--r--   0        0        0      576 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/migrate.py
+-rw-r--r--   0        0        0     1154 2024-03-12 12:13:48.053184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_module.py
+-rw-r--r--   0        0        0     1322 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_permission.py
+-rw-r--r--   0        0        0      711 2024-03-12 12:13:48.081184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/rpc.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/__init__.py
+-rw-r--r--   0        0        0      461 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/group.py
+-rw-r--r--   0        0        0      337 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/permission.py
+-rw-r--r--   0        0        0      190 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/request.py
+-rw-r--r--   0        0        0      319 2024-01-23 09:38:21.737760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/token.py
+-rw-r--r--   0        0        0      697 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/user.py
+-rw-r--r--   0        0        0      518 2024-03-12 12:13:48.085184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/api.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/__init__.py
+-rw-r--r--   0        0        0     1612 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/historical_repo_model.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/__init__.py
+-rw-r--r--   0        0        0     2624 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/api.py
+-rw-r--r--   0        0        0      596 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/event.py
+-rw-r--r--   0        0        0      229 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/model.py
+-rw-r--r--   0        0        0      621 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/repo.py
+-rw-r--r--   0        0        0     2340 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/rpc.py
+-rw-r--r--   0        0        0      552 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/table.py
+-rw-r--r--   0        0        0      434 2024-03-12 12:13:48.101184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/event.py
+-rw-r--r--   0        0        0       58 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/base.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/model/__init__.py
+-rw-r--r--   0        0        0      189 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/model/activity_model.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/repo/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/integration/repo/activity_repo.py
+-rw-r--r--   0        0        0      429 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/migrate.py
+-rw-r--r--   0        0        0     1147 2024-03-12 12:13:48.113184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/register_module.py
+-rw-r--r--   0        0        0      445 2024-03-12 12:13:48.117184 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/rpc.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/schema/__init__.py
+-rw-r--r--   0        0        0      338 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/schema/activity.py
+-rw-r--r--   0        0        0     1000 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/schema/__init__.py
+-rw-r--r--   0        0        0      163 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/schema/frontend_config.py
+-rwxr-xr-x   0        0        0     1950 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/start.sh
+-rw-r--r--   0        0        0     1608 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/template.env
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/__init__.py
+-rw-r--r--   0        0        0     7724 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_group_crud.py
+-rw-r--r--   0        0        0     7782 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_permission_crud.py
+-rw-r--r--   0        0        0     8005 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_crud.py
+-rw-r--r--   0        0        0     8581 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_login.py
+-rw-r--r--   0        0        0      314 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/conftest.py
+-rw-r--r--   0        0        0      278 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/helper.py
+-rw-r--r--   0        0        0     1232 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/test_liveness_and_readiness.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.057442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/__init__.py
+-rw-r--r--   0        0        0     4870 2024-03-12 12:13:48.165185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/add.py
+-rw-r--r--   0        0        0     4057 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/helper.py
+-rw-r--r--   0        0        0       13 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/.gitignore
+-rw-r--r--   0        0        0    11259 2023-09-14 07:29:41.118392 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package-lock.json
+-rw-r--r--   0        0        0      369 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package.json
+-rw-r--r--   0        0        0     1460 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/addNav.ts
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/fastapp/src/frontend/src/lib/config/navData.ts
+-rw-r--r--   0        0        0    12289 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/tsconfig.json
+-rw-r--r--   0        0        0     1335 2024-03-12 12:13:48.177185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/task_factory.py
+-rwxr-xr-x   0        0        0     6304 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/+page.svelte
+-rwxr-xr-x   0        0        0     3517 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.ts
+-rwxr-xr-x   0        0        0     2683 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.ts
+-rwxr-xr-x   0        0        0     2911 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/new/+page.svelte
+-rw-r--r--   0        0        0     3673 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.svelte
+-rw-r--r--   0        0        0       85 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.ts
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/__init__.py
+-rw-r--r--   0        0        0     6838 2024-03-12 12:13:48.225185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/api.py
+-rw-r--r--   0        0        0      478 2024-03-12 12:13:48.229185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/model.py
+-rw-r--r--   0        0        0      780 2024-03-12 12:13:48.237185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/repo.py
+-rw-r--r--   0        0        0     2775 2024-03-12 12:13:48.265185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/rpc.py
+-rw-r--r--   0        0        0      403 2024-03-12 12:13:48.269185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/model/snake_zrb_entity_name_model.py
+-rw-r--r--   0        0        0      336 2024-03-12 12:13:48.273185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/repo/snake_zrb_entity_name_repo.py
+-rw-r--r--   0        0        0      388 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/schema/snake_zrb_entity_name.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/__init__.py
+-rw-r--r--   0        0        0     8206 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/test_snake_zrb_entity_name.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_field/__init__.py
+-rw-r--r--   0        0        0     6406 2024-03-12 12:13:48.337185 zrb-0.9.3/src/zrb/builtin/generator/fastapp_field/add.py
+-rw-r--r--   0        0        0    11041 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/fastapp_field/helper.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/__init__.py
+-rw-r--r--   0        0        0     4607 2024-03-12 12:13:48.401186 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/add.py
+-rw-r--r--   0        0        0    10945 2024-03-12 12:13:48.485186 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/helper.py
+-rw-r--r--   0        0        0      381 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/api.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/component/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/__init__.py
+-rw-r--r--   0        0        0      570 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/table.py
+-rw-r--r--   0        0        0      296 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/event.py
+-rw-r--r--   0        0        0       76 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/base.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/integration/repo/__init__.py
+-rw-r--r--   0        0        0      537 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/migrate.py
+-rw-r--r--   0        0        0     1273 2024-03-12 12:13:48.497186 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/register_module.py
+-rw-r--r--   0        0        0      313 2024-03-03 13:54:05.000858 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/rpc.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/schema/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/pip_package/__init__.py
+-rw-r--r--   0        0        0     3122 2024-03-12 12:13:48.521186 zrb-0.9.3/src/zrb/builtin/generator/pip_package/add.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/__init__.py
+-rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/activate-venv.sh
+-rw-r--r--   0        0        0       86 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/build.sh
+-rw-r--r--   0        0        0       37 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/install-symlink.sh
+-rw-r--r--   0        0        0       38 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/prepare-venv.sh
+-rw-r--r--   0        0        0       80 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/cmd/publish.sh
+-rw-r--r--   0        0        0     3131 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/local.py
+-rw-r--r--   0        0        0        6 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/.gitignore
+-rw-r--r--   0        0        0     1995 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/README.md
+-rw-r--r--   0        0        0      764 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/__init__.py
+-rw-r--r--   0        0        0       38 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/__main__.py
+-rw-r--r--   0        0        0       60 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/src/snake_zrb_package_name/util.py
+-rw-r--r--   0        0        0     2351 2024-03-12 12:13:48.541186 zrb-0.9.3/src/zrb/builtin/generator/plugin/create.py
+-rw-r--r--   0        0        0     1076 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/.github/workflows/_zrb.yml
+-rw-r--r--   0        0        0      218 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/.github/workflows/hello.yml
+-rw-r--r--   0        0        0       32 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/.gitignore
+-rw-r--r--   0        0        0        7 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/.python-version
+-rw-r--r--   0        0        0     2051 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/README.md
+-rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/_cmd/activate-venv.sh
+-rw-r--r--   0        0        0       86 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/_cmd/build.sh
+-rw-r--r--   0        0        0       37 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/_cmd/install-symlink.sh
+-rw-r--r--   0        0        0       38 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/_cmd/prepare-venv.sh
+-rw-r--r--   0        0        0       64 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/_cmd/publish.sh
+-rwxr-xr-x   0        0        0     1938 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/project.sh
+-rw-r--r--   0        0        0      763 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/__init__.py
+-rw-r--r--   0        0        0      121 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/__main__.py
+-rw-r--r--   0        0        0      325 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/src/snake_zrb_package_name/task/example_task.py
+-rw-r--r--   0        0        0      118 2023-12-25 09:04:52.769412 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/template.env
+-rw-r--r--   0        0        0     2459 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/plugin/template/zrb_init.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project/__init__.py
+-rw-r--r--   0        0        0     3303 2024-03-12 12:13:48.589187 zrb-0.9.3/src/zrb/builtin/generator/project/create.py
+-rw-r--r--   0        0        0       56 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project/template/.flake8
+-rw-r--r--   0        0        0     1081 2023-10-18 00:29:25.312347 zrb-0.9.3/src/zrb/builtin/generator/project/template/.github/workflows/_zrb.yml
+-rw-r--r--   0        0        0      218 2023-10-18 00:29:25.312347 zrb-0.9.3/src/zrb/builtin/generator/project/template/.github/workflows/hello.yml
+-rw-r--r--   0        0        0       27 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project/template/.gitignore
+-rw-r--r--   0        0        0        7 2023-10-12 00:54:12.983360 zrb-0.9.3/src/zrb/builtin/generator/project/template/.python-version
+-rw-r--r--   0        0        0     2026 2023-12-08 01:44:50.345704 zrb-0.9.3/src/zrb/builtin/generator/project/template/README.md
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project/template/_automate/__init__.py
+-rwxr-xr-x   0        0        0     1938 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/project/template/project.sh
+-rw-r--r--   0        0        0      520 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/project/template/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project/template/src/.gitkeep
+-rw-r--r--   0        0        0       64 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/project/template/template.env
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project/template/zrb_init.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/project_task/__init__.py
+-rw-r--r--   0        0        0     6083 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/task_factory.py
+-rw-r--r--   0        0        0      644 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/__init__.py
+-rw-r--r--   0        0        0      322 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/build_project_images.py
+-rw-r--r--   0        0        0      298 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/deploy_project.py
+-rw-r--r--   0        0        0      312 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/destroy_project.py
+-rw-r--r--   0        0        0      319 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/push_project_images.py
+-rw-r--r--   0        0        0      342 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/remove_project_containers.py
+-rw-r--r--   0        0        0      294 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project.py
+-rw-r--r--   0        0        0      333 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project_containers.py
+-rw-r--r--   0        0        0      334 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/stop_project_containers.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.061442 zrb-0.9.3/src/zrb/builtin/generator/python_task/__init__.py
+-rw-r--r--   0        0        0     1848 2024-03-12 12:13:48.605187 zrb-0.9.3/src/zrb/builtin/generator/python_task/add.py
+-rw-r--r--   0        0        0      765 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/python_task/template/_automate/snake_zrb_task_name.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/__init__.py
+-rw-r--r--   0        0        0     6515 2024-03-12 12:13:48.657187 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/add.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/__init__.py
+-rw-r--r--   0        0        0     1428 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/_common.py
+-rw-r--r--   0        0        0      334 2024-02-25 00:07:25.670566 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/app-activate-venv.sh
+-rw-r--r--   0        0        0      195 2024-02-18 23:16:10.203317 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/app-start.sh
+-rw-r--r--   0        0        0       29 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-destroy.sh
+-rw-r--r--   0        0        0      126 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-init-stack.sh
+-rw-r--r--   0        0        0       24 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/cmd/pulumi-up.sh
+-rw-r--r--   0        0        0     4836 2024-03-12 12:13:48.689187 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/container.py
+-rw-r--r--   0        0        0     3841 2024-03-12 12:13:48.717187 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/deployment.py
+-rw-r--r--   0        0        0     2235 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/image.py
+-rw-r--r--   0        0        0     1388 2024-03-12 12:13:48.729187 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/local.py
+-rw-r--r--   0        0        0       31 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/.gitignore
+-rw-r--r--   0        0        0       12 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/.gitignore
+-rw-r--r--   0        0        0      137 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
+-rw-r--r--   0        0        0     2633 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0       74 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/requirements.txt
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
+-rw-r--r--   0        0        0        0 2023-08-28 15:53:50.913810 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/template.env
+-rw-r--r--   0        0        0       68 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0      646 2023-10-12 00:54:12.983360 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0       22 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/.dockerignore
+-rw-r--r--   0        0        0       23 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/.gitignore
+-rw-r--r--   0        0        0      311 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/Dockerfile
+-rw-r--r--   0        0        0      511 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/main.py
+-rw-r--r--   0        0        0      568 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/template.env
+-rw-r--r--   0        0        0     3016 2024-02-25 11:35:16.468626 zrb-0.9.3/src/zrb/builtin/git.py
+-rw-r--r--   0        0        0     1168 2024-02-25 11:35:24.964664 zrb-0.9.3/src/zrb/builtin/group.py
+-rw-r--r--   0        0        0        0 2023-12-03 01:12:52.544398 zrb-0.9.3/src/zrb/builtin/helper/__init__.py
+-rw-r--r--   0        0        0     1940 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/helper/reccuring_action.py
+-rw-r--r--   0        0        0     1235 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/md5.py
+-rw-r--r--   0        0        0     1283 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/process.py
+-rw-r--r--   0        0        0     1195 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/project.py
+-rw-r--r--   0        0        0     3866 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/say.py
+-rw-r--r--   0        0        0      989 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/schedule.py
+-rw-r--r--   0        0        0     3087 2024-03-12 12:13:48.753187 zrb-0.9.3/src/zrb/builtin/ubuntu.py
+-rw-r--r--   0        0        0      397 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/update.py
+-rw-r--r--   0        0        0      478 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/version.py
+-rw-r--r--   0        0        0     1191 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/builtin/watch_changes.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/config/__init__.py
+-rw-r--r--   0        0        0     1170 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/config/config.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/accessories/__init__.py
+-rw-r--r--   0        0        0      805 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/helper/accessories/color.py
+-rw-r--r--   0        0        0      509 2024-01-23 09:38:21.741760 zrb-0.9.3/src/zrb/helper/accessories/icon.py
+-rw-r--r--   0        0        0     1477 2024-03-12 12:13:48.769187 zrb-0.9.3/src/zrb/helper/accessories/name.py
+-rw-r--r--   0        0        0      787 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/advertisement.py
+-rw-r--r--   0        0        0      231 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/callable.py
+-rw-r--r--   0        0        0     2050 2024-03-10 01:37:08.821171 zrb-0.9.3/src/zrb/helper/cli.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/codemod/__init__.py
+-rw-r--r--   0        0        0     1252 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_argument_to_function.py
+-rw-r--r--   0        0        0      998 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_argument_to_function_call.py
+-rw-r--r--   0        0        0      825 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_assert_resource.py
+-rw-r--r--   0        0        0     1036 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_function_call.py
+-rw-r--r--   0        0        0     3220 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_import_module.py
+-rw-r--r--   0        0        0     1583 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_key_value_to_dict.py
+-rw-r--r--   0        0        0     3459 2024-03-12 12:13:16.513037 zrb-0.9.3/src/zrb/helper/codemod/add_property_to_class.py
+-rw-r--r--   0        0        0     3191 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/add_upstream_to_task.py
+-rw-r--r--   0        0        0      933 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/append_code_to_function.py
+-rw-r--r--   0        0        0      147 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/codemod/format_code.py
+-rw-r--r--   0        0        0     2045 2024-03-10 01:36:55.389095 zrb-0.9.3/src/zrb/helper/default_env.py
+-rw-r--r--   0        0        0     2046 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/docker_compose/fetch_external_env.py
+-rw-r--r--   0        0        0      686 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/docker_compose/file.py
+-rw-r--r--   0        0        0     4815 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/docstring.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/env_map/__init__.py
+-rw-r--r--   0        0        0     2177 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/env_map/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/file/__init__.py
+-rw-r--r--   0        0        0     1729 2024-03-10 01:36:55.389095 zrb-0.9.3/src/zrb/helper/file/copy_tree.py
+-rw-r--r--   0        0        0      566 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/file/match.py
+-rw-r--r--   0        0        0      809 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/file/text.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/git/__init__.py
+-rw-r--r--   0        0        0     1150 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/git/detect_changes.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/loader/__init__.py
+-rw-r--r--   0        0        0     1757 2024-03-10 01:36:55.389095 zrb-0.9.3/src/zrb/helper/loader/load_module.py
+-rw-r--r--   0        0        0      517 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/log.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/map/__init__.py
+-rw-r--r--   0        0        0      444 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/map/conversion.py
+-rw-r--r--   0        0        0      245 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/python_task.py
+-rw-r--r--   0        0        0      679 2024-03-12 12:13:48.789188 zrb-0.9.3/src/zrb/helper/render_data.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/helper/string/__init__.py
+-rw-r--r--   0        0        0      112 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/string/constant.py
+-rw-r--r--   0        0        0     1431 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/string/conversion.py
+-rw-r--r--   0        0        0      330 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/string/jinja.py
+-rw-r--r--   0        0        0      144 2023-10-07 04:36:46.239224 zrb-0.9.3/src/zrb/helper/string/modification.py
+-rw-r--r--   0        0        0      291 2023-09-07 23:19:19.451089 zrb-0.9.3/src/zrb/helper/string/parse_replacement.py
+-rw-r--r--   0        0        0      402 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/typecheck.py
+-rw-r--r--   0        0        0      312 2024-03-12 12:13:48.793187 zrb-0.9.3/src/zrb/helper/typing.py
+-rw-r--r--   0        0        0     3545 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/helper/util.py
+-rw-r--r--   0        0        0      118 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/runner.py
+-rw-r--r--   0        0        0      229 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/shell-scripts/_common-util.sh
+-rw-r--r--   0        0        0     2999 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/shell-scripts/ensure-docker-is-installed.sh
+-rw-r--r--   0        0        0     1146 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/shell-scripts/ensure-rsync-is-installed.sh
+-rw-r--r--   0        0        0     2414 2024-03-07 06:21:41.700065 zrb-0.9.3/src/zrb/shell-scripts/ensure-ssh-is-installed.sh
+-rw-r--r--   0        0        0      843 2023-12-03 01:12:52.544398 zrb-0.9.3/src/zrb/shell-scripts/notify.ps1
+-rw-r--r--   0        0        0      353 2023-11-09 07:37:41.473343 zrb-0.9.3/src/zrb/shell-scripts/rsync-util.sh
+-rw-r--r--   0        0        0      401 2023-10-07 04:36:46.239224 zrb-0.9.3/src/zrb/shell-scripts/ssh-util.sh
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/task/__init__.py
+-rw-r--r--   0        0        0    36254 2024-03-12 12:13:48.893188 zrb-0.9.3/src/zrb/task/any_task.py
+-rw-r--r--   0        0        0      359 2023-10-21 14:01:33.314524 zrb-0.9.3/src/zrb/task/any_task_event_handler.py
+-rw-r--r--   0        0        0     9220 2024-03-12 12:13:48.973188 zrb-0.9.3/src/zrb/task/base_remote_cmd_task.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:25:11.701393 zrb-0.9.3/src/zrb/task/base_task/__init__.py
+-rw-r--r--   0        0        0    17502 2024-03-12 12:13:49.141189 zrb-0.9.3/src/zrb/task/base_task/base_task.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:25:11.701393 zrb-0.9.3/src/zrb/task/base_task/component/__init__.py
+-rw-r--r--   0        0        0    10300 2024-03-12 12:13:49.245190 zrb-0.9.3/src/zrb/task/base_task/component/base_task_model.py
+-rw-r--r--   0        0        0    11275 2024-03-12 12:13:49.369190 zrb-0.9.3/src/zrb/task/base_task/component/common_task_model.py
+-rw-r--r--   0        0        0      292 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/task/base_task/component/pid_model.py
+-rw-r--r--   0        0        0     4439 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/task/base_task/component/renderer.py
+-rw-r--r--   0        0        0     1950 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/task/base_task/component/trackers.py
+-rw-r--r--   0        0        0     3117 2024-03-12 12:13:49.397190 zrb-0.9.3/src/zrb/task/checker.py
+-rw-r--r--   0        0        0    13890 2024-03-12 12:13:49.553191 zrb-0.9.3/src/zrb/task/cmd_task.py
+-rw-r--r--   0        0        0     2887 2024-03-12 12:13:49.577191 zrb-0.9.3/src/zrb/task/decorator.py
+-rw-r--r--   0        0        0    14017 2024-03-12 12:13:49.697192 zrb-0.9.3/src/zrb/task/docker_compose_task.py
+-rw-r--r--   0        0        0     4639 2024-03-12 12:13:49.761192 zrb-0.9.3/src/zrb/task/flow_task.py
+-rw-r--r--   0        0        0     5172 2024-03-12 12:13:49.817192 zrb-0.9.3/src/zrb/task/http_checker.py
+-rw-r--r--   0        0        0     5986 2024-03-12 12:13:49.869192 zrb-0.9.3/src/zrb/task/notifier.py
+-rw-r--r--   0        0        0     1042 2024-01-23 09:38:21.745760 zrb-0.9.3/src/zrb/task/parallel.py
+-rw-r--r--   0        0        0     4153 2024-03-12 12:13:49.909193 zrb-0.9.3/src/zrb/task/path_checker.py
+-rw-r--r--   0        0        0     6268 2024-03-12 12:13:50.001193 zrb-0.9.3/src/zrb/task/path_watcher.py
+-rw-r--r--   0        0        0     4072 2024-03-12 12:13:50.093194 zrb-0.9.3/src/zrb/task/port_checker.py
+-rw-r--r--   0        0        0     7133 2024-03-12 12:13:50.153194 zrb-0.9.3/src/zrb/task/recurring_task.py
+-rw-r--r--   0        0        0     3709 2024-03-12 12:13:50.189194 zrb-0.9.3/src/zrb/task/remote_cmd_task.py
+-rw-r--r--   0        0        0     6576 2024-03-12 12:13:50.257194 zrb-0.9.3/src/zrb/task/resource_maker.py
+-rw-r--r--   0        0        0     3949 2024-03-12 12:13:50.309195 zrb-0.9.3/src/zrb/task/rsync_task.py
+-rw-r--r--   0        0        0      182 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task/task.py
+-rw-r--r--   0        0        0     3908 2024-03-12 12:13:50.345195 zrb-0.9.3/src/zrb/task/time_watcher.py
+-rw-r--r--   0        0        0       44 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_env/constant.py
+-rw-r--r--   0        0        0     4766 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_env/env.py
+-rw-r--r--   0        0        0     2932 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_env/env_file.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/task_group/__init__.py
+-rw-r--r--   0        0        0     5937 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_group/group.py
+-rw-r--r--   0        0        0        0 2023-08-27 04:24:41.065442 zrb-0.9.3/src/zrb/task_input/__init__.py
+-rw-r--r--   0        0        0     1909 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/any_input.py
+-rw-r--r--   0        0        0     5484 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/base_input.py
+-rw-r--r--   0        0        0     3881 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/bool_input.py
+-rw-r--r--   0        0        0     4129 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/choice_input.py
+-rw-r--r--   0        0        0       42 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/constant.py
+-rw-r--r--   0        0        0     3962 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/float_input.py
+-rw-r--r--   0        0        0     4040 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/int_input.py
+-rw-r--r--   0        0        0     4029 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/password_input.py
+-rw-r--r--   0        0        0     4042 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/str_input.py
+-rw-r--r--   0        0        0     2022 2024-01-23 09:38:21.749760 zrb-0.9.3/src/zrb/task_input/task_input.py
+-rw-r--r--   0        0        0    16500 1970-01-01 00:00:00.000000 zrb-0.9.3/PKG-INFO
```

### Comparing `zrb-0.9.2/LICENSE` & `zrb-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/README.md` & `zrb-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/pyproject.toml` & `zrb-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zrb"
-version = "0.9.2"
+version = "0.9.3"
 description = "A Framework to Enhance Your Workflow"
 authors = ["Go Frendi Gunawan <gofrendiasgard@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/state-alchemists/zrb"
 repository = "https://github.com/state-alchemists/zrb"
 documentation = "https://github.com/state-alchemists/zrb"
```

### Comparing `zrb-0.9.2/src/zrb/__init__.py` & `zrb-0.9.3/src/zrb/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/action/runner.py` & `zrb-0.9.3/src/zrb/action/runner.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/advertisement.py` & `zrb-0.9.3/src/zrb/advertisement.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/base64.py` & `zrb-0.9.3/src/zrb/builtin/base64.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/__init__.py` & `zrb-0.9.3/src/zrb/builtin/devtool/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/aws/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/aws/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/devtool_install.py` & `zrb-0.9.3/src/zrb/builtin/devtool/devtool_install.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/docker/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/docker/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/gcloud/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/gcloud/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/gvm/finalize.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/gvm/finalize.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/helix/install-language-server.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/helix/install-language-server.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/helix/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/helix/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/nvm/finalize.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/nvm/finalize.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/pyenv/download.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/pyenv/download.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/pyenv/finalize.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/pyenv/finalize.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/selenium/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/selenium/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/tmux/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/tmux/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/zsh/install.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/zsh/install.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/devtool/zsh/resource/config.sh` & `zrb-0.9.3/src/zrb/builtin/devtool/zsh/resource/config.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/docker.py` & `zrb-0.9.3/src/zrb/builtin/docker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/env.py` & `zrb-0.9.3/src/zrb/builtin/env.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/eval.py` & `zrb-0.9.3/src/zrb/builtin/eval.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/explain.py` & `zrb-0.9.3/src/zrb/builtin/explain.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/__init__.py` & `zrb-0.9.3/src/zrb/builtin/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/base/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/_common.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/container.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/deployment.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/image.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/main.go` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/src/main.go`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/http-port-build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/http-port-build-custom-image/_automate/generate_snake_zrb_meta_template_name/template/_automate/snake_zrb_app_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/__main__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/app_generator/template/use-helm/_automate/generate_snake_zrb_meta_template_name/template/src/kebab-zrb-app-name/deployment/helm-charts/kebab-zrb-app-name/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/cmd_task/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/cmd_task/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/common/helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/common/helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/common/task_factory.py` & `zrb-0.9.3/src/zrb/builtin/generator/common/task_factory.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/common/task_input.py` & `zrb-0.9.3/src/zrb/builtin/generator/common/task_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/_automate/snake_zrb_task_name.py` & `zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/_automate/snake_zrb_task_name.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.yml` & `zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-zrb-task-name/image/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,31 @@
         "zrbAppHttpLogPort": '{{util.coalesce(input.http_port, "3001") + 2}}',
     },
     template_path=os.path.join(CURRENT_DIR, "template"),
     destination_path="{{ input.project_dir }}",
     excludes=[
         "*/__pycache__",
         "*/deployment/venv",
-        "*/src/kebab-app-name/.venv",
-        "*/src/kebab-app-name/src/frontend/node_modules",
-        "*/src/kebab-app-name/src/frontend/build",
-        "*/src/kebab-app-name/src/frontend/.svelte-kit",
-        "*/src/kebab-app-name/monitoring/clickhouse",
+        "*/src/kebab-zrb-app-name/.venv",
+        "*/src/kebab-zrb-app-name/src/frontend/node_modules",
+        "*/src/kebab-zrb-app-name/src/frontend/build",
+        "*/src/kebab-zrb-app-name/src/frontend/.svelte-kit",
+    ],
+    skip_parsing=[
+        "*.mp3",
+        "*.pdf",
+        "*.exe",
+        "*.dll",
+        "*.bin",
+        "*.iso",
+        "*.png",
+        "*.jpg",
+        "*.gif",
+        "*.ico",
+        "*/monitoring/clickhouse/user_scripts/histogramQuantile",
     ],
 )
 
 register_local_module = create_register_module(
     module_path=f"_automate.{SNAKE_APP_NAME_TPL}.local",
     alias=f"{SNAKE_APP_NAME_TPL}_local",
     inputs=[app_name_input],
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_checker.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_checker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_config.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_config.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env_file.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_env_file.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_get_start_microservices.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_get_start_microservices.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_input.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/container.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/container.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/deployment.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/deployment.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/frontend.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/frontend.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/image.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/image.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/load_test.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/load_test.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/test.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/_automate/snake_zrb_app_name/test.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/__main__.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/__main__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/_common.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/_common.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/app_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/app_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_affinities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_capabilities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_compatibility.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_compatibility.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_errors.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_images.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_ingress.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_labels.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_names.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_resources.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_resources.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_secrets.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_storage.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_tplvalues.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_tplvalues.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_utils.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_warnings.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_cassandra.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mariadb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mongodb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mysql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_postgresql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_redis.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_validations.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/cronjob.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/cronjob.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/pvc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/backup/pvc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/extended-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/initialization-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/initialization-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/primary/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/prometheusrule.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/extended-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/read/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/templates/tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.schema.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/postgresql/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_affinities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_capabilities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_compatibility.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_compatibility.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_errors.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_images.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_ingress.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_labels.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_names.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_resources.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_resources.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_secrets.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_storage.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_tplvalues.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_tplvalues.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_utils.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_warnings.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_cassandra.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mariadb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mongodb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mysql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_postgresql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_redis.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_validations.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/config-secret.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/config-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress-tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress-tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/init-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/init-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/pdb.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/pdb.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/prometheusrule.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/templates/tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.schema.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/rabbitmq/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/LICENSE` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/LICENSE`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/LICENSE` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/LICENSE`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/01-default-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/01-default-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/02-broker-tls-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/ci/02-broker-tls-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/pod-monitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/pod-monitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/tests/01-mm2-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/templates/tests/01-mm2-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/connectors/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/examples/console-enterprise.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/examples/console-enterprise.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/secret.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/tests/test-connection.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/templates/tests/test-connection.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.schema.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/charts/console/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/01-default-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/01-default-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/02-one-node-cluster-no-tls-no-sasl-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/02-one-node-cluster-no-tls-no-sasl-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/03-one-node-cluster-tls-no-sasl-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/03-one-node-cluster-tls-no-sasl-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/04-one-node-cluster-no-tls-sasl-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/04-one-node-cluster-no-tls-sasl-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/05-one-node-cluster-tls-sasl-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/05-one-node-cluster-tls-sasl-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/06-rack-awareness-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/06-rack-awareness-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/07-multiple-listeners-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/07-multiple-listeners-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/08-custom-podantiaffinity-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/08-custom-podantiaffinity-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/09-initcontainers-resources-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/09-initcontainers-resources-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/10-external-addresses-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/10-external-addresses-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/11-update-sasl-users-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/11-update-sasl-users-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/12-external-cert-secrets-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/12-external-cert-secrets-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/13-loadbalancer-tls-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/13-loadbalancer-tls-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/14-prometheus-no-tls-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/14-prometheus-no-tls-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/15-prometheus-tls-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/15-prometheus-tls-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/16-controller-sidecar-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/16-controller-sidecar-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/17-resources-without-unit-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/17-resources-without-unit-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/18-single-external-address-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/18-single-external-address-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/21-eks-tiered-storage-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/21-eks-tiered-storage-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/22-gke-tiered-storage-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/22-gke-tiered-storage-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/23-aks-tiered-storage-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/23-aks-tiered-storage-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/24-eks-tiered-storage-persistent-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/24-eks-tiered-storage-persistent-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/25-gke-tiered-storage-persistent-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/25-gke-tiered-storage-persistent-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/26-aks-tiered-storage-persistent-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/26-aks-tiered-storage-persistent-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/27-eks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/27-eks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/28-gke-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/28-gke-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/29-aks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/29-aks-tiered-storage-persistent-nameoverwrite-with-creds-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/96-audit-logging-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/96-audit-logging-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/97-license-key-values.yaml.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/97-license-key-values.yaml.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/98-license-secret-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/98-license-secret-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/99-none-existent-config-options-with-empty-values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/ci/99-none-existent-config-options-with-empty-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_configmap.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_configmap.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_example-commands.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_example-commands.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_job.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_job.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_statefulset.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_statefulset.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_tplvalues.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/_tplvalues.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/cert-issuers.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/cert-issuers.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/certs.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/certs.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/connectors/connectors.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/connectors/connectors.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/console/configmap-and-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/console/configmap-and-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/poddisruptionbudget.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-install-upgrade-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-install-upgrade-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-upgrade.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/post-upgrade.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/rbac.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/rbac.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.internal.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.internal.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.loadbalancer.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/service.loadbalancer.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/services.nodeport.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/services.nodeport.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-api-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-api-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-auditLogging.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-auditLogging.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-connector-via-console.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-connector-via-console.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-console.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-console.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-internal-external-tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-internal-external-tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-internal-tls-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-internal-tls-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-nodelete.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-nodelete.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-produce-consume.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-produce-consume.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-sasl-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-sasl-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-license-with-console.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-license-with-console.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-lifecycle-scripts.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-lifecycle-scripts.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-loadbalancer-tls.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-loadbalancer-tls.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-nodeport-tls.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-nodeport-tls.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-internal-tls-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-internal-tls-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-prometheus-targets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-prometheus-targets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rack-awareness.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rack-awareness.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rpk-debug-bundle.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-rpk-debug-bundle.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-sasl-updated.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-sasl-updated.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-internal-tls-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-internal-tls-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-status.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-status.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.schema.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/redpanda/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.lock` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.lock`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-rbac.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-rbac.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/crds.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/crds.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/rbac.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/rbac.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-rbac.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-rbac.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-config.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-config.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-mutating-webhook.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-mutating-webhook.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-rbac.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-rbac.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-validating-webhook.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-validating-webhook.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/cert-manager/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_affinities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_capabilities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_errors.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_images.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_ingress.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_labels.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_names.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_secrets.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_storage.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_utils.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_warnings.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_cassandra.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mariadb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mongodb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mysql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_postgresql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_redis.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_validations.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/metrics-svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/pdb.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/pdb.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/prometheusrule.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/scripts-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/scripts-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallations.clickhouse.altinity.com.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallations.clickhouse.altinity.com.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallationtemplates.clickhouse.altinity.com.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallationtemplates.clickhouse.altinity.com.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseoperatorconfigurations.clickhouse.altinity.com.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseoperatorconfigurations.clickhouse.altinity.com.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/_helper.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/_helper.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/clickhouse-instance.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/clickhouse-instance.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/storage-class.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/storage-class.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-configd-files.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-configd-files.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-files.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-files.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-templatesd-files.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-templatesd-files.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-usersd-files.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-usersd-files.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/clickhouse/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/CHANGELOG.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md.gotmpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_params.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_params.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-createSecret.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-createSecret.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-patchWebhook.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-patchWebhook.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/validating-webhook.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/validating-webhook.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-proxyheaders.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-proxyheaders.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-tcp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-tcp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-udp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-udp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-daemonset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-ingressclass.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-ingressclass.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-keda.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-keda.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-poddisruptionbudget.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-prometheusrules.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-prometheusrules.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-internal.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-internal.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-metrics.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-metrics.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-webhook.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-webhook.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-poddisruptionbudget.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_config.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_config.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/daemonset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/daemonset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/tests/test-connection.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/tests/test-connection.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/tests/test-connection.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/tests/test-connection.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/tls-secret.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/tls-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/k8s-infra/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_affinities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_capabilities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_errors.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_images.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_ingress.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_labels.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_names.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_secrets.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_storage.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_utils.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_warnings.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_cassandra.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mariadb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mongodb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mysql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_postgresql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_redis.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_validations.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/Chart.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_affinities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_capabilities.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_errors.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_images.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_ingress.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_labels.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_names.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_secrets.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_storage.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_utils.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_warnings.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_cassandra.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mariadb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mongodb.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mysql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_postgresql.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_redis.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_validations.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/networkpolicy-egress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/networkpolicy-egress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/extended-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/initialization-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/initialization-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/prometheusrule.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/psp.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/extended-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc-headless.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/tls-secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.schema.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap-env-vars.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap-env-vars.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/headless-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/headless-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/init-scripts-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/init-scripts-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/metrics-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/metrics-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/pdb.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/pdb.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/prometheusrule.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/role.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/rolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/serviceaccount.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/tls-secret.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/tls-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/keycloak/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_bucket.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_bucket.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_policy.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_policy.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_user.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_user.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_custom_command.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_custom_command.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/gateway-deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/gateway-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/networkpolicy.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-bucket-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-bucket-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-policy-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-policy-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-user-job.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-user-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-custom-command.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-custom-command.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/pvc.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/pvc.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/secrets.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/securitycontextconstraints.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/securitycontextconstraints.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/servicemonitor.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/templates/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/charts/minio/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/NOTES.txt` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_clickhouse.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_clickhouse.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_helpers.tpl` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/services.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/services.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/alertmanager/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/cert-issuer.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/cert-issuer.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/keda-autoscaler.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/keda-autoscaler.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/frontend/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/hpa.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/keda-autoscaler.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector/keda-autoscaler.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrole.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrolebinding.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/deployment.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/configmap.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/ingress.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/service.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/service.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/statefulset.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/tests/test-connection.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/query-service/tests/test-connection.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-init.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-init.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-upgrade.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/templates/schema-migrator/migrations-upgrade.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/values.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm-charts/signoz/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_postgresql_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_postgresql_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_rabbitmq_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_rabbitmq_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_redpanda_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_redpanda_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_signoz_helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/helm_signoz_helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/template.env` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/deployment/template.env`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.env` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.env`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.yml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-microservices.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-microservices.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-monolith.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp-monolith.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/docs/modular-monolith/images/fastapp.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/locustfile.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/loadtest/locustfile.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-cluster.xml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-cluster.xml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-config.xml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-config.xml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-storage.xml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-storage.xml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-users.xml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/clickhouse-users.xml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/custom-function.xml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/custom-function.xml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile.go` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/clickhouse/user_scripts/histogramQuantile.go`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/frontend/nginx-config.conf` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/frontend/nginx-config.conf`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector/otel-collector-config.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector/otel-collector-config.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector-metrics/otel-collector-metrics-config.yaml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/otel-collector-metrics/otel-collector-metrics-config.yaml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/prometheus.yml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/monitoring/query-service/prometheus.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/Dockerfile` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 COPY frontend .
 RUN npm install --save-dev && npm run build
 
 # Second stage: build the API and copy the frontend build
 FROM python:3.10-slim
 ENV APP_HOST 0.0.0.0
 ENV APP_PORT 8080
+ENV POETRY_VIRTUAL_ENVS_CREATE=false
 WORKDIR /home
 RUN apt update && apt install curl psmisc -y
 RUN pip install -U pip
 RUN pip install "poetry==1.7.1"
 COPY ./pyproject.toml ./pyproject.toml
 RUN poetry install --only main --no-root
 COPY . .
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/error.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/error.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/__init__.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/admin.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/admin.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/consumer.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/publisher.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/kafka/publisher.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/messagebus.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/messagebus.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/mock.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/mock.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/admin.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/admin.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/consumer.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/publisher.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/messagebus/rabbitmq/publisher.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/repo_model.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/model/repo_model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_entity_mixin.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_entity_mixin.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/db_repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/repo/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/caller.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/caller.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/server.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/messagebus/server.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/serializer.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/component/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/config.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 app_logging_level = str_to_logging_level(os.getenv("APP_LOGGING_LEVEL", "INFO"))
 app_host = os.getenv("APP_HOST", "0.0.0.0")
 app_port = int(os.getenv("APP_PORT", "8080"))
 app_reload = str_to_boolean(os.getenv("APP_RELOAD", "true"))
 app_max_not_ready = int(os.getenv("APP_MAX_NOT_READY", "10"))
 
 app_enable_otel = str_to_boolean(os.getenv("APP_ENABLE_OTEL", "false"))
-app_otel_exporter_otlp_endpoint = os.getenv("APP_OTEL_EXPORTER_OTLP_ENDPOINT", "false")
+app_otel_exporter_otlp_endpoint = os.getenv(
+    "APP_OTEL_EXPORTER_OTLP_ENDPOINT", "http://localhost:4317"
+)
 
 app_auth_access_token_cookie_key = os.getenv(
     "PUBLIC_AUTH_ACCESS_TOKEN_COOKIE_KEY", "access_token"
 )
 app_auth_refresh_token_cookie_key = os.getenv(
     "PUBLIC_AUTH_REFRESH_TOKEN_COOKIE_KEY", "refresh_token"
 )
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/package.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/package.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/assets/logo.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/assets/logo.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/helper.ts` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/auth/helper.ts`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectDiv.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectDiv.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/input/arrayOfObjectCheckboxes.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/arrayOfObject/input/arrayOfObjectCheckboxes.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Menu.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Menu.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Navigation.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/Navigation.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/helper.ts` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/components/navigation/helper.ts`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/app.ts` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/app.ts`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/navData.ts` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/lib/config/navData.ts`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/+layout.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/new/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/new/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/new/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/new/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/new/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/new/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/favicon.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/favicon.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/logo.png` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/static/logo.png`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tsconfig.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/conversion.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/conversion.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/migration.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/helper/migration.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_lifespan.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_lifespan.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_state.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/app_state.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/db_connection.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/db_connection.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/log.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/log.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/messagebus.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/messagebus.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/integration/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/api.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/__init__.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/scheme.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/scheme.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/util.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/access_token/util.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/rpc_authorizer.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/authorizer/rpc_authorizer.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/util.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/component/refresh_token/util.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from component.messagebus import Publisher
 from component.rpc import Caller
 from fastapi import Depends, FastAPI
 from module.auth.component import Authorizer
 from module.auth.integration import access_token_scheme
 from module.auth.schema.group import Group, GroupData, GroupResult
 from module.auth.schema.token import AccessTokenData
+from opentelemetry import trace
+
+tracer = trace.get_tracer(__name__)
 
 
 def register_api(
     logger: Logger,
     app: FastAPI,
     authorizer: Authorizer,
     rpc_caller: Caller,
@@ -22,96 +25,108 @@
     @app.get("/api/v1/auth/groups", response_model=GroupResult)
     async def get_groups(
         keyword: str = "",
         limit: int = 100,
         offset: int = 0,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:get"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:get"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_get_group",
-                keyword=keyword,
-                criterion={},
-                limit=limit,
-                offset=offset,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return GroupResult(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_get_group"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_group",
+                    keyword=keyword,
+                    criterion={},
+                    limit=limit,
+                    offset=offset,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return GroupResult(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.get("/api/v1/auth/groups/{id}", response_model=Group)
     async def get_group_by_id(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:group:get_by_id"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:group:get_by_id"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_get_group_by_id",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Group(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_get_group_by_id"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_group_by_id",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Group(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post("/api/v1/auth/groups", response_model=Group)
     async def insert_group(
         data: GroupData, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:group:insert"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:group:insert"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_insert_group",
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Group(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_insert_group"):
+                result_dict = await rpc_caller.call(
+                    "auth_insert_group",
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Group(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.put("/api/v1/auth/groups/{id}", response_model=Group)
     async def update_group(
         id: str,
         data: GroupData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:group:update"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:group:update"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_update_group",
-                id=id,
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Group(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_update_group"):
+                result_dict = await rpc_caller.call(
+                    "auth_update_group",
+                    id=id,
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Group(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.delete("/api/v1/auth/groups/{id}", response_model=Group)
     async def delete_group(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:group:delete"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:group:delete"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_delete_group", id=id, user_token_data=user_token_data.model_dump()
-            )
-            return Group(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_delete_group"):
+                result_dict = await rpc_caller.call(
+                    "auth_delete_group",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Group(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/group/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from component.messagebus import Publisher
 from component.rpc import Caller
 from fastapi import Depends, FastAPI
 from module.auth.component import Authorizer
 from module.auth.integration import access_token_scheme
 from module.auth.schema.permission import Permission, PermissionData, PermissionResult
 from module.auth.schema.token import AccessTokenData
+from opentelemetry import trace
+
+tracer = trace.get_tracer(__name__)
 
 
 def register_api(
     logger: Logger,
     app: FastAPI,
     authorizer: Authorizer,
     rpc_caller: Caller,
@@ -22,99 +25,109 @@
     @app.get("/api/v1/auth/permissions", response_model=PermissionResult)
     async def get_permissions(
         keyword: str = "",
         limit: int = 100,
         offset: int = 0,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:get"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:get"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_get_permission",
-                keyword=keyword,
-                criterion={},
-                limit=limit,
-                offset=offset,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PermissionResult(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_get_permission"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_permission",
+                    keyword=keyword,
+                    criterion={},
+                    limit=limit,
+                    offset=offset,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PermissionResult(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.get("/api/v1/auth/permissions/{id}", response_model=Permission)
     async def get_permission_by_id(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:get_by_id"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:get_by_id"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_get_permission_by_id",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Permission(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_get_permission_by_id"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_permission_by_id",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Permission(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post("/api/v1/auth/permissions", response_model=Permission)
     async def insert_permission(
         data: PermissionData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:insert"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:insert"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_insert_permission",
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Permission(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_insert_permission"):
+                result_dict = await rpc_caller.call(
+                    "auth_insert_permission",
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Permission(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.put("/api/v1/auth/permissions/{id}", response_model=Permission)
     async def update_permission(
         id: str,
         data: PermissionData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:update"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:update"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_update_permission",
-                id=id,
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Permission(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_update_permission"):
+                result_dict = await rpc_caller.call(
+                    "auth_update_permission",
+                    id=id,
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Permission(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.delete("/api/v1/auth/permissions/{id}", response_model=Permission)
     async def delete_permission(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:permission:delete"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:permission:delete"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "auth_delete_permission",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Permission(**result_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_delete_permission"):
+                result_dict = await rpc_caller.call(
+                    "auth_delete_permission",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Permission(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/model.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/permission/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/table.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/table.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from fastapi import Depends, FastAPI
 from fastapi.security import OAuth2PasswordRequestForm
 from module.auth.component import Authorizer
 from module.auth.integration import access_token_scheme, bearer_token_scheme
 from module.auth.schema.request import IsAuthorizedRequest, RefreshTokenRequest
 from module.auth.schema.token import AccessTokenData, TokenResponse
 from module.auth.schema.user import User, UserData, UserLogin, UserResult
+from opentelemetry import trace
+
+tracer = trace.get_tracer(__name__)
 
 
 def register_auth_api(
     logger: Logger,
     app: FastAPI,
     authorizer: Authorizer,
     rpc_caller: Caller,
@@ -31,47 +34,50 @@
 
     @app.post("/api/v1/auth/login", response_model=TokenResponse)
     async def login(data: UserLogin) -> TokenResponse:
         return await _create_token(data=data)
 
     async def _create_token(data: UserLogin) -> TokenResponse:
         try:
-            token_response_dict = await rpc_caller.call(
-                "auth_create_token", login_data=data.model_dump()
-            )
-            return TokenResponse(**token_response_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_create_token"):
+                token_response_dict = await rpc_caller.call(
+                    "auth_create_token", login_data=data.model_dump()
+                )
+                return TokenResponse(**token_response_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post("/api/v1/auth/refresh-token", response_model=TokenResponse)
     async def refresh_token(
         data: RefreshTokenRequest, refresh_token: str = Depends(bearer_token_scheme)
     ) -> TokenResponse:
         try:
-            token_response_dict = await rpc_caller.call(
-                "auth_refresh_token",
-                refresh_token=refresh_token,
-                access_token=data.access_token,
-            )
-            return TokenResponse(**token_response_dict)
+            with tracer.start_as_current_span("auth.rpc.auth_refresh_token"):
+                token_response_dict = await rpc_caller.call(
+                    "auth_refresh_token",
+                    refresh_token=refresh_token,
+                    access_token=data.access_token,
+                )
+                return TokenResponse(**token_response_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post("/api/v1/auth/is-authorized", response_model=Mapping[str, bool])
     async def is_authorized(
         data: IsAuthorizedRequest,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ) -> Mapping[str, str]:
         try:
             user_id = user_token_data.user_id
-            return await rpc_caller.call(
-                "auth_is_user_authorized",
-                id=user_id,
-                permission_name=data.permission_names,
-            )
+            with tracer.start_as_current_span("auth.rpc.auth_is_user_authorized"):
+                return await rpc_caller.call(
+                    "auth_is_user_authorized",
+                    id=user_id,
+                    permission_name=data.permission_names,
+                )
         except Exception as e:
             raise HTTPAPIException(error=e)
 
 
 def register_api(
     logger: Logger,
     app: FastAPI,
@@ -84,96 +90,108 @@
     @app.get("/api/v1/auth/users", response_model=UserResult)
     async def get_users(
         keyword: str = "",
         limit: int = 100,
         offset: int = 0,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:user:get"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
-        try:
-            result_dict = await rpc_caller.call(
-                "auth_get_user",
-                keyword=keyword,
-                criterion={},
-                limit=limit,
-                offset=offset,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return UserResult(**result_dict)
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:user:get"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
+        try:
+            with tracer.start_as_current_span("auth.rpc.auth_get_user"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_user",
+                    keyword=keyword,
+                    criterion={},
+                    limit=limit,
+                    offset=offset,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return UserResult(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.get("/api/v1/auth/users/{id}", response_model=User)
     async def get_user_by_id(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:user:get_by_id"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
-        try:
-            result_dict = await rpc_caller.call(
-                "auth_get_user_by_id",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return User(**result_dict)
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:user:get_by_id"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
+        try:
+            with tracer.start_as_current_span("auth.rpc.auth_get_user_by_id"):
+                result_dict = await rpc_caller.call(
+                    "auth_get_user_by_id",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return User(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post("/api/v1/auth/users", response_model=User)
     async def insert_user(
         data: UserData, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:user:insert"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
-        try:
-            result_dict = await rpc_caller.call(
-                "auth_insert_user",
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return User(**result_dict)
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:user:insert"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
+        try:
+            with tracer.start_as_current_span("auth.rpc.auth_insert_user"):
+                result_dict = await rpc_caller.call(
+                    "auth_insert_user",
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return User(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.put("/api/v1/auth/users/{id}", response_model=User)
     async def update_user(
         id: str,
         data: UserData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:user:update"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
-        try:
-            result_dict = await rpc_caller.call(
-                "auth_update_user",
-                id=id,
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return User(**result_dict)
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:user:update"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
+        try:
+            with tracer.start_as_current_span("auth.rpc.auth_update_user"):
+                result_dict = await rpc_caller.call(
+                    "auth_update_user",
+                    id=id,
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return User(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.delete("/api/v1/auth/users/{id}", response_model=User)
     async def delete_user(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "auth:user:delete"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
-        try:
-            result_dict = await rpc_caller.call(
-                "auth_delete_user", id=id, user_token_data=user_token_data.model_dump()
-            )
-            return User(**result_dict)
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "auth:user:delete"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
+        try:
+            with tracer.start_as_current_span("auth.rpc.auth_delete_user"):
+                result_dict = await rpc_caller.call(
+                    "auth_delete_user",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return User(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/model.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/entity/user/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/__init__.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_scheme.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_scheme.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_util.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/access_token_util.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/user_model.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/model/user_model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/refresh_token_util.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/refresh_token_util.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/user.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/integration/user.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/migrate.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/migrate.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_module.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_permission.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/register_permission.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/user.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/auth/schema/user.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/api.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/historical_repo_model.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/component/historical_repo_model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from component.messagebus import Publisher
 from component.rpc import Caller
 from fastapi import Depends, FastAPI
 from module.auth.component import Authorizer
 from module.auth.integration import access_token_scheme
 from module.auth.schema.token import AccessTokenData
 from module.log.schema.activity import Activity, ActivityResult
+from opentelemetry import trace
+
+tracer = trace.get_tracer(__name__)
 
 
 def register_api(
     logger: Logger,
     app: FastAPI,
     authorizer: Authorizer,
     rpc_caller: Caller,
@@ -22,41 +25,45 @@
     @app.get("/api/v1/log/activities", response_model=ActivityResult)
     async def get_activitys(
         keyword: str = "",
         limit: int = 100,
         offset: int = 0,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "log:activity:get"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "log:activity:get"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "log_get_activity",
-                keyword=keyword,
-                criterion={},
-                limit=limit,
-                offset=offset,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return ActivityResult(**result_dict)
+            with tracer.start_as_current_span("log.rpc.log_get_activity"):
+                result_dict = await rpc_caller.call(
+                    "log_get_activity",
+                    keyword=keyword,
+                    criterion={},
+                    limit=limit,
+                    offset=offset,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return ActivityResult(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.get("/api/v1/log/activities/{id}", response_model=Activity)
     async def get_activity_by_id(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "log:activity:get_by_id"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id, "log:activity:get_by_id"
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "log_get_activity_by_id",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return Activity(**result_dict)
+            with tracer.start_as_current_span("log.rpc.log_get_activity_by_id"):
+                result_dict = await rpc_caller.call(
+                    "log_get_activity_by_id",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return Activity(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/event.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,11 +9,9 @@
 
 def register_event(
     logger: Logger, consumer: Consumer, rpc_caller: Caller, publisher: Publisher
 ):
     logger.info('🥪 Register event handlers for "log.activity"')
 
     @consumer.register("log_new_activity")
-    async def insert(
-        data: Mapping[str, Any],
-    ):
+    async def insert(data: Mapping[str, Any]):
         await activity_model.insert(data=ActivityData(**data))
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/activity/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/table.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/entity/table.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/register_module.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/module/log/register_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/start.sh` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/start.sh`

 * *Files 22% similar despite different names*

```diff
@@ -35,24 +35,29 @@
     APP_OTEL_EXPORTER_OTLP_ENDPOINT="http://localhost:4317"
 fi
 
 ##############################################################################
 # Start kebab-zrb-app-name
 ##############################################################################
 
+# Reload option can only be used when APP_ENABLE_OTEL is false
+_RELOAD=""
+if [ $(_to_boolean "$APP_ENABLE_OTEL") = "false" ] && [ $(_to_boolean "$APP_RELOAD") = "true" ]
+then
+    _RELOAD="--reload"
+fi
+
+# Constructing otel command
+# See: https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/fastapi/fastapi.html#installation
+_OTEL_COMMAND=""
 if [ $(_to_boolean "$APP_ENABLE_OTEL") = "true" ]
 then
-    echo "Start uvicorn with instrumentation, service name: ${APP_NAME}"
-    OTEL_RESOURCE_ATTRIBUTES="service.name=${APP_NAME}" \
-        OTEL_EXPORTER_OTLP_ENDPOINT="$APP_OTEL_EXPORTER_OTLP_ENDPOINT" \
-        poetry run opentelemetry-instrument uvicorn main:app --host "$APP_HOST" --port "$APP_PORT"
-else
-    # reload should only performed if otel is disabled
-    _RELOAD=""
-    if [ $(_to_boolean "$APP_RELOAD") = "true" ]
-    then
-        _RELOAD="--reload"
-    fi
-    # Run uvicorn
-    echo "Start uvicorn"
-    poetry run uvicorn main:app --host "$APP_HOST" --port "$APP_PORT" $_RELOAD
-fi
+    export OTEL_RESOURCE_ATTRIBUTES="service.name=${APP_NAME}"
+    export OTEL_EXPORTER_OTLP_ENDPOINT="$APP_OTEL_EXPORTER_OTLP_ENDPOINT"
+    export OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST=".*"
+    export OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_RESPONSE=".*"
+    _OTEL_COMMAND="opentelemetry-instrument"
+fi
+
+# Run uvicorn
+echo "Start uvicorn"
+poetry run $_OTEL_COMMAND uvicorn main:app --host "$APP_HOST" --port "$APP_PORT" $_RELOAD
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/template.env` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/src/template.env`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_group_crud.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_group_crud.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_permission_crud.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_permission_crud.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_crud.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_crud.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_login.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/auth/test_user_login.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/test_liveness_and_readiness.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp/template/src/kebab-zrb-app-name/test/test_liveness_and_readiness.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package-lock.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package-lock.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/addNav.ts` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/addNav.ts`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/tsconfig.json` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/tsconfig.json`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/task_factory.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/task_factory.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/delete/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/detail/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/new/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/new/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.svelte` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/frontend/src/routes/kebab-zrb-module-name/kebab-zrb-entity-name/update/[id]/+page.svelte`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/api.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from module.auth.integration import access_token_scheme
 from module.auth.schema.token import AccessTokenData
 from module.snake_zrb_module_name.schema.snake_zrb_entity_name import (
     PascalZrbEntityName,
     PascalZrbEntityNameData,
     PascalZrbEntityNameResult,
 )
+from opentelemetry import trace
+
+tracer = trace.get_tracer(__name__)
 
 
 def register_api(
     logger: Logger,
     app: FastAPI,
     authorizer: Authorizer,
     rpc_caller: Caller,
@@ -29,115 +32,136 @@
     )
     async def get_snake_zrb_entity_names(
         keyword: str = "",
         limit: int = 100,
         offset: int = 0,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id, "snake_zrb_module_name:snake_zrb_entity_name:get"
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id,
+                "snake_zrb_module_name:snake_zrb_entity_name:get",
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "snake_zrb_module_name_get_snake_zrb_entity_name",
-                keyword=keyword,
-                criterion={},
-                limit=limit,
-                offset=offset,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PascalZrbEntityNameResult(**result_dict)
+            with tracer.start_as_current_span(
+                "snake_zrb_module_name.rpc.snake_zrb_module_name_get_snake_zrb_entity_name"  # noqa
+            ):
+                result_dict = await rpc_caller.call(
+                    "snake_zrb_module_name_get_snake_zrb_entity_name",
+                    keyword=keyword,
+                    criterion={},
+                    limit=limit,
+                    offset=offset,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PascalZrbEntityNameResult(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.get(
         "/api/v1/kebab-zrb-module-name/kebab-zrb-plural-entity-name/{id}",
         response_model=PascalZrbEntityName,
     )
     async def get_snake_zrb_entity_name_by_id(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id,
-            "snake_zrb_module_name:snake_zrb_entity_name:get_by_id",
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id,
+                "snake_zrb_module_name:snake_zrb_entity_name:get_by_id",
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "snake_zrb_module_name_get_snake_zrb_entity_name_by_id",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PascalZrbEntityName(**result_dict)
+            with tracer.start_as_current_span(
+                "snake_zrb_module_name.rpc.snake_zrb_module_name_get_snake_zrb_entity_name_by_id"  # noqa
+            ):
+                result_dict = await rpc_caller.call(
+                    "snake_zrb_module_name_get_snake_zrb_entity_name_by_id",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PascalZrbEntityName(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.post(
         "/api/v1/kebab-zrb-module-name/kebab-zrb-plural-entity-name",
         response_model=PascalZrbEntityName,
     )
     async def insert_snake_zrb_entity_name(
         data: PascalZrbEntityNameData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id,
-            "snake_zrb_module_name:snake_zrb_entity_name:insert",
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id,
+                "snake_zrb_module_name:snake_zrb_entity_name:insert",
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "snake_zrb_module_name_insert_snake_zrb_entity_name",
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PascalZrbEntityName(**result_dict)
+            with tracer.start_as_current_span(
+                "snake_zrb_module_name.rpc.snake_zrb_module_name_insert_snake_zrb_entity_name"  # noqa
+            ):
+                result_dict = await rpc_caller.call(
+                    "snake_zrb_module_name_insert_snake_zrb_entity_name",
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PascalZrbEntityName(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.put(
         "/api/v1/kebab-zrb-module-name/kebab-zrb-plural-entity-name/{id}",
         response_model=PascalZrbEntityName,
     )
     async def update_snake_zrb_entity_name(
         id: str,
         data: PascalZrbEntityNameData,
         user_token_data: AccessTokenData = Depends(access_token_scheme),
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id,
-            "snake_zrb_module_name:snake_zrb_entity_name:update",
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id,
+                "snake_zrb_module_name:snake_zrb_entity_name:update",
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "snake_zrb_module_name_update_snake_zrb_entity_name",
-                id=id,
-                data=data.model_dump(),
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PascalZrbEntityName(**result_dict)
+            with tracer.start_as_current_span(
+                "snake_zrb_module_name.rpc.snake_zrb_module_name_update_snake_zrb_entity_name"  # noqa
+            ):
+                result_dict = await rpc_caller.call(
+                    "snake_zrb_module_name_update_snake_zrb_entity_name",
+                    id=id,
+                    data=data.model_dump(),
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PascalZrbEntityName(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
 
     @app.delete(
         "/api/v1/kebab-zrb-module-name/kebab-zrb-plural-entity-name/{id}",
         response_model=PascalZrbEntityName,
     )
     async def delete_snake_zrb_entity_name(
         id: str, user_token_data: AccessTokenData = Depends(access_token_scheme)
     ):
-        if not await authorizer.is_having_permission(
-            user_token_data.user_id,
-            "snake_zrb_module_name:snake_zrb_entity_name:delete",
-        ):
-            raise HTTPAPIException(403, "Unauthorized")
+        with tracer.start_as_current_span("authorizer.is_having_permission"):
+            if not await authorizer.is_having_permission(
+                user_token_data.user_id,
+                "snake_zrb_module_name:snake_zrb_entity_name:delete",
+            ):
+                raise HTTPAPIException(403, "Unauthorized")
         try:
-            result_dict = await rpc_caller.call(
-                "snake_zrb_module_name_delete_snake_zrb_entity_name",
-                id=id,
-                user_token_data=user_token_data.model_dump(),
-            )
-            return PascalZrbEntityName(**result_dict)
+            with tracer.start_as_current_span(
+                "snake_zrb_module_name.rpc.snake_zrb_module_name_delete_snake_zrb_entity_name"  # noqa
+            ):
+                result_dict = await rpc_caller.call(
+                    "snake_zrb_module_name_delete_snake_zrb_entity_name",
+                    id=id,
+                    user_token_data=user_token_data.model_dump(),
+                )
+                return PascalZrbEntityName(**result_dict)
         except Exception as e:
             raise HTTPAPIException(error=e)
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/repo.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/repo.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/rpc.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/snake_zrb_entity_name/rpc.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/test_snake_zrb_entity_name.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-zrb-app-name/test/snake_zrb_module_name/test_snake_zrb_entity_name.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_field/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_field/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_field/helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_field/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     task.print_out(f"Read code from: {schema_file_path}")
     code = await read_text_file_async(schema_file_path)
     task.print_out(f'Add column "{snake_column_name}" to the schema')
     code = add_property_to_class(
         code=code,
         class_name=f"{pascal_entity_name}Data",
         property_name=snake_column_name,
-        property_type="str",
+        property_type="Optional[str]",
     )
     task.print_out(f"Write modified code to: {schema_file_path}")
     await write_text_file_async(schema_file_path, code)
 
 
 @typechecked
 async def add_column_to_repo(
```

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/helper.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/helper.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/table.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/entity/table.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/migrate.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/migrate.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/register_module.py` & `zrb-0.9.3/src/zrb/builtin/generator/fastapp_module/template/src/kebab-zrb-app-name/src/module/snake_zrb_module_name/register_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/pip_package/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/pip_package/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/_automate/snake_zrb_package_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/pip_package/template/src/kebab-zrb-package-name/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/create.py` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/create.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/template/.github/workflows/_zrb.yml` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/template/.github/workflows/_zrb.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/template/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/template/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/template/project.sh` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/template/project.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/template/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/plugin/template/zrb_init.py` & `zrb-0.9.3/src/zrb/builtin/generator/plugin/template/zrb_init.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project/create.py` & `zrb-0.9.3/src/zrb/builtin/generator/project/create.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project/template/.github/workflows/_zrb.yml` & `zrb-0.9.3/src/zrb/builtin/generator/project/template/.github/workflows/_zrb.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project/template/README.md` & `zrb-0.9.3/src/zrb/builtin/generator/project/template/README.md`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project/template/project.sh` & `zrb-0.9.3/src/zrb/builtin/generator/project/template/project.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project/template/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/project/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project_task/task_factory.py` & `zrb-0.9.3/src/zrb/builtin/generator/project_task/task_factory.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/project_task/template/_automate/_project/__init__.py` & `zrb-0.9.3/src/zrb/builtin/generator/project_task/template/_automate/_project/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/python_task/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/python_task/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/python_task/template/_automate/snake_zrb_task_name.py` & `zrb-0.9.3/src/zrb/builtin/generator/python_task/template/_automate/snake_zrb_task_name.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/add.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/add.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/_common.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/_common.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/container.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/container.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/deployment.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/deployment.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/image.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/image.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/local.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_zrb_app_name/local.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/__main__.py` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/deployment/__main__.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.yml` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/pyproject.toml` & `zrb-0.9.3/src/zrb/builtin/generator/simple_python_app/template/src/kebab-zrb-app-name/src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/git.py` & `zrb-0.9.3/src/zrb/builtin/git.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/group.py` & `zrb-0.9.3/src/zrb/builtin/group.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/helper/reccuring_action.py` & `zrb-0.9.3/src/zrb/builtin/helper/reccuring_action.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/md5.py` & `zrb-0.9.3/src/zrb/builtin/md5.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/process.py` & `zrb-0.9.3/src/zrb/builtin/process.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/project.py` & `zrb-0.9.3/src/zrb/builtin/project.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/say.py` & `zrb-0.9.3/src/zrb/builtin/say.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/schedule.py` & `zrb-0.9.3/src/zrb/builtin/schedule.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/ubuntu.py` & `zrb-0.9.3/src/zrb/builtin/ubuntu.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/builtin/watch_changes.py` & `zrb-0.9.3/src/zrb/builtin/watch_changes.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/config/config.py` & `zrb-0.9.3/src/zrb/config/config.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/accessories/color.py` & `zrb-0.9.3/src/zrb/helper/accessories/color.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/advertisement.py` & `zrb-0.9.3/src/zrb/helper/advertisement.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/cli.py` & `zrb-0.9.3/src/zrb/helper/cli.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_argument_to_function.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_argument_to_function.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_argument_to_function_call.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_argument_to_function_call.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_assert_resource.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_assert_resource.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_function_call.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_function_call.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_import_module.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_import_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_key_value_to_dict.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_key_value_to_dict.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_property_to_class.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_property_to_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,26 +61,43 @@
     class_name: str,
     property_name: str,
     property_type: str,
     property_value: Optional[str] = None,
 ) -> str:
     module = cst.parse_module(code)
     property_name_node = cst.Name(value=property_name)
-    property_type_node = cst.Annotation(cst.Name(value=property_type))
+    property_type_node = _get_property_type_node(property_type)
     property_value_node = _get_property_value_node(property_value)
     transformed_module = module.visit(
         AddPropertyTransformer(
             class_name=class_name,
             property_name_node=property_name_node,
             property_type_node=property_type_node,
             property_value_node=property_value_node,
         )
     )
     return transformed_module.code
 
 
+def _get_property_type_node(property_type: str) -> cst.Annotation:
+    if property_type.startswith("Optional[") and property_type.endswith("]"):
+        inner_type = property_type[len("Optional[") : -1]
+        return cst.Annotation(
+            annotation=cst.Subscript(
+                value=cst.Name("Optional"),
+                slice=[
+                    cst.SubscriptElement(
+                        slice=cst.Index(value=cst.Name(value=inner_type))
+                    )
+                ],
+            )
+        )
+    else:
+        return cst.Annotation(cst.Name(value=property_type))
+
+
 def _get_property_value_node(
     property_value: Optional[str],
 ) -> Optional[cst.BaseExpression]:
     if property_value is None:
         return None
     return cst.parse_expression(property_value)
```

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/add_upstream_to_task.py` & `zrb-0.9.3/src/zrb/helper/codemod/add_upstream_to_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/codemod/append_code_to_function.py` & `zrb-0.9.3/src/zrb/helper/codemod/append_code_to_function.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/default_env.py` & `zrb-0.9.3/src/zrb/helper/default_env.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/docker_compose/fetch_external_env.py` & `zrb-0.9.3/src/zrb/helper/docker_compose/fetch_external_env.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/docker_compose/file.py` & `zrb-0.9.3/src/zrb/helper/docker_compose/file.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/docstring.py` & `zrb-0.9.3/src/zrb/helper/docstring.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/env_map/fetch.py` & `zrb-0.9.3/src/zrb/helper/env_map/fetch.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/file/copy_tree.py` & `zrb-0.9.3/src/zrb/helper/file/copy_tree.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/file/match.py` & `zrb-0.9.3/src/zrb/helper/file/match.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/file/text.py` & `zrb-0.9.3/src/zrb/helper/file/text.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/git/detect_changes.py` & `zrb-0.9.3/src/zrb/helper/git/detect_changes.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/loader/load_module.py` & `zrb-0.9.3/src/zrb/helper/loader/load_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/log.py` & `zrb-0.9.3/src/zrb/helper/log.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/render_data.py` & `zrb-0.9.3/src/zrb/helper/render_data.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/string/conversion.py` & `zrb-0.9.3/src/zrb/helper/string/conversion.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/helper/util.py` & `zrb-0.9.3/src/zrb/helper/util.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/shell-scripts/ensure-docker-is-installed.sh` & `zrb-0.9.3/src/zrb/shell-scripts/ensure-docker-is-installed.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/shell-scripts/ensure-rsync-is-installed.sh` & `zrb-0.9.3/src/zrb/shell-scripts/ensure-rsync-is-installed.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/shell-scripts/ensure-ssh-is-installed.sh` & `zrb-0.9.3/src/zrb/shell-scripts/ensure-ssh-is-installed.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/shell-scripts/notify.ps1` & `zrb-0.9.3/src/zrb/shell-scripts/notify.ps1`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/any_task.py` & `zrb-0.9.3/src/zrb/task/any_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_remote_cmd_task.py` & `zrb-0.9.3/src/zrb/task/base_remote_cmd_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_task/base_task.py` & `zrb-0.9.3/src/zrb/task/base_task/base_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_task/component/base_task_model.py` & `zrb-0.9.3/src/zrb/task/base_task/component/base_task_model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_task/component/common_task_model.py` & `zrb-0.9.3/src/zrb/task/base_task/component/common_task_model.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_task/component/renderer.py` & `zrb-0.9.3/src/zrb/task/base_task/component/renderer.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/base_task/component/trackers.py` & `zrb-0.9.3/src/zrb/task/base_task/component/trackers.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/checker.py` & `zrb-0.9.3/src/zrb/task/checker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/cmd_task.py` & `zrb-0.9.3/src/zrb/task/cmd_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/decorator.py` & `zrb-0.9.3/src/zrb/task/decorator.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/docker_compose_task.py` & `zrb-0.9.3/src/zrb/task/docker_compose_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/flow_task.py` & `zrb-0.9.3/src/zrb/task/flow_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/http_checker.py` & `zrb-0.9.3/src/zrb/task/http_checker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/notifier.py` & `zrb-0.9.3/src/zrb/task/notifier.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/parallel.py` & `zrb-0.9.3/src/zrb/task/parallel.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/path_checker.py` & `zrb-0.9.3/src/zrb/task/path_checker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/path_watcher.py` & `zrb-0.9.3/src/zrb/task/path_watcher.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/port_checker.py` & `zrb-0.9.3/src/zrb/task/port_checker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/recurring_task.py` & `zrb-0.9.3/src/zrb/task/recurring_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/remote_cmd_task.py` & `zrb-0.9.3/src/zrb/task/remote_cmd_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/resource_maker.py` & `zrb-0.9.3/src/zrb/task/resource_maker.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/rsync_task.py` & `zrb-0.9.3/src/zrb/task/rsync_task.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task/time_watcher.py` & `zrb-0.9.3/src/zrb/task/time_watcher.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_env/env.py` & `zrb-0.9.3/src/zrb/task_env/env.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_env/env_file.py` & `zrb-0.9.3/src/zrb/task_env/env_file.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_group/group.py` & `zrb-0.9.3/src/zrb/task_group/group.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/any_input.py` & `zrb-0.9.3/src/zrb/task_input/any_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/base_input.py` & `zrb-0.9.3/src/zrb/task_input/base_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/bool_input.py` & `zrb-0.9.3/src/zrb/task_input/bool_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/choice_input.py` & `zrb-0.9.3/src/zrb/task_input/choice_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/float_input.py` & `zrb-0.9.3/src/zrb/task_input/float_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/int_input.py` & `zrb-0.9.3/src/zrb/task_input/int_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/password_input.py` & `zrb-0.9.3/src/zrb/task_input/password_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/str_input.py` & `zrb-0.9.3/src/zrb/task_input/str_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/src/zrb/task_input/task_input.py` & `zrb-0.9.3/src/zrb/task_input/task_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.9.2/PKG-INFO` & `zrb-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrb
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Framework to Enhance Your Workflow
 Home-page: https://github.com/state-alchemists/zrb
 License: AGPL-3.0-or-later
 Keywords: Automation,Task Runner,Code Generator,Low Code
 Author: Go Frendi Gunawan
 Author-email: gofrendiasgard@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
```

