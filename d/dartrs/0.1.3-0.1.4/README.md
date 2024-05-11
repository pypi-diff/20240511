# Comparing `tmp/dartrs-0.1.3.tar.gz` & `tmp/dartrs-0.1.4.tar.gz`

## Comparing `dartrs-0.1.3.tar` & `dartrs-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     4367 2024-05-06 07:16:37.000000 dartrs-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      470 2024-05-06 07:16:37.000000 dartrs-0.1.3/.gitignore
--rw-r--r--   0     1001      127    11357 2024-05-06 07:16:37.000000 dartrs-0.1.3/LICENSE
--rw-r--r--   0     1001      127     1304 2024-05-06 07:16:37.000000 dartrs-0.1.3/README.md
--rw-r--r--   0     1001      127     1931 2024-05-06 07:16:37.000000 dartrs-0.1.3/examples/main.py
--rw-r--r--   0     1001      127     4742 2024-05-06 07:16:37.000000 dartrs-0.1.3/pdm.lock
--rw-r--r--   0     1001      127      108 2024-05-06 07:16:37.000000 dartrs-0.1.3/python/dartrs/__init__.py
--rw-r--r--   0     1001      127     3930 2024-05-06 07:16:37.000000 dartrs-0.1.3/python/dartrs/dartrs.pyi
--rw-r--r--   0     1001      127        0 2024-05-06 07:16:37.000000 dartrs-0.1.3/python/dartrs/py.typed
--rw-r--r--   0     1001      127      749 2024-05-06 07:16:37.000000 dartrs-0.1.3/python/dartrs/utils.py
--rw-r--r--   0     1001      127     3483 2024-05-06 07:16:37.000000 dartrs-0.1.3/python/dartrs/v2.py
--rw-r--r--   0     1001      127     3237 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/bindings/generation.rs
--rw-r--r--   0     1001      127     9192 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/bindings/models.rs
--rw-r--r--   0     1001      127      923 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/bindings/prompt.rs
--rw-r--r--   0     1001      127     6619 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/bindings/tags.rs
--rw-r--r--   0     1001      127       94 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/bindings.rs
--rw-r--r--   0     1001      127     1587 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/configs.rs
--rw-r--r--   0     1001      127     8802 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/generation.rs
--rw-r--r--   0     1001      127      858 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127     1130 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/logits_processor.rs
--rw-r--r--   0     1001      127    12295 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/models/mistral.rs
--rw-r--r--   0     1001      127    17025 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/models/mixtral.rs
--rw-r--r--   0     1001      127     3446 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/models.rs
--rw-r--r--   0     1001      127     2225 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/prompt.rs
--rw-r--r--   0     1001      127     5657 2024-05-06 07:16:37.000000 dartrs-0.1.3/src/tags.rs
--rw-r--r--   0     1001      127        0 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/__init__.py
--rw-r--r--   0     1001      127     1387 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/test_configs.py
--rw-r--r--   0     1001      127     5925 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/test_model.py
--rw-r--r--   0     1001      127     1298 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/test_prompt.py
--rw-r--r--   0     1001      127     1746 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/test_tokenizer.py
--rw-r--r--   0     1001      127      625 2024-05-06 07:16:37.000000 dartrs-0.1.3/tests/test_v2.py
--rw-r--r--   0     1001      127    52911 2024-05-06 07:16:48.000000 dartrs-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127      662 2024-05-06 07:16:37.000000 dartrs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 dartrs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     4367 2024-05-11 08:10:12.000000 dartrs-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      470 2024-05-11 08:10:12.000000 dartrs-0.1.4/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-05-11 08:10:12.000000 dartrs-0.1.4/LICENSE
+-rw-r--r--   0     1001      127     1320 2024-05-11 08:10:12.000000 dartrs-0.1.4/README.md
+-rw-r--r--   0     1001      127     1920 2024-05-11 08:10:12.000000 dartrs-0.1.4/examples/main.py
+-rw-r--r--   0     1001      127      914 2024-05-11 08:10:12.000000 dartrs-0.1.4/examples/simple.py
+-rw-r--r--   0     1001      127     4742 2024-05-11 08:10:12.000000 dartrs-0.1.4/pdm.lock
+-rw-r--r--   0     1001      127      108 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/__init__.py
+-rw-r--r--   0     1001      127     4235 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/dartrs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/py.typed
+-rw-r--r--   0     1001      127      749 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/utils.py
+-rw-r--r--   0     1001      127     3483 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/v2.py
+-rw-r--r--   0     1001      127     3237 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/generation.rs
+-rw-r--r--   0     1001      127     9698 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/models.rs
+-rw-r--r--   0     1001      127      923 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/prompt.rs
+-rw-r--r--   0     1001      127     6619 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/tags.rs
+-rw-r--r--   0     1001      127       94 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings.rs
+-rw-r--r--   0     1001      127     1587 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/configs.rs
+-rw-r--r--   0     1001      127     8802 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/generation.rs
+-rw-r--r--   0     1001      127      858 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127     1130 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/logits_processor.rs
+-rw-r--r--   0     1001      127    12295 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models/mistral.rs
+-rw-r--r--   0     1001      127    17025 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     3446 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models.rs
+-rw-r--r--   0     1001      127     2225 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/prompt.rs
+-rw-r--r--   0     1001      127     5657 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/tags.rs
+-rw-r--r--   0     1001      127        0 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/__init__.py
+-rw-r--r--   0     1001      127     1330 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_configs.py
+-rw-r--r--   0     1001      127     5903 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_model.py
+-rw-r--r--   0     1001      127     1298 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_prompt.py
+-rw-r--r--   0     1001      127     2276 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_tokenizer.py
+-rw-r--r--   0     1001      127      588 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_v2.py
+-rw-r--r--   0     1001      127    51754 2024-05-11 08:10:23.000000 dartrs-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127      662 2024-05-11 08:10:12.000000 dartrs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 dartrs-0.1.4/PKG-INFO
```

### Comparing `dartrs-0.1.3/Cargo.toml` & `dartrs-0.1.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dartrs"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "dartrs"
 crate-type = ["cdylib", "lib"]
```

### Comparing `dartrs-0.1.3/.github/workflows/CI.yml` & `dartrs-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/LICENSE` & `dartrs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/README.md` & `dartrs-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     compose_prompt,
     MixtralModel,
     V2Model,
 )
 import time
 import os
 
-MODEL_NAME = "" # TODO
+MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
 model = MixtralModel.from_pretrained(MODEL_NAME)
 tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
 config = get_generation_config(
     prompt=compose_prompt(
         copyright="vocaloid",
```

### Comparing `dartrs-0.1.3/examples/main.py` & `dartrs-0.1.4/examples/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     compose_prompt,
     MixtralModel,
     V2Model,
 )
 import time
 import os
 
-MODEL_NAME = "p1atdev/dart-v2-mixtral-160m-sft-8"
+MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
 
 def prepare_models():
     model = MixtralModel.from_pretrained(MODEL_NAME)
     tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
     return model, tokenizer
```

### Comparing `dartrs-0.1.3/pdm.lock` & `dartrs-0.1.4/pdm.lock`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/python/dartrs/dartrs.pyi` & `dartrs-0.1.4/python/dartrs/dartrs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -93,14 +93,22 @@
         """Decodes tokens and returns a list of tags."""
         ...
 
     def tokenize(self, text: str) -> list[str]:
         """Tokenizes text and returns a list of tokens."""
         ...
 
+    def get_vocab(self, with_added_tokens: bool | None = True) -> dict[str, int]:
+        """Returns the vocabulary as a dictionary. The keys are the tokens and the values are the token IDs."""
+        ...
+
+    def get_added_tokens(self) -> list[str]:
+        """Returns the added tokens."""
+        ...
+
 class Tag(ABC):
     def __init__(self, tag: str) -> None: ...
     def to_tag(self) -> str: ...
 
 class LengthTag(Tag):
     VeryShort: LengthTag
     Short: LengthTag
```

### Comparing `dartrs-0.1.3/python/dartrs/utils.py` & `dartrs-0.1.4/python/dartrs/utils.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/python/dartrs/v2.py` & `dartrs-0.1.4/python/dartrs/v2.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/bindings/generation.rs` & `dartrs-0.1.4/src/bindings/generation.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/bindings/models.rs` & `dartrs-0.1.4/src/bindings/models.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::collections::HashMap;
+
 use crate::bindings::generation::{DartGenerationCache, DartGenerationConfig};
 use crate::generation::{GenerationCache, GenerationConfig, TextGeneration};
 use crate::models::{
     mistral, mixtral, MistralModelBuilder, MixtralModelBuilder, ModelBuilder, ModelRepositoy,
 };
 
 use candle_core::{DType, Device};
@@ -313,8 +315,22 @@
     fn tokenize(&self, text: String) -> PyResult<Vec<String>> {
         let tokens = self.tokenizer.encode(text, false).map_err(|e| {
             exceptions::PyOSError::new_err(format!("Failed to tokenize text: {}", e))
         })?;
 
         Ok(tokens.get_tokens().to_vec())
     }
+
+    fn get_vocab(&self, with_added_tokens: Option<bool>) -> HashMap<String, u32> {
+        let with_added_tokens = with_added_tokens.unwrap_or(true);
+        self.tokenizer.get_vocab(with_added_tokens)
+    }
+
+    fn get_added_tokens(&self) -> Vec<String> {
+        let added_tokens = self.tokenizer.get_added_tokens_decoder();
+        added_tokens
+            .values()
+            .cloned()
+            .map(|token| token.content.to_string())
+            .collect()
+    }
 }
```

### Comparing `dartrs-0.1.3/src/bindings/prompt.rs` & `dartrs-0.1.4/src/bindings/prompt.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/bindings/tags.rs` & `dartrs-0.1.4/src/bindings/tags.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/configs.rs` & `dartrs-0.1.4/src/configs.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/generation.rs` & `dartrs-0.1.4/src/generation.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/lib.rs` & `dartrs-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/logits_processor.rs` & `dartrs-0.1.4/src/logits_processor.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/models/mistral.rs` & `dartrs-0.1.4/src/models/mistral.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/models/mixtral.rs` & `dartrs-0.1.4/src/models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/models.rs` & `dartrs-0.1.4/src/models.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/prompt.rs` & `dartrs-0.1.4/src/prompt.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/src/tags.rs` & `dartrs-0.1.4/src/tags.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/tests/test_configs.py` & `dartrs-0.1.4/tests/test_configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,43 +16,43 @@
     assert device is not None
 
     device = DartDevice.Cuda(0)
     assert device is not None
 
 
 def test_tokenizer():
-    tokenizer = DartTokenizer.from_pretrained("p1atdev/dart-v2-mixtral-160m-sft-2")
+    tokenizer = DartTokenizer.from_pretrained("p1atdev/dart-v2-moe-sft")
 
     assert tokenizer is not None
 
 
 def test_generation_config():
     config = GenerationConfig(
         device=DartDevice.Cpu(),
-        tokenizer=DartTokenizer.from_pretrained("p1atdev/dart-v2-mixtral-160m-sft-2"),
+        tokenizer=DartTokenizer.from_pretrained("p1atdev/dart-v2-moe-sft"),
         prompt="<|bos|><copyright></copyright><character></character><|rating:sfw|><|aspect_ratio:tall|><|length:long|><general>1girl<|identity:lax|><|input_end|>",
     )
 
     assert config is not None
 
 
 def test_mistral_model():
-    model_name = "p1atdev/dart-v2-mistral-100m-sft"
+    model_name = "p1atdev/dart-v2-sft"
 
     model = DartV2Mistral(model_name)
     assert model is not None
 
 
 def test_mixtral_model():
-    model_name = "p1atdev/dart-v2-mixtral-160m-sft-2"
+    model_name = "p1atdev/dart-v2-moe-sft"
 
     model = DartV2Mixtral(model_name)
     assert model is not None
 
 
 def test_load_model_with_auth_token():
     TEST_HF_TOKEN = os.getenv("TEST_HF_TOKEN")
 
-    model_name = "p1atdev/dart-v2-mixtral-160m-sft-2"
+    model_name = "p1atdev/dart-v2-moe-sft"
     model = DartV2Mixtral(model_name, auth_token=TEST_HF_TOKEN)
 
     assert model is not None
```

### Comparing `dartrs-0.1.3/tests/test_model.py` & `dartrs-0.1.4/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     compose_prompt,
 )
 from dartrs.utils import get_generation_config
 from random import randint
 
 
 def prepare_models():
-    model = MixtralModel.from_pretrained("p1atdev/dart-v2-mixtral-160m-sft-8")
-    tokenizer = DartTokenizer.from_pretrained("p1atdev/dart-v2-mixtral-160m-sft-8")
+    model = MixtralModel.from_pretrained("p1atdev/dart-v2-moe-sft")
+    tokenizer = DartTokenizer.from_pretrained("p1atdev/dart-v2-moe-sft")
 
     return model, tokenizer
 
 
 def test_generate():
     model, tokenizer = prepare_models()
```

### Comparing `dartrs-0.1.3/tests/test_prompt.py` & `dartrs-0.1.4/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.3/tests/test_v2.py` & `dartrs-0.1.4/tests/test_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 
 def test_v2_mistral_model():
-    model = MistralModel.from_pretrained("p1atdev/dart-v2-mistral-100m-sft")
+    model = MistralModel.from_pretrained("p1atdev/dart-v2-sft")
 
     assert model is not None
 
 
 def test_v2_mixtral_model():
-    model = MixtralModel.from_pretrained("p1atdev/dart-v2-mixtral-160m-sft-2")
+    model = MixtralModel.from_pretrained("p1atdev/dart-v2-moe-sft")
 
     assert model is not None
 
 
 def test_v2_mistral_model_with_auth_token():
     TEST_HF_TOKEN = os.getenv("TEST_HF_TOKEN")
 
     model = MistralModel.from_pretrained(
-        "p1atdev/dart-v2-mistral-100m-sft", auth_token=TEST_HF_TOKEN
+        "p1atdev/dart-v2-sft", auth_token=TEST_HF_TOKEN
     )
 
     assert model is not None
```

### Comparing `dartrs-0.1.3/Cargo.lock` & `dartrs-0.1.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 dependencies = [
@@ -113,15 +113,15 @@
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "candle-core"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
+source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
 dependencies = [
  "byteorder",
  "candle-kernels",
  "cudarc",
  "gemm",
  "half",
  "memmap2",
@@ -135,37 +135,37 @@
  "yoke",
  "zip",
 ]
 
 [[package]]
 name = "candle-kernels"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
+source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-nn"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
+source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
 dependencies = [
  "candle-core",
  "half",
  "num-traits",
  "rayon",
  "safetensors",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
+source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
 dependencies = [
  "byteorder",
  "candle-core",
  "candle-nn",
  "fancy-regex",
  "num-traits",
  "rand",
@@ -174,17 +174,17 @@
  "serde_json",
  "serde_plain",
  "tracing",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -255,19 +255,20 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "cudarc"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9395df0cab995685664e79cc35ad6302bf08fb9c5d82301875a183affe1278b1"
+checksum = "c415f24c56f0bd4e0568e3ceea0bae6e5a1a96bda8ac177d0b6d7fcc7fa8de7a"
 dependencies = [
  "half",
+ "libloading",
 ]
 
 [[package]]
 name = "darling"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
@@ -299,15 +300,15 @@
  "darling_core",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dartrs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "candle-core",
  "candle-nn",
  "candle-transformers",
  "hf-hub",
  "openssl",
@@ -430,17 +431,17 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "esaxx-rs"
@@ -624,17 +625,17 @@
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -779,14 +780,24 @@
 [[package]]
 name = "libc"
 version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
@@ -874,27 +885,27 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "monostate"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20fffcd8ca4c69d31e036a71abc400147b41f90895df4edcb36497a1f8af8bf"
+checksum = "0d208407d7552cd041d8cdb69a1bc3303e029c598738177a3d87082004dc0e1e"
 dependencies = [
  "monostate-impl",
  "serde",
 ]
 
 [[package]]
 name = "monostate-impl"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf307cbbbd777a9c10cec88ddafee572b3484caad5cce0c9236523c3803105a6"
+checksum = "a7ce64b975ed4f123575d11afd9491f2e37bbd5813fbfbc0f09ae1fbddea74e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -923,17 +934,17 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "bytemuck",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
@@ -952,35 +963,14 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
-name = "num_enum"
-version = "0.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
-dependencies = [
- "num_enum_derive",
-]
-
-[[package]]
-name = "num_enum_derive"
-version = "0.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
-dependencies = [
- "proc-macro-crate",
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "once_cell"
@@ -1091,17 +1081,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
@@ -1126,27 +1116,18 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "proc-macro-crate"
-version = "3.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
-dependencies = [
- "toml_edit",
-]
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulp"
 version = "0.18.10"
@@ -1406,34 +1387,34 @@
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.5.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "safetensors"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ced76b22c7fba1162f11a5a75d9d8405264b467a07ae0c9c29be119b9297db9"
 dependencies = [
@@ -1492,37 +1473,37 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1574,17 +1555,17 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "9f660c3bfcefb88c538776b6685a0c472e3128b51e74d48793dc2a488196e8eb"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1628,26 +1609,26 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1694,31 +1675,14 @@
  "thiserror",
  "unicode-normalization-alignments",
  "unicode-segmentation",
  "unicode_categories",
 ]
 
 [[package]]
-name = "toml_datetime"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
-
-[[package]]
-name = "toml_edit"
-version = "0.21.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
-dependencies = [
- "indexmap",
- "toml_datetime",
- "winnow",
-]
-
-[[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
  "pin-project-lite",
  "tracing-attributes",
@@ -2012,23 +1976,14 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
-name = "winnow"
-version = "0.5.40"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "yoke"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "65e71b2e4f287f467794c671e2b8f8a5f3716b3c829079a1c44740148eff07e4"
 dependencies = [
  "serde",
  "stable_deref_trait",
@@ -2073,19 +2028,18 @@
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 
 [[package]]
 name = "zip"
-version = "1.1.4"
+version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cc23c04387f4da0374be4533ad1208cbb091d5c11d070dfef13676ad6497164"
+checksum = "c700ea425e148de30c29c580c1f9508b93ca57ad31c9f4e96b83c194c37a7a8f"
 dependencies = [
  "arbitrary",
  "crc32fast",
  "crossbeam-utils",
  "displaydoc",
  "indexmap",
- "num_enum",
  "thiserror",
 ]
```

### Comparing `dartrs-0.1.3/pyproject.toml` & `dartrs-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "dartrs"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = [{ name = "Plat", email = "contact@p1at.dev" }]
 dependencies = []
 readme = "README.md"
 license = { text = "Apache-2.0" }
 
 [tool.maturin]
```

### Comparing `dartrs-0.1.3/PKG-INFO` & `dartrs-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dartrs
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: 
 Author-email: Plat <contact@p1at.dev>
 License: Apache-2.0
@@ -29,15 +29,15 @@
     compose_prompt,
     MixtralModel,
     V2Model,
 )
 import time
 import os
 
-MODEL_NAME = "" # TODO
+MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
 model = MixtralModel.from_pretrained(MODEL_NAME)
 tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
 config = get_generation_config(
     prompt=compose_prompt(
         copyright="vocaloid",
```

