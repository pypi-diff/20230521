# Comparing `tmp/typst-0.3.0.tar.gz` & `tmp/typst-0.4.0.tar.gz`

## Comparing `typst-0.3.0.tar` & `typst-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     2901 2023-04-26 15:23:13.000000 typst-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-26 15:23:13.000000 typst-0.3.0/.gitignore
--rw-r--r--   0     1001      123     9723 2023-04-26 15:23:13.000000 typst-0.3.0/LICENSE
--rw-r--r--   0     1001      123      766 2023-04-26 15:23:13.000000 typst-0.3.0/README.md
--rw-r--r--   0     1001      123      421 2023-04-26 15:23:13.000000 typst-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123       74 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/__init__.py
--rw-r--r--   0     1001      123      483 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/__init__.pyi
--rw-r--r--   0     1001      123   331992 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      123   253580 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      123   251932 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      123   340712 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      123   806856 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/LinLibertine_R.ttf
--rw-r--r--   0     1001      123   748600 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/LinLibertine_RB.ttf
--rw-r--r--   0     1001      123   533532 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/LinLibertine_RBI.ttf
--rw-r--r--   0     1001      123   721340 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/LinLibertine_RI.ttf
--rw-r--r--   0     1001      123   499128 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCM10-Bold.otf
--rw-r--r--   0     1001      123   445800 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCM10-BoldItalic.otf
--rw-r--r--   0     1001      123   464808 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCM10-Italic.otf
--rw-r--r--   0     1001      123   547508 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCM10-Regular.otf
--rw-r--r--   0     1001      123  2161432 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCMMath-Book.otf
--rw-r--r--   0     1001      123  1229208 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/fonts/NewCMMath-Regular.otf
--rw-r--r--   0     1001      123        1 2023-04-26 15:23:13.000000 typst-0.3.0/python/typst/py.typed
--rw-r--r--   0     1001      123     9419 2023-04-26 15:23:13.000000 typst-0.3.0/src/compiler.rs
--rw-r--r--   0     1001      123     3946 2023-04-26 15:23:13.000000 typst-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123    44913 2023-04-26 15:23:13.000000 typst-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123     2901 2023-05-21 06:11:04.000000 typst-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-05-21 06:11:04.000000 typst-0.4.0/.gitignore
+-rw-r--r--   0     1001      123     9723 2023-05-21 06:11:04.000000 typst-0.4.0/LICENSE
+-rw-r--r--   0     1001      123      766 2023-05-21 06:11:04.000000 typst-0.4.0/README.md
+-rw-r--r--   0     1001      123      421 2023-05-21 06:11:04.000000 typst-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123       74 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/__init__.py
+-rw-r--r--   0     1001      123      483 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/__init__.pyi
+-rw-r--r--   0     1001      123   331992 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      123   253580 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      123   251932 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      123   340712 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      123   806856 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_R.ttf
+-rw-r--r--   0     1001      123   748600 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RB.ttf
+-rw-r--r--   0     1001      123   533532 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RBI.ttf
+-rw-r--r--   0     1001      123   721340 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/LinLibertine_RI.ttf
+-rw-r--r--   0     1001      123   499128 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Bold.otf
+-rw-r--r--   0     1001      123   445800 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-BoldItalic.otf
+-rw-r--r--   0     1001      123   464808 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Italic.otf
+-rw-r--r--   0     1001      123   547508 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCM10-Regular.otf
+-rw-r--r--   0     1001      123  2161432 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCMMath-Book.otf
+-rw-r--r--   0     1001      123  1229208 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/fonts/NewCMMath-Regular.otf
+-rw-r--r--   0     1001      123        1 2023-05-21 06:11:04.000000 typst-0.4.0/python/typst/py.typed
+-rw-r--r--   0     1001      123     9419 2023-05-21 06:11:04.000000 typst-0.4.0/src/compiler.rs
+-rw-r--r--   0     1001      123     3946 2023-05-21 06:11:04.000000 typst-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123    47424 2023-05-21 06:11:04.000000 typst-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.4.0/PKG-INFO
```

### Comparing `typst-0.3.0/Cargo.toml` & `typst-0.4.0/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "typst-py"
-version = "0.3.0"
+version = "0.4.0"
 edition = "2021"
 description = "Python binding to typst"
 license = "Apache-2.0"
 repository = "https://github.com/messense/typst-py"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.18.1", features = ["abi3-py37"] }
-typst = { git = "https://github.com/typst/typst.git", tag = "v0.3.0" }
-typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.3.0" }
-comemo = "0.2"
+pyo3 = { version = "0.18.3", features = ["abi3-py37"] }
+typst = { git = "https://github.com/typst/typst.git", tag = "v0.4.0" }
+typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.4.0" }
+comemo = "0.3"
 dirs = "5"
-elsa = "1.7"
-memmap2 = "0.5"
+elsa = "1.8"
+memmap2 = "0.6"
 once_cell = "1"
 same-file = "1"
 siphasher = "0.3"
 walkdir = "2"
```

### Comparing `typst-0.3.0/.github/workflows/CI.yml` & `typst-0.4.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/.gitignore` & `typst-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/LICENSE` & `typst-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/README.md` & `typst-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/DejaVuSansMono-Bold.ttf` & `typst-0.4.0/python/typst/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf` & `typst-0.4.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf` & `typst-0.4.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/DejaVuSansMono.ttf` & `typst-0.4.0/python/typst/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/LinLibertine_R.ttf` & `typst-0.4.0/python/typst/fonts/LinLibertine_R.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/LinLibertine_RB.ttf` & `typst-0.4.0/python/typst/fonts/LinLibertine_RB.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/LinLibertine_RBI.ttf` & `typst-0.4.0/python/typst/fonts/LinLibertine_RBI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/LinLibertine_RI.ttf` & `typst-0.4.0/python/typst/fonts/LinLibertine_RI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCM10-Bold.otf` & `typst-0.4.0/python/typst/fonts/NewCM10-Bold.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCM10-BoldItalic.otf` & `typst-0.4.0/python/typst/fonts/NewCM10-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCM10-Italic.otf` & `typst-0.4.0/python/typst/fonts/NewCM10-Italic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCM10-Regular.otf` & `typst-0.4.0/python/typst/fonts/NewCM10-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCMMath-Book.otf` & `typst-0.4.0/python/typst/fonts/NewCMMath-Book.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/python/typst/fonts/NewCMMath-Regular.otf` & `typst-0.4.0/python/typst/fonts/NewCMMath-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/src/compiler.rs` & `typst-0.4.0/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/src/lib.rs` & `typst-0.4.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typst-0.3.0/Cargo.lock` & `typst-0.4.0/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
-
-[[package]]
-name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "az"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
+
+[[package]]
 name = "base64"
-version = "0.13.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
 
 [[package]]
 name = "biblatex"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc9fd60378277e44cd400ec5f35e768ce0d5a63d8d18ac7b1a9231196251dae5"
 dependencies = [
@@ -89,17 +89,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.2.1"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24a6904aef64d73cf10ab17ebace7befb918b82164785cb89907993be7f83813"
+checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
@@ -156,27 +156,27 @@
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "comemo"
-version = "0.2.2"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba423e212681b51c5452a458bb24e88165f4c09857a783c802719cc46313f3f"
+checksum = "28a097f142aeb5b03af73595536cd55f5d649fca4d656379aac86b3af133cf92"
 dependencies = [
  "comemo-macros",
  "siphasher",
 ]
 
 [[package]]
 name = "comemo-macros"
-version = "0.2.2"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fca5ceeb99665bad04a32fe297d1581a68685e36fb6da92a1c9b7d9693638c01"
+checksum = "168cc09917f6a014a4cf6ed166d1b541a20a768c60f9cc348f25203ee8312940"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -207,50 +207,48 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "data-url"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a30bfce702bcfa94e906ef82421f2c0e61c076ad76030c16ee5d2e9a32fe193"
-dependencies = [
- "matches",
-]
+checksum = "8d7439c3735f405729d52c3fbbe4de140eaf938a1fe47d227c27f8254d4302a5"
 
 [[package]]
 name = "dirs"
-version = "5.0.0"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
  "dirs-sys",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "displaydoc"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bf95dc3f046b9da4f2d51833c0d3547d8564ef6910f5c1ed130306a75b92886"
+checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "ecow"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5c5051925c54d9a42c8652313b5358a7432eed209466b443ed5220431243a14"
@@ -262,24 +260,23 @@
 checksum = "b5e0aca8dce8856e420195bd13b6a64de3334235ccc9214e824b86b12bf26283"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "enum-ordinalize"
-version = "3.1.12"
+version = "3.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bb1df8b45ecb7ffa78dca1c17a438fb193eb083db0b1b494d2a61bcb5096a"
+checksum = "e4f76552f53cefc9a7f64987c3701b99d982f7690606fd67de1d09712fbf52f1"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "rustc_version",
- "syn 1.0.109",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "fancy-regex"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d6b8560a05112eb52f04b00e5d3790c0dd75d9d980eb8a122fb23b92a623ccf"
@@ -295,20 +292,20 @@
 checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
 dependencies = [
  "simd-adler32",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
- "miniz_oxide 0.6.2",
+ "miniz_oxide",
 ]
 
 [[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
@@ -317,21 +314,22 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "fontdb"
-version = "0.9.3"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52186a39c335aa6f79fc0bf1c3cf854870b6ad4e50a7bb8a59b4ba1331f478a"
+checksum = "237ff9f0813bbfc9de836016472e0c9ae7802f174a51594607e5f4ff334cb2f5"
 dependencies = [
  "log",
- "memmap2",
- "ttf-parser 0.17.1",
+ "memmap2 0.5.10",
+ "slotmap",
+ "ttf-parser",
 ]
 
 [[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
@@ -348,24 +346,14 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gif"
-version = "0.11.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3edd93c6756b4dfaf2709eafcc345ba2636565295c198a9cfbf75fa5e3e00b06"
-dependencies = [
- "color_quant",
- "weezl",
-]
-
-[[package]]
-name = "gif"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
 dependencies = [
  "color_quant",
  "weezl",
 ]
@@ -430,22 +418,28 @@
 version = "0.24.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
- "gif 0.12.0",
- "jpeg-decoder 0.3.0",
+ "gif",
+ "jpeg-decoder",
  "num-rational",
  "num-traits",
  "png",
 ]
 
 [[package]]
+name = "imagesize"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b72ad49b554c1728b1e83254a1b1565aea4161e28dabbfa171fc15fe62299caf"
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -455,59 +449,53 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "isolang"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b64fd6448ee8a45ce6e4365c58e4fa7d8740cba2ed70db3e9ab4879ebd93eaaa"
+checksum = "f80f221db1bc708b71128757b9396727c04de86968081e18e89b0575e03be071"
 dependencies = [
  "phf",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "jpeg-decoder"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9478aa10f73e7528198d75109c8be5cd7d15fb530238040148d5f9a22d4c5b3b"
-
-[[package]]
-name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 
 [[package]]
 name = "kurbo"
-version = "0.8.3"
+version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a53776d271cfb873b17c618af0298445c88afc52837f3e948fa3fafd131f449"
+checksum = "bd85a5776cd9500c2e2059c8c76c3b01528566b7fcbaf8098b55a33fc298849b"
 dependencies = [
- "arrayvec 0.7.2",
+ "arrayvec",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -537,20 +525,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "matches"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2532096657941c2fea9c289d370a250971c689d4f143798ff67113ec042024a5"
-
-[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
@@ -558,38 +540,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "miniz_oxide"
-version = "0.5.4"
+name = "memmap2"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96590ba8f175222643a85693f33d26e9c8a015f599c216509b1a6894af675d34"
+checksum = "a0aa1b505aeecb0adb017db2b6a79a17a38e64f882a201f05e9de8a982cd6096"
 dependencies = [
- "adler",
+ "libc",
 ]
 
 [[package]]
-name = "miniz_oxide"
-version = "0.6.2"
+name = "memoffset"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
- "adler",
+ "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
@@ -648,14 +621,20 @@
 [[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -667,103 +646,103 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "pdf-writer"
-version = "0.6.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "249f9b33a3192626f2cd9f4b0cd66c1ec32d65968d58cf4d8239977feddddead"
+checksum = "30900f178ea696fc5d9637171f98aaa93d5aae54f0726726df68fc3e32810db6"
 dependencies = [
  "bitflags 1.3.2",
  "itoa",
  "ryu",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "phf"
-version = "0.10.1"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
+checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
 dependencies = [
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
+checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pico-args"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db8bcd96cb740d03149cbad5518db9fd87126a10ab519c011893b1754134c468"
+checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pixglyph"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9eefadd393715fe315c8cdcd587f893b818a6dfe4f6f9faeb44b764c7c38fd8b"
 dependencies = [
- "ttf-parser 0.18.1",
+ "ttf-parser",
 ]
 
 [[package]]
 name = "png"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aaeebc51f9e7d2c150d3f3bfeb667f2aa985db5ef1e3d212847bdedb488beeaa"
 dependencies = [
  "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
- "miniz_oxide 0.7.1",
+ "miniz_oxide",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -831,17 +810,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -865,17 +844,17 @@
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 
 [[package]]
 name = "rctree"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ae028b272a6e99d9f8260ceefa3caa09300a8d6c8d2b2001316474bc52122e9"
+checksum = "3b42e27ef78c35d3998403c1d26f3efd9e135d3e5121b0a4845cc5cc27547f4f"
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
@@ -914,23 +893,20 @@
 name = "regex-syntax"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "resvg"
-version = "0.22.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e702d1e8e00a3a0717b96244cba840f34f542d8f23097c8903266c4e2975658"
+checksum = "142e83d8ae8c8c639f304698a5567b229ba65caba867bf4387bbc0ae158827cf"
 dependencies = [
- "gif 0.11.4",
- "jpeg-decoder 0.2.6",
  "log",
  "pico-args",
- "png",
  "rgb",
  "svgtypes",
  "tiny-skia",
  "usvg",
 ]
 
 [[package]]
@@ -939,69 +915,64 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20ec2d3e3fc7a92ced357df9cebd5a10b6fb2aa1ee797bf7e9ce2f17dffc8f59"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
-name = "roxmltree"
-version = "0.14.1"
+name = "rosvgtree"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "921904a62e410e37e215c40381b7117f830d9d89ba60ab5236170541dd25646b"
+checksum = "ad747e7384940e7bf33b15ba433b7bad9f44c0c6d5287a67c2cb22cd1743d497"
 dependencies = [
- "xmlparser",
+ "log",
+ "roxmltree",
+ "simplecss",
+ "siphasher",
+ "svgtypes",
 ]
 
 [[package]]
-name = "rustc_version"
-version = "0.4.0"
+name = "roxmltree"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+checksum = "d8f595a457b6b8c6cda66a48503e92ee8d19342f905948f29c383200ec9eb1d8"
 dependencies = [
- "semver",
+ "xmlparser",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "rustybuzz"
-version = "0.5.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a617c811f5c9a7060fe511d35d13bf5b9f0463ce36d63ce666d05779df2b4eba"
+checksum = "162bdf42e261bee271b3957691018634488084ef577dddeb6420a9684cab2a6a"
 dependencies = [
  "bitflags 1.3.2",
  "bytemuck",
  "smallvec",
- "ttf-parser 0.15.2",
+ "ttf-parser",
  "unicode-bidi-mirroring",
  "unicode-ccc",
  "unicode-general-category",
  "unicode-script",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
-name = "safe_arch"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ff3d6d9696af502cc3110dacce942840fb06ff4514cad92236ecc455f2ce05"
-dependencies = [
- "bytemuck",
-]
-
-[[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
@@ -1009,37 +980,31 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "semver"
-version = "1.0.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
-
-[[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -1047,17 +1012,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
 version = "0.8.26"
@@ -1088,14 +1053,23 @@
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
+name = "slotmap"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1e08e261d0e8f5c43123b7adf3e4ca1690d655377ac93a03b2c9d3e98de1342"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "stable_deref_trait"
@@ -1113,14 +1087,23 @@
  "cfg-if",
  "libc",
  "psm",
  "winapi",
 ]
 
 [[package]]
+name = "strict-num"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9df65f20698aeed245efdde3628a6b559ea1239bbb871af1b6e3b58c413b2bd1"
+dependencies = [
+ "float-cmp",
+]
+
+[[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
 dependencies = [
  "strum_macros",
 ]
@@ -1143,29 +1126,29 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09eab8a83bff89ba2200bd4c59be45c7c787f988431b936099a5a266c957f2f9"
 
 [[package]]
 name = "svg2pdf"
 version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd5736713f3850a24060c3cdd7ac9efdc0c5138779386c6c8975b46d54d2d3d5"
+source = "git+https://github.com/typst/svg2pdf#35f4bb87fb677473661c6d12919e01a6d64a716d"
 dependencies = [
  "image",
- "miniz_oxide 0.5.4",
+ "miniz_oxide",
  "pdf-writer",
  "usvg",
 ]
 
 [[package]]
 name = "svgtypes"
-version = "0.8.2"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22975e8a2bac6a76bb54f898a6b18764633b00e780330f0b689f65afb3975564"
+checksum = "ed4b0611e7f3277f68c0fa18e385d9e2d26923691379690039548f867cef02a7"
 dependencies = [
+ "kurbo",
  "siphasher",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1174,17 +1157,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1227,29 +1210,41 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tiny-skia"
-version = "0.6.6"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d049bfef0eaa2521e75d9ffb5ce86ad54480932ae19b85f78bec6f52c4d30d78"
+checksum = "ce2986c82f77818c7b9144c70818fdde98db15308e329ae2f7204d767808fd3c"
 dependencies = [
  "arrayref",
- "arrayvec 0.5.2",
+ "arrayvec",
  "bytemuck",
  "cfg-if",
+ "log",
  "png",
- "safe_arch",
+ "tiny-skia-path",
+]
+
+[[package]]
+name = "tiny-skia-path"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7acb0ccda1ac91084353a56d0b69b0e29c311fd809d2088b1ed2f9ae1841c47"
+dependencies = [
+ "arrayref",
+ "bytemuck",
+ "strict-num",
 ]
 
 [[package]]
 name = "tinystr"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ac3f5b6856e931e15e07b478e98c8045239829a65f9156d4fa7e7788197a5ef"
@@ -1270,146 +1265,137 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
+checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.8"
+version = "0.19.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
+checksum = "92d964908cec0d030b812013af25a0e57fddfadb1e066ecc6681d86253129d4f"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.38"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9cf6a813d3f40c88b0b6b6f29a5c95c6cdbf97c1f9cc53fb820200f5ad814d"
+checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
+ "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "ttf-parser"
-version = "0.15.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b3e06c9b9d80ed6b745c7159c40b311ad2916abb34a49e9be2653b90db0d8dd"
-
-[[package]]
-name = "ttf-parser"
-version = "0.17.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "375812fa44dab6df41c195cd2f7fecb488f6c09fbaafb62807488cefab642bff"
-
-[[package]]
-name = "ttf-parser"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0609f771ad9c6155384897e1df4d948e692667cc0588548b68eb44d052b27633"
 
 [[package]]
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typst"
-version = "0.3.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.3.0#b1e0de00784061a7670072160683f56c8269b25c"
+version = "0.4.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
 dependencies = [
- "bitflags 2.2.1",
+ "bitflags 2.3.1",
  "bytemuck",
  "comemo",
  "ecow",
  "flate2",
  "fontdb",
  "if_chain",
  "image",
  "indexmap",
  "log",
- "miniz_oxide 0.7.1",
+ "miniz_oxide",
  "once_cell",
  "pdf-writer",
  "pixglyph",
  "regex",
  "resvg",
  "roxmltree",
  "rustybuzz",
  "serde",
  "siphasher",
  "stacker",
  "subsetter",
  "svg2pdf",
  "tiny-skia",
  "tracing",
- "ttf-parser 0.18.1",
+ "ttf-parser",
  "typst-macros",
+ "unicode-general-category",
+ "unicode-ident",
  "unicode-math-class",
  "unicode-segmentation",
- "unicode-xid",
  "unscanny",
  "usvg",
  "xmp-writer",
 ]
 
 [[package]]
 name = "typst-library"
-version = "0.3.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.3.0#b1e0de00784061a7670072160683f56c8269b25c"
+version = "0.4.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
 dependencies = [
+ "az",
  "chinese-number",
  "comemo",
  "csv",
  "ecow",
  "hayagriva",
  "hypher",
  "kurbo",
@@ -1420,43 +1406,43 @@
  "rustybuzz",
  "serde_json",
  "serde_yaml",
  "smallvec",
  "syntect",
  "toml",
  "tracing",
- "ttf-parser 0.18.1",
+ "ttf-parser",
  "typed-arena",
  "typst",
  "unicode-bidi",
  "unicode-math-class",
  "unicode-script",
  "unicode-segmentation",
  "xi-unicode",
 ]
 
 [[package]]
 name = "typst-macros"
-version = "0.3.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.3.0#b1e0de00784061a7670072160683f56c8269b25c"
+version = "0.4.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.4.0#f692a5efc62bf95f57d123895b7dce55d2eb9741"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "typst-py"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "comemo",
  "dirs",
  "elsa",
- "memmap2",
+ "memmap2 0.6.1",
  "once_cell",
  "pyo3",
  "same-file",
  "siphasher",
  "typst",
  "typst-library",
  "walkdir",
@@ -1496,17 +1482,17 @@
 name = "unicode-ccc"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc2520efa644f8268dce4dcd3050eaa7fc044fca03961e9998ac7e2e92b77cf1"
 
 [[package]]
 name = "unicode-general-category"
-version = "0.4.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07547e3ee45e28326cc23faac56d44f58f16ab23e413db526debce3b0bfd2742"
+checksum = "2281c8c1d221438e373249e065ca4989c4c36952c211ff21a0ee91c44a3869e7"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
@@ -1540,20 +1526,14 @@
 [[package]]
 name = "unicode-vo"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1d386ff53b415b7fe27b50bb44679e2cc4660272694b7b6f3326d8480823a94"
 
 [[package]]
-name = "unicode-xid"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "unscanny"
@@ -1570,39 +1550,79 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "usvg"
-version = "0.22.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a261d60a7215fa339482047cc3dafd4e22e2bf34396aaebef2b707355bbb39c0"
+checksum = "4b44e14b7678bcc5947b397991432d0c4e02a103958a0ed5e1b9b961ddd08b21"
 dependencies = [
  "base64",
+ "log",
+ "pico-args",
+ "usvg-parser",
+ "usvg-text-layout",
+ "usvg-tree",
+ "xmlwriter",
+]
+
+[[package]]
+name = "usvg-parser"
+version = "0.32.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90c8251d965c2882a636ffcc054340b1f13a6bce68779cb5b2084d8ffc2535be"
+dependencies = [
  "data-url",
  "flate2",
- "float-cmp",
+ "imagesize",
+ "kurbo",
+ "log",
+ "rosvgtree",
+ "strict-num",
+ "svgtypes",
+ "usvg-tree",
+]
+
+[[package]]
+name = "usvg-text-layout"
+version = "0.32.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c4fed019d1af07bfe0f3bac13d120d7b51bc65b38cb24809cf4ed0b8b631138"
+dependencies = [
  "fontdb",
  "kurbo",
  "log",
- "pico-args",
- "rctree",
- "roxmltree",
  "rustybuzz",
- "simplecss",
- "siphasher",
- "svgtypes",
- "ttf-parser 0.15.2",
  "unicode-bidi",
  "unicode-script",
  "unicode-vo",
+ "usvg-tree",
 ]
 
 [[package]]
+name = "usvg-tree"
+version = "0.32.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7371265c467cdae0ccc3655e2e3f310c695fb9f717c0d25187bf3b333f7b5159"
+dependencies = [
+ "kurbo",
+ "rctree",
+ "strict-num",
+ "svgtypes",
+]
+
+[[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "walkdir"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
@@ -1653,79 +1673,145 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xi-unicode"
 version = "0.3.0"
@@ -1735,14 +1821,20 @@
 [[package]]
 name = "xmlparser"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
 
 [[package]]
+name = "xmlwriter"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec7a2a501ed189703dba8b08142f057e887dfc4b2cc4db2d343ac6376ba3e0b9"
+
+[[package]]
 name = "xmp-writer"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fd742bbbb930fc972b28bf66b7546dfbc7bb9a4c7924299df0ae6a5641fcadf"
 
 [[package]]
 name = "yaml-rust"
```

### Comparing `typst-0.3.0/PKG-INFO` & `typst-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst
-Version: 0.3.0
+Version: 0.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python binding to typst
 License: Apache-2.0
 Requires-Python: >=3.7
```

