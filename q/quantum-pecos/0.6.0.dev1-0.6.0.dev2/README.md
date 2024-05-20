# Comparing `tmp/quantum_pecos-0.6.0.dev1.tar.gz` & `tmp/quantum_pecos-0.6.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_pecos-0.6.0.dev1.tar", last modified: Wed May 15 17:59:06 2024, max compression
+gzip compressed data, was "quantum_pecos-0.6.0.dev2.tar", last modified: Mon May 20 17:24:01 2024, max compression
```

## Comparing `quantum_pecos-0.6.0.dev1.tar` & `quantum_pecos-0.6.0.dev2.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.383382 quantum_pecos-0.6.0.dev1/
--rw-rw-rw-   0        0        0    11560 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev1/LICENSE
--rw-rw-rw-   0        0        0      136 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0      463 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev1/NOTICE
--rw-rw-rw-   0        0        0    20835 2024-05-15 17:59:06.382883 quantum_pecos-0.6.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     5198 2024-03-10 03:52:18.000000 quantum_pecos-0.6.0.dev1/README.md
--rw-rw-rw-   0        0        0     3243 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.200272 quantum_pecos-0.6.0.dev1/python/
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.207277 quantum_pecos-0.6.0.dev1/python/pecos/
--rw-rw-rw-   0        0        0     1893 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.208932 quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/
--rw-rw-rw-   0        0        0      942 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/__init__.py
--rw-rw-rw-   0        0        0     9739 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/checks2circuit.py
--rw-rw-rw-   0        0        0     5302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/std2chs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.212661 quantum_pecos-0.6.0.dev1/python/pecos/circuits/
--rw-rw-rw-   0        0        0      911 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.220163 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/
--rw-rw-rw-   0        0        0      671 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/__init__.py
--rw-rw-rw-   0        0        0     1437 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/conditionals.py
--rw-rw-rw-   0        0        0     1708 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/cops.py
--rw-rw-rw-   0        0        0     1086 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/fund.py
--rw-rw-rw-   0        0        0     1225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/hyqc.py
--rw-rw-rw-   0        0        0     2830 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/int.py
--rw-rw-rw-   0        0        0     1302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/misc_stmts.py
--rw-rw-rw-   0        0        0     5680 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/qops.py
--rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/qubits.py
--rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/vars.py
--rw-rw-rw-   0        0        0     5033 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/logical_circuit.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.228167 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/
--rw-rw-rw-   0        0        0     1028 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/__init__.py
--rw-rw-rw-   0        0        0      852 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/barrier.py
--rw-rw-rw-   0        0        0     1070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/block.py
--rw-rw-rw-   0        0        0     2283 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/conditionals.py
--rw-rw-rw-   0        0        0     2020 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/expr.py
--rw-rw-rw-   0        0        0      935 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/func.py
--rw-rw-rw-   0        0        0     6986 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/gates.py
--rw-rw-rw-   0        0        0     1592 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/misc.py
--rw-rw-rw-   0        0        0     5616 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/qasm.py
--rw-rw-rw-   0        0        0     1252 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/std_gates.py
--rw-rw-rw-   0        0        0     2312 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/vars.py
--rw-rw-rw-   0        0        0     9989 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/qc2phir.py
--rw-rw-rw-   0        0        0    14990 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/circuits/quantum_circuit.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.230670 quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/classical_interpreter_abc.py
--rw-rw-rw-   0        0        0    12690 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/phir_classical_interpreter.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.231673 quantum_pecos-0.6.0.dev1/python/pecos/decoders/
--rw-rw-rw-   0        0        0      872 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.233673 quantum_pecos-0.6.0.dev1/python/pecos/decoders/dummy_decoder/
--rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/dummy_decoder/__init__.py
--rw-rw-rw-   0        0        0     1171 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/dummy_decoder/dummy_decoder.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.235673 quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/mwpm2d.py
--rw-rw-rw-   0        0        0    17301 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/precomputing.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.239180 quantum_pecos-0.6.0.dev1/python/pecos/engines/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.241183 quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/
--rw-rw-rw-   0        0        0      885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/standard.py
--rw-rw-rw-   0        0        0     2385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/timing_runner.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.245687 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/__init__.py
--rw-rw-rw-   0        0        0     8608 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/binarray.py
--rw-rw-rw-   0        0        0     5087 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/binarray2.py
--rw-rw-rw-   0        0        0     7530 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/classical.py
--rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/cvm.py
--rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/sim_func.py
--rw-rw-rw-   0        0        0     4339 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.249686 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/__init__.py
--rw-rw-rw-   0        0        0     1654 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/pywasm.py
--rw-rw-rw-   0        0        0     1180 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/pywasm3.py
--rw-rw-rw-   0        0        0     2728 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/wasmer.py
--rw-rw-rw-   0        0        0     1634 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/wasmtime.py
--rw-rw-rw-   0        0        0     7574 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine.py
--rw-rw-rw-   0        0        0     4968 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine_multiprocessing.py
--rw-rw-rw-   0        0        0     8509 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine_old.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.257691 quantum_pecos-0.6.0.dev1/python/pecos/error_models/
--rw-rw-rw-   0        0        0     1109 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/__init__.py
--rw-rw-rw-   0        0        0     1849 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/class_errors_circuit.py
--rw-rw-rw-   0        0        0     5704 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/depolarizing_error_model.py
--rw-rw-rw-   0        0        0     5604 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_depolar.py
--rw-rw-rw-   0        0        0     1768 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_model.py
--rw-rw-rw-   0        0        0     1368 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_model_abc.py
--rw-rw-rw-   0        0        0     1035 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/fake_error_model.py
--rw-rw-rw-   0        0        0     5851 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/generic_error_model.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.265196 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/__init__.py
--rw-rw-rw-   0        0        0      958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_initz_bitflip.py
--rw-rw-rw-   0        0        0     1435 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py
--rw-rw-rw-   0        0        0     1450 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_meas_bitflip.py
--rw-rw-rw-   0        0        0     1621 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py
--rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_bitflip.py
--rw-rw-rw-   0        0        0     1488 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py
--rw-rw-rw-   0        0        0     1958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py
--rw-rw-rw-   0        0        0     1761 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py
--rw-rw-rw-   0        0        0     2490 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.269696 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/__init__.py
--rw-rw-rw-   0        0        0     2546 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/gate_groups.py
--rw-rw-rw-   0        0        0     1385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/init_noise.py
--rw-rw-rw-   0        0        0     1593 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/meas_noise.py
--rw-rw-rw-   0        0        0     1337 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/memory_noise.py
--rw-rw-rw-   0        0        0     1207 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/sq_noise.py
--rw-rw-rw-   0        0        0     2943 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/tq_noise.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.273743 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/
--rw-rw-rw-   0        0        0      791 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/__init__.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/depolar_gen.py
--rw-rw-rw-   0        0        0     5732 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/gatewise_gen.py
--rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/xerror_gen.py
--rw-rw-rw-   0        0        0     7322 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/xzerror_gen.py
--rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/zerror_gen.py
--rw-rw-rw-   0        0        0    11841 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/parent_class_error_gen.py
--rw-rw-rw-   0        0        0     5100 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/error_models/simple_depolarizing_error_model.py
--rw-rw-rw-   0        0        0     1026 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.278549 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/foreign_object_abc.py
--rw-rw-rw-   0        0        0     2466 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/object_pool.py
--rw-rw-rw-   0        0        0     1168 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/python.py
--rw-rw-rw-   0        0        0      527 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasm_execution_timer_thread.py
--rw-rw-rw-   0        0        0     3837 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasmer.py
--rw-rw-rw-   0        0        0     5054 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasmtime.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.281049 quantum_pecos-0.6.0.dev1/python/pecos/machines/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/machines/__init__.py
--rw-rw-rw-   0        0        0     2356 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev1/python/pecos/machines/generic_machine.py
--rw-rw-rw-   0        0        0     1591 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/machines/machine_abc.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.286554 quantum_pecos-0.6.0.dev1/python/pecos/misc/
--rw-rw-rw-   0        0        0      840 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/__init__.py
--rw-rw-rw-   0        0        0     2240 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/commute.py
--rw-rw-rw-   0        0        0      838 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/errors.py
--rw-rw-rw-   0        0        0     1681 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/gate_groups.py
--rw-rw-rw-   0        0        0    10545 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/stabilizer_funcs.py
--rw-rw-rw-   0        0        0     1992 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/std_output.py
--rw-rw-rw-   0        0        0     3552 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/symbol_library.py
--rw-rw-rw-   0        0        0     7419 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/misc/threshold_curve.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.288678 quantum_pecos-0.6.0.dev1/python/pecos/op_processors/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/op_processors/__init__.py
--rw-rw-rw-   0        0        0     2266 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/op_processors/generic_op_processor.py
--rw-rw-rw-   0        0        0     1132 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/op_processors/op_processor_abc.py
--rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.292178 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/
--rw-rw-rw-   0        0        0     1147 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.296183 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/__init__.py
--rw-rw-rw-   0        0        0     7774 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/circuit_implementation1.py
--rw-rw-rw-   0        0        0     7702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/color_488.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/gates.py
--rw-rw-rw-   0        0        0     8975 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/instructions.py
--rw-rw-rw-   0        0        0     3576 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/gate_parent_class.py
--rw-rw-rw-   0        0        0     2262 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/helper_functions.py
--rw-rw-rw-   0        0        0     3845 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/instruction_parent_class.py
--rw-rw-rw-   0        0        0     7751 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/plot.py
--rw-rw-rw-   0        0        0     8065 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/qecc_parent_class.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.298683 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/gates.py
--rw-rw-rw-   0        0        0    11245 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/instructions.py
--rw-rw-rw-   0        0        0     9623 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/surface_4444.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.301682 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/gates.py
--rw-rw-rw-   0        0        0    19744 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/instructions.py
--rw-rw-rw-   0        0        0    10241 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.302183 quantum_pecos-0.6.0.dev1/python/pecos/reps/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.308062 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/
--rw-rw-rw-   0        0        0      635 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/block_types.py
--rw-rw-rw-   0        0        0     1961 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/data_types.py
--rw-rw-rw-   0        0        0      236 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/instr_type.py
--rw-rw-rw-   0        0        0     1104 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/list_types.py
--rw-rw-rw-   0        0        0     1103 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/name_resolver.py
--rw-rw-rw-   0        0        0     3167 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/op_types.py
--rw-rw-rw-   0        0        0    10369 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/pypmir.py
--rw-rw-rw-   0        0        0      812 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/types.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.312562 quantum_pecos-0.6.0.dev1/python/pecos/simulators/
--rw-rw-rw-   0        0        0     1878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.315066 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/
--rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/__init__.py
--rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/bindings.py
--rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/gates.py
--rw-rw-rw-   0        0        0     1773 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/state.py
--rw-rw-rw-   0        0        0     2185 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/compile_cython.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.316566 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/
--rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuconn.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.317066 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/
--rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.318566 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/
--rw-rw-rw-   0        0        0      624 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py
--rw-rw-rw-   0        0        0     4489 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.323566 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/__init__.py
--rw-rw-rw-   0        0        0     2010 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/bindings.py
--rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py
--rw-rw-rw-   0        0        0      785 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py
--rw-rw-rw-   0        0        0     3562 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py
--rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py
--rw-rw-rw-   0        0        0     1874 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/state.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.328855 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/
--rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/__init__.py
--rw-rw-rw-   0        0        0     1769 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/bindings.py
--rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_init.py
--rw-rw-rw-   0        0        0     1867 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_meas.py
--rw-rw-rw-   0        0        0     9594 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_one_qubit.py
--rw-rw-rw-   0        0        0    12354 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_two_qubit.py
--rw-rw-rw-   0        0        0     3719 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/state.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.330224 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.331224 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/src/__init__.py
--rw-rw-rw-   0        0        0     6362 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/src/logical_sign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.332723 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/__init__.py
--rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.333724 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/src/__init__.py
--rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/src/logical_sign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.335231 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/__init__.py
--rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.336731 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/src/__init__.py
--rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/src/logical_sign.py
--rw-rw-rw-   0        0        0     2736 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/gate_syms.py
--rw-rw-rw-   0        0        0     2691 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/parent_sim_classes.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.342238 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/
--rw-rw-rw-   0        0        0      710 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/__init__.py
--rw-rw-rw-   0        0        0     2945 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/bindings.py
--rw-rw-rw-   0        0        0      881 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_init.py
--rw-rw-rw-   0        0        0     2985 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_meas.py
--rw-rw-rw-   0        0        0    14031 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_one_qubit.py
--rw-rw-rw-   0        0        0     7900 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_two_qubit.py
--rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/logical_sign.py
--rw-rw-rw-   0        0        0     9712 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/state.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.348295 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/
--rw-rw-rw-   0        0        0      859 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/__init__.py
--rw-rw-rw-   0        0        0     4891 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/bindings.py
--rw-rw-rw-   0        0        0     2213 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_init.py
--rw-rw-rw-   0        0        0     2631 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_meas.py
--rw-rw-rw-   0        0        0     6819 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_one_qubit.py
--rw-rw-rw-   0        0        0     4884 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_two_qubit.py
--rw-rw-rw-   0        0        0     1205 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/helper.py
--rw-rw-rw-   0        0        0     2379 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/logical_sign.py
--rw-rw-rw-   0        0        0     4977 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/state.py
--rw-rw-rw-   0        0        0     2885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/quantum_simulator.py
--rw-rw-rw-   0        0        0     1409 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sim_class_types.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.355298 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/
--rw-rw-rw-   0        0        0     1933 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/bindings.py
--rw-rw-rw-   0        0        0     3225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_init.py
--rw-rw-rw-   0        0        0    11606 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_meas.py
--rw-rw-rw-   0        0        0    33702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_one_qubit.py
--rw-rw-rw-   0        0        0    15954 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_two_qubit.py
--rw-rw-rw-   0        0        0     8070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/logical_sign.py
--rw-rw-rw-   0        0        0     5143 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/refactor.py
--rw-rw-rw-   0        0        0    17202 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/state.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.361915 quantum_pecos-0.6.0.dev1/python/pecos/slr/
--rw-rw-rw-   0        0        0     1170 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/__init__.py
--rw-rw-rw-   0        0        0     2062 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/block.py
--rw-rw-rw-   0        0        0     2688 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/cond_block.py
--rw-rw-rw-   0        0        0     3124 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/cops.py
--rw-rw-rw-   0        0        0      799 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/fund.py
--rw-rw-rw-   0        0        0     3541 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/misc.py
--rw-rw-rw-   0        0        0     1883 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/slr.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.362367 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/
--rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.368876 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/
--rw-rw-rw-   0        0        0      903 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/__init__.py
--rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/cliffords_tq.py
--rw-rw-rw-   0        0        0     1664 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/face_rots.py
--rw-rw-rw-   0        0        0      126 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/hadamards.py
--rw-rw-rw-   0        0        0     4539 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/metaclasses.py
--rw-rw-rw-   0        0        0      297 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/misc.py
--rw-rw-rw-   0        0        0     1272 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/paulis.py
--rw-rw-rw-   0        0        0      870 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/projective.py
--rw-rw-rw-   0        0        0      381 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/rots.py
--rw-rw-rw-   0        0        0      603 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/sqrt_paulis.py
--rw-rw-rw-   0        0        0      878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/util.py
--rw-rw-rw-   0        0        0     3530 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/slr/vars.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.377383 quantum_pecos-0.6.0.dev1/python/pecos/tools/
--rw-rw-rw-   0        0        0     1319 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/__init__.py
--rw-rw-rw-   0        0        0     6558 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/fault_tolerance_checking.py
--rw-rw-rw-   0        0        0    13635 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/fault_tolerance_checks.py
--rw-rw-rw-   0        0        0     5829 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/find_cliffs.py
--rw-rw-rw-   0        0        0     3384 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/logic_circuit_speed.py
--rw-rw-rw-   0        0        0     7186 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/pseudo_threshold_tools.py
--rw-rw-rw-   0        0        0     3630 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/random_circuit_speed.py
--rw-rw-rw-   0        0        0    32511 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/stabilizer_verification.py
--rw-rw-rw-   0        0        0    17415 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/threshold_tools.py
--rw-rw-rw-   0        0        0     1465 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/tool_anticommute.py
--rw-rw-rw-   0        0        0     6963 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/tools/tool_collection.py
--rw-rw-rw-   0        0        0     3802 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/python/pecos/typed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:59:06.381383 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/
--rw-rw-rw-   0        0        0    20835 2024-05-15 17:59:06.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11045 2024-05-15 17:59:06.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 17:59:06.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-15 23:26:47.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      471 2024-05-15 17:59:06.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 17:59:06.000000 quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      680 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 17:59:06.383882 quantum_pecos-0.6.0.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.268051 quantum_pecos-0.6.0.dev2/
+-rw-rw-rw-   0        0        0    11560 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/LICENSE
+-rw-rw-rw-   0        0        0      136 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/MANIFEST.in
+-rw-rw-rw-   0        0        0      463 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/NOTICE
+-rw-rw-rw-   0        0        0    20885 2024-05-20 17:24:01.267551 quantum_pecos-0.6.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     5198 2024-03-10 03:52:18.000000 quantum_pecos-0.6.0.dev2/README.md
+-rw-rw-rw-   0        0        0     3267 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.095383 quantum_pecos-0.6.0.dev2/python/
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.099883 quantum_pecos-0.6.0.dev2/python/pecos/
+-rw-rw-rw-   0        0        0     1907 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.102387 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/
+-rw-rw-rw-   0        0        0      942 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/__init__.py
+-rw-rw-rw-   0        0        0     9739 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/checks2circuit.py
+-rw-rw-rw-   0        0        0     5302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/std2chs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.105888 quantum_pecos-0.6.0.dev2/python/pecos/circuits/
+-rw-rw-rw-   0        0        0      911 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.112391 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/
+-rw-rw-rw-   0        0        0      671 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/__init__.py
+-rw-rw-rw-   0        0        0     1437 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/conditionals.py
+-rw-rw-rw-   0        0        0     1708 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/cops.py
+-rw-rw-rw-   0        0        0     1086 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/fund.py
+-rw-rw-rw-   0        0        0     1225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/hyqc.py
+-rw-rw-rw-   0        0        0     2830 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/int.py
+-rw-rw-rw-   0        0        0     1302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/misc_stmts.py
+-rw-rw-rw-   0        0        0     5680 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qops.py
+-rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qubits.py
+-rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/vars.py
+-rw-rw-rw-   0        0        0     5033 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/logical_circuit.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.119896 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/
+-rw-rw-rw-   0        0        0     1028 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/barrier.py
+-rw-rw-rw-   0        0        0     1070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/block.py
+-rw-rw-rw-   0        0        0     2283 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/conditionals.py
+-rw-rw-rw-   0        0        0     2020 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/expr.py
+-rw-rw-rw-   0        0        0      935 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/func.py
+-rw-rw-rw-   0        0        0     6986 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/gates.py
+-rw-rw-rw-   0        0        0     1592 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/misc.py
+-rw-rw-rw-   0        0        0     5616 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/qasm.py
+-rw-rw-rw-   0        0        0     1252 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/std_gates.py
+-rw-rw-rw-   0        0        0     2312 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/vars.py
+-rw-rw-rw-   0        0        0     9989 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qc2phir.py
+-rw-rw-rw-   0        0        0    14990 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/quantum_circuit.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.121973 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/classical_interpreter_abc.py
+-rw-rw-rw-   0        0        0    12692 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/phir_classical_interpreter.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.122900 quantum_pecos-0.6.0.dev2/python/pecos/decoders/
+-rw-rw-rw-   0        0        0      872 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.124399 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/
+-rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/__init__.py
+-rw-rw-rw-   0        0        0     1171 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/dummy_decoder.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.126399 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/__init__.py
+-rw-rw-rw-   0        0        0     5211 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/mwpm2d.py
+-rw-rw-rw-   0        0        0    17301 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/precomputing.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.128899 quantum_pecos-0.6.0.dev2/python/pecos/engines/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.130900 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/
+-rw-rw-rw-   0        0        0      885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/standard.py
+-rw-rw-rw-   0        0        0     2385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/timing_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.135404 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/__init__.py
+-rw-rw-rw-   0        0        0     8608 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray.py
+-rw-rw-rw-   0        0        0     5391 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray2.py
+-rw-rw-rw-   0        0        0     7544 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/classical.py
+-rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/cvm.py
+-rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/sim_func.py
+-rw-rw-rw-   0        0        0     4353 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.138404 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/__init__.py
+-rw-rw-rw-   0        0        0     1654 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm.py
+-rw-rw-rw-   0        0        0     1180 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm3.py
+-rw-rw-rw-   0        0        0     2728 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmer.py
+-rw-rw-rw-   0        0        0     1634 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmtime.py
+-rw-rw-rw-   0        0        0     7574 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine.py
+-rw-rw-rw-   0        0        0     4968 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_multiprocessing.py
+-rw-rw-rw-   0        0        0     8562 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_old.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.144908 quantum_pecos-0.6.0.dev2/python/pecos/error_models/
+-rw-rw-rw-   0        0        0     1109 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/__init__.py
+-rw-rw-rw-   0        0        0     1849 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/class_errors_circuit.py
+-rw-rw-rw-   0        0        0     5704 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/depolarizing_error_model.py
+-rw-rw-rw-   0        0        0     5604 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_depolar.py
+-rw-rw-rw-   0        0        0     1768 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model.py
+-rw-rw-rw-   0        0        0     1368 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model_abc.py
+-rw-rw-rw-   0        0        0     1035 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/fake_error_model.py
+-rw-rw-rw-   0        0        0     5851 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/generic_error_model.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.151908 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/__init__.py
+-rw-rw-rw-   0        0        0      958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip.py
+-rw-rw-rw-   0        0        0     1435 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py
+-rw-rw-rw-   0        0        0     1450 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip.py
+-rw-rw-rw-   0        0        0     1621 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py
+-rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_bitflip.py
+-rw-rw-rw-   0        0        0     1488 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py
+-rw-rw-rw-   0        0        0     1958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py
+-rw-rw-rw-   0        0        0     1761 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py
+-rw-rw-rw-   0        0        0     2490 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.157913 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/__init__.py
+-rw-rw-rw-   0        0        0     2546 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/gate_groups.py
+-rw-rw-rw-   0        0        0     1385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/init_noise.py
+-rw-rw-rw-   0        0        0     1593 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/meas_noise.py
+-rw-rw-rw-   0        0        0     1337 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/memory_noise.py
+-rw-rw-rw-   0        0        0     1207 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/sq_noise.py
+-rw-rw-rw-   0        0        0     2943 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/tq_noise.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.161914 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/
+-rw-rw-rw-   0        0        0      791 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/__init__.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/depolar_gen.py
+-rw-rw-rw-   0        0        0     5732 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/gatewise_gen.py
+-rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xerror_gen.py
+-rw-rw-rw-   0        0        0     7322 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xzerror_gen.py
+-rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/zerror_gen.py
+-rw-rw-rw-   0        0        0    11841 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/parent_class_error_gen.py
+-rw-rw-rw-   0        0        0     5100 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/simple_depolarizing_error_model.py
+-rw-rw-rw-   0        0        0     1026 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.166419 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/foreign_object_abc.py
+-rw-rw-rw-   0        0        0     2466 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/object_pool.py
+-rw-rw-rw-   0        0        0     1168 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/python.py
+-rw-rw-rw-   0        0        0      527 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasm_execution_timer_thread.py
+-rw-rw-rw-   0        0        0     3837 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmer.py
+-rw-rw-rw-   0        0        0     5054 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmtime.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.168418 quantum_pecos-0.6.0.dev2/python/pecos/machines/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/__init__.py
+-rw-rw-rw-   0        0        0     2356 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/generic_machine.py
+-rw-rw-rw-   0        0        0     1591 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/machine_abc.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.173419 quantum_pecos-0.6.0.dev2/python/pecos/misc/
+-rw-rw-rw-   0        0        0      840 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/__init__.py
+-rw-rw-rw-   0        0        0     2240 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/commute.py
+-rw-rw-rw-   0        0        0      838 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/errors.py
+-rw-rw-rw-   0        0        0     1681 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/gate_groups.py
+-rw-rw-rw-   0        0        0    10545 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/stabilizer_funcs.py
+-rw-rw-rw-   0        0        0     1992 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/std_output.py
+-rw-rw-rw-   0        0        0     3552 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/symbol_library.py
+-rw-rw-rw-   0        0        0     7419 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/threshold_curve.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.175423 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/__init__.py
+-rw-rw-rw-   0        0        0     2266 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/generic_op_processor.py
+-rw-rw-rw-   0        0        0     1132 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/op_processor_abc.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.179423 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/
+-rw-rw-rw-   0        0        0     1147 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.182923 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/__init__.py
+-rw-rw-rw-   0        0        0     7774 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/circuit_implementation1.py
+-rw-rw-rw-   0        0        0     7702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/color_488.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/gates.py
+-rw-rw-rw-   0        0        0     8975 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/instructions.py
+-rw-rw-rw-   0        0        0     3576 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/gate_parent_class.py
+-rw-rw-rw-   0        0        0     2262 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/helper_functions.py
+-rw-rw-rw-   0        0        0     3845 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/instruction_parent_class.py
+-rw-rw-rw-   0        0        0     7751 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/plot.py
+-rw-rw-rw-   0        0        0     8065 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/qecc_parent_class.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.185928 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/gates.py
+-rw-rw-rw-   0        0        0    11245 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/instructions.py
+-rw-rw-rw-   0        0        0     9623 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/surface_4444.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.188428 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/gates.py
+-rw-rw-rw-   0        0        0    19744 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/instructions.py
+-rw-rw-rw-   0        0        0    10241 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.188928 quantum_pecos-0.6.0.dev2/python/pecos/reps/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.194428 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/
+-rw-rw-rw-   0        0        0      675 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/block_types.py
+-rw-rw-rw-   0        0        0     1961 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/data_types.py
+-rw-rw-rw-   0        0        0      236 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/instr_type.py
+-rw-rw-rw-   0        0        0     1104 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/list_types.py
+-rw-rw-rw-   0        0        0     1103 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/name_resolver.py
+-rw-rw-rw-   0        0        0     3167 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/op_types.py
+-rw-rw-rw-   0        0        0    10789 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/pypmir.py
+-rw-rw-rw-   0        0        0      812 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/types.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.198434 quantum_pecos-0.6.0.dev2/python/pecos/simulators/
+-rw-rw-rw-   0        0        0     1878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.201435 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/
+-rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/bindings.py
+-rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/gates.py
+-rw-rw-rw-   0        0        0     1773 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/state.py
+-rw-rw-rw-   0        0        0     2185 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/compile_cython.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.202934 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/
+-rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuconn.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.203434 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/
+-rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.204934 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/
+-rw-rw-rw-   0        0        0      624 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py
+-rw-rw-rw-   0        0        0     4489 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.208938 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/bindings.py
+-rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py
+-rw-rw-rw-   0        0        0      785 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py
+-rw-rw-rw-   0        0        0     3562 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py
+-rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py
+-rw-rw-rw-   0        0        0     1874 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/state.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.213939 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/
+-rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/__init__.py
+-rw-rw-rw-   0        0        0     1769 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/bindings.py
+-rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_init.py
+-rw-rw-rw-   0        0        0     1867 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_meas.py
+-rw-rw-rw-   0        0        0     9594 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_one_qubit.py
+-rw-rw-rw-   0        0        0    12354 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     3719 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/state.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.214939 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.215438 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/__init__.py
+-rw-rw-rw-   0        0        0     6362 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/logical_sign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.218021 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/__init__.py
+-rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.219527 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/__init__.py
+-rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/logical_sign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.221031 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/__init__.py
+-rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.222531 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/__init__.py
+-rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/logical_sign.py
+-rw-rw-rw-   0        0        0     2736 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/gate_syms.py
+-rw-rw-rw-   0        0        0     2691 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/parent_sim_classes.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.228036 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/
+-rw-rw-rw-   0        0        0      710 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/__init__.py
+-rw-rw-rw-   0        0        0     2945 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/bindings.py
+-rw-rw-rw-   0        0        0      881 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_init.py
+-rw-rw-rw-   0        0        0     2985 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_meas.py
+-rw-rw-rw-   0        0        0    14031 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_one_qubit.py
+-rw-rw-rw-   0        0        0     7900 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/logical_sign.py
+-rw-rw-rw-   0        0        0     9712 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/state.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.234536 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/
+-rw-rw-rw-   0        0        0      859 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/__init__.py
+-rw-rw-rw-   0        0        0     4891 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/bindings.py
+-rw-rw-rw-   0        0        0     2213 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_init.py
+-rw-rw-rw-   0        0        0     2631 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_meas.py
+-rw-rw-rw-   0        0        0     6819 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_one_qubit.py
+-rw-rw-rw-   0        0        0     4884 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     1205 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/helper.py
+-rw-rw-rw-   0        0        0     2379 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/logical_sign.py
+-rw-rw-rw-   0        0        0     4977 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/state.py
+-rw-rw-rw-   0        0        0     2885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/quantum_simulator.py
+-rw-rw-rw-   0        0        0     1409 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sim_class_types.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.240541 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/
+-rw-rw-rw-   0        0        0     1933 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/bindings.py
+-rw-rw-rw-   0        0        0     3225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_init.py
+-rw-rw-rw-   0        0        0    11606 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_meas.py
+-rw-rw-rw-   0        0        0    33702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_one_qubit.py
+-rw-rw-rw-   0        0        0    15954 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_two_qubit.py
+-rw-rw-rw-   0        0        0     8070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/logical_sign.py
+-rw-rw-rw-   0        0        0     5143 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/refactor.py
+-rw-rw-rw-   0        0        0    17202 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/state.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.246541 quantum_pecos-0.6.0.dev2/python/pecos/slr/
+-rw-rw-rw-   0        0        0     1170 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/__init__.py
+-rw-rw-rw-   0        0        0     2062 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/block.py
+-rw-rw-rw-   0        0        0     2688 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/cond_block.py
+-rw-rw-rw-   0        0        0     3124 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/cops.py
+-rw-rw-rw-   0        0        0      799 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/fund.py
+-rw-rw-rw-   0        0        0     3541 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/misc.py
+-rw-rw-rw-   0        0        0     1883 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/slr.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.247041 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/
+-rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.254046 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/
+-rw-rw-rw-   0        0        0      903 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/__init__.py
+-rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/cliffords_tq.py
+-rw-rw-rw-   0        0        0     1664 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/face_rots.py
+-rw-rw-rw-   0        0        0      126 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/hadamards.py
+-rw-rw-rw-   0        0        0     4539 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/metaclasses.py
+-rw-rw-rw-   0        0        0      297 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/misc.py
+-rw-rw-rw-   0        0        0     1272 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/paulis.py
+-rw-rw-rw-   0        0        0      870 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/projective.py
+-rw-rw-rw-   0        0        0      381 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/rots.py
+-rw-rw-rw-   0        0        0      603 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/sqrt_paulis.py
+-rw-rw-rw-   0        0        0      878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/util.py
+-rw-rw-rw-   0        0        0     3530 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/vars.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.262051 quantum_pecos-0.6.0.dev2/python/pecos/tools/
+-rw-rw-rw-   0        0        0     1319 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/__init__.py
+-rw-rw-rw-   0        0        0     6558 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checking.py
+-rw-rw-rw-   0        0        0    13635 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checks.py
+-rw-rw-rw-   0        0        0     5829 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/find_cliffs.py
+-rw-rw-rw-   0        0        0     3384 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/logic_circuit_speed.py
+-rw-rw-rw-   0        0        0     7186 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/pseudo_threshold_tools.py
+-rw-rw-rw-   0        0        0     3630 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/random_circuit_speed.py
+-rw-rw-rw-   0        0        0    32511 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/stabilizer_verification.py
+-rw-rw-rw-   0        0        0    17415 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/threshold_tools.py
+-rw-rw-rw-   0        0        0     1465 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_anticommute.py
+-rw-rw-rw-   0        0        0     6963 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_collection.py
+-rw-rw-rw-   0        0        0     3802 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/typed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.266051 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/
+-rw-rw-rw-   0        0        0    20885 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11045 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-15 23:26:47.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      487 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:24:01.268051 quantum_pecos-0.6.0.dev2/setup.cfg
```

### Comparing `quantum_pecos-0.6.0.dev1/LICENSE` & `quantum_pecos-0.6.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/PKG-INFO` & `quantum_pecos-0.6.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-pecos
-Version: 0.6.0.dev1
+Version: 0.6.0.dev2
 Summary: PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond.
 Author: The PECOS Developers
 Maintainer-email: Ciaran Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -220,15 +220,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: phir~=0.3.0
+Requires-Dist: phir<0.4,>=0.3.3
 Requires-Dist: numpy<2.0,>=1.15.0
 Requires-Dist: scipy<2.0,>=1.1.0
 Requires-Dist: networkx<3.0,>=2.1.0
 Requires-Dist: matplotlib<4.0,>=2.2.0
 Provides-Extra: simulators
 Requires-Dist: cython; extra == "simulators"
 Requires-Dist: pybind11<3.0,>=2.2.3; extra == "simulators"
@@ -241,14 +241,15 @@
 Provides-Extra: wasmer
 Requires-Dist: wasmer~=1.1.0; extra == "wasmer"
 Requires-Dist: wasmer_compiler_cranelift~=1.1.0; extra == "wasmer"
 Provides-Extra: visualization
 Requires-Dist: plotly~=5.9.0; extra == "visualization"
 Provides-Extra: tests
 Requires-Dist: pytest>=5.0.0; extra == "tests"
+Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
 Requires-Dist: quantum-pecos[simulators]; extra == "all"
 Requires-Dist: quantum-pecos[wasmtime]; extra == "all"
 Requires-Dist: quantum-pecos[wasmer]; extra == "all"
 Requires-Dist: quantum-pecos[visualization]; extra == "all"
 Requires-Dist: quantum-pecos[tests]; extra == "all"
```

### Comparing `quantum_pecos-0.6.0.dev1/README.md` & `quantum_pecos-0.6.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/pyproject.toml` & `quantum_pecos-0.6.0.dev2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 [build-system]
 requires = ["setuptools>=62.6"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quantum-pecos"
-version = "0.6.0.dev1"
+version = "0.6.0.dev2"
 authors = [
     {name = "The PECOS Developers"},
 ]
 maintainers =[
     {name = "Ciaran Ryan-Anderson", email = "ciaran.ryan-anderson@quantinuum.com"},
 ]
 description = """PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond."""
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE"}
 keywords = ["quantum", "QEC", "simulation", "PECOS"]
 dependencies = [
-    "phir~=0.3.0",
+    "phir>=0.3.3,<0.4",
     "numpy>=1.15.0,<2.0",
     "scipy>=1.1.0,<2.0",
     "networkx>=2.1.0,<3.0",
     "matplotlib>=2.2.0,<4.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -69,15 +69,16 @@
     "wasmer~=1.1.0",
     "wasmer_compiler_cranelift~=1.1.0",
 ]
 visualization = [
     "plotly~=5.9.0",
 ]
 tests = [
-    "pytest>=5.0.0"
+    "pytest>=5.0.0",
+    "hypothesis"
 ]
 all = [
     "quantum-pecos[simulators]",
     "quantum-pecos[wasmtime]",
     "quantum-pecos[wasmer]",
     "quantum-pecos[visualization]",
     "quantum-pecos[tests]",
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 except PackageNotFoundError:
     __version__ = "0.0.0"
 
 # PECOS namespaces
 from pecos import circuit_converters, circuits, decoders, engines, error_models, misc, qeccs, simulators, tools
 from pecos.circuits.quantum_circuit import QuantumCircuit
 from pecos.engines import circuit_runners
-from pecos.engines.cvm.binarray import BinArray
+from pecos.engines.cvm.binarray2 import BinArray2 as BinArray
 from pecos.engines.hybrid_engine_old import HybridEngine
 
 __all__ = [
     "__version__",
     "circuits",
     "qeccs",
     "simulators",
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/checks2circuit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/checks2circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuit_converters/std2chs.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/std2chs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/conditionals.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/conditionals.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/cops.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/cops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/fund.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/fund.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/hyqc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/hyqc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/int.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/int.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/misc_stmts.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/misc_stmts.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/qops.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/qubits.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qubits.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/hyqc/vars.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/logical_circuit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/logical_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/barrier.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/barrier.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/block.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/conditionals.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/conditionals.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/expr.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/expr.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/func.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/func.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/misc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/misc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/qasm.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/std_gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/std_gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qasm/vars.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/qc2phir.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qc2phir.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/circuits/quantum_circuit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/circuits/quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/classical_interpreter_abc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/classical_interpreter_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/classical_interpreters/phir_classical_interpreter.py` & `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/phir_classical_interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,43 +11,33 @@
 
 from __future__ import annotations
 
 import json
 import warnings
 from typing import TYPE_CHECKING, Any
 
-import numpy as np
 from phir.model import PHIRModel
 
 from pecos.classical_interpreters.classical_interpreter_abc import ClassicalInterpreter
-from pecos.reps.pypmir import PyPMIR
+from pecos.reps.pypmir import PyPMIR, signed_data_types, unsigned_data_types
 from pecos.reps.pypmir import types as pt
 
 if TYPE_CHECKING:
     from collections.abc import Generator, Iterable, Sequence
 
     from pecos import QuantumCircuit
     from pecos.foreign_objects.foreign_object_abc import ForeignObject
 
 
 def version2tuple(v):
     """Get version tuple from string."""
     return tuple(map(int, (v.split("."))))
 
 
-data_type_map = {
-    "i8": np.int8,
-    "i16": np.int16,
-    "i32": np.int32,
-    "i64": np.int64,
-    "u8": np.uint8,
-    "u16": np.uint16,
-    "u32": np.uint32,
-    "u64": np.uint64,
-}
+data_type_map = signed_data_types | unsigned_data_types
 
 data_type_map_rev = {v: k for k, v in data_type_map.items()}
 
 
 class PHIRClassicalInterpreter(ClassicalInterpreter):
     """An interpreter that takes in a PHIR program and runs the classical side of the program."""
 
@@ -272,26 +262,28 @@
     def assign_int(self, cvar, val: int):
         i = None
         if isinstance(cvar, (tuple, list)):
             cvar, i = cvar
 
         cid = self.csym2id[cvar]
         dtype = self.cid2dtype[cid]
-        size = self.cvar_meta[cid].size
 
         cval = self.cenv[cid]
         val = dtype(val)
         if i is None:
             cval = val
         else:
             cval &= ~(1 << i)
             cval |= (val & 1) << i
 
-        # mask off bits give the size of the register
-        cval &= (1 << size) - 1
+        if type(cval) not in signed_data_types.values():
+            # mask off bits given the size of the register
+            # (only valid for unsigned data types)
+            size = self.cvar_meta[cid].size
+            cval &= (1 << size) - 1
         self.cenv[cid] = cval
 
     def handle_cops(self, op):
         """Handle the processing of classical operations."""
 
         if op.name == "=":
             args = []
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/dummy_decoder/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/dummy_decoder/dummy_decoder.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/dummy_decoder.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/mwpm2d.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/mwpm2d.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/decoders/mwpm2d/precomputing.py` & `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/precomputing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/standard.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/standard.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/circuit_runners/timing_runner.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/timing_runner.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/binarray.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/binarray2.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from __future__ import annotations
 
 import numpy as np
 
+from pecos.reps.pypmir import unsigned_data_types
+
 
 class BinArray2:
-    def __init__(self, size, value=0, dtype=np.int32) -> None:
+    """As opposed to the original unsigned 32-bit BinArray, this class defaults to signed 64-bit type."""
+
+    def __init__(self, size, value=0, dtype=np.int64) -> None:
         self.size = size
         self.value = None
         self.dtype = dtype
 
         if isinstance(size, int):
             self.size = size
 
@@ -29,23 +33,26 @@
             self.size = len(size)
             value = int(size, 2)
             self.set(value)
 
     def set(self, value):
         if isinstance(value, self.dtype):
             self.value = value
+        elif isinstance(value, BinArray2):
+            self.value = value.value
         else:
             if isinstance(value, str):
                 value = int(value, 2)
 
             self.value = self.dtype(value)
 
     def new_val(self, value):
         b = BinArray2(self.size, value, self.dtype)
-        b.clamp(self.size)
+        if self.dtype in unsigned_data_types.values():
+            b.clamp(self.size)
         return b
 
     def num_bits(self):
         return len(f"{self.value:b}")
 
     def check_size(self):
         if self.num_bits() > self.size:
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/classical.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/classical.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from __future__ import annotations
 
-from pecos.engines.cvm.binarray import BinArray
+from pecos.engines.cvm.binarray2 import BinArray2 as BinArray
 
 
 def set_output(state, circuit, output_spec, output):
     if output_spec is None:
         output_spec = {}
 
     output_spec["__pecos_scratch"] = state.num_qubits
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/cvm.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/cvm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/sim_func.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/sim_func.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import pickle
 from pathlib import Path
 
-from pecos.engines.cvm.binarray import BinArray
+from pecos.engines.cvm.binarray2 import BinArray2 as BinArray
 from pecos.engines.cvm.sim_func import sim_exec
 from pecos.engines.cvm.wasm_vms.pywasm import read_pywasm
 from pecos.engines.cvm.wasm_vms.pywasm3 import read_pywasm3
 from pecos.engines.cvm.wasm_vms.wasmer import read_wasmer
 from pecos.engines.cvm.wasm_vms.wasmtime import read_wasmtime
 from pecos.errors import MissingCCOPError
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/pywasm.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/pywasm3.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm3.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/wasmer.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmer.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/cvm/wasm_vms/wasmtime.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmtime.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine_multiprocessing.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/engines/hybrid_engine_old.py` & `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_old.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 import os
 import random
 import struct
 
 import numpy as np
 
-from pecos.engines.cvm.classical import BinArray, eval_condition, eval_cop, set_output
+from pecos.engines.cvm.binarray2 import BinArray2 as BinArray
+from pecos.engines.cvm.classical import eval_condition, eval_cop, set_output
 from pecos.engines.cvm.wasm import eval_cfunc, get_ccop
 from pecos.error_models.fake_error_model import FakeErrorModel
 from pecos.errors import NotSupportedGateError
 
 
 class HybridEngine:
     """This class represents a standard model for running quantum circuits and adding in errors."""
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/class_errors_circuit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/class_errors_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/depolarizing_error_model.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/depolarizing_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_depolar.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_depolar.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_model.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/error_model_abc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/fake_error_model.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/fake_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/generic_error_model.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/generic_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_initz_bitflip.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_meas_bitflip.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_bitflip.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/gate_groups.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/gate_groups.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/init_noise.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/init_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/meas_noise.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/meas_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/memory_noise.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/memory_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/sq_noise.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/sq_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/noise_impl_old/tq_noise.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/tq_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/depolar_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/depolar_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/gatewise_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/gatewise_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/xerror_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/xzerror_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xzerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/old/zerror_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/zerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/parent_class_error_gen.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/parent_class_error_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/error_models/simple_depolarizing_error_model.py` & `quantum_pecos-0.6.0.dev2/python/pecos/error_models/simple_depolarizing_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/errors.py` & `quantum_pecos-0.6.0.dev2/python/pecos/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/foreign_object_abc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/foreign_object_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/object_pool.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/object_pool.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/python.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/python.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasm_execution_timer_thread.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasm_execution_timer_thread.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasmer.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmer.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/foreign_objects/wasmtime.py` & `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmtime.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/machines/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/machines/generic_machine.py` & `quantum_pecos-0.6.0.dev2/python/pecos/machines/generic_machine.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/machines/machine_abc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/machines/machine_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/commute.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/commute.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/errors.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/gate_groups.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/gate_groups.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/stabilizer_funcs.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/stabilizer_funcs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/std_output.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/std_output.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/symbol_library.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/symbol_library.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/misc/threshold_curve.py` & `quantum_pecos-0.6.0.dev2/python/pecos/misc/threshold_curve.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/op_processors/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/op_processors/generic_op_processor.py` & `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/generic_op_processor.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/op_processors/op_processor_abc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/op_processor_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/circuit_implementation1.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/circuit_implementation1.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/color_488.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/color_488.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/color_488/instructions.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/gate_parent_class.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/gate_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/helper_functions.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/helper_functions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/instruction_parent_class.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/instruction_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/plot.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/plot.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/qecc_parent_class.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/qecc_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/instructions.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_4444/surface_4444.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/surface_4444.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/instructions.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py` & `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-from pecos.reps.pypmir.pypmir import PyPMIR
+from pecos.reps.pypmir.pypmir import PyPMIR, signed_data_types, unsigned_data_types
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/block_types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/block_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/data_types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/data_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/list_types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/list_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/name_resolver.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/name_resolver.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/op_types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/op_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/pypmir.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/pypmir.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,40 @@
 
 
 from __future__ import annotations
 
 from math import pi
 from typing import TYPE_CHECKING, Callable, TypeVar
 
+import numpy as np
+
 from pecos.reps.pypmir import block_types as blk
 from pecos.reps.pypmir import data_types as d
 from pecos.reps.pypmir import op_types as op
 from pecos.reps.pypmir.name_resolver import sim_name_resolver
 
 if TYPE_CHECKING:
     from pecos.reps.pypmir.op_types import QOp
 
 TypeOp = TypeVar("TypeOp", bound=op.Op)
 
+signed_data_types = {
+    "i8": np.int8,
+    "i16": np.int16,
+    "i32": np.int32,
+    "i64": np.int64,
+}
+
+unsigned_data_types = {
+    "u8": np.uint8,
+    "u16": np.uint16,
+    "u32": np.uint32,
+    "u64": np.uint64,
+}
+
 
 class PyPMIR:
     """Pythonic PECOS Middle-level IR. Used to convert PHIR into an object and optimize the data structure for
     simulations.
     """
 
     def __init__(self, metadata: dict | None = None, name_resolver: Callable[[QOp], str] | None = None) -> None:
@@ -225,18 +241,22 @@
         next_qvar_int = 0
 
         for o in phir["ops"]:
             if "data" in o:
                 name = o["data"]
 
                 if name == "cvar_define":
+                    data_type = o["data_type"]
+                    size = int(data_type[1:])
+                    if "size" in o:
+                        size = o["size"]
                     data = d.CVarDefine(
-                        data_type=o["data_type"],
+                        data_type=data_type,
                         variable=o["variable"],
-                        size=o["size"],
+                        size=size,
                         cvar_id=len(p.cvar_meta),
                         metadata=o.get("metadata"),
                     )
 
                     p.cvar_meta.append(data)
                     p.csym2id[data.variable] = data.cvar_id
                     p.cvar_dtypes_set.add(data.data_type)
```

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/reps/pypmir/types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/gates.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cointoss/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/compile_cython.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/compile_cython.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuconn.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuconn.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cuquantum_old/custatevec/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_init.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_meas.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/custatevec/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/setup.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/src/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim/src/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/setup.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/src/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_col/src/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/setup.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/src/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/cysparsesim_row/src/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/gate_syms.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/gate_syms.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/parent_sim_classes.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/parent_sim_classes.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_init.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_meas.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/paulifaultprop/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_init.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_meas.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/helper.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/helper.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/projectq/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/quantum_simulator.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/quantum_simulator.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sim_class_types.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sim_class_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/bindings.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_init.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_meas.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_one_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/cmd_two_qubit.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/logical_sign.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/refactor.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/refactor.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/simulators/sparsesim/state.py` & `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/block.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/cond_block.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/cond_block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/cops.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/cops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/fund.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/fund.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/misc.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/misc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/slr.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/slr.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/cliffords_tq.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/cliffords_tq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/face_rots.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/face_rots.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/metaclasses.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/paulis.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/paulis.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/projective.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/projective.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/std/phys/sqrt_paulis.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/sqrt_paulis.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/util.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/util.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/slr/vars.py` & `quantum_pecos-0.6.0.dev2/python/pecos/slr/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/__init__.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/fault_tolerance_checking.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checking.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/fault_tolerance_checks.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checks.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/find_cliffs.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/find_cliffs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/logic_circuit_speed.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/logic_circuit_speed.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/pseudo_threshold_tools.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/pseudo_threshold_tools.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/random_circuit_speed.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/random_circuit_speed.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/stabilizer_verification.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/stabilizer_verification.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/threshold_tools.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/threshold_tools.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/tool_anticommute.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_anticommute.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/tools/tool_collection.py` & `quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_collection.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/pecos/typed_list.py` & `quantum_pecos-0.6.0.dev2/python/pecos/typed_list.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/PKG-INFO` & `quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-pecos
-Version: 0.6.0.dev1
+Version: 0.6.0.dev2
 Summary: PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond.
 Author: The PECOS Developers
 Maintainer-email: Ciaran Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -220,15 +220,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: phir~=0.3.0
+Requires-Dist: phir<0.4,>=0.3.3
 Requires-Dist: numpy<2.0,>=1.15.0
 Requires-Dist: scipy<2.0,>=1.1.0
 Requires-Dist: networkx<3.0,>=2.1.0
 Requires-Dist: matplotlib<4.0,>=2.2.0
 Provides-Extra: simulators
 Requires-Dist: cython; extra == "simulators"
 Requires-Dist: pybind11<3.0,>=2.2.3; extra == "simulators"
@@ -241,14 +241,15 @@
 Provides-Extra: wasmer
 Requires-Dist: wasmer~=1.1.0; extra == "wasmer"
 Requires-Dist: wasmer_compiler_cranelift~=1.1.0; extra == "wasmer"
 Provides-Extra: visualization
 Requires-Dist: plotly~=5.9.0; extra == "visualization"
 Provides-Extra: tests
 Requires-Dist: pytest>=5.0.0; extra == "tests"
+Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
 Requires-Dist: quantum-pecos[simulators]; extra == "all"
 Requires-Dist: quantum-pecos[wasmtime]; extra == "all"
 Requires-Dist: quantum-pecos[wasmer]; extra == "all"
 Requires-Dist: quantum-pecos[visualization]; extra == "all"
 Requires-Dist: quantum-pecos[tests]; extra == "all"
```

### Comparing `quantum_pecos-0.6.0.dev1/python/quantum_pecos.egg-info/SOURCES.txt` & `quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

