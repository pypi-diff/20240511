# Comparing `tmp/unicorn_donkey-3.2.2.dev20240510222739.tar.gz` & `tmp/unicorn_donkey-3.2.2.dev20240510233735.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn_donkey-3.2.2.dev20240510222739.tar", max compression
+gzip compressed data, was "unicorn_donkey-3.2.2.dev20240510233735.tar", max compression
```

## Comparing `unicorn_donkey-3.2.2.dev20240510222739.tar` & `unicorn_donkey-3.2.2.dev20240510233735.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    11356 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/LICENSE.txt
--rw-r--r--   0        0        0    15790 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/README.md
--rw-r--r--   0        0        0      394 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/__init__.py
--rw-r--r--   0        0        0        5 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/__version__
--rw-r--r--   0        0        0      199 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/config.py
--rw-r--r--   0        0        0     4258 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/openapi.py
--rw-r--r--   0        0        0      934 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/pinecone_config.py
--rw-r--r--   0        0        0       30 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/control/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/control/index_host_store.py
--rw-r--r--   0        0        0    24671 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/control/pinecone.py
--rw-r--r--   0        0        0        0 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/__init__.py
--rw-r--r--   0        0        0      912 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/__init__.py
--rw-r--r--   0        0        0      226 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/__init__.py
--rw-r--r--   0        0        0    44181 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/data_plane_api.py
--rw-r--r--   0        0        0     5335 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/inference_api.py
--rw-r--r--   0        0        0    42855 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/manage_indexes_api.py
--rw-r--r--   0        0        0    37047 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api_client.py
--rw-r--r--   0        0        0     1037 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17126 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/configuration.py
--rw-r--r--   0        0        0     5275 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/__init__.py
--rw-r--r--   0        0        0    11438 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/collection_list.py
--rw-r--r--   0        0        0    13037 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/collection_model.py
--rw-r--r--   0        0        0    11532 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request.py
--rw-r--r--   0        0        0    11555 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request_spec.py
--rw-r--r--   0        0        0    12268 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request_spec_pod.py
--rw-r--r--   0        0        0    12068 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0        0        0    13960 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/create_index_request.py
--rw-r--r--   0        0        0    12890 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/delete_request.py
--rw-r--r--   0        0        0    11727 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0        0        0    12928 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0        0        0    11474 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embedding.py
--rw-r--r--   0        0        0    11176 2024-05-10 22:18:31.648514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_inputs.py
--rw-r--r--   0        0        0    11918 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_list.py
--rw-r--r--   0        0        0    11225 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_list_usage.py
--rw-r--r--   0        0        0    11962 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_parameters.py
--rw-r--r--   0        0        0    11779 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/error_response.py
--rw-r--r--   0        0        0    11913 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0        0        0    11368 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_list.py
--rw-r--r--   0        0        0    14023 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model.py
--rw-r--r--   0        0        0    11700 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model_spec.py
--rw-r--r--   0        0        0    11830 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model_status.py
--rw-r--r--   0        0        0    12075 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11791 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_response400.py
--rw-r--r--   0        0        0    12846 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_response400_error.py
--rw-r--r--   0        0        0    11140 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/list_item.py
--rw-r--r--   0        0        0    12236 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/list_response.py
--rw-r--r--   0        0        0    11545 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0        0        0    11156 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pagination.py
--rw-r--r--   0        0        0    14771 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pod_spec.py
--rw-r--r--   0        0        0    11500 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pod_spec_metadata_config.py
--rw-r--r--   0        0        0    11361 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0        0        0    12278 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0        0        0    15454 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_request.py
--rw-r--r--   0        0        0    12556 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_response.py
--rw-r--r--   0        0        0    13173 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_vector.py
--rw-r--r--   0        0        0    11744 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0        0        0    12977 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0        0        0    12098 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/serverless_spec.py
--rw-r--r--   0        0        0    11734 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0        0        0    11536 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0        0        0    12781 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/update_request.py
--rw-r--r--   0        0        0    11921 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0        0        0    11283 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0        0        0    11278 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/usage.py
--rw-r--r--   0        0        0    12592 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/vector.py
--rw-r--r--   0        0        0    80542 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model_utils.py
--rw-r--r--   0        0        0     4002 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/models/__init__.py
--rw-r--r--   0        0        0    14209 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/rest.py
--rw-r--r--   0        0        0    76084 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0        0        0    24258 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2.pyi
--rw-r--r--   0        0        0    14276 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0      291 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/__init__.py
--rw-r--r--   0        0        0     2125 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/errors.py
--rw-r--r--   0        0        0    27458 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/index.py
--rw-r--r--   0        0        0     1730 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/sparse_vector_factory.py
--rw-r--r--   0        0        0     2815 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/vector_factory.py
--rw-r--r--   0        0        0     4027 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/deprecation_warnings.py
--rw-r--r--   0        0        0     1033 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/exceptions.py
--rw-r--r--   0        0        0     1300 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/__init__.py
--rw-r--r--   0        0        0     5875 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/base.py
--rw-r--r--   0        0        0     1728 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/config.py
--rw-r--r--   0        0        0      961 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/future.py
--rw-r--r--   0        0        0    28020 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/index_grpc.py
--rw-r--r--   0        0        0     4166 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/pinecone.py
--rw-r--r--   0        0        0     3193 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/retry.py
--rw-r--r--   0        0        0     2000 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/sparse_values_factory.py
--rw-r--r--   0        0        0     2996 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/utils.py
--rw-r--r--   0        0        0     3841 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/vector_factory_grpc.py
--rw-r--r--   0        0        0        0 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/inference/__init__.py
--rw-r--r--   0        0        0      839 2024-05-10 22:18:31.652514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/inference/build_parameters_dict_for_inference.py
--rw-r--r--   0        0        0     3726 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/inference/embeddings.py
--rw-r--r--   0        0        0      600 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/__init__.py
--rw-r--r--   0        0        0      277 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/collection_description.py
--rw-r--r--   0        0        0      852 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/collection_list.py
--rw-r--r--   0        0        0      765 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/embeddings_list.py
--rw-r--r--   0        0        0     1330 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/index_description.py
--rw-r--r--   0        0        0      718 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/index_list.py
--rw-r--r--   0        0        0      198 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/list_response.py
--rw-r--r--   0        0        0     2189 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/pod_spec.py
--rw-r--r--   0        0        0      164 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/serverless_spec.py
--rw-r--r--   0        0        0      348 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/__init__.py
--rw-r--r--   0        0        0      288 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/check_kwargs.py
--rw-r--r--   0        0        0      722 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/constants.py
--rw-r--r--   0        0        0      785 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/convert_to_list.py
--rw-r--r--   0        0        0      263 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/deprecation_notice.py
--rw-r--r--   0        0        0      750 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/error_handling.py
--rw-r--r--   0        0        0      193 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/fix_tuple_length.py
--rw-r--r--   0        0        0      206 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/normalize_host.py
--rw-r--r--   0        0        0      527 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/setup_openapi_client.py
--rw-r--r--   0        0        0     1011 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/user_agent.py
--rw-r--r--   0        0        0      157 2024-05-10 22:18:31.656514 unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/version.py
--rw-r--r--   0        0        0     3312 2024-05-10 22:27:40.111386 unicorn_donkey-3.2.2.dev20240510222739/pyproject.toml
--rw-r--r--   0        0        0    17921 1970-01-01 00:00:00.000000 unicorn_donkey-3.2.2.dev20240510222739/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-10 23:28:37.394439 unicorn_donkey-3.2.2.dev20240510233735/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-05-10 23:37:36.395760 unicorn_donkey-3.2.2.dev20240510233735/README.md
+-rw-r--r--   0        0        0      394 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/__init__.py
+-rw-r--r--   0        0        0        5 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/__version__
+-rw-r--r--   0        0        0      199 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/config.py
+-rw-r--r--   0        0        0     4258 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/openapi.py
+-rw-r--r--   0        0        0      934 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/pinecone_config.py
+-rw-r--r--   0        0        0       30 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/control/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/control/index_host_store.py
+-rw-r--r--   0        0        0    24671 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/control/pinecone.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/__init__.py
+-rw-r--r--   0        0        0      912 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/__init__.py
+-rw-r--r--   0        0        0    44181 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/data_plane_api.py
+-rw-r--r--   0        0        0     5335 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/inference_api.py
+-rw-r--r--   0        0        0    42855 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/manage_indexes_api.py
+-rw-r--r--   0        0        0    37047 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api_client.py
+-rw-r--r--   0        0        0     1037 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17126 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/configuration.py
+-rw-r--r--   0        0        0     5275 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11438 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/collection_list.py
+-rw-r--r--   0        0        0    13037 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/collection_model.py
+-rw-r--r--   0        0        0    11532 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request.py
+-rw-r--r--   0        0        0    11555 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request_spec.py
+-rw-r--r--   0        0        0    12268 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request_spec_pod.py
+-rw-r--r--   0        0        0    12068 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0        0        0    13960 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/create_index_request.py
+-rw-r--r--   0        0        0    12890 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0        0        0    11727 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0        0        0    12928 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0        0        0    11474 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embedding.py
+-rw-r--r--   0        0        0    11176 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_inputs.py
+-rw-r--r--   0        0        0    11918 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_list.py
+-rw-r--r--   0        0        0    11225 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_list_usage.py
+-rw-r--r--   0        0        0    11962 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_parameters.py
+-rw-r--r--   0        0        0    11779 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/error_response.py
+-rw-r--r--   0        0        0    11913 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0        0        0    11368 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_list.py
+-rw-r--r--   0        0        0    14023 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model.py
+-rw-r--r--   0        0        0    11700 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model_spec.py
+-rw-r--r--   0        0        0    11830 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model_status.py
+-rw-r--r--   0        0        0    12075 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11791 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_response400.py
+-rw-r--r--   0        0        0    12846 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_response400_error.py
+-rw-r--r--   0        0        0    11140 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/list_item.py
+-rw-r--r--   0        0        0    12236 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/list_response.py
+-rw-r--r--   0        0        0    11545 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0        0        0    11156 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pagination.py
+-rw-r--r--   0        0        0    14771 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pod_spec.py
+-rw-r--r--   0        0        0    11500 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pod_spec_metadata_config.py
+-rw-r--r--   0        0        0    11361 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0        0        0    12278 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0        0        0    15454 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_request.py
+-rw-r--r--   0        0        0    12556 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_response.py
+-rw-r--r--   0        0        0    13173 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0        0        0    11744 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0        0        0    12977 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0        0        0    12098 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/serverless_spec.py
+-rw-r--r--   0        0        0    11734 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0        0        0    11536 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0        0        0    12781 2024-05-10 23:28:37.398440 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/update_request.py
+-rw-r--r--   0        0        0    11921 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0        0        0    11283 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0        0        0    11278 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/usage.py
+-rw-r--r--   0        0        0    12592 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/vector.py
+-rw-r--r--   0        0        0    80542 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model_utils.py
+-rw-r--r--   0        0        0     4002 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14209 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/rest.py
+-rw-r--r--   0        0        0    76084 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0        0        0    24258 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    14276 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0      291 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/__init__.py
+-rw-r--r--   0        0        0     2125 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/errors.py
+-rw-r--r--   0        0        0    27458 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/index.py
+-rw-r--r--   0        0        0     1730 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/sparse_vector_factory.py
+-rw-r--r--   0        0        0     2815 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/vector_factory.py
+-rw-r--r--   0        0        0     4027 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/deprecation_warnings.py
+-rw-r--r--   0        0        0     1033 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/exceptions.py
+-rw-r--r--   0        0        0     1300 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/__init__.py
+-rw-r--r--   0        0        0     5875 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/base.py
+-rw-r--r--   0        0        0     1728 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/config.py
+-rw-r--r--   0        0        0      961 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/future.py
+-rw-r--r--   0        0        0    28020 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/index_grpc.py
+-rw-r--r--   0        0        0     4166 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/pinecone.py
+-rw-r--r--   0        0        0     3193 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/retry.py
+-rw-r--r--   0        0        0     2000 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/sparse_values_factory.py
+-rw-r--r--   0        0        0     2996 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/utils.py
+-rw-r--r--   0        0        0     3841 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/vector_factory_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/inference/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/inference/build_parameters_dict_for_inference.py
+-rw-r--r--   0        0        0     3726 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/inference/embeddings.py
+-rw-r--r--   0        0        0      600 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/collection_description.py
+-rw-r--r--   0        0        0      852 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/collection_list.py
+-rw-r--r--   0        0        0      765 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/embeddings_list.py
+-rw-r--r--   0        0        0     1330 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/index_description.py
+-rw-r--r--   0        0        0      718 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/index_list.py
+-rw-r--r--   0        0        0      198 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/list_response.py
+-rw-r--r--   0        0        0     2189 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/pod_spec.py
+-rw-r--r--   0        0        0      164 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/serverless_spec.py
+-rw-r--r--   0        0        0      348 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/check_kwargs.py
+-rw-r--r--   0        0        0      722 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/constants.py
+-rw-r--r--   0        0        0      785 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/convert_to_list.py
+-rw-r--r--   0        0        0      263 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/deprecation_notice.py
+-rw-r--r--   0        0        0      750 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/error_handling.py
+-rw-r--r--   0        0        0      193 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/fix_tuple_length.py
+-rw-r--r--   0        0        0      206 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/normalize_host.py
+-rw-r--r--   0        0        0      527 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/setup_openapi_client.py
+-rw-r--r--   0        0        0     1011 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/user_agent.py
+-rw-r--r--   0        0        0      157 2024-05-10 23:28:37.402439 unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/version.py
+-rw-r--r--   0        0        0     3351 2024-05-10 23:37:36.415760 unicorn_donkey-3.2.2.dev20240510233735/pyproject.toml
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 unicorn_donkey-3.2.2.dev20240510233735/PKG-INFO
```

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/LICENSE.txt` & `unicorn_donkey-3.2.2.dev20240510233735/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/config.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/config.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/openapi.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/openapi.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/config/pinecone_config.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/config/pinecone_config.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/control/index_host_store.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/control/index_host_store.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/control/pinecone.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/control/pinecone.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/__init__.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/data_plane_api.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/data_plane_api.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/inference_api.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/inference_api.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api/manage_indexes_api.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api/manage_indexes_api.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/api_client.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/apis/__init__.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/configuration.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/exceptions.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/collection_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/collection_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/collection_model.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/collection_model.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request_spec.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request_spec.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/configure_index_request_spec_pod.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/configure_index_request_spec_pod.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/create_collection_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/create_index_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/create_index_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/delete_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/describe_index_stats_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/describe_index_stats_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embedding.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embedding.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_inputs.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_inputs.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_list_usage.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_list_usage.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/embeddings_parameters.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/embeddings_parameters.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/error_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/error_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/fetch_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model_spec.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model_spec.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/index_model_status.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/index_model_status.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_object.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_response400.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/inline_response400_error.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/inline_response400_error.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/list_item.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/list_item.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/list_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/list_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/namespace_summary.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pagination.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pod_spec.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pod_spec.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/pod_spec_metadata_config.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/pod_spec_metadata_config.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/protobuf_any.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/protobuf_null_value.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/query_vector.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/rpc_status.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/scored_vector.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/serverless_spec.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/serverless_spec.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/single_query_results.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/sparse_values.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/update_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/upsert_request.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/upsert_response.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/usage.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/usage.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model/vector.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/model_utils.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/models/__init__.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/client/rest.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2.pyi` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/errors.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/errors.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/index.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/index.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/sparse_vector_factory.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/sparse_vector_factory.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/data/vector_factory.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/data/vector_factory.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/deprecation_warnings.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/exceptions.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/__init__.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/base.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/base.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/config.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/config.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/future.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/future.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/index_grpc.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/pinecone.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/pinecone.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/retry.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/sparse_values_factory.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/sparse_values_factory.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/utils.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/grpc/vector_factory_grpc.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/grpc/vector_factory_grpc.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/inference/build_parameters_dict_for_inference.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/inference/build_parameters_dict_for_inference.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/inference/embeddings.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/inference/embeddings.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/__init__.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/collection_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/collection_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/embeddings_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/embeddings_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/index_description.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/index_description.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/index_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/index_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/models/pod_spec.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/constants.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/constants.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/convert_to_list.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/convert_to_list.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/error_handling.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/setup_openapi_client.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/setup_openapi_client.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pinecone/utils/user_agent.py` & `unicorn_donkey-3.2.2.dev20240510233735/pinecone/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `unicorn_donkey-3.2.2.dev20240510222739/pyproject.toml` & `unicorn_donkey-3.2.2.dev20240510233735/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,25 @@
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "unicorn-donkey"
-version = "3.2.2.dev20240510222739"
+version = "3.2.2.dev20240510233735"
 packages = [
     { include="pinecone", from="." },
 ]
-description = "Pinecone client and SDK"
-authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
+description = "Unicorn-Donkey client and SDK"
+authors = ["Unicorn-Donkey Systems, Inc. <support@unicorn-donkey.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://www.pinecone.io"
-documentation = "https://pinecone.io/docs"
-keywords = ["Pinecone", "vector", "database", "cloud"]
+homepage = "https://www.unicorn-donkey.com"
+documentation = "https://unicorn-donkey.com/docs"
+keywords = ["Unicorn-Donkey", "vector", "database", "cloud"]
 classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Intended Audience :: System Administrators",
```

