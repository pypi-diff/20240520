# Comparing `tmp/cryojax-0.3.0rc1.tar.gz` & `tmp/cryojax-0.3.0rc2.tar.gz`

## Comparing `cryojax-0.3.0rc1.tar` & `cryojax-0.3.0rc2.tar`

### file list

```diff
@@ -1,130 +1,134 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.gitattributes
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/mkdocs.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.github/workflows/testing.yml
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/index.md
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/_static/custom_css.css
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/_static/mathjax.js
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/api/simulator/scattering_potential.md
--rw-r--r--   0        0        0  1156032 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/cross-correlation-search.ipynb
--rw-r--r--   0        0        0   511326 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/read-dataset.ipynb
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/simulate-helix.ipynb
--rw-r--r--   0        0        0   269240 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/simulate-image.ipynb
--rw-r--r--   0        0        0   137942 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/simulate-micrograph.ipynb
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/test-multiatom.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/data/.gitkeep
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/data/ribosome_4ug0_micrograph.mrc
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/data/ribosome_4ug0_micrograph.mrcs
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/data/ribosome_4ug0_particles.star
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/__init__.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/_errors.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/_filter_specs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/_filtered_transformations.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/cryojax_version.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/constants/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/constants/_load_atoms.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/constants/_unit_conversions.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/constants/element_params.npy
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/coordinates/__init__.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/coordinates/_coordinate_functions.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/coordinates/_coordinate_wrappers.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_dataset.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_particle_stack.py
--rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_relion.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/__init__.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/cif.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/gemmi.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/mdtraj.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/mrc.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/pdb.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/data/_io/starfile.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_average.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_edges.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_fft.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_map_coordinates.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_normalize.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_rescale_pixel_size.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/_spectrum.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/__init__.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/_filters.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/_fourier_operator.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/_masks.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/_operator.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/image/operators/_real_operator.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/__init__.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/custom_types.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/pytree_manipulation.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/search_loop.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/search_method.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_transforms/__init__.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_transforms/lie_group_transforms.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/_transforms/transforms.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/distributions/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/distributions/_base_distribution.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/inference/distributions/_gaussian_distributions.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/rotations/__init__.py
--rw-r--r--   0        0        0    16051 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/rotations/_lie_group.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/rotations/_rotation.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/rotations/_utils.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/__init__.py
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_detector.py
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_imaging_pipeline.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_instrument_config.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_pose.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_solvent.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_assembly/__init__.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_assembly/assembly.py
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_assembly/helix.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/base_potential_integrator.py
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/fourier_voxel_extract.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/nufft_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/__init__.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/atom_potential.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/base_potential.py
--rw-r--r--   0        0        0    23744 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/voxel_potential.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_scattering_theory/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_scattering_theory/base_scattering_theory.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_scattering_theory/linear_scattering_theory.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/base_conformation.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/base_ensemble.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/discrete_ensemble.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/ensemble_batcher.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/__init__.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/base_transfer_theory.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/common_functions.py
--rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/conftest.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_agree_with_cistem.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_atom_routines.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_detector.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_ensemble.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_fft.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_grid_search.py
--rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_helix.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_normalize.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_pose_agreement.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_potential.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_shape.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/test_voxels_from_atoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/data/.gitkeep
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/data/1uao.pdb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/data/3j9g_potential_ps4_4.mrc
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/tests/data/3j9g_subunit_potential_ps4_4.mrc
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/LICENSE
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/README.md
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0    39366 2020-02-02 00:00:00.000000 cryojax-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.gitattributes
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/mkdocs.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/index.md
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/_static/custom_css.css
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/_static/mathjax.js
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/api/simulator/scattering_potential.md
+-rw-r--r--   0        0        0   116102 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/compute-potential.ipynb
+-rw-r--r--   0        0        0  1156055 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/cross-correlation-search.ipynb
+-rw-r--r--   0        0        0   511312 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/read-dataset.ipynb
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/simulate-helix.ipynb
+-rw-r--r--   0        0        0   258172 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/simulate-image.ipynb
+-rw-r--r--   0        0        0   122431 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/simulate-micrograph.ipynb
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/test-multiatom.ipynb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/5w0s.pdb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/groel_5w0s_scattering_potential.mrc
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/ribosome_4ug0_micrograph.mrc
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/ribosome_4ug0_micrograph.mrcs
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/ribosome_4ug0_particles.star
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/_errors.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/_filter_specs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/_filtered_transformations.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/_loop.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/cryojax_version.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/constants/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/constants/_scattering_factor_parameters.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/constants/_unit_conversions.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/constants/peng1996_element_params.npy
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/coordinates/__init__.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/coordinates/_geometry.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/coordinates/_make_coordinate_grids.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/data/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/data/_dataset.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/data/_particle_stack.py
+-rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/data/_relion.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_average.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_downsample.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_edges.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_fft.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_map_coordinates.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_normalize.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_rescale_pixel_size.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/_spectrum.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/__init__.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/_filters.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/_fourier_operator.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/_masks.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/_operator.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/image/operators/_real_operator.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/__init__.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/custom_types.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/pytree_manipulation.py
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/search_loop.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/search_method.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_transforms/__init__.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_transforms/lie_group_transforms.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/_transforms/transforms.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/distributions/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/distributions/_base_distribution.py
+-rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/inference/distributions/_gaussian_distributions.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/__init__.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/_gemmi.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/_mdtraj.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/_mrc.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/_pdb_and_cif.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/io/_starfile.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/rotations/__init__.py
+-rw-r--r--   0        0        0    16051 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/rotations/_lie_group.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/rotations/_rotation.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/rotations/_utils.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/__init__.py
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_detector.py
+-rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_imaging_pipeline.py
+-rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_instrument_config.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_pose.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_solvent.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_assembly/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_assembly/assembly.py
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_assembly/helix.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/base_potential_integrator.py
+-rw-r--r--   0        0        0     8260 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/fourier_voxel_extract.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/nufft_project.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/__init__.py
+-rw-r--r--   0        0        0    17903 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/atom_potential.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/base_potential.py
+-rw-r--r--   0        0        0    16928 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/voxel_potential.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/base_scattering_theory.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/common_functions.py
+-rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/weak_phase_scattering_theory.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/base_conformation.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/base_ensemble.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/discrete_ensemble.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/ensemble_batcher.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/__init__.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/base_transfer_theory.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/common_functions.py
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_agree_with_cistem.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_atom_routines.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_detector.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_ensemble.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_fft.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_grid_search.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_helix.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_normalize.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_pose_agreement.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_potential.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_shape.py
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/test_voxels_from_atoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/data/.gitkeep
+-rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/data/1uao.pdb
+-rw-r--r--   0        0        0  1049600 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/data/3j9g_potential_ps4_4.mrc
+-rw-r--r--   0        0        0  1049600 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/tests/data/3j9g_subunit_potential_ps4_4.mrc
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/LICENSE
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    39358 2020-02-02 00:00:00.000000 cryojax-0.3.0rc2/PKG-INFO
```

### Comparing `cryojax-0.3.0rc1/.pre-commit-config.yaml` & `cryojax-0.3.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/CONTRIBUTING.md` & `cryojax-0.3.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/mkdocs.yml` & `cryojax-0.3.0rc2/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
               members_order: source
               heading_level: 4
 
 nav:
     - 'index.md'
     - Examples:
         - Introductory:
+            - Compute a scattering potential: 'examples/compute-potential.ipynb'
             - Simulate an image: 'examples/simulate-image.ipynb'
             - Read a particle stack: 'examples/read-dataset.ipynb'
         - Intermediate:
             - Simulate a batch of images: 'examples/simulate-micrograph.ipynb'
             - Run a cross-correlation search: 'examples/cross-correlation-search.ipynb'
     - Simulator API:
         - 'api/simulator/scattering_potential.md'
```

### Comparing `cryojax-0.3.0rc1/.github/workflows/build_docs.yml` & `cryojax-0.3.0rc2/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/.github/workflows/release.yml` & `cryojax-0.3.0rc2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/.github/workflows/testing.yml` & `cryojax-0.3.0rc2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/docs/index.md` & `cryojax-0.3.0rc2/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
 import cryojax.simulator as cxs
-from cryojax.data import read_array_with_spacing_from_mrc
+from cryojax.io import read_array_with_spacing_from_mrc
 
 # Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
 potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
 # ... now, instantiate the pose. Angles are given in degrees
 pose = cxs.EulerAnglePose(
@@ -62,17 +62,17 @@
     view_theta=80.0,
     view_psi=-10.0,
 )
 # ... now, build the ensemble. In this case, the ensemble is just a single structure
 structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+Here, the 3D scattering potential array is read from `filename` (see the documentation [here](https://mjo22.github.io/cryojax/examples/compute-potential/) for an example of how to generate the potential). Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and subsequently the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
 
-Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `WeakPhaseScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
 # Initialize the scattering theory. First, instantiate fourier slice extraction
 potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
 # ... next, the contrast transfer theory
@@ -80,15 +80,15 @@
     defocus_in_angstroms=9800.0,
     astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
     amplitude_contrast_ratio=0.1
 )
 transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
 # ... now for the scattering theory
-scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
+scattering_theory = cxs.WeakPhaseScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
 The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
 # Finally, build the image formation model
```

### Comparing `cryojax-0.3.0rc1/docs/_static/custom_css.css` & `cryojax-0.3.0rc2/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/docs/api/simulator/scattering_potential.md` & `cryojax-0.3.0rc2/docs/api/simulator/scattering_potential.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,92 +4,104 @@
 
 ???+ abstract "`cryojax.simulator.AbstractPotentialRepresentation`"
     ::: cryojax.simulator.AbstractPotentialRepresentation
         options:
             members:
                 - rotate_to_pose
 
+## Atom-based scattering potentials
+
+???+ abstract "`cryojax.simulator.AbstractAtomicPotential`"
+
+    ::: cryojax.simulator.AbstractAtomicPotential
+        options:
+            members:
+                - atom_positions
+                - as_real_voxel_grid
+
+::: cryojax.simulator.GaussianMixtureAtomicPotential
+        options:
+            members:
+                - __init__
+                - rotate_to_pose
+                - as_real_voxel_grid
+
+
+??? abstract "`cryojax.simulator.AbstractTabulatedAtomicPotential`"
+
+    ::: cryojax.simulator.AbstractTabulatedAtomicPotential
+        options:
+            members:
+                - b_factors
+
+
+::: cryojax.simulator.PengAtomicPotential
+        options:
+            members:
+                - __init__
+                - rotate_to_pose
+                - as_real_voxel_grid
+
+
 ## Voxel-based scattering potentials
 
-???+ abstract "`cryojax.simulator.AbstractVoxelPotential`"
+??? abstract "`cryojax.simulator.AbstractVoxelPotential`"
 
     ::: cryojax.simulator.AbstractVoxelPotential
         options:
             members:
                 - voxel_size
                 - is_real
                 - shape
-                - rotate_to_pose
                 - from_real_voxel_grid
-                - from_atoms
 
 ### Fourier-space voxel representations
 
-??? abstract "`cryojax.simulator.AbstractFourierVoxelGridPotential`"
-
-    ::: cryojax.simulator.AbstractFourierVoxelGridPotential
-        options:
-            members:
-                - __init__
-
 !!! info "Fourier-space conventions"
-    - The `fourier_voxel_grid` and `wrapped_frequency_slice` arguments to
-    `FourierVoxelGrid.__init__` should be loaded with the zero frequency
+    - The `fourier_voxel_grid` and `frequency_slice` arguments to
+    `FourierVoxelGridPotential.__init__` should be loaded with the zero frequency
     component in the center of the box.
     - The parameters in an `AbstractPose` represent a rotation in real-space. This means that when calling `FourierVoxelGridPotential.rotate_to_pose`,
     frequencies are rotated by the inverse rotation as stored in the pose.
 
 ::: cryojax.simulator.FourierVoxelGridPotential
         options:
             members:
                 - __init__
-                - wrapped_frequency_slice_in_angstroms
                 - from_real_voxel_grid
-                - from_atoms
+                - rotate_to_pose
+                - frequency_slice_in_angstroms
+                - shape
 
 ---
 
 ::: cryojax.simulator.FourierVoxelGridPotentialInterpolator
         options:
             members:
                 - __init__
-                - wrapped_frequency_slice_in_angstroms
                 - from_real_voxel_grid
-                - from_atoms
+                - rotate_to_pose
+                - frequency_slice_in_angstroms
+                - shape
+
 
 ### Real-space voxel representations
 
 ::: cryojax.simulator.RealVoxelGridPotential
         options:
             members:
                 - __init__
-                - wrapped_coordinate_grid_in_angstroms
                 - from_real_voxel_grid
-                - from_atoms
+                - rotate_to_pose
+                - coordinate_grid_in_angstroms
+                - shape
 
 ---
 
 ::: cryojax.simulator.RealVoxelCloudPotential
         options:
             members:
                 - __init__
-                - wrapped_coordinate_list_in_angstroms
                 - from_real_voxel_grid
-                - from_atoms
-
-### Pure function API
-
-::: cryojax.simulator.build_real_space_voxels_from_atoms
-        options:
-            heading_level: 5
-
----
-
-::: cryojax.simulator.evaluate_3d_atom_potential
-        options:
-            heading_level: 5
-
----
-
-::: cryojax.simulator.evaluate_3d_real_space_gaussian
-        options:
-            heading_level: 5
+                - rotate_to_pose
+                - coordinate_list_in_angstroms
+                - shape
```

### Comparing `cryojax-0.3.0rc1/docs/examples/cross-correlation-search.ipynb` & `cryojax-0.3.0rc2/docs/examples/cross-correlation-search.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992407796451914%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(5, \'\\n\')]}}, 3: {\'source\': {insert: [(3, "    The '*

 * *            'cisTEM scattering potential has been modified slightly because at the time of writing '*

 * *            "this, `cryojax` scattering potentials have different conventions than `cisTEM`'s. In "*

 * *            'particular, the `cisTEM` scattering potential was multiplied by a factor of $4 \\\\pi '*

 * *            '/(\\\\textrm{voxel size} \\\\times \\\\textrm{wavelength})$.")], delete: [3]}}, 4: '*

 * *            "{ […]*

```diff
@@ -5,14 +5,15 @@
             "metadata": {},
             "source": [
                 "This is a tutorial that demonstrates a cross-correlation-based grid search for the underlying pose of a known structure. The idea of the search follows `cisTEM`'s 2D template matching program.\n",
                 "\n",
                 "This is also a tutorial for using `cryojax`'s grid search API. In `cryojax.inference`, the function `run_grid_search` provides a flexible API for minimizing a loss function with grid search, while the abstract interface `AbstractGridSearchMethod` provides a way to extend the API. See the documentation for more information.\n",
                 "\n",
                 "*Reference*:\n",
+                "\n",
                 "- Lucas, Bronwyn A., et al. \"Locating macromolecular assemblies in cells by 2D template matching with cisTEM.\" Elife 10 (2021): e68946.*"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
@@ -47,24 +48,24 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "First, load the template. This template happens to be generated from cisTEM.\n",
                 "\n",
                 "!!! note \n",
-                "    The cisTEM scattering potential has been modified slightly because at the time of writing this, `cryojax` scattering potentials have different conventions than `cisTEM`'s. In particular, the `cisTEM` scattering potential was multiplied by a factor of $1/(\\textrm{voxel size} \\times \\textrm{wavelength})$."
+                "    The cisTEM scattering potential has been modified slightly because at the time of writing this, `cryojax` scattering potentials have different conventions than `cisTEM`'s. In particular, the `cisTEM` scattering potential was multiplied by a factor of $4 \\pi /(\\textrm{voxel size} \\times \\textrm{wavelength})$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from cryojax.data import read_array_with_spacing_from_mrc\n",
+                "from cryojax.io import read_array_with_spacing_from_mrc\n",
                 "\n",
                 "\n",
                 "# First, load the template. This template happens to be generated from cisTEM\n",
                 "filename = \"./data/ribosome_4ug0_scattering_potential_from_cistem.mrc\"\n",
                 "template, voxel_size = read_array_with_spacing_from_mrc(filename)\n",
                 "potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(\n",
                 "    template, voxel_size, pad_scale=1.5\n",
@@ -186,17 +187,17 @@
             "source": [
                 "# ... create the structural ensemble\n",
                 "structural_ensemble = cxs.SingleStructureEnsemble(\n",
                 "    conformational_space=potential, pose=pose_grid\n",
                 ")\n",
                 "# ... now the scattering theory\n",
                 "transfer_theory = cxs.ContrastTransferTheory(particle_stack.ctf)\n",
-                "projection_method = cxs.FourierSliceExtraction(interpolation_order=1)\n",
-                "scattering_theory = cxs.LinearScatteringTheory(\n",
-                "    structural_ensemble, projection_method, transfer_theory\n",
+                "potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)\n",
+                "scattering_theory = cxs.WeakPhaseScatteringTheory(\n",
+                "    structural_ensemble, potential_integrator, transfer_theory\n",
                 ")\n",
                 "# ... and finally the imaging pipeline.\n",
                 "imaging_pipeline = cxs.ContrastImagingPipeline(\n",
                 "    particle_stack.instrument_config, scattering_theory\n",
                 ")"
             ]
         },
```

### Comparing `cryojax-0.3.0rc1/docs/examples/read-dataset.ipynb` & `cryojax-0.3.0rc2/docs/examples/read-dataset.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999561403508772%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(10, '    "*

 * *            "relion_particle.instrument_config.frequency_grid_in_angstroms\\n')], delete: [10]}}}"}*

```diff
@@ -289,15 +289,15 @@
                 "# Get the particle\n",
                 "relion_particle = dataset[0]\n",
                 "# ... and the image in fourier space\n",
                 "fourier_image = rfftn(relion_particle.image_stack)\n",
                 "# ... and the cartesian coordinate system\n",
                 "pixel_size = relion_particle.instrument_config.pixel_size\n",
                 "frequency_grid_in_angstroms = (\n",
-                "    relion_particle.instrument_config.wrapped_frequency_grid_in_angstroms.get()\n",
+                "    relion_particle.instrument_config.frequency_grid_in_angstroms\n",
                 ")\n",
                 "# ... now, compute a radial coordinate system\n",
                 "radial_frequency_grid_in_angstroms = jnp.linalg.norm(frequency_grid_in_angstroms, axis=-1)\n",
                 "# ... plot the image in fourier space and the radial frequency grid\n",
                 "fig, axes = plt.subplots(figsize=(5, 4), ncols=2)\n",
                 "plot_image(\n",
                 "    jnp.log(jnp.abs(jnp.fft.fftshift(fourier_image, axes=(0,))) ** 2),\n",
```

### Comparing `cryojax-0.3.0rc1/docs/examples/simulate-helix.ipynb` & `cryojax-0.3.0rc2/docs/examples/simulate-helix.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/docs/examples/simulate-micrograph.ipynb` & `cryojax-0.3.0rc2/docs/examples/simulate-micrograph.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989550051791549%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(6, '    from cryojax.io import "*

 * *            "read_array_with_spacing_from_mrc\\n')], delete: [6]}}, 5: {'source': {insert: [(1, "*

 * *            '\'filename = "./data/groel_5w0s_scattering_potential.mrc"\\n\')], delete: [1]}}, 7: '*

 * *            "{'source': {insert: [(29, '    theory = cxs.WeakPhaseScatteringTheory(\\n')], delete: "*

 * *            "[29]}}, 8: {'source': {insert: [(3, '    says that we do not want to broadcast that "*

 * *            'leaf (of course, this only wor […]*

```diff
@@ -50,15 +50,15 @@
             "source": [
                 "# CryoJAX imports\n",
                 "from jaxtyping import install_import_hook\n",
                 "\n",
                 "\n",
                 "with install_import_hook(\"cryojax\", \"typeguard.typechecked\"):\n",
                 "    import cryojax.simulator as cxs\n",
-                "    from cryojax.data import read_array_with_spacing_from_mrc\n",
+                "    from cryojax.io import read_array_with_spacing_from_mrc\n",
                 "    from cryojax.rotations import SO3"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -68,15 +68,15 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# First, load the scattering potential and projection method\n",
-                "filename = \"./data/ribosome_4ug0_scattering_potential_from_cistem.mrc\"\n",
+                "filename = \"./data/groel_5w0s_scattering_potential.mrc\"\n",
                 "real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)\n",
                 "potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(\n",
                 "    real_voxel_grid, voxel_size, pad_scale=2\n",
                 ")\n",
                 "# ... now the projection method\n",
                 "potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)\n",
                 "# ... and the contrast transfer theory\n",
@@ -134,30 +134,28 @@
                 "    # zero\n",
                 "    offset_in_angstroms = jnp.pad(in_plane_offset_in_angstroms, ((0, 1),))\n",
                 "    # ... build the pose\n",
                 "    pose = cxs.QuaternionPose.from_rotation_and_translation(rotation, offset_in_angstroms)\n",
                 "    # ... build the ensemble\n",
                 "    structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)\n",
                 "    # ... and finally the scattering theory and return\n",
-                "    theory = cxs.LinearScatteringTheory(\n",
+                "    theory = cxs.WeakPhaseScatteringTheory(\n",
                 "        structural_ensemble, potential_integrator, transfer_theory\n",
                 "    )\n",
                 "    return cxs.ContrastImagingPipeline(config, theory)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "!!! info \"What's with the `out_axes=eqxi.if_mapped(axis=0)`?\"\n",
                 "    \n",
                 "    When we create a pytree with `eqx.filter_vmap` (or `jax.vmap`), `out_axes` should have the same structure as the output pytree. If `out_axes` is set to `None` at a particular leaf, this\n",
-                "    says that we do not want to broadcast that leaf (of course, this only works for unmapped leaves). By default `jax.vmap` sets `out_axes=0`, so all unmapped leaves get broadcasted. `equinox` allows us to pass `out_axes=eqxi.if_mapped(axes=0)`, which specifies *not* to broadcast pytree leaves unless the leaves are directly mapped.\n",
-                "\n",
-                "    When building a `ContrastImagingPipeline`, it is very important that we do not broadcast arbitrary leaves! For example, an `InstrumentConfig` stores the coordinate systems for our image. Without the `out_axes=eqxi.if_mapped(axes=0)` specification, the `make_imaging_pipeline` would output an `ContrastImagingPipeline.instrument_config` whose coordinate systems have a batch dimension. This takes up unecessary memory."
+                "    says that we do not want to broadcast that leaf (of course, this only works for unmapped leaves). By default `jax.vmap` sets `out_axes=0`, so all unmapped leaves get broadcasted. `equinox` allows us to pass `out_axes=eqxi.if_mapped(axes=0)`, which specifies *not* to broadcast pytree leaves unless the leaves are directly mapped."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
@@ -242,15 +240,15 @@
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAhYAAAFNCAYAAABc5iZ6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/H5lhTAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOy9eZRcZbU2/tSpeZ7HHpNOZ4JA/AJCnHBAoyLKcgL8PhmuwpULKqL+FMTLpOLSq6CCotfxqiz9cMD7KTIKeO8FBZEAEhIy9NxdXfM81zm/P3rtzamTU9XV6U7SCfWsldWpU6fO8J73vO9+9372szWSJEnooYceeuihhx56WAEIR/sCeuihhx566KGH4wc9w6KHHnrooYceelgx9AyLHnrooYceeuhhxdAzLHrooYceeuihhxVDz7DooYceeuihhx5WDD3Dooceeuihhx56WDH0DIseeuihhx566GHF0DMseuihhx566KGHFUPPsOihhx566KGHHlYMPcOihx66wJNPPolXvepVsFqt0Gg02Llz59G+pJcFCoUCPvzhDyMUCkGj0eDKK6882pfUEddffz00Gs3Rvoweejiq6BkWbfDjH/8YGo0Gf/vb3472pRx3eOyxx3D99dcjk8kclfPPzs7i+uuv79o4qNfreN/73odUKoVbbrkFP/3pTzE0NHR4L7IHAMCXvvQl/PjHP8Zll12Gn/70p/jgBz94tC+phx56WAS6o30BPbz88Nhjj+GGG27ARRddBJfLdcTPPzs7ixtuuAHDw8PYunXrovvv378fExMT+Pd//3d8+MMfPvwX2APjT3/6E04//XRcd911R/tSeuihhy7R81j0sKohiiIqlcpRvYZYLAYAK2oEFYvFFTvW8YxYLHbI7b4a+k4PPbwc0TMsloCLLroINpsNk5OTeMc73gGbzYa+vj7cfvvtAIDnnnsOb3zjG2G1WjE0NIQ777yz5fepVAqf+tSnsGXLFthsNjgcDrztbW/DM888c9C5JiYm8M53vhNWqxWBQACf+MQncN9990Gj0eCRRx5p2fevf/0r3vrWt8LpdMJiseCMM87A//zP/3R1T5VKBddffz3Wr18Pk8mEcDiMd7/73di/fz/vUywW8clPfhIDAwMwGo3YsGED/u3f/g3KwrgajQZXXHEF7r77bpx44okwGo044YQTcO+99/I+119/PT796U8DANasWQONRgONRoPx8fGWY/z85z/HCSecAKPRyL//t3/7N7zqVa+C1+uF2WzGtm3b8Ktf/eqge3rggQfwmte8Bi6XCzabDRs2bMA111wDAHjkkUdw6qmnAgAuvvhiPv+Pf/xj1fa56KKLcMYZZwAA3ve+90Gj0eD1r389f/+nP/0Jr33ta2G1WuFyufCud70LL7zwQssxKO6+a9cufOADH4Db7cZrXvOats9kKf1EDZ3uH3gpzEdtTnjkkUcO6l+vf/3rceKJJ+LZZ5/FGWecAYvFgnXr1nG7P/roozjttNNgNpuxYcMGPPjgg11dYywWw4c+9CEEg0GYTCacfPLJ+MlPfnLQtYyNjeEPf/jDQf1EDSvRd7rpw4T//u//xqmnngqTyYSRkRF897vfVb2uRqOBm266CSMjIzAajRgeHsY111yDarXast/w8DDe8Y534JFHHsEpp5wCs9mMLVu28PP4zW9+gy1btsBkMmHbtm14+umnF2tmftZ//vOf8c///M/wer1wOBy44IILkE6nD9r/29/+NrddJBLB5ZdfflDIcu/evXjPe96DUCgEk8mE/v5+nHfeechmsy37/exnP8O2bdtgNpvh8Xhw3nnnYWpq6pCO1cMxBqkHVfzoRz+SAEhPPvkkb7vwwgslk8kkbd68WfrIRz4i3X777dKrXvUqCYD0ox/9SIpEItKnP/1p6Vvf+pZ0wgknSFqtVjpw4AD//sknn5RGRkakz372s9J3v/td6cYbb5T6+vokp9MpzczM8H6FQkFau3atZDabpc9+9rPSrbfeKr3yla+UTj75ZAmA9PDDD/O+Dz30kGQwGKTt27dLX/va16RbbrlFOumkkySDwSD99a9/7XiPjUZDetOb3iQBkM477zzptttuk26++WbpjW98o3T33XdLkiRJoihKb3zjGyWNRiN9+MMflm677Tbp7LPPlgBIV155ZcvxAEgnn3yyFA6HpZtuukm69dZbpbVr10oWi0VKJBKSJEnSM888I51//vkSAOmWW26RfvrTn0o//elPpUKhwMfYtGmT5Pf7pRtuuEG6/fbbpaefflqSJEnq7++X/uVf/kW67bbbpK9//evSK1/5SgmA9Pvf/56v4R//+IdkMBikU045RfrGN74h3XHHHdKnPvUp6XWve50kSZIUjUalG2+8UQIgXXrppXz+/fv3q7bRY489Jl1zzTUSAOljH/uY9NOf/lS6//77JUmSpAceeEDS6XTS+vXrpa985SvSDTfcIPl8PsntdktjY2N8jOuuu04CIG3evFl617veJX3729+Wbr/99rbPpdt+oobF7l+SXurb8muUJEl6+OGHD+pfZ5xxhhSJRKSBgQHu25s3b5a0Wq30i1/8QgqFQtL1118v3XrrrXyNuVyu4zWWSiVp06ZNkl6vlz7xiU9I3/zmN6XXvva1EgDp1ltvlSRp4Tn99Kc/lXw+n7R169aD+okaltt36BiL9WFJkqRnn31WMpvN0uDgoHTzzTdLN910kxQMBqWTTjpJUg6rF154oQRAeu973yvdfvvt0gUXXCABkM4555yW/YaGhqQNGzZI4XBYuv7666VbbrlF6uvrk2w2m/Szn/1MGhwclL785S9LX/7ylyWn0ymtW7dOajabHduanvWWLVuk1772tdI3v/lN6fLLL5cEQZBe97rXSaIo8r7UT88880zpW9/6lnTFFVdIWq1WOvXUU6VarSZJkiRVq1VpzZo1UiQSkb7whS9I3//+96UbbrhBOvXUU6Xx8XE+1he+8AVJo9FI5557rvTtb3+b343h4WEpnU4v6Vg9HHvoGRZt0M6wACB96Utf4m3pdFoym82SRqORfvGLX/D23bt3SwCk6667jrdVKpWDBoKxsTHJaDRKN954I2/72te+JgHgyV2SJKlcLksbN25sGfhFUZRGR0elHTt2tAwQpVJJWrNmjfTmN7+54z3+8Ic/lABIX//61w/6jo539913SwCkL3zhCy3fv/e975U0Go20b98+3gZAMhgMLdueeeYZCYD0rW99i7d99atfVZ3Y6BiCIEjPP//8Qd+VSqWWz7VaTTrxxBOlN77xjbztlltukQBI8Xi87X0/+eSTbAx2A5pw77rrrpbtW7dulQKBgJRMJnnbM888IwmCIF1wwQW8jQbs888/v6vzddtP1NDN/S/VsAAg3XnnnbyN+rYgCNJf/vIX3n7fffd11a633nqrBED62c9+xttqtZq0fft2yWaztRgmQ0ND0llnndXxeITl9h06Rjd9+JxzzpFMJpM0MTHB23bt2iVptdoWw2Lnzp0SAOnDH/5wy3k+9alPSQCkP/3pTy33CkB67LHHeBu1qdlsbjnXd7/73YOelRroWW/bto2NA0mSpK985SsSAOl3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vxtarRY33HDDQf1YkiQkk8muj9XDsYmex+II4h3veAduvPFGXHzxxXjVq16F5557Dj//+c9bVggA8M///M+47bbbcP755+PjH/84wuEwfv7zn8NkMgF4acUvCAK+//3v421vextOOOEEXHzxxejr68PMzAwefvhhOBwO/L//9//aXs8FF1yA//iP/8BVV12FJ554Aq997WtRLBbx4IMP4l/+5V/wrne9C2effTbe8IY34HOf+xzGx8dx8skn4/7778fvfvc7XHnllS0kt26xbds2AMDnPvc5nHfeedDr9Tj77LM7rvDPOussfP3rX8db3/pWfOADH0AsFsPtt9+OdevW4dlnn+X9brzxRvz5z3/GWWedhaGhIcRiMXz7299Gf38/a0eMjIzA5XLhjjvugN1uh9VqxWmnndY1B4Lw1a9+FW9729uwfft2fOhDH0K5XMa3vvUtOJ1OXH/99UtuF0K3/UQN3dz/CSecgNNPPx1XX301UqkUPB4PfvGLXxw0yB8uXHrppfjud7+Liy66CE899RSGh4fxq1/9Cv/zP/+DW2+99SA+z3LRbd9ZCm644Qbce++9eO1rX4t/+Zd/YcPohBNOaDnmySefjAsvvBDf+973kMlkcMYZZ+CJJ57AT37yE5xzzjktXoTDiVqthje96U14//vfjz179uDb3/42XvOa1zBB3O/34+qrr8YNN9yAt771rXjnO9/J+5166qn4P//n/wBY0G254oor8L73vQ/r169Ho9HAT3/6U2i1WrznPe8BsPB+feELX8DVV1+N8fFxnHPOObDb7RgbG8Nvf/tbXHrppfjUpz7V1bF6OEZxFDJRjgm0Sze1Wq0H7XvGGWdIJ5xwwkHblalylUpF+uQnPymFw2HJbDZLr371q6XHH39cOuOMM6Qzzjij5bcHDhyQzjrrLMlsNkt+v1/65Cc/Kf3617+WALSk+EnSQtrWu9/9bsnr9UpGo1EaGhqS3v/+90sPPfTQovdZKpWkz33uc9KaNWskvV4vhUIh6b3vfW+LrkM+n5c+8YlPSJFIRNLr9dLo6Kj01a9+tSXFVZIWUvUuv/xy1Xa48MILW7bddNNNUl9fnyQIQkvqY7tjSJIk/eAHP5BGR0clo9Eobdy4UfrRj37EqZyEhx56SHrXu94lRSIRyWAwSJFIRDr//POlF198seVYv/vd76TNmzdL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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAhYAAAFNCAYAAABc5iZ6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8g+/7EAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOy9eZhkVZUtvmKe5znnrLkKqkALxFIRFbREWuVJO2C3DO3Q0tC2oP4UtZVBxecAqCBoO7bK03Z+7QAILfhaQGmkZCgoqrIq54iMeZ4jzu+P/PbmRFREZuRQVVlVd31ffpl548Ydzj33nH32XnttlRBCQIECBQoUKFCgYBWgPtYXoECBAgUKFCg4caAYFgoUKFCgQIGCVYNiWChQoECBAgUKVg2KYaFAgQIFChQoWDUohoUCBQoUKFCgYNWgGBYKFChQoECBglWDYlgoUKBAgQIFClYNimGhQIECBQoUKFg1KIaFAgUKFChQoGDVoBgWChT0gEcffRQveclLYLFYoFKpsGfPnmN9SScF8vk83vWudyEYDEKlUuH973//sb6kBXHddddBpVId68tQoOCYQjEsuuA73/kOVCoV/ud//udYX8oJh4ceegjXXXcd0un0MTn/7Owsrrvuup6Ng1qthje/+c1IJpO45ZZb8L3vfQ/Dw8NH9iIVAAA+85nP4Dvf+Q6uuOIKfO9738M73vGOY31JChQoWATaY30BCk4+PPTQQ7j++utx2WWXwel0HvXzz87O4vrrr8fIyAhOP/30RfcfGxvDxMQE/u3f/g3vete7jvwFKmD813/9F1784hfjk5/85LG+FAUKFPQIxWOhYE2j2WyiXC4f02uIRqMAsKpGUKFQWLVjnciIRqPLbve10HcUKDgZoRgWS8Bll10Gq9WKyclJ/M3f/A2sViv6+/tx++23AwCefPJJvOpVr4LFYsHw8DDuuuuulu8nk0l88IMfxPbt22G1WmG323H++efjr3/962HnmpiYwBve8AZYLBb4/X5cffXVuOeee6BSqfDAAw+07PunP/0Jr33ta+FwOGA2m3HOOefgj3/8Y0/3VC6Xcd1112HTpk0wGo0IhUJ405vehLGxMd6nUCjgAx/4AAYHB2EwGLB582Z84QtfQHthXJVKhauuugq/+MUvcOqpp8JgMOCUU07B3Xffzftcd911+NCHPgQAGB0dhUqlgkqlwvj4eMsxfvCDH+CUU06BwWDg73/hC1/AS17yEng8HphMJuzcuRM/+clPDrun3/3ud3jZy14Gp9MJq9WKzZs346Mf/SgA4IEHHsCZZ54JALj88sv5/N/5znc6ts9ll12Gc845BwDw5je/GSqVCq94xSv48//6r//C2WefDYvFAqfTiTe+8Y145plnWo5Bcfe9e/fi7W9/O1wuF172spd1fSZL6SedsND9A8+H+ajNCQ888MBh/esVr3gFTj31VDzxxBM455xzYDabsWHDBm73Bx98EGeddRZMJhM2b96M++67r6drjEajeOc734lAIACj0YjTTjsN3/3udw+7lkOHDuHXv/71Yf2kE1aj7/TShwn//d//jTPPPBNGoxHr16/H1772tY7XVa/XceONN2L9+vUwGAwYGRnBRz/6UVQqlZb9RkZG8Dd/8zd44IEHcMYZZ8BkMmH79u38PH72s59h+/btMBqN2LlzJx5//PHFmpmf9R/+8Af84z/+IzweD+x2Oy655BKkUqnD9v/qV7/KbdfX14crr7zysJDl/v37cdFFFyEYDMJoNGJgYABve9vbkMlkWvb7/ve/j507d8JkMsHtduNtb3sbpqamlnUsBccZhIKO+Pa3vy0AiEcffZS3XXrppcJoNIpt27aJ9773veL2228XL3nJSwQA8e1vf1v09fWJD33oQ+IrX/mKOOWUU4RGoxEHDx7k7z/66KNi/fr14iMf+Yj42te+Jm644QbR398vHA6HmJmZ4f3y+bxYt26dMJlM4iMf+Yi49dZbxYte9CJx2mmnCQDi97//Pe97//33C71eL3bt2iW++MUviltuuUXs2LFD6PV68ac//WnBe6zX6+Lcc88VAMTb3vY2cdttt4mbbrpJvOpVrxK/+MUvhBBCNJtN8apXvUqoVCrxrne9S9x2223i9a9/vQAg3v/+97ccD4A47bTTRCgUEjfeeKO49dZbxbp164TZbBbxeFwIIcRf//pXcfHFFwsA4pZbbhHf+973xPe+9z2Rz+f5GFu3bhU+n09cf/314vbbbxePP/64EEKIgYEB8U//9E/itttuEzfffLN40YteJACIX/3qV3wNTz31lNDr9eKMM84QX/rSl8Sdd94pPvjBD4qXv/zlQgghIpGIuOGGGwQA8Z73vIfPPzY21rGNHnroIfHRj35UABDve9/7xPe+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/uZv/gY33HADLr/8crzkJS/Bk08+iR/84ActKwQA+Md//EfcdtttuPjii/Ev//IvCIVC+MEPfgCj0Qjg+RW/Wq3GN77xDZx//vk45ZRTcPnll6O/vx8zMzP4/e9/D7vdjv/8z//sej2XXHIJ/v3f/x3XXHMN/vznP+Pss89GoVDAfffdh3/6p3/CG9/4Rrz+9a/HK1/5SnzsYx/D+Pg4TjvtNNx777345S9/ife///0tJLdesXPnTgDAxz72MbztbW+DTqfD61//+gVX+BdccAFuvvlmvPa1r8Xb3/52RKNR3H777diwYQOeeOIJ3u+GG27AH/7wB1xwwQUYHh5GNBrFV7/6VQwMDLB2xPr16+F0OnHnnXfCZrPBYrHgrLPO6pkDQfj85z+P888/H7t27cI73/lOlEolfOUrX4HD4cB111235HYh9NpPOqGX+z/llFPw4he/GNdeey2SySTcbjd++MMfHjbIHym85z3vwde+9jVcdtlleOyxxzAyMoKf/OQn+OMf/4hbb731MD7PStFr31kKrr/+etx99904++yz8U//9E9sGJ1yyiktxzzttNNw6aWX4utf/zrS6TTOOecc/PnPf8Z3v/tdXHjhhS1ehCOJarWKc889F295y1uwb98+fPWrX8XLXvYyJoj7fD5ce+21uP766/Ha174Wb3jDG3i/M888E3//938PYF635aqrrsKb3/xmbNq0CfV6Hd/73veg0Whw0UUXAZh/vz71qU/h2muvxfj4OC688ELYbDYcOnQIP//5z/Ge97wHH/zgB3s6loLjFMcgE+W4QLd0U4vFcti+55xzjjjllFMO296eKlcul8UHPvABEQqFhMlkEi996UvFww8/LM455xxxzjnntHz34MGD4oILLhAmk0n4fD7xgQ98QPz0pz8VAFpS/ISYT9t605veJDwejzAYDGJ4eFi85S1vEffff/+i91ksFsXHPvYxMTo6KnQ6nQgGg+Jv//ZvW3QdcrmcuPrqq0VfX5/Q6XRi48aN4vOf/3xLiqsQ86l6V155Zcd2uPTSS1u23XjjjaK/v1+o1eqW1MduxxBCiG9+85ti48aNwmAwiC1btohvf/vbnMpJuP/++8Ub3/hG0dfXJ/R6vejr6xMXX3yxeO6551qO9ctf/lJs27ZNaLXaRVMku6WbCiHEfffdJ1760pcKk8kk7Ha7eP3r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",
                         "text/plain": [
                             "<Figure size 550x550 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
```

### Comparing `cryojax-0.3.0rc1/docs/examples/test-multiatom.ipynb` & `cryojax-0.3.0rc2/docs/examples/test-multiatom.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/docs/examples/data/ribosome_4ug0_particles.star` & `cryojax-0.3.0rc2/docs/examples/data/ribosome_4ug0_particles.star`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/_errors.py` & `cryojax-0.3.0rc2/src/cryojax/_errors.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/_filter_specs.py` & `cryojax-0.3.0rc2/src/cryojax/_filter_specs.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/_filtered_transformations.py` & `cryojax-0.3.0rc2/src/cryojax/_filtered_transformations.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/constants/element_params.npy` & `cryojax-0.3.0rc2/src/cryojax/constants/peng1996_element_params.npy`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/coordinates/_coordinate_functions.py` & `cryojax-0.3.0rc2/src/cryojax/coordinates/_make_coordinate_grids.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,103 @@
 """
-Functions for creating and operating on coordinate systems.
+Functions for creating coordinate systems.
 """
 
 from typing import Optional
 
 import jax.numpy as jnp
 import numpy as np
-from jaxtyping import Array, Float, Inexact
+from jaxtyping import Array, Float
 
 
-def make_coordinates(
-    shape: tuple[int, ...], grid_spacing: float | Float[np.ndarray, ""] = 1.0
+def make_coordinate_grid(
+    shape: tuple[int, ...],
+    grid_spacing: float | Float[np.ndarray, ""] | Float[Array, ""] = 1.0,
 ) -> Float[Array, "*shape ndim"]:
     """
     Create a real-space cartesian coordinate system on a grid.
 
-    Arguments
-    ---------
-    shape :
-        Shape of the voxel grid, with
-        ``ndim = len(shape)``.
-    grid_spacing :
-        The grid spacing, in units of length.
-
-    Returns
-    -------
-    coordinate_grid :
-        Cartesian coordinate system in real space.
+    **Arguments:**
+
+    - `shape`: Shape of the voxel grid, with `ndim = len(shape)`.
+    - `grid_spacing`: The grid spacing, in units of length.
+
+    **Returns:**
+
+    A cartesian coordinate system in real space.
     """
     coordinate_grid = _make_coordinates_or_frequencies(
         shape, grid_spacing=grid_spacing, real_space=True
     )
     return coordinate_grid
 
 
-def make_frequencies(
+def make_frequency_grid(
     shape: tuple[int, ...],
-    grid_spacing: float | Float[np.ndarray, ""] = 1.0,
+    grid_spacing: float | Float[np.ndarray, ""] | Float[Array, ""] = 1.0,
     half_space: bool = True,
 ) -> Float[Array, "*shape ndim"]:
-    """
-    Create a fourier-space cartesian coordinate system on a grid.
+    """Create a fourier-space cartesian coordinate system on a grid.
     The zero-frequency component is in the beginning.
 
     Arguments
     ---------
-    shape :
-        Shape of the voxel grid, with
-        ``ndim = len(shape)``.
-    grid_spacing :
-        The grid spacing, in units of length.
-    half_space :
+    - `shape`: Shape of the voxel grid, with `ndim = len(shape)`.
+    - `grid_spacing`: The grid spacing, in units of length.
+    - `half_space`:
         Return a frequency grid on the half space.
-        ``shape[-1]`` is the axis on which the negative
+        `shape[-1]` is the axis on which the negative
         frequencies are omitted.
 
-    Returns
-    -------
-    frequency_grid :
-        Cartesian coordinate system in frequency space.
+    **Returns:**
+
+    A cartesian coordinate system in frequency space.
     """
     frequency_grid = _make_coordinates_or_frequencies(
         shape,
         grid_spacing=grid_spacing,
         real_space=False,
         half_space=half_space,
     )
     return frequency_grid
 
 
-def cartesian_to_polar(
-    freqs: Float[Array, "y_dim x_dim 2"], square: bool = False
-) -> tuple[Inexact[Array, "y_dim x_dim"], Inexact[Array, "y_dim x_dim"]]:
-    """
-    Convert from cartesian to polar coordinates.
-
-    Arguments
-    ---------
-    freqs :
-        The cartesian coordinate system.
-    square :
-        If ``True``, return the square of the
-        radial coordinate :math:`|r|^2`. Otherwise,
-        return :math:`|r|`.
-    """
-    theta = jnp.arctan2(freqs[..., 0], freqs[..., 1])
-    k_sqr = jnp.sum(jnp.square(freqs), axis=-1)
-    if square:
-        return k_sqr, theta
+def make_frequency_slice(
+    shape: tuple[int, int],
+    grid_spacing: float | Float[np.ndarray, ""] | Float[Array, ""] = 1.0,
+    half_space: bool = True,
+) -> Float[Array, "1 {shape[0]} {shape[1]} 3"]:
+    """Create a fourier-space cartesian coordinate system on a grid. The
+    zero-frequency component is in the *center*. This is different
+    than in [`make_frequency_grid`][].
+
+    **Returns:**
+
+    The central, $q_z = 0$ slice of a 3D frequency grid `$(q_x, q_y, q_z)$`.
+    """
+    frequency_slice = make_frequency_grid(shape, grid_spacing, half_space=half_space)
+    if half_space:
+        frequency_slice = jnp.fft.fftshift(frequency_slice, axes=(0,))
     else:
-        kr = jnp.sqrt(k_sqr)
-        return kr, theta
+        frequency_slice = jnp.fft.fftshift(frequency_slice, axes=(0, 1))
+    frequency_slice = jnp.expand_dims(
+        jnp.pad(
+            frequency_slice,
+            ((0, 0), (0, 0), (0, 1)),
+            mode="constant",
+            constant_values=0.0,
+        ),
+        axis=0,
+    )
+    return frequency_slice
 
 
 def _make_coordinates_or_frequencies(
     shape: tuple[int, ...],
-    grid_spacing: float | Float[np.ndarray, ""] = 1.0,
+    grid_spacing: float | Float[np.ndarray, ""] | Float[Array, ""] = 1.0,
     real_space: bool = False,
     half_space: bool = True,
 ) -> Float[Array, "*shape ndim"]:
     ndim = len(shape)
     coords1D = []
     for idx in range(ndim):
         if real_space:
@@ -133,15 +131,15 @@
         )
 
     return coords
 
 
 def _make_coordinates_or_frequencies_1d(
     size: int,
-    grid_spacing: float | Float[np.ndarray, ""],
+    grid_spacing: float | Float[np.ndarray, ""] | Float[Array, ""],
     real_space: bool = False,
     rfftfreq: Optional[bool] = None,
 ) -> Float[Array, " size"]:
     """One-dimensional coordinates in real or fourier space"""
     if real_space:
         make_1d = lambda size, dx: jnp.fft.fftshift(jnp.fft.fftfreq(size, 1 / dx)) * size
     else:
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/io/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from ._dataset import AbstractDataset as AbstractDataset
-from ._io import (
+from ._gemmi import (
+    center_gemmi_model as center_gemmi_model,
     clean_gemmi_structure as clean_gemmi_structure,
-    extract_atom_positions_and_names as extract_atom_positions_and_names,
+    extract_atom_positions_and_numbers as extract_atom_positions_and_numbers,
     extract_gemmi_atoms as extract_gemmi_atoms,
     get_atom_info_from_gemmi_model as get_atom_info_from_gemmi_model,
+)
+from ._mdtraj import (
     get_atom_info_from_mdtraj as get_atom_info_from_mdtraj,
     mdtraj_load_from_file as mdtraj_load_from_file,
-    read_and_validate_starfile as read_and_validate_starfile,
+)
+from ._mrc import (
     read_array_from_mrc as read_array_from_mrc,
     read_array_with_spacing_from_mrc as read_array_with_spacing_from_mrc,
-    read_atoms_from_cif as read_atoms_from_cif,
-    read_atoms_from_pdb as read_atoms_from_pdb,
     write_image_stack_to_mrc as write_image_stack_to_mrc,
     write_image_to_mrc as write_image_to_mrc,
     write_volume_to_mrc as write_volume_to_mrc,
 )
-from ._particle_stack import (
-    AbstractParticleStack as AbstractParticleStack,
-)
-from ._relion import (
-    HelicalRelionDataset as HelicalRelionDataset,
-    RelionDataset as RelionDataset,
-    RelionParticleStack as RelionParticleStack,
+from ._pdb_and_cif import (
+    read_atoms_from_cif as read_atoms_from_cif,
+    read_atoms_from_pdb as read_atoms_from_pdb,
 )
+from ._starfile import read_and_validate_starfile as read_and_validate_starfile
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_dataset.py` & `cryojax-0.3.0rc2/src/cryojax/data/_dataset.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_relion.py` & `cryojax-0.3.0rc2/src/cryojax/data/_relion.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import equinox as eqx
 import jax.numpy as jnp
 import mrcfile
 import numpy as np
 import pandas as pd
 from jaxtyping import Array, Float, Int
 
+from ..io import read_and_validate_starfile
 from ..simulator import ContrastTransferFunction, EulerAnglePose, InstrumentConfig
 from ._dataset import AbstractDataset
-from ._io import read_and_validate_starfile
 from ._particle_stack import AbstractParticleStack
 
 
 RELION_REQUIRED_OPTICS_KEYS = [
     "rlnImageSize",
     "rlnVoltage",
     "rlnImagePixelSize",
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_io/gemmi.py` & `cryojax-0.3.0rc2/src/cryojax/io/_gemmi.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,43 +25,63 @@
     atom_positions: numpy array
         Array of coordinates containing atomic positions
     atom_element_names: numpy array
         Array of atomic element names
 
     """
     atoms = extract_gemmi_atoms(model)
-    atom_positions, atom_element_names = extract_atom_positions_and_names(atoms)
-    return atom_positions, atom_element_names
+    atom_positions, atom_element_numbers = extract_atom_positions_and_numbers(atoms)
+    return atom_positions, atom_element_numbers
 
 
-def clean_gemmi_structure(structure=None):
+def clean_gemmi_structure(structure):
     """
     Clean Gemmi Structure.
 
     Parameters
     ----------
     structure : Gemmi Class
         Gemmi Structure object
 
     Returns
     -------
     structure : Gemmi Class
         Same object, cleaned up of unnecessary atoms.
 
     """
-    if structure is not None:
-        structure.remove_alternative_conformations()
-        structure.remove_hydrogens()
-        structure.remove_waters()
-        structure.remove_ligands_and_waters()
-        structure.remove_empty_chains()
+    structure.remove_alternative_conformations()
+    structure.remove_hydrogens()
+    structure.remove_waters()
+    structure.remove_ligands_and_waters()
+    structure.remove_empty_chains()
 
     return structure
 
 
+def center_gemmi_model(model):
+    """
+    Translates model so that its center of mass coincides with the origin.
+
+    Parameters
+    ----------
+    model : Gemmi Class
+        Gemmi model
+    """
+    import gemmi
+
+    com = model.calculate_center_of_mass()
+    model.transform_pos_and_adp(
+        gemmi.Transform(
+            gemmi.Mat33(),  # rotation matrix is identity
+            gemmi.Vec3(-1 * com.x, -1 * com.y, -1 * com.z),
+        )
+    )
+    return model
+
+
 def extract_gemmi_atoms(model, chains=None, split_chains=False):
     """
     Extract Gemmi atoms from the input Gemmi model, separated by chain.
 
     Parameters
     ----------
     model : Gemmi Class
@@ -88,15 +108,15 @@
 
     if not split_chains:
         atoms = list(itertools.chain.from_iterable(atoms))
 
     return atoms
 
 
-def extract_atom_positions_and_names(
+def extract_atom_positions_and_numbers(
     atoms,
 ) -> tuple[Float[np.ndarray, "N 3"], Int[np.ndarray, " N"]]:
     """
     Interpret Gemmi atoms and extract a single parameter type.
 
     Parameters
     ----------
@@ -116,7 +136,29 @@
     # if list of Gemmi atoms, convert into a list of list
     if type(atoms[0]) != list:
         atoms = [atoms]
 
     positions = np.array([at.pos.tolist() for ch in atoms for at in ch])
     atomic_numbers = np.array([at.element.atomic_number for ch in atoms for at in ch])
     return positions, atomic_numbers
+
+
+def extract_atom_b_factors(atoms) -> Float[np.ndarray, "N 3"]:
+    """
+    Interpret Gemmi atoms and extract a single parameter type.
+
+    Parameters
+    ----------
+    atoms : list (of list(s)) of Gemmi atoms
+        Gemmi atom objects associated with each chain
+
+    Returns
+    -------
+    b_factors :
+        Gemmi B-factors
+    """
+    # if list of Gemmi atoms, convert into a list of list
+    if type(atoms[0]) != list:
+        atoms = [atoms]
+
+    b_factors = np.array([at.b_iso for ch in atoms for at in ch])
+    return b_factors
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_io/mdtraj.py` & `cryojax-0.3.0rc2/src/cryojax/io/_mdtraj.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_io/mrc.py` & `cryojax-0.3.0rc2/src/cryojax/io/_mrc.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/data/_io/starfile.py` & `cryojax-0.3.0rc2/src/cryojax/io/_starfile.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/image/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from . import operators as operators
 from ._average import radial_average as radial_average
+from ._downsample import (
+    downsample_with_fourier_cropping as downsample_with_fourier_cropping,
+)
 from ._edges import (
     crop_to_shape as crop_to_shape,
     crop_to_shape_with_center as crop_to_shape_with_center,
     pad_to_shape as pad_to_shape,
     resize_with_crop_or_pad as resize_with_crop_or_pad,
 )
 from ._fft import (
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_average.py` & `cryojax-0.3.0rc2/src/cryojax/image/_average.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_edges.py` & `cryojax-0.3.0rc2/src/cryojax/image/_edges.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_fft.py` & `cryojax-0.3.0rc2/src/cryojax/image/_fft.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_map_coordinates.py` & `cryojax-0.3.0rc2/src/cryojax/image/_map_coordinates.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_normalize.py` & `cryojax-0.3.0rc2/src/cryojax/image/_normalize.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_rescale_pixel_size.py` & `cryojax-0.3.0rc2/src/cryojax/image/_rescale_pixel_size.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/_spectrum.py` & `cryojax-0.3.0rc2/src/cryojax/image/_spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 """
 Helper routines to compute power spectra.
 """
 
-from typing import Optional, overload
+from typing import Literal, Optional, overload
 
 import jax.numpy as jnp
 from jaxtyping import Array, Complex, Float
 
 from ._average import radial_average
 
 
 @overload
 def powerspectrum(
     fourier_image: Complex[Array, "y_dim x_dim"],
     radial_frequency_grid: Float[Array, "y_dim x_dim"],
     pixel_size: Float[Array, ""] | float,
     *,
+    to_grid: Literal[False] = False,
+    interpolation_mode: str = "nearest",
     k_min: Optional[Float[Array, ""] | float] = None,
     k_max: Optional[Float[Array, ""] | float] = None,
 ) -> tuple[Float[Array, " n_bins"], Float[Array, " n_bins"]]: ...
 
 
 @overload
 def powerspectrum(
     fourier_image: Complex[Array, "z_dim y_dim x_dim"],
     radial_frequency_grid: Float[Array, "z_dim y_dim x_dim"],
     pixel_size: Float[Array, ""] | float,
     *,
+    to_grid: Literal[False] = False,
+    interpolation_mode: str = "nearest",
     k_min: Optional[Float[Array, ""] | float] = None,
     k_max: Optional[Float[Array, ""] | float] = None,
 ) -> tuple[Float[Array, " n_bins"], Float[Array, " n_bins"]]: ...
 
 
 @overload
 def powerspectrum(
     fourier_image: Complex[Array, "y_dim x_dim"],
     radial_frequency_grid: Float[Array, "y_dim x_dim"],
     pixel_size: Float[Array, ""] | float,
     *,
-    to_grid: bool = False,
+    to_grid: Literal[True] = True,
     interpolation_mode: str = "nearest",
     k_min: Optional[Float[Array, ""] | float] = None,
     k_max: Optional[Float[Array, ""] | float] = None,
-) -> (
-    tuple[Float[Array, " n_bins"], Float[Array, " n_bins"]]
-    | tuple[Float[Array, " n_bins"], Float[Array, "y_dim x_dim"], Float[Array, " n_bins"]]
-): ...
+) -> tuple[
+    Float[Array, " n_bins"], Float[Array, "y_dim x_dim"], Float[Array, " n_bins"]
+]: ...
 
 
 @overload
 def powerspectrum(
     fourier_image: Complex[Array, "z_dim y_dim x_dim"],
     radial_frequency_grid: Float[Array, "z_dim y_dim x_dim"],
     pixel_size: Float[Array, ""] | float,
     *,
-    to_grid: bool = False,
+    to_grid: Literal[True] = True,
     interpolation_mode: str = "nearest",
     k_min: Optional[Float[Array, ""] | float] = None,
     k_max: Optional[Float[Array, ""] | float] = None,
-) -> (
-    tuple[Float[Array, " n_bins"], Float[Array, " n_bins"]]
-    | tuple[
-        Float[Array, " n_bins"],
-        Float[Array, "z_dim y_dim x_dim"],
-        Float[Array, " n_bins"],
-    ]
-): ...
+) -> tuple[
+    Float[Array, " n_bins"],
+    Float[Array, "z_dim y_dim x_dim"],
+    Float[Array, " n_bins"],
+]: ...
 
 
 def powerspectrum(
     fourier_image: Complex[Array, "y_dim x_dim"] | Complex[Array, "z_dim y_dim x_dim"],
     radial_frequency_grid: (
         Float[Array, "y_dim x_dim"] | Float[Array, "z_dim y_dim x_dim"]
     ),
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/_filters.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional, overload
 
 import jax
 import jax.numpy as jnp
 from equinox import field
 from jaxtyping import Array, Complex, Float, Inexact
 
-from ...coordinates import make_frequencies
+from ...coordinates import make_frequency_grid
 from .._edges import resize_with_crop_or_pad
 from .._fft import irfftn, rfftn
 from .._spectrum import powerspectrum
 from ._operator import AbstractImageMultiplier
 
 
 class AbstractFilter(AbstractImageMultiplier, strict=True):
@@ -215,15 +215,15 @@
 
     Returns
     -------
     filter :
         The whitening filter.
     """
     # Make coordinates
-    micrograph_frequency_grid_in_angstroms = make_frequencies(micrograph.shape)
+    micrograph_frequency_grid_in_angstroms = make_frequency_grid(micrograph.shape)
     # Transform to fourier space
     fourier_micrograph = rfftn(micrograph)
     # Compute norms
     radial_frequency_grid = jnp.linalg.norm(
         micrograph_frequency_grid_in_angstroms, axis=-1
     )
     # Compute power spectrum
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/_fourier_operator.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/_fourier_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,25 +160,19 @@
 
 
 class FourierGaussian(AbstractFourierOperator, strict=True):
     r"""This operator represents a simple gaussian.
     Specifically, this is
 
     .. math::
-        P(k) = \kappa \exp(- \beta k^2 / 2),
+        P(k) = \kappa \exp(- \beta k^2 / 4),
 
     where :math:`k^2 = k_x^2 + k_y^2` is the length of the
     wave vector. Here, :math:`\beta` has dimensions of length
-    squared. In 2D, the real-space version of this function is given
-    by
-
-    .. math::
-        g(r) = \frac{\kappa}{2\pi \beta} \exp(- r^2 / (2 \beta)),
-
-    where :math:`r^2 = x^2 + y^2`.
+    squared.
     """
 
     amplitude: Float[Array, ""] = field(default=1.0, converter=jnp.asarray)
     b_factor: Float[Array, ""] = field(default=1.0, converter=error_if_not_positive)
 
     @overload
     def __call__(
@@ -191,15 +185,15 @@
     ) -> Float[Array, "z_dim y_dim x_dim"]: ...
 
     @override
     def __call__(
         self, freqs: Float[Array, "y_dim x_dim 2"] | Float[Array, "z_dim y_dim x_dim 3"]
     ) -> Float[Array, "y_dim x_dim"] | Float[Array, "z_dim y_dim x_dim"]:
         k_sqr = jnp.sum(freqs**2, axis=-1)
-        scaling = self.amplitude * jnp.exp(-0.5 * self.b_factor * k_sqr)
+        scaling = self.amplitude * jnp.exp(-0.25 * self.b_factor * k_sqr)
         return scaling
 
 
 FourierGaussian.__init__.__doc__ = """**Arguments:**
 
 - `amplitude`: The amplitude of the operator, equal to $\\kappa$
            in the above equation.
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/_masks.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/_masks.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/_operator.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/_operator.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/image/operators/_real_operator.py` & `cryojax-0.3.0rc2/src/cryojax/image/operators/_real_operator.py`

 * *Files 23% similar despite different names*

```diff
@@ -48,39 +48,39 @@
         raise NotImplementedError
 
 
 RealOperatorLike = AbstractRealOperator | AbstractImageOperator
 
 
 class Gaussian2D(AbstractRealOperator, strict=True):
-    r"""This operator represents a simple gaussian.
+    """This operator represents a simple gaussian in 2D.
     Specifically, this is
 
-    $$g(r) = \frac{\kappa}{2\pi \beta} \exp(- (r - r_0)^2 / (2 \beta))$$
+    $$g(r) = \\frac{\\kappa}{2\\pi \beta} \\exp(- (r - r_0)^2 / (2 \\sigma))$$
 
     where $r^2 = x^2 + y^2$.
     """
 
     amplitude: Float[Array, ""] = field(default=1.0, converter=jnp.asarray)
-    b_factor: Float[Array, ""] = field(default=1.0, converter=error_if_not_positive)
+    variance: Float[Array, ""] = field(default=1.0, converter=error_if_not_positive)
     offset: Float[Array, "2"] = field(default=(0.0, 0.0), converter=jnp.asarray)
 
     @override
     def __call__(
         self, coords: Float[Array, "y_dim x_dim 2"]
     ) -> Float[Array, "y_dim x_dim"]:
         r_sqr = jnp.sum((coords - self.offset) ** 2, axis=-1)
-        scaling = (self.amplitude / jnp.sqrt(2 * jnp.pi * self.b_factor)) * jnp.exp(
-            -0.5 * r_sqr / self.b_factor
+        scaling = (self.amplitude / jnp.sqrt(2 * jnp.pi * self.variance)) * jnp.exp(
+            -0.5 * r_sqr / self.variance
         )
         return scaling
 
 
 Gaussian2D.__init__.__doc__ = """**Arguments:**
 
 - `amplitude`: The amplitude of the operator, equal to $\\kappa$
                in the above equation.
-- `b_factor`: The variance of the gaussian, equal to $\\beta$
+- `variance`: The variance of the gaussian, equal to $\\sigma$
               in the above equation.
 - `offset`: An offset to the origin, equal to $r_0$
             in the above equation.
 """
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/pytree_manipulation.py` & `cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/pytree_manipulation.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/search_loop.py` & `cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/search_loop.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from typing import Any, Optional
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
-from jax.experimental import host_callback
 from jaxtyping import Array, PyTree
-from tqdm.auto import tqdm
 
+from ..._loop import fori_loop_tqdm_decorator
 from .custom_types import PyTreeGrid, PyTreeGridPoint
 from .pytree_manipulation import (
     tree_grid_shape,
     tree_grid_take,
     tree_grid_unravel_index,
 )
 from .search_method import AbstractGridSearchMethod
@@ -139,115 +138,14 @@
                 f"is equal to {grid_size}, and the batch size is equal "
                 f"to {method.batch_size}."
             )
         n_iterations = grid_size // method.batch_size
         body_fun = batched_body_fun
     # Run and unpack results
     if progress_bar:
-        body_fun = _loop_tqdm(n_iterations, print_every)(body_fun)
+        body_fun = fori_loop_tqdm_decorator(n_iterations, print_every)(body_fun)
     final_carry = jax.lax.fori_loop(0, n_iterations, body_fun, init_carry)
     dynamic_final_state, _ = final_carry
     final_state = eqx.combine(static_state, dynamic_final_state)
     # Return the solution
     solution = method.postprocess(tree_grid, final_state, f_struct, is_leaf=is_leaf)
     return solution
-
-
-def _loop_tqdm(
-    n_iterations: int,
-    print_every: Optional[int] = None,
-    **kwargs,
-) -> Callable:
-    """Add a tqdm progress bar to `body_fun` used in `jax.lax.fori_loop`.
-    This function is based on the implementation in [`jax_tqdm`](https://github.com/jeremiecoullon/jax-tqdm)
-    """
-
-    _update_progress_bar, close_tqdm = _build_tqdm(n_iterations, print_every, **kwargs)
-
-    def _fori_loop_tqdm_decorator(func):
-        def wrapper_progress_bar(i, val):
-            _update_progress_bar(i)
-            result = func(i, val)
-            return close_tqdm(result, i)
-
-        return wrapper_progress_bar
-
-    return _fori_loop_tqdm_decorator
-
-
-def _build_tqdm(
-    n_iterations: int,
-    print_every: Optional[int] = None,
-    **kwargs,
-) -> tuple[Callable, Callable]:
-    """Build the tqdm progress bar on the host."""
-
-    desc = kwargs.pop("desc", f"Running for {n_iterations:,} iterations")
-    message = kwargs.pop("message", desc)
-    for kwarg in ("total", "mininterval", "maxinterval", "miniters"):
-        kwargs.pop(kwarg, None)
-
-    tqdm_bars = {}
-
-    if print_every is None:
-        if n_iterations > 20:
-            print_every = int(n_iterations / 20)
-        else:
-            print_every = 1
-    else:
-        if print_every < 1:
-            raise ValueError(
-                "The number of iterations per progress bar update should "
-                f"be greater than 0. Got {print_every}."
-            )
-        elif print_every > n_iterations:
-            raise ValueError(
-                "The number of iterations per progress bar update should be less "
-                f"than the number of iterations, equal to {n_iterations}. "
-                f"Got {print_every}."
-            )
-
-    remainder = n_iterations % print_every
-
-    def _define_tqdm(arg, transform):
-        tqdm_bars[0] = tqdm(range(n_iterations), **kwargs)
-        tqdm_bars[0].set_description(message, refresh=False)
-
-    def _update_tqdm(arg, transform):
-        tqdm_bars[0].update(arg)
-
-    def _update_progress_bar(iter_num):
-        _ = jax.lax.cond(
-            iter_num == 0,
-            lambda _: host_callback.id_tap(_define_tqdm, None, result=iter_num),
-            lambda _: iter_num,
-            operand=None,
-        )
-
-        _ = jax.lax.cond(
-            # update tqdm every multiple of `print_rate` except at the end
-            (iter_num % print_every == 0) & (iter_num != n_iterations - remainder),
-            lambda _: host_callback.id_tap(_update_tqdm, print_every, result=iter_num),
-            lambda _: iter_num,
-            operand=None,
-        )
-
-        _ = jax.lax.cond(
-            # update tqdm by `remainder`
-            iter_num == n_iterations - remainder,
-            lambda _: host_callback.id_tap(_update_tqdm, remainder, result=iter_num),
-            lambda _: iter_num,
-            operand=None,
-        )
-
-    def _close_tqdm(arg, transform):
-        tqdm_bars[0].close()
-
-    def close_tqdm(result, iter_num):
-        return jax.lax.cond(
-            iter_num == n_iterations - 1,
-            lambda _: host_callback.id_tap(_close_tqdm, None, result=result),
-            lambda _: result,
-            operand=None,
-        )
-
-    return _update_progress_bar, close_tqdm
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/_grid_search/search_method.py` & `cryojax-0.3.0rc2/src/cryojax/inference/_grid_search/search_method.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/_transforms/lie_group_transforms.py` & `cryojax-0.3.0rc2/src/cryojax/inference/_transforms/lie_group_transforms.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/_transforms/transforms.py` & `cryojax-0.3.0rc2/src/cryojax/inference/_transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/distributions/_base_distribution.py` & `cryojax-0.3.0rc2/src/cryojax/inference/distributions/_base_distribution.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/inference/distributions/_gaussian_distributions.py` & `cryojax-0.3.0rc2/src/cryojax/inference/distributions/_gaussian_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,15 @@
             Array,
             "{self.imaging_pipeline.instrument_config.y_dim} "
             "{self.imaging_pipeline.instrument_config.x_dim//2+1}",
         ]
     ):
         """Sample from the gaussian noise model."""
         pipeline = self.imaging_pipeline
-        freqs = (
-            pipeline.instrument_config.wrapped_padded_frequency_grid_in_angstroms.get()
-        )
+        freqs = pipeline.instrument_config.padded_frequency_grid_in_angstroms
         # Compute the zero mean variance and scale up to be independent of the number of
         # pixels
         padded_n_pixels = pipeline.instrument_config.padded_n_pixels
         std = jnp.sqrt(padded_n_pixels * self.variance_function(freqs))
         noise = pipeline.postprocess(
             std
             * jr.normal(rng_key, shape=freqs.shape[0:-1])
@@ -132,15 +130,15 @@
 
         **Arguments:**
 
         - `observed` : The observed data in fourier space.
         """
         pipeline = self.imaging_pipeline
         n_pixels = pipeline.instrument_config.n_pixels
-        freqs = pipeline.instrument_config.wrapped_frequency_grid_in_angstroms.get()
+        freqs = pipeline.instrument_config.frequency_grid_in_angstroms
         # Compute the variance and scale up to be independent of the number of pixels
         variance = n_pixels * self.variance_function(freqs)
         # Create simulated data
         simulated = self.compute_signal(get_real=False)
         # Compute residuals
         residuals = simulated - observed
         # Compute standard normal random variables
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/rotations/_lie_group.py` & `cryojax-0.3.0rc2/src/cryojax/rotations/_lie_group.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/rotations/_rotation.py` & `cryojax-0.3.0rc2/src/cryojax/rotations/_rotation.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/rotations/_utils.py` & `cryojax-0.3.0rc2/src/cryojax/rotations/_utils.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,31 @@
     AbstractFourierVoxelExtraction as AbstractFourierVoxelExtraction,
     AbstractPotentialIntegrator as AbstractPotentialIntegrator,
     AbstractVoxelPotentialIntegrator as AbstractVoxelPotentialIntegrator,
     FourierSliceExtraction as FourierSliceExtraction,
     NufftProjection as NufftProjection,
 )
 from ._potential_representation import (
-    AbstractFourierVoxelGridPotential as AbstractFourierVoxelGridPotential,
+    AbstractAtomicPotential as AbstractAtomicPotential,
     AbstractPotentialRepresentation as AbstractPotentialRepresentation,
+    AbstractTabulatedAtomicPotential as AbstractTabulatedAtomicPotential,
     AbstractVoxelPotential as AbstractVoxelPotential,
-    build_real_space_voxels_from_atoms as build_real_space_voxels_from_atoms,
-    evaluate_3d_atom_potential as evaluate_3d_atom_potential,
-    evaluate_3d_real_space_gaussian as evaluate_3d_real_space_gaussian,
     FourierVoxelGridPotential as FourierVoxelGridPotential,
     FourierVoxelGridPotentialInterpolator as FourierVoxelGridPotentialInterpolator,
+    GaussianMixtureAtomicPotential as GaussianMixtureAtomicPotential,
+    PengAtomicPotential as PengAtomicPotential,
     RealVoxelCloudPotential as RealVoxelCloudPotential,
     RealVoxelGridPotential as RealVoxelGridPotential,
 )
 from ._scattering_theory import (
-    AbstractLinearScatteringTheory as AbstractLinearScatteringTheory,
     AbstractScatteringTheory as AbstractScatteringTheory,
-    LinearScatteringTheory as LinearScatteringTheory,
+    AbstractWeakPhaseScatteringTheory as AbstractWeakPhaseScatteringTheory,
+    compute_phase_shifts_from_integrated_potential as compute_phase_shifts_from_integrated_potential,  # noqa: E501
     LinearSuperpositionScatteringTheory as LinearSuperpositionScatteringTheory,
+    WeakPhaseScatteringTheory as WeakPhaseScatteringTheory,
 )
 from ._solvent import (
     AbstractIce as AbstractIce,
     GaussianIce as GaussianIce,
 )
 from ._structural_ensemble import (
     AbstractConformationalVariable as AbstractConformationalVariable,
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_detector.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         instrument_config: InstrumentConfig,
         key: Optional[PRNGKeyArray] = None,
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         """Pass the image through the detector model."""
         N_pix = np.prod(instrument_config.padded_shape)
-        frequency_grid = instrument_config.wrapped_padded_frequency_grid_in_pixels.get()
+        frequency_grid = instrument_config.padded_frequency_grid_in_pixels
         # Compute the time-integrated electron flux in pixels
         electrons_per_pixel = (
             instrument_config.electrons_per_angstrom_squared
             * instrument_config.pixel_size**2
         )
         # ... now the total number of electrons over the entire image
         electrons_per_image = N_pix * electrons_per_pixel
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_imaging_pipeline.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_imaging_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,17 +97,15 @@
         else:
             # ... otherwise, apply filter, crop, and mask, again trying to
             # minimize moving back and forth between real and fourier space
             is_filter_applied = True if self.filter is None else False
             if (
                 self.filter is not None
                 and self.filter.buffer.shape
-                == instrument_config.wrapped_padded_frequency_grid_in_pixels.get().shape[
-                    0:2
-                ]
+                == instrument_config.padded_frequency_grid_in_pixels.shape[0:2]
             ):
                 # ... apply the filter here if it is the same size as the padded
                 # coordinates
                 is_filter_applied = True
                 image = self.filter(image)
             image = irfftn(image, s=instrument_config.padded_shape)
             image = instrument_config.crop_to_shape(image)
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_pose.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_pose.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_solvent.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_solvent.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import jax.random as jr
 import numpy as np
 from equinox import Module
 from jaxtyping import Array, Complex, PRNGKeyArray
 
 from ..image.operators import FourierOperatorLike
 from ._instrument_config import InstrumentConfig
+from ._scattering_theory import compute_phase_shifts_from_integrated_potential
 
 
 class AbstractIce(Module, strict=True):
     """Base class for an ice model."""
 
     @abstractmethod
     def sample_fourier_phase_shifts_from_ice(
@@ -50,17 +51,17 @@
 
 class GaussianIce(AbstractIce, strict=True):
     r"""Ice modeled as gaussian noise.
 
     **Attributes:**
 
     - `variance` : A function that computes the variance
-                 of the ice, modeled as colored gaussian noise.
-                 The dimensions of this function are a squared
-                 phase contrast.
+                   of the ice, modeled as colored gaussian noise.
+                   The dimensions of this function are the square
+                   of the dimensions of an integrated potential.
     """
 
     variance: FourierOperatorLike
 
     def __init__(self, variance: FourierOperatorLike):
         self.variance = variance
 
@@ -68,20 +69,22 @@
     def sample_fourier_phase_shifts_from_ice(
         self, key: PRNGKeyArray, instrument_config: InstrumentConfig
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         """Sample a realization of the ice phase shifts as colored gaussian noise."""
         N_pix = np.prod(instrument_config.padded_shape)
-        frequency_grid_in_angstroms = (
-            instrument_config.wrapped_padded_frequency_grid_in_angstroms.get()
-        )
+        frequency_grid_in_angstroms = instrument_config.padded_frequency_grid_in_angstroms
         # Compute standard deviation, scaling up by the variance by the number
         # of pixels to make the realization independent pixel-independent in real-space.
         std = jnp.sqrt(N_pix * self.variance(frequency_grid_in_angstroms))
-        ice_phase_at_exit_plane = std * jr.normal(
+        ice_integrated_potential_at_exit_plane = std * jr.normal(
             key,
             shape=frequency_grid_in_angstroms.shape[0:-1],
             dtype=complex,
         ).at[0, 0].set(0.0)
+        ice_phase_shifts_at_exit_plane = compute_phase_shifts_from_integrated_potential(
+            ice_integrated_potential_at_exit_plane,
+            instrument_config.wavelength_in_angstroms,
+        )
 
-        return ice_phase_at_exit_plane
+        return ice_phase_shifts_at_exit_plane
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_assembly/assembly.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_assembly/helix.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_assembly/helix.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/base_potential_integrator.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/base_potential_integrator.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/fourier_voxel_extract.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/fourier_voxel_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         instrument_config: InstrumentConfig,
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         """Compute a projection of the real-space potential by extracting
         a central slice in fourier space.
         """
-        frequency_slice = potential.wrapped_frequency_slice_in_pixels.get()
+        frequency_slice = potential.frequency_slice_in_pixels
         N = frequency_slice.shape[1]
         if potential.shape != (N, N, N):
             raise AttributeError(
                 "Only cubic boxes are supported for fourier slice extraction."
             )
         # Compute the fourier projection
         if isinstance(potential, FourierVoxelGridPotentialInterpolator):
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_integrator/nufft_project.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_integrator/nufft_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,23 +59,21 @@
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         """Rasterize image with non-uniform FFTs."""
         if isinstance(potential, RealVoxelGridPotential):
             shape = potential.shape
             fourier_projection = self.project_voxel_cloud_with_nufft(
                 potential.real_voxel_grid.ravel(),
-                potential.wrapped_coordinate_grid_in_pixels.get().reshape(
-                    (math.prod(shape), 3)
-                ),
+                potential.coordinate_grid_in_pixels.reshape((math.prod(shape), 3)),
                 instrument_config.padded_shape,
             )
         elif isinstance(potential, RealVoxelCloudPotential):
             fourier_projection = self.project_voxel_cloud_with_nufft(
                 potential.voxel_weights,
-                potential.wrapped_coordinate_list_in_pixels.get(),
+                potential.coordinate_list_in_pixels,
                 instrument_config.padded_shape,
             )
         else:
             raise ValueError(
                 "Supported density representations are RealVoxelGrid and VoxelCloud."
             )
         return fourier_projection
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/base_potential.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/base_potential.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_potential_representation/voxel_potential.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_potential_representation/voxel_potential.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 """
 Voxel-based representations of the scattering potential.
 """
 
 from abc import abstractmethod
 from functools import cached_property
-from typing import (
-    Any,
-    cast,
-    ClassVar,
-    Optional,
-)
+from typing import cast, ClassVar, Optional
 from typing_extensions import override, Self
 
 import equinox as eqx
-import jax
 import jax.numpy as jnp
 import numpy as np
 from equinox import AbstractClassVar, AbstractVar, field
-from jaxtyping import Array, Complex, Float, Int
+from jaxtyping import Array, Complex, Float
 
 from ..._errors import error_if_not_positive
-from ...constants import get_form_factor_params
-from ...coordinates import CoordinateGrid, CoordinateList, FrequencySlice
+from ...coordinates import make_coordinate_grid, make_frequency_slice
 from ...image import (
     compute_spline_coefficients,
     crop_to_shape,
     fftn,
     pad_to_shape,
 )
 from ...image.operators import AbstractFilter
@@ -53,60 +46,45 @@
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     ) -> Self:
         """Load an `AbstractVoxelPotential` from real-valued 3D electron
         scattering potential.
         """
         raise NotImplementedError
 
-    @classmethod
-    @abstractmethod
-    def from_atoms(
-        cls,
-        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
-        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[
-            Float[Array, "n_atoms n_form_factors"]
-            | Float[np.ndarray, "n_atoms n_form_factors"]
-        ] = None,
-        **kwargs: Any,
-    ) -> Self:
-        """Load an `AbstractVoxelPotential` from atom positions and identities."""
-        raise NotImplementedError
-
 
+# Not public API
 class AbstractFourierVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstract interface of a 3D scattering potential voxel grid
     in fourier-space.
     """
 
-    wrapped_frequency_slice_in_pixels: AbstractVar[FrequencySlice]
+    frequency_slice_in_pixels: AbstractVar[Float[Array, "1 dim dim 3"]]
 
     @abstractmethod
     def __init__(
         self,
         fourier_voxel_grid: Complex[Array, "dim dim dim"],
-        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        frequency_slice_in_pixels: Float[Array, "1 dim dim 3"],
         voxel_size: Float[Array, ""] | float,
     ):
         raise NotImplementedError
 
     @cached_property
-    def wrapped_frequency_slice_in_angstroms(self) -> FrequencySlice:
-        """The `wrapped_frequency_slice` in angstroms."""
-        return self.wrapped_frequency_slice_in_pixels / self.voxel_size
+    def frequency_slice_in_angstroms(self) -> Float[Array, "1 dim dim 3"]:
+        """The `frequency_slice_in_pixels` in angstroms."""
+        return _safe_multiply_grid_by_constant(
+            self.frequency_slice_in_pixels, 1 / self.voxel_size
+        )
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
+        """Return a new potential with a rotated `frequency_slice_in_pixels`."""
         return eqx.tree_at(
-            lambda d: d.wrapped_frequency_slice_in_pixels.array,
+            lambda d: d.frequency_slice_in_pixels,
             self,
-            pose.rotate_coordinates(
-                self.wrapped_frequency_slice_in_pixels.get(), inverse=True
-            ),
+            pose.rotate_coordinates(self.frequency_slice_in_pixels, inverse=True),
         )
 
     @classmethod
     def from_real_voxel_grid(
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
@@ -132,15 +110,15 @@
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Pad template
         if pad_scale < 1.0:
-            raise ValueError("pad_scale must be greater than 1.0")
+            raise ValueError("`pad_scale` must be greater than 1.0")
         # ... always pad to even size to avoid interpolation issues in
         # fourier slice extraction.
         padded_shape = cast(
             tuple[int, int, int],
             tuple([int(s * pad_scale) for s in real_voxel_grid.shape]),
         )
         padded_real_voxel_grid = pad_to_shape(
@@ -153,106 +131,68 @@
             fftn(padded_real_voxel_grid)
             if filter is None
             else filter(fftn(padded_real_voxel_grid))
         )
         # ... store the potential grid with the zero frequency component in the center
         fourier_voxel_grid = jnp.fft.fftshift(fourier_voxel_grid_with_zero_in_corner)
         # ... create in-plane frequency slice on the half space
-        frequency_slice = FrequencySlice(
+        frequency_slice = make_frequency_slice(
             cast(tuple[int, int], padded_real_voxel_grid.shape[:-1]), half_space=False
         )
 
         return cls(fourier_voxel_grid, frequency_slice, voxel_size)
 
-    @classmethod
-    def from_atoms(
-        cls,
-        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
-        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[
-            Float[Array, "n_atoms n_form_factors"]
-            | Float[np.ndarray, "n_atoms n_form_factors"]
-        ] = None,
-        **kwargs: Any,
-    ) -> Self:
-        """Load an `AbstractFourierVoxelGridPotential` from atom positions and
-        identities.
-
-        **Arguments:**
-
-        - `**kwargs`: Passed to `AbstractFourierVoxelGridPotential.from_real_voxel_grid`
-        """
-        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
-        a_vals, b_vals = get_form_factor_params(
-            jnp.asarray(atom_identities), form_factors
-        )
-
-        potential = build_real_space_voxels_from_atoms(
-            jnp.asarray(atom_positions),
-            a_vals,
-            b_vals,
-            coordinate_grid_in_angstroms.get(),
-        )
-
-        return cls.from_real_voxel_grid(
-            potential,
-            voxel_size,
-            **kwargs,
-        )
-
 
 class FourierVoxelGridPotential(AbstractFourierVoxelGridPotential):
     """A 3D scattering potential voxel grid in fourier-space."""
 
     fourier_voxel_grid: Complex[Array, "dim dim dim"]
-    wrapped_frequency_slice_in_pixels: FrequencySlice
+    frequency_slice_in_pixels: Float[Array, "1 dim dim 3"]
     voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = False
 
     @override
     def __init__(
         self,
         fourier_voxel_grid: Complex[Array, "dim dim dim"],
-        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        frequency_slice_in_pixels: Float[Array, "1 dim dim 3"],
         voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `fourier_voxel_grid`: The cubic voxel grid in fourier space.
-        - `wrapped_frequency_slice_in_pixels`: Frequency slice coordinate system,
-                                               wrapped in a `FrequencySlice` object.
+        - `frequency_slice_in_pixels`: Frequency slice coordinate system.
         - `voxel_size`: The voxel size.
         """
         self.fourier_voxel_grid = jnp.asarray(fourier_voxel_grid)
-        self.wrapped_frequency_slice_in_pixels = wrapped_frequency_slice_in_pixels
+        self.frequency_slice_in_pixels = frequency_slice_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
+        """The shape of the `fourier_voxel_grid`."""
         return cast(tuple[int, int, int], self.fourier_voxel_grid.shape)
 
 
 class FourierVoxelGridPotentialInterpolator(AbstractFourierVoxelGridPotential):
     """A 3D scattering potential voxel grid in fourier-space, represented
     by spline coefficients.
     """
 
     coefficients: Float[Array, "coeff_dim coeff_dim coeff_dim"]
-    wrapped_frequency_slice_in_pixels: FrequencySlice
+    frequency_slice_in_pixels: Float[Array, "1 dim dim 3"]
     voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = False
 
     def __init__(
         self,
         fourier_voxel_grid: Float[Array, "dim dim dim"],
-        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        frequency_slice_in_pixels: Float[Array, "1 dim dim 3"],
         voxel_size: Float[Array, ""] | float,
     ):
         """
         !!! note
             The argument `fourier_voxel_grid` is used to set
             `FourierVoxelGridPotentialInterpolator.coefficients` in the `__init__`,
             but it is not stored in the class. For example,
@@ -264,209 +204,180 @@
             assert hasattr(voxels, "fourier_voxel_grid")  # This will return an error
             assert hasattr(voxels, "coefficients")  # Instead, store spline coefficients
             ```
 
         **Arguments:**
 
         - `fourier_voxel_grid`: The cubic voxel grid in fourier space.
-        - `wrapped_frequency_slice_in_pixels`: Frequency slice coordinate system,
+        - `frequency_slice_in_pixels`: Frequency slice coordinate system,
                                                wrapped in a `FrequencySlice` object.
         - `voxel_size`: The voxel size.
         """
         self.coefficients = compute_spline_coefficients(jnp.asarray(fourier_voxel_grid))
-        self.wrapped_frequency_slice_in_pixels = wrapped_frequency_slice_in_pixels
+        self.frequency_slice_in_pixels = frequency_slice_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
+        """The shape of the original `fourier_voxel_grid` from which
+        `coefficients` were computed.
+        """
         return cast(tuple[int, int, int], tuple([s - 2 for s in self.coefficients.shape]))
 
 
 class RealVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstraction of a 3D scattering potential voxel grid in real-space."""
 
     real_voxel_grid: Float[Array, "dim dim dim"]
-    wrapped_coordinate_grid_in_pixels: CoordinateGrid
+    coordinate_grid_in_pixels: Float[Array, "dim dim dim 3"]
     voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = True
 
     def __init__(
         self,
         real_voxel_grid: Float[Array, "dim dim dim"],
-        wrapped_coordinate_grid_in_pixels: CoordinateGrid,
+        coordinate_grid_in_pixels: Float[Array, "dim dim dim 3"],
         voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `real_voxel_grid`: The voxel grid in fourier space.
-        - `wrapped_coordinate_grid_in_pixels`: A coordinate grid, wrapped into a
-                                               `CoordinateGrid` object.
+        - `coordinate_grid_in_pixels`: A coordinate grid.
         - `voxel_size`: The voxel size.
         """
         self.real_voxel_grid = jnp.asarray(real_voxel_grid)
-        self.wrapped_coordinate_grid_in_pixels = wrapped_coordinate_grid_in_pixels
+        self.coordinate_grid_in_pixels = coordinate_grid_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
+        """The shape of the `real_voxel_grid`."""
         return cast(tuple[int, int, int], self.real_voxel_grid.shape)
 
     @cached_property
-    def wrapped_coordinate_grid_in_angstroms(self) -> CoordinateGrid:
-        """The `coordinate_grid` in angstroms."""
-        return self.voxel_size * self.wrapped_coordinate_grid_in_pixels  # type: ignore
+    def coordinate_grid_in_angstroms(self) -> Float[Array, "dim dim dim 3"]:
+        """The `coordinate_grid_in_pixels` in angstroms."""
+        return _safe_multiply_grid_by_constant(
+            self.coordinate_grid_in_pixels, self.voxel_size
+        )
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
+        """Return a new potential with a rotated
+        `coordinate_grid_in_pixels`.
+        """
         return eqx.tree_at(
-            lambda d: d.wrapped_coordinate_grid_in_pixels.array,
+            lambda d: d.coordinate_grid_in_pixels,
             self,
-            pose.rotate_coordinates(
-                self.wrapped_coordinate_grid_in_pixels.get(), inverse=False
-            ),
+            pose.rotate_coordinates(self.coordinate_grid_in_pixels, inverse=False),
         )
 
     @classmethod
     def from_real_voxel_grid(
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
-        coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
+        coordinate_grid_in_pixels: Optional[Float[Array, "dim dim dim 3"]] = None,
         crop_scale: Optional[float] = None,
     ) -> Self:
         """Load a `RealVoxelGridPotential` from a real-valued 3D electron
         scattering potential voxel grid.
 
         **Arguments:**
 
         - `real_voxel_grid`: An electron scattering potential voxel grid in real space.
         - `voxel_size`: The voxel size of `real_voxel_grid`.
         - `crop_scale`: Scale factor at which to crop `real_voxel_grid`.
-                      Must be a value less than `1.0`.
+                        Must be a value greater than `1`.
         """
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Make coordinates if not given
         if coordinate_grid_in_pixels is None:
             # Option for cropping template
             if crop_scale is not None:
-                if crop_scale > 1.0:
-                    raise ValueError("crop_scale must be less than 1.0")
+                if crop_scale < 1.0:
+                    raise ValueError("`crop_scale` must be greater than 1.0")
                 cropped_shape = cast(
                     tuple[int, int, int],
-                    tuple([int(s * crop_scale) for s in real_voxel_grid.shape[-3:]]),
+                    tuple([int(s / crop_scale) for s in real_voxel_grid.shape[-3:]]),
                 )
                 real_voxel_grid = crop_to_shape(real_voxel_grid, cropped_shape)
-            coordinate_grid_in_pixels = CoordinateGrid(real_voxel_grid.shape[-3:])
+            coordinate_grid_in_pixels = make_coordinate_grid(real_voxel_grid.shape[-3:])
 
         return cls(real_voxel_grid, coordinate_grid_in_pixels, voxel_size)
 
-    @classmethod
-    def from_atoms(
-        cls,
-        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
-        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[
-            Float[Array, "n_atoms n_form_factors"]
-            | Float[np.ndarray, "n_atoms n_form_factors"]
-        ] = None,
-        **kwargs: Any,
-    ) -> Self:
-        """Load a `RealVoxelGridPotential` from atom positions and identities.
-
-        **Arguments:**
-
-        - `**kwargs`: Passed to `RealVoxelGridPotential.from_real_voxel_grid`
-        """
-        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
-        a_vals, b_vals = get_form_factor_params(
-            jnp.asarray(atom_identities), form_factors
-        )
-
-        real_voxel_grid = build_real_space_voxels_from_atoms(
-            jnp.asarray(atom_positions),
-            a_vals,
-            b_vals,
-            coordinate_grid_in_angstroms.get(),
-        )
-
-        return cls.from_real_voxel_grid(
-            real_voxel_grid,
-            voxel_size,
-            coordinate_grid_in_pixels=coordinate_grid_in_angstroms / voxel_size,
-            **kwargs,
-        )
-
 
 class RealVoxelCloudPotential(AbstractVoxelPotential, strict=True):
     """Abstraction of a 3D electron scattering potential voxel point cloud.
 
     !!! info
         This object is similar to the `RealVoxelGridPotential`. Instead
         of storing the whole voxel grid, a `RealVoxelCloudPotential` need
         only store points of non-zero scattering potential. Therefore,
         a `RealVoxelCloudPotential` stores a point cloud of scattering potential
         voxel values. Instantiating with the `from_real_voxel_grid` constructor
         will automatically mask points of zero scattering potential.
     """
 
     voxel_weights: Float[Array, " size"]
-    wrapped_coordinate_list_in_pixels: CoordinateList
+    coordinate_list_in_pixels: Float[Array, "size 3"]
     voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = True
 
     def __init__(
         self,
         voxel_weights: Float[Array, " size"],
-        wrapped_coordinate_list_in_pixels: CoordinateList,
+        coordinate_list_in_pixels: Float[Array, "size 3"],
         voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `voxel_weights`: A point-cloud of voxel scattering potential values.
-        - `wrapped_coordinate_list_in_pixels`: Coordinate list for the `voxel_weights`,
-                                               wrapped in a `CoordinateList` object.
+        - `coordinate_list_in_pixels`: Coordinate list for the `voxel_weights`.
         - `voxel_size`: The voxel size.
         """
         self.voxel_weights = jnp.asarray(voxel_weights)
-        self.wrapped_coordinate_list_in_pixels = wrapped_coordinate_list_in_pixels
+        self.coordinate_list_in_pixels = coordinate_list_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int]:
+        """The shape of `voxel_weights`."""
         return cast(tuple[int], self.voxel_weights.shape)
 
     @cached_property
-    def wrapped_coordinate_list_in_angstroms(self) -> CoordinateList:
-        """The `coordinate_list` in angstroms."""
-        return self.voxel_size * self.wrapped_coordinate_list_in_pixels  # type: ignore
+    def coordinate_list_in_angstroms(self) -> Float[Array, "size 3"]:
+        """The `coordinate_list_in_pixels` in angstroms."""
+        return _safe_multiply_list_by_constant(
+            self.coordinate_list_in_pixels, self.voxel_size
+        )
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
+        """Return a new potential with a rotated
+        `coordinate_list_in_pixels`.
+        """
         return eqx.tree_at(
-            lambda d: d.wrapped_coordinate_list_in_pixels.array,
+            lambda d: d.coordinate_list_in_pixels,
             self,
-            pose.rotate_coordinates(
-                self.wrapped_coordinate_list_in_pixels.get(), inverse=False
-            ),
+            pose.rotate_coordinates(self.coordinate_list_in_pixels, inverse=False),
         )
 
     @classmethod
     def from_real_voxel_grid(
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
-        coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
+        coordinate_grid_in_pixels: Optional[Float[Array, "dim dim dim 3"]] = None,
         rtol: float = 1e-05,
         atol: float = 1e-08,
         size: Optional[int] = None,
         fill_value: Optional[float] = None,
     ) -> Self:
         """Load an `RealVoxelCloudPotential` from a real-valued 3D electron
         scattering potential voxel grid.
@@ -488,148 +399,37 @@
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Make coordinates if not given
         if coordinate_grid_in_pixels is None:
-            coordinate_grid_in_pixels = CoordinateGrid(real_voxel_grid.shape)
+            coordinate_grid_in_pixels = make_coordinate_grid(real_voxel_grid.shape)
         # ... mask zeros to store smaller arrays. This
         # option is not jittable.
         nonzero = jnp.where(
             ~jnp.isclose(real_voxel_grid, 0.0, rtol=rtol, atol=atol),
             size=size,
             fill_value=fill_value,
         )
         flat_potential = real_voxel_grid[nonzero]
-        coordinate_list = CoordinateList(coordinate_grid_in_pixels.get()[nonzero])
+        coordinate_list = coordinate_grid_in_pixels[nonzero]
 
         return cls(flat_potential, coordinate_list, voxel_size)
 
-    @classmethod
-    def from_atoms(
-        cls,
-        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
-        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[
-            Float[Array, "n_atoms n_form_factors"]
-            | Float[np.ndarray, "n_atoms n_form_factors"]
-        ] = None,
-        **kwargs: Any,
-    ) -> Self:
-        """Load a `RealVoxelCloudPotential` from atom positions and identities.
-
-        **Arguments:**
-
-        - `**kwargs`: Passed to `RealVoxelCloudPotential.from_real_voxel_grid`
-        """
-        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
-        a_vals, b_vals = get_form_factor_params(
-            jnp.asarray(atom_identities), form_factors
-        )
-
-        real_voxel_grid = build_real_space_voxels_from_atoms(
-            jnp.asarray(atom_positions),
-            a_vals,
-            b_vals,
-            coordinate_grid_in_angstroms.get(),
-        )
-
-        return cls.from_real_voxel_grid(
-            real_voxel_grid,
-            voxel_size,
-            coordinate_grid_in_pixels=coordinate_grid_in_angstroms / voxel_size,
-            **kwargs,
-        )
-
-
-def evaluate_3d_real_space_gaussian(
-    coordinate_grid_in_angstroms: Float[Array, "z_dim y_dim x_dim 3"],
-    atom_position: Float[Array, "3"],
-    a: Float[Array, ""],
-    b: Float[Array, ""],
-) -> Float[Array, "z_dim y_dim x_dim"]:
-    """Evaluate a gaussian on a 3D grid.
-    The naming convention for parameters follows "Robust
-    Parameterization of Elastic and Absorptive Electron Atomic Scattering
-    Factors" by Peng et al.
-
-    **Arguments:**
-
-    - `coordinate_grid`: The coordinate system of the grid.
-    - `pos`: The center of the gaussian.
-    - `a`: A scale factor.
-    - `b`: The scale of the gaussian.
-
-    **Returns:**
-
-    The potential of the gaussian on the grid.
-    """
-    b_inverse = 4.0 * jnp.pi / b
-    sq_distances = jnp.sum(
-        b_inverse * (coordinate_grid_in_angstroms - atom_position) ** 2, axis=-1
-    )
-    return jnp.exp(-jnp.pi * sq_distances) * a * b_inverse ** (3.0 / 2.0)
-
-
-def evaluate_3d_atom_potential(
-    coordinate_grid_in_angstroms: Float[Array, "z_dim y_dim x_dim 3"],
-    atom_position: Float[Array, "3"],
-    atomic_as: Float[Array, " n_form_factors"],
-    atomic_bs: Float[Array, " n_form_factors"],
-) -> Float[Array, "z_dim y_dim x_dim"]:
-    """Evaluates the electron potential of a single atom on a 3D grid.
-
-    **Arguments:**
-
-    - `coordinate_grid_in_angstroms`: The coordinate system of the grid.
-    - `atom_position`: The location of the atom.
-    - `atomic_as`: The intensity values for each gaussian in the atom.
-    - `atomic_bs`: The inverse scale factors for each gaussian in the atom.
-
-    **Returns:**
 
-    The potential of the atom evaluated on the grid.
+def _safe_multiply_grid_by_constant(
+    grid: Float[Array, "z_dim y_dim x_dim 3"], constant: Float[Array, ""]
+) -> Float[Array, "z_dim y_dim x_dim 3"]:
+    """Multiplies a coordinate grid by a constant in a
+    safe way for gradient computation.
     """
-    eval_fxn = jax.vmap(evaluate_3d_real_space_gaussian, in_axes=(None, None, 0, 0))
-    return jnp.sum(
-        eval_fxn(coordinate_grid_in_angstroms, atom_position, atomic_as, atomic_bs),
-        axis=0,
-    )
+    return jnp.where(grid != 0.0, jnp.asarray(constant) * grid, 0.0)
 
 
-@jax.jit
-def build_real_space_voxels_from_atoms(
-    atom_positions: Float[Array, "n_atoms 3"],
-    ff_a: Float[Array, "n_atoms n_form_factors"],
-    ff_b: Float[Array, "n_atoms n_form_factors"],
-    coordinate_grid_in_angstroms: Float[Array, "dim dim dim 3"],
-) -> Float[Array, "dim dim dim"]:
+def _safe_multiply_list_by_constant(
+    coordinate_list: Float[Array, "size 3"], constant: Float[Array, ""]
+) -> Float[Array, "size 3"]:
+    """Multiplies a coordinate grid by a constant in a
+    safe way for gradient computation.
     """
-    Build a voxel representation of an atomic model.
-
-    **Arguments**
-
-    - `atom_coords`: The coordinates of the atoms.
-    - `ff_a`: Intensity values for each Gaussian in the atom
-    - `ff_b` : The inverse scale factors for each Gaussian in the atom
-    - `coordinate_grid` : The coordinates of each voxel in the grid.
-
-    **Returns:**
-
-    The voxel representation of the atomic model.
-    """
-    voxel_grid_buffer = jnp.zeros(coordinate_grid_in_angstroms.shape[:-1])
-
-    def add_gaussian_to_potential(i, potential):
-        potential += evaluate_3d_atom_potential(
-            coordinate_grid_in_angstroms, atom_positions[i], ff_a[i], ff_b[i]
-        )
-        return potential
-
-    voxel_grid = jax.lax.fori_loop(
-        0, atom_positions.shape[0], add_gaussian_to_potential, voxel_grid_buffer
-    )
-
-    return voxel_grid
+    return jnp.where(coordinate_list != 0.0, jnp.asarray(constant) * coordinate_list, 0.0)
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_scattering_theory/base_scattering_theory.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/base_scattering_theory.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_scattering_theory/linear_scattering_theory.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_scattering_theory/weak_phase_scattering_theory.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 from .._structural_ensemble import (
     AbstractConformationalVariable,
     AbstractStructuralEnsemble,
     AbstractStructuralEnsembleBatcher,
 )
 from .._transfer_theory import ContrastTransferTheory
 from .base_scattering_theory import AbstractScatteringTheory
+from .common_functions import compute_phase_shifts_from_integrated_potential
 
 
-class AbstractLinearScatteringTheory(AbstractScatteringTheory, strict=True):
+class AbstractWeakPhaseScatteringTheory(AbstractScatteringTheory, strict=True):
     """Base class for a scattering theory in linear image formation theory
     (the weak-phase approximation).
     """
 
     @abstractmethod
     def compute_fourier_phase_shifts_at_exit_plane(
         self,
@@ -55,15 +56,15 @@
         )
         fourier_squared_wavefunction_at_detector_plane = (
             (2 * fourier_contrast_at_detector_plane).at[0, 0].add(1.0 * N1 * N2)
         )
         return fourier_squared_wavefunction_at_detector_plane
 
 
-class LinearScatteringTheory(AbstractLinearScatteringTheory, strict=True):
+class WeakPhaseScatteringTheory(AbstractWeakPhaseScatteringTheory, strict=True):
     """Base linear image formation theory."""
 
     structural_ensemble: AbstractStructuralEnsemble
     potential_integrator: AbstractPotentialIntegrator
     transfer_theory: ContrastTransferTheory
     solvent: Optional[AbstractIce] = None
 
@@ -73,15 +74,15 @@
         instrument_config: InstrumentConfig,
         rng_key: Optional[PRNGKeyArray] = None,
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         # Compute the phase shifts in the exit plane
         fourier_phase_shifts_at_exit_plane = (
-            _compute_phase_shifts_from_projected_potential(
+            _compute_phase_shifts_from_integrated_potential(
                 self.structural_ensemble, self.potential_integrator, instrument_config
             )
         )
 
         if rng_key is not None:
             # Get the potential of the specimen plus the ice
             if self.solvent is not None:
@@ -109,26 +110,27 @@
             instrument_config,
             defocus_offset=self.structural_ensemble.pose.offset_z_in_angstroms,
         )
 
         return fourier_contrast_at_detector_plane
 
 
-LinearScatteringTheory.__init__.__doc__ = """**Arguments:**
+WeakPhaseScatteringTheory.__init__.__doc__ = """**Arguments:**
 
 - `structural_ensemble`: The structural ensemble of scattering potentials.
 - `potential_integrator`: The method for integrating the scattering potential.
 - `transfer_theory`: The contrast transfer theory.
 - `solvent`: The model for the solvent.
 """
 
 
-class LinearSuperpositionScatteringTheory(AbstractLinearScatteringTheory, strict=True):
+class LinearSuperpositionScatteringTheory(AbstractWeakPhaseScatteringTheory, strict=True):
     """Compute the superposition of images of the structural ensemble batch returned by
-    the `AbstractStructuralEnsembleBatcher`.
+    the `AbstractStructuralEnsembleBatcher`. This must operate in the weak phase
+    approximation.
     """
 
     structural_ensemble_batcher: AbstractStructuralEnsembleBatcher
     potential_integrator: AbstractPotentialIntegrator
     transfer_theory: ContrastTransferTheory
     solvent: Optional[AbstractIce] = None
 
@@ -140,15 +142,15 @@
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         @partial(eqx.filter_vmap, in_axes=(0, None, None))
         def compute_image_stack(ensemble_vmap, ensemble_no_vmap, instrument_config):
             ensemble = eqx.combine(ensemble_vmap, ensemble_no_vmap)
             fourier_phase_shifts_at_exit_plane = (
-                _compute_phase_shifts_from_projected_potential(
+                _compute_phase_shifts_from_integrated_potential(
                     ensemble, self.potential_integrator, instrument_config
                 )
             )
             return fourier_phase_shifts_at_exit_plane
 
         @eqx.filter_jit
         def compute_image_superposition(
@@ -191,15 +193,15 @@
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         @partial(eqx.filter_vmap, in_axes=(0, None, None))
         def compute_image_stack(ensemble_vmap, ensemble_no_vmap, instrument_config):
             ensemble = eqx.combine(ensemble_vmap, ensemble_no_vmap)
             fourier_phase_shifts_at_exit_plane = (
-                _compute_phase_shifts_from_projected_potential(
+                _compute_phase_shifts_from_integrated_potential(
                     ensemble, self.potential_integrator, instrument_config
                 )
             )
             fourier_contrast_at_detector_plane = self.transfer_theory(
                 fourier_phase_shifts_at_exit_plane, instrument_config
             )
 
@@ -250,29 +252,27 @@
                                  would be an `AbstractAssembly` concrete class.
 - `potential_integrator`: The method for integrating the specimen potential.
 - `transfer_theory`: The contrast transfer theory.
 - `solvent`: The model for the solvent.
 """
 
 
-def _compute_phase_shifts_from_projected_potential(
+def _compute_phase_shifts_from_integrated_potential(
     structural_ensemble, potential_integrator, instrument_config
 ):
     # Get potential in the lab frame
     potential = structural_ensemble.get_potential_in_lab_frame()
     # Compute the phase shifts in the exit plane
-    fourier_projected_potential = (
+    fourier_integrated_potential = (
         potential_integrator.compute_fourier_integrated_potential(
             potential, instrument_config
         )
     )
     # Compute in-plane translation through fourier phase shifts
     translational_phase_shifts = structural_ensemble.pose.compute_shifts(
-        instrument_config.wrapped_padded_frequency_grid_in_angstroms.get()
+        instrument_config.padded_frequency_grid_in_angstroms
     )
-    # The phase shifts in the exit plane multiplies the wavelength x
-    # projected potential (here with units of inverse angstroms) x the translation
-    return (
-        instrument_config.wavelength_in_angstroms
-        * fourier_projected_potential
-        * translational_phase_shifts
+    # Compute the phase shifts in exit plane and multiply by the translation.
+    phase_shifts_in_exit_plane = compute_phase_shifts_from_integrated_potential(
+        fourier_integrated_potential, instrument_config.wavelength_in_angstroms
     )
+    return phase_shifts_in_exit_plane * translational_phase_shifts
```

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/__init__.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/base_ensemble.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/base_ensemble.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_structural_ensemble/discrete_ensemble.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_structural_ensemble/discrete_ensemble.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/base_transfer_theory.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/base_transfer_theory.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/common_functions.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/common_functions.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py` & `cryojax-0.3.0rc2/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,15 @@
         ],
         instrument_config: InstrumentConfig,
         defocus_offset: Float[Array, ""] | float = 0.0,
     ) -> Complex[
         Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
     ]:
         """Apply the CTF directly to the phase shifts in the exit plane."""
-        frequency_grid = (
-            instrument_config.wrapped_padded_frequency_grid_in_angstroms.get()
-        )
+        frequency_grid = instrument_config.padded_frequency_grid_in_angstroms
         # Compute the CTF
         ctf_array = self.envelope(frequency_grid) * self.ctf(
             frequency_grid,
             wavelength_in_angstroms=instrument_config.wavelength_in_angstroms,
             defocus_offset=defocus_offset,
         )
         # ... compute the contrast as the CTF multiplied by the exit plane
```

### Comparing `cryojax-0.3.0rc1/tests/conftest.py` & `cryojax-0.3.0rc2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pytest
 from jaxtyping import install_import_hook
 
 
 with install_import_hook("cryojax", "typeguard.typechecked"):
     import cryojax as cryojax
     import cryojax.simulator as cs
-    from cryojax.data import read_array_with_spacing_from_mrc
     from cryojax.image import operators as op, rfftn
+    from cryojax.io import read_array_with_spacing_from_mrc
 
 
 # jax.config.update("jax_numpy_dtype_promotion", "strict")
 # jax.config.update("jax_numpy_rank_promotion", "raise")
 jax.config.update("jax_enable_x64", True)
 
 
@@ -92,21 +92,21 @@
     return cs.FourierVoxelGridPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size, pad_scale=1.3
     )
 
 
 @pytest.fixture
 def filters(config):
-    return op.LowpassFilter(config.wrapped_padded_frequency_grid_in_pixels.get())
+    return op.LowpassFilter(config.padded_frequency_grid_in_pixels)
 
 
 @pytest.fixture
 def masks(config):
     return op.CircularMask(
-        config.wrapped_padded_coordinate_grid_in_angstroms.get(),
+        config.padded_coordinate_grid_in_angstroms,
         radius=20 * float(config.pixel_size),
     )
 
 
 @pytest.fixture
 def transfer_theory():
     return cs.ContrastTransferTheory(ctf=cs.ContrastTransferFunction())
@@ -136,22 +136,22 @@
 @pytest.fixture
 def solvent():
     return cs.GaussianIce(op.Constant(0.001**2))
 
 
 @pytest.fixture
 def theory(specimen, projection_method, transfer_theory, solvent):
-    return cs.LinearScatteringTheory(
+    return cs.WeakPhaseScatteringTheory(
         specimen, projection_method, transfer_theory, solvent
     )
 
 
 @pytest.fixture
 def theory_with_solvent(specimen, projection_method, transfer_theory, solvent):
-    return cs.LinearScatteringTheory(
+    return cs.WeakPhaseScatteringTheory(
         specimen, projection_method, transfer_theory, solvent
     )
 
 
 @pytest.fixture
 def noiseless_model(config, theory):
     return cs.IntensityImagingPipeline(instrument_config=config, scattering_theory=theory)
```

### Comparing `cryojax-0.3.0rc1/tests/test_agree_with_cistem.py` & `cryojax-0.3.0rc2/tests/test_agree_with_cistem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pytest
 from pycistem.core import AnglesAndShifts, CTF as cisCTF, Image  # pyright: ignore
 
 import cryojax.simulator as cs
-from cryojax.coordinates import cartesian_to_polar, make_frequencies
-from cryojax.data import read_array_with_spacing_from_mrc
+from cryojax.coordinates import cartesian_to_polar, make_frequency_grid
 from cryojax.image import irfftn, powerspectrum
+from cryojax.io import read_array_with_spacing_from_mrc
 from cryojax.simulator import ContrastTransferFunction, EulerAnglePose
 
 
 jax.config.update("jax_enable_x64", True)
 
 
 @pytest.mark.parametrize(
@@ -29,15 +29,15 @@
     ],
 )
 def test_ctf_with_cistem(defocus1, defocus2, asti_angle, kV, cs, ac, pixel_size):
     """Test CTF model against cisTEM.
 
     Modified from https://github.com/jojoelfe/contrasttransferfunction"""
     shape = (512, 512)
-    freqs = make_frequencies(shape, pixel_size)
+    freqs = make_frequency_grid(shape, pixel_size)
     k_sqr, theta = cartesian_to_polar(freqs, square=True)
     # Compute cryojax CTF
     optics = ContrastTransferFunction(
         defocus_in_angstroms=defocus1,
         astigmatism_in_angstroms=defocus2 - defocus1,
         astigmatism_angle=asti_angle,
         voltage_in_kilovolts=kV,
```

### Comparing `cryojax-0.3.0rc1/tests/test_atom_routines.py` & `cryojax-0.3.0rc2/tests/test_atom_routines.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/tests/test_detector.py` & `cryojax-0.3.0rc2/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/tests/test_ensemble.py` & `cryojax-0.3.0rc2/tests/test_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 
 def test_conformation(potential, pose, projection_method, transfer_theory, config):
     potential = tuple([potential for _ in range(3)])
     ensemble = DiscreteStructuralEnsemble(
         potential, pose, conformation=DiscreteConformationalVariable(0)
     )
-    theory = cxs.LinearScatteringTheory(ensemble, projection_method, transfer_theory)
+    theory = cxs.WeakPhaseScatteringTheory(ensemble, projection_method, transfer_theory)
     _ = theory.compute_fourier_phase_shifts_at_exit_plane(config)
 
 
 def test_conformation_vmap(potential, pose, projection_method, transfer_theory, config):
     # Build Ensemble
     state_space = tuple([potential for _ in range(3)])
     ensemble = DiscreteStructuralEnsemble(
         state_space,
         pose,
         conformation=jax.vmap(lambda value: DiscreteConformationalVariable(value))(
             jnp.asarray((0, 1, 2, 1, 0))
         ),
     )
-    theory = cxs.LinearScatteringTheory(ensemble, projection_method, transfer_theory)
+    theory = cxs.WeakPhaseScatteringTheory(ensemble, projection_method, transfer_theory)
     # Setup vmap
     is_vmap = lambda x: isinstance(x, DiscreteConformationalVariable)
     to_vmap = jtu.tree_map(is_vmap, theory, is_leaf=is_vmap)
     vmap, novmap = eqx.partition(theory, to_vmap)
 
     @partial(jax.vmap, in_axes=[0, None, None])
     def compute_conformation_stack(vmap, novmap, config):
```

### Comparing `cryojax-0.3.0rc1/tests/test_fft.py` & `cryojax-0.3.0rc2/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/tests/test_grid_search.py` & `cryojax-0.3.0rc2/tests/test_grid_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytest
 from jaxtyping import Array, install_import_hook
 
 
 with install_import_hook("cryojax", "typeguard.typechecked"):
     import cryojax.inference as cxi
-    from cryojax.coordinates import make_coordinates
+    from cryojax.coordinates import make_coordinate_grid
 
 
 class ExampleModule(eqx.Module):
     a_1: Array
     a_2: Array
     a_3: Array
     placeholder: None
@@ -70,15 +70,15 @@
     )
 
 
 @pytest.mark.parametrize("batch_size", [None, 1, 10])
 def test_run_grid_search(batch_size):
     # Compute full landscape of simple analytic "cost function"
     dim = 200
-    coords = make_coordinates((dim, dim))
+    coords = make_coordinate_grid((dim, dim))
     variance, offset = jnp.asarray(10.0), jnp.asarray((2.0, -1.0))
     landscape = jax.vmap(jax.vmap(cost_fn, in_axes=[0, None]), in_axes=[0, None])(
         coords, (variance, offset)
     )
     # Find the true minimum value and its location
     true_min_eval = landscape.min()
     true_min_idx = jnp.squeeze(jnp.argwhere(landscape == true_min_eval))
```

### Comparing `cryojax-0.3.0rc1/tests/test_helix.py` & `cryojax-0.3.0rc2/tests/test_helix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pytest
 
 import cryojax.simulator as cs
-from cryojax.data import read_array_with_spacing_from_mrc
 from cryojax.image import irfftn, normalize_image
+from cryojax.io import read_array_with_spacing_from_mrc
 
 
 def build_helix(sample_subunit_mrc_path, n_subunits_per_start) -> cs.HelicalAssembly:
     real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(
         sample_subunit_mrc_path
     )
     subunit_density = cs.FourierVoxelGridPotential.from_real_voxel_grid(
@@ -133,15 +133,15 @@
     helix = build_helix(sample_subunit_mrc_path, 2)
     specimen_39jg = cs.SingleStructureEnsemble(potential, cs.EulerAnglePose())
     superposition_theory = cs.LinearSuperpositionScatteringTheory(
         helix,
         cs.FourierSliceExtraction(),
         cs.ContrastTransferTheory(cs.IdealContrastTransferFunction()),
     )
-    theory = cs.LinearScatteringTheory(
+    theory = cs.WeakPhaseScatteringTheory(
         specimen_39jg,
         cs.FourierSliceExtraction(),
         cs.ContrastTransferTheory(cs.IdealContrastTransferFunction()),
     )
     pipeline_for_assembly = cs.ContrastImagingPipeline(
         instrument_config=config, scattering_theory=superposition_theory
     )
```

### Comparing `cryojax-0.3.0rc1/tests/test_normalize.py` & `cryojax-0.3.0rc2/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/tests/test_pose_agreement.py` & `cryojax-0.3.0rc2/tests/test_pose_agreement.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/tests/test_shape.py` & `cryojax-0.3.0rc2/tests/test_shape.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jax
 import numpy as np
 import pytest
 
 import cryojax.simulator as cs
-from cryojax.data import read_array_with_spacing_from_mrc
 from cryojax.image import crop_to_shape
+from cryojax.io import read_array_with_spacing_from_mrc
 
 
 jax.config.update("jax_enable_x64", True)
 
 
 @pytest.mark.parametrize("model", ["noisy_model"])
 def test_real_shape(model, request):
@@ -22,23 +22,18 @@
 
 @pytest.mark.parametrize("model", ["noisy_model"])
 def test_fourier_shape(model, request):
     """Make sure shapes are as expected in fourier space."""
     model = request.getfixturevalue(model)
     image = model.render(get_real=False)
     padded_image = model.render(postprocess=False, get_real=False)
-    assert (
-        image.shape
-        == model.instrument_config.wrapped_frequency_grid_in_pixels.get().shape[0:2]
-    )
+    assert image.shape == model.instrument_config.frequency_grid_in_pixels.shape[0:2]
     assert (
         padded_image.shape
-        == model.instrument_config.wrapped_padded_frequency_grid_in_pixels.get().shape[
-            0:2
-        ]
+        == model.instrument_config.padded_frequency_grid_in_pixels.shape[0:2]
     )
 
 
 @pytest.mark.parametrize("shape", [(65, 65), (65, 64), (64, 65)])
 def test_even_vs_odd_image_shape(shape, sample_mrc_path, pixel_size):
     control_shape = (64, 64)
     real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(sample_mrc_path)
@@ -46,15 +41,15 @@
         real_voxel_grid, voxel_size
     )
     assert control_shape == potential.fourier_voxel_grid.shape[0:2]
     pose = cs.EulerAnglePose()
     method = cs.FourierSliceExtraction()
     specimen = cs.SingleStructureEnsemble(potential, pose)
     transfer_theory = cs.ContrastTransferTheory(cs.ContrastTransferFunction())
-    theory = cs.LinearScatteringTheory(specimen, method, transfer_theory)
+    theory = cs.WeakPhaseScatteringTheory(specimen, method, transfer_theory)
     config_control = cs.InstrumentConfig(
         control_shape, pixel_size, voltage_in_kilovolts=300.0
     )
     config_test = cs.InstrumentConfig(shape, pixel_size, voltage_in_kilovolts=300.0)
     pipeline_control = cs.ContrastImagingPipeline(config_control, theory)
     pipeline_test = cs.ContrastImagingPipeline(config_test, theory)
```

### Comparing `cryojax-0.3.0rc1/LICENSE` & `cryojax-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryojax-0.3.0rc1/README.md` & `cryojax-0.3.0rc2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
 import cryojax.simulator as cxs
-from cryojax.data import read_array_with_spacing_from_mrc
+from cryojax.io import read_array_with_spacing_from_mrc
 
 # Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
 potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
 # ... now, instantiate the pose. Angles are given in degrees
 pose = cxs.EulerAnglePose(
@@ -69,17 +69,17 @@
     view_theta=80.0,
     view_psi=-10.0,
 )
 # ... now, build the ensemble. In this case, the ensemble is just a single structure
 structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+Here, the 3D scattering potential array is read from `filename` (see the documentation [here](https://mjo22.github.io/cryojax/examples/compute-potential/) for an example of how to generate the potential). Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and subsequently the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
 
-Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `WeakPhaseScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
 # Initialize the scattering theory. First, instantiate fourier slice extraction
 potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
 # ... next, the contrast transfer theory
@@ -87,15 +87,15 @@
     defocus_in_angstroms=9800.0,
     astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
     amplitude_contrast_ratio=0.1
 )
 transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
 # ... now for the scattering theory
-scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
+scattering_theory = cxs.WeakPhaseScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
 The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
 # Finally, build the image formation model
```

### Comparing `cryojax-0.3.0rc1/pyproject.toml` & `cryojax-0.3.0rc2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -24,18 +24,19 @@
     "jaxtyping>=0.2.23",
     "lineax",
     "mrcfile",
     "starfile",
     "pandas",
     "typing_extensions>=4.5.0",
     "tqdm",
+    "gemmi",
 ]
 
 [project.optional-dependencies]
-test = ["pytest", "pycistem", "gemmi"]
+test = ["pytest", "pycistem"]
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `cryojax-0.3.0rc1/PKG-INFO` & `cryojax-0.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cryojax
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: Cryo-EM image simulation and analysis powered by JAX
 Project-URL: repository, https://github.com/mjo22/cryojax
 Author-email: Michael O'Brien <michaelobrien@g.harvard.edu>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -515,25 +515,25 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: equinox>=0.11.0
+Requires-Dist: gemmi
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxtyping>=0.2.23
 Requires-Dist: lineax
 Requires-Dist: mrcfile
 Requires-Dist: pandas
 Requires-Dist: starfile
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: test
-Requires-Dist: gemmi; extra == 'test'
 Requires-Dist: pycistem; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 <h1 align='center'>cryoJAX</h1>
 
 ![Tests](https://github.com/mjo22/cryojax/actions/workflows/testing.yml/badge.svg)
@@ -587,15 +587,15 @@
 
 First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
 import cryojax.simulator as cxs
-from cryojax.data import read_array_with_spacing_from_mrc
+from cryojax.io import read_array_with_spacing_from_mrc
 
 # Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
 potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
 # ... now, instantiate the pose. Angles are given in degrees
 pose = cxs.EulerAnglePose(
@@ -605,17 +605,17 @@
     view_theta=80.0,
     view_psi=-10.0,
 )
 # ... now, build the ensemble. In this case, the ensemble is just a single structure
 structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+Here, the 3D scattering potential array is read from `filename` (see the documentation [here](https://mjo22.github.io/cryojax/examples/compute-potential/) for an example of how to generate the potential). Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and subsequently the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
 
-Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `WeakPhaseScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
 # Initialize the scattering theory. First, instantiate fourier slice extraction
 potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
 # ... next, the contrast transfer theory
@@ -623,15 +623,15 @@
     defocus_in_angstroms=9800.0,
     astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
     amplitude_contrast_ratio=0.1
 )
 transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
 # ... now for the scattering theory
-scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
+scattering_theory = cxs.WeakPhaseScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
 The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
 # Finally, build the image formation model
```

