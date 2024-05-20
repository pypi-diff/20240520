# Comparing `tmp/renify-0.1.0.tar.gz` & `tmp/renify-0.1.1.tar.gz`

## Comparing `renify-0.1.0.tar` & `renify-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 renify-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3051 2024-02-26 13:45:49.000000 renify-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     1676 2024-02-26 13:45:49.000000 renify-0.1.0/.github/workflows/rust.yml
--rw-r--r--   0     1001      127      440 2024-02-26 13:45:49.000000 renify-0.1.0/.gitignore
--rw-r--r--   0     1001      127    22370 2024-02-26 13:46:01.000000 renify-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1066 2024-02-26 13:45:49.000000 renify-0.1.0/LICENSE
--rw-r--r--   0     1001      127     1965 2024-02-26 13:45:49.000000 renify-0.1.0/README.md
--rw-r--r--   0     1001      127  3747753 2024-02-26 13:45:49.000000 renify-0.1.0/assets/demo.gif
--rw-r--r--   0     1001      127       29 2024-02-26 13:45:49.000000 renify-0.1.0/rust-toolchain.toml
--rw-r--r--   0     1001      127     1491 2024-02-26 13:45:49.000000 renify-0.1.0/src/cli.rs
--rw-r--r--   0     1001      127    32468 2024-02-26 13:45:49.000000 renify-0.1.0/src/impl_.rs
--rw-r--r--   0     1001      127      111 2024-02-26 13:45:49.000000 renify-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127      111 2024-02-26 13:45:49.000000 renify-0.1.0/src/main.rs
--rw-r--r--   0     1001      127     1193 2024-02-26 13:45:49.000000 renify-0.1.0/src/method.rs
--rw-r--r--   0     1001      127      392 2024-02-26 13:45:49.000000 renify-0.1.0/src/target.rs
--rw-r--r--   0     1001      127     1260 2024-02-26 13:45:49.000000 renify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3230 1970-01-01 00:00:00.000000 renify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 renify-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3051 2024-05-20 06:53:20.000000 renify-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1676 2024-05-20 06:53:20.000000 renify-0.1.1/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127      440 2024-05-20 06:53:20.000000 renify-0.1.1/.gitignore
+-rw-r--r--   0     1001      127    21690 2024-05-20 06:53:32.000000 renify-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1066 2024-05-20 06:53:20.000000 renify-0.1.1/LICENSE
+-rw-r--r--   0     1001      127     1991 2024-05-20 06:53:20.000000 renify-0.1.1/README.md
+-rw-r--r--   0     1001      127  3747753 2024-05-20 06:53:20.000000 renify-0.1.1/assets/demo.gif
+-rw-r--r--   0     1001      127       29 2024-05-20 06:53:20.000000 renify-0.1.1/rust-toolchain.toml
+-rw-r--r--   0     1001      127     1376 2024-05-20 06:53:20.000000 renify-0.1.1/src/cli.rs
+-rw-r--r--   0     1001      127    35963 2024-05-20 06:53:20.000000 renify-0.1.1/src/impl_.rs
+-rw-r--r--   0     1001      127      938 2024-05-20 06:53:20.000000 renify-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127       99 2024-05-20 06:53:20.000000 renify-0.1.1/src/main.rs
+-rw-r--r--   0     1001      127     1175 2024-05-20 06:53:20.000000 renify-0.1.1/src/method.rs
+-rw-r--r--   0     1001      127      392 2024-05-20 06:53:20.000000 renify-0.1.1/src/target.rs
+-rw-r--r--   0     1001      127      302 2024-05-20 06:53:20.000000 renify-0.1.1/src/task.rs
+-rw-r--r--   0     1001      127     1260 2024-05-20 06:53:20.000000 renify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 renify-0.1.1/PKG-INFO
```

### Comparing `renify-0.1.0/Cargo.toml` & `renify-0.1.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "renify"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 description = "A simple cli tool for batch renaming files and folders, written in Rust."
 repository = "https://github.com/jamjamjon/renify"
 authors = ["Jamjamjon <jamjamjon.usls@gmail.com>"]
 license = "MIT"
```

### Comparing `renify-0.1.0/.github/workflows/ci.yml` & `renify-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `renify-0.1.0/.github/workflows/rust.yml` & `renify-0.1.1/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `renify-0.1.0/Cargo.lock` & `renify-0.1.1/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -15,143 +15,138 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.12"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b09b5178381e0874812a9b157f7fe84982617e48f71f4e3235482775e5b540"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
-
-[[package]]
-name = "bitflags"
-version = "1.3.2"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.88"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.34"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
@@ -159,17 +154,17 @@
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "console"
 version = "0.15.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e1f83fc076bd6dd27517eacdf25fef6c4dfe5f1d7448bafaaf3a26f13b5e4eb"
 dependencies = [
@@ -224,44 +219,44 @@
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
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
 name = "fastrand"
-version = "2.0.1"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
@@ -293,70 +288,75 @@
  "number_prefix",
  "portable-atomic",
  "unicode-width",
 ]
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "number_prefix"
 version = "0.4.0"
@@ -385,26 +385,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -432,36 +432,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
-name = "redox_syscall"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
-dependencies = [
- "bitflags 1.3.2",
-]
-
-[[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "renify"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "console",
  "dialoguer",
  "dirs",
@@ -469,19 +460,19 @@
  "rand",
  "uuid",
  "walkdir",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -497,196 +488,174 @@
 name = "shell-words"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24188a676b6ae68c3b2cb3a01be17fbf7240ce009799bb56d5b1409051e78fde"
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.51"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ab617d94515e94ae53b8406c628598680aa0c9587474ecbe58188f7b345d66c"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tempfile"
-version = "3.10.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a365e8cd18e44762ef95d87f284f4b5cd04107fec2ff3052bd6a3e6069669e67"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
-
-[[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -696,15 +665,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -716,109 +685,116 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d380ba1dc7187569a8a9e91ed34b8ccfc33123bbacb8c0aed2d1ad7f3ef2dc5f"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.3",
- "windows_aarch64_msvc 0.52.3",
- "windows_i686_gnu 0.52.3",
- "windows_i686_msvc 0.52.3",
- "windows_x86_64_gnu 0.52.3",
- "windows_x86_64_gnullvm 0.52.3",
- "windows_x86_64_msvc 0.52.3",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68e5dcfb9413f53afd9c8f86e56a7b4d86d9a2fa26090ea2dc9e40fba56c6ec6"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dab469ebbc45798319e69eebf92308e541ce46760b49b18c6b3fe5e8965b30f"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.3"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a4e9b6a7cac734a8b4138a4e1044eac3404d8326b6c0f939276560687a033fb"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28b0ec9c422ca95ff34a78755cfa6ad4a51371da2a5ace67500cf7ca5f232c58"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "704131571ba93e89d7cd43482277d6632589b18ecf4468f591fbae0a8b101614"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42079295511643151e98d61c38c0acc444e52dd42ab456f7ccfd5152e8ecf21c"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `renify-0.1.0/LICENSE` & `renify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renify-0.1.0/README.md` & `renify-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 
 ![Example GIF](assets/demo.gif)
 
 # Installation
 ```
 pip install renify
+# or
+cargo install renify
 ```
 
 # Usage
 ### Renaming - 重命名
 For those new to Renify, consider using the following code for **interactive mode**:
 ```bash
 renify -i <File or Folder Path>
```

### Comparing `renify-0.1.0/assets/demo.gif` & `renify-0.1.1/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `renify-0.1.0/src/cli.rs` & `renify-0.1.1/src/cli.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-use crate::{Method, Target};
+use crate::{Method, Target, Task};
 
 #[derive(clap::Parser, Debug)]
 #[command(author, version, about, long_about = None)]
 pub struct Cli {
     /// Source: File & directory
-    #[arg(short, long, required = true, value_name("Source"))]
     pub input: String,
 
     /// Target: File & directory
     #[arg(short, long, value_enum, value_name("Target"))]
     pub target: Option<Target>,
 
+    /// Tasks: rename & undo with history
+    #[arg(short, long, value_enum)]
+    pub task: Option<Task>,
+
     /// Methods for renaming
     #[arg(short, long, value_enum)]
     pub method: Option<Method>,
 
     /// Doing recursively or not
     #[arg(short, long)]
     pub recursive: Option<bool>,
@@ -45,16 +48,8 @@
     pub indiscriminate: bool,
 
     // #[arg(short, long)]
     // pub hidden_included: bool,
     /// Execute without asking
     #[arg(short, long)]
     pub yes: bool,
-
-    /// Roll back
-    #[arg(long)]
-    pub roll: bool,
-
-    /// Cache file
-    #[arg(long, default_value_t = String::from(".renify_cache"))]
-    pub cache: String,
 }
```

### Comparing `renify-0.1.0/src/impl_.rs` & `renify-0.1.1/src/impl_.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,162 +1,221 @@
 use anyhow::Result;
 use dialoguer::theme::ColorfulTheme;
-use indicatif::{ProgressBar, ProgressState, ProgressStyle};
 use rand::{distributions::Alphanumeric, thread_rng, Rng};
 use std::collections::{BTreeMap, HashMap};
 use std::io::Write;
 use std::path::{Path, PathBuf};
 use uuid::Uuid;
 use walkdir::{DirEntry, WalkDir};
 
-use crate::{Cli, Method, Target};
-
-const STR_NOT_ALLOWED: &str = "<>:/\"|?*'`"; // TODO
-const HELLO: &str = "👋 Welcome to Renify\n";
+use crate::{
+    build_progressbar, Cli, Method, Target, Task, BIT_MAX, CHECK_MARK, CROSS_MARK, INVALID_CHARS,
+};
 
 impl Cli {
     pub fn run(&mut self) -> Result<()> {
-        println!("{}", console::Style::new().white().bright().apply_to(HELLO));
-
         let theme = Self::build_theme();
-        let s = if self.roll {
-            self.roll_back()?;
-            "You have successfully reverted to the previous state!"
-        } else {
-            self.rename(&theme)?;
-            "Done!"
-        };
-        println!(
-            "\n\n{}{}",
-            console::Emoji("👏 ", ""),
-            console::Style::new().white().bright().apply_to(s)
-        );
-        println!(
-            "{}{} {} {}",
-            console::Emoji("✨ ", ""),
-            console::Style::new()
-                .white()
-                .bright()
-                .apply_to("Note that you can always use"),
-            console::Style::new()
-                .color256(49)
-                .bright()
-                .apply_to("`renify -i . --roll`"),
-            console::Style::new()
-                .white()
-                .bright()
-                .apply_to("to revert to the previous state of the modifications."),
-        );
 
+        // Task
+        self.ask_task(&theme)?;
+        match &self.task {
+            None => anyhow::bail!("{CROSS_MARK} No task specified"),
+            Some(task) => match task {
+                Task::Rename => self.rename(&theme)?,
+                Task::Undo => self.undo(&theme)?,
+            },
+        }
         Ok(())
     }
 
     pub fn rename(&mut self, theme: &ColorfulTheme) -> Result<()> {
         // source & target
         let source_type = self.check_source()?;
         self.ask_target(source_type, theme)?;
         let ys = self.fetch_targets(&self.input)?;
 
+        // cache
+        let mut dir_cache = match std::env::current_dir() {
+            Err(err) => anyhow::bail!("Cache folder get current_dir: {err}."),
+            Ok(mut d) => {
+                d.push(".renify-cache");
+                if !d.exists() {
+                    std::fs::create_dir_all(&d).expect("Cache folder failed to create: {err}.");
+                }
+                d
+            }
+        };
+
         // continue?
         if ys.is_empty() {
             self.status_log(
                 false,
                 "Found",
                 &format!("{:?} x0", self.target.unwrap()),
-                "No targets found",
+                "Not Found",
             );
         } else {
             let ntotal = ys
                 .values()
                 .fold(0, |nx, x| nx + x.values().fold(0, |ny, y| ny + y.len()));
             self.status_log(
                 true,
                 "Found",
                 &format!("{:?} x{}", self.target.unwrap(), ntotal),
                 "",
             );
 
-            // check method
+            // Method
             self.ask_method(theme)?;
 
-            // question asking according to different methods
-            match self.method.unwrap() {
-                Method::Random => self.ask_nbit(theme, ntotal)?,
-                Method::Znum => {
-                    self.ask_start_from(theme)?;
-                    self.ask_nbit(theme, ntotal + self.start.unwrap())?;
-                }
-                Method::Num => self.ask_start_from(theme)?,
-                Method::Time => self.ask_delimiter(theme)?,
-                Method::Prefix | Method::Append => {
-                    self.ask_delimiter(theme)?;
-                    self.ask_with(theme)?;
-                }
-                _ => {}
+            // Question asking
+            match &self.method {
+                None => anyhow::bail!("{CROSS_MARK} No task specified"),
+                Some(method) => match method {
+                    Method::Random => self.ask_nbit(theme, ntotal)?,
+                    Method::Znum => {
+                        self.ask_start_from(theme)?;
+                        self.ask_nbit(theme, ntotal + self.start.unwrap())?;
+                    }
+                    Method::Num => self.ask_start_from(theme)?,
+                    Method::Time => self.ask_delimiter(theme)?,
+                    Method::Prefix | Method::Append => {
+                        self.ask_delimiter(theme)?;
+                        self.ask_with(theme)?;
+                    }
+                    _ => {}
+                },
             }
 
             if !self.yes
                 && !dialoguer::Confirm::with_theme(theme)
                     .with_prompt("Ready to go")
                     .default(true)
                     .show_default(true)
                     .wait_for_newline(true)
                     .interact()?
             {
                 self.status_log(false, "Task cancelled.", "", "");
             }
-            let pb = self.build_progressbar(ntotal as u64, " Renaming".to_string());
+            let pb = build_progressbar(ntotal as u64, " Renaming");
             let mut map_pf_stem = HashMap::<PathBuf, String>::new();
             let mut map_pd_cnt: HashMap<PathBuf, usize> = HashMap::new();
+
+            // cache file
+            dir_cache.push(chrono::Local::now().format("%Y%m%d%H%M%S%f").to_string());
             let mut f_cache = std::fs::OpenOptions::new()
                 .read(true)
                 .write(true)
                 .create(true)
                 .truncate(true)
-                .open(&self.cache)?;
+                .open(dir_cache)?;
 
             // loop
             for (_, paths) in ys.iter().rev() {
                 for (pd, pfs) in paths.iter() {
                     for pf in pfs.iter() {
                         pb.inc(1);
-                        let path_new = self.gen_uniq(pf, pd, &mut map_pd_cnt, &mut map_pf_stem);
+                        let path_new = self.gen_uniq(pf, pd, &mut map_pd_cnt, &mut map_pf_stem)?;
                         self.rename_and_cache(pf, &path_new, &mut f_cache)?;
                     }
                 }
             }
             pb.finish();
         }
         Ok(())
     }
 
-    pub fn roll_back(&self) -> Result<()> {
-        if !std::path::Path::new(&self.cache).exists() {
-            self.status_log(
-                false,
-                "Execution cache",
-                "Not Found",
-                "Please run renify beforehand",
-            );
-        }
-        let contents = std::fs::read_to_string(&self.cache)?;
-        let pb =
-            self.build_progressbar(contents.lines().count() as u64, " Rolling Back".to_string());
-        let mut f_cache = std::fs::OpenOptions::new()
-            .read(true)
-            .write(true)
-            .create(true)
-            .truncate(true)
-            .open(&self.cache)?;
-        for line in contents.lines().rev() {
-            pb.inc(1);
-            let v: Vec<&str> = line.split(' ').collect();
-            self.rename_and_cache(v[1], v[0], &mut f_cache)?;
-        }
-        pb.finish();
+    fn undo(&self, theme: &ColorfulTheme) -> Result<()> {
+        match std::env::current_dir() {
+            Err(err) => anyhow::bail!("Cache folder get current_dir: {err}."),
+            Ok(mut d) => {
+                d.push(".renify-cache");
+                if !d.exists() {
+                    self.status_log(
+                        false,
+                        "Failed to undo",
+                        "No caches found",
+                        "Please run renify beforehand",
+                    );
+                } else {
+                    // glob
+                    let mut ys = Vec::new();
+                    for entry in d.read_dir().expect("read_dir call failed").flatten() {
+                        ys.push(entry.path().to_str().unwrap().to_string());
+                    }
+
+                    if ys.is_empty() {
+                        self.status_log(
+                            false,
+                            "Failed to undo",
+                            "No caches found",
+                            "Please run renify beforehand",
+                        );
+                    }
+
+                    // sort
+                    ys.sort_by(|a, b| {
+                        std::fs::metadata(a)
+                            .unwrap()
+                            .modified()
+                            .unwrap()
+                            .partial_cmp(&std::fs::metadata(b).unwrap().modified().unwrap())
+                            .unwrap()
+                            .reverse()
+                    });
+
+                    // asking
+                    let i = dialoguer::Select::with_theme(theme)
+                        .with_prompt("Cache")
+                        .default(0)
+                        .items(&ys[..])
+                        .interact()?;
+
+                    // undo
+                    let yys: Vec<_> = ys.drain(i + 1..).collect();
+                    for y in ys.iter() {
+                        let contents = match std::fs::read_to_string(y) {
+                            Ok(s) => s,
+                            Err(err) => {
+                                anyhow::bail!("Error when read_to_string: {err}")
+                            }
+                        };
+                        let pb = build_progressbar(contents.lines().count() as u64, " Undoing");
+                        for line in contents.lines().rev() {
+                            pb.inc(1);
+                            let v: Vec<&str> = line.split(' ').collect();
+                            match std::fs::rename(v[1], v[0]) {
+                                Ok(_) => {}
+                                Err(err) => {
+                                    anyhow::bail!("Error when renaming: {err}")
+                                }
+                            };
+                        }
+                        match std::fs::remove_file(y) {
+                            Ok(_) => {}
+                            Err(err) => {
+                                anyhow::bail!("Error when removing file: {err}")
+                            }
+                        }
+                        pb.finish();
+                    }
+
+                    // cleanup
+                    if yys.is_empty() {
+                        match std::fs::remove_dir(d) {
+                            Ok(_) => {}
+                            Err(err) => {
+                                anyhow::bail!("Error when removing directory: {err}")
+                            }
+                        }
+                    }
+                }
+            }
+        };
+
         Ok(())
     }
 
     fn fetch_targets<P: AsRef<Path>>(
         &self,
         source: P,
     ) -> Result<BTreeMap<usize, BTreeMap<PathBuf, Vec<PathBuf>>>> {
@@ -272,95 +331,101 @@
 
     pub fn gen_uniq(
         &self,
         pf: &Path,
         pd: &Path,
         map_pd_cnt: &mut HashMap<PathBuf, usize>,
         map_pf_stem: &mut HashMap<PathBuf, String>,
-    ) -> PathBuf {
-        // generate unique file stem
+    ) -> Result<PathBuf> {
+        // Generate unique file stem
         if !self.indiscriminate {
             if let Target::File = self.target.unwrap() {
                 let path_wo_ext = pf.with_extension("");
                 if !map_pf_stem.is_empty() && map_pf_stem.contains_key(&path_wo_ext) {
                     let _stem = &map_pf_stem[&path_wo_ext];
                     let mut path_new = pf.with_file_name(_stem);
                     if let Some(suffix) = pf.extension() {
                         path_new = path_new.with_extension(suffix);
                     }
-                    return path_new;
+                    return Ok(path_new);
                 }
             }
         }
 
         loop {
-            let stem = match self.method.unwrap() {
-                Method::Time => chrono::Local::now()
-                    .format(&format!(
-                        "%Y{}%m{}%d{}%H{}%M{}%S{}%f",
-                        self.delimiter.as_ref().unwrap(),
-                        self.delimiter.as_ref().unwrap(),
-                        self.delimiter.as_ref().unwrap(),
-                        self.delimiter.as_ref().unwrap(),
-                        self.delimiter.as_ref().unwrap(),
-                        self.delimiter.as_ref().unwrap()
-                    ))
-                    .to_string(),
-                Method::Uuid => Uuid::new_v4().to_string(),
-                Method::Prefix => {
-                    assert!(
+            let stem = match &self.method {
+                None => anyhow::bail!("{CROSS_MARK} No task specified"),
+                Some(method) => match method {
+                    Method::Time => chrono::Local::now()
+                        .format(&format!(
+                            "%Y{}%m{}%d{}%H{}%M{}%S{}%f",
+                            self.delimiter.as_ref().unwrap(),
+                            self.delimiter.as_ref().unwrap(),
+                            self.delimiter.as_ref().unwrap(),
+                            self.delimiter.as_ref().unwrap(),
+                            self.delimiter.as_ref().unwrap(),
+                            self.delimiter.as_ref().unwrap()
+                        ))
+                        .to_string(),
+                    Method::Uuid => Uuid::new_v4().to_string(),
+                    Method::Prefix => {
+                        assert!(
                             self.with.is_some(),
                             "> You should set the prefix content by `--with` when using `Method::Prefix`."
                         );
-                    let stem = pf.file_stem().unwrap().to_str().unwrap();
-                    format!(
-                        "{}{}{}",
-                        self.with.clone().unwrap(),
-                        self.delimiter.as_ref().unwrap(),
-                        stem
-                    )
-                }
-                Method::Append => {
-                    assert!(
+                        let stem = pf.file_stem().unwrap().to_str().unwrap();
+                        format!(
+                            "{}{}{}",
+                            self.with.clone().unwrap(),
+                            self.delimiter.as_ref().unwrap(),
+                            stem
+                        )
+                    }
+                    Method::Append => {
+                        assert!(
                             self.with.is_some(),
                             "> You should set the postfix content by `--with` when using `Method::Append`."
                         );
-                    let stem = pf.file_stem().unwrap().to_str().unwrap();
-                    format!(
-                        "{}{}{}",
-                        stem,
-                        self.delimiter.as_ref().unwrap(),
-                        self.with.clone().unwrap()
-                    )
-                }
-                Method::Num | Method::Znum => {
-                    let count = map_pd_cnt
-                        .entry(pd.to_path_buf())
-                        .or_insert(self.start.unwrap() - 1);
-                    *count += 1;
-                    if let Method::Znum = self.method.unwrap() {
-                        format!("{:0>1$}", count, self.nbits.unwrap())
-                    } else {
+                        let stem = pf.file_stem().unwrap().to_str().unwrap();
+                        format!(
+                            "{}{}{}",
+                            stem,
+                            self.delimiter.as_ref().unwrap(),
+                            self.with.clone().unwrap()
+                        )
+                    }
+                    Method::Num => {
+                        let count = map_pd_cnt
+                            .entry(pd.to_path_buf())
+                            .or_insert(self.start.unwrap() - 1);
+                        *count += 1;
                         count.to_string()
                     }
-                }
-                Method::Random => thread_rng()
-                    .sample_iter(&Alphanumeric)
-                    .take(self.nbits.unwrap())
-                    .map(char::from)
-                    .collect(),
-                // Method::Lowercase => {
-                //     let stem = pf.file_stem().unwrap().to_str().unwrap().to_lowercase();
-                //     stem
-                // }
-                // Method::Uppercase => {
-                //     let stem = pf.file_stem().unwrap().to_str().unwrap().to_uppercase();
-                //     stem
-                // }
-                _ => todo!(),
+                    Method::Znum => {
+                        let count = map_pd_cnt
+                            .entry(pd.to_path_buf())
+                            .or_insert(self.start.unwrap() - 1);
+                        *count += 1;
+                        format!("{:0>1$}", count, self.nbits.unwrap())
+                    }
+                    Method::Random => thread_rng()
+                        .sample_iter(&Alphanumeric)
+                        .take(self.nbits.unwrap())
+                        .map(char::from)
+                        .collect(),
+                    // Method::Lowercase => {
+                    //     let stem = pf.file_stem().unwrap().to_str().unwrap().to_lowercase();
+                    //     stem
+                    // }
+                    // Method::Uppercase => {
+                    //     let stem = pf.file_stem().unwrap().to_str().unwrap().to_uppercase();
+                    //     stem
+                    // }
+                    // _ => todo!(),
+                },
             };
 
             // check if new stem file exists
             let mut p_new = pf.with_file_name(stem);
 
             // extend with suffix
             if let Some(suffix) = pf.extension() {
@@ -373,22 +438,25 @@
                     let _stem = p_new.file_stem().unwrap().to_str().unwrap().to_string();
                     let path_wo_ext = pf.with_extension("");
                     map_pf_stem.insert(path_wo_ext, _stem);
                 }
             }
 
             if !p_new.exists() {
-                break p_new;
+                break Ok(p_new);
             } else {
-                match self.method.unwrap() {
-                    // Method::Uppercase | Method::Lowercase | Method::Num | Method::Znum => {
-                    Method::Num | Method::Znum => {
-                        break pf.to_path_buf();
-                    }
-                    _ => {}
+                match &self.method {
+                    None => anyhow::bail!("{CROSS_MARK} No task specified"),
+                    Some(method) => match method {
+                        // Method::Uppercase | Method::Lowercase | Method::Num | Method::Znum => {
+                        Method::Num | Method::Znum => {
+                            break Ok(pf.to_path_buf());
+                        }
+                        _ => {}
+                    },
                 }
             }
         }
     }
 
     fn _is_hidden(&self, entry: &DirEntry) -> bool {
         entry
@@ -438,24 +506,24 @@
         if status {
             print!(
                 "{}",
                 console::Style::new()
                     .bold()
                     .color256(49)
                     .bright()
-                    .apply_to("✔  ")
+                    .apply_to(format!("{}  ", CHECK_MARK))
             );
         } else {
             print!(
                 "{}",
                 console::Style::new()
                     .bold()
                     .color256(9)
                     .bright()
-                    .apply_to("✘  ")
+                    .apply_to(format!("{}  ", CROSS_MARK))
             );
         }
 
         // t1
         print!(
             "{}",
             console::Style::new().white().bold().bright().apply_to(t1)
@@ -507,22 +575,51 @@
             true,
             "Source",
             match type_ {
                 Target::Dir | Target::File => p,
                 Target::Symlink => &self.input,
             },
             match type_ {
-                Target::Dir => "A Folder",
-                Target::File => "A File",
-                Target::Symlink => "A Symlink",
+                Target::Dir => "Folders",
+                Target::File => "Files",
+                Target::Symlink => "Symlinks",
             },
         );
         Ok(type_)
     }
 
+    fn ask_task(&mut self, theme: &ColorfulTheme) -> Result<()> {
+        match &self.task {
+            None => {
+                let selections = &["Rename", "Undo with history"];
+                let i = dialoguer::Select::with_theme(theme)
+                    .with_prompt("Task")
+                    .default(0)
+                    .items(&selections[..])
+                    .interact()?;
+                self.task = Some(Task::from(selections[i]));
+            }
+            Some(task) => {
+                self.status_log(
+                    true,
+                    "Task",
+                    &format!("{:?}", task),
+                    &format!(
+                        "--task {}",
+                        match task {
+                            Task::Rename => "Rename",
+                            Task::Undo => "Undo",
+                        }
+                    ),
+                );
+            }
+        }
+        Ok(())
+    }
+
     fn ask_target(&mut self, source_type: Target, theme: &ColorfulTheme) -> Result<()> {
         match source_type {
             Target::Symlink => {
                 self.status_log(false, "Source Error", "Not Supported", "Symlink");
             }
             Target::File => {
                 self.target = Some(Target::File);
@@ -572,32 +669,30 @@
             );
         }
 
         Ok(())
     }
 
     fn ask_method(&mut self, theme: &ColorfulTheme) -> Result<()> {
-        match self.method {
+        match &self.method {
             None => {
                 let selections = &[
                     "Random",
                     "Uuid",
                     "Time",
                     "Numbered",
-                    "Zero-Numbered",
+                    "ZeroNumbered",
                     "Prefix",
                     "Append",
-                    // "Lowercase",
-                    // "Uppercase",
                 ];
                 let i = dialoguer::Select::with_theme(theme)
-                    .with_prompt("Select method")
+                    .with_prompt("Method")
                     .default(0)
-                    .max_length(10)
-                    .items(&selections[..])
+                    // .max_length(10)
+                    .items(selections)
                     .interact()?;
                 self.method = Some(Method::from(selections[i]));
             }
             Some(method) => {
                 self.status_log(
                     true,
                     "Method",
@@ -608,15 +703,14 @@
                             Method::Random => "random",
                             Method::Time => "time",
                             Method::Num => "num",
                             Method::Znum => "znum",
                             Method::Prefix => "prefix",
                             Method::Append => "append",
                             Method::Uuid => "uuid",
-                            _ => "",
                         }
                     ),
                 );
             }
         }
         Ok(())
     }
@@ -697,31 +791,33 @@
             num /= base;
         }
         result.chars().rev().collect()
     }
 
     fn ask_nbit(&mut self, theme: &ColorfulTheme, ntotal: usize) -> Result<()> {
         //  calculate the bit_min
-        let n_min = match self.method.unwrap() {
-            Method::Znum => ntotal.to_string().len(),
-            Method::Random => Self::decimal_to_62(ntotal).len(),
-            _ => 0,
+        let n_min = match &self.method {
+            None => anyhow::bail!("{CROSS_MARK} No task specified"),
+            Some(method) => match method {
+                Method::Znum => ntotal.to_string().len(),
+                Method::Random => Self::decimal_to_62(ntotal).len(),
+                _ => 0,
+            },
         };
-        let n_max = n_min + 5;
-        let err_msg = format!("It should be between {} to {}.", n_min, n_max);
+        let err_msg = format!("It should be between {} to {}.", n_min, BIT_MAX);
         match self.nbits {
             None => {
                 self.nbits = Some(
                     dialoguer::Input::with_theme(theme)
                         .with_prompt("The number of bits")
                         .with_initial_text(n_min.to_string())
                         .validate_with(|input: &String| -> Result<(), &str> {
                             match input.parse::<usize>() {
                                 Ok(n) => {
-                                    if !(n_min..=n_max).contains(&n) {
+                                    if !(n_min..=BIT_MAX).contains(&n) {
                                         Err(&err_msg)
                                     } else {
                                         Ok(())
                                     }
                                 }
                                 Err(_) => Err("This is not a number!"),
                             }
@@ -729,15 +825,15 @@
                         .allow_empty(false)
                         .interact_text()?
                         .parse::<usize>()?,
                 );
             }
             Some(n) => {
                 // validate
-                if !(n_min..=n_max).contains(&n) {
+                if !(n_min..=BIT_MAX).contains(&n) {
                     self.status_log(false, "The number of bits", &n.to_string(), &err_msg);
                 }
                 self.status_log(
                     true,
                     "The number of bits",
                     &format!("{:?}", n),
                     &format!("--nbits {}", n),
@@ -745,28 +841,25 @@
             }
         }
 
         Ok(())
     }
 
     fn ask_depth(&mut self, theme: &ColorfulTheme) -> Result<()> {
-        let depth_max = self.max_depth(&self.input);
+        let max_ = self.max_depth(&self.input);
         match self.depth {
             None => {
                 let depth = dialoguer::Input::with_theme(theme)
-                    .with_prompt(format!(
-                        "The depth of folder (max: {}, 0: to the end)",
-                        depth_max
-                    ))
-                    .with_initial_text("0".to_string())
+                    .with_prompt("Depth")
+                    .with_initial_text(max_.to_string())
                     .validate_with(|input: &String| -> Result<(), &str> {
                         match input.parse::<usize>() {
                             Ok(n) => {
-                                if !(0..=depth_max).contains(&n) {
-                                    Err("It should be between 0 to max depth found.")
+                                if !(0..=max_).contains(&n) {
+                                    Err("It should be between 0 and `max_depth` given.")
                                 } else {
                                     Ok(())
                                 }
                             }
                             Err(_) => Err("This is not a number!"),
                         }
                     })
@@ -785,26 +878,26 @@
             }
         }
         Ok(())
     }
 
     fn ask_delimiter(&mut self, theme: &ColorfulTheme) -> Result<()> {
         let err_msg = format!(
-            "Wrong char! These are usually not allowed: {}",
-            STR_NOT_ALLOWED
+            "Illegal characters! These are usually not allowed: {}",
+            INVALID_CHARS
         );
         match &self.delimiter {
             None => {
                 self.delimiter = Some(
                     dialoguer::Input::with_theme(theme)
                         .with_prompt("Delimiter")
                         .with_initial_text("-".to_string())
                         .validate_with({
                             |input: &String| -> Result<(), &str> {
-                                if input.as_str().chars().any(|c| STR_NOT_ALLOWED.contains(c)) {
+                                if input.as_str().chars().any(|c| INVALID_CHARS.contains(c)) {
                                     Err(&err_msg)
                                 } else {
                                     Ok(())
                                 }
                             }
                         })
                         .allow_empty(true)
@@ -822,25 +915,25 @@
         }
 
         Ok(())
     }
 
     fn ask_with(&mut self, theme: &ColorfulTheme) -> Result<()> {
         let err_msg = format!(
-            "Wrong char! These are usually not allowed: {}",
-            STR_NOT_ALLOWED
+            "Illegal characters! These are usually not allowed: {}",
+            INVALID_CHARS
         );
         match &self.with {
             None => {
                 self.with = Some(
                     dialoguer::Input::with_theme(theme)
                         .with_prompt("What text with")
                         .validate_with({
                             |input: &String| -> Result<(), &str> {
-                                if input.as_str().chars().any(|c| STR_NOT_ALLOWED.contains(c)) {
+                                if input.as_str().chars().any(|c| INVALID_CHARS.contains(c)) {
                                     Err(&err_msg)
                                 } else {
                                     Ok(())
                                 }
                             }
                         })
                         .allow_empty(false)
@@ -861,51 +954,38 @@
             defaults_style: console::Style::new().bold().color256(49),
             hint_style: console::Style::new().white().dim(),
             values_style: console::Style::new().color256(49).bright(),
             prompt_style: console::Style::new().white().bold().bright(),
             prompt_prefix: console::Style::new()
                 .bold()
                 .color256(9)
-                .apply_to("? ".to_string()),
+                .apply_to("❓ ".to_string()),
             prompt_suffix: console::Style::new().white().dim().apply_to("› ".into()),
             success_prefix: console::Style::new()
                 .bold()
                 .color256(49)
                 .bright()
-                .apply_to("✔ ".to_string()),
+                .apply_to(format!("{} ", CHECK_MARK)),
             success_suffix: console::Style::new()
                 .bold()
                 .white()
                 .dim()
                 .apply_to("·".to_string()),
             error_prefix: console::Style::new()
                 .bold()
                 .color256(9)
                 .bright()
-                .apply_to("✘ ".to_string()),
+                .apply_to(format!("{} ", CROSS_MARK)),
             error_style: console::Style::new().color256(9).bold().bright(),
             active_item_prefix: console::Style::new()
                 .bold()
                 .apply_to(console::Emoji("👉", "").to_string()),
             inactive_item_prefix: console::Style::new()
                 .white()
                 .dim()
                 .apply_to("  ".to_string()),
             active_item_style: console::Style::new().bold().color256(49).bright(),
             inactive_item_style: console::Style::new().white().dim(),
             ..Default::default()
         }
     }
-
-    fn build_progressbar(&self, size: u64, prefix: String) -> ProgressBar {
-        let pb = ProgressBar::new(size);
-        pb.set_style(
-            ProgressStyle::with_template(
-                "{spinner:.green.bold} {prefix:.bold} [{bar:.magenta.bright.bold/white.dim}] {human_pos}/{human_len} ({percent}% | {eta} | {elapsed_precise})"
-            )
-            .unwrap()
-            .with_key("eta", |state: &ProgressState, w: &mut dyn std::fmt::Write | write!(w, "{:.2}s", state.eta().as_secs_f64()).unwrap())
-            .progress_chars("#>-"));
-        pb.set_prefix(prefix);
-        pb
-    }
 }
```

### Comparing `renify-0.1.0/pyproject.toml` & `renify-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `renify-0.1.0/PKG-INFO` & `renify-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: renify
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
@@ -40,14 +40,16 @@
 
 
 ![Example GIF](assets/demo.gif)
 
 # Installation
 ```
 pip install renify
+# or
+cargo install renify
 ```
 
 # Usage
 ### Renaming - 重命名
 For those new to Renify, consider using the following code for **interactive mode**:
 ```bash
 renify -i <File or Folder Path>
```

