# Comparing `tmp/nbed-0.0.3.tar.gz` & `tmp/nbed-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbed-0.0.3.tar", max compression
+gzip compressed data, was "nbed-0.0.4.tar", max compression
```

## Comparing `nbed-0.0.3.tar` & `nbed-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4563 2023-12-05 23:06:47.013455 nbed-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     6148 2023-12-01 12:45:01.979152 nbed-0.0.3/nbed/.DS_Store
--rw-r--r--   0        0        0      182 2023-12-01 12:45:01.979209 nbed-0.0.3/nbed/__init__.py
--rw-r--r--   0        0        0    42462 2023-12-06 20:03:33.608069 nbed-0.0.3/nbed/driver.py
--rw-r--r--   0        0        0     6952 2023-12-05 23:06:47.026185 nbed-0.0.3/nbed/embed.py
--rw-r--r--   0        0        0      494 2023-12-05 23:06:47.026286 nbed-0.0.3/nbed/exceptions.py
--rw-r--r--   0        0        0    24261 2023-12-06 20:40:46.399408 nbed-0.0.3/nbed/ham_builder.py
--rw-r--r--   0        0        0     9032 2023-12-05 23:06:47.026947 nbed-0.0.3/nbed/ham_converter.py
--rw-r--r--   0        0        0      267 2023-12-01 12:45:01.979682 nbed-0.0.3/nbed/localizers/__init__.py
--rw-r--r--   0        0        0     9183 2023-12-05 23:06:47.027151 nbed-0.0.3/nbed/localizers/base.py
--rw-r--r--   0        0        0    17078 2023-12-05 23:06:47.027438 nbed-0.0.3/nbed/localizers/pyscf.py
--rw-r--r--   0        0        0     9394 2023-12-05 23:06:47.027772 nbed-0.0.3/nbed/localizers/spade.py
--rw-r--r--   0        0        0     3683 2023-12-05 23:06:47.027892 nbed-0.0.3/nbed/mol_plot.py
--rw-r--r--   0        0        0      230 2023-12-05 23:06:47.028109 nbed-0.0.3/nbed/scf/__init__.py
--rw-r--r--   0        0        0     2633 2023-12-05 23:06:47.028276 nbed-0.0.3/nbed/scf/embedded_hcore_funcs.py
--rw-r--r--   0        0        0     5532 2023-12-05 23:06:47.028519 nbed-0.0.3/nbed/scf/huzinaga_hf.py
--rw-r--r--   0        0        0     6154 2023-12-05 23:06:47.028611 nbed-0.0.3/nbed/scf/huzinaga_ks.py
--rw-r--r--   0        0        0    17965 2023-12-05 23:06:47.028913 nbed-0.0.3/nbed/utils.py
--rw-r--r--   0        0        0     1397 2023-12-06 22:02:21.451658 nbed-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 nbed-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4563 2023-12-05 23:06:47.013455 nbed-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     6148 2023-12-01 12:45:01.979152 nbed-0.0.4/nbed/.DS_Store
+-rw-r--r--   0        0        0      182 2023-12-01 12:45:01.979209 nbed-0.0.4/nbed/__init__.py
+-rw-r--r--   0        0        0    42705 2024-05-17 14:13:50.199607 nbed-0.0.4/nbed/driver.py
+-rw-r--r--   0        0        0     6952 2024-02-21 11:24:54.910982 nbed-0.0.4/nbed/embed.py
+-rw-r--r--   0        0        0      494 2023-12-05 23:06:47.026286 nbed-0.0.4/nbed/exceptions.py
+-rw-r--r--   0        0        0    24510 2024-05-17 15:05:01.193327 nbed-0.0.4/nbed/ham_builder.py
+-rw-r--r--   0        0        0     9032 2023-12-05 23:06:47.026947 nbed-0.0.4/nbed/ham_converter.py
+-rw-r--r--   0        0        0      267 2023-12-01 12:45:01.979682 nbed-0.0.4/nbed/localizers/__init__.py
+-rw-r--r--   0        0        0     9183 2023-12-05 23:06:47.027151 nbed-0.0.4/nbed/localizers/base.py
+-rw-r--r--   0        0        0    17078 2023-12-07 15:04:42.222953 nbed-0.0.4/nbed/localizers/pyscf.py
+-rw-r--r--   0        0        0    10566 2024-05-17 15:05:01.193773 nbed-0.0.4/nbed/localizers/spade.py
+-rw-r--r--   0        0        0     3683 2023-12-05 23:06:47.027892 nbed-0.0.4/nbed/mol_plot.py
+-rw-r--r--   0        0        0      230 2023-12-05 23:06:47.028109 nbed-0.0.4/nbed/scf/__init__.py
+-rw-r--r--   0        0        0     2613 2024-05-17 15:05:01.194084 nbed-0.0.4/nbed/scf/embedded_hcore_funcs.py
+-rw-r--r--   0        0        0     5532 2023-12-05 23:06:47.028519 nbed-0.0.4/nbed/scf/huzinaga_hf.py
+-rw-r--r--   0        0        0     6154 2023-12-05 23:06:47.028611 nbed-0.0.4/nbed/scf/huzinaga_ks.py
+-rw-r--r--   0        0        0    17965 2023-12-05 23:06:47.028913 nbed-0.0.4/nbed/utils.py
+-rw-r--r--   0        0        0     1458 2024-05-17 15:05:01.194350 nbed-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 nbed-0.0.4/PKG-INFO
```

### Comparing `nbed-0.0.3/LICENSE.md` & `nbed-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/.DS_Store` & `nbed-0.0.4/nbed/.DS_Store`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/driver.py` & `nbed-0.0.4/nbed/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 class NbedDriver:
     """Function to return the embedding Qubit Hamiltonian.
 
     Args:
         geometry (str): Path to .xyz file containing molecular geometry or raw xyz string.
         n_active_atoms (int): The number of atoms to include in the active region.
         basis (str): The name of an atomic orbital basis set to use for chemistry calculations.
-        xc_functonal (str): The name of an Exchange-Correlation functional to be used for DFT.
+        xc_functional (str): The name of an Exchange-Correlation functional to be used for DFT.
         projector (str): Projector to screen out environment orbitals, One of 'mu' or 'huzinaga'.
         localization (str): Orbital localization method to use. One of 'spade', 'pipek-mezey', 'boys' or 'ibo'.
         convergence (float): The convergence tolerance for energy calculations.
         charge (int): Charge of molecular species
         mu_level_shift (float): Level shift parameter to use for mu-projector.
         run_ccsd_emb (bool): Whether or not to find the CCSD energy of embbeded system for reference.
         run_fci_emb (bool): Whether or not to find the FCI energy of embbeded system for reference.
@@ -99,15 +99,15 @@
         localization: Optional[str] = "spade",
         convergence: Optional[float] = 1e-6,
         charge: Optional[int] = 0,
         spin: Optional[int] = 0,
         mu_level_shift: Optional[float] = 1e6,
         run_ccsd_emb: Optional[bool] = False,
         run_fci_emb: Optional[bool] = False,
-        run_virtual_localization: Optional[bool] = False,
+        run_virtual_localization: Optional[bool] = True,
         run_dft_in_dft: Optional[bool] = False,
         max_ram_memory: Optional[int] = 4000,
         pyscf_print_level: int = 1,
         unit: Optional[str] = "angstrom",
         occupied_threshold: Optional[float] = 0.95,
         virtual_threshold: Optional[float] = 0.95,
         max_shells: Optional[int] = 4,
@@ -267,15 +267,15 @@
 
     @cached_property
     def _global_ks(self):
         """Method to run full cheap molecule RKS DFT calculation.
 
         Note this is necessary to perform localization procedure.
         """
-        logger.debug("Running full system RKS DFT.")
+        logger.debug("Running full system KS DFT.")
         mol_full = self._build_mol()
 
         global_ks = scf.RKS(mol_full) if self._restricted_scf else scf.UKS(mol_full)
         logger.debug(f"{type(global_ks)}")
         global_ks.conv_tol = self.convergence
         global_ks.xc = self.xc_functional
         global_ks.max_memory = self.max_ram_memory
@@ -357,15 +357,15 @@
 
     def _init_local_ks(self, xc_functional: str) -> Union[dft.uks.UKS, dft.rks.RKS]:
         """Function to build embedded Hartree Fock object for active subsystem.
 
         Note this function overwrites the total number of electrons to only include active number.
 
         Args:
-            xc_functonal (str): XC functional to use in embedded calculation.
+            xc_functional (str): XC functional to use in embedded calculation.
 
         Returns:
             local_ks (pyscf.dft.rks.RKS or pyscf.dft.uks.UKS): embedded Kohn-Sham DFT object.
         """
         logger.debug("Initialising localised RKS object.")
         embedded_mol: gto.Mole = self._build_mol()
 
@@ -524,65 +524,73 @@
             env_projector = np.array([env_projector_alpha, env_projector_beta])
 
         return env_projector
 
     def _run_emb_CCSD(
         self,
         emb_pyscf_scf_rhf: Union[scf.RHF, scf.UHF],
-        frozen_orb_list: Optional[list] = None,
+        frozen: Optional[list] = None,
     ) -> Tuple[cc.CCSD, float]:
         """Function run CCSD on embedded restricted Hartree Fock object.
 
         Note emb_pyscf_scf_rhf is RHF object for the active embedded subsystem (defined in localized basis)
         (see get_embedded_rhf method)
 
         Args:
             emb_pyscf_scf_rhf (scf.RHF): PySCF restricted Hartree Fock object of active embedded subsystem
-            frozen_orb_list (List): A path to an .xyz file describing molecular geometry.
+            frozen (List): A path to an .xyz file describing molecular geometry.
 
         Returns:
             ccsd (cc.CCSD): PySCF CCSD object
             e_ccsd_corr (float): electron correlation CCSD energy
         """
         logger.debug("Starting embedded CCSD calculation.")
-        ccsd = cc.CCSD(emb_pyscf_scf_rhf)
+        ccsd = cc.CCSD(emb_pyscf_scf_rhf, frozen=frozen)
         ccsd.conv_tol = self.convergence
         ccsd.max_memory = self.max_ram_memory
         ccsd.verbose = self.pyscf_print_level
 
-        # Set which orbitals are to be frozen
-        ccsd.frozen = frozen_orb_list
         e_ccsd_corr, _, _ = ccsd.kernel()
         logger.info(f"Embedded CCSD energy: {e_ccsd_corr}")
         return ccsd, e_ccsd_corr
 
     def _run_emb_FCI(
         self,
         emb_pyscf_scf_rhf: Union[scf.RHF, scf.UHF],
-        frozen_orb_list: Optional[list] = None,
+        frozen: Optional[list] = None,
     ) -> fci.FCI:
         """Function run FCI on embedded restricted Hartree Fock object.
 
         Note emb_pyscf_scf_rhf is RHF object for the active embedded subsystem (defined in localized basis)
         (see get_embedded_rhf method)
 
         Args:
             emb_pyscf_scf_rhf (scf.RHF): PySCF restricted Hartree Fock object of active embedded subsystem
-            frozen_orb_list (List): A path to an .xyz file describing moleclar geometry.
+            frozen (List): A path to an .xyz file describing moleclar geometry.
 
         Returns:
             fci_scf (fci.FCI): PySCF FCI object
         """
         logger.debug("Starting embedded FCI calculation.")
-        fci_scf = fci.FCI(emb_pyscf_scf_rhf)
+        if frozen is None:
+            fci_scf = fci.FCI(emb_pyscf_scf_rhf)
+        else:
+            from pyscf import mcscf
+
+            fci_scf = mcscf.CASSCF(
+                emb_pyscf_scf_rhf,
+                emb_pyscf_scf_rhf.mol.nelec,
+                emb_pyscf_scf_rhf.mol.nao - len(frozen),
+            )
+            fci_scf.sort_mo(
+                [i + 1 for i in range(emb_pyscf_scf_rhf.mol.nao) if i not in frozen]
+            )
         fci_scf.conv_tol = self.convergence
         fci_scf.verbose = self.pyscf_print_level
         fci_scf.max_memory = self.max_ram_memory
-
-        fci_scf.frozen = frozen_orb_list
         fci_scf.run()
         logger.info(f"FCI embedding energy: {fci_scf.e_tot}")
         return fci_scf
 
     def _mu_embed(
         self, localized_scf: StreamObject, dft_potential: np.ndarray
     ) -> Tuple[StreamObject, np.ndarray]:
@@ -1015,35 +1023,34 @@
             )
             logger.debug(f"Classical energy: {result['classical_energy']}")
 
             # Virtual localization
             if self.run_virtual_localization is True:
                 logger.debug("Performing virtual localization.")
                 self.localized_system.localize_virtual(result["scf"])
+                self.cl_shells = self.localized_system.shells
 
             # Calculate ccsd or fci energy
             if self.run_ccsd_emb is True:
                 logger.debug("Performing CCSD-in-DFT embedding.")
-                ccsd_emb, e_ccsd_corr = self._run_emb_CCSD(
-                    result["scf"], frozen_orb_list=None
-                )
+                ccsd_emb, e_ccsd_corr = self._run_emb_CCSD(result["scf"], frozen=None)
                 result["e_ccsd"] = (
                     ccsd_emb.e_tot
                     + self.e_env
                     + self.two_e_cross
                     - result["correction"]
                     - result["beta_correction"]
                 )
-                result["ccsd_emb"] = ccsd_emb.e_hf - e_ccsd_corr - e_nuc
+                result["ccsd_emb"] = ccsd_emb.e_tot - e_nuc
 
                 logger.info(f"CCSD Energy {name}:\t{result['e_ccsd']}")
 
             if self.run_fci_emb is True:
                 logger.debug("Performing FCI-in-DFT embedding.")
-                fci_emb = self._run_emb_FCI(result["scf"], frozen_orb_list=None)
+                fci_emb = self._run_emb_FCI(result["scf"], frozen=None)
                 result["e_fci"] = (
                     (fci_emb.e_tot)
                     + self.e_env
                     + self.two_e_cross
                     - result["correction"]
                     - result["beta_correction"]
                 )
```

### Comparing `nbed-0.0.3/nbed/embed.py` & `nbed-0.0.4/nbed/embed.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/ham_builder.py` & `nbed-0.0.4/nbed/ham_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,20 @@
                 active_indices,
                 active_indices,
                 active_indices,
                 active_indices,
             )
         ]
 
-        self.occupancy = self.scf_method.mo_occ[..., active_indices]
+        if self.scf_method.mo_occ.ndim == 1:
+            self.occupancy = self.scf_method.mo_occ[active_indices]
+        else:
+            self.occupancy = np.vstack(
+                (self.scf_method.mo_occ[0], self.scf_method.mo_occ[1])
+            )[:, active_indices]
 
         logger.debug("Active space reduced.")
         logger.debug(f"{one_body_integrals_new.shape}")
         logger.debug(f"{two_body_integrals_new.shape}")
         return core_constant, one_body_integrals_new, two_body_integrals_new
 
     def _spinorb_from_spatial(
@@ -504,19 +509,20 @@
                 logger.debug("Unreduced Hamiltonain found.")
                 return qham
 
             logger.debug("Converting to Symmer PauliWordOp")
             pwop = PauliwordOp.from_openfermion(qham)
 
             logger.debug("Creating reference state.")
+            logger.debug(f"{self.occupancy=}")
             electrons = self.occupancy.sum()
-            states = (2 * self.occupancy.shape[-1]) - self.occupancy.sum()
-            logger.debug(f"{electrons=} {states=}")
-            hf_state = np.hstack((np.ones(int(electrons)), np.zeros(int(states))))
-            logger.debug(f"{hf_state.shape=}")
+            virtuals = (2 * self.occupancy.shape[-1]) - self.occupancy.sum()
+            logger.debug(f"{electrons=} {virtuals=}")
+            hf_state = np.hstack((np.ones(int(electrons)), np.zeros(int(virtuals))))
+            logger.debug(f"{hf_state=}")
 
             # We have to do these separately because QubitSubspaceManager requires n_qubits
             if taper is True:
                 logger.debug("Running QubitTapering")
                 pwop = QubitTapering(pwop).taper_it(ref_state=hf_state)
             if contextual_space is True and n_qubits is not None:
                 logger.debug("Creating QubitSubspaceManager.")
```

### Comparing `nbed-0.0.3/nbed/ham_converter.py` & `nbed-0.0.4/nbed/ham_converter.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/localizers/base.py` & `nbed-0.0.4/nbed/localizers/base.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/localizers/pyscf.py` & `nbed-0.0.4/nbed/localizers/pyscf.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/localizers/spade.py` & `nbed-0.0.4/nbed/localizers/spade.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         """Initialize SPADE Localizer object."""
         super().__init__(
             global_scf,
             n_active_atoms,
         )
         self.max_shells = max_shells
         self.shells = None
+        self.singular_values = None
 
     def _localize_spin(
         self, c_matrix: np.ndarray, occupancy: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
         """Localize orbitals of one spin using SPADE.
 
         Args:
@@ -127,14 +128,16 @@
         """
         logger.debug("Localising virtual orbital spin with concentric localization.")
 
         logger.debug("Creating projected molecule object.")
         projected_mol = gto.mole.Mole()
         projected_mol.atom = embedded_scf.mol.atom
         projected_mol.basis = embedded_scf.mol.basis  # can be anything
+        projected_mol.charge = embedded_scf.mol.charge
+        projected_mol.spin = embedded_scf.mol.spin
         projected_mf = scf.RKS(projected_mol)
         n_act_proj_aos = projected_mol.aoslice_by_atom()[self._n_active_atoms - 1][-1]
         logger.debug(f"{n_act_proj_aos=}")
 
         projected_overlap = projected_mf.get_ovlp(embedded_scf.mol)[
             :n_act_proj_aos, :n_act_proj_aos
         ]
@@ -147,81 +150,86 @@
             effective_virt = embedded_scf.mo_coeff[:, occ == 0]
         else:
             occ = np.array([embedded_scf.mo_occ[0], embedded_scf.mo_occ[1]])
             effective_virt = np.array(
                 [embedded_scf.mo_coeff[i][:, occ[i] == 0] for i in [0, 1]]
             )
 
-        logger.debug(f"N effective viruals: {effective_virt.shape}")
+        logger.debug(f"N effective virtuals: {effective_virt.shape}")
 
         left = np.linalg.inv(projected_overlap) @ overlap_two_basis @ effective_virt
         _, sigma, right_vectors = np.linalg.svd(
             np.swapaxes(left, -1, -2) @ overlap_two_basis @ effective_virt
         )
         logger.debug(f"Singular values: {sigma}")
 
+        # record singular values for analysis
+        singular_values = []
+        singular_values.append(sigma)
+
         if self._restricted:
             c_total = embedded_scf.mo_coeff[:, occ > 0]
         else:
             sigma = np.min(sigma, axis=0)
             c_total = np.array(
                 [
                     embedded_scf.mo_coeff[0][:, occ[0] > 0],
                     embedded_scf.mo_coeff[1][:, occ[1] > 0],
                 ]
             )
+        logger.debug(f"Initial {c_total.shape=} (nocc)")
 
         shell_size = np.sum(sigma[:n_act_proj_aos] >= 1e-15)
         logger.debug(f"{shell_size=}")
 
         right_vectors = np.swapaxes(right_vectors, -1, -2)
         v_span, v_ker = np.split(
             right_vectors, [shell_size], axis=-1
         )  # 0 but instability
 
         logger.debug(f"{v_span.shape=}")
         logger.debug(f"{v_ker.shape=}")
 
         c_ispan = effective_virt @ v_span
-        # We'll transform this in the loop
-        c_iker = effective_virt
+        c_iker = effective_virt @ v_ker
 
         c_total = np.concatenate((c_total, c_ispan), axis=-1)
 
         # keep track of the number of orbitals in each shell
-        shells = []
-        shells.append(c_total.shape[-1])
+        self.shells = []
+        self.shells.append(c_total.shape[-1])
         logger.debug("Created 0th shell.")
 
+        if v_ker.shape[-1] == 0:
+            logger.debug("No kernel for 0th shell, cannot perform CL.")
+            logger.debug(
+                "This is expected for molecules with majority active MOs occupied."
+            )
+            return
+        elif v_ker.shape[-1] == 1:
+            logger.debug(
+                "Kernel is 1 for 0th shell, ending CL as cannot perform SVD of vector."
+            )
+            c_total = np.concatenate((c_total, c_iker), axis=-1)
+            self.shells.append(c_total.shape[-1])
+            return
+
         fock_operator = embedded_scf.get_fock()
         # why use the overlap for the first shell and then the fock for the rest?
 
         for ishell in range(1, self.max_shells + 1):
             logger.debug("Beginning Concentric Localization Iteration")
             logger.debug(f"Shell {ishell}.")
 
-            logger.debug(f"{v_ker.shape[-1]=}")
-            if v_ker.shape[-1] > 1:
-                logger.debug("Kernel dimension is greater than 1, continuing CL.")
-                c_iker = c_iker @ v_ker
-            elif v_ker.shape[-1] == 1:
-                logger.debug("Kernel is 1, ending CL as cannot perform SVD of vector.")
-                c_total = np.concatenate((c_total, c_iker @ v_span), axis=-1)
-                shells.append(c_total.shape[-1])
-                break
-            else:
-                # This means that all virtual orbitals have been included.
-                logger.debug("No kernel, ending CL.")
-                break
-
-            logger.debug(f"{c_ispan.shape=}, {fock_operator.shape=}, {c_iker.shape=}")
-            _, sigma, right_vectors = linalg.svd(
-                np.swapaxes(c_ispan, -1, -2) @ fock_operator @ c_iker
+            logger.debug(f"{c_total.shape=}, {fock_operator.shape=}, {c_iker.shape=}")
+            _, sigma, right_vectors = np.linalg.svd(
+                np.swapaxes(c_total, -1, -2) @ fock_operator @ c_iker
             )
             logger.debug(f"Singular values: {sigma}")
+            singular_values.append(sigma)
             if not self._restricted:
                 sigma = np.min(sigma, axis=0)
             logger.debug(f"{right_vectors.shape=}")
 
             shell_size = np.sum(sigma[:n_act_proj_aos] >= 1e-15)
             logger.debug(f"{shell_size=}")
             if shell_size == 0:
@@ -232,17 +240,39 @@
             v_span, v_ker = np.split(
                 right_vectors, [shell_size], axis=-1
             )  # 0 but instability
 
             logger.debug(f"{v_span.shape=}")
             logger.debug(f"{v_ker.shape=}")
 
-            c_total = np.concatenate((c_total, c_iker @ v_span), axis=-1)
-            logger.debug("Adding shell to total C matrix.")
-            shells.append(c_total.shape[-1])
-            logger.debug(f"{c_total.shape=}")
+            # span must be done first as both need to use old c_iker
+            c_ispan = c_iker @ v_span
+            c_total = np.concatenate((c_total, c_ispan), axis=-1)
+            self.shells.append(c_total.shape[-1])
 
-        self.shells = shells
-        logger.debug(f"Shell indices: {shells}")
+            if v_ker.shape[-1] >= 1:
+                logger.debug("Kernel dimension is greater than 1, continuing CL.")
+                # in-place update
+                c_iker = c_iker @ v_ker
 
-        embedded_scf.mo_coeff = c_total
+                if v_ker.shape[-1] == 1:
+                    logger.debug(
+                        "Kernel is 1, ending CL as cannot perform SVD of vector."
+                    )
+                    c_total = np.concatenate((c_total, c_iker), axis=-1)
+                    self.shells.append(c_total.shape[-1])
+                    break
+            else:
+                # This means that all virtual orbitals have been included.
+                logger.debug("No kernel, ending CL.")
+                break
+
+        logger.debug(f"Shell indices: {self.shells}")
+
+        self.singular_values = singular_values
+
+        if self._restricted:
+            embedded_scf.mo_coeff = c_total  # <- is there any issue with using half of the cmatrix in localized form?
+        else:
+            embedded_scf.mo_coeff[0] = c_total[0]
+            embedded_scf.mo_coeff[1] = c_total[1]
         logger.debug("Completed Concentric Localization.")
```

### Comparing `nbed-0.0.3/nbed/mol_plot.py` & `nbed-0.0.4/nbed/mol_plot.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/scf/embedded_hcore_funcs.py` & `nbed-0.0.4/nbed/scf/embedded_hcore_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pyscf import ao2mo
 
 
 def energy_elec(mf, dm=None, h1e=None, vhf=None) -> Tuple[float, float]:
     """Electronic energy of Unrestricted Hartree-Fock.
 
     Note this function has side effects which cause mf.scf_summary updated.
-    This version is
 
     Args:
         mf (pyscf.scf.hf.HF): Hartree-Fock object
         dm (np.ndarray): Density matrix
         h1e (np.ndarray): Core Hamiltonian
         vhf (np.ndarray): 2-electron contribution to effective potential
```

### Comparing `nbed-0.0.3/nbed/scf/huzinaga_hf.py` & `nbed-0.0.4/nbed/scf/huzinaga_hf.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/scf/huzinaga_ks.py` & `nbed-0.0.4/nbed/scf/huzinaga_ks.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/nbed/utils.py` & `nbed-0.0.4/nbed/utils.py`

 * *Files identical despite different names*

### Comparing `nbed-0.0.3/pyproject.toml` & `nbed-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "nbed"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
-authors = ["Michael Williams <michael.williams.20@ucl.ac.uk>"]
+authors = ["Michael Williams de la Bastida <michael.williams.20@ucl.ac.uk>", "Alexis Ralli <alexis.ralli.18@ucl.ac.uk>"]
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
@@ -35,25 +35,28 @@
 pandoc = "^2.3"
 poetry = "^1.7.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-nbsphinx = "^0.8.8"
+nbsphinx = "^0.9.0"
 Sphinx = "^5"
 sphinx-rtd-theme = "^1.0.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 
+
+
+
 [tool.poetry.scripts]
 nbed = "nbed.embed:cli"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `nbed-0.0.3/PKG-INFO` & `nbed-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nbed
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
-Author: Michael Williams
+Author: Michael Williams de la Bastida
 Author-email: michael.williams.20@ucl.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PennyLane (>=0.33.0,<0.34.0)
```

