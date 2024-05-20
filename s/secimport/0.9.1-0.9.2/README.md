# Comparing `tmp/secimport-0.9.1.tar.gz` & `tmp/secimport-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.9.1.tar", max compression
+gzip compressed data, was "secimport-0.9.2.tar", max compression
```

## Comparing `secimport-0.9.1.tar` & `secimport-0.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1069 2023-07-11 14:18:19.681406 secimport-0.9.1/LICENSE
--rw-r--r--   0        0        0    13200 2023-07-11 14:18:19.681406 secimport-0.9.1/README.md
--rw-r--r--   0        0        0     1719 2023-07-11 14:18:19.681406 secimport-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      437 2023-07-11 14:18:19.681406 secimport-0.9.1/secimport/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      362 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      125 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      110 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       72 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       71 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0     8757 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22263 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0     1645 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       67 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      176 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       40 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      553 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1203 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/new_template.bt
--rw-r--r--   0        0        0      502 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0      112 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0    10949 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/system_calls.py
--rw-r--r--   0        0        0     8885 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      415 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      662 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      134 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      124 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       64 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1606 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1081 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1753 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2587 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0     8813 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      172 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      177 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       31 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      436 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      969 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       30 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1238 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4389 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0    16216 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/cli.py
--rwxr-xr-x   0        0        0    22294 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3098 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/sandbox_helper.py
--rw-r--r--   0        0        0    13923 1970-01-01 00:00:00.000000 secimport-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-11-27 14:34:20.057666 secimport-0.9.2/LICENSE
+-rw-r--r--   0        0        0    13750 2023-11-27 14:34:20.057666 secimport-0.9.2/README.md
+-rw-r--r--   0        0        0     1719 2023-11-27 14:34:20.061666 secimport-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8757 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22263 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0     1645 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0    10949 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/common/system_calls.py
+-rw-r--r--   0        0        0     8885 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    16746 2023-11-27 14:34:20.061666 secimport-0.9.2/secimport/cli.py
+-rwxr-xr-x   0        0        0    22257 2023-11-27 14:34:20.065666 secimport-0.9.2/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3098 2023-11-27 14:34:20.065666 secimport-0.9.2/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0    14524 1970-01-01 00:00:00.000000 secimport-0.9.2/PKG-INFO
```

### Comparing `secimport-0.9.1/LICENSE` & `secimport-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/README.md` & `secimport-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,739 +87,774 @@
 00000560: 6420 7361 6e64 626f 7820 746f 6f6c 6b69  d sandbox toolki
 00000570: 742e 3c62 723e 0a49 7420 7472 6163 6573  t.<br>.It traces
 00000580: 2079 6f75 7220 636f 6465 2c20 616e 6420   your code, and 
 00000590: 7275 6e73 2061 6e20 6578 6563 7574 6162  runs an executab
 000005a0: 6c65 2074 6861 7420 616c 6c6f 7773 206f  le that allows o
 000005b0: 6e6c 7920 7468 6520 7361 6d65 2073 7973  nly the same sys
 000005c0: 6361 6c6c 732c 2070 6572 206d 6f64 756c  calls, per modul
-000005d0: 652e 0a0a 2323 2320 5468 6520 7072 6f62  e...### The prob
-000005e0: 6c65 6d0a 5472 6164 6974 696f 6e61 6c20  lem.Traditional 
-000005f0: 746f 6f6c 7320 6c69 6b65 2073 6563 636f  tools like secco
-00000600: 6d70 206f 7220 4170 7041 726d 6f72 2065  mp or AppArmor e
-00000610: 6e66 6f72 6365 2073 7973 6361 6c6c 7320  nforce syscalls 
-00000620: 666f 7220 7468 6520 656e 7469 7265 2070  for the entire p
-00000630: 726f 6365 7373 2e3c 6272 3e53 6f6d 6574  rocess.<br>Somet
-00000640: 6869 6e67 206c 696b 6520 6061 6c6c 6f77  hing like `allow
-00000650: 6564 5f73 7973 6361 6c6c 733d 5b22 7265  ed_syscalls=["re
-00000660: 6164 222c 226f 7065 6e61 7422 2c22 6269  ad","openat","bi
-00000670: 6e64 222c 2277 7269 7465 225d 602c 2077  nd","write"]`, w
-00000680: 6869 6368 2069 7320 6772 6561 742c 2062  hich is great, b
-00000690: 7574 206e 6f74 2065 6e6f 7567 6820 666f  ut not enough fo
-000006a0: 7220 7079 7468 6f6e 2773 2061 7474 6163  r python's attac
-000006b0: 6b20 7375 7266 6163 652e 3c62 723e 0a0a  k surface.<br>..
-000006c0: 2323 2320 5468 6520 736f 6c75 7469 6f6e  ### The solution
-000006d0: 0a60 7365 6369 6d70 6f72 7460 2069 7320  .`secimport` is 
-000006e0: 6162 6c65 2074 6f20 7472 6163 6520 7768  able to trace wh
-000006f0: 6963 6820 7379 7363 616c 6c73 2065 6163  ich syscalls eac
-00000700: 6820 6d6f 6475 6c65 2069 6e20 796f 7572  h module in your
-00000710: 2063 6f64 6520 7573 6573 2028 6279 2070   code uses (by p
-00000720: 6163 6b61 6765 206e 616d 6529 2e3c 6272  ackage name).<br
-00000730: 3e0a 4166 7465 7220 7472 6163 696e 672c  >.After tracing,
-00000740: 2073 6563 696d 706f 7274 2063 7265 6174   secimport creat
-00000750: 6573 2061 204a 534f 4e2f 5941 4d4c 2070  es a JSON/YAML p
-00000760: 6f6c 6963 7920 666f 7220 796f 7572 2063  olicy for your c
-00000770: 6f64 652e 2049 7420 636f 6d70 696c 6573  ode. It compiles
-00000780: 2069 7420 696e 746f 2061 2068 6967 682d   it into a high-
-00000790: 7065 7266 6f72 6d61 6e63 6520 6542 5046  performance eBPF
-000007a0: 2069 6e73 7472 756d 656e 7461 7469 6f6e   instrumentation
-000007b0: 2073 6372 6970 7420 2873 6d61 6c6c 6572   script (smaller
-000007c0: 2074 6865 6e20 3531 3220 6279 7465 7320   then 512 bytes 
-000007d0: 6f76 6572 616c 6c29 2c20 7468 6174 206c  overall), that l
-000007e0: 6f6f 6b73 206c 696b 6520 3c61 3e74 6869  ooks like <a>thi
-000007f0: 733c 2f61 3e2e 0a60 6060 0a6d 6f64 756c  s</a>..```.modul
-00000800: 6573 3a0a 2020 7265 7175 6573 7473 3a0a  es:.  requests:.
-00000810: 2020 2020 6465 7374 7275 6374 6976 653a      destructive:
-00000820: 2074 7275 6520 2020 2020 2320 7768 656e   true     # when
-00000830: 2074 7275 652c 2073 6563 696d 706f 7274   true, secimport
-00000840: 2077 696c 6c20 6b69 6c6c 206f 6e20 7669   will kill on vi
-00000850: 6c61 7469 6f6e 2069 6e73 7465 6164 206f  lation instead o
-00000860: 6620 6c6f 6767 696e 672e 0a20 2020 2073  f logging..    s
-00000870: 7973 6361 6c6c 5f61 6c6c 6f77 6c69 7374  yscall_allowlist
-00000880: 3a0a 2020 2020 2020 2d20 6663 686d 6f64  :.      - fchmod
-00000890: 0a20 2020 2020 202d 2067 6574 656e 7472  .      - getentr
-000008a0: 6f70 790a 2020 2020 2020 2d20 6765 7470  opy.      - getp
-000008b0: 6772 700a 2020 2020 2020 2d20 6765 7472  grp.      - getr
-000008c0: 6c69 6d69 740a 2e2e 2e0a 6060 600a 596f  limit.....```.Yo
-000008d0: 7520 6361 6e20 616c 736f 2075 7365 204a  u can also use J
-000008e0: 534f 4e20 696e 7374 6165 6164 206f 6620  SON instaead of 
-000008f0: 5941 4d4c 2c20 616e 6420 6576 656e 2063  YAML, and even c
-00000900: 6f6e 6669 6e65 2062 7569 6c74 696e 2070  onfine builtin p
-00000910: 7974 686f 6e20 6d6f 6475 6c65 732e 3c62  ython modules.<b
-00000920: 723e 0a41 6e20 6578 616d 706c 6520 706f  r>.An example po
-00000930: 6c69 6379 2074 6861 7420 7573 6573 206c  licy that uses l
-00000940: 6f67 6769 6e67 2c20 6d75 6c74 6970 726f  ogging, multipro
-00000950: 6365 7373 696e 672c 206f 7320 616e 6420  cessing, os and 
-00000960: 6669 6c65 7379 7374 656d 2077 696c 6c20  filesystem will 
-00000970: 6c6f 6f6b 2061 7070 726f 7869 6d61 7465  look approximate
-00000980: 6c79 206c 696b 6520 7468 6973 3a0a 6060  ly like this:.``
-00000990: 600a 2e2e 2e0a 2020 2020 222f 776f 726b  `.....    "/work
-000009a0: 7370 6163 652f 5079 7468 6f6e 2d33 2e31  space/Python-3.1
-000009b0: 302e 302f 4c69 622f 6c6f 6767 696e 672f  0.0/Lib/logging/
-000009c0: 5f5f 696e 6974 5f5f 2e70 7922 3a20 5b0a  __init__.py": [.
-000009d0: 2020 2020 2020 2020 2220 636c 6f63 6b5f          " clock_
-000009e0: 6765 7474 696d 6522 2c0a 2020 2020 2020  gettime",.      
-000009f0: 2020 2220 6765 7470 6964 222c 0a20 2020    " getpid",.   
-00000a00: 2020 2020 2022 2077 7269 7465 220a 2020       " write".  
-00000a10: 2020 5d2c 0a20 2020 2022 2f77 6f72 6b73    ],.    "/works
-00000a20: 7061 6365 2f50 7974 686f 6e2d 332e 3130  pace/Python-3.10
-00000a30: 2e30 2f4c 6962 2f6d 756c 7469 7072 6f63  .0/Lib/multiproc
-00000a40: 6573 7369 6e67 2f70 726f 6365 7373 2e70  essing/process.p
-00000a50: 7922 3a20 5b0a 2020 2020 2020 2020 2220  y": [.        " 
-00000a60: 6765 7463 7764 222c 0a20 2020 2020 2020  getcwd",.       
-00000a70: 2022 2067 6574 7069 6422 2c0a 2020 2020   " getpid",.    
-00000a80: 2020 2020 2220 6765 7472 616e 646f 6d22      " getrandom"
-00000a90: 0a20 2020 205d 2c0a 2020 2020 222f 776f  .    ],.    "/wo
-00000aa0: 726b 7370 6163 652f 5079 7468 6f6e 2d33  rkspace/Python-3
-00000ab0: 2e31 302e 302f 4c69 622f 6d75 6c74 6970  .10.0/Lib/multip
-00000ac0: 726f 6365 7373 696e 672f 7574 696c 2e70  rocessing/util.p
-00000ad0: 7922 3a20 5b0a 2020 2020 2020 2020 2220  y": [.        " 
-00000ae0: 7072 6c69 6d69 7436 3422 0a20 2020 205d  prlimit64".    ]
-00000af0: 2c0a 2020 2020 222f 776f 726b 7370 6163  ,.    "/workspac
-00000b00: 652f 5079 7468 6f6e 2d33 2e31 302e 302f  e/Python-3.10.0/
-00000b10: 4c69 622f 6f73 2e70 7922 3a20 5b0a 2020  Lib/os.py": [.  
-00000b20: 2020 2020 2020 2220 7265 6164 220a 2020        " read".  
-00000b30: 2020 5d2c 0a20 2020 2022 2f77 6f72 6b73    ],.    "/works
-00000b40: 7061 6365 2f50 7974 686f 6e2d 332e 3130  pace/Python-3.10
-00000b50: 2e30 2f4c 6962 2f70 6c61 7466 6f72 6d2e  .0/Lib/platform.
-00000b60: 7079 223a 205b 0a20 2020 2020 2020 2022  py": [.        "
-00000b70: 2075 6e61 6d65 220a 2020 2020 5d2c 0a20   uname".    ],. 
-00000b80: 2020 2022 2f77 6f72 6b73 7061 6365 2f50     "/workspace/P
-00000b90: 7974 686f 6e2d 332e 3130 2e30 2f4c 6962  ython-3.10.0/Lib
-00000ba0: 2f70 6f73 6978 7061 7468 2e70 7922 3a20  /posixpath.py": 
-00000bb0: 5b0a 2020 2020 2020 2020 2220 636c 6f73  [.        " clos
-00000bc0: 6522 2c0a 2020 2020 2020 2020 2220 6673  e",.        " fs
-00000bd0: 7461 7422 2c0a 2020 2020 2020 2020 2220  tat",.        " 
-00000be0: 6765 7463 7764 222c 0a20 2020 2020 2020  getcwd",.       
-00000bf0: 2022 2067 6574 6465 6e74 7336 3422 2c0a   " getdents64",.
-00000c00: 2020 2020 2020 2020 2220 6f70 656e 6174          " openat
-00000c10: 220a 2020 2020 5d2c 0a20 2020 2022 2f77  ".    ],.    "/w
-00000c20: 6f72 6b73 7061 6365 2f50 7974 686f 6e2d  orkspace/Python-
-00000c30: 332e 3130 2e30 2f4c 6962 2f72 616e 646f  3.10.0/Lib/rando
-00000c40: 6d2e 7079 223a 205b 0a20 2020 2020 2020  m.py": [.       
-00000c50: 2022 2067 6574 7261 6e64 6f6d 220a 2020   " getrandom".  
-00000c60: 2020 5d2c 0a2e 2e2e 0a60 6060 0a49 7420    ],.....```.It 
-00000c70: 7761 7320 6372 6561 7465 6420 6279 2074  was created by t
-00000c80: 7261 6369 6e67 2074 6865 2063 6f64 652e  racing the code.
-00000c90: 2073 6563 696d 706f 7274 2061 7574 6f6d   secimport autom
-00000ca0: 6174 6963 616c 6c79 2066 696e 6473 2074  atically finds t
-00000cb0: 6865 7365 2070 6572 2d6d 6f64 756c 6520  hese per-module 
-00000cc0: 7379 7363 616c 6c73 2066 6f72 2079 6f75  syscalls for you
-00000cd0: 2e0a 0a46 696e 616c 6c79 2c20 796f 7520  ...Finally, you 
-00000ce0: 636f 6e76 6572 7420 7468 6973 2070 6f6c  convert this pol
-00000cf0: 6963 7920 696e 746f 2061 6e20 7361 6e64  icy into an sand
-00000d00: 626f 7820 2865 4250 4620 696e 7374 7275  box (eBPF instru
-00000d10: 6d65 6e74 6174 696f 6e20 7363 7269 7074  mentation script
-00000d20: 2920 746f 2072 756e 2074 6865 2070 7974  ) to run the pyt
-00000d30: 686f 6e20 7072 6f63 6573 7320 696e 2070  hon process in p
-00000d40: 726f 6475 6374 696f 6e2e 2052 756e 6e69  roduction. Runni
-00000d50: 6e67 2074 6865 2073 616e 6462 6f78 2077  ng the sandbox w
-00000d60: 696c 6c20 656e 666f 7265 2070 7974 686f  ill enfore pytho
-00000d70: 6e20 746f 206f 6265 7920 616e 7920 6769  n to obey any gi
-00000d80: 7665 6e20 706f 6c69 6379 2e0a 0a60 7365  ven policy...`se
-00000d90: 6369 6d70 6f72 7460 2069 7320 6772 6561  cimport` is grea
-00000da0: 7420 666f 722e 2e2e 0a2d 2050 7265 7665  t for....- Preve
-00000db0: 6e74 696e 6720 436f 6465 2045 7865 6375  nting Code Execu
-00000dc0: 7469 6f6e 3a20 7265 6475 6365 2074 6865  tion: reduce the
-00000dd0: 2072 6973 6b20 6f66 2073 7570 706c 7920   risk of supply 
-00000de0: 6368 6169 6e20 6174 7461 636b 732e 0a20  chain attacks.. 
-00000df0: 202d 2054 7261 6365 2074 6865 2073 7973   - Trace the sys
-00000e00: 6361 6c6c 7320 666c 6f77 206f 6620 796f  calls flow of yo
-00000e10: 7572 2061 7070 6c69 6361 7469 6f6e 2061  ur application a
-00000e20: 7420 7468 6520 7573 6572 2d73 7061 6365  t the user-space
-00000e30: 2f6f 732f 6b65 726e 656c 206c 6576 656c  /os/kernel level
-00000e40: 2061 6e64 2070 6572 206d 6f64 756c 652e   and per module.
-00000e50: 0a20 202d 2052 756e 2079 6f75 7220 6170  .  - Run your ap
-00000e60: 706c 6963 6174 696f 6e20 7768 696c 6520  plication while 
-00000e70: 656e 666f 7263 696e 6720 7379 7363 616c  enforcing syscal
-00000e80: 6c73 2070 6572 206d 6f64 756c 652e 0a20  ls per module.. 
-00000e90: 2020 202d 2055 706f 6e20 7669 6f6c 6174     - Upon violat
-00000ea0: 696f 6e20 6f66 2074 6865 2070 6f6c 6963  ion of the polic
-00000eb0: 792c 2069 7420 6361 6e20 6c6f 672c 2073  y, it can log, s
-00000ec0: 746f 702c 206f 7220 6b69 6c6c 2074 6865  top, or kill the
-00000ed0: 2070 726f 6365 7373 2e0a 2d20 5072 6f74   process..- Prot
-00000ee0: 6563 7420 796f 7572 7365 6c66 2066 726f  ect yourself fro
-00000ef0: 6d20 5243 453a 0a20 202d 2073 6563 696d  m RCE:.  - secim
-00000f00: 706f 7274 206d 616b 6573 2031 6461 7920  port makes 1day 
-00000f10: 6174 7461 636b 7320 6c65 7373 206f 6620  attacks less of 
-00000f20: 616e 2069 7373 7565 2c20 6265 6361 7573  an issue, becaus
-00000f30: 6520 6974 2070 7265 7665 6e74 7320 7468  e it prevents th
-00000f40: 6520 636f 6465 2066 6f72 6d20 7275 6e6e  e code form runn
-00000f50: 696e 672e 2049 6620 796f 7520 6172 6520  ing. If you are 
-00000f60: 7573 696e 6720 6120 7675 6c6e 6572 6162  using a vulnerab
-00000f70: 6c65 2070 6163 6b61 6765 2061 6e64 2073  le package and s
-00000f80: 6f6d 656f 6e65 2065 7870 6c6f 6974 6564  omeone exploited
-00000f90: 2069 742c 2079 6f75 7220 706f 6c69 6379   it, your policy
-00000fa0: 2077 696c 6c20 6e6f 7420 616c 6c6f 7720   will not allow 
-00000fb0: 7468 6973 2065 7870 6c6f 6974 2773 2073  this exploit's s
-00000fc0: 7973 6361 6c6c 7320 616e 6420 6974 2077  yscalls and it w
-00000fd0: 696c 6c20 6265 2068 616e 646c 6564 2061  ill be handled a
-00000fe0: 7320 796f 7520 7769 7368 2e0a 2020 2d20  s you wish..  - 
-00000ff0: 4176 6f69 6420 696e 6369 6465 6e74 7320  Avoid incidents 
-00001000: 6c69 6b65 203c 6120 6872 6566 3d22 6874  like <a href="ht
-00001010: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00001020: 6961 2e6f 7267 2f77 696b 692f 4c6f 6734  ia.org/wiki/Log4
-00001030: 5368 656c 6c22 3e6c 6f67 3473 6865 6c6c  Shell">log4shell
-00001040: 3c2f 613e 2e20 4120 6c6f 6767 696e 6720  </a>. A logging 
-00001050: 6c69 6272 6172 7920 7265 7175 6972 6573  library requires
-00001060: 2076 6572 7920 6665 7720 7379 7363 616c   very few syscal
-00001070: 6c73 2c20 616e 6420 6974 2073 686f 756c  ls, and it shoul
-00001080: 6420 6e65 7665 7220 7275 6e20 636f 6d6d  d never run comm
-00001090: 616e 6420 7573 696e 6720 666f 726b 2c20  and using fork, 
-000010a0: 6578 6563 7665 206f 7220 7370 6177 6e2e  execve or spawn.
-000010b0: 0a20 2020 202d 2054 6865 2073 7973 6361  .    - The sysca
-000010c0: 6c6c 7320 7468 6174 2022 6661 7374 6170  lls that "fastap
-000010d0: 6922 2c20 226e 756d 7079 2220 6f72 2022  i", "numpy" or "
-000010e0: 7265 7175 6573 7473 2220 7573 6520 6172  requests" use ar
-000010f0: 6520 7665 7279 2064 6966 6665 7265 6e74  e very different
-00001100: 2e0a 2d20 4c6f 6164 2041 4920 4d6f 6465  ..- Load AI Mode
-00001110: 6c73 2066 726f 6d20 496e 7365 6375 7265  ls from Insecure
-00001120: 2053 6f75 7263 6573 0a20 202d 204d 6f64   Sources.  - Mod
-00001130: 656c 7320 6672 6f6d 2075 6e73 6166 6520  els from unsafe 
-00001140: 736f 7572 6365 2028 6875 6767 696e 6766  source (huggingf
-00001150: 6163 652c 2074 6f72 6368 2068 7562 2c20  ace, torch hub, 
-00001160: 616e 6420 7079 746f 7263 6820 7069 636b  and pytorch pick
-00001170: 6c65 6420 6d6f 6465 6c73 2920 6361 6e20  led models) can 
-00001180: 6265 206c 696d 6974 6564 2074 6f20 7275  be limited to ru
-00001190: 6e20 6f6e 6c79 2061 2073 6574 206f 6620  n only a set of 
-000011a0: 7379 7363 616c 6c73 2e20 5243 4520 6c69  syscalls. RCE li
-000011b0: 6b65 2027 696d 706f 7274 206f 733b 6f73  ke 'import os;os
-000011c0: 2e73 7973 7465 6d28 2e2e 2e29 2720 736f  .system(...)' so
-000011d0: 6d65 7768 6572 6520 6465 6570 2069 6e20  mewhere deep in 
-000011e0: 7468 6520 636f 6465 2077 696c 6c20 6265  the code will be
-000011f0: 2063 6174 6368 6564 2062 7920 7365 6369   catched by seci
-00001200: 6d70 6f72 742e 0a2d 204d 696e 696d 616c  mport..- Minimal
-00001210: 2050 6572 666f 726d 616e 6365 2049 6d70   Performance Imp
-00001220: 6163 740a 2020 2d20 2048 6173 206e 6567  act.  -  Has neg
-00001230: 6c69 6769 626c 6520 7065 7266 6f72 6d61  ligible performa
-00001240: 6e63 6520 696d 7061 6374 2061 6e64 2069  nce impact and i
-00001250: 7320 7072 6f64 7563 7469 6f6e 2d72 6561  s production-rea
-00001260: 6479 2074 6861 6e6b 7320 746f 2065 4250  dy thanks to eBP
-00001270: 462e 2043 6865 636b 206f 7574 2074 6865  F. Check out the
-00001280: 205b 5065 7266 6f72 6d61 6e63 655d 2868   [Performance](h
-00001290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000012a0: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
-000012b0: 7274 2f77 696b 692f 5065 7266 6f72 6d61  rt/wiki/Performa
-000012c0: 6e63 652d 4265 6e63 686d 6172 6b73 2920  nce-Benchmarks) 
-000012d0: 6265 6e63 686d 6172 6b73 2e0a 2d20 5472  benchmarks..- Tr
-000012e0: 6163 6520 7768 6963 6820 7379 7363 616c  ace which syscal
-000012f0: 6c73 2061 7265 2063 616c 6c65 6420 6279  ls are called by
-00001300: 2065 6163 6820 6d6f 6475 6c65 2069 6e20   each module in 
-00001310: 796f 7572 2063 6f64 652e 0a20 202d 2073  your code..  - s
-00001320: 6563 696d 706f 7274 2075 7365 7320 5553  ecimport uses US
-00001330: 4454 2028 5573 6572 6c61 6e64 2053 7461  DT (Userland Sta
-00001340: 7469 6361 6c6c 7920 4465 6669 6e65 6420  tically Defined 
-00001350: 5472 6163 696e 6729 2074 6f67 6574 6865  Tracing) togethe
-00001360: 7220 7769 7468 206b 6572 6e65 6c20 7072  r with kernel pr
-00001370: 6f62 6573 2069 6e20 7468 6520 7275 6e74  obes in the runt
-00001380: 696d 6520 7573 696e 6720 6542 5046 206f  ime using eBPF o
-00001390: 7220 6474 7261 6365 2069 6e73 7472 756d  r dtrace instrum
-000013a0: 656e 7461 7469 6f6e 2073 6372 6970 7473  entation scripts
-000013b0: 2e0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000013c0: 6e0a 5465 7374 6564 206f 6e20 5562 756e  n.Tested on Ubun
-000013d0: 7475 2c20 4465 6269 616e 2c20 526f 636b  tu, Debian, Rock
-000013e0: 7920 284c 696e 7578 2078 3836 2f41 4d44  y (Linux x86/AMD
-000013f0: 2f41 524d 2920 616e 6420 4d61 634f 5320  /ARM) and MacOS 
-00001400: 696e 2028 7838 362f 4d31 292e 2049 6620  in (x86/M1). If 
-00001410: 796f 7520 7275 6e20 6f6e 204d 6163 4f53  you run on MacOS
-00001420: 2079 6f75 2077 696c 6c20 6e65 6564 2074   you will need t
-00001430: 6f20 3c61 2068 7265 663d 2268 7474 7073  o <a href="https
-00001440: 3a2f 2f67 6974 6875 622e 636f 6d2f 6176  ://github.com/av
-00001450: 696c 756d 2f73 6563 696d 706f 7274 2f62  ilum/secimport/b
-00001460: 6c6f 622f 6d61 7374 6572 2f64 6f63 732f  lob/master/docs/
-00001470: 4d41 435f 4f53 5f55 5345 5253 2e6d 6422  MAC_OS_USERS.md"
-00001480: 3e64 6973 6162 6c65 2053 4950 2066 6f72  >disable SIP for
-00001490: 2064 7472 6163 652e 203c 2f61 3e0a 0a23   dtrace. </a>..#
-000014a0: 2320 5769 7468 2044 6f63 6b65 720a 466f  # With Docker.Fo
-000014b0: 7220 7175 6963 6b65 7220 6576 616c 7561  r quicker evalua
-000014c0: 7469 6f6e 2c20 7765 2072 6563 6f6d 6d65  tion, we recomme
-000014d0: 6e64 2075 7369 6e67 2074 6865 203c 6120  nd using the <a 
-000014e0: 6872 6566 3d22 5b64 6f63 732f 446f 636b  href="[docs/Dock
-000014f0: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00001500: 7562 2e63 6f6d 2f61 7669 6c75 6d2f 7365  ub.com/avilum/se
-00001510: 6369 6d70 6f72 742f 626c 6f62 2f6d 6173  cimport/blob/mas
-00001520: 7465 722f 646f 636b 6572 2f52 4541 444d  ter/docker/READM
-00001530: 452e 6d64 2922 3e53 6563 696d 706f 7274  E.md)">Secimport
-00001540: 2044 6f63 6b65 7220 496d 6167 653c 2f61   Docker Image</a
-00001550: 3e20 696e 7374 6561 6420 6f66 2073 656c  > instead of sel
-00001560: 662d 696e 7374 616c 6c69 6e67 2e3c 6272  f-installing.<br
-00001570: 3e0a 2d20 4275 696c 6420 616e 6420 7275  >.- Build and ru
-00001580: 6e20 7468 6520 446f 636b 6572 2063 6f6e  n the Docker con
-00001590: 7461 696e 6572 2077 6974 6820 6120 6375  tainer with a cu
-000015a0: 7374 6f6d 206b 6572 6e65 6c20 7468 6174  stom kernel that
-000015b0: 206d 6174 6368 6573 2079 6f75 7220 6578   matches your ex
-000015c0: 6973 7469 6e67 204f 5320 6b65 726e 656c  isting OS kernel
-000015d0: 2076 6572 7369 6f6e 3a0a 2020 6060 600a   version:.  ```.
-000015e0: 2020 6364 2064 6f63 6b65 722f 2026 2620    cd docker/ && 
-000015f0: 2e2f 6275 696c 642e 7368 2026 2620 2e2f  ./build.sh && ./
-00001600: 7275 6e2e 7368 0a20 2060 6060 0a20 2041  run.sh.  ```.  A
-00001610: 2074 656d 706f 7261 7279 2063 6f6e 7461   temporary conta
-00001620: 696e 6572 2077 696c 6c20 6265 2063 7265  iner will be cre
-00001630: 6174 6564 2c20 616e 6420 796f 7520 7769  ated, and you wi
-00001640: 6c6c 2062 6520 6c6f 6767 6564 2069 6e20  ll be logged in 
-00001650: 6173 2074 6865 2072 6f6f 7420 7573 6572  as the root user
-00001660: 2e0a 0a23 2320 5769 7468 6f75 7420 446f  ...## Without Do
-00001670: 636b 6572 0a31 2e20 496e 7374 616c 6c20  cker.1. Install 
-00001680: 7079 7468 6f6e 2077 6974 6820 5553 4454  python with USDT
-00001690: 2070 726f 6265 7320 6279 203c 6120 6872   probes by <a hr
-000016a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000016b0: 7562 2e63 6f6d 2f61 7669 6c75 6d2f 7365  ub.com/avilum/se
-000016c0: 6369 6d70 6f72 742f 7769 6b69 2f49 6e73  cimport/wiki/Ins
-000016d0: 7461 6c6c 6174 696f 6e23 7079 7468 6f6e  tallation#python
-000016e0: 2d69 6e74 6572 7072 6574 6572 2d72 6571  -interpreter-req
-000016f0: 7569 7265 6d65 6e74 7322 3e63 6f6e 6669  uirements">confi
-00001700: 6775 7269 6e67 2069 7420 7769 7468 2027  guring it with '
-00001710: 2d2d 6474 7261 6365 273c 2f61 3e0a 322e  --dtrace'</a>.2.
-00001720: 2049 6e73 7461 6c6c 206f 6e65 206f 6620   Install one of 
-00001730: 7468 6520 6261 636b 656e 6473 3a20 3c61  the backends: <a
-00001740: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00001750: 6974 6875 622e 636f 6d2f 6176 696c 756d  ithub.com/avilum
-00001760: 2f73 6563 696d 706f 7274 2f77 696b 692f  /secimport/wiki/
-00001770: 496e 7374 616c 6c61 7469 6f6e 223e 6542  Installation">eB
-00001780: 5046 206f 7220 4454 7261 6365 3c2f 613e  PF or DTrace</a>
-00001790: 2e0a 332e 2049 6e73 7461 6c6c 2073 6563  ..3. Install sec
-000017a0: 696d 706f 7274 0a20 202d 2049 6e73 7461  import.  - Insta
-000017b0: 6c6c 2066 726f 6d20 7079 7069 0a20 2020  ll from pypi.   
-000017c0: 202d 2060 6060 0a20 2020 2020 2070 7974   - ```.      pyt
-000017d0: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
-000017e0: 616c 6c20 7365 6369 6d70 6f72 740a 2020  all secimport.  
-000017f0: 2020 2020 6060 600a 2020 2d20 496e 7374      ```.  - Inst
-00001800: 616c 6c20 6672 6f6d 2073 6f75 7263 650a  all from source.
-00001810: 2020 2020 2d20 6060 600a 2020 2020 2020      - ```.      
-00001820: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-00001830: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
-00001840: 6c75 6d2f 7365 6369 6d70 6f72 742e 6769  lum/secimport.gi
-00001850: 7420 2626 2063 6420 7365 6369 6d70 6f72  t && cd secimpor
-00001860: 740a 2020 2020 2020 7079 7468 6f6e 3320  t.      python3 
-00001870: 2d6d 2070 6970 2069 6e73 7461 6c6c 2070  -m pip install p
-00001880: 6f65 7472 7920 2626 2070 7974 686f 6e33  oetry && python3
-00001890: 202d 6d20 706f 6574 7279 2069 6e73 7461   -m poetry insta
-000018a0: 6c6c 0a20 2020 2020 2060 6060 0a0a 0a23  ll.      ```...#
-000018b0: 2320 5573 6167 650a 546f 2073 616e 6462  # Usage.To sandb
-000018c0: 6f78 2079 6f75 7220 7072 6f67 7261 6d20  ox your program 
-000018d0: 7573 696e 6720 7468 6520 434c 492c 2073  using the CLI, s
-000018e0: 7461 7274 2061 2062 7066 7472 6163 6520  tart a bpftrace 
-000018f0: 7072 6f67 7261 6d20 7468 6174 206c 6f67  program that log
-00001900: 7320 616c 6c20 7468 6520 7379 7363 616c  s all the syscal
-00001910: 6c73 2066 6f72 2061 6c6c 2074 6865 206d  ls for all the m
-00001920: 6f64 756c 6573 2069 6e20 796f 7572 2061  odules in your a
-00001930: 7070 6c69 6361 7469 6f6e 2069 6e74 6f20  pplication into 
-00001940: 6120 6669 6c65 2077 6974 6820 7468 6520  a file with the 
-00001950: 7365 6369 6d70 6f72 7420 7472 6163 6520  secimport trace 
-00001960: 636f 6d6d 616e 642e 204f 6e63 6520 796f  command. Once yo
-00001970: 7520 6861 7665 2063 6f76 6572 6564 2074  u have covered t
-00001980: 6865 206c 6f67 6963 2079 6f75 2077 6f75  he logic you wou
-00001990: 6c64 206c 696b 6520 746f 2073 616e 6462  ld like to sandb
-000019a0: 6f78 2c20 6869 7420 4354 524c 2b43 206f  ox, hit CTRL+C o
-000019b0: 7220 4354 524c 2b44 2c20 6f72 2077 6169  r CTRL+D, or wai
-000019c0: 7420 666f 7220 7468 6520 7072 6f67 7261  t for the progra
-000019d0: 6d20 746f 2066 696e 6973 682e 2054 6865  m to finish. The
-000019e0: 6e2c 2062 7569 6c64 2061 2073 616e 6462  n, build a sandb
-000019f0: 6f78 2066 726f 6d20 7468 6520 7472 6163  ox from the trac
-00001a00: 6520 7573 696e 6720 7468 6520 7365 6369  e using the seci
-00001a10: 6d70 6f72 7420 6275 696c 6420 636f 6d6d  mport build comm
-00001a20: 616e 642c 2061 6e64 2072 756e 2074 6865  and, and run the
-00001a30: 2073 616e 6462 6f78 2077 6974 6820 7468   sandbox with th
-00001a40: 6520 7365 6369 6d70 6f72 7420 7275 6e20  e secimport run 
-00001a50: 636f 6d6d 616e 642e 0a0a 6060 6073 6865  command...```she
-00001a60: 6c6c 0a4e 414d 450a 2020 2020 7365 6369  ll.NAME.    seci
-00001a70: 6d70 6f72 7420 2d20 6973 2061 2063 6f6d  mport - is a com
-00001a80: 7072 6568 656e 7369 7665 2074 6f6f 6c6b  prehensive toolk
-00001a90: 6974 2064 6573 6967 6e65 6420 746f 2065  it designed to e
-00001aa0: 6e61 626c 6520 7468 6520 7472 6163 696e  nable the tracin
-00001ab0: 672c 2063 6f6e 7374 7275 6374 696f 6e2c  g, construction,
-00001ac0: 2061 6e64 2065 7865 6375 7469 6f6e 206f   and execution o
-00001ad0: 6620 7365 6375 7265 2050 7974 686f 6e20  f secure Python 
-00001ae0: 7275 6e74 696d 6573 2e20 4974 206c 6576  runtimes. It lev
-00001af0: 6572 6167 6573 2055 5344 5420 7072 6f62  erages USDT prob
-00001b00: 6573 2061 6e64 2065 4250 462f 4454 7261  es and eBPF/DTra
-00001b10: 6365 2074 6563 686e 6f6c 6f67 6965 7320  ce technologies 
-00001b20: 746f 2065 6e68 616e 6365 2074 6865 206f  to enhance the o
-00001b30: 7665 7261 6c6c 2073 6563 7572 6974 7920  verall security 
-00001b40: 6d65 6173 7572 6573 2e0a 0a53 594e 4f50  measures...SYNOP
-00001b50: 5349 530a 2020 2020 7365 6369 6d70 6f72  SIS.    secimpor
-00001b60: 7420 434f 4d4d 414e 440a 0a44 4553 4352  t COMMAND..DESCR
-00001b70: 4950 5449 4f4e 0a20 2020 2068 7474 7073  IPTION.    https
-00001b80: 3a2f 2f67 6974 6875 622e 636f 6d2f 6176  ://github.com/av
-00001b90: 696c 756d 2f73 6563 696d 706f 7274 2f77  ilum/secimport/w
-00001ba0: 696b 692f 436f 6d6d 616e 642d 4c69 6e65  iki/Command-Line
-00001bb0: 2d55 7361 6765 0a0a 2020 2020 574f 524b  -Usage..    WORK
-00001bc0: 464c 4f57 3a0a 2020 2020 2020 2020 2020  FLOW:.          
-00001bd0: 2020 312e 2073 6563 696d 706f 7274 2074    1. secimport t
-00001be0: 7261 6365 202f 2073 6563 696d 706f 7274  race / secimport
-00001bf0: 2073 6865 6c6c 0a20 2020 2020 2020 2020   shell.         
-00001c00: 2020 2032 2e20 7365 6369 6d70 6f72 7420     2. secimport 
-00001c10: 6275 696c 640a 2020 2020 2020 2020 2020  build.          
-00001c20: 2020 332e 2073 6563 696d 706f 7274 2072    3. secimport r
-00001c30: 756e 0a0a 2020 2020 5155 4943 4b53 5441  un..    QUICKSTA
-00001c40: 5254 3a0a 2020 2020 2020 2020 2020 2020  RT:.            
-00001c50: 2420 7365 6369 6d70 6f72 7420 696e 7465  $ secimport inte
-00001c60: 7261 6374 6976 650a 0a20 2020 2045 5841  ractive..    EXA
-00001c70: 4d50 4c45 533a 0a20 2020 2020 2020 2031  MPLES:.        1
-00001c80: 2e20 7472 6163 653a 0a20 2020 2020 2020  . trace:.       
-00001c90: 2020 2020 2024 2020 7365 6369 6d70 6f72       $  secimpor
-00001ca0: 7420 7472 6163 650a 2020 2020 2020 2020  t trace.        
-00001cb0: 2020 2020 2420 2073 6563 696d 706f 7274      $  secimport
-00001cc0: 2074 7261 6365 202d 680a 2020 2020 2020   trace -h.      
-00001cd0: 2020 2020 2020 2420 2073 6563 696d 706f        $  secimpo
-00001ce0: 7274 2074 7261 6365 5f70 6964 2031 3233  rt trace_pid 123
-00001cf0: 0a20 2020 2020 2020 2020 2020 2024 2020  .            $  
-00001d00: 7365 6369 6d70 6f72 7420 7472 6163 655f  secimport trace_
-00001d10: 7069 6420 2d68 0a20 2020 2020 2020 2032  pid -h.        2
-00001d20: 2e20 6275 696c 643a 0a20 2020 2020 2020  . build:.       
-00001d30: 2020 2020 2023 2073 6563 696d 706f 7274       # secimport
-00001d40: 2062 7569 6c64 0a20 2020 2020 2020 2020   build.         
-00001d50: 2020 2024 2073 6563 696d 706f 7274 2062     $ secimport b
-00001d60: 7569 6c64 202d 680a 2020 2020 2020 2020  uild -h.        
-00001d70: 332e 2072 756e 3a0a 2020 2020 2020 2020  3. run:.        
-00001d80: 2020 2020 2420 2073 6563 696d 706f 7274      $  secimport
-00001d90: 2072 756e 0a20 2020 2020 2020 2020 2020   run.           
-00001da0: 2024 2020 7365 6369 6d70 6f72 7420 7275   $  secimport ru
-00001db0: 6e20 2d2d 656e 7472 7970 6f69 6e74 206d  n --entrypoint m
-00001dc0: 795f 6375 7374 6f6d 5f6d 6169 6e2e 7079  y_custom_main.py
-00001dd0: 0a20 2020 2020 2020 2020 2020 2024 2020  .            $  
-00001de0: 7365 6369 6d70 6f72 7420 7275 6e20 2d2d  secimport run --
-00001df0: 656e 7472 7970 6f69 6e74 206d 795f 6375  entrypoint my_cu
-00001e00: 7374 6f6d 5f6d 6169 6e2e 7079 202d 2d73  stom_main.py --s
-00001e10: 746f 705f 6f6e 5f76 696f 6c61 7469 6f6e  top_on_violation
-00001e20: 3d74 7275 650a 2020 2020 2020 2020 2020  =true.          
-00001e30: 2020 2420 2073 6563 696d 706f 7274 2072    $  secimport r
-00001e40: 756e 202d 2d65 6e74 7279 706f 696e 7420  un --entrypoint 
-00001e50: 6d79 5f63 7573 746f 6d5f 6d61 696e 2e70  my_custom_main.p
-00001e60: 7920 2d2d 6b69 6c6c 5f6f 6e5f 7669 6f6c  y --kill_on_viol
-00001e70: 6174 696f 6e3d 7472 7565 0a20 2020 2020  ation=true.     
-00001e80: 2020 2020 2020 2024 2020 7365 6369 6d70         $  secimp
-00001e90: 6f72 7420 7275 6e20 2d2d 7361 6e64 626f  ort run --sandbo
-00001ea0: 785f 6578 6563 7574 6162 6c65 202f 7061  x_executable /pa
-00001eb0: 7468 2f74 6f2f 6d79 5f73 616e 6462 6f78  th/to/my_sandbox
-00001ec0: 2e62 7420 2d2d 7069 6420 3238 3834 0a20  .bt --pid 2884. 
-00001ed0: 2020 2020 2020 2020 2020 2024 2020 7365             $  se
-00001ee0: 6369 6d70 6f72 7420 7275 6e20 2d2d 7361  cimport run --sa
-00001ef0: 6e64 626f 785f 6578 6563 7574 6162 6c65  ndbox_executable
-00001f00: 202f 7061 7468 2f74 6f2f 6d79 5f73 616e   /path/to/my_san
-00001f10: 6462 6f78 2e62 7420 2d2d 7361 6e64 626f  dbox.bt --sandbo
-00001f20: 785f 6c6f 6766 696c 6520 6d79 5f6c 6f67  x_logfile my_log
-00001f30: 2e6c 6f67 0a20 2020 2020 2020 2020 2020  .log.           
-00001f40: 2024 2020 7365 6369 6d70 6f72 7420 7275   $  secimport ru
-00001f50: 6e20 2d68 0a0a 434f 4d4d 414e 4453 0a20  n -h..COMMANDS. 
-00001f60: 2020 2043 4f4d 4d41 4e44 2069 7320 6f6e     COMMAND is on
-00001f70: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-00001f80: 6e67 3a0a 0a20 2020 2020 6275 696c 640a  ng:..     build.
-00001f90: 2020 2020 2020 2043 6f6d 7069 6c65 7320         Compiles 
-00001fa0: 6120 7472 6163 6520 6c6f 6720 2874 7261  a trace log (tra
-00001fb0: 6365 2e6c 6f67 292e 2043 7265 6174 6573  ce.log). Creates
-00001fc0: 2074 6865 2073 616e 6462 6f78 2065 7865   the sandbox exe
-00001fd0: 6375 7461 626c 6520 2869 6e73 7472 756d  cutable (instrum
-00001fe0: 656e 7461 7469 6f6e 2073 6372 6970 7429  entation script)
-00001ff0: 2066 6f72 2065 6163 6820 7375 7070 6f72   for each suppor
-00002000: 7465 6420 6261 636b 656e 6420 4974 2075  ted backend It u
-00002010: 7365 7320 6063 7265 6174 655f 7072 6f66  ses `create_prof
-00002020: 696c 655f 6672 6f6d 5f74 7261 6365 202e  ile_from_trace .
-00002030: 2e2e 6020 616e 6420 6073 616e 6462 6f78  ..` and `sandbox
-00002040: 5f66 726f 6d5f 7072 6f66 696c 6560 2e0a  _from_profile`..
-00002050: 0a20 2020 2020 636f 6d70 696c 655f 7361  .     compile_sa
-00002060: 6e64 626f 785f 6672 6f6d 5f70 726f 6669  ndbox_from_profi
-00002070: 6c65 0a20 2020 2020 2020 4765 6e65 7261  le.       Genera
-00002080: 7465 7320 6120 7461 696c 6f72 2d6d 6164  tes a tailor-mad
-00002090: 6520 7361 6e64 626f 7820 7468 6174 2077  e sandbox that w
-000020a0: 696c 6c20 656e 666f 7263 6520 6120 6769  ill enforce a gi
-000020b0: 7665 6e20 7961 6d6c 2070 726f 6669 6c65  ven yaml profile
-000020c0: 2f70 6f6c 6963 7920 696e 2072 756e 7469  /policy in runti
-000020d0: 6d65 2e0a 0a20 2020 2020 696e 7465 7261  me...     intera
-000020e0: 6374 6976 650a 0a20 2020 2020 7275 6e0a  ctive..     run.
-000020f0: 2020 2020 2020 2052 756e 2061 2070 7974         Run a pyt
-00002100: 686f 6e20 7072 6f63 6573 7320 696e 7369  hon process insi
-00002110: 6465 2074 6865 2073 616e 6462 6f78 2e0a  de the sandbox..
-00002120: 0a20 2020 2020 7368 656c 6c0a 2020 2020  .     shell.    
-00002130: 2020 2041 6c74 6572 6e61 7469 7665 2073     Alternative s
-00002140: 796e 7461 7820 666f 7220 7365 6369 6d70  yntax for secimp
-00002150: 6f72 7420 2274 7261 6365 222e 0a0a 2020  ort "trace"...  
-00002160: 2020 2074 7261 6365 0a20 2020 2020 2020     trace.       
-00002170: 5472 6163 6573 2061 2070 7974 686f 6e20  Traces a python 
-00002180: 7072 6f63 6573 7320 7573 696e 6720 616e  process using an
-00002190: 2065 6e74 7279 706f 696e 7420 6f72 2069   entrypoint or i
-000021a0: 6e74 6572 6163 7469 7665 2069 6e74 6572  nteractive inter
-000021b0: 7072 6574 6572 2e20 4974 206d 6967 6874  preter. It might
-000021c0: 2072 6571 7569 7265 2073 7564 6f20 7072   require sudo pr
-000021d0: 6976 696c 6c65 6765 7320 6f6e 2073 6f6d  ivilleges on som
-000021e0: 6520 686f 7374 732e 0a0a 2020 2020 2074  e hosts...     t
-000021f0: 7261 6365 5f70 6964 0a20 2020 2020 2020  race_pid.       
-00002200: 5472 6163 6573 2061 2072 756e 6e69 6e67  Traces a running
-00002210: 2070 726f 6365 7373 2062 7920 7069 642e   process by pid.
-00002220: 2049 7420 6d69 6768 7420 7265 7175 6972   It might requir
-00002230: 6520 7375 646f 2070 7269 7669 6c6c 6567  e sudo privilleg
-00002240: 6573 206f 6e20 736f 6d65 2068 6f73 7473  es on some hosts
-00002250: 2e0a 6060 600a 0a23 2320 5374 6f70 206f  ..```..## Stop o
-00002260: 6e20 7669 6f6c 6174 696f 6e0a 6060 600a  n violation.```.
-00002270: 726f 6f74 4031 6263 3035 3331 6439 3164  root@1bc0531d91d
-00002280: 303a 2f77 6f72 6b73 7061 6365 2320 7365  0:/workspace# se
-00002290: 6369 6d70 6f72 7420 7275 6e20 202d 2d73  cimport run  --s
-000022a0: 746f 705f 6f6e 5f76 696f 6c61 7469 6f6e  top_on_violation
-000022b0: 3d74 7275 650a 203e 3e3e 2073 6563 696d  =true. >>> secim
-000022c0: 706f 7274 2072 756e 0a5b 5741 524e 494e  port run.[WARNIN
-000022d0: 475d 3a20 5468 6973 2073 616e 6462 6f78  G]: This sandbox
-000022e0: 2077 696c 6c20 7365 6e64 2053 4947 5354   will send SIGST
-000022f0: 4f50 2074 6f20 7468 6520 7072 6f67 7261  OP to the progra
-00002300: 6d20 7570 6f6e 2076 696f 6c61 7469 6f6e  m upon violation
-00002310: 2e0a 2052 554e 4e49 4e47 2053 414e 4442  .. RUNNING SANDB
-00002320: 4f58 2e2e 2e20 5b27 2e2f 7361 6e64 626f  OX... ['./sandbo
-00002330: 782e 6274 272c 2027 2d2d 756e 7361 6665  x.bt', '--unsafe
-00002340: 272c 2027 202d 6320 272c 2027 2f77 6f72  ', ' -c ', '/wor
-00002350: 6b73 7061 6365 2f50 7974 686f 6e2d 332e  kspace/Python-3.
-00002360: 3130 2e30 2f70 7974 686f 6e27 2c20 2753  10.0/python', 'S
-00002370: 544f 5027 5d0a 4174 7461 6368 696e 6720  TOP'].Attaching 
-00002380: 3420 7072 6f62 6573 2e2e 2e0a 5079 7468  4 probes....Pyth
-00002390: 6f6e 2033 2e31 302e 3020 2864 6566 6175  on 3.10.0 (defau
-000023a0: 6c74 2c20 4170 7220 3238 2032 3032 332c  lt, Apr 28 2023,
-000023b0: 2031 313a 3332 3a34 3029 205b 4743 4320   11:32:40) [GCC 
-000023c0: 392e 342e 305d 206f 6e20 6c69 6e75 780a  9.4.0] on linux.
-000023d0: 5479 7065 2022 6865 6c70 222c 2022 636f  Type "help", "co
-000023e0: 7079 7269 6768 7422 2c20 2263 7265 6469  pyright", "credi
-000023f0: 7473 2220 6f72 2022 6c69 6365 6e73 6522  ts" or "license"
-00002400: 2066 6f72 206d 6f72 6520 696e 666f 726d   for more inform
-00002410: 6174 696f 6e2e 0a3e 3e3e 2069 6d70 6f72  ation..>>> impor
-00002420: 7420 6f73 0a3e 3e3e 206f 732e 7379 7374  t os.>>> os.syst
-00002430: 656d 2827 7073 2729 0a5b 5345 4355 5249  em('ps').[SECURI
-00002440: 5459 2050 524f 4649 4c45 2056 494f 4c41  TY PROFILE VIOLA
-00002450: 5445 445d 3a20 3c73 7464 696e 3e20 6361  TED]: <stdin> ca
-00002460: 6c6c 6564 2073 7973 6361 6c6c 2035 3620  lled syscall 56 
-00002470: 6174 2064 6570 7468 2038 3032 320a 0a5e  at depth 8022..^
-00002480: 5e5e 2053 544f 5050 494e 4720 5052 4f43  ^^ STOPPING PROC
-00002490: 4553 5320 3835 3931 3820 4455 4520 544f  ESS 85918 DUE TO
-000024a0: 2053 5953 4341 4c4c 2056 494f 4c41 5449   SYSCALL VIOLATI
-000024b0: 4f4e 205e 5e5e 0a09 0950 524f 4345 5353  ON ^^^...PROCESS
-000024c0: 2038 3539 3138 2053 544f 5050 4544 2e0a   85918 STOPPED..
-000024d0: 6060 600a 0a23 2320 4b69 6c6c 206f 6e20  ```..## Kill on 
-000024e0: 7669 6f6c 6174 696f 6e0a 6060 600a 726f  violation.```.ro
-000024f0: 6f74 4065 6534 6263 3939 6262 3031 313a  ot@ee4bc99bb011:
-00002500: 2f77 6f72 6b73 7061 6365 2320 7365 6369  /workspace# seci
-00002510: 6d70 6f72 7420 7275 6e20 2d2d 6b69 6c6c  mport run --kill
-00002520: 5f6f 6e5f 7669 6f6c 6174 696f 6e0a 203e  _on_violation. >
-00002530: 3e3e 2073 6563 696d 706f 7274 2072 756e  >> secimport run
-00002540: 0a5b 5741 524e 494e 475d 3a20 5468 6973  .[WARNING]: This
-00002550: 2073 616e 6462 6f78 2077 696c 6c20 7365   sandbox will se
-00002560: 6e64 2053 4947 4b49 4c4c 2074 6f20 7468  nd SIGKILL to th
-00002570: 6520 7072 6f67 7261 6d20 7570 6f6e 2076  e program upon v
-00002580: 696f 6c61 7469 6f6e 2e0a 2052 554e 4e49  iolation.. RUNNI
-00002590: 4e47 2053 414e 4442 4f58 2e2e 2e20 5b27  NG SANDBOX... ['
-000025a0: 2e2f 7361 6e64 626f 782e 6274 272c 2027  ./sandbox.bt', '
-000025b0: 2d2d 756e 7361 6665 272c 2027 202d 6320  --unsafe', ' -c 
-000025c0: 272c 2027 2f77 6f72 6b73 7061 6365 2f50  ', '/workspace/P
-000025d0: 7974 686f 6e2d 332e 3130 2e30 2f70 7974  ython-3.10.0/pyt
-000025e0: 686f 6e27 2c20 274b 494c 4c27 5d0a 696d  hon', 'KILL'].im
-000025f0: 706f 7274 206f 730a 6f41 7474 6163 6869  port os.oAttachi
-00002600: 6e67 2034 2070 726f 6265 732e 2e2e 0a73  ng 4 probes....s
-00002610: 5079 7468 6f6e 2033 2e31 302e 3020 2864  Python 3.10.0 (d
-00002620: 6566 6175 6c74 2c20 4170 7220 3238 2032  efault, Apr 28 2
-00002630: 3032 332c 2031 313a 3332 3a34 3029 205b  023, 11:32:40) [
-00002640: 4743 4320 392e 342e 305d 206f 6e20 6c69  GCC 9.4.0] on li
-00002650: 6e75 780a 5479 7065 2022 6865 6c70 222c  nux.Type "help",
-00002660: 2022 636f 7079 7269 6768 7422 2c20 2263   "copyright", "c
-00002670: 7265 6469 7473 2220 6f72 2022 6c69 6365  redits" or "lice
-00002680: 6e73 6522 2066 6f72 206d 6f72 6520 696e  nse" for more in
-00002690: 666f 726d 6174 696f 6e2e 0a3e 3e3e 2069  formation..>>> i
-000026a0: 6d70 6f72 7420 6f73 0a3e 3e3e 206f 732e  mport os.>>> os.
-000026b0: 7379 7374 656d 2827 7073 2729 0a5b 5345  system('ps').[SE
-000026c0: 4355 5249 5459 2050 524f 4649 4c45 2056  CURITY PROFILE V
-000026d0: 494f 4c41 5445 445d 3a20 3c73 7464 696e  IOLATED]: <stdin
-000026e0: 3e20 6361 6c6c 6564 2073 7973 6361 6c6c  > called syscall
-000026f0: 2035 3620 6174 2064 6570 7468 2038 3032   56 at depth 802
-00002700: 320a 0a5e 5e5e 204b 494c 4c49 4e47 2050  2..^^^ KILLING P
-00002710: 524f 4345 5353 2038 3634 3636 2044 5545  ROCESS 86466 DUE
-00002720: 2054 4f20 5359 5343 414c 4c20 5649 4f4c   TO SYSCALL VIOL
-00002730: 4154 494f 4e20 5e5e 5e0a 0909 4b49 4c4c  ATION ^^^...KILL
-00002740: 4544 2e0a 2053 414e 4442 4f58 2045 5849  ED.. SANDBOX EXI
-00002750: 5445 443b 0a60 6060 0a0a 2323 2044 796e  TED;.```..## Dyn
-00002760: 616d 6963 2070 726f 6669 6c69 6e67 202d  amic profiling -
-00002770: 2074 7261 6365 2c20 6275 696c 6420 7361   trace, build sa
-00002780: 6e64 626f 782c 2072 756e 2e0a 6060 6073  ndbox, run..```s
-00002790: 6865 6c6c 0a72 6f6f 7440 3166 6133 6436  hell.root@1fa3d6
-000027a0: 6630 3939 3839 3a2f 776f 726b 7370 6163  f09989:/workspac
-000027b0: 6523 2073 6563 696d 706f 7274 2069 6e74  e# secimport int
-000027c0: 6572 6163 7469 7665 0a0a 4c65 7427 7320  eractive..Let's 
-000027d0: 6372 6561 7465 206f 7572 2066 6972 7374  create our first
-000027e0: 2074 6169 6c6f 722d 6d61 6465 2073 616e   tailor-made san
-000027f0: 6462 6f78 2077 6974 6820 7365 6369 6d70  dbox with secimp
-00002800: 6f72 7421 0a2d 2041 2070 7974 686f 6e20  ort!.- A python 
-00002810: 7368 656c 6c20 7769 6c6c 2062 6520 6f70  shell will be op
-00002820: 656e 6564 0a2d 2054 6865 2062 6568 6176  ened.- The behav
-00002830: 696f 7220 7769 6c6c 2062 6520 7265 636f  ior will be reco
-00002840: 7264 6564 2e0a 0a4f 4b3f 2028 7929 3a20  rded...OK? (y): 
-00002850: 790a 203e 3e3e 2073 6563 696d 706f 7274  y. >>> secimport
-00002860: 2074 7261 6365 0a0a 5452 4143 494e 473a   trace..TRACING:
-00002870: 205b 272f 776f 726b 7370 6163 652f 7365   ['/workspace/se
-00002880: 6369 6d70 6f72 742f 7072 6f66 696c 6573  cimport/profiles
-00002890: 2f74 7261 6365 2e62 7427 2c20 272d 6327  /trace.bt', '-c'
-000028a0: 2c20 272f 776f 726b 7370 6163 652f 5079  , '/workspace/Py
-000028b0: 7468 6f6e 2d33 2e31 302e 302f 7079 7468  thon-3.10.0/pyth
-000028c0: 6f6e 272c 2027 2d6f 272c 2027 7472 6163  on', '-o', 'trac
-000028d0: 652e 6c6f 6727 5d0a 0a20 2020 2020 2020  e.log']..       
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2050 7265 7373 2043 5452 4c2b 4420 746f   Press CTRL+D to
-00002900: 2073 746f 7020 7468 6520 7472 6163 653b   stop the trace;
-00002910: 0a0a 5079 7468 6f6e 2033 2e31 302e 3020  ..Python 3.10.0 
-00002920: 2864 6566 6175 6c74 2c20 4d61 7220 3139  (default, Mar 19
-00002930: 2032 3032 332c 2030 383a 3334 3a34 3629   2023, 08:34:46)
-00002940: 205b 4743 4320 392e 342e 305d 206f 6e20   [GCC 9.4.0] on 
-00002950: 6c69 6e75 780a 5479 7065 2022 6865 6c70  linux.Type "help
-00002960: 222c 2022 636f 7079 7269 6768 7422 2c20  ", "copyright", 
-00002970: 2263 7265 6469 7473 2220 6f72 2022 6c69  "credits" or "li
-00002980: 6365 6e73 6522 2066 6f72 206d 6f72 6520  cense" for more 
-00002990: 696e 666f 726d 6174 696f 6e2e 0a3e 3e3e  information..>>>
-000029a0: 2069 6d70 6f72 7420 7468 6973 0a3e 3e3e   import this.>>>
-000029b0: 0a20 5452 4143 494e 4720 444f 4e45 3b0a  . TRACING DONE;.
-000029c0: 203e 3e3e 2073 6563 696d 706f 7274 2062   >>> secimport b
-000029d0: 7569 6c64 0a0a 5345 4349 4d50 4f52 5420  uild..SECIMPORT 
-000029e0: 434f 4d50 494c 494e 472e 2e2e 0a0a 4352  COMPILING.....CR
-000029f0: 4541 5445 4420 4a53 4f4e 2054 454d 504c  EATED JSON TEMPL
-00002a00: 4154 453a 2020 706f 6c69 6379 2e6a 736f  ATE:  policy.jso
-00002a10: 6e0a 4352 4541 5445 4420 5941 4d4c 2054  n.CREATED YAML T
-00002a20: 454d 504c 4154 453a 2020 706f 6c69 6379  EMPLATE:  policy
-00002a30: 2e79 616d 6c0a 636f 6d70 696c 696e 6720  .yaml.compiling 
-00002a40: 7465 6d70 6c61 7465 2070 6f6c 6963 792e  template policy.
-00002a50: 7961 6d6c 0a44 5452 4143 4520 5341 4e44  yaml.DTRACE SAND
-00002a60: 424f 583a 2020 7361 6e64 626f 782e 640a  BOX:  sandbox.d.
-00002a70: 4250 4654 5243 4520 5341 4e44 424f 583a  BPFTRCE SANDBOX:
-00002a80: 2020 7361 6e64 626f 782e 6274 0a60 6060    sandbox.bt.```
-00002a90: 0a0a 4e6f 772c 206c 6574 2773 2072 756e  ..Now, let's run
-00002aa0: 2074 6865 2073 616e 6462 6f78 210a 6060   the sandbox!.``
-00002ab0: 6070 7974 686f 6e0a 2d20 5275 6e20 7468  `python.- Run th
-00002ac0: 6520 7361 6d65 2063 6f6d 6d61 6e64 7320  e same commands 
-00002ad0: 6173 2062 6566 6f72 652c 2074 6865 7920  as before, they 
-00002ae0: 7368 6f75 6c64 2072 756e 2077 6974 686f  should run witho
-00002af0: 7574 2061 6e79 2070 726f 626c 656d 3b2e  ut any problem;.
-00002b00: 0a2d 2044 6f20 736f 6d65 7468 696e 6720  .- Do something 
-00002b10: 6e65 7720 696e 2074 6865 2073 6865 6c6c  new in the shell
-00002b20: 3b20 652e 673a 2020 203e 3e3e 205f 5f69  ; e.g:   >>> __i
-00002b30: 6d70 6f72 745f 5f28 226f 7322 292e 7379  mport__("os").sy
-00002b40: 7374 656d 2822 7073 2229 0a0a 2020 2020  stem("ps")..    
-00002b50: 2020 2020 4f4b 3f20 2879 293a 2079 0a20      OK? (y): y. 
-00002b60: 3e3e 3e20 7365 6369 6d70 6f72 7420 7275  >>> secimport ru
-00002b70: 6e0a 2052 554e 4e49 4e47 2053 414e 4442  n. RUNNING SANDB
-00002b80: 4f58 2e2e 2e20 5b27 2e2f 7361 6e64 626f  OX... ['./sandbo
-00002b90: 782e 6274 272c 2027 2d2d 756e 7361 6665  x.bt', '--unsafe
-00002ba0: 272c 2027 202d 6320 272c 2027 2f77 6f72  ', ' -c ', '/wor
-00002bb0: 6b73 7061 6365 2f50 7974 686f 6e2d 332e  kspace/Python-3.
-00002bc0: 3130 2e30 2f70 7974 686f 6e27 5d0a 4174  10.0/python'].At
-00002bd0: 7461 6368 696e 6720 3520 7072 6f62 6573  taching 5 probes
-00002be0: 2e2e 2e0a 5245 4749 5354 4552 494e 4720  ....REGISTERING 
-00002bf0: 5359 5343 414c 4c53 2e2e 2e0a 5354 4152  SYSCALLS....STAR
-00002c00: 5445 440a 5079 7468 6f6e 2033 2e31 302e  TED.Python 3.10.
-00002c10: 3020 2864 6566 6175 6c74 2c20 4d61 7220  0 (default, Mar 
-00002c20: 3139 2032 3032 332c 2030 383a 3334 3a34  19 2023, 08:34:4
-00002c30: 3629 205b 4743 4320 392e 342e 305d 206f  6) [GCC 9.4.0] o
-00002c40: 6e20 6c69 6e75 780a 5479 7065 2022 6865  n linux.Type "he
-00002c50: 6c70 222c 2022 636f 7079 7269 6768 7422  lp", "copyright"
-00002c60: 2c20 2263 7265 6469 7473 2220 6f72 2022  , "credits" or "
-00002c70: 6c69 6365 6e73 6522 2066 6f72 206d 6f72  license" for mor
-00002c80: 6520 696e 666f 726d 6174 696f 6e2e 0a3e  e information..>
-00002c90: 3e3e 2069 6d70 6f72 7420 7468 6973 0a3e  >> import this.>
-00002ca0: 3e3e 2069 6d70 6f72 7420 6f73 0a5b 5345  >> import os.[SE
-00002cb0: 4349 4d50 4f52 5420 5649 4f4c 4154 494f  CIMPORT VIOLATIO
-00002cc0: 4e5d 3a20 3c73 7464 696e 3e20 6361 6c6c  N]: <stdin> call
-00002cd0: 6564 2073 7973 6361 6c6c 2069 6f63 746c  ed syscall ioctl
-00002ce0: 2061 7420 6465 7074 6820 300a 5b53 4543   at depth 0.[SEC
-00002cf0: 494d 504f 5254 2056 494f 4c41 5449 4f4e  IMPORT VIOLATION
-00002d00: 5d3a 203c 7374 6469 6e3e 2063 616c 6c65  ]: <stdin> calle
-00002d10: 6420 7379 7363 616c 6c20 696f 6374 6c20  d syscall ioctl 
-00002d20: 6174 2064 6570 7468 2030 0a60 6060 0a0a  at depth 0.```..
-00002d30: 466f 7220 6d6f 7265 2064 6574 6169 6c65  For more detaile
-00002d40: 6420 7573 6167 6520 696e 7374 7275 6374  d usage instruct
-00002d50: 696f 6e73 2c20 7365 6520 7468 6520 5b43  ions, see the [C
-00002d60: 6f6d 6d61 6e64 2d4c 696e 6520 5573 6167  ommand-Line Usag
-00002d70: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00002d80: 622e 636f 6d2f 6176 696c 756d 2f73 6563  b.com/avilum/sec
-00002d90: 696d 706f 7274 2f77 696b 692f 436f 6d6d  import/wiki/Comm
-00002da0: 616e 642d 4c69 6e65 2d55 7361 6765 2920  and-Line-Usage) 
-00002db0: 7061 6765 2e0a 0a23 2320 6e73 6a61 696c  page...## nsjail
-00002dc0: 2073 7570 706f 7274 2028 7365 6363 6f6d   support (seccom
-00002dd0: 7029 0a42 6573 6964 6520 7468 6520 7361  p).Beside the sa
-00002de0: 6e64 626f 7820 7468 6174 2073 6563 696d  ndbox that secim
-00002df0: 706f 7274 2062 7569 6c64 732c 203c 6272  port builds, <br
-00002e00: 3e0a 5468 6520 6073 6563 696d 706f 7274  >.The `secimport
-00002e10: 2062 7569 6c64 6020 636f 6d6d 616e 6420   build` command 
-00002e20: 6372 6561 7465 7320 616e 203c 6120 6872  creates an <a hr
-00002e30: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00002e40: 7562 2e63 6f6d 2f67 6f6f 676c 652f 6e73  ub.com/google/ns
-00002e50: 6a61 696c 223e 6e73 6a61 696c 3c2f 613e  jail">nsjail</a>
-00002e60: 2073 616e 6462 6f78 2077 6974 6820 7365   sandbox with se
-00002e70: 6363 6f6d 7020 7072 6f66 696c 6520 666f  ccomp profile fo
-00002e80: 7220 796f 7572 2074 7261 6365 6420 636f  r your traced co
-00002e90: 6465 2e3c 6272 3e20 606e 736a 6169 6c60  de.<br> `nsjail`
-00002ea0: 2065 6e61 626c 6573 206e 616d 6573 7061   enables namespa
-00002eb0: 6365 2073 616e 6462 6f78 696e 6720 7769  ce sandboxing wi
-00002ec0: 7468 2073 6563 636f 6d70 206f 6e20 6c69  th seccomp on li
-00002ed0: 6e75 783c 6272 3e0a 6073 6563 696d 706f  nux<br>.`secimpo
-00002ee0: 7274 6020 6175 746f 6d61 7469 6361 6c6c  rt` automaticall
-00002ef0: 7920 6765 6e65 7261 7465 7320 7365 6363  y generates secc
-00002f00: 6f6d 7020 7072 6f66 696c 6573 2074 6f20  omp profiles to 
-00002f10: 7573 6520 7769 7468 2060 6e73 6a61 696c  use with `nsjail
-00002f20: 6020 6173 2065 7865 6375 7461 626c 6520  ` as executable 
-00002f30: 6261 7368 2073 6372 6970 742e 0a49 7420  bash script..It 
-00002f40: 6361 6e20 6265 2075 7365 6420 746f 206c  can be used to l
-00002f50: 696d 6974 2074 6865 2073 7973 6361 6c6c  imit the syscall
-00002f60: 7320 6f66 2074 6865 2065 6e74 6972 6520  s of the entire 
-00002f70: 7079 7468 6f6e 2070 726f 6365 7373 2c20  python process, 
-00002f80: 6173 2061 6e6f 7468 6572 206c 6179 6572  as another layer
-00002f90: 206f 6620 6465 6665 6e63 652e 0a0a 2323   of defence...##
-00002fa0: 2050 7974 686f 6e20 4150 490a 0a49 6e73   Python API..Ins
-00002fb0: 7465 6164 206f 6620 434c 492c 2079 6f75  tead of CLI, you
-00002fc0: 2063 616e 2061 6c73 6f20 7573 6520 6073   can also use `s
-00002fd0: 6563 696d 706f 7274 6020 6279 2072 6570  ecimport` by rep
-00002fe0: 6c61 6369 6e67 2022 6069 6d70 6f72 7460  lacing "`import`
-00002ff0: 2220 7769 7468 2022 6073 6563 696d 706f  " with "`secimpo
-00003000: 7274 2e73 6563 7572 655f 696d 706f 7274  rt.secure_import
-00003010: 6022 2066 6f72 2073 656c 6563 7465 6420  `" for selected 
-00003020: 6d6f 6475 6c65 732e 2053 6565 2074 6865  modules. See the
-00003030: 205b 5079 7468 6f6e 2049 6d70 6f72 7473   [Python Imports
-00003040: 5d28 6578 616d 706c 6573 2f70 7974 686f  ](examples/pytho
-00003050: 6e5f 696d 706f 7274 732f 2920 6578 616d  n_imports/) exam
-00003060: 706c 6520 666f 7220 6d6f 7265 2064 6574  ple for more det
-00003070: 6169 6c73 2e0a 0a23 2320 446f 636b 6572  ails...## Docker
-00003080: 0a54 6865 2071 7569 636b 6573 7420 7761  .The quickest wa
-00003090: 7920 746f 2065 7661 6c75 6174 6520 6073  y to evaluate `s
-000030a0: 6563 696d 706f 7274 6020 6973 2074 6f20  ecimport` is to 
-000030b0: 7573 6520 6f75 7220 5b44 6f63 6b65 7220  use our [Docker 
-000030c0: 636f 6e74 6169 6e65 725d 2864 6f63 6b65  container](docke
-000030d0: 722f 5245 4144 4d45 2e6d 6429 2c20 7768  r/README.md), wh
-000030e0: 6963 6820 696e 636c 7564 6573 2060 6270  ich includes `bp
-000030f0: 6674 7261 6365 6020 2860 6562 7066 6029  ftrace` (`ebpf`)
-00003100: 2061 6e64 206f 7468 6572 2070 6c75 672d   and other plug-
-00003110: 616e 642d 706c 6179 2065 7861 6d70 6c65  and-play example
-00003120: 732e 0a0a 0a23 2320 4578 616d 706c 6573  s....## Examples
-00003130: 0a0a 5468 6520 5b53 616e 6462 6f78 2045  ..The [Sandbox E
-00003140: 7861 6d70 6c65 735d 2868 7474 7073 3a2f  xamples](https:/
-00003150: 2f67 6974 6875 622e 636f 6d2f 6176 696c  /github.com/avil
-00003160: 756d 2f73 6563 696d 706f 7274 2f77 696b  um/secimport/wik
-00003170: 692f 5361 6e64 626f 782d 4578 616d 706c  i/Sandbox-Exampl
-00003180: 6573 2920 7061 6765 2063 6f6e 7461 696e  es) page contain
-00003190: 7320 6261 7369 6320 616e 6420 6164 7661  s basic and adva
-000031a0: 6e63 6564 2072 6561 6c2d 776f 726c 6420  nced real-world 
-000031b0: 6578 616d 706c 6573 2e0a 0a23 2320 436f  examples...## Co
-000031c0: 6e74 7269 6275 7469 6e67 0a0a 466f 7220  ntributing..For 
-000031d0: 696e 666f 726d 6174 696f 6e20 6f6e 2068  information on h
-000031e0: 6f77 2074 6f20 636f 6e74 7269 6275 7465  ow to contribute
-000031f0: 2074 6f20 6073 6563 696d 706f 7274 602c   to `secimport`,
-00003200: 2073 6565 2074 6865 205b 436f 6e74 7269   see the [Contri
-00003210: 6275 7469 6e67 5d28 6874 7470 733a 2f2f  buting](https://
-00003220: 6769 7468 7562 2e63 6f6d 2f61 7669 6c75  github.com/avilu
-00003230: 6d2f 7365 6369 6d70 6f72 742f 626c 6f62  m/secimport/blob
-00003240: 2f6d 6173 7465 722f 646f 6373 2f43 4f4e  /master/docs/CON
-00003250: 5452 4942 5554 494e 472e 6d64 2920 6775  TRIBUTING.md) gu
-00003260: 6964 652e 0a0a 2323 2052 6f61 646d 6170  ide...## Roadmap
-00003270: 0a0a 5365 6520 7468 6520 5b52 6f61 646d  ..See the [Roadm
-00003280: 6170 5d28 6874 7470 733a 2f2f 6769 7468  ap](https://gith
-00003290: 7562 2e63 6f6d 2f61 7669 6c75 6d2f 7365  ub.com/avilum/se
-000032a0: 6369 6d70 6f72 742f 626c 6f62 2f6d 6173  cimport/blob/mas
-000032b0: 7465 722f 646f 6373 2f52 4f41 444d 4150  ter/docs/ROADMAP
-000032c0: 2e6d 6429 2066 6f72 2074 6865 2070 6c61  .md) for the pla
-000032d0: 6e6e 6564 2066 6561 7475 7265 7320 616e  nned features an
-000032e0: 6420 6465 7665 6c6f 706d 656e 7420 6d69  d development mi
-000032f0: 6c65 7374 6f6e 6573 2e0a 0a23 2320 4368  lestones...## Ch
-00003300: 616e 6765 6c6f 670a 0a53 6565 2074 6865  angelog..See the
-00003310: 205b 4368 616e 6765 6c6f 675d 2868 7474   [Changelog](htt
-00003320: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003330: 6176 696c 756d 2f73 6563 696d 706f 7274  avilum/secimport
-00003340: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-00003350: 732f 4348 414e 4745 4c4f 472e 6d64 2920  s/CHANGELOG.md) 
-00003360: 666f 7220 6465 7665 6c6f 706d 656e 7420  for development 
-00003370: 7072 6f67 7265 7373 2061 6e64 2065 7869  progress and exi
-00003380: 7374 696e 6720 6665 6174 7572 6573 2e0a  sting features..
+000005d0: 652e 0a0a 5465 6368 6e69 6361 6c20 426c  e...Technical Bl
+000005e0: 6f67 7320 2846 7265 6520 5265 6164 696e  ogs (Free Readin
+000005f0: 6729 3a0a 312e 203c 6120 6872 6566 3d22  g):.1. <a href="
+00000600: 6874 7470 733a 2f2f 696e 666f 7365 6377  https://infosecw
+00000610: 7269 7465 7570 732e 636f 6d2f 7361 6e64  riteups.com/sand
+00000620: 626f 7869 6e67 2d70 7974 686f 6e2d 6d6f  boxing-python-mo
+00000630: 6475 6c65 732d 696e 2d79 6f75 722d 636f  dules-in-your-co
+00000640: 6465 2d31 6535 3930 6437 3166 6332 363f  de-1e590d71fc26?
+00000650: 736f 7572 6365 3d66 7269 656e 6473 5f6c  source=friends_l
+00000660: 696e 6b26 736b 3d35 6539 6132 6661 3464  ink&sk=5e9a2fa4d
+00000670: 3439 3231 6166 3065 6339 3466 3137 3566  4921af0ec94f175f
+00000680: 3765 6534 3966 3922 3e73 6563 696d 706f  7ee49f9">secimpo
+00000690: 7274 202b 2044 7472 6163 653c 2f61 3e0a  rt + Dtrace</a>.
+000006a0: 322e 203c 6120 6872 6566 3d22 6874 7470  2. <a href="http
+000006b0: 733a 2f2f 696e 666f 7365 6377 7269 7465  s://infosecwrite
+000006c0: 7570 732e 636f 6d2f 7365 6375 7269 6e67  ups.com/securing
+000006d0: 2d70 7974 6f72 6368 2d6d 6f64 656c 732d  -pytorch-models-
+000006e0: 7769 7468 2d65 6270 662d 3766 3735 3733  with-ebpf-7f7573
+000006f0: 3262 3834 3264 3f73 6f75 7263 653d 6672  2b842d?source=fr
+00000700: 6965 6e64 735f 6c69 6e6b 2673 6b3d 3134  iends_link&sk=14
+00000710: 6438 6462 3430 3361 6166 3636 3732 3461  d8db403aaf66724a
+00000720: 3861 3639 6234 6465 6132 3465 3132 223e  8a69b4dea24e12">
+00000730: 7365 6369 6d70 7274 202b 2065 4250 4620  secimprt + eBPF 
+00000740: 2b20 5079 546f 7263 683c 2f61 3e0a 332e  + PyTorch</a>.3.
+00000750: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000760: 2f2f 6176 692d 6c75 6d65 6c73 6b79 2e6d  //avi-lumelsky.m
+00000770: 6564 6975 6d2e 636f 6d2f 7365 6375 7265  edium.com/secure
+00000780: 2d66 6173 7461 7069 2d77 6974 682d 6562  -fastapi-with-eb
+00000790: 7066 2d37 3234 6434 6165 6638 6439 653f  pf-724d4aef8d9e?
+000007a0: 736f 7572 6365 3d66 7269 656e 6473 5f6c  source=friends_l
+000007b0: 696e 6b26 736b 3d62 3031 6136 6239 3765  ink&sk=b01a6b97e
+000007c0: 6630 3930 3033 6235 3363 6435 3263 3437  f09003b53cd52c47
+000007d0: 3930 3137 6230 3322 3e73 6563 696d 706f  9017b03">secimpo
+000007e0: 7274 202b 2065 4250 4620 2b20 4661 7374  rt + eBPF + Fast
+000007f0: 4150 4920 3c2f 613e 0a0a 2323 2320 5468  API </a>..### Th
+00000800: 6520 7072 6f62 6c65 6d0a 5472 6164 6974  e problem.Tradit
+00000810: 696f 6e61 6c20 746f 6f6c 7320 6c69 6b65  ional tools like
+00000820: 2073 6563 636f 6d70 206f 7220 4170 7041   seccomp or AppA
+00000830: 726d 6f72 2065 6e66 6f72 6365 2073 7973  rmor enforce sys
+00000840: 6361 6c6c 7320 666f 7220 7468 6520 656e  calls for the en
+00000850: 7469 7265 2070 726f 6365 7373 2e3c 6272  tire process.<br
+00000860: 3e53 6f6d 6574 6869 6e67 206c 696b 6520  >Something like 
+00000870: 6061 6c6c 6f77 6564 5f73 7973 6361 6c6c  `allowed_syscall
+00000880: 733d 5b22 7265 6164 222c 226f 7065 6e61  s=["read","opena
+00000890: 7422 2c22 6269 6e64 222c 2277 7269 7465  t","bind","write
+000008a0: 225d 602c 2077 6869 6368 2069 7320 6772  "]`, which is gr
+000008b0: 6561 742c 2062 7574 206e 6f74 2065 6e6f  eat, but not eno
+000008c0: 7567 6820 666f 7220 7079 7468 6f6e 2773  ugh for python's
+000008d0: 2061 7474 6163 6b20 7375 7266 6163 652e   attack surface.
+000008e0: 3c62 723e 0a0a 2323 2320 5468 6520 736f  <br>..### The so
+000008f0: 6c75 7469 6f6e 0a60 7365 6369 6d70 6f72  lution.`secimpor
+00000900: 7460 2069 7320 6162 6c65 2074 6f20 7472  t` is able to tr
+00000910: 6163 6520 7768 6963 6820 7379 7363 616c  ace which syscal
+00000920: 6c73 2065 6163 6820 6d6f 6475 6c65 2069  ls each module i
+00000930: 6e20 796f 7572 2063 6f64 6520 7573 6573  n your code uses
+00000940: 2028 6279 2070 6163 6b61 6765 206e 616d   (by package nam
+00000950: 6529 2e3c 6272 3e0a 4166 7465 7220 7472  e).<br>.After tr
+00000960: 6163 696e 672c 2073 6563 696d 706f 7274  acing, secimport
+00000970: 2063 7265 6174 6573 2061 204a 534f 4e2f   creates a JSON/
+00000980: 5941 4d4c 2070 6f6c 6963 7920 666f 7220  YAML policy for 
+00000990: 796f 7572 2063 6f64 652e 2049 7420 636f  your code. It co
+000009a0: 6d70 696c 6573 2069 7420 696e 746f 2061  mpiles it into a
+000009b0: 2068 6967 682d 7065 7266 6f72 6d61 6e63   high-performanc
+000009c0: 6520 6542 5046 2069 6e73 7472 756d 656e  e eBPF instrumen
+000009d0: 7461 7469 6f6e 2073 6372 6970 7420 2873  tation script (s
+000009e0: 6d61 6c6c 6572 2074 6865 6e20 3531 3220  maller then 512 
+000009f0: 6279 7465 7320 6f76 6572 616c 6c29 2c20  bytes overall), 
+00000a00: 7468 6174 206c 6f6f 6b73 206c 696b 6520  that looks like 
+00000a10: 3c61 3e74 6869 733c 2f61 3e2e 0a60 6060  <a>this</a>..```
+00000a20: 0a6d 6f64 756c 6573 3a0a 2020 7265 7175  .modules:.  requ
+00000a30: 6573 7473 3a0a 2020 2020 6465 7374 7275  ests:.    destru
+00000a40: 6374 6976 653a 2074 7275 6520 2020 2020  ctive: true     
+00000a50: 2320 7768 656e 2074 7275 652c 2073 6563  # when true, sec
+00000a60: 696d 706f 7274 2077 696c 6c20 6b69 6c6c  import will kill
+00000a70: 206f 6e20 7669 6c61 7469 6f6e 2069 6e73   on vilation ins
+00000a80: 7465 6164 206f 6620 6c6f 6767 696e 672e  tead of logging.
+00000a90: 0a20 2020 2073 7973 6361 6c6c 5f61 6c6c  .    syscall_all
+00000aa0: 6f77 6c69 7374 3a0a 2020 2020 2020 2d20  owlist:.      - 
+00000ab0: 6663 686d 6f64 0a20 2020 2020 202d 2067  fchmod.      - g
+00000ac0: 6574 656e 7472 6f70 790a 2020 2020 2020  etentropy.      
+00000ad0: 2d20 6765 7470 6772 700a 2020 2020 2020  - getpgrp.      
+00000ae0: 2d20 6765 7472 6c69 6d69 740a 2e2e 2e0a  - getrlimit.....
+00000af0: 6060 600a 596f 7520 6361 6e20 616c 736f  ```.You can also
+00000b00: 2075 7365 204a 534f 4e20 696e 7374 6165   use JSON instae
+00000b10: 6164 206f 6620 5941 4d4c 2c20 616e 6420  ad of YAML, and 
+00000b20: 6576 656e 2063 6f6e 6669 6e65 2062 7569  even confine bui
+00000b30: 6c74 696e 2070 7974 686f 6e20 6d6f 6475  ltin python modu
+00000b40: 6c65 732e 3c62 723e 0a41 6e20 6578 616d  les.<br>.An exam
+00000b50: 706c 6520 706f 6c69 6379 2074 6861 7420  ple policy that 
+00000b60: 7573 6573 206c 6f67 6769 6e67 2c20 6d75  uses logging, mu
+00000b70: 6c74 6970 726f 6365 7373 696e 672c 206f  ltiprocessing, o
+00000b80: 7320 616e 6420 6669 6c65 7379 7374 656d  s and filesystem
+00000b90: 2077 696c 6c20 6c6f 6f6b 2061 7070 726f   will look appro
+00000ba0: 7869 6d61 7465 6c79 206c 696b 6520 7468  ximately like th
+00000bb0: 6973 3a0a 6060 600a 2e2e 2e0a 2020 2020  is:.```.....    
+00000bc0: 222f 776f 726b 7370 6163 652f 5079 7468  "/workspace/Pyth
+00000bd0: 6f6e 2d33 2e31 302e 302f 4c69 622f 6c6f  on-3.10.0/Lib/lo
+00000be0: 6767 696e 672f 5f5f 696e 6974 5f5f 2e70  gging/__init__.p
+00000bf0: 7922 3a20 5b0a 2020 2020 2020 2020 2220  y": [.        " 
+00000c00: 636c 6f63 6b5f 6765 7474 696d 6522 2c0a  clock_gettime",.
+00000c10: 2020 2020 2020 2020 2220 6765 7470 6964          " getpid
+00000c20: 222c 0a20 2020 2020 2020 2022 2077 7269  ",.        " wri
+00000c30: 7465 220a 2020 2020 5d2c 0a20 2020 2022  te".    ],.    "
+00000c40: 2f77 6f72 6b73 7061 6365 2f50 7974 686f  /workspace/Pytho
+00000c50: 6e2d 332e 3130 2e30 2f4c 6962 2f6d 756c  n-3.10.0/Lib/mul
+00000c60: 7469 7072 6f63 6573 7369 6e67 2f70 726f  tiprocessing/pro
+00000c70: 6365 7373 2e70 7922 3a20 5b0a 2020 2020  cess.py": [.    
+00000c80: 2020 2020 2220 6765 7463 7764 222c 0a20      " getcwd",. 
+00000c90: 2020 2020 2020 2022 2067 6574 7069 6422         " getpid"
+00000ca0: 2c0a 2020 2020 2020 2020 2220 6765 7472  ,.        " getr
+00000cb0: 616e 646f 6d22 0a20 2020 205d 2c0a 2020  andom".    ],.  
+00000cc0: 2020 222f 776f 726b 7370 6163 652f 5079    "/workspace/Py
+00000cd0: 7468 6f6e 2d33 2e31 302e 302f 4c69 622f  thon-3.10.0/Lib/
+00000ce0: 6d75 6c74 6970 726f 6365 7373 696e 672f  multiprocessing/
+00000cf0: 7574 696c 2e70 7922 3a20 5b0a 2020 2020  util.py": [.    
+00000d00: 2020 2020 2220 7072 6c69 6d69 7436 3422      " prlimit64"
+00000d10: 0a20 2020 205d 2c0a 2020 2020 222f 776f  .    ],.    "/wo
+00000d20: 726b 7370 6163 652f 5079 7468 6f6e 2d33  rkspace/Python-3
+00000d30: 2e31 302e 302f 4c69 622f 6f73 2e70 7922  .10.0/Lib/os.py"
+00000d40: 3a20 5b0a 2020 2020 2020 2020 2220 7265  : [.        " re
+00000d50: 6164 220a 2020 2020 5d2c 0a20 2020 2022  ad".    ],.    "
+00000d60: 2f77 6f72 6b73 7061 6365 2f50 7974 686f  /workspace/Pytho
+00000d70: 6e2d 332e 3130 2e30 2f4c 6962 2f70 6c61  n-3.10.0/Lib/pla
+00000d80: 7466 6f72 6d2e 7079 223a 205b 0a20 2020  tform.py": [.   
+00000d90: 2020 2020 2022 2075 6e61 6d65 220a 2020       " uname".  
+00000da0: 2020 5d2c 0a20 2020 2022 2f77 6f72 6b73    ],.    "/works
+00000db0: 7061 6365 2f50 7974 686f 6e2d 332e 3130  pace/Python-3.10
+00000dc0: 2e30 2f4c 6962 2f70 6f73 6978 7061 7468  .0/Lib/posixpath
+00000dd0: 2e70 7922 3a20 5b0a 2020 2020 2020 2020  .py": [.        
+00000de0: 2220 636c 6f73 6522 2c0a 2020 2020 2020  " close",.      
+00000df0: 2020 2220 6673 7461 7422 2c0a 2020 2020    " fstat",.    
+00000e00: 2020 2020 2220 6765 7463 7764 222c 0a20      " getcwd",. 
+00000e10: 2020 2020 2020 2022 2067 6574 6465 6e74         " getdent
+00000e20: 7336 3422 2c0a 2020 2020 2020 2020 2220  s64",.        " 
+00000e30: 6f70 656e 6174 220a 2020 2020 5d2c 0a20  openat".    ],. 
+00000e40: 2020 2022 2f77 6f72 6b73 7061 6365 2f50     "/workspace/P
+00000e50: 7974 686f 6e2d 332e 3130 2e30 2f4c 6962  ython-3.10.0/Lib
+00000e60: 2f72 616e 646f 6d2e 7079 223a 205b 0a20  /random.py": [. 
+00000e70: 2020 2020 2020 2022 2067 6574 7261 6e64         " getrand
+00000e80: 6f6d 220a 2020 2020 5d2c 0a2e 2e2e 0a60  om".    ],.....`
+00000e90: 6060 0a49 7420 7761 7320 6372 6561 7465  ``.It was create
+00000ea0: 6420 6279 2074 7261 6369 6e67 2074 6865  d by tracing the
+00000eb0: 2063 6f64 652e 2073 6563 696d 706f 7274   code. secimport
+00000ec0: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
+00000ed0: 696e 6473 2074 6865 7365 2070 6572 2d6d  inds these per-m
+00000ee0: 6f64 756c 6520 7379 7363 616c 6c73 2066  odule syscalls f
+00000ef0: 6f72 2079 6f75 2e0a 0a46 696e 616c 6c79  or you...Finally
+00000f00: 2c20 796f 7520 636f 6e76 6572 7420 7468  , you convert th
+00000f10: 6973 2070 6f6c 6963 7920 696e 746f 2061  is policy into a
+00000f20: 6e20 7361 6e64 626f 7820 2865 4250 4620  n sandbox (eBPF 
+00000f30: 696e 7374 7275 6d65 6e74 6174 696f 6e20  instrumentation 
+00000f40: 7363 7269 7074 2920 746f 2072 756e 2074  script) to run t
+00000f50: 6865 2070 7974 686f 6e20 7072 6f63 6573  he python proces
+00000f60: 7320 696e 2070 726f 6475 6374 696f 6e2e  s in production.
+00000f70: 2052 756e 6e69 6e67 2074 6865 2073 616e   Running the san
+00000f80: 6462 6f78 2077 696c 6c20 656e 666f 7265  dbox will enfore
+00000f90: 2070 7974 686f 6e20 746f 206f 6265 7920   python to obey 
+00000fa0: 616e 7920 6769 7665 6e20 706f 6c69 6379  any given policy
+00000fb0: 2e0a 0a60 7365 6369 6d70 6f72 7460 2069  ...`secimport` i
+00000fc0: 7320 6772 6561 7420 666f 722e 2e2e 0a2d  s great for....-
+00000fd0: 2050 7265 7665 6e74 696e 6720 436f 6465   Preventing Code
+00000fe0: 2045 7865 6375 7469 6f6e 3a20 7265 6475   Execution: redu
+00000ff0: 6365 2074 6865 2072 6973 6b20 6f66 2073  ce the risk of s
+00001000: 7570 706c 7920 6368 6169 6e20 6174 7461  upply chain atta
+00001010: 636b 732e 0a20 202d 2054 7261 6365 2074  cks..  - Trace t
+00001020: 6865 2073 7973 6361 6c6c 7320 666c 6f77  he syscalls flow
+00001030: 206f 6620 796f 7572 2061 7070 6c69 6361   of your applica
+00001040: 7469 6f6e 2061 7420 7468 6520 7573 6572  tion at the user
+00001050: 2d73 7061 6365 2f6f 732f 6b65 726e 656c  -space/os/kernel
+00001060: 206c 6576 656c 2061 6e64 2070 6572 206d   level and per m
+00001070: 6f64 756c 652e 0a20 202d 2052 756e 2079  odule..  - Run y
+00001080: 6f75 7220 6170 706c 6963 6174 696f 6e20  our application 
+00001090: 7768 696c 6520 656e 666f 7263 696e 6720  while enforcing 
+000010a0: 7379 7363 616c 6c73 2070 6572 206d 6f64  syscalls per mod
+000010b0: 756c 652e 0a20 2020 202d 2055 706f 6e20  ule..    - Upon 
+000010c0: 7669 6f6c 6174 696f 6e20 6f66 2074 6865  violation of the
+000010d0: 2070 6f6c 6963 792c 2069 7420 6361 6e20   policy, it can 
+000010e0: 6c6f 672c 2073 746f 702c 206f 7220 6b69  log, stop, or ki
+000010f0: 6c6c 2074 6865 2070 726f 6365 7373 2e0a  ll the process..
+00001100: 2d20 5072 6f74 6563 7420 796f 7572 7365  - Protect yourse
+00001110: 6c66 2066 726f 6d20 5243 453a 0a20 202d  lf from RCE:.  -
+00001120: 2073 6563 696d 706f 7274 206d 616b 6573   secimport makes
+00001130: 2031 6461 7920 6174 7461 636b 7320 6c65   1day attacks le
+00001140: 7373 206f 6620 616e 2069 7373 7565 2c20  ss of an issue, 
+00001150: 6265 6361 7573 6520 6974 2070 7265 7665  because it preve
+00001160: 6e74 7320 7468 6520 636f 6465 2066 6f72  nts the code for
+00001170: 6d20 7275 6e6e 696e 672e 2049 6620 796f  m running. If yo
+00001180: 7520 6172 6520 7573 696e 6720 6120 7675  u are using a vu
+00001190: 6c6e 6572 6162 6c65 2070 6163 6b61 6765  lnerable package
+000011a0: 2061 6e64 2073 6f6d 656f 6e65 2065 7870   and someone exp
+000011b0: 6c6f 6974 6564 2069 742c 2079 6f75 7220  loited it, your 
+000011c0: 706f 6c69 6379 2077 696c 6c20 6e6f 7420  policy will not 
+000011d0: 616c 6c6f 7720 7468 6973 2065 7870 6c6f  allow this explo
+000011e0: 6974 2773 2073 7973 6361 6c6c 7320 616e  it's syscalls an
+000011f0: 6420 6974 2077 696c 6c20 6265 2068 616e  d it will be han
+00001200: 646c 6564 2061 7320 796f 7520 7769 7368  dled as you wish
+00001210: 2e0a 2020 2d20 4176 6f69 6420 696e 6369  ..  - Avoid inci
+00001220: 6465 6e74 7320 6c69 6b65 203c 6120 6872  dents like <a hr
+00001230: 6566 3d22 6874 7470 733a 2f2f 656e 2e77  ef="https://en.w
+00001240: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00001250: 692f 4c6f 6734 5368 656c 6c22 3e6c 6f67  i/Log4Shell">log
+00001260: 3473 6865 6c6c 3c2f 613e 2e20 4120 6c6f  4shell</a>. A lo
+00001270: 6767 696e 6720 6c69 6272 6172 7920 7265  gging library re
+00001280: 7175 6972 6573 2076 6572 7920 6665 7720  quires very few 
+00001290: 7379 7363 616c 6c73 2c20 616e 6420 6974  syscalls, and it
+000012a0: 2073 686f 756c 6420 6e65 7665 7220 7275   should never ru
+000012b0: 6e20 636f 6d6d 616e 6420 7573 696e 6720  n command using 
+000012c0: 666f 726b 2c20 6578 6563 7665 206f 7220  fork, execve or 
+000012d0: 7370 6177 6e2e 0a20 2020 202d 2054 6865  spawn..    - The
+000012e0: 2073 7973 6361 6c6c 7320 7468 6174 2022   syscalls that "
+000012f0: 6661 7374 6170 6922 2c20 226e 756d 7079  fastapi", "numpy
+00001300: 2220 6f72 2022 7265 7175 6573 7473 2220  " or "requests" 
+00001310: 7573 6520 6172 6520 7665 7279 2064 6966  use are very dif
+00001320: 6665 7265 6e74 2e0a 2d20 4c6f 6164 2041  ferent..- Load A
+00001330: 4920 4d6f 6465 6c73 2066 726f 6d20 496e  I Models from In
+00001340: 7365 6375 7265 2053 6f75 7263 6573 0a20  secure Sources. 
+00001350: 202d 204d 6f64 656c 7320 6672 6f6d 2075   - Models from u
+00001360: 6e73 6166 6520 736f 7572 6365 2028 6875  nsafe source (hu
+00001370: 6767 696e 6766 6163 652c 2074 6f72 6368  ggingface, torch
+00001380: 2068 7562 2c20 616e 6420 7079 746f 7263   hub, and pytorc
+00001390: 6820 7069 636b 6c65 6420 6d6f 6465 6c73  h pickled models
+000013a0: 2920 6361 6e20 6265 206c 696d 6974 6564  ) can be limited
+000013b0: 2074 6f20 7275 6e20 6f6e 6c79 2061 2073   to run only a s
+000013c0: 6574 206f 6620 7379 7363 616c 6c73 2e20  et of syscalls. 
+000013d0: 5243 4520 6c69 6b65 2027 696d 706f 7274  RCE like 'import
+000013e0: 206f 733b 6f73 2e73 7973 7465 6d28 2e2e   os;os.system(..
+000013f0: 2e29 2720 736f 6d65 7768 6572 6520 6465  .)' somewhere de
+00001400: 6570 2069 6e20 7468 6520 636f 6465 2077  ep in the code w
+00001410: 696c 6c20 6265 2063 6174 6368 6564 2062  ill be catched b
+00001420: 7920 7365 6369 6d70 6f72 742e 0a2d 204d  y secimport..- M
+00001430: 696e 696d 616c 2050 6572 666f 726d 616e  inimal Performan
+00001440: 6365 2049 6d70 6163 740a 2020 2d20 2048  ce Impact.  -  H
+00001450: 6173 206e 6567 6c69 6769 626c 6520 7065  as negligible pe
+00001460: 7266 6f72 6d61 6e63 6520 696d 7061 6374  rformance impact
+00001470: 2061 6e64 2069 7320 7072 6f64 7563 7469   and is producti
+00001480: 6f6e 2d72 6561 6479 2074 6861 6e6b 7320  on-ready thanks 
+00001490: 746f 2065 4250 462e 2043 6865 636b 206f  to eBPF. Check o
+000014a0: 7574 2074 6865 205b 5065 7266 6f72 6d61  ut the [Performa
+000014b0: 6e63 655d 2868 7474 7073 3a2f 2f67 6974  nce](https://git
+000014c0: 6875 622e 636f 6d2f 6176 696c 756d 2f73  hub.com/avilum/s
+000014d0: 6563 696d 706f 7274 2f77 696b 692f 5065  ecimport/wiki/Pe
+000014e0: 7266 6f72 6d61 6e63 652d 4265 6e63 686d  rformance-Benchm
+000014f0: 6172 6b73 2920 6265 6e63 686d 6172 6b73  arks) benchmarks
+00001500: 2e0a 2d20 5472 6163 6520 7768 6963 6820  ..- Trace which 
+00001510: 7379 7363 616c 6c73 2061 7265 2063 616c  syscalls are cal
+00001520: 6c65 6420 6279 2065 6163 6820 6d6f 6475  led by each modu
+00001530: 6c65 2069 6e20 796f 7572 2063 6f64 652e  le in your code.
+00001540: 0a20 202d 2073 6563 696d 706f 7274 2075  .  - secimport u
+00001550: 7365 7320 5553 4454 2028 5573 6572 6c61  ses USDT (Userla
+00001560: 6e64 2053 7461 7469 6361 6c6c 7920 4465  nd Statically De
+00001570: 6669 6e65 6420 5472 6163 696e 6729 2074  fined Tracing) t
+00001580: 6f67 6574 6865 7220 7769 7468 206b 6572  ogether with ker
+00001590: 6e65 6c20 7072 6f62 6573 2069 6e20 7468  nel probes in th
+000015a0: 6520 7275 6e74 696d 6520 7573 696e 6720  e runtime using 
+000015b0: 6542 5046 206f 7220 6474 7261 6365 2069  eBPF or dtrace i
+000015c0: 6e73 7472 756d 656e 7461 7469 6f6e 2073  nstrumentation s
+000015d0: 6372 6970 7473 2e0a 2323 2049 6e73 7461  cripts..## Insta
+000015e0: 6c6c 6174 696f 6e0a 5465 7374 6564 206f  llation.Tested o
+000015f0: 6e20 5562 756e 7475 2c20 4465 6269 616e  n Ubuntu, Debian
+00001600: 2c20 526f 636b 7920 284c 696e 7578 2078  , Rocky (Linux x
+00001610: 3836 2f41 4d44 2f41 524d 2920 616e 6420  86/AMD/ARM) and 
+00001620: 4d61 634f 5320 696e 2028 7838 362f 4d31  MacOS in (x86/M1
+00001630: 292e 2049 6620 796f 7520 7275 6e20 6f6e  ). If you run on
+00001640: 204d 6163 4f53 2079 6f75 2077 696c 6c20   MacOS you will 
+00001650: 6e65 6564 2074 6f20 3c61 2068 7265 663d  need to <a href=
+00001660: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001670: 636f 6d2f 6176 696c 756d 2f73 6563 696d  com/avilum/secim
+00001680: 706f 7274 2f62 6c6f 622f 6d61 7374 6572  port/blob/master
+00001690: 2f64 6f63 732f 4d41 435f 4f53 5f55 5345  /docs/MAC_OS_USE
+000016a0: 5253 2e6d 6422 3e64 6973 6162 6c65 2053  RS.md">disable S
+000016b0: 4950 2066 6f72 2064 7472 6163 652e 203c  IP for dtrace. <
+000016c0: 2f61 3e0a 0a23 2320 5769 7468 2044 6f63  /a>..## With Doc
+000016d0: 6b65 720a 466f 7220 7175 6963 6b65 7220  ker.For quicker 
+000016e0: 6576 616c 7561 7469 6f6e 2c20 7765 2072  evaluation, we r
+000016f0: 6563 6f6d 6d65 6e64 2075 7369 6e67 2074  ecommend using t
+00001700: 6865 203c 6120 6872 6566 3d22 5b64 6f63  he <a href="[doc
+00001710: 732f 446f 636b 6572 5d28 6874 7470 733a  s/Docker](https:
+00001720: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
+00001730: 6c75 6d2f 7365 6369 6d70 6f72 742f 626c  lum/secimport/bl
+00001740: 6f62 2f6d 6173 7465 722f 646f 636b 6572  ob/master/docker
+00001750: 2f52 4541 444d 452e 6d64 2922 3e53 6563  /README.md)">Sec
+00001760: 696d 706f 7274 2044 6f63 6b65 7220 496d  import Docker Im
+00001770: 6167 653c 2f61 3e20 696e 7374 6561 6420  age</a> instead 
+00001780: 6f66 2073 656c 662d 696e 7374 616c 6c69  of self-installi
+00001790: 6e67 2e3c 6272 3e0a 2d20 4275 696c 6420  ng.<br>.- Build 
+000017a0: 616e 6420 7275 6e20 7468 6520 446f 636b  and run the Dock
+000017b0: 6572 2063 6f6e 7461 696e 6572 2077 6974  er container wit
+000017c0: 6820 6120 6375 7374 6f6d 206b 6572 6e65  h a custom kerne
+000017d0: 6c20 7468 6174 206d 6174 6368 6573 2079  l that matches y
+000017e0: 6f75 7220 6578 6973 7469 6e67 204f 5320  our existing OS 
+000017f0: 6b65 726e 656c 2076 6572 7369 6f6e 3a0a  kernel version:.
+00001800: 2020 6060 600a 2020 6364 2064 6f63 6b65    ```.  cd docke
+00001810: 722f 2026 2620 2e2f 6275 696c 642e 7368  r/ && ./build.sh
+00001820: 2026 2620 2e2f 7275 6e2e 7368 0a20 2060   && ./run.sh.  `
+00001830: 6060 0a20 2041 2074 656d 706f 7261 7279  ``.  A temporary
+00001840: 2063 6f6e 7461 696e 6572 2077 696c 6c20   container will 
+00001850: 6265 2063 7265 6174 6564 2c20 616e 6420  be created, and 
+00001860: 796f 7520 7769 6c6c 2062 6520 6c6f 6767  you will be logg
+00001870: 6564 2069 6e20 6173 2074 6865 2072 6f6f  ed in as the roo
+00001880: 7420 7573 6572 2e0a 0a23 2320 5769 7468  t user...## With
+00001890: 6f75 7420 446f 636b 6572 0a31 2e20 496e  out Docker.1. In
+000018a0: 7374 616c 6c20 7079 7468 6f6e 2077 6974  stall python wit
+000018b0: 6820 5553 4454 2070 726f 6265 7320 6279  h USDT probes by
+000018c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000018d0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
+000018e0: 6c75 6d2f 7365 6369 6d70 6f72 742f 7769  lum/secimport/wi
+000018f0: 6b69 2f49 6e73 7461 6c6c 6174 696f 6e23  ki/Installation#
+00001900: 7079 7468 6f6e 2d69 6e74 6572 7072 6574  python-interpret
+00001910: 6572 2d72 6571 7569 7265 6d65 6e74 7322  er-requirements"
+00001920: 3e63 6f6e 6669 6775 7269 6e67 2069 7420  >configuring it 
+00001930: 7769 7468 2027 2d2d 6474 7261 6365 273c  with '--dtrace'<
+00001940: 2f61 3e0a 322e 2049 6e73 7461 6c6c 206f  /a>.2. Install o
+00001950: 6e65 206f 6620 7468 6520 6261 636b 656e  ne of the backen
+00001960: 6473 3a20 3c61 2068 7265 663d 2268 7474  ds: <a href="htt
+00001970: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001980: 6176 696c 756d 2f73 6563 696d 706f 7274  avilum/secimport
+00001990: 2f77 696b 692f 496e 7374 616c 6c61 7469  /wiki/Installati
+000019a0: 6f6e 223e 6542 5046 206f 7220 4454 7261  on">eBPF or DTra
+000019b0: 6365 3c2f 613e 2e0a 332e 2049 6e73 7461  ce</a>..3. Insta
+000019c0: 6c6c 2073 6563 696d 706f 7274 0a20 202d  ll secimport.  -
+000019d0: 2049 6e73 7461 6c6c 2066 726f 6d20 7079   Install from py
+000019e0: 7069 0a20 2020 202d 2060 6060 0a20 2020  pi.    - ```.   
+000019f0: 2020 2070 7974 686f 6e33 202d 6d20 7069     python3 -m pi
+00001a00: 7020 696e 7374 616c 6c20 7365 6369 6d70  p install secimp
+00001a10: 6f72 740a 2020 2020 2020 6060 600a 2020  ort.      ```.  
+00001a20: 2d20 496e 7374 616c 6c20 6672 6f6d 2073  - Install from s
+00001a30: 6f75 7263 650a 2020 2020 2d20 6060 600a  ource.    - ```.
+00001a40: 2020 2020 2020 6769 7420 636c 6f6e 6520        git clone 
+00001a50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001a60: 6f6d 2f61 7669 6c75 6d2f 7365 6369 6d70  om/avilum/secimp
+00001a70: 6f72 742e 6769 7420 2626 2063 6420 7365  ort.git && cd se
+00001a80: 6369 6d70 6f72 740a 2020 2020 2020 7079  cimport.      py
+00001a90: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
+00001aa0: 7461 6c6c 2070 6f65 7472 7920 2626 2070  tall poetry && p
+00001ab0: 7974 686f 6e33 202d 6d20 706f 6574 7279  ython3 -m poetry
+00001ac0: 2069 6e73 7461 6c6c 0a20 2020 2020 2060   install.      `
+00001ad0: 6060 0a0a 0a23 2320 5573 6167 650a 546f  ``...## Usage.To
+00001ae0: 2073 616e 6462 6f78 2079 6f75 7220 7072   sandbox your pr
+00001af0: 6f67 7261 6d20 7573 696e 6720 7468 6520  ogram using the 
+00001b00: 434c 492c 2073 7461 7274 2061 2062 7066  CLI, start a bpf
+00001b10: 7472 6163 6520 7072 6f67 7261 6d20 7468  trace program th
+00001b20: 6174 206c 6f67 7320 616c 6c20 7468 6520  at logs all the 
+00001b30: 7379 7363 616c 6c73 2066 6f72 2061 6c6c  syscalls for all
+00001b40: 2074 6865 206d 6f64 756c 6573 2069 6e20   the modules in 
+00001b50: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
+00001b60: 2069 6e74 6f20 6120 6669 6c65 2077 6974   into a file wit
+00001b70: 6820 7468 6520 7365 6369 6d70 6f72 7420  h the secimport 
+00001b80: 7472 6163 6520 636f 6d6d 616e 642e 204f  trace command. O
+00001b90: 6e63 6520 796f 7520 6861 7665 2063 6f76  nce you have cov
+00001ba0: 6572 6564 2074 6865 206c 6f67 6963 2079  ered the logic y
+00001bb0: 6f75 2077 6f75 6c64 206c 696b 6520 746f  ou would like to
+00001bc0: 2073 616e 6462 6f78 2c20 6869 7420 4354   sandbox, hit CT
+00001bd0: 524c 2b43 206f 7220 4354 524c 2b44 2c20  RL+C or CTRL+D, 
+00001be0: 6f72 2077 6169 7420 666f 7220 7468 6520  or wait for the 
+00001bf0: 7072 6f67 7261 6d20 746f 2066 696e 6973  program to finis
+00001c00: 682e 2054 6865 6e2c 2062 7569 6c64 2061  h. Then, build a
+00001c10: 2073 616e 6462 6f78 2066 726f 6d20 7468   sandbox from th
+00001c20: 6520 7472 6163 6520 7573 696e 6720 7468  e trace using th
+00001c30: 6520 7365 6369 6d70 6f72 7420 6275 696c  e secimport buil
+00001c40: 6420 636f 6d6d 616e 642c 2061 6e64 2072  d command, and r
+00001c50: 756e 2074 6865 2073 616e 6462 6f78 2077  un the sandbox w
+00001c60: 6974 6820 7468 6520 7365 6369 6d70 6f72  ith the secimpor
+00001c70: 7420 7275 6e20 636f 6d6d 616e 642e 0a0a  t run command...
+00001c80: 6060 6073 6865 6c6c 0a4e 414d 450a 2020  ```shell.NAME.  
+00001c90: 2020 7365 6369 6d70 6f72 7420 2d20 6973    secimport - is
+00001ca0: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
+00001cb0: 2074 6f6f 6c6b 6974 2064 6573 6967 6e65   toolkit designe
+00001cc0: 6420 746f 2065 6e61 626c 6520 7468 6520  d to enable the 
+00001cd0: 7472 6163 696e 672c 2063 6f6e 7374 7275  tracing, constru
+00001ce0: 6374 696f 6e2c 2061 6e64 2065 7865 6375  ction, and execu
+00001cf0: 7469 6f6e 206f 6620 7365 6375 7265 2050  tion of secure P
+00001d00: 7974 686f 6e20 7275 6e74 696d 6573 2e20  ython runtimes. 
+00001d10: 4974 206c 6576 6572 6167 6573 2055 5344  It leverages USD
+00001d20: 5420 7072 6f62 6573 2061 6e64 2065 4250  T probes and eBP
+00001d30: 462f 4454 7261 6365 2074 6563 686e 6f6c  F/DTrace technol
+00001d40: 6f67 6965 7320 746f 2065 6e68 616e 6365  ogies to enhance
+00001d50: 2074 6865 206f 7665 7261 6c6c 2073 6563   the overall sec
+00001d60: 7572 6974 7920 6d65 6173 7572 6573 2e0a  urity measures..
+00001d70: 0a53 594e 4f50 5349 530a 2020 2020 7365  .SYNOPSIS.    se
+00001d80: 6369 6d70 6f72 7420 434f 4d4d 414e 440a  cimport COMMAND.
+00001d90: 0a44 4553 4352 4950 5449 4f4e 0a20 2020  .DESCRIPTION.   
+00001da0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001db0: 636f 6d2f 6176 696c 756d 2f73 6563 696d  com/avilum/secim
+00001dc0: 706f 7274 2f77 696b 692f 436f 6d6d 616e  port/wiki/Comman
+00001dd0: 642d 4c69 6e65 2d55 7361 6765 0a0a 2020  d-Line-Usage..  
+00001de0: 2020 574f 524b 464c 4f57 3a0a 2020 2020    WORKFLOW:.    
+00001df0: 2020 2020 2020 2020 312e 2073 6563 696d          1. secim
+00001e00: 706f 7274 2074 7261 6365 202f 2073 6563  port trace / sec
+00001e10: 696d 706f 7274 2073 6865 6c6c 0a20 2020  import shell.   
+00001e20: 2020 2020 2020 2020 2032 2e20 7365 6369           2. seci
+00001e30: 6d70 6f72 7420 6275 696c 640a 2020 2020  mport build.    
+00001e40: 2020 2020 2020 2020 332e 2073 6563 696d          3. secim
+00001e50: 706f 7274 2072 756e 0a0a 2020 2020 5155  port run..    QU
+00001e60: 4943 4b53 5441 5254 3a0a 2020 2020 2020  ICKSTART:.      
+00001e70: 2020 2020 2020 2420 7365 6369 6d70 6f72        $ secimpor
+00001e80: 7420 696e 7465 7261 6374 6976 650a 0a20  t interactive.. 
+00001e90: 2020 2045 5841 4d50 4c45 533a 0a20 2020     EXAMPLES:.   
+00001ea0: 2020 2020 2031 2e20 7472 6163 653a 0a20       1. trace:. 
+00001eb0: 2020 2020 2020 2020 2020 2024 2020 7365             $  se
+00001ec0: 6369 6d70 6f72 7420 7472 6163 650a 2020  cimport trace.  
+00001ed0: 2020 2020 2020 2020 2020 2420 2073 6563            $  sec
+00001ee0: 696d 706f 7274 2074 7261 6365 202d 680a  import trace -h.
+00001ef0: 2020 2020 2020 2020 2020 2020 2420 2073              $  s
+00001f00: 6563 696d 706f 7274 2074 7261 6365 5f70  ecimport trace_p
+00001f10: 6964 2031 3233 0a20 2020 2020 2020 2020  id 123.         
+00001f20: 2020 2024 2020 7365 6369 6d70 6f72 7420     $  secimport 
+00001f30: 7472 6163 655f 7069 6420 2d68 0a20 2020  trace_pid -h.   
+00001f40: 2020 2020 2032 2e20 6275 696c 643a 0a20       2. build:. 
+00001f50: 2020 2020 2020 2020 2020 2023 2073 6563             # sec
+00001f60: 696d 706f 7274 2062 7569 6c64 0a20 2020  import build.   
+00001f70: 2020 2020 2020 2020 2024 2073 6563 696d           $ secim
+00001f80: 706f 7274 2062 7569 6c64 202d 680a 2020  port build -h.  
+00001f90: 2020 2020 2020 332e 2072 756e 3a0a 2020        3. run:.  
+00001fa0: 2020 2020 2020 2020 2020 2420 2073 6563            $  sec
+00001fb0: 696d 706f 7274 2072 756e 0a20 2020 2020  import run.     
+00001fc0: 2020 2020 2020 2024 2020 7365 6369 6d70         $  secimp
+00001fd0: 6f72 7420 7275 6e20 2d2d 656e 7472 7970  ort run --entryp
+00001fe0: 6f69 6e74 206d 795f 6375 7374 6f6d 5f6d  oint my_custom_m
+00001ff0: 6169 6e2e 7079 0a20 2020 2020 2020 2020  ain.py.         
+00002000: 2020 2024 2020 7365 6369 6d70 6f72 7420     $  secimport 
+00002010: 7275 6e20 2d2d 656e 7472 7970 6f69 6e74  run --entrypoint
+00002020: 206d 795f 6375 7374 6f6d 5f6d 6169 6e2e   my_custom_main.
+00002030: 7079 202d 2d73 746f 705f 6f6e 5f76 696f  py --stop_on_vio
+00002040: 6c61 7469 6f6e 3d74 7275 650a 2020 2020  lation=true.    
+00002050: 2020 2020 2020 2020 2420 2073 6563 696d          $  secim
+00002060: 706f 7274 2072 756e 202d 2d65 6e74 7279  port run --entry
+00002070: 706f 696e 7420 6d79 5f63 7573 746f 6d5f  point my_custom_
+00002080: 6d61 696e 2e70 7920 2d2d 6b69 6c6c 5f6f  main.py --kill_o
+00002090: 6e5f 7669 6f6c 6174 696f 6e3d 7472 7565  n_violation=true
+000020a0: 0a20 2020 2020 2020 2020 2020 2024 2020  .            $  
+000020b0: 7365 6369 6d70 6f72 7420 7275 6e20 2d2d  secimport run --
+000020c0: 7361 6e64 626f 785f 6578 6563 7574 6162  sandbox_executab
+000020d0: 6c65 202f 7061 7468 2f74 6f2f 6d79 5f73  le /path/to/my_s
+000020e0: 616e 6462 6f78 2e62 7420 2d2d 7069 6420  andbox.bt --pid 
+000020f0: 3238 3834 0a20 2020 2020 2020 2020 2020  2884.           
+00002100: 2024 2020 7365 6369 6d70 6f72 7420 7275   $  secimport ru
+00002110: 6e20 2d2d 7361 6e64 626f 785f 6578 6563  n --sandbox_exec
+00002120: 7574 6162 6c65 202f 7061 7468 2f74 6f2f  utable /path/to/
+00002130: 6d79 5f73 616e 6462 6f78 2e62 7420 2d2d  my_sandbox.bt --
+00002140: 7361 6e64 626f 785f 6c6f 6766 696c 6520  sandbox_logfile 
+00002150: 6d79 5f6c 6f67 2e6c 6f67 0a20 2020 2020  my_log.log.     
+00002160: 2020 2020 2020 2024 2020 7365 6369 6d70         $  secimp
+00002170: 6f72 7420 7275 6e20 2d68 0a0a 434f 4d4d  ort run -h..COMM
+00002180: 414e 4453 0a20 2020 2043 4f4d 4d41 4e44  ANDS.    COMMAND
+00002190: 2069 7320 6f6e 6520 6f66 2074 6865 2066   is one of the f
+000021a0: 6f6c 6c6f 7769 6e67 3a0a 0a20 2020 2020  ollowing:..     
+000021b0: 6275 696c 640a 2020 2020 2020 2043 6f6d  build.       Com
+000021c0: 7069 6c65 7320 6120 7472 6163 6520 6c6f  piles a trace lo
+000021d0: 6720 2874 7261 6365 2e6c 6f67 292e 2043  g (trace.log). C
+000021e0: 7265 6174 6573 2074 6865 2073 616e 6462  reates the sandb
+000021f0: 6f78 2065 7865 6375 7461 626c 6520 2869  ox executable (i
+00002200: 6e73 7472 756d 656e 7461 7469 6f6e 2073  nstrumentation s
+00002210: 6372 6970 7429 2066 6f72 2065 6163 6820  cript) for each 
+00002220: 7375 7070 6f72 7465 6420 6261 636b 656e  supported backen
+00002230: 6420 4974 2075 7365 7320 6063 7265 6174  d It uses `creat
+00002240: 655f 7072 6f66 696c 655f 6672 6f6d 5f74  e_profile_from_t
+00002250: 7261 6365 202e 2e2e 6020 616e 6420 6073  race ...` and `s
+00002260: 616e 6462 6f78 5f66 726f 6d5f 7072 6f66  andbox_from_prof
+00002270: 696c 6560 2e0a 0a20 2020 2020 636f 6d70  ile`...     comp
+00002280: 696c 655f 7361 6e64 626f 785f 6672 6f6d  ile_sandbox_from
+00002290: 5f70 726f 6669 6c65 0a20 2020 2020 2020  _profile.       
+000022a0: 4765 6e65 7261 7465 7320 6120 7461 696c  Generates a tail
+000022b0: 6f72 2d6d 6164 6520 7361 6e64 626f 7820  or-made sandbox 
+000022c0: 7468 6174 2077 696c 6c20 656e 666f 7263  that will enforc
+000022d0: 6520 6120 6769 7665 6e20 7961 6d6c 2070  e a given yaml p
+000022e0: 726f 6669 6c65 2f70 6f6c 6963 7920 696e  rofile/policy in
+000022f0: 2072 756e 7469 6d65 2e0a 0a20 2020 2020   runtime...     
+00002300: 696e 7465 7261 6374 6976 650a 0a20 2020  interactive..   
+00002310: 2020 7275 6e0a 2020 2020 2020 2052 756e    run.       Run
+00002320: 2061 2070 7974 686f 6e20 7072 6f63 6573   a python proces
+00002330: 7320 696e 7369 6465 2074 6865 2073 616e  s inside the san
+00002340: 6462 6f78 2e0a 0a20 2020 2020 7368 656c  dbox...     shel
+00002350: 6c0a 2020 2020 2020 2041 6c74 6572 6e61  l.       Alterna
+00002360: 7469 7665 2073 796e 7461 7820 666f 7220  tive syntax for 
+00002370: 7365 6369 6d70 6f72 7420 2274 7261 6365  secimport "trace
+00002380: 222e 0a0a 2020 2020 2074 7261 6365 0a20  "...     trace. 
+00002390: 2020 2020 2020 5472 6163 6573 2061 2070        Traces a p
+000023a0: 7974 686f 6e20 7072 6f63 6573 7320 7573  ython process us
+000023b0: 696e 6720 616e 2065 6e74 7279 706f 696e  ing an entrypoin
+000023c0: 7420 6f72 2069 6e74 6572 6163 7469 7665  t or interactive
+000023d0: 2069 6e74 6572 7072 6574 6572 2e20 4974   interpreter. It
+000023e0: 206d 6967 6874 2072 6571 7569 7265 2073   might require s
+000023f0: 7564 6f20 7072 6976 696c 6c65 6765 7320  udo privilleges 
+00002400: 6f6e 2073 6f6d 6520 686f 7374 732e 0a0a  on some hosts...
+00002410: 2020 2020 2074 7261 6365 5f70 6964 0a20       trace_pid. 
+00002420: 2020 2020 2020 5472 6163 6573 2061 2072        Traces a r
+00002430: 756e 6e69 6e67 2070 726f 6365 7373 2062  unning process b
+00002440: 7920 7069 642e 2049 7420 6d69 6768 7420  y pid. It might 
+00002450: 7265 7175 6972 6520 7375 646f 2070 7269  require sudo pri
+00002460: 7669 6c6c 6567 6573 206f 6e20 736f 6d65  villeges on some
+00002470: 2068 6f73 7473 2e0a 6060 600a 0a23 2320   hosts..```..## 
+00002480: 5374 6f70 206f 6e20 7669 6f6c 6174 696f  Stop on violatio
+00002490: 6e0a 6060 600a 726f 6f74 4031 6263 3035  n.```.root@1bc05
+000024a0: 3331 6439 3164 303a 2f77 6f72 6b73 7061  31d91d0:/workspa
+000024b0: 6365 2320 7365 6369 6d70 6f72 7420 7275  ce# secimport ru
+000024c0: 6e20 202d 2d73 746f 705f 6f6e 5f76 696f  n  --stop_on_vio
+000024d0: 6c61 7469 6f6e 3d74 7275 650a 203e 3e3e  lation=true. >>>
+000024e0: 2073 6563 696d 706f 7274 2072 756e 0a5b   secimport run.[
+000024f0: 5741 524e 494e 475d 3a20 5468 6973 2073  WARNING]: This s
+00002500: 616e 6462 6f78 2077 696c 6c20 7365 6e64  andbox will send
+00002510: 2053 4947 5354 4f50 2074 6f20 7468 6520   SIGSTOP to the 
+00002520: 7072 6f67 7261 6d20 7570 6f6e 2076 696f  program upon vio
+00002530: 6c61 7469 6f6e 2e0a 2052 554e 4e49 4e47  lation.. RUNNING
+00002540: 2053 414e 4442 4f58 2e2e 2e20 5b27 2e2f   SANDBOX... ['./
+00002550: 7361 6e64 626f 782e 6274 272c 2027 2d2d  sandbox.bt', '--
+00002560: 756e 7361 6665 272c 2027 202d 6320 272c  unsafe', ' -c ',
+00002570: 2027 2f77 6f72 6b73 7061 6365 2f50 7974   '/workspace/Pyt
+00002580: 686f 6e2d 332e 3130 2e30 2f70 7974 686f  hon-3.10.0/pytho
+00002590: 6e27 2c20 2753 544f 5027 5d0a 4174 7461  n', 'STOP'].Atta
+000025a0: 6368 696e 6720 3420 7072 6f62 6573 2e2e  ching 4 probes..
+000025b0: 2e0a 5079 7468 6f6e 2033 2e31 302e 3020  ..Python 3.10.0 
+000025c0: 2864 6566 6175 6c74 2c20 4170 7220 3238  (default, Apr 28
+000025d0: 2032 3032 332c 2031 313a 3332 3a34 3029   2023, 11:32:40)
+000025e0: 205b 4743 4320 392e 342e 305d 206f 6e20   [GCC 9.4.0] on 
+000025f0: 6c69 6e75 780a 5479 7065 2022 6865 6c70  linux.Type "help
+00002600: 222c 2022 636f 7079 7269 6768 7422 2c20  ", "copyright", 
+00002610: 2263 7265 6469 7473 2220 6f72 2022 6c69  "credits" or "li
+00002620: 6365 6e73 6522 2066 6f72 206d 6f72 6520  cense" for more 
+00002630: 696e 666f 726d 6174 696f 6e2e 0a3e 3e3e  information..>>>
+00002640: 2069 6d70 6f72 7420 6f73 0a3e 3e3e 206f   import os.>>> o
+00002650: 732e 7379 7374 656d 2827 7073 2729 0a5b  s.system('ps').[
+00002660: 5345 4355 5249 5459 2050 524f 4649 4c45  SECURITY PROFILE
+00002670: 2056 494f 4c41 5445 445d 3a20 3c73 7464   VIOLATED]: <std
+00002680: 696e 3e20 6361 6c6c 6564 2073 7973 6361  in> called sysca
+00002690: 6c6c 2035 3620 6174 2064 6570 7468 2038  ll 56 at depth 8
+000026a0: 3032 320a 0a5e 5e5e 2053 544f 5050 494e  022..^^^ STOPPIN
+000026b0: 4720 5052 4f43 4553 5320 3835 3931 3820  G PROCESS 85918 
+000026c0: 4455 4520 544f 2053 5953 4341 4c4c 2056  DUE TO SYSCALL V
+000026d0: 494f 4c41 5449 4f4e 205e 5e5e 0a09 0950  IOLATION ^^^...P
+000026e0: 524f 4345 5353 2038 3539 3138 2053 544f  ROCESS 85918 STO
+000026f0: 5050 4544 2e0a 6060 600a 0a23 2320 4b69  PPED..```..## Ki
+00002700: 6c6c 206f 6e20 7669 6f6c 6174 696f 6e0a  ll on violation.
+00002710: 6060 600a 726f 6f74 4065 6534 6263 3939  ```.root@ee4bc99
+00002720: 6262 3031 313a 2f77 6f72 6b73 7061 6365  bb011:/workspace
+00002730: 2320 7365 6369 6d70 6f72 7420 7275 6e20  # secimport run 
+00002740: 2d2d 6b69 6c6c 5f6f 6e5f 7669 6f6c 6174  --kill_on_violat
+00002750: 696f 6e0a 203e 3e3e 2073 6563 696d 706f  ion. >>> secimpo
+00002760: 7274 2072 756e 0a5b 5741 524e 494e 475d  rt run.[WARNING]
+00002770: 3a20 5468 6973 2073 616e 6462 6f78 2077  : This sandbox w
+00002780: 696c 6c20 7365 6e64 2053 4947 4b49 4c4c  ill send SIGKILL
+00002790: 2074 6f20 7468 6520 7072 6f67 7261 6d20   to the program 
+000027a0: 7570 6f6e 2076 696f 6c61 7469 6f6e 2e0a  upon violation..
+000027b0: 2052 554e 4e49 4e47 2053 414e 4442 4f58   RUNNING SANDBOX
+000027c0: 2e2e 2e20 5b27 2e2f 7361 6e64 626f 782e  ... ['./sandbox.
+000027d0: 6274 272c 2027 2d2d 756e 7361 6665 272c  bt', '--unsafe',
+000027e0: 2027 202d 6320 272c 2027 2f77 6f72 6b73   ' -c ', '/works
+000027f0: 7061 6365 2f50 7974 686f 6e2d 332e 3130  pace/Python-3.10
+00002800: 2e30 2f70 7974 686f 6e27 2c20 274b 494c  .0/python', 'KIL
+00002810: 4c27 5d0a 696d 706f 7274 206f 730a 6f41  L'].import os.oA
+00002820: 7474 6163 6869 6e67 2034 2070 726f 6265  ttaching 4 probe
+00002830: 732e 2e2e 0a73 5079 7468 6f6e 2033 2e31  s....sPython 3.1
+00002840: 302e 3020 2864 6566 6175 6c74 2c20 4170  0.0 (default, Ap
+00002850: 7220 3238 2032 3032 332c 2031 313a 3332  r 28 2023, 11:32
+00002860: 3a34 3029 205b 4743 4320 392e 342e 305d  :40) [GCC 9.4.0]
+00002870: 206f 6e20 6c69 6e75 780a 5479 7065 2022   on linux.Type "
+00002880: 6865 6c70 222c 2022 636f 7079 7269 6768  help", "copyrigh
+00002890: 7422 2c20 2263 7265 6469 7473 2220 6f72  t", "credits" or
+000028a0: 2022 6c69 6365 6e73 6522 2066 6f72 206d   "license" for m
+000028b0: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
+000028c0: 0a3e 3e3e 2069 6d70 6f72 7420 6f73 0a3e  .>>> import os.>
+000028d0: 3e3e 206f 732e 7379 7374 656d 2827 7073  >> os.system('ps
+000028e0: 2729 0a5b 5345 4355 5249 5459 2050 524f  ').[SECURITY PRO
+000028f0: 4649 4c45 2056 494f 4c41 5445 445d 3a20  FILE VIOLATED]: 
+00002900: 3c73 7464 696e 3e20 6361 6c6c 6564 2073  <stdin> called s
+00002910: 7973 6361 6c6c 2035 3620 6174 2064 6570  yscall 56 at dep
+00002920: 7468 2038 3032 320a 0a5e 5e5e 204b 494c  th 8022..^^^ KIL
+00002930: 4c49 4e47 2050 524f 4345 5353 2038 3634  LING PROCESS 864
+00002940: 3636 2044 5545 2054 4f20 5359 5343 414c  66 DUE TO SYSCAL
+00002950: 4c20 5649 4f4c 4154 494f 4e20 5e5e 5e0a  L VIOLATION ^^^.
+00002960: 0909 4b49 4c4c 4544 2e0a 2053 414e 4442  ..KILLED.. SANDB
+00002970: 4f58 2045 5849 5445 443b 0a60 6060 0a0a  OX EXITED;.```..
+00002980: 2323 2044 796e 616d 6963 2070 726f 6669  ## Dynamic profi
+00002990: 6c69 6e67 202d 2074 7261 6365 2c20 6275  ling - trace, bu
+000029a0: 696c 6420 7361 6e64 626f 782c 2072 756e  ild sandbox, run
+000029b0: 2e0a 6060 6073 6865 6c6c 0a72 6f6f 7440  ..```shell.root@
+000029c0: 3166 6133 6436 6630 3939 3839 3a2f 776f  1fa3d6f09989:/wo
+000029d0: 726b 7370 6163 6523 2073 6563 696d 706f  rkspace# secimpo
+000029e0: 7274 2069 6e74 6572 6163 7469 7665 0a0a  rt interactive..
+000029f0: 4c65 7427 7320 6372 6561 7465 206f 7572  Let's create our
+00002a00: 2066 6972 7374 2074 6169 6c6f 722d 6d61   first tailor-ma
+00002a10: 6465 2073 616e 6462 6f78 2077 6974 6820  de sandbox with 
+00002a20: 7365 6369 6d70 6f72 7421 0a2d 2041 2070  secimport!.- A p
+00002a30: 7974 686f 6e20 7368 656c 6c20 7769 6c6c  ython shell will
+00002a40: 2062 6520 6f70 656e 6564 0a2d 2054 6865   be opened.- The
+00002a50: 2062 6568 6176 696f 7220 7769 6c6c 2062   behavior will b
+00002a60: 6520 7265 636f 7264 6564 2e0a 0a4f 4b3f  e recorded...OK?
+00002a70: 2028 7929 3a20 790a 203e 3e3e 2073 6563   (y): y. >>> sec
+00002a80: 696d 706f 7274 2074 7261 6365 0a0a 5452  import trace..TR
+00002a90: 4143 494e 473a 205b 272f 776f 726b 7370  ACING: ['/worksp
+00002aa0: 6163 652f 7365 6369 6d70 6f72 742f 7072  ace/secimport/pr
+00002ab0: 6f66 696c 6573 2f74 7261 6365 2e62 7427  ofiles/trace.bt'
+00002ac0: 2c20 272d 6327 2c20 272f 776f 726b 7370  , '-c', '/worksp
+00002ad0: 6163 652f 5079 7468 6f6e 2d33 2e31 302e  ace/Python-3.10.
+00002ae0: 302f 7079 7468 6f6e 272c 2027 2d6f 272c  0/python', '-o',
+00002af0: 2027 7472 6163 652e 6c6f 6727 5d0a 0a20   'trace.log'].. 
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 2050 7265 7373 2043 5452         Press CTR
+00002b20: 4c2b 4420 746f 2073 746f 7020 7468 6520  L+D to stop the 
+00002b30: 7472 6163 653b 0a0a 5079 7468 6f6e 2033  trace;..Python 3
+00002b40: 2e31 302e 3020 2864 6566 6175 6c74 2c20  .10.0 (default, 
+00002b50: 4d61 7220 3139 2032 3032 332c 2030 383a  Mar 19 2023, 08:
+00002b60: 3334 3a34 3629 205b 4743 4320 392e 342e  34:46) [GCC 9.4.
+00002b70: 305d 206f 6e20 6c69 6e75 780a 5479 7065  0] on linux.Type
+00002b80: 2022 6865 6c70 222c 2022 636f 7079 7269   "help", "copyri
+00002b90: 6768 7422 2c20 2263 7265 6469 7473 2220  ght", "credits" 
+00002ba0: 6f72 2022 6c69 6365 6e73 6522 2066 6f72  or "license" for
+00002bb0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00002bc0: 6e2e 0a3e 3e3e 2069 6d70 6f72 7420 7468  n..>>> import th
+00002bd0: 6973 0a3e 3e3e 0a20 5452 4143 494e 4720  is.>>>. TRACING 
+00002be0: 444f 4e45 3b0a 203e 3e3e 2073 6563 696d  DONE;. >>> secim
+00002bf0: 706f 7274 2062 7569 6c64 0a0a 5345 4349  port build..SECI
+00002c00: 4d50 4f52 5420 434f 4d50 494c 494e 472e  MPORT COMPILING.
+00002c10: 2e2e 0a0a 4352 4541 5445 4420 4a53 4f4e  ....CREATED JSON
+00002c20: 2054 454d 504c 4154 453a 2020 706f 6c69   TEMPLATE:  poli
+00002c30: 6379 2e6a 736f 6e0a 4352 4541 5445 4420  cy.json.CREATED 
+00002c40: 5941 4d4c 2054 454d 504c 4154 453a 2020  YAML TEMPLATE:  
+00002c50: 706f 6c69 6379 2e79 616d 6c0a 636f 6d70  policy.yaml.comp
+00002c60: 696c 696e 6720 7465 6d70 6c61 7465 2070  iling template p
+00002c70: 6f6c 6963 792e 7961 6d6c 0a44 5452 4143  olicy.yaml.DTRAC
+00002c80: 4520 5341 4e44 424f 583a 2020 7361 6e64  E SANDBOX:  sand
+00002c90: 626f 782e 640a 4250 4654 5243 4520 5341  box.d.BPFTRCE SA
+00002ca0: 4e44 424f 583a 2020 7361 6e64 626f 782e  NDBOX:  sandbox.
+00002cb0: 6274 0a60 6060 0a0a 4e6f 772c 206c 6574  bt.```..Now, let
+00002cc0: 2773 2072 756e 2074 6865 2073 616e 6462  's run the sandb
+00002cd0: 6f78 210a 6060 6070 7974 686f 6e0a 2d20  ox!.```python.- 
+00002ce0: 5275 6e20 7468 6520 7361 6d65 2063 6f6d  Run the same com
+00002cf0: 6d61 6e64 7320 6173 2062 6566 6f72 652c  mands as before,
+00002d00: 2074 6865 7920 7368 6f75 6c64 2072 756e   they should run
+00002d10: 2077 6974 686f 7574 2061 6e79 2070 726f   without any pro
+00002d20: 626c 656d 3b2e 0a2d 2044 6f20 736f 6d65  blem;..- Do some
+00002d30: 7468 696e 6720 6e65 7720 696e 2074 6865  thing new in the
+00002d40: 2073 6865 6c6c 3b20 652e 673a 2020 203e   shell; e.g:   >
+00002d50: 3e3e 205f 5f69 6d70 6f72 745f 5f28 226f  >> __import__("o
+00002d60: 7322 292e 7379 7374 656d 2822 7073 2229  s").system("ps")
+00002d70: 0a0a 2020 2020 2020 2020 4f4b 3f20 2879  ..        OK? (y
+00002d80: 293a 2079 0a20 3e3e 3e20 7365 6369 6d70  ): y. >>> secimp
+00002d90: 6f72 7420 7275 6e0a 2052 554e 4e49 4e47  ort run. RUNNING
+00002da0: 2053 414e 4442 4f58 2e2e 2e20 5b27 2e2f   SANDBOX... ['./
+00002db0: 7361 6e64 626f 782e 6274 272c 2027 2d2d  sandbox.bt', '--
+00002dc0: 756e 7361 6665 272c 2027 202d 6320 272c  unsafe', ' -c ',
+00002dd0: 2027 2f77 6f72 6b73 7061 6365 2f50 7974   '/workspace/Pyt
+00002de0: 686f 6e2d 332e 3130 2e30 2f70 7974 686f  hon-3.10.0/pytho
+00002df0: 6e27 5d0a 4174 7461 6368 696e 6720 3520  n'].Attaching 5 
+00002e00: 7072 6f62 6573 2e2e 2e0a 5245 4749 5354  probes....REGIST
+00002e10: 4552 494e 4720 5359 5343 414c 4c53 2e2e  ERING SYSCALLS..
+00002e20: 2e0a 5354 4152 5445 440a 5079 7468 6f6e  ..STARTED.Python
+00002e30: 2033 2e31 302e 3020 2864 6566 6175 6c74   3.10.0 (default
+00002e40: 2c20 4d61 7220 3139 2032 3032 332c 2030  , Mar 19 2023, 0
+00002e50: 383a 3334 3a34 3629 205b 4743 4320 392e  8:34:46) [GCC 9.
+00002e60: 342e 305d 206f 6e20 6c69 6e75 780a 5479  4.0] on linux.Ty
+00002e70: 7065 2022 6865 6c70 222c 2022 636f 7079  pe "help", "copy
+00002e80: 7269 6768 7422 2c20 2263 7265 6469 7473  right", "credits
+00002e90: 2220 6f72 2022 6c69 6365 6e73 6522 2066  " or "license" f
+00002ea0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00002eb0: 696f 6e2e 0a3e 3e3e 2069 6d70 6f72 7420  ion..>>> import 
+00002ec0: 7468 6973 0a3e 3e3e 2069 6d70 6f72 7420  this.>>> import 
+00002ed0: 6f73 0a5b 5345 4349 4d50 4f52 5420 5649  os.[SECIMPORT VI
+00002ee0: 4f4c 4154 494f 4e5d 3a20 3c73 7464 696e  OLATION]: <stdin
+00002ef0: 3e20 6361 6c6c 6564 2073 7973 6361 6c6c  > called syscall
+00002f00: 2069 6f63 746c 2061 7420 6465 7074 6820   ioctl at depth 
+00002f10: 300a 5b53 4543 494d 504f 5254 2056 494f  0.[SECIMPORT VIO
+00002f20: 4c41 5449 4f4e 5d3a 203c 7374 6469 6e3e  LATION]: <stdin>
+00002f30: 2063 616c 6c65 6420 7379 7363 616c 6c20   called syscall 
+00002f40: 696f 6374 6c20 6174 2064 6570 7468 2030  ioctl at depth 0
+00002f50: 0a60 6060 0a0a 466f 7220 6d6f 7265 2064  .```..For more d
+00002f60: 6574 6169 6c65 6420 7573 6167 6520 696e  etailed usage in
+00002f70: 7374 7275 6374 696f 6e73 2c20 7365 6520  structions, see 
+00002f80: 7468 6520 5b43 6f6d 6d61 6e64 2d4c 696e  the [Command-Lin
+00002f90: 6520 5573 6167 655d 2868 7474 7073 3a2f  e Usage](https:/
+00002fa0: 2f67 6974 6875 622e 636f 6d2f 6176 696c  /github.com/avil
+00002fb0: 756d 2f73 6563 696d 706f 7274 2f77 696b  um/secimport/wik
+00002fc0: 692f 436f 6d6d 616e 642d 4c69 6e65 2d55  i/Command-Line-U
+00002fd0: 7361 6765 2920 7061 6765 2e0a 0a23 2320  sage) page...## 
+00002fe0: 6e73 6a61 696c 2073 7570 706f 7274 2028  nsjail support (
+00002ff0: 7365 6363 6f6d 7029 0a42 6573 6964 6520  seccomp).Beside 
+00003000: 7468 6520 7361 6e64 626f 7820 7468 6174  the sandbox that
+00003010: 2073 6563 696d 706f 7274 2062 7569 6c64   secimport build
+00003020: 732c 203c 6272 3e0a 5468 6520 6073 6563  s, <br>.The `sec
+00003030: 696d 706f 7274 2062 7569 6c64 6020 636f  import build` co
+00003040: 6d6d 616e 6420 6372 6561 7465 7320 616e  mmand creates an
+00003050: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00003060: 2f2f 6769 7468 7562 2e63 6f6d 2f67 6f6f  //github.com/goo
+00003070: 676c 652f 6e73 6a61 696c 223e 6e73 6a61  gle/nsjail">nsja
+00003080: 696c 3c2f 613e 2073 616e 6462 6f78 2077  il</a> sandbox w
+00003090: 6974 6820 7365 6363 6f6d 7020 7072 6f66  ith seccomp prof
+000030a0: 696c 6520 666f 7220 796f 7572 2074 7261  ile for your tra
+000030b0: 6365 6420 636f 6465 2e3c 6272 3e20 606e  ced code.<br> `n
+000030c0: 736a 6169 6c60 2065 6e61 626c 6573 206e  sjail` enables n
+000030d0: 616d 6573 7061 6365 2073 616e 6462 6f78  amespace sandbox
+000030e0: 696e 6720 7769 7468 2073 6563 636f 6d70  ing with seccomp
+000030f0: 206f 6e20 6c69 6e75 783c 6272 3e0a 6073   on linux<br>.`s
+00003100: 6563 696d 706f 7274 6020 6175 746f 6d61  ecimport` automa
+00003110: 7469 6361 6c6c 7920 6765 6e65 7261 7465  tically generate
+00003120: 7320 7365 6363 6f6d 7020 7072 6f66 696c  s seccomp profil
+00003130: 6573 2074 6f20 7573 6520 7769 7468 2060  es to use with `
+00003140: 6e73 6a61 696c 6020 6173 2065 7865 6375  nsjail` as execu
+00003150: 7461 626c 6520 6261 7368 2073 6372 6970  table bash scrip
+00003160: 742e 0a49 7420 6361 6e20 6265 2075 7365  t..It can be use
+00003170: 6420 746f 206c 696d 6974 2074 6865 2073  d to limit the s
+00003180: 7973 6361 6c6c 7320 6f66 2074 6865 2065  yscalls of the e
+00003190: 6e74 6972 6520 7079 7468 6f6e 2070 726f  ntire python pro
+000031a0: 6365 7373 2c20 6173 2061 6e6f 7468 6572  cess, as another
+000031b0: 206c 6179 6572 206f 6620 6465 6665 6e63   layer of defenc
+000031c0: 652e 0a0a 2323 2050 7974 686f 6e20 4150  e...## Python AP
+000031d0: 490a 0a49 6e73 7465 6164 206f 6620 434c  I..Instead of CL
+000031e0: 492c 2079 6f75 2063 616e 2061 6c73 6f20  I, you can also 
+000031f0: 7573 6520 6073 6563 696d 706f 7274 6020  use `secimport` 
+00003200: 6279 2072 6570 6c61 6369 6e67 2022 6069  by replacing "`i
+00003210: 6d70 6f72 7460 2220 7769 7468 2022 6073  mport`" with "`s
+00003220: 6563 696d 706f 7274 2e73 6563 7572 655f  ecimport.secure_
+00003230: 696d 706f 7274 6022 2066 6f72 2073 656c  import`" for sel
+00003240: 6563 7465 6420 6d6f 6475 6c65 732e 2053  ected modules. S
+00003250: 6565 2074 6865 205b 5079 7468 6f6e 2049  ee the [Python I
+00003260: 6d70 6f72 7473 5d28 6578 616d 706c 6573  mports](examples
+00003270: 2f70 7974 686f 6e5f 696d 706f 7274 732f  /python_imports/
+00003280: 2920 6578 616d 706c 6520 666f 7220 6d6f  ) example for mo
+00003290: 7265 2064 6574 6169 6c73 2e0a 0a23 2320  re details...## 
+000032a0: 446f 636b 6572 0a54 6865 2071 7569 636b  Docker.The quick
+000032b0: 6573 7420 7761 7920 746f 2065 7661 6c75  est way to evalu
+000032c0: 6174 6520 6073 6563 696d 706f 7274 6020  ate `secimport` 
+000032d0: 6973 2074 6f20 7573 6520 6f75 7220 5b44  is to use our [D
+000032e0: 6f63 6b65 7220 636f 6e74 6169 6e65 725d  ocker container]
+000032f0: 2864 6f63 6b65 722f 5245 4144 4d45 2e6d  (docker/README.m
+00003300: 6429 2c20 7768 6963 6820 696e 636c 7564  d), which includ
+00003310: 6573 2060 6270 6674 7261 6365 6020 2860  es `bpftrace` (`
+00003320: 6562 7066 6029 2061 6e64 206f 7468 6572  ebpf`) and other
+00003330: 2070 6c75 672d 616e 642d 706c 6179 2065   plug-and-play e
+00003340: 7861 6d70 6c65 732e 0a0a 0a23 2320 4578  xamples....## Ex
+00003350: 616d 706c 6573 0a0a 5468 6520 5b53 616e  amples..The [San
+00003360: 6462 6f78 2045 7861 6d70 6c65 735d 2868  dbox Examples](h
+00003370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003380: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
+00003390: 7274 2f77 696b 692f 5361 6e64 626f 782d  rt/wiki/Sandbox-
+000033a0: 4578 616d 706c 6573 2920 7061 6765 2063  Examples) page c
+000033b0: 6f6e 7461 696e 7320 6261 7369 6320 616e  ontains basic an
+000033c0: 6420 6164 7661 6e63 6564 2072 6561 6c2d  d advanced real-
+000033d0: 776f 726c 6420 6578 616d 706c 6573 2e0a  world examples..
+000033e0: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+000033f0: 0a0a 466f 7220 696e 666f 726d 6174 696f  ..For informatio
+00003400: 6e20 6f6e 2068 6f77 2074 6f20 636f 6e74  n on how to cont
+00003410: 7269 6275 7465 2074 6f20 6073 6563 696d  ribute to `secim
+00003420: 706f 7274 602c 2073 6565 2074 6865 205b  port`, see the [
+00003430: 436f 6e74 7269 6275 7469 6e67 5d28 6874  Contributing](ht
+00003440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003450: 2f61 7669 6c75 6d2f 7365 6369 6d70 6f72  /avilum/secimpor
+00003460: 742f 626c 6f62 2f6d 6173 7465 722f 646f  t/blob/master/do
+00003470: 6373 2f43 4f4e 5452 4942 5554 494e 472e  cs/CONTRIBUTING.
+00003480: 6d64 2920 6775 6964 652e 0a0a 2323 2052  md) guide...## R
+00003490: 6f61 646d 6170 0a0a 5365 6520 7468 6520  oadmap..See the 
+000034a0: 5b52 6f61 646d 6170 5d28 6874 7470 733a  [Roadmap](https:
+000034b0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
+000034c0: 6c75 6d2f 7365 6369 6d70 6f72 742f 626c  lum/secimport/bl
+000034d0: 6f62 2f6d 6173 7465 722f 646f 6373 2f52  ob/master/docs/R
+000034e0: 4f41 444d 4150 2e6d 6429 2066 6f72 2074  OADMAP.md) for t
+000034f0: 6865 2070 6c61 6e6e 6564 2066 6561 7475  he planned featu
+00003500: 7265 7320 616e 6420 6465 7665 6c6f 706d  res and developm
+00003510: 656e 7420 6d69 6c65 7374 6f6e 6573 2e0a  ent milestones..
+00003520: 0a23 2320 4368 616e 6765 6c6f 670a 0a53  .## Changelog..S
+00003530: 6565 2074 6865 205b 4368 616e 6765 6c6f  ee the [Changelo
+00003540: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00003550: 622e 636f 6d2f 6176 696c 756d 2f73 6563  b.com/avilum/sec
+00003560: 696d 706f 7274 2f62 6c6f 622f 6d61 7374  import/blob/mast
+00003570: 6572 2f64 6f63 732f 4348 414e 4745 4c4f  er/docs/CHANGELO
+00003580: 472e 6d64 2920 666f 7220 6465 7665 6c6f  G.md) for develo
+00003590: 706d 656e 7420 7072 6f67 7265 7373 2061  pment progress a
+000035a0: 6e64 2065 7869 7374 696e 6720 6665 6174  nd existing feat
+000035b0: 7572 6573 2e0a                           ures..
```

### Comparing `secimport-0.9.1/pyproject.toml` & `secimport-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secimport"
-version = "0.9.1"
+version = "0.9.2"
 description = "A sandbox/supervisor for python modules."
 authors = ["Avi Lumelsky"]
 license = "MIT"
 homepage = "https://github.com/avilum/secimport"
 readme = "README.md"
 packages = [
     { include = "secimport" },
```

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.9.2/secimport/backends/bpftrace_backend/bpftrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.9.2/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.9.2/secimport/backends/bpftrace_backend/default.yaml.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.9.2/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.9.2/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/bpftrace_backend/new_template.bt` & `secimport-0.9.2/secimport/backends/bpftrace_backend/new_template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/common/system_calls.py` & `secimport-0.9.2/secimport/backends/common/system_calls.py`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/common/utils.py` & `secimport-0.9.2/secimport/backends/common/utils.py`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/default.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/dtrace_backend.py` & `secimport-0.9.2/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.9.2/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/secimport/cli.py` & `secimport-0.9.2/secimport/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 from pathlib import Path
 import stat
 import fire
 import sys
 import yaml
+import subprocess
 import secimport
 from secimport.backends.common.utils import SECIMPORT_ROOT
 
 
 class COLORS:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
@@ -199,25 +200,30 @@
     ):
         """Traces a python process using an entrypoint or interactive interpreter. It might require sudo privilleges on some hosts.
         Args:
             entrypoint (str, optional): A python script path to trace. If not specified, a python interactive shell will be opened in the foregraound. This shell, or the given command, will be traced and logged to the "trace_log_file" argument.
             python_interpreter (str, optional): The path of the python executable interpreter to trace. Defaults to sys.executable.
             trace_log_file (str, optional): The log file to write the trace into. Defaults to "trace.log".
         """
+        with_dtrace = subprocess.check_output([python_interpreter, '-c', 'import sysconfig; print(sysconfig.get_config_var("WITH_DTRACE"))'], encoding='utf-8')
+        if with_dtrace.strip() != "1":
+            colored_print(COLORS.FAIL, f"\nIt seems that {python_interpreter} was compiled without --with-dtrace=1. secimport will probably not work properly!\n")
+
         if entrypoint:
             # entrypoint_cmd = str(Path(entrypoint).absolute())
             entrypoint_cmd = f'bash -c "{python_interpreter} {entrypoint}"'
         else:
             entrypoint_cmd = python_interpreter
         cmd = [
             f"{SECIMPORT_ROOT}/profiles/trace.bt",
             "-c",
             f"{entrypoint_cmd}",
             "-o",
             f"{trace_log_file}",
+            f"{python_interpreter}",
         ]
         colored_print(COLORS.HEADER, "\nTracing using ", cmd)
         colored_print(
             COLORS.BOLD,
             "Press CTRL+D or CTRL+C to stop the trace gracefully.\n",
         )
         os.system(" ".join(cmd))
@@ -233,20 +239,24 @@
         """Traces a running process by pid. It might require sudo privilleges on some hosts.
 
         Args:
             pid (int): process pid to trace
             trace_log_file (str): The output file to write the trace into.
         """
         assert isinstance(pid, int), f"pid must be an int, got: {pid}"
+
+        python_interpreter = (Path('/proc') / str(pid) / 'exe').resolve()
+
         cmd = [
             str(SECIMPORT_ROOT) + "/profiles/trace.bt",
             "-p",
             f"{pid}",
             "-o",
             f"{trace_log_file}",
+            f"{python_interpreter}"
         ]
         colored_print(COLORS.HEADER, "\nTRACING PID:")
         colored_print(COLORS.OKBLUE, pid)
         input("\t\t\tPress CTRL+D/CTRL+C to stop the trace;")
         os.system(" ".join(cmd))
         colored_print(COLORS.ENDC)
```

### Comparing `secimport-0.9.1/secimport/profiles/trace.bt` & `secimport-0.9.2/secimport/profiles/trace.bt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env bpftrace
 
 // A profiling script that logs all the syscalls, per python module.
 // It can be attached to a running process using -p or can be used to trace a python shell interactively.
 //
 // Usage:
-// ./trace.bt -c Python-3.10.0/python
+// ./trace.bt Python-3.10.0/python -c Python-3.10.0/python
 
 BEGIN {
     // Mapping all syscalls both ways, based on https://github.com/iovisor/bpftrace/blob/2c7a7a598dbe1aa790db2dfe2db242aa69137d5b/tools/syscount.bt
     // Generates using bash:
     //   $ apt-get install auditd
     //   $ ausyscall --dump | awk 'NR > 1 { printf("\t@sysname[%d] = \"%s\";\n", $1, $2); }';
     printf("REGISTERING SYSCALLS...\n");
@@ -684,25 +684,25 @@
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
     printf("Tracing Modules - Exit gracefully with Ctrl+D\n")
 }
 
-usdt:/workspace/Python-3.10.0/python:function__entry {
+usdt:$1:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
         @globals["current_module"] = str(arg0);
 
         // To trace python calls in the console, uncomment:
         // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]) ;
 }
 
-usdt:/workspace/Python-3.10.0/python:function__return {
+usdt:$1:function__return {
         @["depth"]--;
 }
 
 tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
     // @modules_syscalls[@globals["current_module"], @sysname[args->id], @["depth"]] = count();
     @modules_syscalls[@globals["current_module"], @sysname[args->id]] = count();
     @syscalls[@sysname[args->id]] = count();
```

### Comparing `secimport-0.9.1/secimport/sandbox_helper.py` & `secimport-0.9.2/secimport/sandbox_helper.py`

 * *Files identical despite different names*

### Comparing `secimport-0.9.1/PKG-INFO` & `secimport-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7365 6369  : 2.1.Name: seci
 00000020: 6d70 6f72 740a 5665 7273 696f 6e3a 2030  mport.Version: 0
-00000030: 2e39 2e31 0a53 756d 6d61 7279 3a20 4120  .9.1.Summary: A 
+00000030: 2e39 2e32 0a53 756d 6d61 7279 3a20 4120  .9.2.Summary: A 
 00000040: 7361 6e64 626f 782f 7375 7065 7276 6973  sandbox/supervis
 00000050: 6f72 2066 6f72 2070 7974 686f 6e20 6d6f  or for python mo
 00000060: 6475 6c65 732e 0a48 6f6d 652d 7061 6765  dules..Home-page
 00000070: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000080: 2e63 6f6d 2f61 7669 6c75 6d2f 7365 6369  .com/avilum/seci
 00000090: 6d70 6f72 740a 4c69 6365 6e73 653a 204d  mport.License: M
 000000a0: 4954 0a41 7574 686f 723a 2041 7669 204c  IT.Author: Avi L
@@ -32,840 +32,877 @@
 000001f0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
 00000200: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 00000210: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000220: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
 00000230: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
 00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000260: 332e 3131 0a52 6571 7569 7265 732d 4469  3.11.Requires-Di
-00000270: 7374 3a20 5079 5941 4d4c 2028 3e3d 362e  st: PyYAML (>=6.
-00000280: 302c 3c37 2e30 290a 5265 7175 6972 6573  0,<7.0).Requires
-00000290: 2d44 6973 743a 2066 6972 6520 283e 3d30  -Dist: fire (>=0
-000002a0: 2e34 2c3c 302e 3629 0a44 6573 6372 6970  .4,<0.6).Descrip
-000002b0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000002c0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000002d0: 0a0a 3c21 2d2d 2053 5441 5254 2064 6f63  ..<!-- START doc
-000002e0: 746f 6320 6765 6e65 7261 7465 6420 544f  toc generated TO
-000002f0: 4320 706c 6561 7365 206b 6565 7020 636f  C please keep co
-00000300: 6d6d 656e 7420 6865 7265 2074 6f20 616c  mment here to al
-00000310: 6c6f 7720 6175 746f 2075 7064 6174 6520  low auto update 
-00000320: 2d2d 3e0a 3c21 2d2d 2044 4f4e 2754 2045  -->.<!-- DON'T E
-00000330: 4449 5420 5448 4953 2053 4543 5449 4f4e  DIT THIS SECTION
-00000340: 2c20 494e 5354 4541 4420 5245 2d52 554e  , INSTEAD RE-RUN
-00000350: 2064 6f63 746f 6320 544f 2055 5044 4154   doctoc TO UPDAT
-00000360: 4520 2d2d 3e0a 2a2a 5461 626c 6520 6f66  E -->.**Table of
-00000370: 2043 6f6e 7465 6e74 732a 2a20 202a 6765   Contents**  *ge
-00000380: 6e65 7261 7465 6420 7769 7468 205b 446f  nerated with [Do
-00000390: 6354 6f63 5d28 6874 7470 733a 2f2f 6769  cToc](https://gi
-000003a0: 7468 7562 2e63 6f6d 2f74 686c 6f72 656e  thub.com/thloren
-000003b0: 7a2f 646f 6374 6f63 292a 0a0a 2d20 5b73  z/doctoc)*..- [s
-000003c0: 6563 696d 706f 7274 5d28 2373 6563 696d  ecimport](#secim
-000003d0: 706f 7274 290a 2020 2d20 5b54 6865 2054  port).  - [The T
-000003e0: 6169 6c6f 722d 4d61 6465 2053 616e 6462  ailor-Made Sandb
-000003f0: 6f78 2066 6f72 2059 6f75 7220 4170 706c  ox for Your Appl
-00000400: 6963 6174 696f 6e5d 2823 7468 652d 7461  ication](#the-ta
-00000410: 696c 6f72 2d6d 6164 652d 7361 6e64 626f  ilor-made-sandbo
-00000420: 782d 666f 722d 796f 7572 2d61 7070 6c69  x-for-your-appli
-00000430: 6361 7469 6f6e 290a 2020 2020 2d20 5b54  cation).    - [T
-00000440: 6865 2070 726f 626c 656d 5d28 2374 6865  he problem](#the
-00000450: 2d70 726f 626c 656d 290a 2020 2020 2d20  -problem).    - 
-00000460: 5b54 6865 2073 6f6c 7574 696f 6e5d 2823  [The solution](#
-00000470: 7468 652d 736f 6c75 7469 6f6e 290a 2020  the-solution).  
-00000480: 2d20 5b49 6e73 7461 6c6c 6174 696f 6e5d  - [Installation]
-00000490: 2823 696e 7374 616c 6c61 7469 6f6e 290a  (#installation).
-000004a0: 2020 2d20 5b57 6974 6820 446f 636b 6572    - [With Docker
-000004b0: 5d28 2377 6974 682d 646f 636b 6572 290a  ](#with-docker).
-000004c0: 2020 2d20 5b57 6974 686f 7574 2044 6f63    - [Without Doc
-000004d0: 6b65 725d 2823 7769 7468 6f75 742d 646f  ker](#without-do
-000004e0: 636b 6572 290a 2020 2d20 5b55 7361 6765  cker).  - [Usage
-000004f0: 5d28 2375 7361 6765 290a 2020 2d20 5b53  ](#usage).  - [S
-00000500: 746f 7020 6f6e 2076 696f 6c61 7469 6f6e  top on violation
-00000510: 5d28 2373 746f 702d 6f6e 2d76 696f 6c61  ](#stop-on-viola
-00000520: 7469 6f6e 290a 2020 2d20 5b4b 696c 6c20  tion).  - [Kill 
-00000530: 6f6e 2076 696f 6c61 7469 6f6e 5d28 236b  on violation](#k
-00000540: 696c 6c2d 6f6e 2d76 696f 6c61 7469 6f6e  ill-on-violation
-00000550: 290a 2020 2d20 5b44 796e 616d 6963 2070  ).  - [Dynamic p
-00000560: 726f 6669 6c69 6e67 202d 2074 7261 6365  rofiling - trace
-00000570: 2c20 6275 696c 6420 7361 6e64 626f 782c  , build sandbox,
-00000580: 2072 756e 2e5d 2823 6479 6e61 6d69 632d   run.](#dynamic-
-00000590: 7072 6f66 696c 696e 672d 2d2d 7472 6163  profiling---trac
-000005a0: 652d 6275 696c 642d 7361 6e64 626f 782d  e-build-sandbox-
-000005b0: 7275 6e29 0a20 202d 205b 6e73 6a61 696c  run).  - [nsjail
-000005c0: 2073 7570 706f 7274 2028 7365 6363 6f6d   support (seccom
-000005d0: 7029 5d28 236e 736a 6169 6c2d 7375 7070  p)](#nsjail-supp
-000005e0: 6f72 742d 7365 6363 6f6d 7029 0a20 202d  ort-seccomp).  -
-000005f0: 205b 5079 7468 6f6e 2041 5049 5d28 2370   [Python API](#p
-00000600: 7974 686f 6e2d 6170 6929 0a20 202d 205b  ython-api).  - [
-00000610: 446f 636b 6572 5d28 2364 6f63 6b65 7229  Docker](#docker)
-00000620: 0a20 202d 205b 4578 616d 706c 6573 5d28  .  - [Examples](
-00000630: 2365 7861 6d70 6c65 7329 0a20 202d 205b  #examples).  - [
-00000640: 436f 6e74 7269 6275 7469 6e67 5d28 2363  Contributing](#c
-00000650: 6f6e 7472 6962 7574 696e 6729 0a20 202d  ontributing).  -
-00000660: 205b 526f 6164 6d61 705d 2823 726f 6164   [Roadmap](#road
-00000670: 6d61 7029 0a20 202d 205b 4368 616e 6765  map).  - [Change
-00000680: 6c6f 675d 2823 6368 616e 6765 6c6f 6729  log](#changelog)
-00000690: 0a0a 3c21 2d2d 2045 4e44 2064 6f63 746f  ..<!-- END docto
-000006a0: 6320 6765 6e65 7261 7465 6420 544f 4320  c generated TOC 
-000006b0: 706c 6561 7365 206b 6565 7020 636f 6d6d  please keep comm
-000006c0: 656e 7420 6865 7265 2074 6f20 616c 6c6f  ent here to allo
-000006d0: 7720 6175 746f 2075 7064 6174 6520 2d2d  w auto update --
-000006e0: 3e0a 0a23 2073 6563 696d 706f 7274 0a5b  >..# secimport.[
-000006f0: 215b 5570 6c6f 6164 2050 7974 686f 6e20  ![Upload Python 
-00000700: 5061 636b 6167 655d 2868 7474 7073 3a2f  Package](https:/
-00000710: 2f67 6974 6875 622e 636f 6d2f 6176 696c  /github.com/avil
-00000720: 756d 2f73 6563 696d 706f 7274 2f61 6374  um/secimport/act
-00000730: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00000740: 7974 686f 6e2d 7075 626c 6973 682e 796d  ython-publish.ym
-00000750: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-00000760: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000770: 2f61 7669 6c75 6d2f 7365 6369 6d70 6f72  /avilum/secimpor
-00000780: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
-00000790: 6f77 732f 7079 7468 6f6e 2d70 7562 6c69  ows/python-publi
-000007a0: 7368 2e79 6d6c 290a 215b 5d28 6874 7470  sh.yml).![](http
-000007b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007c0: 696f 2f62 6164 6765 2f54 6573 745f 436f  io/badge/Test_Co
-000007d0: 7665 7261 6765 2d39 3025 2d62 6c75 6529  verage-90%-blue)
-000007e0: 0a0a 0a23 2320 5468 6520 5461 696c 6f72  ...## The Tailor
-000007f0: 2d4d 6164 6520 5361 6e64 626f 7820 666f  -Made Sandbox fo
-00000800: 7220 596f 7572 2041 7070 6c69 6361 7469  r Your Applicati
-00000810: 6f6e 0a73 6563 696d 706f 7274 2069 7320  on.secimport is 
-00000820: 7072 6f64 7563 7469 6f6e 2d6f 7269 656e  production-orien
-00000830: 7465 6420 7361 6e64 626f 7820 746f 6f6c  ted sandbox tool
-00000840: 6b69 742e 3c62 723e 0a49 7420 7472 6163  kit.<br>.It trac
-00000850: 6573 2079 6f75 7220 636f 6465 2c20 616e  es your code, an
-00000860: 6420 7275 6e73 2061 6e20 6578 6563 7574  d runs an execut
-00000870: 6162 6c65 2074 6861 7420 616c 6c6f 7773  able that allows
-00000880: 206f 6e6c 7920 7468 6520 7361 6d65 2073   only the same s
-00000890: 7973 6361 6c6c 732c 2070 6572 206d 6f64  yscalls, per mod
-000008a0: 756c 652e 0a0a 2323 2320 5468 6520 7072  ule...### The pr
-000008b0: 6f62 6c65 6d0a 5472 6164 6974 696f 6e61  oblem.Traditiona
-000008c0: 6c20 746f 6f6c 7320 6c69 6b65 2073 6563  l tools like sec
-000008d0: 636f 6d70 206f 7220 4170 7041 726d 6f72  comp or AppArmor
-000008e0: 2065 6e66 6f72 6365 2073 7973 6361 6c6c   enforce syscall
-000008f0: 7320 666f 7220 7468 6520 656e 7469 7265  s for the entire
-00000900: 2070 726f 6365 7373 2e3c 6272 3e53 6f6d   process.<br>Som
-00000910: 6574 6869 6e67 206c 696b 6520 6061 6c6c  ething like `all
-00000920: 6f77 6564 5f73 7973 6361 6c6c 733d 5b22  owed_syscalls=["
-00000930: 7265 6164 222c 226f 7065 6e61 7422 2c22  read","openat","
-00000940: 6269 6e64 222c 2277 7269 7465 225d 602c  bind","write"]`,
-00000950: 2077 6869 6368 2069 7320 6772 6561 742c   which is great,
-00000960: 2062 7574 206e 6f74 2065 6e6f 7567 6820   but not enough 
-00000970: 666f 7220 7079 7468 6f6e 2773 2061 7474  for python's att
-00000980: 6163 6b20 7375 7266 6163 652e 3c62 723e  ack surface.<br>
-00000990: 0a0a 2323 2320 5468 6520 736f 6c75 7469  ..### The soluti
-000009a0: 6f6e 0a60 7365 6369 6d70 6f72 7460 2069  on.`secimport` i
-000009b0: 7320 6162 6c65 2074 6f20 7472 6163 6520  s able to trace 
-000009c0: 7768 6963 6820 7379 7363 616c 6c73 2065  which syscalls e
-000009d0: 6163 6820 6d6f 6475 6c65 2069 6e20 796f  ach module in yo
-000009e0: 7572 2063 6f64 6520 7573 6573 2028 6279  ur code uses (by
-000009f0: 2070 6163 6b61 6765 206e 616d 6529 2e3c   package name).<
-00000a00: 6272 3e0a 4166 7465 7220 7472 6163 696e  br>.After tracin
-00000a10: 672c 2073 6563 696d 706f 7274 2063 7265  g, secimport cre
-00000a20: 6174 6573 2061 204a 534f 4e2f 5941 4d4c  ates a JSON/YAML
-00000a30: 2070 6f6c 6963 7920 666f 7220 796f 7572   policy for your
-00000a40: 2063 6f64 652e 2049 7420 636f 6d70 696c   code. It compil
-00000a50: 6573 2069 7420 696e 746f 2061 2068 6967  es it into a hig
-00000a60: 682d 7065 7266 6f72 6d61 6e63 6520 6542  h-performance eB
-00000a70: 5046 2069 6e73 7472 756d 656e 7461 7469  PF instrumentati
-00000a80: 6f6e 2073 6372 6970 7420 2873 6d61 6c6c  on script (small
-00000a90: 6572 2074 6865 6e20 3531 3220 6279 7465  er then 512 byte
-00000aa0: 7320 6f76 6572 616c 6c29 2c20 7468 6174  s overall), that
-00000ab0: 206c 6f6f 6b73 206c 696b 6520 3c61 3e74   looks like <a>t
-00000ac0: 6869 733c 2f61 3e2e 0a60 6060 0a6d 6f64  his</a>..```.mod
-00000ad0: 756c 6573 3a0a 2020 7265 7175 6573 7473  ules:.  requests
-00000ae0: 3a0a 2020 2020 6465 7374 7275 6374 6976  :.    destructiv
-00000af0: 653a 2074 7275 6520 2020 2020 2320 7768  e: true     # wh
-00000b00: 656e 2074 7275 652c 2073 6563 696d 706f  en true, secimpo
-00000b10: 7274 2077 696c 6c20 6b69 6c6c 206f 6e20  rt will kill on 
-00000b20: 7669 6c61 7469 6f6e 2069 6e73 7465 6164  vilation instead
-00000b30: 206f 6620 6c6f 6767 696e 672e 0a20 2020   of logging..   
-00000b40: 2073 7973 6361 6c6c 5f61 6c6c 6f77 6c69   syscall_allowli
-00000b50: 7374 3a0a 2020 2020 2020 2d20 6663 686d  st:.      - fchm
-00000b60: 6f64 0a20 2020 2020 202d 2067 6574 656e  od.      - geten
-00000b70: 7472 6f70 790a 2020 2020 2020 2d20 6765  tropy.      - ge
-00000b80: 7470 6772 700a 2020 2020 2020 2d20 6765  tpgrp.      - ge
-00000b90: 7472 6c69 6d69 740a 2e2e 2e0a 6060 600a  trlimit.....```.
-00000ba0: 596f 7520 6361 6e20 616c 736f 2075 7365  You can also use
-00000bb0: 204a 534f 4e20 696e 7374 6165 6164 206f   JSON instaead o
-00000bc0: 6620 5941 4d4c 2c20 616e 6420 6576 656e  f YAML, and even
-00000bd0: 2063 6f6e 6669 6e65 2062 7569 6c74 696e   confine builtin
-00000be0: 2070 7974 686f 6e20 6d6f 6475 6c65 732e   python modules.
-00000bf0: 3c62 723e 0a41 6e20 6578 616d 706c 6520  <br>.An example 
-00000c00: 706f 6c69 6379 2074 6861 7420 7573 6573  policy that uses
-00000c10: 206c 6f67 6769 6e67 2c20 6d75 6c74 6970   logging, multip
-00000c20: 726f 6365 7373 696e 672c 206f 7320 616e  rocessing, os an
-00000c30: 6420 6669 6c65 7379 7374 656d 2077 696c  d filesystem wil
-00000c40: 6c20 6c6f 6f6b 2061 7070 726f 7869 6d61  l look approxima
-00000c50: 7465 6c79 206c 696b 6520 7468 6973 3a0a  tely like this:.
-00000c60: 6060 600a 2e2e 2e0a 2020 2020 222f 776f  ```.....    "/wo
-00000c70: 726b 7370 6163 652f 5079 7468 6f6e 2d33  rkspace/Python-3
-00000c80: 2e31 302e 302f 4c69 622f 6c6f 6767 696e  .10.0/Lib/loggin
-00000c90: 672f 5f5f 696e 6974 5f5f 2e70 7922 3a20  g/__init__.py": 
-00000ca0: 5b0a 2020 2020 2020 2020 2220 636c 6f63  [.        " cloc
-00000cb0: 6b5f 6765 7474 696d 6522 2c0a 2020 2020  k_gettime",.    
-00000cc0: 2020 2020 2220 6765 7470 6964 222c 0a20      " getpid",. 
-00000cd0: 2020 2020 2020 2022 2077 7269 7465 220a         " write".
-00000ce0: 2020 2020 5d2c 0a20 2020 2022 2f77 6f72      ],.    "/wor
-00000cf0: 6b73 7061 6365 2f50 7974 686f 6e2d 332e  kspace/Python-3.
-00000d00: 3130 2e30 2f4c 6962 2f6d 756c 7469 7072  10.0/Lib/multipr
-00000d10: 6f63 6573 7369 6e67 2f70 726f 6365 7373  ocessing/process
-00000d20: 2e70 7922 3a20 5b0a 2020 2020 2020 2020  .py": [.        
-00000d30: 2220 6765 7463 7764 222c 0a20 2020 2020  " getcwd",.     
-00000d40: 2020 2022 2067 6574 7069 6422 2c0a 2020     " getpid",.  
-00000d50: 2020 2020 2020 2220 6765 7472 616e 646f        " getrando
-00000d60: 6d22 0a20 2020 205d 2c0a 2020 2020 222f  m".    ],.    "/
-00000d70: 776f 726b 7370 6163 652f 5079 7468 6f6e  workspace/Python
-00000d80: 2d33 2e31 302e 302f 4c69 622f 6d75 6c74  -3.10.0/Lib/mult
-00000d90: 6970 726f 6365 7373 696e 672f 7574 696c  iprocessing/util
-00000da0: 2e70 7922 3a20 5b0a 2020 2020 2020 2020  .py": [.        
-00000db0: 2220 7072 6c69 6d69 7436 3422 0a20 2020  " prlimit64".   
-00000dc0: 205d 2c0a 2020 2020 222f 776f 726b 7370   ],.    "/worksp
-00000dd0: 6163 652f 5079 7468 6f6e 2d33 2e31 302e  ace/Python-3.10.
-00000de0: 302f 4c69 622f 6f73 2e70 7922 3a20 5b0a  0/Lib/os.py": [.
-00000df0: 2020 2020 2020 2020 2220 7265 6164 220a          " read".
-00000e00: 2020 2020 5d2c 0a20 2020 2022 2f77 6f72      ],.    "/wor
-00000e10: 6b73 7061 6365 2f50 7974 686f 6e2d 332e  kspace/Python-3.
-00000e20: 3130 2e30 2f4c 6962 2f70 6c61 7466 6f72  10.0/Lib/platfor
-00000e30: 6d2e 7079 223a 205b 0a20 2020 2020 2020  m.py": [.       
-00000e40: 2022 2075 6e61 6d65 220a 2020 2020 5d2c   " uname".    ],
-00000e50: 0a20 2020 2022 2f77 6f72 6b73 7061 6365  .    "/workspace
-00000e60: 2f50 7974 686f 6e2d 332e 3130 2e30 2f4c  /Python-3.10.0/L
-00000e70: 6962 2f70 6f73 6978 7061 7468 2e70 7922  ib/posixpath.py"
-00000e80: 3a20 5b0a 2020 2020 2020 2020 2220 636c  : [.        " cl
-00000e90: 6f73 6522 2c0a 2020 2020 2020 2020 2220  ose",.        " 
-00000ea0: 6673 7461 7422 2c0a 2020 2020 2020 2020  fstat",.        
-00000eb0: 2220 6765 7463 7764 222c 0a20 2020 2020  " getcwd",.     
-00000ec0: 2020 2022 2067 6574 6465 6e74 7336 3422     " getdents64"
-00000ed0: 2c0a 2020 2020 2020 2020 2220 6f70 656e  ,.        " open
-00000ee0: 6174 220a 2020 2020 5d2c 0a20 2020 2022  at".    ],.    "
-00000ef0: 2f77 6f72 6b73 7061 6365 2f50 7974 686f  /workspace/Pytho
-00000f00: 6e2d 332e 3130 2e30 2f4c 6962 2f72 616e  n-3.10.0/Lib/ran
-00000f10: 646f 6d2e 7079 223a 205b 0a20 2020 2020  dom.py": [.     
-00000f20: 2020 2022 2067 6574 7261 6e64 6f6d 220a     " getrandom".
-00000f30: 2020 2020 5d2c 0a2e 2e2e 0a60 6060 0a49      ],.....```.I
-00000f40: 7420 7761 7320 6372 6561 7465 6420 6279  t was created by
-00000f50: 2074 7261 6369 6e67 2074 6865 2063 6f64   tracing the cod
-00000f60: 652e 2073 6563 696d 706f 7274 2061 7574  e. secimport aut
-00000f70: 6f6d 6174 6963 616c 6c79 2066 696e 6473  omatically finds
-00000f80: 2074 6865 7365 2070 6572 2d6d 6f64 756c   these per-modul
-00000f90: 6520 7379 7363 616c 6c73 2066 6f72 2079  e syscalls for y
-00000fa0: 6f75 2e0a 0a46 696e 616c 6c79 2c20 796f  ou...Finally, yo
-00000fb0: 7520 636f 6e76 6572 7420 7468 6973 2070  u convert this p
-00000fc0: 6f6c 6963 7920 696e 746f 2061 6e20 7361  olicy into an sa
-00000fd0: 6e64 626f 7820 2865 4250 4620 696e 7374  ndbox (eBPF inst
-00000fe0: 7275 6d65 6e74 6174 696f 6e20 7363 7269  rumentation scri
-00000ff0: 7074 2920 746f 2072 756e 2074 6865 2070  pt) to run the p
-00001000: 7974 686f 6e20 7072 6f63 6573 7320 696e  ython process in
-00001010: 2070 726f 6475 6374 696f 6e2e 2052 756e   production. Run
-00001020: 6e69 6e67 2074 6865 2073 616e 6462 6f78  ning the sandbox
-00001030: 2077 696c 6c20 656e 666f 7265 2070 7974   will enfore pyt
-00001040: 686f 6e20 746f 206f 6265 7920 616e 7920  hon to obey any 
-00001050: 6769 7665 6e20 706f 6c69 6379 2e0a 0a60  given policy...`
-00001060: 7365 6369 6d70 6f72 7460 2069 7320 6772  secimport` is gr
-00001070: 6561 7420 666f 722e 2e2e 0a2d 2050 7265  eat for....- Pre
-00001080: 7665 6e74 696e 6720 436f 6465 2045 7865  venting Code Exe
-00001090: 6375 7469 6f6e 3a20 7265 6475 6365 2074  cution: reduce t
-000010a0: 6865 2072 6973 6b20 6f66 2073 7570 706c  he risk of suppl
-000010b0: 7920 6368 6169 6e20 6174 7461 636b 732e  y chain attacks.
-000010c0: 0a20 202d 2054 7261 6365 2074 6865 2073  .  - Trace the s
-000010d0: 7973 6361 6c6c 7320 666c 6f77 206f 6620  yscalls flow of 
-000010e0: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-000010f0: 2061 7420 7468 6520 7573 6572 2d73 7061   at the user-spa
-00001100: 6365 2f6f 732f 6b65 726e 656c 206c 6576  ce/os/kernel lev
-00001110: 656c 2061 6e64 2070 6572 206d 6f64 756c  el and per modul
-00001120: 652e 0a20 202d 2052 756e 2079 6f75 7220  e..  - Run your 
-00001130: 6170 706c 6963 6174 696f 6e20 7768 696c  application whil
-00001140: 6520 656e 666f 7263 696e 6720 7379 7363  e enforcing sysc
-00001150: 616c 6c73 2070 6572 206d 6f64 756c 652e  alls per module.
-00001160: 0a20 2020 202d 2055 706f 6e20 7669 6f6c  .    - Upon viol
-00001170: 6174 696f 6e20 6f66 2074 6865 2070 6f6c  ation of the pol
-00001180: 6963 792c 2069 7420 6361 6e20 6c6f 672c  icy, it can log,
-00001190: 2073 746f 702c 206f 7220 6b69 6c6c 2074   stop, or kill t
-000011a0: 6865 2070 726f 6365 7373 2e0a 2d20 5072  he process..- Pr
-000011b0: 6f74 6563 7420 796f 7572 7365 6c66 2066  otect yourself f
-000011c0: 726f 6d20 5243 453a 0a20 202d 2073 6563  rom RCE:.  - sec
-000011d0: 696d 706f 7274 206d 616b 6573 2031 6461  import makes 1da
-000011e0: 7920 6174 7461 636b 7320 6c65 7373 206f  y attacks less o
-000011f0: 6620 616e 2069 7373 7565 2c20 6265 6361  f an issue, beca
-00001200: 7573 6520 6974 2070 7265 7665 6e74 7320  use it prevents 
-00001210: 7468 6520 636f 6465 2066 6f72 6d20 7275  the code form ru
-00001220: 6e6e 696e 672e 2049 6620 796f 7520 6172  nning. If you ar
-00001230: 6520 7573 696e 6720 6120 7675 6c6e 6572  e using a vulner
-00001240: 6162 6c65 2070 6163 6b61 6765 2061 6e64  able package and
-00001250: 2073 6f6d 656f 6e65 2065 7870 6c6f 6974   someone exploit
-00001260: 6564 2069 742c 2079 6f75 7220 706f 6c69  ed it, your poli
-00001270: 6379 2077 696c 6c20 6e6f 7420 616c 6c6f  cy will not allo
-00001280: 7720 7468 6973 2065 7870 6c6f 6974 2773  w this exploit's
-00001290: 2073 7973 6361 6c6c 7320 616e 6420 6974   syscalls and it
-000012a0: 2077 696c 6c20 6265 2068 616e 646c 6564   will be handled
-000012b0: 2061 7320 796f 7520 7769 7368 2e0a 2020   as you wish..  
-000012c0: 2d20 4176 6f69 6420 696e 6369 6465 6e74  - Avoid incident
-000012d0: 7320 6c69 6b65 203c 6120 6872 6566 3d22  s like <a href="
-000012e0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000012f0: 6564 6961 2e6f 7267 2f77 696b 692f 4c6f  edia.org/wiki/Lo
-00001300: 6734 5368 656c 6c22 3e6c 6f67 3473 6865  g4Shell">log4she
-00001310: 6c6c 3c2f 613e 2e20 4120 6c6f 6767 696e  ll</a>. A loggin
-00001320: 6720 6c69 6272 6172 7920 7265 7175 6972  g library requir
-00001330: 6573 2076 6572 7920 6665 7720 7379 7363  es very few sysc
-00001340: 616c 6c73 2c20 616e 6420 6974 2073 686f  alls, and it sho
-00001350: 756c 6420 6e65 7665 7220 7275 6e20 636f  uld never run co
-00001360: 6d6d 616e 6420 7573 696e 6720 666f 726b  mmand using fork
-00001370: 2c20 6578 6563 7665 206f 7220 7370 6177  , execve or spaw
-00001380: 6e2e 0a20 2020 202d 2054 6865 2073 7973  n..    - The sys
-00001390: 6361 6c6c 7320 7468 6174 2022 6661 7374  calls that "fast
-000013a0: 6170 6922 2c20 226e 756d 7079 2220 6f72  api", "numpy" or
-000013b0: 2022 7265 7175 6573 7473 2220 7573 6520   "requests" use 
-000013c0: 6172 6520 7665 7279 2064 6966 6665 7265  are very differe
-000013d0: 6e74 2e0a 2d20 4c6f 6164 2041 4920 4d6f  nt..- Load AI Mo
-000013e0: 6465 6c73 2066 726f 6d20 496e 7365 6375  dels from Insecu
-000013f0: 7265 2053 6f75 7263 6573 0a20 202d 204d  re Sources.  - M
-00001400: 6f64 656c 7320 6672 6f6d 2075 6e73 6166  odels from unsaf
-00001410: 6520 736f 7572 6365 2028 6875 6767 696e  e source (huggin
-00001420: 6766 6163 652c 2074 6f72 6368 2068 7562  gface, torch hub
-00001430: 2c20 616e 6420 7079 746f 7263 6820 7069  , and pytorch pi
-00001440: 636b 6c65 6420 6d6f 6465 6c73 2920 6361  ckled models) ca
-00001450: 6e20 6265 206c 696d 6974 6564 2074 6f20  n be limited to 
-00001460: 7275 6e20 6f6e 6c79 2061 2073 6574 206f  run only a set o
-00001470: 6620 7379 7363 616c 6c73 2e20 5243 4520  f syscalls. RCE 
-00001480: 6c69 6b65 2027 696d 706f 7274 206f 733b  like 'import os;
-00001490: 6f73 2e73 7973 7465 6d28 2e2e 2e29 2720  os.system(...)' 
-000014a0: 736f 6d65 7768 6572 6520 6465 6570 2069  somewhere deep i
-000014b0: 6e20 7468 6520 636f 6465 2077 696c 6c20  n the code will 
-000014c0: 6265 2063 6174 6368 6564 2062 7920 7365  be catched by se
-000014d0: 6369 6d70 6f72 742e 0a2d 204d 696e 696d  cimport..- Minim
-000014e0: 616c 2050 6572 666f 726d 616e 6365 2049  al Performance I
-000014f0: 6d70 6163 740a 2020 2d20 2048 6173 206e  mpact.  -  Has n
-00001500: 6567 6c69 6769 626c 6520 7065 7266 6f72  egligible perfor
-00001510: 6d61 6e63 6520 696d 7061 6374 2061 6e64  mance impact and
-00001520: 2069 7320 7072 6f64 7563 7469 6f6e 2d72   is production-r
-00001530: 6561 6479 2074 6861 6e6b 7320 746f 2065  eady thanks to e
-00001540: 4250 462e 2043 6865 636b 206f 7574 2074  BPF. Check out t
-00001550: 6865 205b 5065 7266 6f72 6d61 6e63 655d  he [Performance]
-00001560: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001570: 636f 6d2f 6176 696c 756d 2f73 6563 696d  com/avilum/secim
-00001580: 706f 7274 2f77 696b 692f 5065 7266 6f72  port/wiki/Perfor
-00001590: 6d61 6e63 652d 4265 6e63 686d 6172 6b73  mance-Benchmarks
-000015a0: 2920 6265 6e63 686d 6172 6b73 2e0a 2d20  ) benchmarks..- 
-000015b0: 5472 6163 6520 7768 6963 6820 7379 7363  Trace which sysc
-000015c0: 616c 6c73 2061 7265 2063 616c 6c65 6420  alls are called 
-000015d0: 6279 2065 6163 6820 6d6f 6475 6c65 2069  by each module i
-000015e0: 6e20 796f 7572 2063 6f64 652e 0a20 202d  n your code..  -
-000015f0: 2073 6563 696d 706f 7274 2075 7365 7320   secimport uses 
-00001600: 5553 4454 2028 5573 6572 6c61 6e64 2053  USDT (Userland S
-00001610: 7461 7469 6361 6c6c 7920 4465 6669 6e65  tatically Define
-00001620: 6420 5472 6163 696e 6729 2074 6f67 6574  d Tracing) toget
-00001630: 6865 7220 7769 7468 206b 6572 6e65 6c20  her with kernel 
-00001640: 7072 6f62 6573 2069 6e20 7468 6520 7275  probes in the ru
-00001650: 6e74 696d 6520 7573 696e 6720 6542 5046  ntime using eBPF
-00001660: 206f 7220 6474 7261 6365 2069 6e73 7472   or dtrace instr
-00001670: 756d 656e 7461 7469 6f6e 2073 6372 6970  umentation scrip
-00001680: 7473 2e0a 2323 2049 6e73 7461 6c6c 6174  ts..## Installat
-00001690: 696f 6e0a 5465 7374 6564 206f 6e20 5562  ion.Tested on Ub
-000016a0: 756e 7475 2c20 4465 6269 616e 2c20 526f  untu, Debian, Ro
-000016b0: 636b 7920 284c 696e 7578 2078 3836 2f41  cky (Linux x86/A
-000016c0: 4d44 2f41 524d 2920 616e 6420 4d61 634f  MD/ARM) and MacO
-000016d0: 5320 696e 2028 7838 362f 4d31 292e 2049  S in (x86/M1). I
-000016e0: 6620 796f 7520 7275 6e20 6f6e 204d 6163  f you run on Mac
-000016f0: 4f53 2079 6f75 2077 696c 6c20 6e65 6564  OS you will need
-00001700: 2074 6f20 3c61 2068 7265 663d 2268 7474   to <a href="htt
-00001710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001720: 6176 696c 756d 2f73 6563 696d 706f 7274  avilum/secimport
-00001730: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-00001740: 732f 4d41 435f 4f53 5f55 5345 5253 2e6d  s/MAC_OS_USERS.m
-00001750: 6422 3e64 6973 6162 6c65 2053 4950 2066  d">disable SIP f
-00001760: 6f72 2064 7472 6163 652e 203c 2f61 3e0a  or dtrace. </a>.
-00001770: 0a23 2320 5769 7468 2044 6f63 6b65 720a  .## With Docker.
-00001780: 466f 7220 7175 6963 6b65 7220 6576 616c  For quicker eval
-00001790: 7561 7469 6f6e 2c20 7765 2072 6563 6f6d  uation, we recom
-000017a0: 6d65 6e64 2075 7369 6e67 2074 6865 203c  mend using the <
-000017b0: 6120 6872 6566 3d22 5b64 6f63 732f 446f  a href="[docs/Do
-000017c0: 636b 6572 5d28 6874 7470 733a 2f2f 6769  cker](https://gi
-000017d0: 7468 7562 2e63 6f6d 2f61 7669 6c75 6d2f  thub.com/avilum/
-000017e0: 7365 6369 6d70 6f72 742f 626c 6f62 2f6d  secimport/blob/m
-000017f0: 6173 7465 722f 646f 636b 6572 2f52 4541  aster/docker/REA
-00001800: 444d 452e 6d64 2922 3e53 6563 696d 706f  DME.md)">Secimpo
-00001810: 7274 2044 6f63 6b65 7220 496d 6167 653c  rt Docker Image<
-00001820: 2f61 3e20 696e 7374 6561 6420 6f66 2073  /a> instead of s
-00001830: 656c 662d 696e 7374 616c 6c69 6e67 2e3c  elf-installing.<
-00001840: 6272 3e0a 2d20 4275 696c 6420 616e 6420  br>.- Build and 
-00001850: 7275 6e20 7468 6520 446f 636b 6572 2063  run the Docker c
-00001860: 6f6e 7461 696e 6572 2077 6974 6820 6120  ontainer with a 
-00001870: 6375 7374 6f6d 206b 6572 6e65 6c20 7468  custom kernel th
-00001880: 6174 206d 6174 6368 6573 2079 6f75 7220  at matches your 
-00001890: 6578 6973 7469 6e67 204f 5320 6b65 726e  existing OS kern
-000018a0: 656c 2076 6572 7369 6f6e 3a0a 2020 6060  el version:.  ``
-000018b0: 600a 2020 6364 2064 6f63 6b65 722f 2026  `.  cd docker/ &
-000018c0: 2620 2e2f 6275 696c 642e 7368 2026 2620  & ./build.sh && 
-000018d0: 2e2f 7275 6e2e 7368 0a20 2060 6060 0a20  ./run.sh.  ```. 
-000018e0: 2041 2074 656d 706f 7261 7279 2063 6f6e   A temporary con
-000018f0: 7461 696e 6572 2077 696c 6c20 6265 2063  tainer will be c
-00001900: 7265 6174 6564 2c20 616e 6420 796f 7520  reated, and you 
-00001910: 7769 6c6c 2062 6520 6c6f 6767 6564 2069  will be logged i
-00001920: 6e20 6173 2074 6865 2072 6f6f 7420 7573  n as the root us
-00001930: 6572 2e0a 0a23 2320 5769 7468 6f75 7420  er...## Without 
-00001940: 446f 636b 6572 0a31 2e20 496e 7374 616c  Docker.1. Instal
-00001950: 6c20 7079 7468 6f6e 2077 6974 6820 5553  l python with US
-00001960: 4454 2070 726f 6265 7320 6279 203c 6120  DT probes by <a 
-00001970: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001980: 7468 7562 2e63 6f6d 2f61 7669 6c75 6d2f  thub.com/avilum/
-00001990: 7365 6369 6d70 6f72 742f 7769 6b69 2f49  secimport/wiki/I
-000019a0: 6e73 7461 6c6c 6174 696f 6e23 7079 7468  nstallation#pyth
-000019b0: 6f6e 2d69 6e74 6572 7072 6574 6572 2d72  on-interpreter-r
-000019c0: 6571 7569 7265 6d65 6e74 7322 3e63 6f6e  equirements">con
-000019d0: 6669 6775 7269 6e67 2069 7420 7769 7468  figuring it with
-000019e0: 2027 2d2d 6474 7261 6365 273c 2f61 3e0a   '--dtrace'</a>.
-000019f0: 322e 2049 6e73 7461 6c6c 206f 6e65 206f  2. Install one o
-00001a00: 6620 7468 6520 6261 636b 656e 6473 3a20  f the backends: 
-00001a10: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001a20: 2f67 6974 6875 622e 636f 6d2f 6176 696c  /github.com/avil
-00001a30: 756d 2f73 6563 696d 706f 7274 2f77 696b  um/secimport/wik
-00001a40: 692f 496e 7374 616c 6c61 7469 6f6e 223e  i/Installation">
-00001a50: 6542 5046 206f 7220 4454 7261 6365 3c2f  eBPF or DTrace</
-00001a60: 613e 2e0a 332e 2049 6e73 7461 6c6c 2073  a>..3. Install s
-00001a70: 6563 696d 706f 7274 0a20 202d 2049 6e73  ecimport.  - Ins
-00001a80: 7461 6c6c 2066 726f 6d20 7079 7069 0a20  tall from pypi. 
-00001a90: 2020 202d 2060 6060 0a20 2020 2020 2070     - ```.      p
-00001aa0: 7974 686f 6e33 202d 6d20 7069 7020 696e  ython3 -m pip in
-00001ab0: 7374 616c 6c20 7365 6369 6d70 6f72 740a  stall secimport.
-00001ac0: 2020 2020 2020 6060 600a 2020 2d20 496e        ```.  - In
-00001ad0: 7374 616c 6c20 6672 6f6d 2073 6f75 7263  stall from sourc
-00001ae0: 650a 2020 2020 2d20 6060 600a 2020 2020  e.    - ```.    
-00001af0: 2020 6769 7420 636c 6f6e 6520 6874 7470    git clone http
-00001b00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00001b10: 7669 6c75 6d2f 7365 6369 6d70 6f72 742e  vilum/secimport.
-00001b20: 6769 7420 2626 2063 6420 7365 6369 6d70  git && cd secimp
-00001b30: 6f72 740a 2020 2020 2020 7079 7468 6f6e  ort.      python
-00001b40: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
-00001b50: 2070 6f65 7472 7920 2626 2070 7974 686f   poetry && pytho
-00001b60: 6e33 202d 6d20 706f 6574 7279 2069 6e73  n3 -m poetry ins
-00001b70: 7461 6c6c 0a20 2020 2020 2060 6060 0a0a  tall.      ```..
-00001b80: 0a23 2320 5573 6167 650a 546f 2073 616e  .## Usage.To san
-00001b90: 6462 6f78 2079 6f75 7220 7072 6f67 7261  dbox your progra
-00001ba0: 6d20 7573 696e 6720 7468 6520 434c 492c  m using the CLI,
-00001bb0: 2073 7461 7274 2061 2062 7066 7472 6163   start a bpftrac
-00001bc0: 6520 7072 6f67 7261 6d20 7468 6174 206c  e program that l
-00001bd0: 6f67 7320 616c 6c20 7468 6520 7379 7363  ogs all the sysc
-00001be0: 616c 6c73 2066 6f72 2061 6c6c 2074 6865  alls for all the
-00001bf0: 206d 6f64 756c 6573 2069 6e20 796f 7572   modules in your
-00001c00: 2061 7070 6c69 6361 7469 6f6e 2069 6e74   application int
-00001c10: 6f20 6120 6669 6c65 2077 6974 6820 7468  o a file with th
-00001c20: 6520 7365 6369 6d70 6f72 7420 7472 6163  e secimport trac
-00001c30: 6520 636f 6d6d 616e 642e 204f 6e63 6520  e command. Once 
-00001c40: 796f 7520 6861 7665 2063 6f76 6572 6564  you have covered
-00001c50: 2074 6865 206c 6f67 6963 2079 6f75 2077   the logic you w
-00001c60: 6f75 6c64 206c 696b 6520 746f 2073 616e  ould like to san
-00001c70: 6462 6f78 2c20 6869 7420 4354 524c 2b43  dbox, hit CTRL+C
-00001c80: 206f 7220 4354 524c 2b44 2c20 6f72 2077   or CTRL+D, or w
-00001c90: 6169 7420 666f 7220 7468 6520 7072 6f67  ait for the prog
-00001ca0: 7261 6d20 746f 2066 696e 6973 682e 2054  ram to finish. T
-00001cb0: 6865 6e2c 2062 7569 6c64 2061 2073 616e  hen, build a san
-00001cc0: 6462 6f78 2066 726f 6d20 7468 6520 7472  dbox from the tr
-00001cd0: 6163 6520 7573 696e 6720 7468 6520 7365  ace using the se
-00001ce0: 6369 6d70 6f72 7420 6275 696c 6420 636f  cimport build co
-00001cf0: 6d6d 616e 642c 2061 6e64 2072 756e 2074  mmand, and run t
-00001d00: 6865 2073 616e 6462 6f78 2077 6974 6820  he sandbox with 
-00001d10: 7468 6520 7365 6369 6d70 6f72 7420 7275  the secimport ru
-00001d20: 6e20 636f 6d6d 616e 642e 0a0a 6060 6073  n command...```s
-00001d30: 6865 6c6c 0a4e 414d 450a 2020 2020 7365  hell.NAME.    se
-00001d40: 6369 6d70 6f72 7420 2d20 6973 2061 2063  cimport - is a c
-00001d50: 6f6d 7072 6568 656e 7369 7665 2074 6f6f  omprehensive too
-00001d60: 6c6b 6974 2064 6573 6967 6e65 6420 746f  lkit designed to
-00001d70: 2065 6e61 626c 6520 7468 6520 7472 6163   enable the trac
-00001d80: 696e 672c 2063 6f6e 7374 7275 6374 696f  ing, constructio
-00001d90: 6e2c 2061 6e64 2065 7865 6375 7469 6f6e  n, and execution
-00001da0: 206f 6620 7365 6375 7265 2050 7974 686f   of secure Pytho
-00001db0: 6e20 7275 6e74 696d 6573 2e20 4974 206c  n runtimes. It l
-00001dc0: 6576 6572 6167 6573 2055 5344 5420 7072  everages USDT pr
-00001dd0: 6f62 6573 2061 6e64 2065 4250 462f 4454  obes and eBPF/DT
-00001de0: 7261 6365 2074 6563 686e 6f6c 6f67 6965  race technologie
-00001df0: 7320 746f 2065 6e68 616e 6365 2074 6865  s to enhance the
-00001e00: 206f 7665 7261 6c6c 2073 6563 7572 6974   overall securit
-00001e10: 7920 6d65 6173 7572 6573 2e0a 0a53 594e  y measures...SYN
-00001e20: 4f50 5349 530a 2020 2020 7365 6369 6d70  OPSIS.    secimp
-00001e30: 6f72 7420 434f 4d4d 414e 440a 0a44 4553  ort COMMAND..DES
-00001e40: 4352 4950 5449 4f4e 0a20 2020 2068 7474  CRIPTION.    htt
-00001e50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001e60: 6176 696c 756d 2f73 6563 696d 706f 7274  avilum/secimport
-00001e70: 2f77 696b 692f 436f 6d6d 616e 642d 4c69  /wiki/Command-Li
-00001e80: 6e65 2d55 7361 6765 0a0a 2020 2020 574f  ne-Usage..    WO
-00001e90: 524b 464c 4f57 3a0a 2020 2020 2020 2020  RKFLOW:.        
-00001ea0: 2020 2020 312e 2073 6563 696d 706f 7274      1. secimport
-00001eb0: 2074 7261 6365 202f 2073 6563 696d 706f   trace / secimpo
-00001ec0: 7274 2073 6865 6c6c 0a20 2020 2020 2020  rt shell.       
-00001ed0: 2020 2020 2032 2e20 7365 6369 6d70 6f72       2. secimpor
-00001ee0: 7420 6275 696c 640a 2020 2020 2020 2020  t build.        
-00001ef0: 2020 2020 332e 2073 6563 696d 706f 7274      3. secimport
-00001f00: 2072 756e 0a0a 2020 2020 5155 4943 4b53   run..    QUICKS
-00001f10: 5441 5254 3a0a 2020 2020 2020 2020 2020  TART:.          
-00001f20: 2020 2420 7365 6369 6d70 6f72 7420 696e    $ secimport in
-00001f30: 7465 7261 6374 6976 650a 0a20 2020 2045  teractive..    E
-00001f40: 5841 4d50 4c45 533a 0a20 2020 2020 2020  XAMPLES:.       
-00001f50: 2031 2e20 7472 6163 653a 0a20 2020 2020   1. trace:.     
-00001f60: 2020 2020 2020 2024 2020 7365 6369 6d70         $  secimp
-00001f70: 6f72 7420 7472 6163 650a 2020 2020 2020  ort trace.      
-00001f80: 2020 2020 2020 2420 2073 6563 696d 706f        $  secimpo
-00001f90: 7274 2074 7261 6365 202d 680a 2020 2020  rt trace -h.    
-00001fa0: 2020 2020 2020 2020 2420 2073 6563 696d          $  secim
-00001fb0: 706f 7274 2074 7261 6365 5f70 6964 2031  port trace_pid 1
-00001fc0: 3233 0a20 2020 2020 2020 2020 2020 2024  23.            $
-00001fd0: 2020 7365 6369 6d70 6f72 7420 7472 6163    secimport trac
-00001fe0: 655f 7069 6420 2d68 0a20 2020 2020 2020  e_pid -h.       
-00001ff0: 2032 2e20 6275 696c 643a 0a20 2020 2020   2. build:.     
-00002000: 2020 2020 2020 2023 2073 6563 696d 706f         # secimpo
-00002010: 7274 2062 7569 6c64 0a20 2020 2020 2020  rt build.       
-00002020: 2020 2020 2024 2073 6563 696d 706f 7274       $ secimport
-00002030: 2062 7569 6c64 202d 680a 2020 2020 2020   build -h.      
-00002040: 2020 332e 2072 756e 3a0a 2020 2020 2020    3. run:.      
-00002050: 2020 2020 2020 2420 2073 6563 696d 706f        $  secimpo
-00002060: 7274 2072 756e 0a20 2020 2020 2020 2020  rt run.         
-00002070: 2020 2024 2020 7365 6369 6d70 6f72 7420     $  secimport 
-00002080: 7275 6e20 2d2d 656e 7472 7970 6f69 6e74  run --entrypoint
-00002090: 206d 795f 6375 7374 6f6d 5f6d 6169 6e2e   my_custom_main.
-000020a0: 7079 0a20 2020 2020 2020 2020 2020 2024  py.            $
-000020b0: 2020 7365 6369 6d70 6f72 7420 7275 6e20    secimport run 
-000020c0: 2d2d 656e 7472 7970 6f69 6e74 206d 795f  --entrypoint my_
-000020d0: 6375 7374 6f6d 5f6d 6169 6e2e 7079 202d  custom_main.py -
-000020e0: 2d73 746f 705f 6f6e 5f76 696f 6c61 7469  -stop_on_violati
-000020f0: 6f6e 3d74 7275 650a 2020 2020 2020 2020  on=true.        
-00002100: 2020 2020 2420 2073 6563 696d 706f 7274      $  secimport
-00002110: 2072 756e 202d 2d65 6e74 7279 706f 696e   run --entrypoin
-00002120: 7420 6d79 5f63 7573 746f 6d5f 6d61 696e  t my_custom_main
-00002130: 2e70 7920 2d2d 6b69 6c6c 5f6f 6e5f 7669  .py --kill_on_vi
-00002140: 6f6c 6174 696f 6e3d 7472 7565 0a20 2020  olation=true.   
-00002150: 2020 2020 2020 2020 2024 2020 7365 6369           $  seci
-00002160: 6d70 6f72 7420 7275 6e20 2d2d 7361 6e64  mport run --sand
-00002170: 626f 785f 6578 6563 7574 6162 6c65 202f  box_executable /
-00002180: 7061 7468 2f74 6f2f 6d79 5f73 616e 6462  path/to/my_sandb
-00002190: 6f78 2e62 7420 2d2d 7069 6420 3238 3834  ox.bt --pid 2884
-000021a0: 0a20 2020 2020 2020 2020 2020 2024 2020  .            $  
-000021b0: 7365 6369 6d70 6f72 7420 7275 6e20 2d2d  secimport run --
-000021c0: 7361 6e64 626f 785f 6578 6563 7574 6162  sandbox_executab
-000021d0: 6c65 202f 7061 7468 2f74 6f2f 6d79 5f73  le /path/to/my_s
-000021e0: 616e 6462 6f78 2e62 7420 2d2d 7361 6e64  andbox.bt --sand
-000021f0: 626f 785f 6c6f 6766 696c 6520 6d79 5f6c  box_logfile my_l
-00002200: 6f67 2e6c 6f67 0a20 2020 2020 2020 2020  og.log.         
-00002210: 2020 2024 2020 7365 6369 6d70 6f72 7420     $  secimport 
-00002220: 7275 6e20 2d68 0a0a 434f 4d4d 414e 4453  run -h..COMMANDS
-00002230: 0a20 2020 2043 4f4d 4d41 4e44 2069 7320  .    COMMAND is 
-00002240: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
-00002250: 7769 6e67 3a0a 0a20 2020 2020 6275 696c  wing:..     buil
-00002260: 640a 2020 2020 2020 2043 6f6d 7069 6c65  d.       Compile
-00002270: 7320 6120 7472 6163 6520 6c6f 6720 2874  s a trace log (t
-00002280: 7261 6365 2e6c 6f67 292e 2043 7265 6174  race.log). Creat
-00002290: 6573 2074 6865 2073 616e 6462 6f78 2065  es the sandbox e
-000022a0: 7865 6375 7461 626c 6520 2869 6e73 7472  xecutable (instr
-000022b0: 756d 656e 7461 7469 6f6e 2073 6372 6970  umentation scrip
-000022c0: 7429 2066 6f72 2065 6163 6820 7375 7070  t) for each supp
-000022d0: 6f72 7465 6420 6261 636b 656e 6420 4974  orted backend It
-000022e0: 2075 7365 7320 6063 7265 6174 655f 7072   uses `create_pr
-000022f0: 6f66 696c 655f 6672 6f6d 5f74 7261 6365  ofile_from_trace
-00002300: 202e 2e2e 6020 616e 6420 6073 616e 6462   ...` and `sandb
-00002310: 6f78 5f66 726f 6d5f 7072 6f66 696c 6560  ox_from_profile`
-00002320: 2e0a 0a20 2020 2020 636f 6d70 696c 655f  ...     compile_
-00002330: 7361 6e64 626f 785f 6672 6f6d 5f70 726f  sandbox_from_pro
-00002340: 6669 6c65 0a20 2020 2020 2020 4765 6e65  file.       Gene
-00002350: 7261 7465 7320 6120 7461 696c 6f72 2d6d  rates a tailor-m
-00002360: 6164 6520 7361 6e64 626f 7820 7468 6174  ade sandbox that
-00002370: 2077 696c 6c20 656e 666f 7263 6520 6120   will enforce a 
-00002380: 6769 7665 6e20 7961 6d6c 2070 726f 6669  given yaml profi
-00002390: 6c65 2f70 6f6c 6963 7920 696e 2072 756e  le/policy in run
-000023a0: 7469 6d65 2e0a 0a20 2020 2020 696e 7465  time...     inte
-000023b0: 7261 6374 6976 650a 0a20 2020 2020 7275  ractive..     ru
-000023c0: 6e0a 2020 2020 2020 2052 756e 2061 2070  n.       Run a p
-000023d0: 7974 686f 6e20 7072 6f63 6573 7320 696e  ython process in
-000023e0: 7369 6465 2074 6865 2073 616e 6462 6f78  side the sandbox
-000023f0: 2e0a 0a20 2020 2020 7368 656c 6c0a 2020  ...     shell.  
-00002400: 2020 2020 2041 6c74 6572 6e61 7469 7665       Alternative
-00002410: 2073 796e 7461 7820 666f 7220 7365 6369   syntax for seci
-00002420: 6d70 6f72 7420 2274 7261 6365 222e 0a0a  mport "trace"...
-00002430: 2020 2020 2074 7261 6365 0a20 2020 2020       trace.     
-00002440: 2020 5472 6163 6573 2061 2070 7974 686f    Traces a pytho
-00002450: 6e20 7072 6f63 6573 7320 7573 696e 6720  n process using 
-00002460: 616e 2065 6e74 7279 706f 696e 7420 6f72  an entrypoint or
-00002470: 2069 6e74 6572 6163 7469 7665 2069 6e74   interactive int
-00002480: 6572 7072 6574 6572 2e20 4974 206d 6967  erpreter. It mig
-00002490: 6874 2072 6571 7569 7265 2073 7564 6f20  ht require sudo 
-000024a0: 7072 6976 696c 6c65 6765 7320 6f6e 2073  privilleges on s
-000024b0: 6f6d 6520 686f 7374 732e 0a0a 2020 2020  ome hosts...    
-000024c0: 2074 7261 6365 5f70 6964 0a20 2020 2020   trace_pid.     
-000024d0: 2020 5472 6163 6573 2061 2072 756e 6e69    Traces a runni
-000024e0: 6e67 2070 726f 6365 7373 2062 7920 7069  ng process by pi
-000024f0: 642e 2049 7420 6d69 6768 7420 7265 7175  d. It might requ
-00002500: 6972 6520 7375 646f 2070 7269 7669 6c6c  ire sudo privill
-00002510: 6567 6573 206f 6e20 736f 6d65 2068 6f73  eges on some hos
-00002520: 7473 2e0a 6060 600a 0a23 2320 5374 6f70  ts..```..## Stop
-00002530: 206f 6e20 7669 6f6c 6174 696f 6e0a 6060   on violation.``
-00002540: 600a 726f 6f74 4031 6263 3035 3331 6439  `.root@1bc0531d9
-00002550: 3164 303a 2f77 6f72 6b73 7061 6365 2320  1d0:/workspace# 
-00002560: 7365 6369 6d70 6f72 7420 7275 6e20 202d  secimport run  -
-00002570: 2d73 746f 705f 6f6e 5f76 696f 6c61 7469  -stop_on_violati
-00002580: 6f6e 3d74 7275 650a 203e 3e3e 2073 6563  on=true. >>> sec
-00002590: 696d 706f 7274 2072 756e 0a5b 5741 524e  import run.[WARN
-000025a0: 494e 475d 3a20 5468 6973 2073 616e 6462  ING]: This sandb
-000025b0: 6f78 2077 696c 6c20 7365 6e64 2053 4947  ox will send SIG
-000025c0: 5354 4f50 2074 6f20 7468 6520 7072 6f67  STOP to the prog
-000025d0: 7261 6d20 7570 6f6e 2076 696f 6c61 7469  ram upon violati
-000025e0: 6f6e 2e0a 2052 554e 4e49 4e47 2053 414e  on.. RUNNING SAN
-000025f0: 4442 4f58 2e2e 2e20 5b27 2e2f 7361 6e64  DBOX... ['./sand
-00002600: 626f 782e 6274 272c 2027 2d2d 756e 7361  box.bt', '--unsa
-00002610: 6665 272c 2027 202d 6320 272c 2027 2f77  fe', ' -c ', '/w
-00002620: 6f72 6b73 7061 6365 2f50 7974 686f 6e2d  orkspace/Python-
-00002630: 332e 3130 2e30 2f70 7974 686f 6e27 2c20  3.10.0/python', 
-00002640: 2753 544f 5027 5d0a 4174 7461 6368 696e  'STOP'].Attachin
-00002650: 6720 3420 7072 6f62 6573 2e2e 2e0a 5079  g 4 probes....Py
-00002660: 7468 6f6e 2033 2e31 302e 3020 2864 6566  thon 3.10.0 (def
-00002670: 6175 6c74 2c20 4170 7220 3238 2032 3032  ault, Apr 28 202
-00002680: 332c 2031 313a 3332 3a34 3029 205b 4743  3, 11:32:40) [GC
-00002690: 4320 392e 342e 305d 206f 6e20 6c69 6e75  C 9.4.0] on linu
-000026a0: 780a 5479 7065 2022 6865 6c70 222c 2022  x.Type "help", "
-000026b0: 636f 7079 7269 6768 7422 2c20 2263 7265  copyright", "cre
-000026c0: 6469 7473 2220 6f72 2022 6c69 6365 6e73  dits" or "licens
-000026d0: 6522 2066 6f72 206d 6f72 6520 696e 666f  e" for more info
-000026e0: 726d 6174 696f 6e2e 0a3e 3e3e 2069 6d70  rmation..>>> imp
-000026f0: 6f72 7420 6f73 0a3e 3e3e 206f 732e 7379  ort os.>>> os.sy
-00002700: 7374 656d 2827 7073 2729 0a5b 5345 4355  stem('ps').[SECU
-00002710: 5249 5459 2050 524f 4649 4c45 2056 494f  RITY PROFILE VIO
-00002720: 4c41 5445 445d 3a20 3c73 7464 696e 3e20  LATED]: <stdin> 
-00002730: 6361 6c6c 6564 2073 7973 6361 6c6c 2035  called syscall 5
-00002740: 3620 6174 2064 6570 7468 2038 3032 320a  6 at depth 8022.
-00002750: 0a5e 5e5e 2053 544f 5050 494e 4720 5052  .^^^ STOPPING PR
-00002760: 4f43 4553 5320 3835 3931 3820 4455 4520  OCESS 85918 DUE 
-00002770: 544f 2053 5953 4341 4c4c 2056 494f 4c41  TO SYSCALL VIOLA
-00002780: 5449 4f4e 205e 5e5e 0a09 0950 524f 4345  TION ^^^...PROCE
-00002790: 5353 2038 3539 3138 2053 544f 5050 4544  SS 85918 STOPPED
-000027a0: 2e0a 6060 600a 0a23 2320 4b69 6c6c 206f  ..```..## Kill o
-000027b0: 6e20 7669 6f6c 6174 696f 6e0a 6060 600a  n violation.```.
-000027c0: 726f 6f74 4065 6534 6263 3939 6262 3031  root@ee4bc99bb01
-000027d0: 313a 2f77 6f72 6b73 7061 6365 2320 7365  1:/workspace# se
-000027e0: 6369 6d70 6f72 7420 7275 6e20 2d2d 6b69  cimport run --ki
-000027f0: 6c6c 5f6f 6e5f 7669 6f6c 6174 696f 6e0a  ll_on_violation.
-00002800: 203e 3e3e 2073 6563 696d 706f 7274 2072   >>> secimport r
-00002810: 756e 0a5b 5741 524e 494e 475d 3a20 5468  un.[WARNING]: Th
-00002820: 6973 2073 616e 6462 6f78 2077 696c 6c20  is sandbox will 
-00002830: 7365 6e64 2053 4947 4b49 4c4c 2074 6f20  send SIGKILL to 
-00002840: 7468 6520 7072 6f67 7261 6d20 7570 6f6e  the program upon
-00002850: 2076 696f 6c61 7469 6f6e 2e0a 2052 554e   violation.. RUN
-00002860: 4e49 4e47 2053 414e 4442 4f58 2e2e 2e20  NING SANDBOX... 
-00002870: 5b27 2e2f 7361 6e64 626f 782e 6274 272c  ['./sandbox.bt',
-00002880: 2027 2d2d 756e 7361 6665 272c 2027 202d   '--unsafe', ' -
-00002890: 6320 272c 2027 2f77 6f72 6b73 7061 6365  c ', '/workspace
-000028a0: 2f50 7974 686f 6e2d 332e 3130 2e30 2f70  /Python-3.10.0/p
-000028b0: 7974 686f 6e27 2c20 274b 494c 4c27 5d0a  ython', 'KILL'].
-000028c0: 696d 706f 7274 206f 730a 6f41 7474 6163  import os.oAttac
-000028d0: 6869 6e67 2034 2070 726f 6265 732e 2e2e  hing 4 probes...
-000028e0: 0a73 5079 7468 6f6e 2033 2e31 302e 3020  .sPython 3.10.0 
-000028f0: 2864 6566 6175 6c74 2c20 4170 7220 3238  (default, Apr 28
-00002900: 2032 3032 332c 2031 313a 3332 3a34 3029   2023, 11:32:40)
-00002910: 205b 4743 4320 392e 342e 305d 206f 6e20   [GCC 9.4.0] on 
-00002920: 6c69 6e75 780a 5479 7065 2022 6865 6c70  linux.Type "help
-00002930: 222c 2022 636f 7079 7269 6768 7422 2c20  ", "copyright", 
-00002940: 2263 7265 6469 7473 2220 6f72 2022 6c69  "credits" or "li
-00002950: 6365 6e73 6522 2066 6f72 206d 6f72 6520  cense" for more 
-00002960: 696e 666f 726d 6174 696f 6e2e 0a3e 3e3e  information..>>>
-00002970: 2069 6d70 6f72 7420 6f73 0a3e 3e3e 206f   import os.>>> o
-00002980: 732e 7379 7374 656d 2827 7073 2729 0a5b  s.system('ps').[
-00002990: 5345 4355 5249 5459 2050 524f 4649 4c45  SECURITY PROFILE
-000029a0: 2056 494f 4c41 5445 445d 3a20 3c73 7464   VIOLATED]: <std
-000029b0: 696e 3e20 6361 6c6c 6564 2073 7973 6361  in> called sysca
-000029c0: 6c6c 2035 3620 6174 2064 6570 7468 2038  ll 56 at depth 8
-000029d0: 3032 320a 0a5e 5e5e 204b 494c 4c49 4e47  022..^^^ KILLING
-000029e0: 2050 524f 4345 5353 2038 3634 3636 2044   PROCESS 86466 D
-000029f0: 5545 2054 4f20 5359 5343 414c 4c20 5649  UE TO SYSCALL VI
-00002a00: 4f4c 4154 494f 4e20 5e5e 5e0a 0909 4b49  OLATION ^^^...KI
-00002a10: 4c4c 4544 2e0a 2053 414e 4442 4f58 2045  LLED.. SANDBOX E
-00002a20: 5849 5445 443b 0a60 6060 0a0a 2323 2044  XITED;.```..## D
-00002a30: 796e 616d 6963 2070 726f 6669 6c69 6e67  ynamic profiling
-00002a40: 202d 2074 7261 6365 2c20 6275 696c 6420   - trace, build 
-00002a50: 7361 6e64 626f 782c 2072 756e 2e0a 6060  sandbox, run..``
-00002a60: 6073 6865 6c6c 0a72 6f6f 7440 3166 6133  `shell.root@1fa3
-00002a70: 6436 6630 3939 3839 3a2f 776f 726b 7370  d6f09989:/worksp
-00002a80: 6163 6523 2073 6563 696d 706f 7274 2069  ace# secimport i
-00002a90: 6e74 6572 6163 7469 7665 0a0a 4c65 7427  nteractive..Let'
-00002aa0: 7320 6372 6561 7465 206f 7572 2066 6972  s create our fir
-00002ab0: 7374 2074 6169 6c6f 722d 6d61 6465 2073  st tailor-made s
-00002ac0: 616e 6462 6f78 2077 6974 6820 7365 6369  andbox with seci
-00002ad0: 6d70 6f72 7421 0a2d 2041 2070 7974 686f  mport!.- A pytho
-00002ae0: 6e20 7368 656c 6c20 7769 6c6c 2062 6520  n shell will be 
-00002af0: 6f70 656e 6564 0a2d 2054 6865 2062 6568  opened.- The beh
-00002b00: 6176 696f 7220 7769 6c6c 2062 6520 7265  avior will be re
-00002b10: 636f 7264 6564 2e0a 0a4f 4b3f 2028 7929  corded...OK? (y)
-00002b20: 3a20 790a 203e 3e3e 2073 6563 696d 706f  : y. >>> secimpo
-00002b30: 7274 2074 7261 6365 0a0a 5452 4143 494e  rt trace..TRACIN
-00002b40: 473a 205b 272f 776f 726b 7370 6163 652f  G: ['/workspace/
-00002b50: 7365 6369 6d70 6f72 742f 7072 6f66 696c  secimport/profil
-00002b60: 6573 2f74 7261 6365 2e62 7427 2c20 272d  es/trace.bt', '-
-00002b70: 6327 2c20 272f 776f 726b 7370 6163 652f  c', '/workspace/
-00002b80: 5079 7468 6f6e 2d33 2e31 302e 302f 7079  Python-3.10.0/py
-00002b90: 7468 6f6e 272c 2027 2d6f 272c 2027 7472  thon', '-o', 'tr
-00002ba0: 6163 652e 6c6f 6727 5d0a 0a20 2020 2020  ace.log']..     
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2050 7265 7373 2043 5452 4c2b 4420     Press CTRL+D 
-00002bd0: 746f 2073 746f 7020 7468 6520 7472 6163  to stop the trac
-00002be0: 653b 0a0a 5079 7468 6f6e 2033 2e31 302e  e;..Python 3.10.
-00002bf0: 3020 2864 6566 6175 6c74 2c20 4d61 7220  0 (default, Mar 
-00002c00: 3139 2032 3032 332c 2030 383a 3334 3a34  19 2023, 08:34:4
-00002c10: 3629 205b 4743 4320 392e 342e 305d 206f  6) [GCC 9.4.0] o
-00002c20: 6e20 6c69 6e75 780a 5479 7065 2022 6865  n linux.Type "he
-00002c30: 6c70 222c 2022 636f 7079 7269 6768 7422  lp", "copyright"
-00002c40: 2c20 2263 7265 6469 7473 2220 6f72 2022  , "credits" or "
-00002c50: 6c69 6365 6e73 6522 2066 6f72 206d 6f72  license" for mor
-00002c60: 6520 696e 666f 726d 6174 696f 6e2e 0a3e  e information..>
-00002c70: 3e3e 2069 6d70 6f72 7420 7468 6973 0a3e  >> import this.>
-00002c80: 3e3e 0a20 5452 4143 494e 4720 444f 4e45  >>. TRACING DONE
-00002c90: 3b0a 203e 3e3e 2073 6563 696d 706f 7274  ;. >>> secimport
-00002ca0: 2062 7569 6c64 0a0a 5345 4349 4d50 4f52   build..SECIMPOR
-00002cb0: 5420 434f 4d50 494c 494e 472e 2e2e 0a0a  T COMPILING.....
-00002cc0: 4352 4541 5445 4420 4a53 4f4e 2054 454d  CREATED JSON TEM
-00002cd0: 504c 4154 453a 2020 706f 6c69 6379 2e6a  PLATE:  policy.j
-00002ce0: 736f 6e0a 4352 4541 5445 4420 5941 4d4c  son.CREATED YAML
-00002cf0: 2054 454d 504c 4154 453a 2020 706f 6c69   TEMPLATE:  poli
-00002d00: 6379 2e79 616d 6c0a 636f 6d70 696c 696e  cy.yaml.compilin
-00002d10: 6720 7465 6d70 6c61 7465 2070 6f6c 6963  g template polic
-00002d20: 792e 7961 6d6c 0a44 5452 4143 4520 5341  y.yaml.DTRACE SA
-00002d30: 4e44 424f 583a 2020 7361 6e64 626f 782e  NDBOX:  sandbox.
-00002d40: 640a 4250 4654 5243 4520 5341 4e44 424f  d.BPFTRCE SANDBO
-00002d50: 583a 2020 7361 6e64 626f 782e 6274 0a60  X:  sandbox.bt.`
-00002d60: 6060 0a0a 4e6f 772c 206c 6574 2773 2072  ``..Now, let's r
-00002d70: 756e 2074 6865 2073 616e 6462 6f78 210a  un the sandbox!.
-00002d80: 6060 6070 7974 686f 6e0a 2d20 5275 6e20  ```python.- Run 
-00002d90: 7468 6520 7361 6d65 2063 6f6d 6d61 6e64  the same command
-00002da0: 7320 6173 2062 6566 6f72 652c 2074 6865  s as before, the
-00002db0: 7920 7368 6f75 6c64 2072 756e 2077 6974  y should run wit
-00002dc0: 686f 7574 2061 6e79 2070 726f 626c 656d  hout any problem
-00002dd0: 3b2e 0a2d 2044 6f20 736f 6d65 7468 696e  ;..- Do somethin
-00002de0: 6720 6e65 7720 696e 2074 6865 2073 6865  g new in the she
-00002df0: 6c6c 3b20 652e 673a 2020 203e 3e3e 205f  ll; e.g:   >>> _
-00002e00: 5f69 6d70 6f72 745f 5f28 226f 7322 292e  _import__("os").
-00002e10: 7379 7374 656d 2822 7073 2229 0a0a 2020  system("ps")..  
-00002e20: 2020 2020 2020 4f4b 3f20 2879 293a 2079        OK? (y): y
-00002e30: 0a20 3e3e 3e20 7365 6369 6d70 6f72 7420  . >>> secimport 
-00002e40: 7275 6e0a 2052 554e 4e49 4e47 2053 414e  run. RUNNING SAN
-00002e50: 4442 4f58 2e2e 2e20 5b27 2e2f 7361 6e64  DBOX... ['./sand
-00002e60: 626f 782e 6274 272c 2027 2d2d 756e 7361  box.bt', '--unsa
-00002e70: 6665 272c 2027 202d 6320 272c 2027 2f77  fe', ' -c ', '/w
-00002e80: 6f72 6b73 7061 6365 2f50 7974 686f 6e2d  orkspace/Python-
-00002e90: 332e 3130 2e30 2f70 7974 686f 6e27 5d0a  3.10.0/python'].
-00002ea0: 4174 7461 6368 696e 6720 3520 7072 6f62  Attaching 5 prob
-00002eb0: 6573 2e2e 2e0a 5245 4749 5354 4552 494e  es....REGISTERIN
-00002ec0: 4720 5359 5343 414c 4c53 2e2e 2e0a 5354  G SYSCALLS....ST
-00002ed0: 4152 5445 440a 5079 7468 6f6e 2033 2e31  ARTED.Python 3.1
-00002ee0: 302e 3020 2864 6566 6175 6c74 2c20 4d61  0.0 (default, Ma
-00002ef0: 7220 3139 2032 3032 332c 2030 383a 3334  r 19 2023, 08:34
-00002f00: 3a34 3629 205b 4743 4320 392e 342e 305d  :46) [GCC 9.4.0]
-00002f10: 206f 6e20 6c69 6e75 780a 5479 7065 2022   on linux.Type "
-00002f20: 6865 6c70 222c 2022 636f 7079 7269 6768  help", "copyrigh
-00002f30: 7422 2c20 2263 7265 6469 7473 2220 6f72  t", "credits" or
-00002f40: 2022 6c69 6365 6e73 6522 2066 6f72 206d   "license" for m
-00002f50: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-00002f60: 0a3e 3e3e 2069 6d70 6f72 7420 7468 6973  .>>> import this
-00002f70: 0a3e 3e3e 2069 6d70 6f72 7420 6f73 0a5b  .>>> import os.[
-00002f80: 5345 4349 4d50 4f52 5420 5649 4f4c 4154  SECIMPORT VIOLAT
-00002f90: 494f 4e5d 3a20 3c73 7464 696e 3e20 6361  ION]: <stdin> ca
-00002fa0: 6c6c 6564 2073 7973 6361 6c6c 2069 6f63  lled syscall ioc
-00002fb0: 746c 2061 7420 6465 7074 6820 300a 5b53  tl at depth 0.[S
-00002fc0: 4543 494d 504f 5254 2056 494f 4c41 5449  ECIMPORT VIOLATI
-00002fd0: 4f4e 5d3a 203c 7374 6469 6e3e 2063 616c  ON]: <stdin> cal
-00002fe0: 6c65 6420 7379 7363 616c 6c20 696f 6374  led syscall ioct
-00002ff0: 6c20 6174 2064 6570 7468 2030 0a60 6060  l at depth 0.```
-00003000: 0a0a 466f 7220 6d6f 7265 2064 6574 6169  ..For more detai
-00003010: 6c65 6420 7573 6167 6520 696e 7374 7275  led usage instru
-00003020: 6374 696f 6e73 2c20 7365 6520 7468 6520  ctions, see the 
-00003030: 5b43 6f6d 6d61 6e64 2d4c 696e 6520 5573  [Command-Line Us
-00003040: 6167 655d 2868 7474 7073 3a2f 2f67 6974  age](https://git
-00003050: 6875 622e 636f 6d2f 6176 696c 756d 2f73  hub.com/avilum/s
-00003060: 6563 696d 706f 7274 2f77 696b 692f 436f  ecimport/wiki/Co
-00003070: 6d6d 616e 642d 4c69 6e65 2d55 7361 6765  mmand-Line-Usage
-00003080: 2920 7061 6765 2e0a 0a23 2320 6e73 6a61  ) page...## nsja
-00003090: 696c 2073 7570 706f 7274 2028 7365 6363  il support (secc
-000030a0: 6f6d 7029 0a42 6573 6964 6520 7468 6520  omp).Beside the 
-000030b0: 7361 6e64 626f 7820 7468 6174 2073 6563  sandbox that sec
-000030c0: 696d 706f 7274 2062 7569 6c64 732c 203c  import builds, <
-000030d0: 6272 3e0a 5468 6520 6073 6563 696d 706f  br>.The `secimpo
-000030e0: 7274 2062 7569 6c64 6020 636f 6d6d 616e  rt build` comman
-000030f0: 6420 6372 6561 7465 7320 616e 203c 6120  d creates an <a 
-00003100: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00003110: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
-00003120: 6e73 6a61 696c 223e 6e73 6a61 696c 3c2f  nsjail">nsjail</
-00003130: 613e 2073 616e 6462 6f78 2077 6974 6820  a> sandbox with 
-00003140: 7365 6363 6f6d 7020 7072 6f66 696c 6520  seccomp profile 
-00003150: 666f 7220 796f 7572 2074 7261 6365 6420  for your traced 
-00003160: 636f 6465 2e3c 6272 3e20 606e 736a 6169  code.<br> `nsjai
-00003170: 6c60 2065 6e61 626c 6573 206e 616d 6573  l` enables names
-00003180: 7061 6365 2073 616e 6462 6f78 696e 6720  pace sandboxing 
-00003190: 7769 7468 2073 6563 636f 6d70 206f 6e20  with seccomp on 
-000031a0: 6c69 6e75 783c 6272 3e0a 6073 6563 696d  linux<br>.`secim
-000031b0: 706f 7274 6020 6175 746f 6d61 7469 6361  port` automatica
-000031c0: 6c6c 7920 6765 6e65 7261 7465 7320 7365  lly generates se
-000031d0: 6363 6f6d 7020 7072 6f66 696c 6573 2074  ccomp profiles t
-000031e0: 6f20 7573 6520 7769 7468 2060 6e73 6a61  o use with `nsja
-000031f0: 696c 6020 6173 2065 7865 6375 7461 626c  il` as executabl
-00003200: 6520 6261 7368 2073 6372 6970 742e 0a49  e bash script..I
-00003210: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-00003220: 206c 696d 6974 2074 6865 2073 7973 6361   limit the sysca
-00003230: 6c6c 7320 6f66 2074 6865 2065 6e74 6972  lls of the entir
-00003240: 6520 7079 7468 6f6e 2070 726f 6365 7373  e python process
-00003250: 2c20 6173 2061 6e6f 7468 6572 206c 6179  , as another lay
-00003260: 6572 206f 6620 6465 6665 6e63 652e 0a0a  er of defence...
-00003270: 2323 2050 7974 686f 6e20 4150 490a 0a49  ## Python API..I
-00003280: 6e73 7465 6164 206f 6620 434c 492c 2079  nstead of CLI, y
-00003290: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
-000032a0: 6073 6563 696d 706f 7274 6020 6279 2072  `secimport` by r
-000032b0: 6570 6c61 6369 6e67 2022 6069 6d70 6f72  eplacing "`impor
-000032c0: 7460 2220 7769 7468 2022 6073 6563 696d  t`" with "`secim
-000032d0: 706f 7274 2e73 6563 7572 655f 696d 706f  port.secure_impo
-000032e0: 7274 6022 2066 6f72 2073 656c 6563 7465  rt`" for selecte
-000032f0: 6420 6d6f 6475 6c65 732e 2053 6565 2074  d modules. See t
-00003300: 6865 205b 5079 7468 6f6e 2049 6d70 6f72  he [Python Impor
-00003310: 7473 5d28 6578 616d 706c 6573 2f70 7974  ts](examples/pyt
-00003320: 686f 6e5f 696d 706f 7274 732f 2920 6578  hon_imports/) ex
-00003330: 616d 706c 6520 666f 7220 6d6f 7265 2064  ample for more d
-00003340: 6574 6169 6c73 2e0a 0a23 2320 446f 636b  etails...## Dock
-00003350: 6572 0a54 6865 2071 7569 636b 6573 7420  er.The quickest 
-00003360: 7761 7920 746f 2065 7661 6c75 6174 6520  way to evaluate 
-00003370: 6073 6563 696d 706f 7274 6020 6973 2074  `secimport` is t
-00003380: 6f20 7573 6520 6f75 7220 5b44 6f63 6b65  o use our [Docke
-00003390: 7220 636f 6e74 6169 6e65 725d 2864 6f63  r container](doc
-000033a0: 6b65 722f 5245 4144 4d45 2e6d 6429 2c20  ker/README.md), 
-000033b0: 7768 6963 6820 696e 636c 7564 6573 2060  which includes `
-000033c0: 6270 6674 7261 6365 6020 2860 6562 7066  bpftrace` (`ebpf
-000033d0: 6029 2061 6e64 206f 7468 6572 2070 6c75  `) and other plu
-000033e0: 672d 616e 642d 706c 6179 2065 7861 6d70  g-and-play examp
-000033f0: 6c65 732e 0a0a 0a23 2320 4578 616d 706c  les....## Exampl
-00003400: 6573 0a0a 5468 6520 5b53 616e 6462 6f78  es..The [Sandbox
-00003410: 2045 7861 6d70 6c65 735d 2868 7474 7073   Examples](https
-00003420: 3a2f 2f67 6974 6875 622e 636f 6d2f 6176  ://github.com/av
-00003430: 696c 756d 2f73 6563 696d 706f 7274 2f77  ilum/secimport/w
-00003440: 696b 692f 5361 6e64 626f 782d 4578 616d  iki/Sandbox-Exam
-00003450: 706c 6573 2920 7061 6765 2063 6f6e 7461  ples) page conta
-00003460: 696e 7320 6261 7369 6320 616e 6420 6164  ins basic and ad
-00003470: 7661 6e63 6564 2072 6561 6c2d 776f 726c  vanced real-worl
-00003480: 6420 6578 616d 706c 6573 2e0a 0a23 2320  d examples...## 
-00003490: 436f 6e74 7269 6275 7469 6e67 0a0a 466f  Contributing..Fo
-000034a0: 7220 696e 666f 726d 6174 696f 6e20 6f6e  r information on
-000034b0: 2068 6f77 2074 6f20 636f 6e74 7269 6275   how to contribu
-000034c0: 7465 2074 6f20 6073 6563 696d 706f 7274  te to `secimport
-000034d0: 602c 2073 6565 2074 6865 205b 436f 6e74  `, see the [Cont
-000034e0: 7269 6275 7469 6e67 5d28 6874 7470 733a  ributing](https:
-000034f0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
-00003500: 6c75 6d2f 7365 6369 6d70 6f72 742f 626c  lum/secimport/bl
-00003510: 6f62 2f6d 6173 7465 722f 646f 6373 2f43  ob/master/docs/C
-00003520: 4f4e 5452 4942 5554 494e 472e 6d64 2920  ONTRIBUTING.md) 
-00003530: 6775 6964 652e 0a0a 2323 2052 6f61 646d  guide...## Roadm
-00003540: 6170 0a0a 5365 6520 7468 6520 5b52 6f61  ap..See the [Roa
-00003550: 646d 6170 5d28 6874 7470 733a 2f2f 6769  dmap](https://gi
-00003560: 7468 7562 2e63 6f6d 2f61 7669 6c75 6d2f  thub.com/avilum/
-00003570: 7365 6369 6d70 6f72 742f 626c 6f62 2f6d  secimport/blob/m
-00003580: 6173 7465 722f 646f 6373 2f52 4f41 444d  aster/docs/ROADM
-00003590: 4150 2e6d 6429 2066 6f72 2074 6865 2070  AP.md) for the p
-000035a0: 6c61 6e6e 6564 2066 6561 7475 7265 7320  lanned features 
-000035b0: 616e 6420 6465 7665 6c6f 706d 656e 7420  and development 
-000035c0: 6d69 6c65 7374 6f6e 6573 2e0a 0a23 2320  milestones...## 
-000035d0: 4368 616e 6765 6c6f 670a 0a53 6565 2074  Changelog..See t
-000035e0: 6865 205b 4368 616e 6765 6c6f 675d 2868  he [Changelog](h
-000035f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003600: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
-00003610: 7274 2f62 6c6f 622f 6d61 7374 6572 2f64  rt/blob/master/d
-00003620: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
-00003630: 2920 666f 7220 6465 7665 6c6f 706d 656e  ) for developmen
-00003640: 7420 7072 6f67 7265 7373 2061 6e64 2065  t progress and e
-00003650: 7869 7374 696e 6720 6665 6174 7572 6573  xisting features
-00003660: 2e0a 0a                                  ...
+00000260: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
+00000270: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000290: 3a3a 2033 2e31 320a 5265 7175 6972 6573  :: 3.12.Requires
+000002a0: 2d44 6973 743a 2050 7959 414d 4c20 283e  -Dist: PyYAML (>
+000002b0: 3d36 2e30 2c3c 372e 3029 0a52 6571 7569  =6.0,<7.0).Requi
+000002c0: 7265 732d 4469 7374 3a20 6669 7265 2028  res-Dist: fire (
+000002d0: 3e3d 302e 342c 3c30 2e36 290a 4465 7363  >=0.4,<0.6).Desc
+000002e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000300: 6f77 6e0a 0a3c 212d 2d20 5354 4152 5420  own..<!-- START 
+00000310: 646f 6374 6f63 2067 656e 6572 6174 6564  doctoc generated
+00000320: 2054 4f43 2070 6c65 6173 6520 6b65 6570   TOC please keep
+00000330: 2063 6f6d 6d65 6e74 2068 6572 6520 746f   comment here to
+00000340: 2061 6c6c 6f77 2061 7574 6f20 7570 6461   allow auto upda
+00000350: 7465 202d 2d3e 0a3c 212d 2d20 444f 4e27  te -->.<!-- DON'
+00000360: 5420 4544 4954 2054 4849 5320 5345 4354  T EDIT THIS SECT
+00000370: 494f 4e2c 2049 4e53 5445 4144 2052 452d  ION, INSTEAD RE-
+00000380: 5255 4e20 646f 6374 6f63 2054 4f20 5550  RUN doctoc TO UP
+00000390: 4441 5445 202d 2d3e 0a2a 2a54 6162 6c65  DATE -->.**Table
+000003a0: 206f 6620 436f 6e74 656e 7473 2a2a 2020   of Contents**  
+000003b0: 2a67 656e 6572 6174 6564 2077 6974 6820  *generated with 
+000003c0: 5b44 6f63 546f 635d 2868 7474 7073 3a2f  [DocToc](https:/
+000003d0: 2f67 6974 6875 622e 636f 6d2f 7468 6c6f  /github.com/thlo
+000003e0: 7265 6e7a 2f64 6f63 746f 6329 2a0a 0a2d  renz/doctoc)*..-
+000003f0: 205b 7365 6369 6d70 6f72 745d 2823 7365   [secimport](#se
+00000400: 6369 6d70 6f72 7429 0a20 202d 205b 5468  cimport).  - [Th
+00000410: 6520 5461 696c 6f72 2d4d 6164 6520 5361  e Tailor-Made Sa
+00000420: 6e64 626f 7820 666f 7220 596f 7572 2041  ndbox for Your A
+00000430: 7070 6c69 6361 7469 6f6e 5d28 2374 6865  pplication](#the
+00000440: 2d74 6169 6c6f 722d 6d61 6465 2d73 616e  -tailor-made-san
+00000450: 6462 6f78 2d66 6f72 2d79 6f75 722d 6170  dbox-for-your-ap
+00000460: 706c 6963 6174 696f 6e29 0a20 2020 202d  plication).    -
+00000470: 205b 5468 6520 7072 6f62 6c65 6d5d 2823   [The problem](#
+00000480: 7468 652d 7072 6f62 6c65 6d29 0a20 2020  the-problem).   
+00000490: 202d 205b 5468 6520 736f 6c75 7469 6f6e   - [The solution
+000004a0: 5d28 2374 6865 2d73 6f6c 7574 696f 6e29  ](#the-solution)
+000004b0: 0a20 202d 205b 496e 7374 616c 6c61 7469  .  - [Installati
+000004c0: 6f6e 5d28 2369 6e73 7461 6c6c 6174 696f  on](#installatio
+000004d0: 6e29 0a20 202d 205b 5769 7468 2044 6f63  n).  - [With Doc
+000004e0: 6b65 725d 2823 7769 7468 2d64 6f63 6b65  ker](#with-docke
+000004f0: 7229 0a20 202d 205b 5769 7468 6f75 7420  r).  - [Without 
+00000500: 446f 636b 6572 5d28 2377 6974 686f 7574  Docker](#without
+00000510: 2d64 6f63 6b65 7229 0a20 202d 205b 5573  -docker).  - [Us
+00000520: 6167 655d 2823 7573 6167 6529 0a20 202d  age](#usage).  -
+00000530: 205b 5374 6f70 206f 6e20 7669 6f6c 6174   [Stop on violat
+00000540: 696f 6e5d 2823 7374 6f70 2d6f 6e2d 7669  ion](#stop-on-vi
+00000550: 6f6c 6174 696f 6e29 0a20 202d 205b 4b69  olation).  - [Ki
+00000560: 6c6c 206f 6e20 7669 6f6c 6174 696f 6e5d  ll on violation]
+00000570: 2823 6b69 6c6c 2d6f 6e2d 7669 6f6c 6174  (#kill-on-violat
+00000580: 696f 6e29 0a20 202d 205b 4479 6e61 6d69  ion).  - [Dynami
+00000590: 6320 7072 6f66 696c 696e 6720 2d20 7472  c profiling - tr
+000005a0: 6163 652c 2062 7569 6c64 2073 616e 6462  ace, build sandb
+000005b0: 6f78 2c20 7275 6e2e 5d28 2364 796e 616d  ox, run.](#dynam
+000005c0: 6963 2d70 726f 6669 6c69 6e67 2d2d 2d74  ic-profiling---t
+000005d0: 7261 6365 2d62 7569 6c64 2d73 616e 6462  race-build-sandb
+000005e0: 6f78 2d72 756e 290a 2020 2d20 5b6e 736a  ox-run).  - [nsj
+000005f0: 6169 6c20 7375 7070 6f72 7420 2873 6563  ail support (sec
+00000600: 636f 6d70 295d 2823 6e73 6a61 696c 2d73  comp)](#nsjail-s
+00000610: 7570 706f 7274 2d73 6563 636f 6d70 290a  upport-seccomp).
+00000620: 2020 2d20 5b50 7974 686f 6e20 4150 495d    - [Python API]
+00000630: 2823 7079 7468 6f6e 2d61 7069 290a 2020  (#python-api).  
+00000640: 2d20 5b44 6f63 6b65 725d 2823 646f 636b  - [Docker](#dock
+00000650: 6572 290a 2020 2d20 5b45 7861 6d70 6c65  er).  - [Example
+00000660: 735d 2823 6578 616d 706c 6573 290a 2020  s](#examples).  
+00000670: 2d20 5b43 6f6e 7472 6962 7574 696e 675d  - [Contributing]
+00000680: 2823 636f 6e74 7269 6275 7469 6e67 290a  (#contributing).
+00000690: 2020 2d20 5b52 6f61 646d 6170 5d28 2372    - [Roadmap](#r
+000006a0: 6f61 646d 6170 290a 2020 2d20 5b43 6861  oadmap).  - [Cha
+000006b0: 6e67 656c 6f67 5d28 2363 6861 6e67 656c  ngelog](#changel
+000006c0: 6f67 290a 0a3c 212d 2d20 454e 4420 646f  og)..<!-- END do
+000006d0: 6374 6f63 2067 656e 6572 6174 6564 2054  ctoc generated T
+000006e0: 4f43 2070 6c65 6173 6520 6b65 6570 2063  OC please keep c
+000006f0: 6f6d 6d65 6e74 2068 6572 6520 746f 2061  omment here to a
+00000700: 6c6c 6f77 2061 7574 6f20 7570 6461 7465  llow auto update
+00000710: 202d 2d3e 0a0a 2320 7365 6369 6d70 6f72   -->..# secimpor
+00000720: 740a 5b21 5b55 706c 6f61 6420 5079 7468  t.[![Upload Pyth
+00000730: 6f6e 2050 6163 6b61 6765 5d28 6874 7470  on Package](http
+00000740: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000750: 7669 6c75 6d2f 7365 6369 6d70 6f72 742f  vilum/secimport/
+00000760: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000770: 732f 7079 7468 6f6e 2d70 7562 6c69 7368  s/python-publish
+00000780: 2e79 6d6c 2f62 6164 6765 2e73 7667 295d  .yml/badge.svg)]
+00000790: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000007a0: 636f 6d2f 6176 696c 756d 2f73 6563 696d  com/avilum/secim
+000007b0: 706f 7274 2f61 6374 696f 6e73 2f77 6f72  port/actions/wor
+000007c0: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7075  kflows/python-pu
+000007d0: 626c 6973 682e 796d 6c29 0a21 5b5d 2868  blish.yml).![](h
+000007e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000007f0: 6473 2e69 6f2f 6261 6467 652f 5465 7374  ds.io/badge/Test
+00000800: 5f43 6f76 6572 6167 652d 3930 252d 626c  _Coverage-90%-bl
+00000810: 7565 290a 0a0a 2323 2054 6865 2054 6169  ue)...## The Tai
+00000820: 6c6f 722d 4d61 6465 2053 616e 6462 6f78  lor-Made Sandbox
+00000830: 2066 6f72 2059 6f75 7220 4170 706c 6963   for Your Applic
+00000840: 6174 696f 6e0a 7365 6369 6d70 6f72 7420  ation.secimport 
+00000850: 6973 2070 726f 6475 6374 696f 6e2d 6f72  is production-or
+00000860: 6965 6e74 6564 2073 616e 6462 6f78 2074  iented sandbox t
+00000870: 6f6f 6c6b 6974 2e3c 6272 3e0a 4974 2074  oolkit.<br>.It t
+00000880: 7261 6365 7320 796f 7572 2063 6f64 652c  races your code,
+00000890: 2061 6e64 2072 756e 7320 616e 2065 7865   and runs an exe
+000008a0: 6375 7461 626c 6520 7468 6174 2061 6c6c  cutable that all
+000008b0: 6f77 7320 6f6e 6c79 2074 6865 2073 616d  ows only the sam
+000008c0: 6520 7379 7363 616c 6c73 2c20 7065 7220  e syscalls, per 
+000008d0: 6d6f 6475 6c65 2e0a 0a54 6563 686e 6963  module...Technic
+000008e0: 616c 2042 6c6f 6773 2028 4672 6565 2052  al Blogs (Free R
+000008f0: 6561 6469 6e67 293a 0a31 2e20 3c61 2068  eading):.1. <a h
+00000900: 7265 663d 2268 7474 7073 3a2f 2f69 6e66  ref="https://inf
+00000910: 6f73 6563 7772 6974 6575 7073 2e63 6f6d  osecwriteups.com
+00000920: 2f73 616e 6462 6f78 696e 672d 7079 7468  /sandboxing-pyth
+00000930: 6f6e 2d6d 6f64 756c 6573 2d69 6e2d 796f  on-modules-in-yo
+00000940: 7572 2d63 6f64 652d 3165 3539 3064 3731  ur-code-1e590d71
+00000950: 6663 3236 3f73 6f75 7263 653d 6672 6965  fc26?source=frie
+00000960: 6e64 735f 6c69 6e6b 2673 6b3d 3565 3961  nds_link&sk=5e9a
+00000970: 3266 6134 6434 3932 3161 6630 6563 3934  2fa4d4921af0ec94
+00000980: 6631 3735 6637 6565 3439 6639 223e 7365  f175f7ee49f9">se
+00000990: 6369 6d70 6f72 7420 2b20 4474 7261 6365  cimport + Dtrace
+000009a0: 3c2f 613e 0a32 2e20 3c61 2068 7265 663d  </a>.2. <a href=
+000009b0: 2268 7474 7073 3a2f 2f69 6e66 6f73 6563  "https://infosec
+000009c0: 7772 6974 6575 7073 2e63 6f6d 2f73 6563  writeups.com/sec
+000009d0: 7572 696e 672d 7079 746f 7263 682d 6d6f  uring-pytorch-mo
+000009e0: 6465 6c73 2d77 6974 682d 6562 7066 2d37  dels-with-ebpf-7
+000009f0: 6637 3537 3332 6238 3432 643f 736f 7572  f75732b842d?sour
+00000a00: 6365 3d66 7269 656e 6473 5f6c 696e 6b26  ce=friends_link&
+00000a10: 736b 3d31 3464 3864 6234 3033 6161 6636  sk=14d8db403aaf6
+00000a20: 3637 3234 6138 6136 3962 3464 6561 3234  6724a8a69b4dea24
+00000a30: 6531 3222 3e73 6563 696d 7072 7420 2b20  e12">secimprt + 
+00000a40: 6542 5046 202b 2050 7954 6f72 6368 3c2f  eBPF + PyTorch</
+00000a50: 613e 0a33 2e20 3c61 2068 7265 663d 2268  a>.3. <a href="h
+00000a60: 7474 7073 3a2f 2f61 7669 2d6c 756d 656c  ttps://avi-lumel
+00000a70: 736b 792e 6d65 6469 756d 2e63 6f6d 2f73  sky.medium.com/s
+00000a80: 6563 7572 652d 6661 7374 6170 692d 7769  ecure-fastapi-wi
+00000a90: 7468 2d65 6270 662d 3732 3464 3461 6566  th-ebpf-724d4aef
+00000aa0: 3864 3965 3f73 6f75 7263 653d 6672 6965  8d9e?source=frie
+00000ab0: 6e64 735f 6c69 6e6b 2673 6b3d 6230 3161  nds_link&sk=b01a
+00000ac0: 3662 3937 6566 3039 3030 3362 3533 6364  6b97ef09003b53cd
+00000ad0: 3532 6334 3739 3031 3762 3033 223e 7365  52c479017b03">se
+00000ae0: 6369 6d70 6f72 7420 2b20 6542 5046 202b  cimport + eBPF +
+00000af0: 2046 6173 7441 5049 203c 2f61 3e0a 0a23   FastAPI </a>..#
+00000b00: 2323 2054 6865 2070 726f 626c 656d 0a54  ## The problem.T
+00000b10: 7261 6469 7469 6f6e 616c 2074 6f6f 6c73  raditional tools
+00000b20: 206c 696b 6520 7365 6363 6f6d 7020 6f72   like seccomp or
+00000b30: 2041 7070 4172 6d6f 7220 656e 666f 7263   AppArmor enforc
+00000b40: 6520 7379 7363 616c 6c73 2066 6f72 2074  e syscalls for t
+00000b50: 6865 2065 6e74 6972 6520 7072 6f63 6573  he entire proces
+00000b60: 732e 3c62 723e 536f 6d65 7468 696e 6720  s.<br>Something 
+00000b70: 6c69 6b65 2060 616c 6c6f 7765 645f 7379  like `allowed_sy
+00000b80: 7363 616c 6c73 3d5b 2272 6561 6422 2c22  scalls=["read","
+00000b90: 6f70 656e 6174 222c 2262 696e 6422 2c22  openat","bind","
+00000ba0: 7772 6974 6522 5d60 2c20 7768 6963 6820  write"]`, which 
+00000bb0: 6973 2067 7265 6174 2c20 6275 7420 6e6f  is great, but no
+00000bc0: 7420 656e 6f75 6768 2066 6f72 2070 7974  t enough for pyt
+00000bd0: 686f 6e27 7320 6174 7461 636b 2073 7572  hon's attack sur
+00000be0: 6661 6365 2e3c 6272 3e0a 0a23 2323 2054  face.<br>..### T
+00000bf0: 6865 2073 6f6c 7574 696f 6e0a 6073 6563  he solution.`sec
+00000c00: 696d 706f 7274 6020 6973 2061 626c 6520  import` is able 
+00000c10: 746f 2074 7261 6365 2077 6869 6368 2073  to trace which s
+00000c20: 7973 6361 6c6c 7320 6561 6368 206d 6f64  yscalls each mod
+00000c30: 756c 6520 696e 2079 6f75 7220 636f 6465  ule in your code
+00000c40: 2075 7365 7320 2862 7920 7061 636b 6167   uses (by packag
+00000c50: 6520 6e61 6d65 292e 3c62 723e 0a41 6674  e name).<br>.Aft
+00000c60: 6572 2074 7261 6369 6e67 2c20 7365 6369  er tracing, seci
+00000c70: 6d70 6f72 7420 6372 6561 7465 7320 6120  mport creates a 
+00000c80: 4a53 4f4e 2f59 414d 4c20 706f 6c69 6379  JSON/YAML policy
+00000c90: 2066 6f72 2079 6f75 7220 636f 6465 2e20   for your code. 
+00000ca0: 4974 2063 6f6d 7069 6c65 7320 6974 2069  It compiles it i
+00000cb0: 6e74 6f20 6120 6869 6768 2d70 6572 666f  nto a high-perfo
+00000cc0: 726d 616e 6365 2065 4250 4620 696e 7374  rmance eBPF inst
+00000cd0: 7275 6d65 6e74 6174 696f 6e20 7363 7269  rumentation scri
+00000ce0: 7074 2028 736d 616c 6c65 7220 7468 656e  pt (smaller then
+00000cf0: 2035 3132 2062 7974 6573 206f 7665 7261   512 bytes overa
+00000d00: 6c6c 292c 2074 6861 7420 6c6f 6f6b 7320  ll), that looks 
+00000d10: 6c69 6b65 203c 613e 7468 6973 3c2f 613e  like <a>this</a>
+00000d20: 2e0a 6060 600a 6d6f 6475 6c65 733a 0a20  ..```.modules:. 
+00000d30: 2072 6571 7565 7374 733a 0a20 2020 2064   requests:.    d
+00000d40: 6573 7472 7563 7469 7665 3a20 7472 7565  estructive: true
+00000d50: 2020 2020 2023 2077 6865 6e20 7472 7565       # when true
+00000d60: 2c20 7365 6369 6d70 6f72 7420 7769 6c6c  , secimport will
+00000d70: 206b 696c 6c20 6f6e 2076 696c 6174 696f   kill on vilatio
+00000d80: 6e20 696e 7374 6561 6420 6f66 206c 6f67  n instead of log
+00000d90: 6769 6e67 2e0a 2020 2020 7379 7363 616c  ging..    syscal
+00000da0: 6c5f 616c 6c6f 776c 6973 743a 0a20 2020  l_allowlist:.   
+00000db0: 2020 202d 2066 6368 6d6f 640a 2020 2020     - fchmod.    
+00000dc0: 2020 2d20 6765 7465 6e74 726f 7079 0a20    - getentropy. 
+00000dd0: 2020 2020 202d 2067 6574 7067 7270 0a20       - getpgrp. 
+00000de0: 2020 2020 202d 2067 6574 726c 696d 6974       - getrlimit
+00000df0: 0a2e 2e2e 0a60 6060 0a59 6f75 2063 616e  .....```.You can
+00000e00: 2061 6c73 6f20 7573 6520 4a53 4f4e 2069   also use JSON i
+00000e10: 6e73 7461 6561 6420 6f66 2059 414d 4c2c  nstaead of YAML,
+00000e20: 2061 6e64 2065 7665 6e20 636f 6e66 696e   and even confin
+00000e30: 6520 6275 696c 7469 6e20 7079 7468 6f6e  e builtin python
+00000e40: 206d 6f64 756c 6573 2e3c 6272 3e0a 416e   modules.<br>.An
+00000e50: 2065 7861 6d70 6c65 2070 6f6c 6963 7920   example policy 
+00000e60: 7468 6174 2075 7365 7320 6c6f 6767 696e  that uses loggin
+00000e70: 672c 206d 756c 7469 7072 6f63 6573 7369  g, multiprocessi
+00000e80: 6e67 2c20 6f73 2061 6e64 2066 696c 6573  ng, os and files
+00000e90: 7973 7465 6d20 7769 6c6c 206c 6f6f 6b20  ystem will look 
+00000ea0: 6170 7072 6f78 696d 6174 656c 7920 6c69  approximately li
+00000eb0: 6b65 2074 6869 733a 0a60 6060 0a2e 2e2e  ke this:.```....
+00000ec0: 0a20 2020 2022 2f77 6f72 6b73 7061 6365  .    "/workspace
+00000ed0: 2f50 7974 686f 6e2d 332e 3130 2e30 2f4c  /Python-3.10.0/L
+00000ee0: 6962 2f6c 6f67 6769 6e67 2f5f 5f69 6e69  ib/logging/__ini
+00000ef0: 745f 5f2e 7079 223a 205b 0a20 2020 2020  t__.py": [.     
+00000f00: 2020 2022 2063 6c6f 636b 5f67 6574 7469     " clock_getti
+00000f10: 6d65 222c 0a20 2020 2020 2020 2022 2067  me",.        " g
+00000f20: 6574 7069 6422 2c0a 2020 2020 2020 2020  etpid",.        
+00000f30: 2220 7772 6974 6522 0a20 2020 205d 2c0a  " write".    ],.
+00000f40: 2020 2020 222f 776f 726b 7370 6163 652f      "/workspace/
+00000f50: 5079 7468 6f6e 2d33 2e31 302e 302f 4c69  Python-3.10.0/Li
+00000f60: 622f 6d75 6c74 6970 726f 6365 7373 696e  b/multiprocessin
+00000f70: 672f 7072 6f63 6573 732e 7079 223a 205b  g/process.py": [
+00000f80: 0a20 2020 2020 2020 2022 2067 6574 6377  .        " getcw
+00000f90: 6422 2c0a 2020 2020 2020 2020 2220 6765  d",.        " ge
+00000fa0: 7470 6964 222c 0a20 2020 2020 2020 2022  tpid",.        "
+00000fb0: 2067 6574 7261 6e64 6f6d 220a 2020 2020   getrandom".    
+00000fc0: 5d2c 0a20 2020 2022 2f77 6f72 6b73 7061  ],.    "/workspa
+00000fd0: 6365 2f50 7974 686f 6e2d 332e 3130 2e30  ce/Python-3.10.0
+00000fe0: 2f4c 6962 2f6d 756c 7469 7072 6f63 6573  /Lib/multiproces
+00000ff0: 7369 6e67 2f75 7469 6c2e 7079 223a 205b  sing/util.py": [
+00001000: 0a20 2020 2020 2020 2022 2070 726c 696d  .        " prlim
+00001010: 6974 3634 220a 2020 2020 5d2c 0a20 2020  it64".    ],.   
+00001020: 2022 2f77 6f72 6b73 7061 6365 2f50 7974   "/workspace/Pyt
+00001030: 686f 6e2d 332e 3130 2e30 2f4c 6962 2f6f  hon-3.10.0/Lib/o
+00001040: 732e 7079 223a 205b 0a20 2020 2020 2020  s.py": [.       
+00001050: 2022 2072 6561 6422 0a20 2020 205d 2c0a   " read".    ],.
+00001060: 2020 2020 222f 776f 726b 7370 6163 652f      "/workspace/
+00001070: 5079 7468 6f6e 2d33 2e31 302e 302f 4c69  Python-3.10.0/Li
+00001080: 622f 706c 6174 666f 726d 2e70 7922 3a20  b/platform.py": 
+00001090: 5b0a 2020 2020 2020 2020 2220 756e 616d  [.        " unam
+000010a0: 6522 0a20 2020 205d 2c0a 2020 2020 222f  e".    ],.    "/
+000010b0: 776f 726b 7370 6163 652f 5079 7468 6f6e  workspace/Python
+000010c0: 2d33 2e31 302e 302f 4c69 622f 706f 7369  -3.10.0/Lib/posi
+000010d0: 7870 6174 682e 7079 223a 205b 0a20 2020  xpath.py": [.   
+000010e0: 2020 2020 2022 2063 6c6f 7365 222c 0a20       " close",. 
+000010f0: 2020 2020 2020 2022 2066 7374 6174 222c         " fstat",
+00001100: 0a20 2020 2020 2020 2022 2067 6574 6377  .        " getcw
+00001110: 6422 2c0a 2020 2020 2020 2020 2220 6765  d",.        " ge
+00001120: 7464 656e 7473 3634 222c 0a20 2020 2020  tdents64",.     
+00001130: 2020 2022 206f 7065 6e61 7422 0a20 2020     " openat".   
+00001140: 205d 2c0a 2020 2020 222f 776f 726b 7370   ],.    "/worksp
+00001150: 6163 652f 5079 7468 6f6e 2d33 2e31 302e  ace/Python-3.10.
+00001160: 302f 4c69 622f 7261 6e64 6f6d 2e70 7922  0/Lib/random.py"
+00001170: 3a20 5b0a 2020 2020 2020 2020 2220 6765  : [.        " ge
+00001180: 7472 616e 646f 6d22 0a20 2020 205d 2c0a  trandom".    ],.
+00001190: 2e2e 2e0a 6060 600a 4974 2077 6173 2063  ....```.It was c
+000011a0: 7265 6174 6564 2062 7920 7472 6163 696e  reated by tracin
+000011b0: 6720 7468 6520 636f 6465 2e20 7365 6369  g the code. seci
+000011c0: 6d70 6f72 7420 6175 746f 6d61 7469 6361  mport automatica
+000011d0: 6c6c 7920 6669 6e64 7320 7468 6573 6520  lly finds these 
+000011e0: 7065 722d 6d6f 6475 6c65 2073 7973 6361  per-module sysca
+000011f0: 6c6c 7320 666f 7220 796f 752e 0a0a 4669  lls for you...Fi
+00001200: 6e61 6c6c 792c 2079 6f75 2063 6f6e 7665  nally, you conve
+00001210: 7274 2074 6869 7320 706f 6c69 6379 2069  rt this policy i
+00001220: 6e74 6f20 616e 2073 616e 6462 6f78 2028  nto an sandbox (
+00001230: 6542 5046 2069 6e73 7472 756d 656e 7461  eBPF instrumenta
+00001240: 7469 6f6e 2073 6372 6970 7429 2074 6f20  tion script) to 
+00001250: 7275 6e20 7468 6520 7079 7468 6f6e 2070  run the python p
+00001260: 726f 6365 7373 2069 6e20 7072 6f64 7563  rocess in produc
+00001270: 7469 6f6e 2e20 5275 6e6e 696e 6720 7468  tion. Running th
+00001280: 6520 7361 6e64 626f 7820 7769 6c6c 2065  e sandbox will e
+00001290: 6e66 6f72 6520 7079 7468 6f6e 2074 6f20  nfore python to 
+000012a0: 6f62 6579 2061 6e79 2067 6976 656e 2070  obey any given p
+000012b0: 6f6c 6963 792e 0a0a 6073 6563 696d 706f  olicy...`secimpo
+000012c0: 7274 6020 6973 2067 7265 6174 2066 6f72  rt` is great for
+000012d0: 2e2e 2e0a 2d20 5072 6576 656e 7469 6e67  ....- Preventing
+000012e0: 2043 6f64 6520 4578 6563 7574 696f 6e3a   Code Execution:
+000012f0: 2072 6564 7563 6520 7468 6520 7269 736b   reduce the risk
+00001300: 206f 6620 7375 7070 6c79 2063 6861 696e   of supply chain
+00001310: 2061 7474 6163 6b73 2e0a 2020 2d20 5472   attacks..  - Tr
+00001320: 6163 6520 7468 6520 7379 7363 616c 6c73  ace the syscalls
+00001330: 2066 6c6f 7720 6f66 2079 6f75 7220 6170   flow of your ap
+00001340: 706c 6963 6174 696f 6e20 6174 2074 6865  plication at the
+00001350: 2075 7365 722d 7370 6163 652f 6f73 2f6b   user-space/os/k
+00001360: 6572 6e65 6c20 6c65 7665 6c20 616e 6420  ernel level and 
+00001370: 7065 7220 6d6f 6475 6c65 2e0a 2020 2d20  per module..  - 
+00001380: 5275 6e20 796f 7572 2061 7070 6c69 6361  Run your applica
+00001390: 7469 6f6e 2077 6869 6c65 2065 6e66 6f72  tion while enfor
+000013a0: 6369 6e67 2073 7973 6361 6c6c 7320 7065  cing syscalls pe
+000013b0: 7220 6d6f 6475 6c65 2e0a 2020 2020 2d20  r module..    - 
+000013c0: 5570 6f6e 2076 696f 6c61 7469 6f6e 206f  Upon violation o
+000013d0: 6620 7468 6520 706f 6c69 6379 2c20 6974  f the policy, it
+000013e0: 2063 616e 206c 6f67 2c20 7374 6f70 2c20   can log, stop, 
+000013f0: 6f72 206b 696c 6c20 7468 6520 7072 6f63  or kill the proc
+00001400: 6573 732e 0a2d 2050 726f 7465 6374 2079  ess..- Protect y
+00001410: 6f75 7273 656c 6620 6672 6f6d 2052 4345  ourself from RCE
+00001420: 3a0a 2020 2d20 7365 6369 6d70 6f72 7420  :.  - secimport 
+00001430: 6d61 6b65 7320 3164 6179 2061 7474 6163  makes 1day attac
+00001440: 6b73 206c 6573 7320 6f66 2061 6e20 6973  ks less of an is
+00001450: 7375 652c 2062 6563 6175 7365 2069 7420  sue, because it 
+00001460: 7072 6576 656e 7473 2074 6865 2063 6f64  prevents the cod
+00001470: 6520 666f 726d 2072 756e 6e69 6e67 2e20  e form running. 
+00001480: 4966 2079 6f75 2061 7265 2075 7369 6e67  If you are using
+00001490: 2061 2076 756c 6e65 7261 626c 6520 7061   a vulnerable pa
+000014a0: 636b 6167 6520 616e 6420 736f 6d65 6f6e  ckage and someon
+000014b0: 6520 6578 706c 6f69 7465 6420 6974 2c20  e exploited it, 
+000014c0: 796f 7572 2070 6f6c 6963 7920 7769 6c6c  your policy will
+000014d0: 206e 6f74 2061 6c6c 6f77 2074 6869 7320   not allow this 
+000014e0: 6578 706c 6f69 7427 7320 7379 7363 616c  exploit's syscal
+000014f0: 6c73 2061 6e64 2069 7420 7769 6c6c 2062  ls and it will b
+00001500: 6520 6861 6e64 6c65 6420 6173 2079 6f75  e handled as you
+00001510: 2077 6973 682e 0a20 202d 2041 766f 6964   wish..  - Avoid
+00001520: 2069 6e63 6964 656e 7473 206c 696b 6520   incidents like 
+00001530: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001540: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00001550: 672f 7769 6b69 2f4c 6f67 3453 6865 6c6c  g/wiki/Log4Shell
+00001560: 223e 6c6f 6734 7368 656c 6c3c 2f61 3e2e  ">log4shell</a>.
+00001570: 2041 206c 6f67 6769 6e67 206c 6962 7261   A logging libra
+00001580: 7279 2072 6571 7569 7265 7320 7665 7279  ry requires very
+00001590: 2066 6577 2073 7973 6361 6c6c 732c 2061   few syscalls, a
+000015a0: 6e64 2069 7420 7368 6f75 6c64 206e 6576  nd it should nev
+000015b0: 6572 2072 756e 2063 6f6d 6d61 6e64 2075  er run command u
+000015c0: 7369 6e67 2066 6f72 6b2c 2065 7865 6376  sing fork, execv
+000015d0: 6520 6f72 2073 7061 776e 2e0a 2020 2020  e or spawn..    
+000015e0: 2d20 5468 6520 7379 7363 616c 6c73 2074  - The syscalls t
+000015f0: 6861 7420 2266 6173 7461 7069 222c 2022  hat "fastapi", "
+00001600: 6e75 6d70 7922 206f 7220 2272 6571 7565  numpy" or "reque
+00001610: 7374 7322 2075 7365 2061 7265 2076 6572  sts" use are ver
+00001620: 7920 6469 6666 6572 656e 742e 0a2d 204c  y different..- L
+00001630: 6f61 6420 4149 204d 6f64 656c 7320 6672  oad AI Models fr
+00001640: 6f6d 2049 6e73 6563 7572 6520 536f 7572  om Insecure Sour
+00001650: 6365 730a 2020 2d20 4d6f 6465 6c73 2066  ces.  - Models f
+00001660: 726f 6d20 756e 7361 6665 2073 6f75 7263  rom unsafe sourc
+00001670: 6520 2868 7567 6769 6e67 6661 6365 2c20  e (huggingface, 
+00001680: 746f 7263 6820 6875 622c 2061 6e64 2070  torch hub, and p
+00001690: 7974 6f72 6368 2070 6963 6b6c 6564 206d  ytorch pickled m
+000016a0: 6f64 656c 7329 2063 616e 2062 6520 6c69  odels) can be li
+000016b0: 6d69 7465 6420 746f 2072 756e 206f 6e6c  mited to run onl
+000016c0: 7920 6120 7365 7420 6f66 2073 7973 6361  y a set of sysca
+000016d0: 6c6c 732e 2052 4345 206c 696b 6520 2769  lls. RCE like 'i
+000016e0: 6d70 6f72 7420 6f73 3b6f 732e 7379 7374  mport os;os.syst
+000016f0: 656d 282e 2e2e 2927 2073 6f6d 6577 6865  em(...)' somewhe
+00001700: 7265 2064 6565 7020 696e 2074 6865 2063  re deep in the c
+00001710: 6f64 6520 7769 6c6c 2062 6520 6361 7463  ode will be catc
+00001720: 6865 6420 6279 2073 6563 696d 706f 7274  hed by secimport
+00001730: 2e0a 2d20 4d69 6e69 6d61 6c20 5065 7266  ..- Minimal Perf
+00001740: 6f72 6d61 6e63 6520 496d 7061 6374 0a20  ormance Impact. 
+00001750: 202d 2020 4861 7320 6e65 676c 6967 6962   -  Has negligib
+00001760: 6c65 2070 6572 666f 726d 616e 6365 2069  le performance i
+00001770: 6d70 6163 7420 616e 6420 6973 2070 726f  mpact and is pro
+00001780: 6475 6374 696f 6e2d 7265 6164 7920 7468  duction-ready th
+00001790: 616e 6b73 2074 6f20 6542 5046 2e20 4368  anks to eBPF. Ch
+000017a0: 6563 6b20 6f75 7420 7468 6520 5b50 6572  eck out the [Per
+000017b0: 666f 726d 616e 6365 5d28 6874 7470 733a  formance](https:
+000017c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7669  //github.com/avi
+000017d0: 6c75 6d2f 7365 6369 6d70 6f72 742f 7769  lum/secimport/wi
+000017e0: 6b69 2f50 6572 666f 726d 616e 6365 2d42  ki/Performance-B
+000017f0: 656e 6368 6d61 726b 7329 2062 656e 6368  enchmarks) bench
+00001800: 6d61 726b 732e 0a2d 2054 7261 6365 2077  marks..- Trace w
+00001810: 6869 6368 2073 7973 6361 6c6c 7320 6172  hich syscalls ar
+00001820: 6520 6361 6c6c 6564 2062 7920 6561 6368  e called by each
+00001830: 206d 6f64 756c 6520 696e 2079 6f75 7220   module in your 
+00001840: 636f 6465 2e0a 2020 2d20 7365 6369 6d70  code..  - secimp
+00001850: 6f72 7420 7573 6573 2055 5344 5420 2855  ort uses USDT (U
+00001860: 7365 726c 616e 6420 5374 6174 6963 616c  serland Statical
+00001870: 6c79 2044 6566 696e 6564 2054 7261 6369  ly Defined Traci
+00001880: 6e67 2920 746f 6765 7468 6572 2077 6974  ng) together wit
+00001890: 6820 6b65 726e 656c 2070 726f 6265 7320  h kernel probes 
+000018a0: 696e 2074 6865 2072 756e 7469 6d65 2075  in the runtime u
+000018b0: 7369 6e67 2065 4250 4620 6f72 2064 7472  sing eBPF or dtr
+000018c0: 6163 6520 696e 7374 7275 6d65 6e74 6174  ace instrumentat
+000018d0: 696f 6e20 7363 7269 7074 732e 0a23 2320  ion scripts..## 
+000018e0: 496e 7374 616c 6c61 7469 6f6e 0a54 6573  Installation.Tes
+000018f0: 7465 6420 6f6e 2055 6275 6e74 752c 2044  ted on Ubuntu, D
+00001900: 6562 6961 6e2c 2052 6f63 6b79 2028 4c69  ebian, Rocky (Li
+00001910: 6e75 7820 7838 362f 414d 442f 4152 4d29  nux x86/AMD/ARM)
+00001920: 2061 6e64 204d 6163 4f53 2069 6e20 2878   and MacOS in (x
+00001930: 3836 2f4d 3129 2e20 4966 2079 6f75 2072  86/M1). If you r
+00001940: 756e 206f 6e20 4d61 634f 5320 796f 7520  un on MacOS you 
+00001950: 7769 6c6c 206e 6565 6420 746f 203c 6120  will need to <a 
+00001960: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001970: 7468 7562 2e63 6f6d 2f61 7669 6c75 6d2f  thub.com/avilum/
+00001980: 7365 6369 6d70 6f72 742f 626c 6f62 2f6d  secimport/blob/m
+00001990: 6173 7465 722f 646f 6373 2f4d 4143 5f4f  aster/docs/MAC_O
+000019a0: 535f 5553 4552 532e 6d64 223e 6469 7361  S_USERS.md">disa
+000019b0: 626c 6520 5349 5020 666f 7220 6474 7261  ble SIP for dtra
+000019c0: 6365 2e20 3c2f 613e 0a0a 2323 2057 6974  ce. </a>..## Wit
+000019d0: 6820 446f 636b 6572 0a46 6f72 2071 7569  h Docker.For qui
+000019e0: 636b 6572 2065 7661 6c75 6174 696f 6e2c  cker evaluation,
+000019f0: 2077 6520 7265 636f 6d6d 656e 6420 7573   we recommend us
+00001a00: 696e 6720 7468 6520 3c61 2068 7265 663d  ing the <a href=
+00001a10: 225b 646f 6373 2f44 6f63 6b65 725d 2868  "[docs/Docker](h
+00001a20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a30: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
+00001a40: 7274 2f62 6c6f 622f 6d61 7374 6572 2f64  rt/blob/master/d
+00001a50: 6f63 6b65 722f 5245 4144 4d45 2e6d 6429  ocker/README.md)
+00001a60: 223e 5365 6369 6d70 6f72 7420 446f 636b  ">Secimport Dock
+00001a70: 6572 2049 6d61 6765 3c2f 613e 2069 6e73  er Image</a> ins
+00001a80: 7465 6164 206f 6620 7365 6c66 2d69 6e73  tead of self-ins
+00001a90: 7461 6c6c 696e 672e 3c62 723e 0a2d 2042  talling.<br>.- B
+00001aa0: 7569 6c64 2061 6e64 2072 756e 2074 6865  uild and run the
+00001ab0: 2044 6f63 6b65 7220 636f 6e74 6169 6e65   Docker containe
+00001ac0: 7220 7769 7468 2061 2063 7573 746f 6d20  r with a custom 
+00001ad0: 6b65 726e 656c 2074 6861 7420 6d61 7463  kernel that matc
+00001ae0: 6865 7320 796f 7572 2065 7869 7374 696e  hes your existin
+00001af0: 6720 4f53 206b 6572 6e65 6c20 7665 7273  g OS kernel vers
+00001b00: 696f 6e3a 0a20 2060 6060 0a20 2063 6420  ion:.  ```.  cd 
+00001b10: 646f 636b 6572 2f20 2626 202e 2f62 7569  docker/ && ./bui
+00001b20: 6c64 2e73 6820 2626 202e 2f72 756e 2e73  ld.sh && ./run.s
+00001b30: 680a 2020 6060 600a 2020 4120 7465 6d70  h.  ```.  A temp
+00001b40: 6f72 6172 7920 636f 6e74 6169 6e65 7220  orary container 
+00001b50: 7769 6c6c 2062 6520 6372 6561 7465 642c  will be created,
+00001b60: 2061 6e64 2079 6f75 2077 696c 6c20 6265   and you will be
+00001b70: 206c 6f67 6765 6420 696e 2061 7320 7468   logged in as th
+00001b80: 6520 726f 6f74 2075 7365 722e 0a0a 2323  e root user...##
+00001b90: 2057 6974 686f 7574 2044 6f63 6b65 720a   Without Docker.
+00001ba0: 312e 2049 6e73 7461 6c6c 2070 7974 686f  1. Install pytho
+00001bb0: 6e20 7769 7468 2055 5344 5420 7072 6f62  n with USDT prob
+00001bc0: 6573 2062 7920 3c61 2068 7265 663d 2268  es by <a href="h
+00001bd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001be0: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
+00001bf0: 7274 2f77 696b 692f 496e 7374 616c 6c61  rt/wiki/Installa
+00001c00: 7469 6f6e 2370 7974 686f 6e2d 696e 7465  tion#python-inte
+00001c10: 7270 7265 7465 722d 7265 7175 6972 656d  rpreter-requirem
+00001c20: 656e 7473 223e 636f 6e66 6967 7572 696e  ents">configurin
+00001c30: 6720 6974 2077 6974 6820 272d 2d64 7472  g it with '--dtr
+00001c40: 6163 6527 3c2f 613e 0a32 2e20 496e 7374  ace'</a>.2. Inst
+00001c50: 616c 6c20 6f6e 6520 6f66 2074 6865 2062  all one of the b
+00001c60: 6163 6b65 6e64 733a 203c 6120 6872 6566  ackends: <a href
+00001c70: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00001c80: 2e63 6f6d 2f61 7669 6c75 6d2f 7365 6369  .com/avilum/seci
+00001c90: 6d70 6f72 742f 7769 6b69 2f49 6e73 7461  mport/wiki/Insta
+00001ca0: 6c6c 6174 696f 6e22 3e65 4250 4620 6f72  llation">eBPF or
+00001cb0: 2044 5472 6163 653c 2f61 3e2e 0a33 2e20   DTrace</a>..3. 
+00001cc0: 496e 7374 616c 6c20 7365 6369 6d70 6f72  Install secimpor
+00001cd0: 740a 2020 2d20 496e 7374 616c 6c20 6672  t.  - Install fr
+00001ce0: 6f6d 2070 7970 690a 2020 2020 2d20 6060  om pypi.    - ``
+00001cf0: 600a 2020 2020 2020 7079 7468 6f6e 3320  `.      python3 
+00001d00: 2d6d 2070 6970 2069 6e73 7461 6c6c 2073  -m pip install s
+00001d10: 6563 696d 706f 7274 0a20 2020 2020 2060  ecimport.      `
+00001d20: 6060 0a20 202d 2049 6e73 7461 6c6c 2066  ``.  - Install f
+00001d30: 726f 6d20 736f 7572 6365 0a20 2020 202d  rom source.    -
+00001d40: 2060 6060 0a20 2020 2020 2067 6974 2063   ```.      git c
+00001d50: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00001d60: 6875 622e 636f 6d2f 6176 696c 756d 2f73  hub.com/avilum/s
+00001d70: 6563 696d 706f 7274 2e67 6974 2026 2620  ecimport.git && 
+00001d80: 6364 2073 6563 696d 706f 7274 0a20 2020  cd secimport.   
+00001d90: 2020 2070 7974 686f 6e33 202d 6d20 7069     python3 -m pi
+00001da0: 7020 696e 7374 616c 6c20 706f 6574 7279  p install poetry
+00001db0: 2026 2620 7079 7468 6f6e 3320 2d6d 2070   && python3 -m p
+00001dc0: 6f65 7472 7920 696e 7374 616c 6c0a 2020  oetry install.  
+00001dd0: 2020 2020 6060 600a 0a0a 2323 2055 7361      ```...## Usa
+00001de0: 6765 0a54 6f20 7361 6e64 626f 7820 796f  ge.To sandbox yo
+00001df0: 7572 2070 726f 6772 616d 2075 7369 6e67  ur program using
+00001e00: 2074 6865 2043 4c49 2c20 7374 6172 7420   the CLI, start 
+00001e10: 6120 6270 6674 7261 6365 2070 726f 6772  a bpftrace progr
+00001e20: 616d 2074 6861 7420 6c6f 6773 2061 6c6c  am that logs all
+00001e30: 2074 6865 2073 7973 6361 6c6c 7320 666f   the syscalls fo
+00001e40: 7220 616c 6c20 7468 6520 6d6f 6475 6c65  r all the module
+00001e50: 7320 696e 2079 6f75 7220 6170 706c 6963  s in your applic
+00001e60: 6174 696f 6e20 696e 746f 2061 2066 696c  ation into a fil
+00001e70: 6520 7769 7468 2074 6865 2073 6563 696d  e with the secim
+00001e80: 706f 7274 2074 7261 6365 2063 6f6d 6d61  port trace comma
+00001e90: 6e64 2e20 4f6e 6365 2079 6f75 2068 6176  nd. Once you hav
+00001ea0: 6520 636f 7665 7265 6420 7468 6520 6c6f  e covered the lo
+00001eb0: 6769 6320 796f 7520 776f 756c 6420 6c69  gic you would li
+00001ec0: 6b65 2074 6f20 7361 6e64 626f 782c 2068  ke to sandbox, h
+00001ed0: 6974 2043 5452 4c2b 4320 6f72 2043 5452  it CTRL+C or CTR
+00001ee0: 4c2b 442c 206f 7220 7761 6974 2066 6f72  L+D, or wait for
+00001ef0: 2074 6865 2070 726f 6772 616d 2074 6f20   the program to 
+00001f00: 6669 6e69 7368 2e20 5468 656e 2c20 6275  finish. Then, bu
+00001f10: 696c 6420 6120 7361 6e64 626f 7820 6672  ild a sandbox fr
+00001f20: 6f6d 2074 6865 2074 7261 6365 2075 7369  om the trace usi
+00001f30: 6e67 2074 6865 2073 6563 696d 706f 7274  ng the secimport
+00001f40: 2062 7569 6c64 2063 6f6d 6d61 6e64 2c20   build command, 
+00001f50: 616e 6420 7275 6e20 7468 6520 7361 6e64  and run the sand
+00001f60: 626f 7820 7769 7468 2074 6865 2073 6563  box with the sec
+00001f70: 696d 706f 7274 2072 756e 2063 6f6d 6d61  import run comma
+00001f80: 6e64 2e0a 0a60 6060 7368 656c 6c0a 4e41  nd...```shell.NA
+00001f90: 4d45 0a20 2020 2073 6563 696d 706f 7274  ME.    secimport
+00001fa0: 202d 2069 7320 6120 636f 6d70 7265 6865   - is a comprehe
+00001fb0: 6e73 6976 6520 746f 6f6c 6b69 7420 6465  nsive toolkit de
+00001fc0: 7369 676e 6564 2074 6f20 656e 6162 6c65  signed to enable
+00001fd0: 2074 6865 2074 7261 6369 6e67 2c20 636f   the tracing, co
+00001fe0: 6e73 7472 7563 7469 6f6e 2c20 616e 6420  nstruction, and 
+00001ff0: 6578 6563 7574 696f 6e20 6f66 2073 6563  execution of sec
+00002000: 7572 6520 5079 7468 6f6e 2072 756e 7469  ure Python runti
+00002010: 6d65 732e 2049 7420 6c65 7665 7261 6765  mes. It leverage
+00002020: 7320 5553 4454 2070 726f 6265 7320 616e  s USDT probes an
+00002030: 6420 6542 5046 2f44 5472 6163 6520 7465  d eBPF/DTrace te
+00002040: 6368 6e6f 6c6f 6769 6573 2074 6f20 656e  chnologies to en
+00002050: 6861 6e63 6520 7468 6520 6f76 6572 616c  hance the overal
+00002060: 6c20 7365 6375 7269 7479 206d 6561 7375  l security measu
+00002070: 7265 732e 0a0a 5359 4e4f 5053 4953 0a20  res...SYNOPSIS. 
+00002080: 2020 2073 6563 696d 706f 7274 2043 4f4d     secimport COM
+00002090: 4d41 4e44 0a0a 4445 5343 5249 5054 494f  MAND..DESCRIPTIO
+000020a0: 4e0a 2020 2020 6874 7470 733a 2f2f 6769  N.    https://gi
+000020b0: 7468 7562 2e63 6f6d 2f61 7669 6c75 6d2f  thub.com/avilum/
+000020c0: 7365 6369 6d70 6f72 742f 7769 6b69 2f43  secimport/wiki/C
+000020d0: 6f6d 6d61 6e64 2d4c 696e 652d 5573 6167  ommand-Line-Usag
+000020e0: 650a 0a20 2020 2057 4f52 4b46 4c4f 573a  e..    WORKFLOW:
+000020f0: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
+00002100: 7365 6369 6d70 6f72 7420 7472 6163 6520  secimport trace 
+00002110: 2f20 7365 6369 6d70 6f72 7420 7368 656c  / secimport shel
+00002120: 6c0a 2020 2020 2020 2020 2020 2020 322e  l.            2.
+00002130: 2073 6563 696d 706f 7274 2062 7569 6c64   secimport build
+00002140: 0a20 2020 2020 2020 2020 2020 2033 2e20  .            3. 
+00002150: 7365 6369 6d70 6f72 7420 7275 6e0a 0a20  secimport run.. 
+00002160: 2020 2051 5549 434b 5354 4152 543a 0a20     QUICKSTART:. 
+00002170: 2020 2020 2020 2020 2020 2024 2073 6563             $ sec
+00002180: 696d 706f 7274 2069 6e74 6572 6163 7469  import interacti
+00002190: 7665 0a0a 2020 2020 4558 414d 504c 4553  ve..    EXAMPLES
+000021a0: 3a0a 2020 2020 2020 2020 312e 2074 7261  :.        1. tra
+000021b0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+000021c0: 2420 2073 6563 696d 706f 7274 2074 7261  $  secimport tra
+000021d0: 6365 0a20 2020 2020 2020 2020 2020 2024  ce.            $
+000021e0: 2020 7365 6369 6d70 6f72 7420 7472 6163    secimport trac
+000021f0: 6520 2d68 0a20 2020 2020 2020 2020 2020  e -h.           
+00002200: 2024 2020 7365 6369 6d70 6f72 7420 7472   $  secimport tr
+00002210: 6163 655f 7069 6420 3132 330a 2020 2020  ace_pid 123.    
+00002220: 2020 2020 2020 2020 2420 2073 6563 696d          $  secim
+00002230: 706f 7274 2074 7261 6365 5f70 6964 202d  port trace_pid -
+00002240: 680a 2020 2020 2020 2020 322e 2062 7569  h.        2. bui
+00002250: 6c64 3a0a 2020 2020 2020 2020 2020 2020  ld:.            
+00002260: 2320 7365 6369 6d70 6f72 7420 6275 696c  # secimport buil
+00002270: 640a 2020 2020 2020 2020 2020 2020 2420  d.            $ 
+00002280: 7365 6369 6d70 6f72 7420 6275 696c 6420  secimport build 
+00002290: 2d68 0a20 2020 2020 2020 2033 2e20 7275  -h.        3. ru
+000022a0: 6e3a 0a20 2020 2020 2020 2020 2020 2024  n:.            $
+000022b0: 2020 7365 6369 6d70 6f72 7420 7275 6e0a    secimport run.
+000022c0: 2020 2020 2020 2020 2020 2020 2420 2073              $  s
+000022d0: 6563 696d 706f 7274 2072 756e 202d 2d65  ecimport run --e
+000022e0: 6e74 7279 706f 696e 7420 6d79 5f63 7573  ntrypoint my_cus
+000022f0: 746f 6d5f 6d61 696e 2e70 790a 2020 2020  tom_main.py.    
+00002300: 2020 2020 2020 2020 2420 2073 6563 696d          $  secim
+00002310: 706f 7274 2072 756e 202d 2d65 6e74 7279  port run --entry
+00002320: 706f 696e 7420 6d79 5f63 7573 746f 6d5f  point my_custom_
+00002330: 6d61 696e 2e70 7920 2d2d 7374 6f70 5f6f  main.py --stop_o
+00002340: 6e5f 7669 6f6c 6174 696f 6e3d 7472 7565  n_violation=true
+00002350: 0a20 2020 2020 2020 2020 2020 2024 2020  .            $  
+00002360: 7365 6369 6d70 6f72 7420 7275 6e20 2d2d  secimport run --
+00002370: 656e 7472 7970 6f69 6e74 206d 795f 6375  entrypoint my_cu
+00002380: 7374 6f6d 5f6d 6169 6e2e 7079 202d 2d6b  stom_main.py --k
+00002390: 696c 6c5f 6f6e 5f76 696f 6c61 7469 6f6e  ill_on_violation
+000023a0: 3d74 7275 650a 2020 2020 2020 2020 2020  =true.          
+000023b0: 2020 2420 2073 6563 696d 706f 7274 2072    $  secimport r
+000023c0: 756e 202d 2d73 616e 6462 6f78 5f65 7865  un --sandbox_exe
+000023d0: 6375 7461 626c 6520 2f70 6174 682f 746f  cutable /path/to
+000023e0: 2f6d 795f 7361 6e64 626f 782e 6274 202d  /my_sandbox.bt -
+000023f0: 2d70 6964 2032 3838 340a 2020 2020 2020  -pid 2884.      
+00002400: 2020 2020 2020 2420 2073 6563 696d 706f        $  secimpo
+00002410: 7274 2072 756e 202d 2d73 616e 6462 6f78  rt run --sandbox
+00002420: 5f65 7865 6375 7461 626c 6520 2f70 6174  _executable /pat
+00002430: 682f 746f 2f6d 795f 7361 6e64 626f 782e  h/to/my_sandbox.
+00002440: 6274 202d 2d73 616e 6462 6f78 5f6c 6f67  bt --sandbox_log
+00002450: 6669 6c65 206d 795f 6c6f 672e 6c6f 670a  file my_log.log.
+00002460: 2020 2020 2020 2020 2020 2020 2420 2073              $  s
+00002470: 6563 696d 706f 7274 2072 756e 202d 680a  ecimport run -h.
+00002480: 0a43 4f4d 4d41 4e44 530a 2020 2020 434f  .COMMANDS.    CO
+00002490: 4d4d 414e 4420 6973 206f 6e65 206f 6620  MMAND is one of 
+000024a0: 7468 6520 666f 6c6c 6f77 696e 673a 0a0a  the following:..
+000024b0: 2020 2020 2062 7569 6c64 0a20 2020 2020       build.     
+000024c0: 2020 436f 6d70 696c 6573 2061 2074 7261    Compiles a tra
+000024d0: 6365 206c 6f67 2028 7472 6163 652e 6c6f  ce log (trace.lo
+000024e0: 6729 2e20 4372 6561 7465 7320 7468 6520  g). Creates the 
+000024f0: 7361 6e64 626f 7820 6578 6563 7574 6162  sandbox executab
+00002500: 6c65 2028 696e 7374 7275 6d65 6e74 6174  le (instrumentat
+00002510: 696f 6e20 7363 7269 7074 2920 666f 7220  ion script) for 
+00002520: 6561 6368 2073 7570 706f 7274 6564 2062  each supported b
+00002530: 6163 6b65 6e64 2049 7420 7573 6573 2060  ackend It uses `
+00002540: 6372 6561 7465 5f70 726f 6669 6c65 5f66  create_profile_f
+00002550: 726f 6d5f 7472 6163 6520 2e2e 2e60 2061  rom_trace ...` a
+00002560: 6e64 2060 7361 6e64 626f 785f 6672 6f6d  nd `sandbox_from
+00002570: 5f70 726f 6669 6c65 602e 0a0a 2020 2020  _profile`...    
+00002580: 2063 6f6d 7069 6c65 5f73 616e 6462 6f78   compile_sandbox
+00002590: 5f66 726f 6d5f 7072 6f66 696c 650a 2020  _from_profile.  
+000025a0: 2020 2020 2047 656e 6572 6174 6573 2061       Generates a
+000025b0: 2074 6169 6c6f 722d 6d61 6465 2073 616e   tailor-made san
+000025c0: 6462 6f78 2074 6861 7420 7769 6c6c 2065  dbox that will e
+000025d0: 6e66 6f72 6365 2061 2067 6976 656e 2079  nforce a given y
+000025e0: 616d 6c20 7072 6f66 696c 652f 706f 6c69  aml profile/poli
+000025f0: 6379 2069 6e20 7275 6e74 696d 652e 0a0a  cy in runtime...
+00002600: 2020 2020 2069 6e74 6572 6163 7469 7665       interactive
+00002610: 0a0a 2020 2020 2072 756e 0a20 2020 2020  ..     run.     
+00002620: 2020 5275 6e20 6120 7079 7468 6f6e 2070    Run a python p
+00002630: 726f 6365 7373 2069 6e73 6964 6520 7468  rocess inside th
+00002640: 6520 7361 6e64 626f 782e 0a0a 2020 2020  e sandbox...    
+00002650: 2073 6865 6c6c 0a20 2020 2020 2020 416c   shell.       Al
+00002660: 7465 726e 6174 6976 6520 7379 6e74 6178  ternative syntax
+00002670: 2066 6f72 2073 6563 696d 706f 7274 2022   for secimport "
+00002680: 7472 6163 6522 2e0a 0a20 2020 2020 7472  trace"...     tr
+00002690: 6163 650a 2020 2020 2020 2054 7261 6365  ace.       Trace
+000026a0: 7320 6120 7079 7468 6f6e 2070 726f 6365  s a python proce
+000026b0: 7373 2075 7369 6e67 2061 6e20 656e 7472  ss using an entr
+000026c0: 7970 6f69 6e74 206f 7220 696e 7465 7261  ypoint or intera
+000026d0: 6374 6976 6520 696e 7465 7270 7265 7465  ctive interprete
+000026e0: 722e 2049 7420 6d69 6768 7420 7265 7175  r. It might requ
+000026f0: 6972 6520 7375 646f 2070 7269 7669 6c6c  ire sudo privill
+00002700: 6567 6573 206f 6e20 736f 6d65 2068 6f73  eges on some hos
+00002710: 7473 2e0a 0a20 2020 2020 7472 6163 655f  ts...     trace_
+00002720: 7069 640a 2020 2020 2020 2054 7261 6365  pid.       Trace
+00002730: 7320 6120 7275 6e6e 696e 6720 7072 6f63  s a running proc
+00002740: 6573 7320 6279 2070 6964 2e20 4974 206d  ess by pid. It m
+00002750: 6967 6874 2072 6571 7569 7265 2073 7564  ight require sud
+00002760: 6f20 7072 6976 696c 6c65 6765 7320 6f6e  o privilleges on
+00002770: 2073 6f6d 6520 686f 7374 732e 0a60 6060   some hosts..```
+00002780: 0a0a 2323 2053 746f 7020 6f6e 2076 696f  ..## Stop on vio
+00002790: 6c61 7469 6f6e 0a60 6060 0a72 6f6f 7440  lation.```.root@
+000027a0: 3162 6330 3533 3164 3931 6430 3a2f 776f  1bc0531d91d0:/wo
+000027b0: 726b 7370 6163 6523 2073 6563 696d 706f  rkspace# secimpo
+000027c0: 7274 2072 756e 2020 2d2d 7374 6f70 5f6f  rt run  --stop_o
+000027d0: 6e5f 7669 6f6c 6174 696f 6e3d 7472 7565  n_violation=true
+000027e0: 0a20 3e3e 3e20 7365 6369 6d70 6f72 7420  . >>> secimport 
+000027f0: 7275 6e0a 5b57 4152 4e49 4e47 5d3a 2054  run.[WARNING]: T
+00002800: 6869 7320 7361 6e64 626f 7820 7769 6c6c  his sandbox will
+00002810: 2073 656e 6420 5349 4753 544f 5020 746f   send SIGSTOP to
+00002820: 2074 6865 2070 726f 6772 616d 2075 706f   the program upo
+00002830: 6e20 7669 6f6c 6174 696f 6e2e 0a20 5255  n violation.. RU
+00002840: 4e4e 494e 4720 5341 4e44 424f 582e 2e2e  NNING SANDBOX...
+00002850: 205b 272e 2f73 616e 6462 6f78 2e62 7427   ['./sandbox.bt'
+00002860: 2c20 272d 2d75 6e73 6166 6527 2c20 2720  , '--unsafe', ' 
+00002870: 2d63 2027 2c20 272f 776f 726b 7370 6163  -c ', '/workspac
+00002880: 652f 5079 7468 6f6e 2d33 2e31 302e 302f  e/Python-3.10.0/
+00002890: 7079 7468 6f6e 272c 2027 5354 4f50 275d  python', 'STOP']
+000028a0: 0a41 7474 6163 6869 6e67 2034 2070 726f  .Attaching 4 pro
+000028b0: 6265 732e 2e2e 0a50 7974 686f 6e20 332e  bes....Python 3.
+000028c0: 3130 2e30 2028 6465 6661 756c 742c 2041  10.0 (default, A
+000028d0: 7072 2032 3820 3230 3233 2c20 3131 3a33  pr 28 2023, 11:3
+000028e0: 323a 3430 2920 5b47 4343 2039 2e34 2e30  2:40) [GCC 9.4.0
+000028f0: 5d20 6f6e 206c 696e 7578 0a54 7970 6520  ] on linux.Type 
+00002900: 2268 656c 7022 2c20 2263 6f70 7972 6967  "help", "copyrig
+00002910: 6874 222c 2022 6372 6564 6974 7322 206f  ht", "credits" o
+00002920: 7220 226c 6963 656e 7365 2220 666f 7220  r "license" for 
+00002930: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00002940: 2e0a 3e3e 3e20 696d 706f 7274 206f 730a  ..>>> import os.
+00002950: 3e3e 3e20 6f73 2e73 7973 7465 6d28 2770  >>> os.system('p
+00002960: 7327 290a 5b53 4543 5552 4954 5920 5052  s').[SECURITY PR
+00002970: 4f46 494c 4520 5649 4f4c 4154 4544 5d3a  OFILE VIOLATED]:
+00002980: 203c 7374 6469 6e3e 2063 616c 6c65 6420   <stdin> called 
+00002990: 7379 7363 616c 6c20 3536 2061 7420 6465  syscall 56 at de
+000029a0: 7074 6820 3830 3232 0a0a 5e5e 5e20 5354  pth 8022..^^^ ST
+000029b0: 4f50 5049 4e47 2050 524f 4345 5353 2038  OPPING PROCESS 8
+000029c0: 3539 3138 2044 5545 2054 4f20 5359 5343  5918 DUE TO SYSC
+000029d0: 414c 4c20 5649 4f4c 4154 494f 4e20 5e5e  ALL VIOLATION ^^
+000029e0: 5e0a 0909 5052 4f43 4553 5320 3835 3931  ^...PROCESS 8591
+000029f0: 3820 5354 4f50 5045 442e 0a60 6060 0a0a  8 STOPPED..```..
+00002a00: 2323 204b 696c 6c20 6f6e 2076 696f 6c61  ## Kill on viola
+00002a10: 7469 6f6e 0a60 6060 0a72 6f6f 7440 6565  tion.```.root@ee
+00002a20: 3462 6339 3962 6230 3131 3a2f 776f 726b  4bc99bb011:/work
+00002a30: 7370 6163 6523 2073 6563 696d 706f 7274  space# secimport
+00002a40: 2072 756e 202d 2d6b 696c 6c5f 6f6e 5f76   run --kill_on_v
+00002a50: 696f 6c61 7469 6f6e 0a20 3e3e 3e20 7365  iolation. >>> se
+00002a60: 6369 6d70 6f72 7420 7275 6e0a 5b57 4152  cimport run.[WAR
+00002a70: 4e49 4e47 5d3a 2054 6869 7320 7361 6e64  NING]: This sand
+00002a80: 626f 7820 7769 6c6c 2073 656e 6420 5349  box will send SI
+00002a90: 474b 494c 4c20 746f 2074 6865 2070 726f  GKILL to the pro
+00002aa0: 6772 616d 2075 706f 6e20 7669 6f6c 6174  gram upon violat
+00002ab0: 696f 6e2e 0a20 5255 4e4e 494e 4720 5341  ion.. RUNNING SA
+00002ac0: 4e44 424f 582e 2e2e 205b 272e 2f73 616e  NDBOX... ['./san
+00002ad0: 6462 6f78 2e62 7427 2c20 272d 2d75 6e73  dbox.bt', '--uns
+00002ae0: 6166 6527 2c20 2720 2d63 2027 2c20 272f  afe', ' -c ', '/
+00002af0: 776f 726b 7370 6163 652f 5079 7468 6f6e  workspace/Python
+00002b00: 2d33 2e31 302e 302f 7079 7468 6f6e 272c  -3.10.0/python',
+00002b10: 2027 4b49 4c4c 275d 0a69 6d70 6f72 7420   'KILL'].import 
+00002b20: 6f73 0a6f 4174 7461 6368 696e 6720 3420  os.oAttaching 4 
+00002b30: 7072 6f62 6573 2e2e 2e0a 7350 7974 686f  probes....sPytho
+00002b40: 6e20 332e 3130 2e30 2028 6465 6661 756c  n 3.10.0 (defaul
+00002b50: 742c 2041 7072 2032 3820 3230 3233 2c20  t, Apr 28 2023, 
+00002b60: 3131 3a33 323a 3430 2920 5b47 4343 2039  11:32:40) [GCC 9
+00002b70: 2e34 2e30 5d20 6f6e 206c 696e 7578 0a54  .4.0] on linux.T
+00002b80: 7970 6520 2268 656c 7022 2c20 2263 6f70  ype "help", "cop
+00002b90: 7972 6967 6874 222c 2022 6372 6564 6974  yright", "credit
+00002ba0: 7322 206f 7220 226c 6963 656e 7365 2220  s" or "license" 
+00002bb0: 666f 7220 6d6f 7265 2069 6e66 6f72 6d61  for more informa
+00002bc0: 7469 6f6e 2e0a 3e3e 3e20 696d 706f 7274  tion..>>> import
+00002bd0: 206f 730a 3e3e 3e20 6f73 2e73 7973 7465   os.>>> os.syste
+00002be0: 6d28 2770 7327 290a 5b53 4543 5552 4954  m('ps').[SECURIT
+00002bf0: 5920 5052 4f46 494c 4520 5649 4f4c 4154  Y PROFILE VIOLAT
+00002c00: 4544 5d3a 203c 7374 6469 6e3e 2063 616c  ED]: <stdin> cal
+00002c10: 6c65 6420 7379 7363 616c 6c20 3536 2061  led syscall 56 a
+00002c20: 7420 6465 7074 6820 3830 3232 0a0a 5e5e  t depth 8022..^^
+00002c30: 5e20 4b49 4c4c 494e 4720 5052 4f43 4553  ^ KILLING PROCES
+00002c40: 5320 3836 3436 3620 4455 4520 544f 2053  S 86466 DUE TO S
+00002c50: 5953 4341 4c4c 2056 494f 4c41 5449 4f4e  YSCALL VIOLATION
+00002c60: 205e 5e5e 0a09 094b 494c 4c45 442e 0a20   ^^^...KILLED.. 
+00002c70: 5341 4e44 424f 5820 4558 4954 4544 3b0a  SANDBOX EXITED;.
+00002c80: 6060 600a 0a23 2320 4479 6e61 6d69 6320  ```..## Dynamic 
+00002c90: 7072 6f66 696c 696e 6720 2d20 7472 6163  profiling - trac
+00002ca0: 652c 2062 7569 6c64 2073 616e 6462 6f78  e, build sandbox
+00002cb0: 2c20 7275 6e2e 0a60 6060 7368 656c 6c0a  , run..```shell.
+00002cc0: 726f 6f74 4031 6661 3364 3666 3039 3938  root@1fa3d6f0998
+00002cd0: 393a 2f77 6f72 6b73 7061 6365 2320 7365  9:/workspace# se
+00002ce0: 6369 6d70 6f72 7420 696e 7465 7261 6374  cimport interact
+00002cf0: 6976 650a 0a4c 6574 2773 2063 7265 6174  ive..Let's creat
+00002d00: 6520 6f75 7220 6669 7273 7420 7461 696c  e our first tail
+00002d10: 6f72 2d6d 6164 6520 7361 6e64 626f 7820  or-made sandbox 
+00002d20: 7769 7468 2073 6563 696d 706f 7274 210a  with secimport!.
+00002d30: 2d20 4120 7079 7468 6f6e 2073 6865 6c6c  - A python shell
+00002d40: 2077 696c 6c20 6265 206f 7065 6e65 640a   will be opened.
+00002d50: 2d20 5468 6520 6265 6861 7669 6f72 2077  - The behavior w
+00002d60: 696c 6c20 6265 2072 6563 6f72 6465 642e  ill be recorded.
+00002d70: 0a0a 4f4b 3f20 2879 293a 2079 0a20 3e3e  ..OK? (y): y. >>
+00002d80: 3e20 7365 6369 6d70 6f72 7420 7472 6163  > secimport trac
+00002d90: 650a 0a54 5241 4349 4e47 3a20 5b27 2f77  e..TRACING: ['/w
+00002da0: 6f72 6b73 7061 6365 2f73 6563 696d 706f  orkspace/secimpo
+00002db0: 7274 2f70 726f 6669 6c65 732f 7472 6163  rt/profiles/trac
+00002dc0: 652e 6274 272c 2027 2d63 272c 2027 2f77  e.bt', '-c', '/w
+00002dd0: 6f72 6b73 7061 6365 2f50 7974 686f 6e2d  orkspace/Python-
+00002de0: 332e 3130 2e30 2f70 7974 686f 6e27 2c20  3.10.0/python', 
+00002df0: 272d 6f27 2c20 2774 7261 6365 2e6c 6f67  '-o', 'trace.log
+00002e00: 275d 0a0a 2020 2020 2020 2020 2020 2020  ']..            
+00002e10: 2020 2020 2020 2020 2020 2020 5072 6573              Pres
+00002e20: 7320 4354 524c 2b44 2074 6f20 7374 6f70  s CTRL+D to stop
+00002e30: 2074 6865 2074 7261 6365 3b0a 0a50 7974   the trace;..Pyt
+00002e40: 686f 6e20 332e 3130 2e30 2028 6465 6661  hon 3.10.0 (defa
+00002e50: 756c 742c 204d 6172 2031 3920 3230 3233  ult, Mar 19 2023
+00002e60: 2c20 3038 3a33 343a 3436 2920 5b47 4343  , 08:34:46) [GCC
+00002e70: 2039 2e34 2e30 5d20 6f6e 206c 696e 7578   9.4.0] on linux
+00002e80: 0a54 7970 6520 2268 656c 7022 2c20 2263  .Type "help", "c
+00002e90: 6f70 7972 6967 6874 222c 2022 6372 6564  opyright", "cred
+00002ea0: 6974 7322 206f 7220 226c 6963 656e 7365  its" or "license
+00002eb0: 2220 666f 7220 6d6f 7265 2069 6e66 6f72  " for more infor
+00002ec0: 6d61 7469 6f6e 2e0a 3e3e 3e20 696d 706f  mation..>>> impo
+00002ed0: 7274 2074 6869 730a 3e3e 3e0a 2054 5241  rt this.>>>. TRA
+00002ee0: 4349 4e47 2044 4f4e 453b 0a20 3e3e 3e20  CING DONE;. >>> 
+00002ef0: 7365 6369 6d70 6f72 7420 6275 696c 640a  secimport build.
+00002f00: 0a53 4543 494d 504f 5254 2043 4f4d 5049  .SECIMPORT COMPI
+00002f10: 4c49 4e47 2e2e 2e0a 0a43 5245 4154 4544  LING.....CREATED
+00002f20: 204a 534f 4e20 5445 4d50 4c41 5445 3a20   JSON TEMPLATE: 
+00002f30: 2070 6f6c 6963 792e 6a73 6f6e 0a43 5245   policy.json.CRE
+00002f40: 4154 4544 2059 414d 4c20 5445 4d50 4c41  ATED YAML TEMPLA
+00002f50: 5445 3a20 2070 6f6c 6963 792e 7961 6d6c  TE:  policy.yaml
+00002f60: 0a63 6f6d 7069 6c69 6e67 2074 656d 706c  .compiling templ
+00002f70: 6174 6520 706f 6c69 6379 2e79 616d 6c0a  ate policy.yaml.
+00002f80: 4454 5241 4345 2053 414e 4442 4f58 3a20  DTRACE SANDBOX: 
+00002f90: 2073 616e 6462 6f78 2e64 0a42 5046 5452   sandbox.d.BPFTR
+00002fa0: 4345 2053 414e 4442 4f58 3a20 2073 616e  CE SANDBOX:  san
+00002fb0: 6462 6f78 2e62 740a 6060 600a 0a4e 6f77  dbox.bt.```..Now
+00002fc0: 2c20 6c65 7427 7320 7275 6e20 7468 6520  , let's run the 
+00002fd0: 7361 6e64 626f 7821 0a60 6060 7079 7468  sandbox!.```pyth
+00002fe0: 6f6e 0a2d 2052 756e 2074 6865 2073 616d  on.- Run the sam
+00002ff0: 6520 636f 6d6d 616e 6473 2061 7320 6265  e commands as be
+00003000: 666f 7265 2c20 7468 6579 2073 686f 756c  fore, they shoul
+00003010: 6420 7275 6e20 7769 7468 6f75 7420 616e  d run without an
+00003020: 7920 7072 6f62 6c65 6d3b 2e0a 2d20 446f  y problem;..- Do
+00003030: 2073 6f6d 6574 6869 6e67 206e 6577 2069   something new i
+00003040: 6e20 7468 6520 7368 656c 6c3b 2065 2e67  n the shell; e.g
+00003050: 3a20 2020 3e3e 3e20 5f5f 696d 706f 7274  :   >>> __import
+00003060: 5f5f 2822 6f73 2229 2e73 7973 7465 6d28  __("os").system(
+00003070: 2270 7322 290a 0a20 2020 2020 2020 204f  "ps")..        O
+00003080: 4b3f 2028 7929 3a20 790a 203e 3e3e 2073  K? (y): y. >>> s
+00003090: 6563 696d 706f 7274 2072 756e 0a20 5255  ecimport run. RU
+000030a0: 4e4e 494e 4720 5341 4e44 424f 582e 2e2e  NNING SANDBOX...
+000030b0: 205b 272e 2f73 616e 6462 6f78 2e62 7427   ['./sandbox.bt'
+000030c0: 2c20 272d 2d75 6e73 6166 6527 2c20 2720  , '--unsafe', ' 
+000030d0: 2d63 2027 2c20 272f 776f 726b 7370 6163  -c ', '/workspac
+000030e0: 652f 5079 7468 6f6e 2d33 2e31 302e 302f  e/Python-3.10.0/
+000030f0: 7079 7468 6f6e 275d 0a41 7474 6163 6869  python'].Attachi
+00003100: 6e67 2035 2070 726f 6265 732e 2e2e 0a52  ng 5 probes....R
+00003110: 4547 4953 5445 5249 4e47 2053 5953 4341  EGISTERING SYSCA
+00003120: 4c4c 532e 2e2e 0a53 5441 5254 4544 0a50  LLS....STARTED.P
+00003130: 7974 686f 6e20 332e 3130 2e30 2028 6465  ython 3.10.0 (de
+00003140: 6661 756c 742c 204d 6172 2031 3920 3230  fault, Mar 19 20
+00003150: 3233 2c20 3038 3a33 343a 3436 2920 5b47  23, 08:34:46) [G
+00003160: 4343 2039 2e34 2e30 5d20 6f6e 206c 696e  CC 9.4.0] on lin
+00003170: 7578 0a54 7970 6520 2268 656c 7022 2c20  ux.Type "help", 
+00003180: 2263 6f70 7972 6967 6874 222c 2022 6372  "copyright", "cr
+00003190: 6564 6974 7322 206f 7220 226c 6963 656e  edits" or "licen
+000031a0: 7365 2220 666f 7220 6d6f 7265 2069 6e66  se" for more inf
+000031b0: 6f72 6d61 7469 6f6e 2e0a 3e3e 3e20 696d  ormation..>>> im
+000031c0: 706f 7274 2074 6869 730a 3e3e 3e20 696d  port this.>>> im
+000031d0: 706f 7274 206f 730a 5b53 4543 494d 504f  port os.[SECIMPO
+000031e0: 5254 2056 494f 4c41 5449 4f4e 5d3a 203c  RT VIOLATION]: <
+000031f0: 7374 6469 6e3e 2063 616c 6c65 6420 7379  stdin> called sy
+00003200: 7363 616c 6c20 696f 6374 6c20 6174 2064  scall ioctl at d
+00003210: 6570 7468 2030 0a5b 5345 4349 4d50 4f52  epth 0.[SECIMPOR
+00003220: 5420 5649 4f4c 4154 494f 4e5d 3a20 3c73  T VIOLATION]: <s
+00003230: 7464 696e 3e20 6361 6c6c 6564 2073 7973  tdin> called sys
+00003240: 6361 6c6c 2069 6f63 746c 2061 7420 6465  call ioctl at de
+00003250: 7074 6820 300a 6060 600a 0a46 6f72 206d  pth 0.```..For m
+00003260: 6f72 6520 6465 7461 696c 6564 2075 7361  ore detailed usa
+00003270: 6765 2069 6e73 7472 7563 7469 6f6e 732c  ge instructions,
+00003280: 2073 6565 2074 6865 205b 436f 6d6d 616e   see the [Comman
+00003290: 642d 4c69 6e65 2055 7361 6765 5d28 6874  d-Line Usage](ht
+000032a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000032b0: 2f61 7669 6c75 6d2f 7365 6369 6d70 6f72  /avilum/secimpor
+000032c0: 742f 7769 6b69 2f43 6f6d 6d61 6e64 2d4c  t/wiki/Command-L
+000032d0: 696e 652d 5573 6167 6529 2070 6167 652e  ine-Usage) page.
+000032e0: 0a0a 2323 206e 736a 6169 6c20 7375 7070  ..## nsjail supp
+000032f0: 6f72 7420 2873 6563 636f 6d70 290a 4265  ort (seccomp).Be
+00003300: 7369 6465 2074 6865 2073 616e 6462 6f78  side the sandbox
+00003310: 2074 6861 7420 7365 6369 6d70 6f72 7420   that secimport 
+00003320: 6275 696c 6473 2c20 3c62 723e 0a54 6865  builds, <br>.The
+00003330: 2060 7365 6369 6d70 6f72 7420 6275 696c   `secimport buil
+00003340: 6460 2063 6f6d 6d61 6e64 2063 7265 6174  d` command creat
+00003350: 6573 2061 6e20 3c61 2068 7265 663d 2268  es an <a href="h
+00003360: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003370: 6d2f 676f 6f67 6c65 2f6e 736a 6169 6c22  m/google/nsjail"
+00003380: 3e6e 736a 6169 6c3c 2f61 3e20 7361 6e64  >nsjail</a> sand
+00003390: 626f 7820 7769 7468 2073 6563 636f 6d70  box with seccomp
+000033a0: 2070 726f 6669 6c65 2066 6f72 2079 6f75   profile for you
+000033b0: 7220 7472 6163 6564 2063 6f64 652e 3c62  r traced code.<b
+000033c0: 723e 2060 6e73 6a61 696c 6020 656e 6162  r> `nsjail` enab
+000033d0: 6c65 7320 6e61 6d65 7370 6163 6520 7361  les namespace sa
+000033e0: 6e64 626f 7869 6e67 2077 6974 6820 7365  ndboxing with se
+000033f0: 6363 6f6d 7020 6f6e 206c 696e 7578 3c62  ccomp on linux<b
+00003400: 723e 0a60 7365 6369 6d70 6f72 7460 2061  r>.`secimport` a
+00003410: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+00003420: 6572 6174 6573 2073 6563 636f 6d70 2070  erates seccomp p
+00003430: 726f 6669 6c65 7320 746f 2075 7365 2077  rofiles to use w
+00003440: 6974 6820 606e 736a 6169 6c60 2061 7320  ith `nsjail` as 
+00003450: 6578 6563 7574 6162 6c65 2062 6173 6820  executable bash 
+00003460: 7363 7269 7074 2e0a 4974 2063 616e 2062  script..It can b
+00003470: 6520 7573 6564 2074 6f20 6c69 6d69 7420  e used to limit 
+00003480: 7468 6520 7379 7363 616c 6c73 206f 6620  the syscalls of 
+00003490: 7468 6520 656e 7469 7265 2070 7974 686f  the entire pytho
+000034a0: 6e20 7072 6f63 6573 732c 2061 7320 616e  n process, as an
+000034b0: 6f74 6865 7220 6c61 7965 7220 6f66 2064  other layer of d
+000034c0: 6566 656e 6365 2e0a 0a23 2320 5079 7468  efence...## Pyth
+000034d0: 6f6e 2041 5049 0a0a 496e 7374 6561 6420  on API..Instead 
+000034e0: 6f66 2043 4c49 2c20 796f 7520 6361 6e20  of CLI, you can 
+000034f0: 616c 736f 2075 7365 2060 7365 6369 6d70  also use `secimp
+00003500: 6f72 7460 2062 7920 7265 706c 6163 696e  ort` by replacin
+00003510: 6720 2260 696d 706f 7274 6022 2077 6974  g "`import`" wit
+00003520: 6820 2260 7365 6369 6d70 6f72 742e 7365  h "`secimport.se
+00003530: 6375 7265 5f69 6d70 6f72 7460 2220 666f  cure_import`" fo
+00003540: 7220 7365 6c65 6374 6564 206d 6f64 756c  r selected modul
+00003550: 6573 2e20 5365 6520 7468 6520 5b50 7974  es. See the [Pyt
+00003560: 686f 6e20 496d 706f 7274 735d 2865 7861  hon Imports](exa
+00003570: 6d70 6c65 732f 7079 7468 6f6e 5f69 6d70  mples/python_imp
+00003580: 6f72 7473 2f29 2065 7861 6d70 6c65 2066  orts/) example f
+00003590: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
+000035a0: 0a0a 2323 2044 6f63 6b65 720a 5468 6520  ..## Docker.The 
+000035b0: 7175 6963 6b65 7374 2077 6179 2074 6f20  quickest way to 
+000035c0: 6576 616c 7561 7465 2060 7365 6369 6d70  evaluate `secimp
+000035d0: 6f72 7460 2069 7320 746f 2075 7365 206f  ort` is to use o
+000035e0: 7572 205b 446f 636b 6572 2063 6f6e 7461  ur [Docker conta
+000035f0: 696e 6572 5d28 646f 636b 6572 2f52 4541  iner](docker/REA
+00003600: 444d 452e 6d64 292c 2077 6869 6368 2069  DME.md), which i
+00003610: 6e63 6c75 6465 7320 6062 7066 7472 6163  ncludes `bpftrac
+00003620: 6560 2028 6065 6270 6660 2920 616e 6420  e` (`ebpf`) and 
+00003630: 6f74 6865 7220 706c 7567 2d61 6e64 2d70  other plug-and-p
+00003640: 6c61 7920 6578 616d 706c 6573 2e0a 0a0a  lay examples....
+00003650: 2323 2045 7861 6d70 6c65 730a 0a54 6865  ## Examples..The
+00003660: 205b 5361 6e64 626f 7820 4578 616d 706c   [Sandbox Exampl
+00003670: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00003680: 7562 2e63 6f6d 2f61 7669 6c75 6d2f 7365  ub.com/avilum/se
+00003690: 6369 6d70 6f72 742f 7769 6b69 2f53 616e  cimport/wiki/San
+000036a0: 6462 6f78 2d45 7861 6d70 6c65 7329 2070  dbox-Examples) p
+000036b0: 6167 6520 636f 6e74 6169 6e73 2062 6173  age contains bas
+000036c0: 6963 2061 6e64 2061 6476 616e 6365 6420  ic and advanced 
+000036d0: 7265 616c 2d77 6f72 6c64 2065 7861 6d70  real-world examp
+000036e0: 6c65 732e 0a0a 2323 2043 6f6e 7472 6962  les...## Contrib
+000036f0: 7574 696e 670a 0a46 6f72 2069 6e66 6f72  uting..For infor
+00003700: 6d61 7469 6f6e 206f 6e20 686f 7720 746f  mation on how to
+00003710: 2063 6f6e 7472 6962 7574 6520 746f 2060   contribute to `
+00003720: 7365 6369 6d70 6f72 7460 2c20 7365 6520  secimport`, see 
+00003730: 7468 6520 5b43 6f6e 7472 6962 7574 696e  the [Contributin
+00003740: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00003750: 622e 636f 6d2f 6176 696c 756d 2f73 6563  b.com/avilum/sec
+00003760: 696d 706f 7274 2f62 6c6f 622f 6d61 7374  import/blob/mast
+00003770: 6572 2f64 6f63 732f 434f 4e54 5249 4255  er/docs/CONTRIBU
+00003780: 5449 4e47 2e6d 6429 2067 7569 6465 2e0a  TING.md) guide..
+00003790: 0a23 2320 526f 6164 6d61 700a 0a53 6565  .## Roadmap..See
+000037a0: 2074 6865 205b 526f 6164 6d61 705d 2868   the [Roadmap](h
+000037b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000037c0: 6d2f 6176 696c 756d 2f73 6563 696d 706f  m/avilum/secimpo
+000037d0: 7274 2f62 6c6f 622f 6d61 7374 6572 2f64  rt/blob/master/d
+000037e0: 6f63 732f 524f 4144 4d41 502e 6d64 2920  ocs/ROADMAP.md) 
+000037f0: 666f 7220 7468 6520 706c 616e 6e65 6420  for the planned 
+00003800: 6665 6174 7572 6573 2061 6e64 2064 6576  features and dev
+00003810: 656c 6f70 6d65 6e74 206d 696c 6573 746f  elopment milesto
+00003820: 6e65 732e 0a0a 2323 2043 6861 6e67 656c  nes...## Changel
+00003830: 6f67 0a0a 5365 6520 7468 6520 5b43 6861  og..See the [Cha
+00003840: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
+00003850: 6769 7468 7562 2e63 6f6d 2f61 7669 6c75  github.com/avilu
+00003860: 6d2f 7365 6369 6d70 6f72 742f 626c 6f62  m/secimport/blob
+00003870: 2f6d 6173 7465 722f 646f 6373 2f43 4841  /master/docs/CHA
+00003880: 4e47 454c 4f47 2e6d 6429 2066 6f72 2064  NGELOG.md) for d
+00003890: 6576 656c 6f70 6d65 6e74 2070 726f 6772  evelopment progr
+000038a0: 6573 7320 616e 6420 6578 6973 7469 6e67  ess and existing
+000038b0: 2066 6561 7475 7265 732e 0a0a             features...
```

