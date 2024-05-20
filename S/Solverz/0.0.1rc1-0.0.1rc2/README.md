# Comparing `tmp/solverz-0.0.1rc1.tar.gz` & `tmp/solverz-0.0.1rc2.tar.gz`

## Comparing `solverz-0.0.1rc1.tar` & `solverz-0.0.1rc2.tar`

### file list

```diff
@@ -1,125 +1,127 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/.gitattributes
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/requirements.txt
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/res.png
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/.github/workflows/debug github action.yml
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/.github/workflows/doc-deploy.yml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/make_module.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/make_pyfunc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/matlab_printer.py
--rw-r--r--   0        0        0    36205 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/py_printer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/test/__init__.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/code_printer/test/test_py_printer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/__init__.py
--rw-r--r--   0        0        0    17894 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/eqn.py
--rw-r--r--   0        0        0    26475 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/equations.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/param.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/trigger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/test/__init__.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/test/test_DAE.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/test/test_Param.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/test/test_eqn.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/equation/test/test_jac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/model/__init__.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/model/basic.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/Array.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/custom_function.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/num_eqn.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/numjac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/test/__init__.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/test/test_Array.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/test/test_custom_func.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/num_api/test/test_numjac.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/__init__.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/fdesolver.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/laesolver.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/option.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/parser.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/solution.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/stats.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/__init__.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/beuler.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/daeic.py
--rw-r--r--   0        0        0    21751 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/rodas.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/trapezoidal.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/daesolver/utilities.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/nlaesolver/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/nlaesolver/cnr.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/nlaesolver/lm.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/nlaesolver/nr.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/nlaesolver/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/odesolver/__init__.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/odesolver/ode45.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/odesolver/rock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/test/__init__.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/solvers/test/test_rodas_event.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/__init__.py
--rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/functions.py
--rw-r--r--   0        0        0    16690 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/matrix_calculus.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/symbols.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/test/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/test/test_finite_difference.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/test/test_matrix_calculus.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/test/test_num_alg.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/sym_algebra/test/test_symbols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/__init__.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/address.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/io.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/profile.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/type_checker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/test/__init__.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/utilities/test/test_address.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/variable/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/variable/ssymbol.py
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/variable/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/variable/test/__init__.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/Solverz/variable/test/test_variable.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/Makefile
--rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/make.bat
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/requirements.txt
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/ext/convert-svg-to-pdf.py
--rw-r--r--   0        0        0    17382 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/ext/docscrape.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/ext/docscrape_sphinx.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/ext/numpydoc.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/advanced.md
--rw-r--r--   0        0        0     7779 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/contributing.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/gethelp.md
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/gettingstart.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/index.rst
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/install.md
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/intro.md
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/_static/custom.css
--rw-r--r--   0        0        0    68647 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/_static/sympylogo.png
--rw-r--r--   0        0        0   167361 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/_static/sympylogo_big.png
--rw-r--r--   0        0        0   191208 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/pics/Hierarchy_of_equations.png
--rw-r--r--   0        0        0    53578 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/pics/difference_stencil.png
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/pics/res.png
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/docs/src/reference/index.rst
--rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/4node3pipe.xlsx
--rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/4node3pipe_bench.xlsx
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/4node3pipe_change_sign.xlsx
--rw-r--r--   0        0        0    15910 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/4node3pipe_change_sign_bench.xlsx
--rw-r--r--   0        0        0    21963 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/dae_test.xlsx
--rw-r--r--   0        0        0    30787 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/dynamic_gas_flow_single_pipe.xlsx
--rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/ode_test.xlsx
--rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/test_burger.xlsx
--rw-r--r--   0        0        0  1412117 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/test_m3b9.xlsx
--rw-r--r--   0        0        0    41225 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/test_ode45.xlsx
--rw-r--r--   0        0        0  2246743 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/instances/test_sirk.xlsx
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_0.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_dae.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_dhspf.py
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_dhspf_change_sign.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_dyn_gas_flow_single_pipe.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_gasflow.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/tests/test_m3b9.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/.gitignore
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 solverz-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.gitattributes
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/requirements.txt
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/res.png
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.github/workflows/debug github action.yml
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.github/workflows/doc-deploy.yml
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/make_module.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/make_pyfunc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/matlab_printer.py
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/py_printer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/test/__init__.py
+-rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/code_printer/test/test_py_printer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/__init__.py
+-rw-r--r--   0        0        0    17407 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/eqn.py
+-rw-r--r--   0        0        0    25834 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/equations.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/param.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/trigger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/test/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/test/test_DAE.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/test/test_Param.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/test/test_eqn.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/equation/test/test_jac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/model/__init__.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/model/basic.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/Array.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/__init__.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/custom_function.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/num_eqn.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/numjac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/test/__init__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/test/test_Array.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/test/test_custom_func.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/num_api/test/test_numjac.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/fdesolver.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/laesolver.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/option.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/parser.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/solution.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/stats.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/__init__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/beuler.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/daeic.py
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/rodas.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/trapezoidal.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/daesolver/utilities.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/nlaesolver/__init__.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/nlaesolver/cnr.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/nlaesolver/lm.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/nlaesolver/nr.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/nlaesolver/utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/odesolver/__init__.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/odesolver/ode45.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/odesolver/rock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/test/__init__.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/solvers/test/test_rodas_event.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/__init__.py
+-rw-r--r--   0        0        0    16332 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/functions.py
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/matrix_calculus.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/symbols.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/test/__init__.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/test/test_finite_difference.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/test/test_matrix_calculus.py
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/test/test_num_alg.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/sym_algebra/test/test_symbols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/address.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/io.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/profile.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/type_checker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/test/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/utilities/test/test_address.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/variable/__init__.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/variable/ssymbol.py
+-rw-r--r--   0        0        0     9663 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/variable/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/variable/test/__init__.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/Solverz/variable/test/test_variable.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/Makefile
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/make.bat
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/requirements.txt
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/ext/convert-svg-to-pdf.py
+-rw-r--r--   0        0        0    16828 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/ext/docscrape.py
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/ext/docscrape_sphinx.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/ext/numpydoc.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/advanced.md
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/conf.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/contributing.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/gethelp.md
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/gettingstart.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/index.rst
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/install.md
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/intro.md
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/_static/custom.css
+-rw-r--r--   0        0        0    68647 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/_static/sympylogo.png
+-rw-r--r--   0        0        0   167361 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/_static/sympylogo_big.png
+-rw-r--r--   0        0        0   191208 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/pics/Hierarchy_of_equations.png
+-rw-r--r--   0        0        0    53578 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/pics/difference_stencil.png
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/pics/res.png
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/docs/src/reference/index.rst
+-rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/4node3pipe.xlsx
+-rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/4node3pipe_bench.xlsx
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/4node3pipe_change_sign.xlsx
+-rw-r--r--   0        0        0    15910 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/4node3pipe_change_sign_bench.xlsx
+-rw-r--r--   0        0        0    21963 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/dae_test.xlsx
+-rw-r--r--   0        0        0    30787 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/dynamic_gas_flow_single_pipe.xlsx
+-rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/ode_test.xlsx
+-rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/test_burger.xlsx
+-rw-r--r--   0        0        0  1412117 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/test_m3b9.xlsx
+-rw-r--r--   0        0        0    41225 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/test_ode45.xlsx
+-rw-r--r--   0        0        0  2246743 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/instances/test_sirk.xlsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_0.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_dae.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_dhspf.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_dhspf_change_sign.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_dyn_gas_flow_single_pipe.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_gasflow.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/tests/test_m3b9.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 solverz-0.0.1rc2/PKG-INFO
```

### Comparing `solverz-0.0.1rc1/res.png` & `solverz-0.0.1rc2/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/.github/workflows/doc-deploy.yml` & `solverz-0.0.1rc2/.github/workflows/doc-deploy.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/.github/workflows/python-package.yml` & `solverz-0.0.1rc2/.github/workflows/python-package.yml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# This workflow will install Python dependencies (if not cached), run tests and lint with a variety of Python versions
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
-
-name: Python package
-
-on: [push]
-
-jobs:
-  build:
-
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        os: [ windows-latest ]
-
-    steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-        cache: 'pip' # caching pip dependencies
-    - run: |
-        pip install -r requirements.txt
-        cd docs/
-        pip install -r requirements.txt
-        cd ..
-    - run: | # run both independent pytest and doctest
-        pytest -vv
+# This workflow will install Python dependencies (if not cached), run tests and lint with a variety of Python versions
+# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
+
+name: Python package
+
+on: [push]
+
+jobs:
+  build:
+
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ windows-latest ]
+
+    steps:
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.11'
+        cache: 'pip' # caching pip dependencies
+    - run: |
+        pip install -r requirements.txt
+        cd docs/
+        pip install -r requirements.txt
+        cd ..
+    - run: | # run both independent pytest and doctest
+        pytest -vv
```

### Comparing `solverz-0.0.1rc1/Solverz/__init__.py` & `solverz-0.0.1rc2/Solverz/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from Solverz.equation.eqn import Eqn, Ode, HyperbolicPde
-from Solverz.equation.equations import AE, FDAE, DAE
-from Solverz.equation.param import Param, IdxParam, TimeSeriesParam
-from Solverz.sym_algebra.symbols import idx, Para, iVar, iAliasVar
-from Solverz.sym_algebra.functions import Sign, Abs, transpose, exp, Diag, Mat_Mul, sin, cos, Min, AntiWindUp, Saturation
-from Solverz.num_api.custom_function import minmod_flag, minmod
-from Solverz.variable.variables import Vars, TimeVars, as_Vars
-from Solverz.solvers import *
-from Solverz.code_printer.make_pyfunc import made_numerical
-from Solverz.code_printer.py_printer import render_modules
-from Solverz.code_printer.make_module import module_printer
-from Solverz.utilities.io import save, load, save_result
-from Solverz.utilities.profile import count_time
-from Solverz.variable.ssymbol import Var, AliasVar
-from Solverz.model.basic import Model
+from Solverz.equation.eqn import Eqn, Ode, HyperbolicPde
+from Solverz.equation.equations import AE, FDAE, DAE
+from Solverz.equation.param import Param, IdxParam, TimeSeriesParam
+from Solverz.sym_algebra.symbols import idx, Para, iVar, iAliasVar
+from Solverz.sym_algebra.functions import Sign, Abs, transpose, exp, Diag, Mat_Mul, sin, cos, Min, AntiWindUp, Saturation
+from Solverz.num_api.custom_function import minmod_flag, minmod
+from Solverz.variable.variables import Vars, TimeVars, as_Vars
+from Solverz.solvers import *
+from Solverz.code_printer.make_pyfunc import made_numerical
+from Solverz.code_printer.py_printer import render_modules
+from Solverz.code_printer.make_module import module_printer
+from Solverz.utilities.io import save, load, save_result
+from Solverz.utilities.profile import count_time
+from Solverz.variable.ssymbol import Var, AliasVar
+from Solverz.model.basic import Model
```

### Comparing `solverz-0.0.1rc1/Solverz/code_printer/test/test_py_printer.py` & `solverz-0.0.1rc2/Solverz/code_printer/test/test_py_printer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-import inspect
-import os
-import shutil
-import sys
-
-import numpy as np
-from sympy import symbols, pycode, Integer
-
-from Solverz import as_Vars, Eqn, AE, sin, made_numerical
-from Solverz.code_printer.make_module import module_printer
-from Solverz.code_printer.py_printer import _parse_jac_eqn_address, _parse_jac_var_address, _parse_jac_data, \
-    print_J_block, _print_var_parser
-from Solverz.sym_algebra.symbols import idx, iVar, Para
-
-
-def test_address_parser():
-    eqn_address = slice(0, 1)
-    assert pycode(_parse_jac_eqn_address(eqn_address, 1, False)) == '0'
-    assert _parse_jac_eqn_address(eqn_address, 2, False).__repr__() == 'slice(0, 1, None)'
-    assert pycode(_parse_jac_eqn_address(eqn_address, 1, True)) == '[0]'
-    assert pycode(_parse_jac_eqn_address(eqn_address, 2, True)) == 'arange(0, 1)[value_coo.row]'
-
-    eqn_address = slice(0, 5)
-    assert pycode(_parse_jac_eqn_address(eqn_address, 1, False)) == 'arange(0, 5)'
-    assert pycode(_parse_jac_eqn_address(eqn_address, 1, True)) == 'arange(0, 5)'
-    assert _parse_jac_eqn_address(eqn_address, 2, False).__repr__() == 'slice(0, 5, None)'
-    assert _parse_jac_eqn_address(eqn_address, 2, True).__repr__() == 'arange(0, 5)[value_coo.row]'
-
-    v_address = slice(0, 1)
-    assert pycode(_parse_jac_var_address(v_address, 1, None, False)) == 'arange(0, 1)'
-    assert pycode(_parse_jac_var_address(v_address, 1, None, True)) == 'arange(0, 1)'
-    assert _parse_jac_var_address(v_address, 2, None, False).__repr__() == 'slice(0, 1, None)'
-    assert pycode(_parse_jac_var_address(v_address, 2, None, True)) == 'arange(0, 1)[value_coo.col]'
-
-    v_address = slice(0, 3)
-    # _parse_jac_var_address(v_address, 2, v_idx, True)
-    assert _parse_jac_var_address(v_address, 2, None, False).__repr__() == 'slice(0, 3, None)'
-    assert _parse_jac_var_address(v_address, 2, None, True).__repr__() == 'arange(0, 3)[value_coo.col]'
-    assert pycode(_parse_jac_var_address(v_address, 1, None, True)) == 'arange(0, 3)'
-    assert pycode(_parse_jac_var_address(v_address, 1, None, False)) == 'arange(0, 3)'
-    assert pycode(_parse_jac_var_address(v_address, 0, 2, True, 3)) == '3*[2]'
-    assert pycode(_parse_jac_var_address(v_address, 1, 2, True, 3)) == '3*[2]'
-
-    M = idx('M')
-    assert _parse_jac_var_address(v_address, 2, M, True).__repr__() == 'arange(0, 3)[M[value_coo.col]]'
-    assert pycode(_parse_jac_var_address(v_address, 2, M, False)) == 'arange(0, 3)[M]'
-    assert _parse_jac_var_address(v_address, 1, M, True).__repr__() == 'arange(0, 3)[M]'
-    assert pycode(_parse_jac_var_address(v_address, 1, M, False)) == 'arange(0, 3)[M]'
-
-    v_idx = [0, 1, 2]
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == 'arange(0, 3)'
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == 'arange(0, 3)'
-    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, True)) == 'arange(0, 3)[value_coo.col]'
-    assert _parse_jac_var_address(v_address, 2, v_idx, False).__repr__() == 'slice(0, 3, None)'
-
-    v_address = slice(0, 10)
-    v_idx = [0, 2, 4, 6]
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == '[0, 2, 4, 6]'
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == '[0, 2, 4, 6]'
-    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, True)) == 'array([0,2,4,6])[value_coo.col]'
-    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, False)) == '[0, 2, 4, 6]'
-
-    v_idx = 2
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == '[2]'
-    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == '2'
-    assert _parse_jac_var_address(v_address, 2, v_idx, True).__repr__() == 'array([2])[value_coo.col]'
-    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, False)) == '2'
-
-    x, y = symbols('x, y')
-    assert pycode(_parse_jac_data(5, 1, x * y)) == 'x*y'
-    assert pycode(_parse_jac_data(5, 0, x * y)) == '5*((x*y).tolist())'
-    assert pycode(_parse_jac_data(5, 0, 3, rhs_v_type='Number')) == '5*[3]'
-    assert pycode(_parse_jac_data(5, 2, 3)) == 'value_coo.data'
-
-
-def test_var_parser():
-    assert pycode(_print_var_parser('x', '0', slice(0, 1))) == 'x_tag_0 = y_0[0:1]'
-    assert pycode(_print_var_parser('x', '0', slice(3, 6))) == 'x_tag_0 = y_0[3:6]'
-
-
-# def test_F_printer():
-#     F = _print_F_assignment(slice(20, 21), iVar('x'))
-#     assert pycode(F) == '_F_[20:21] = x'
-#     F = _print_F_assignment(slice(20, 23), iVar('x'))
-#     assert pycode(F) == '_F_[20:23] = x'
-
-
-def test_J_block_printer():
-    # dense
-    Jb = print_J_block(slice(0, 3),
-                       slice(3, 6),
-                       0,
-                       None,
-                       iVar('omega_b'),
-                       False)
-    assert pycode(Jb) == '[J_[arange(0, 3),arange(3, 6)] += omega_b]'
-    Jb = print_J_block(slice(3, 6),
-                       slice(12, 21),
-                       1,
-                       idx('g'),
-                       -iVar('Ixg') / iVar('Tj'),
-                       False)
-    assert pycode(Jb) == '[J_[arange(3, 6),arange(12, 21)[g]] += -Ixg/Tj]'
-    Jb = print_J_block(slice(12, 15),
-                       slice(6, 9),
-                       0,
-                       None,
-                       1,
-                       False)
-    assert pycode(Jb) == '[J_[arange(12, 15),arange(6, 9)] += 1]'
-    Jb = print_J_block(slice(18, 24),
-                       slice(12, 21),
-                       2,
-                       None,
-                       iVar('G')[idx('ng'), :],
-                       False)
-    assert pycode(Jb) == '[J_[18:24,12:21] += G[ng,:]]'
-
-    Jb = print_J_block(slice(30, 31),
-                       slice(0, 10),
-                       2,
-                       None,
-                       Para('G', dim=2),
-                       False)
-    assert pycode(Jb) == '[J_[30:31,0:10] += G]'
-
-    # sparse
-    Jb = print_J_block(slice(39, 47),
-                       slice(15, 26),
-                       0,
-                       [0, 1, 2, 3, 4, 5, 9, 10],
-                       Integer(1),
-                       True,
-                       rhs_v_dtpe='Number')
-    assert pycode(
-        Jb) == '[row.extend(arange(39, 47)), col.extend([15, 16, 17, 18, 19, 20, 24, 25]), data.extend(8*[1])]'
-
-    Jb = print_J_block(slice(248, 259),
-                       slice(269, 280),
-                       0,
-                       None,
-                       Para('dt') * Para('va') ** 2 / Para('S'),
-                       True)
-    assert pycode(
-        Jb) == '[row.extend(arange(248, 259)), col.extend(arange(269, 280)), data.extend(11*((dt*va**2/S).tolist()))]'
-
-    Jb = print_J_block(slice(281, 292),
-                       slice(281, 292),
-                       1,
-                       None,
-                       Para('dx') + iVar('p'),
-                       True)
-    assert pycode(Jb) == '[row.extend(arange(281, 292)), col.extend(arange(281, 292)), data.extend(dx + p)]'
-
-    Jb = print_J_block(slice(0, 3),
-                       slice(3, 6),
-                       2,
-                       None,
-                       iVar('omega_b'),
-                       True)
-    assert pycode(
-        Jb) == '[value_coo = coo_array(omega_b), row.extend(arange(0, 3)[value_coo.row]), col.extend(arange(3, 6)[value_coo.col]), data.extend(value_coo.data)]'
-
-    Jb = print_J_block(slice(3, 6),
-                       slice(12, 21),
-                       2,
-                       idx('g'),
-                       Para('G'),
-                       True)
-    assert pycode(
-        Jb) == '[value_coo = coo_array(G), row.extend(arange(3, 6)[value_coo.row]), col.extend(arange(12, 21)[g[value_coo.col]]), data.extend(value_coo.data)]'
-
-    Jb = print_J_block(slice(39, 47),
-                       slice(15, 26),
-                       2,
-                       [0, 1, 2, 3, 4, 5, 9, 10],
-                       Para('G'),
-                       True)
-    assert pycode(
-        Jb) == '[value_coo = coo_array(G), row.extend(arange(39, 47)[value_coo.row]), col.extend(array([15,16,17,18,19,20,24,25])[value_coo.col]), data.extend(value_coo.data)]'
-
-    Jb = print_J_block(slice(39, 47),
-                       slice(15, 26),
-                       2,
-                       slice(0, 5),
-                       Para('G'),
-                       True)
-    assert pycode(
-        Jb) == '[value_coo = coo_array(G), row.extend(arange(39, 47)[value_coo.row]), col.extend(arange(15, 20)[value_coo.col]), data.extend(value_coo.data)]'
-
-
-def test_py_printer():
-    x = iVar('x', [1, 1])
-    f1 = Eqn('f1', 2 * x[0] + x[1])
-    f2 = Eqn('f2', x[0] ** 2 + sin(x[1]))
-
-    F = AE([f1, f2])
-    y = as_Vars([x])
-
-    current_file_path = os.path.abspath(__file__)
-    current_folder = os.path.dirname(current_file_path)
-
-    test_folder_path = current_folder + '\\Solverz_testaabbccddeeffgghh'
-
-    pyprinter = module_printer(F,
-                               y,
-                               'test_eqn1',
-                               directory=test_folder_path + '\\a_test_direc',
-                               jit=True)
-    pyprinter.render()
-
-    pyprinter1 = module_printer(F,
-                                y,
-                                'test_eqn2',
-                                directory=test_folder_path + '\\a_test_direc',
-                                jit=False)
-    pyprinter1.render()
-
-    sys.path.extend([test_folder_path + '\\a_test_direc'])
-
-    from test_eqn1 import mdl, y
-    from test_eqn1.num_func import inner_F, inner_F0, inner_F1, inner_J
-
-    F0 = mdl.F(y, mdl.p)
-    J0 = mdl.J(y, mdl.p)
-    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
-    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
-
-    assert inspect.getsource(
-        inner_F) == '@njit(cache=True)\ndef inner_F(_F_, x):\n    _F_[0:1] = inner_F0(x)\n    _F_[1:2] = inner_F1(x)\n    return _F_\n'
-    assert inspect.getsource(inner_F0.func_code) == '@njit(cache=True)\ndef inner_F0(x):\n    return 2*x[0] + x[1]\n'
-    assert inspect.getsource(
-        inner_F1.func_code) == '@njit(cache=True)\ndef inner_F1(x):\n    return x[0]**2 + sin(x[1])\n'
-    assert inspect.getsource(
-        inner_J) == '@njit(cache=True)\ndef inner_J(_data_, x):\n    _data_[2:3] = inner_J0(x)\n    _data_[3:4] = inner_J1(x)\n    return _data_\n'
-
-    from test_eqn2 import mdl, y
-    from test_eqn2.num_func import inner_F, inner_F0, inner_F1, inner_J
-
-    F0 = mdl.F(y, mdl.p)
-    J0 = mdl.J(y, mdl.p)
-    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
-    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
-
-    assert inspect.getsource(
-        inner_F) == 'def inner_F(_F_, x):\n    _F_[0:1] = inner_F0(x)\n    _F_[1:2] = inner_F1(x)\n    return _F_\n'
-    assert inspect.getsource(inner_F0) == 'def inner_F0(x):\n    return 2*x[0] + x[1]\n'
-    assert inspect.getsource(inner_F1) == 'def inner_F1(x):\n    return x[0]**2 + sin(x[1])\n'
-    assert inspect.getsource(
-        inner_J) == 'def inner_J(_data_, x):\n    _data_[2:3] = inner_J0(x)\n    _data_[3:4] = inner_J1(x)\n    return _data_\n'
-
-    shutil.rmtree(test_folder_path)
-
-
-def test_made_numerical():
-    x = iVar('x', [1, 1])
-    f1 = Eqn('f1', 2 * x[0] + x[1])
-    f2 = Eqn('f2', x[0] ** 2 + sin(x[1]))
-
-    F = AE([f1, f2])
-    y = as_Vars([x])
-    nF, code = made_numerical(F, y, sparse=True, output_code=True)
-    F0 = nF.F(y, nF.p)
-    J0 = nF.J(y, nF.p)
-    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
-    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
+import inspect
+import os
+import shutil
+import sys
+
+import numpy as np
+from sympy import symbols, pycode, Integer
+
+from Solverz import as_Vars, Eqn, AE, sin, made_numerical
+from Solverz.code_printer.make_module import module_printer
+from Solverz.code_printer.py_printer import _parse_jac_eqn_address, _parse_jac_var_address, _parse_jac_data, \
+    print_J_block, _print_var_parser
+from Solverz.sym_algebra.symbols import idx, iVar, Para
+
+
+def test_address_parser():
+    eqn_address = slice(0, 1)
+    assert pycode(_parse_jac_eqn_address(eqn_address, 1, False)) == '0'
+    assert _parse_jac_eqn_address(eqn_address, 2, False).__repr__() == 'slice(0, 1, None)'
+    assert pycode(_parse_jac_eqn_address(eqn_address, 1, True)) == '[0]'
+    assert pycode(_parse_jac_eqn_address(eqn_address, 2, True)) == 'arange(0, 1)[value_coo.row]'
+
+    eqn_address = slice(0, 5)
+    assert pycode(_parse_jac_eqn_address(eqn_address, 1, False)) == 'arange(0, 5)'
+    assert pycode(_parse_jac_eqn_address(eqn_address, 1, True)) == 'arange(0, 5)'
+    assert _parse_jac_eqn_address(eqn_address, 2, False).__repr__() == 'slice(0, 5, None)'
+    assert _parse_jac_eqn_address(eqn_address, 2, True).__repr__() == 'arange(0, 5)[value_coo.row]'
+
+    v_address = slice(0, 1)
+    assert pycode(_parse_jac_var_address(v_address, 1, None, False)) == 'arange(0, 1)'
+    assert pycode(_parse_jac_var_address(v_address, 1, None, True)) == 'arange(0, 1)'
+    assert _parse_jac_var_address(v_address, 2, None, False).__repr__() == 'slice(0, 1, None)'
+    assert pycode(_parse_jac_var_address(v_address, 2, None, True)) == 'arange(0, 1)[value_coo.col]'
+
+    v_address = slice(0, 3)
+    # _parse_jac_var_address(v_address, 2, v_idx, True)
+    assert _parse_jac_var_address(v_address, 2, None, False).__repr__() == 'slice(0, 3, None)'
+    assert _parse_jac_var_address(v_address, 2, None, True).__repr__() == 'arange(0, 3)[value_coo.col]'
+    assert pycode(_parse_jac_var_address(v_address, 1, None, True)) == 'arange(0, 3)'
+    assert pycode(_parse_jac_var_address(v_address, 1, None, False)) == 'arange(0, 3)'
+    assert pycode(_parse_jac_var_address(v_address, 0, 2, True, 3)) == '3*[2]'
+    assert pycode(_parse_jac_var_address(v_address, 1, 2, True, 3)) == '3*[2]'
+
+    M = idx('M')
+    assert _parse_jac_var_address(v_address, 2, M, True).__repr__() == 'arange(0, 3)[M[value_coo.col]]'
+    assert pycode(_parse_jac_var_address(v_address, 2, M, False)) == 'arange(0, 3)[M]'
+    assert _parse_jac_var_address(v_address, 1, M, True).__repr__() == 'arange(0, 3)[M]'
+    assert pycode(_parse_jac_var_address(v_address, 1, M, False)) == 'arange(0, 3)[M]'
+
+    v_idx = [0, 1, 2]
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == 'arange(0, 3)'
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == 'arange(0, 3)'
+    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, True)) == 'arange(0, 3)[value_coo.col]'
+    assert _parse_jac_var_address(v_address, 2, v_idx, False).__repr__() == 'slice(0, 3, None)'
+
+    v_address = slice(0, 10)
+    v_idx = [0, 2, 4, 6]
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == '[0, 2, 4, 6]'
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == '[0, 2, 4, 6]'
+    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, True)) == 'array([0,2,4,6])[value_coo.col]'
+    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, False)) == '[0, 2, 4, 6]'
+
+    v_idx = 2
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, True)) == '[2]'
+    assert pycode(_parse_jac_var_address(v_address, 1, v_idx, False)) == '2'
+    assert _parse_jac_var_address(v_address, 2, v_idx, True).__repr__() == 'array([2])[value_coo.col]'
+    assert pycode(_parse_jac_var_address(v_address, 2, v_idx, False)) == '2'
+
+    x, y = symbols('x, y')
+    assert pycode(_parse_jac_data(5, 1, x * y)) == 'x*y'
+    assert pycode(_parse_jac_data(5, 0, x * y)) == '5*((x*y).tolist())'
+    assert pycode(_parse_jac_data(5, 0, 3, rhs_v_type='Number')) == '5*[3]'
+    assert pycode(_parse_jac_data(5, 2, 3)) == 'value_coo.data'
+
+
+def test_var_parser():
+    assert pycode(_print_var_parser('x', '0', slice(0, 1))) == 'x_tag_0 = y_0[0:1]'
+    assert pycode(_print_var_parser('x', '0', slice(3, 6))) == 'x_tag_0 = y_0[3:6]'
+
+
+# def test_F_printer():
+#     F = _print_F_assignment(slice(20, 21), iVar('x'))
+#     assert pycode(F) == '_F_[20:21] = x'
+#     F = _print_F_assignment(slice(20, 23), iVar('x'))
+#     assert pycode(F) == '_F_[20:23] = x'
+
+
+def test_J_block_printer():
+    # dense
+    Jb = print_J_block(slice(0, 3),
+                       slice(3, 6),
+                       0,
+                       None,
+                       iVar('omega_b'),
+                       False)
+    assert pycode(Jb) == '[J_[arange(0, 3),arange(3, 6)] += omega_b]'
+    Jb = print_J_block(slice(3, 6),
+                       slice(12, 21),
+                       1,
+                       idx('g'),
+                       -iVar('Ixg') / iVar('Tj'),
+                       False)
+    assert pycode(Jb) == '[J_[arange(3, 6),arange(12, 21)[g]] += -Ixg/Tj]'
+    Jb = print_J_block(slice(12, 15),
+                       slice(6, 9),
+                       0,
+                       None,
+                       1,
+                       False)
+    assert pycode(Jb) == '[J_[arange(12, 15),arange(6, 9)] += 1]'
+    Jb = print_J_block(slice(18, 24),
+                       slice(12, 21),
+                       2,
+                       None,
+                       iVar('G')[idx('ng'), :],
+                       False)
+    assert pycode(Jb) == '[J_[18:24,12:21] += G[ng,:]]'
+
+    Jb = print_J_block(slice(30, 31),
+                       slice(0, 10),
+                       2,
+                       None,
+                       Para('G', dim=2),
+                       False)
+    assert pycode(Jb) == '[J_[30:31,0:10] += G]'
+
+    # sparse
+    Jb = print_J_block(slice(39, 47),
+                       slice(15, 26),
+                       0,
+                       [0, 1, 2, 3, 4, 5, 9, 10],
+                       Integer(1),
+                       True,
+                       rhs_v_dtpe='Number')
+    assert pycode(
+        Jb) == '[row.extend(arange(39, 47)), col.extend([15, 16, 17, 18, 19, 20, 24, 25]), data.extend(8*[1])]'
+
+    Jb = print_J_block(slice(248, 259),
+                       slice(269, 280),
+                       0,
+                       None,
+                       Para('dt') * Para('va') ** 2 / Para('S'),
+                       True)
+    assert pycode(
+        Jb) == '[row.extend(arange(248, 259)), col.extend(arange(269, 280)), data.extend(11*((dt*va**2/S).tolist()))]'
+
+    Jb = print_J_block(slice(281, 292),
+                       slice(281, 292),
+                       1,
+                       None,
+                       Para('dx') + iVar('p'),
+                       True)
+    assert pycode(Jb) == '[row.extend(arange(281, 292)), col.extend(arange(281, 292)), data.extend(dx + p)]'
+
+    Jb = print_J_block(slice(0, 3),
+                       slice(3, 6),
+                       2,
+                       None,
+                       iVar('omega_b'),
+                       True)
+    assert pycode(
+        Jb) == '[value_coo = coo_array(omega_b), row.extend(arange(0, 3)[value_coo.row]), col.extend(arange(3, 6)[value_coo.col]), data.extend(value_coo.data)]'
+
+    Jb = print_J_block(slice(3, 6),
+                       slice(12, 21),
+                       2,
+                       idx('g'),
+                       Para('G'),
+                       True)
+    assert pycode(
+        Jb) == '[value_coo = coo_array(G), row.extend(arange(3, 6)[value_coo.row]), col.extend(arange(12, 21)[g[value_coo.col]]), data.extend(value_coo.data)]'
+
+    Jb = print_J_block(slice(39, 47),
+                       slice(15, 26),
+                       2,
+                       [0, 1, 2, 3, 4, 5, 9, 10],
+                       Para('G'),
+                       True)
+    assert pycode(
+        Jb) == '[value_coo = coo_array(G), row.extend(arange(39, 47)[value_coo.row]), col.extend(array([15,16,17,18,19,20,24,25])[value_coo.col]), data.extend(value_coo.data)]'
+
+    Jb = print_J_block(slice(39, 47),
+                       slice(15, 26),
+                       2,
+                       slice(0, 5),
+                       Para('G'),
+                       True)
+    assert pycode(
+        Jb) == '[value_coo = coo_array(G), row.extend(arange(39, 47)[value_coo.row]), col.extend(arange(15, 20)[value_coo.col]), data.extend(value_coo.data)]'
+
+
+def test_py_printer():
+    x = iVar('x', [1, 1])
+    f1 = Eqn('f1', 2 * x[0] + x[1])
+    f2 = Eqn('f2', x[0] ** 2 + sin(x[1]))
+
+    F = AE([f1, f2])
+    y = as_Vars([x])
+
+    current_file_path = os.path.abspath(__file__)
+    current_folder = os.path.dirname(current_file_path)
+
+    test_folder_path = current_folder + '\\Solverz_testaabbccddeeffgghh'
+
+    pyprinter = module_printer(F,
+                               y,
+                               'test_eqn1',
+                               directory=test_folder_path + '\\a_test_direc',
+                               jit=True)
+    pyprinter.render()
+
+    pyprinter1 = module_printer(F,
+                                y,
+                                'test_eqn2',
+                                directory=test_folder_path + '\\a_test_direc',
+                                jit=False)
+    pyprinter1.render()
+
+    sys.path.extend([test_folder_path + '\\a_test_direc'])
+
+    from test_eqn1 import mdl, y
+    from test_eqn1.num_func import inner_F, inner_F0, inner_F1, inner_J
+
+    F0 = mdl.F(y, mdl.p)
+    J0 = mdl.J(y, mdl.p)
+    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
+    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
+
+    assert inspect.getsource(
+        inner_F) == '@njit(cache=True)\ndef inner_F(_F_, x):\n    _F_[0:1] = inner_F0(x)\n    _F_[1:2] = inner_F1(x)\n    return _F_\n'
+    assert inspect.getsource(inner_F0.func_code) == '@njit(cache=True)\ndef inner_F0(x):\n    return 2*x[0] + x[1]\n'
+    assert inspect.getsource(
+        inner_F1.func_code) == '@njit(cache=True)\ndef inner_F1(x):\n    return x[0]**2 + sin(x[1])\n'
+    assert inspect.getsource(
+        inner_J) == '@njit(cache=True)\ndef inner_J(_data_, x):\n    _data_[2:3] = inner_J0(x)\n    _data_[3:4] = inner_J1(x)\n    return _data_\n'
+
+    from test_eqn2 import mdl, y
+    from test_eqn2.num_func import inner_F, inner_F0, inner_F1, inner_J
+
+    F0 = mdl.F(y, mdl.p)
+    J0 = mdl.J(y, mdl.p)
+    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
+    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
+
+    assert inspect.getsource(
+        inner_F) == 'def inner_F(_F_, x):\n    _F_[0:1] = inner_F0(x)\n    _F_[1:2] = inner_F1(x)\n    return _F_\n'
+    assert inspect.getsource(inner_F0) == 'def inner_F0(x):\n    return 2*x[0] + x[1]\n'
+    assert inspect.getsource(inner_F1) == 'def inner_F1(x):\n    return x[0]**2 + sin(x[1])\n'
+    assert inspect.getsource(
+        inner_J) == 'def inner_J(_data_, x):\n    _data_[2:3] = inner_J0(x)\n    _data_[3:4] = inner_J1(x)\n    return _data_\n'
+
+    shutil.rmtree(test_folder_path)
+
+
+def test_made_numerical():
+    x = iVar('x', [1, 1])
+    f1 = Eqn('f1', 2 * x[0] + x[1])
+    f2 = Eqn('f2', x[0] ** 2 + sin(x[1]))
+
+    F = AE([f1, f2])
+    y = as_Vars([x])
+    nF, code = made_numerical(F, y, sparse=True, output_code=True)
+    F0 = nF.F(y, nF.p)
+    J0 = nF.J(y, nF.p)
+    np.testing.assert_allclose(F0, np.array([2 * 1 + 1, 1 + np.sin(1)]), rtol=1e-8)
+    np.testing.assert_allclose(J0.toarray(), np.array([[2, 1], [2, 0.54030231]]), rtol=1e-8)
```

### Comparing `solverz-0.0.1rc1/Solverz/equation/equations.py` & `solverz-0.0.1rc2/Solverz/equation/equations.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,641 +1,641 @@
-from __future__ import annotations
-
-import warnings
-from numbers import Number
-from typing import Union, List, Dict, Tuple
-from copy import deepcopy
-
-import numpy as np
-from sympy import Symbol, Integer, Expr, Number as SymNumber
-from scipy.sparse import csc_array, coo_array
-# from cvxopt import spmatrix, matrix
-
-from Solverz.equation.eqn import Eqn, Ode, EqnDiff
-from Solverz.equation.param import ParamBase, Param, IdxParam
-from Solverz.sym_algebra.symbols import iVar, idx, IdxVar, Para, iAliasVar
-from Solverz.sym_algebra.functions import Slice
-from Solverz.variable.variables import Vars
-from Solverz.utilities.address import Address, combine_Address
-from Solverz.num_api.Array import Array
-
-
-class Equations:
-
-    def __init__(self,
-                 eqn: Union[List[Eqn], Eqn],
-                 name: str = None,
-                 matrix_container='scipy'):
-        self.name = name
-
-        self.EQNs: Dict[str, Eqn] = dict()
-        self.SYMBOLS: Dict[str, Symbol] = dict()
-        self.a = Address()  # equation address
-        self.var_address = Address()  # variable address
-        self.esize: Dict[str, int] = dict()  # size of each equation
-        self.vsize: int = 0  # size of variables
-        self.f_list = []
-        self.g_list = []
-        self.matrix_container = matrix_container
-        self.PARAM: Dict[str, ParamBase] = dict()
-        self.triggerable_quantity: Dict[str, str] = dict()
-        self.jac_element_address = Address()
-
-        if isinstance(eqn, Eqn):
-            eqn = [eqn]
-
-        for eqn_ in eqn:
-            self.add_eqn(eqn_)
-
-    def add_eqn(self, eqn: Eqn):
-        if eqn.name in self.EQNs.keys():
-            raise ValueError(f"Equation {eqn.name} already defined!")
-        self.EQNs.update({eqn.name: eqn})
-        self.SYMBOLS.update(eqn.SYMBOLS)
-        self.a.add(eqn.name)
-        if isinstance(eqn, Eqn) and not isinstance(eqn, Ode):
-            self.g_list = self.g_list + [eqn.name]
-        elif isinstance(eqn, Ode):
-            self.f_list = self.f_list + [eqn.name]
-
-        for symbol_ in eqn.SYMBOLS.values():
-            if isinstance(symbol_, (Para, iAliasVar)):
-                # this is not fully initialize of Parameters, please use param_initializer
-                self.PARAM[symbol_.name] = Param(symbol_.name, value=symbol_.value, dim=symbol_.dim)
-            elif isinstance(symbol_, idx):
-                self.PARAM[symbol_.name] = IdxParam(symbol_.name, value=symbol_.value)
-
-        self.EQNs[eqn.name].derive_derivative()
-
-    def assign_eqn_var_address(self, *xys: Vars):
-        pass
-
-    @property
-    def eqn_size(self):
-        # total size of all the equations
-        return np.sum(np.array(list(self.esize.values())))
-
-    def is_param_defined(self, param: str) -> bool:
-
-        if param in self.SYMBOLS:
-            return True
-        else:
-            return False
-
-    with warnings.catch_warnings():
-        warnings.simplefilter("once")
-
-    def param_initializer(self, name, param: ParamBase):
-        if not self.is_param_defined(name):
-            warnings.warn(f'Parameter {name} not defined in equations!')
-        if isinstance(param, ParamBase):
-            self.PARAM[name] = param
-            if param.triggerable:
-                self.triggerable_quantity[param.name] = param.trigger_var
-        else:
-            raise TypeError(f"Unsupported parameter type {type(param)}")
-
-    def update_param(self, *args):
-
-        if isinstance(args[0], str):
-            # Update specified params
-            param: str = args[0]
-            value: Union[np.ndarray, list, Number] = args[1]
-            try:
-                if param in self.PARAM:
-                    self.PARAM[param].v = value
-            except KeyError:
-                warnings.warn(f'Equations have no parameter: {param}')
-        elif isinstance(args[0], Vars):
-            # Update params with Vars. For example, to update x0 in trapezoid rules.
-            vars_: Vars = args[0]
-            for param_name in self.PARAM.keys():
-                if param_name in vars_.var_list:
-                    self.PARAM[param_name].v = vars_[param_name]
-
-    def eval(self, eqn_name: str, *args: Union[np.ndarray]) -> np.ndarray:
-        """
-        Evaluate equations
-        :param eqn_name:
-        :param args:
-        :return:
-        """
-        return Array(self.EQNs[eqn_name].NUM_EQN(*args), dim=1)
-
-    def trigger_param_updater(self, eqn: Eqn, *xys):
-        # update/initialize triggerable params
-        if len(xys) > 0:
-            for para_name, trigger_var in self.triggerable_quantity.items():
-                trigger_func = self.PARAM[para_name].trigger_fun
-                args = []
-                for var in trigger_var:
-                    var_value = None
-                    if var in self.PARAM:
-                        var_value = self.PARAM[var].v
-                    else:
-                        for y in xys:
-                            if var in y.var_list:
-                                var_value = y[var]
-                    if var_value is None:
-                        raise ValueError(f'Para/iVar {var} not defined')
-                    else:
-                        args.append(var_value)
-                temp = trigger_func(*args)
-                if self.PARAM[para_name].v is None:
-                    self.PARAM[para_name].v = temp
-                else:
-                    if type(temp) is not type(self.PARAM[para_name].v):
-                        raise TypeError(
-                            f"The return types of trigger func for param {para_name} must be {type(self.PARAM[para_name].v)}")
-
-    def obtain_eqn_args(self, eqn: Eqn, t=None, *xys: Vars) -> List[np.ndarray]:
-        """
-        Obtain the args of equations
-        """
-
-        self.trigger_param_updater(eqn, *xys)
-
-        args = []
-        for symbol in eqn.SYMBOLS.values():
-            value_obtained = False
-            if symbol.name in self.PARAM:
-                temp = self.PARAM[symbol.name].get_v_t(t)
-                if temp is None:
-                    raise TypeError(f'Parameter {symbol.name} uninitialized')
-                args.append(temp)
-                value_obtained = True
-            else:
-                for y in xys:
-                    if symbol.name in y.var_list:
-                        args.append(y[symbol.name])
-                        value_obtained = True
-            if not value_obtained:
-                raise ValueError(f'Cannot find the values of variable {symbol.name}')
-        return args
-
-    def eval_diffs(self, eqn_name: str, var_name: str, *args: np.ndarray) -> np.ndarray:
-        """
-        Evaluate derivative of equations
-        :param eqn_name:
-        :param var_name:
-        :param args:
-        :return:
-        """
-        return self.EQNs[eqn_name].derivatives[var_name].NUM_EQN(*args)
-
-    def parse_address(self, eqn_name, var_name, eqndiff, t=None, *xys):
-        var_idx = eqndiff.var_idx
-        var_idx_func = eqndiff.var_idx_func
-
-        equation_address = self.a.v[eqn_name]
-        if var_idx is None:
-            variable_address = self.var_address.v[var_name]
-        elif isinstance(var_idx, (float, int)):
-            variable_address = self.var_address.v[var_name][var_idx: var_idx + 1]
-        elif isinstance(var_idx, str):
-            variable_address = self.var_address.v[var_name][np.ix_(self.PARAM[var_idx].v.reshape((-1,)))]
-        elif isinstance(var_idx, slice):
-            variable_address = self.var_address.v[var_name][
-                var_idx_func.NUM_EQN(*self.obtain_eqn_args(var_idx_func, t, *xys))]
-        elif isinstance(var_idx, Expr):
-            args = self.obtain_eqn_args(var_idx_func, *xys)
-            variable_address = self.var_address.v[var_name][var_idx_func.NUM_EQN(*args).reshape(-1, )]
-        elif isinstance(var_idx, list):
-            variable_address = self.var_address.v[var_name][var_idx]
-        else:
-            raise TypeError(f"Unsupported variable index {var_idx} for equation {eqn_name}")
-
-        return equation_address, variable_address
-
-    def evalf(self, expr: Expr, t, *xys: Vars) -> np.ndarray:
-        eqn = Eqn('Solverz evalf temporal equation', expr)
-        args = self.obtain_eqn_args(eqn, t, *xys)
-        return eqn.NUM_EQN(*args)
-
-
-class AE(Equations):
-
-    def __init__(self,
-                 eqn: Union[List[Eqn], Eqn],
-                 name: str = None,
-                 matrix_container='scipy'):
-        super().__init__(eqn, name, matrix_container)
-
-        # Check if some equation in self.eqn is Eqn.
-        # If not, raise error
-        if len(self.f_list) > 0:
-            raise ValueError(f'Ode found. This object should be DAE!')
-
-    def assign_eqn_var_address(self, *xys: Vars):
-        """
-        ASSIGN ADDRESSES TO EQUATIONS
-        """
-        y = xys[0]
-
-        temp = 0
-        for eqn_name in self.EQNs.keys():
-            geval = self.g(y, eqn_name)
-            if isinstance(geval, Number):
-                eqn_size = 1
-            else:
-                eqn_size = geval.shape[0]
-            self.a.update(eqn_name, eqn_size)
-            temp = temp + eqn_size
-            self.esize[eqn_name] = eqn_size
-        self.var_address = y.a
-        self.vsize = y.total_size
-
-        # assign dim of derivatives, which is indispensable in Jac printer
-        gy = self.g_y(y)
-        for gy_tuple in gy:
-            eqn_name = gy_tuple[0]
-            var_name = gy_tuple[1]
-            eqndiff = gy_tuple[2]
-            value = gy_tuple[3]
-            if isinstance(value, (np.ndarray, csc_array)):
-                # We use coo_array here because by default when converting to CSR or CSC format,
-                # duplicate (i,j) entries will be summed together.
-                # This facilitates efficient construction of finite element matrices and the like.
-                if value.ndim == 2:  # matrix
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
-
-                elif value.ndim == 1 and value.shape[0] != 1:  # vector
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
-                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
-                else:
-                    raise ValueError("Unknown derivative value dimension type!")
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
-            elif isinstance(value, (Number, SymNumber)):
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
-            else:
-                raise ValueError(f"Unknown derivative data type {type(value)}!")
-
-    def g(self, y: Vars, eqn: str = None) -> np.ndarray:
-        """
-
-        :param y:
-        :param eqn:
-        :return:
-        """
-        temp = []
-        if not eqn:
-            for eqn_name, eqn_ in self.EQNs.items():
-                args = self.obtain_eqn_args(eqn_, None, y)
-                g_eqny = self.eval(eqn_name, *args)
-                g_eqny = g_eqny.toarray() if isinstance(g_eqny, csc_array) else g_eqny
-                temp.append(g_eqny.reshape(-1, ))
-            return np.hstack(temp)
-        else:
-            args = self.obtain_eqn_args(self.EQNs[eqn], None, y)
-            return self.eval(eqn, *args)
-
-    def g_y(self, y: Vars, eqn: List[str] = None, var: List[str] = None) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
-        """
-        generate Jacobian matrices of Eqn object with respect to var object
-        :param y:
-        :param eqn:
-        :param var:
-        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
-        """
-        if not eqn:
-            eqn = list(self.EQNs.keys())
-        if not var:
-            var = list(y.var_list)
-
-        gy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
-
-        for eqn_name in eqn:
-            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
-            for var_name in var:
-                for key, value in eqn_diffs.items():
-                    if var_name == value.diff_var_name:  # f is viewed as f[k]
-                        args = self.obtain_eqn_args(eqn_diffs[key], None, y)
-                        temp = self.eval_diffs(eqn_name, key, *args)
-                        gy = [*gy, (eqn_name, var_name, eqn_diffs[key], temp)]
-        return gy
-
-    def __repr__(self):
-        if not self.eqn_size:
-            return f"Algebraic equation {self.name} with addresses uninitialized"
-        else:
-            return f"Algebraic equation {self.name} ({self.eqn_size}×{self.vsize})"
-
-
-class FDAE(AE):
-
-    def __init__(self,
-                 eqn: Union[List[Eqn], Eqn],
-                 nstep: int,
-                 name: str = None,
-                 matrix_container='scipy'):
-        super().__init__(eqn, name, matrix_container)
-
-        self.nstep = nstep
-
-    def __repr__(self):
-        if not self.eqn_size:
-            return f"FDAE {self.name} with addresses uninitialized"
-        else:
-            return f"FDAE {self.name} ({self.eqn_size}×{self.vsize})"
-
-
-class DAE(Equations):
-
-    def __init__(self,
-                 eqn: Union[List[Eqn], Eqn],
-                 name: str = None,
-                 matrix_container='scipy'
-                 ):
-
-        super().__init__(eqn, name, matrix_container)
-
-        self.state_num: int = 0  # number of state variables
-        self.algebra_num: int = 0  # number of algebraic variables
-
-        # Check if some equation in self.eqn is Ode.
-        # If not, raise error
-        if len(self.f_list) == 0:
-            raise ValueError(f'No ODE found. You should initialise AE instead!')
-
-    def assign_eqn_var_address(self, *xys: Vars):
-        """
-        ASSIGN ADDRESSES TO EQUATIONS f and g
-        """
-
-        temp = 0
-        for eqn_name in self.f_list:
-            feval = self.f(None, *xys, eqn=eqn_name)
-            lhs_eval = self.eval_lhs(None, *xys, eqn=eqn_name)
-            if isinstance(feval, Number):
-                rhs_size = 1
-            else:
-                rhs_size = feval.shape[0]
-            if isinstance(lhs_eval, Number):
-                lhs_size = 1
-            else:
-                lhs_size = lhs_eval.shape[0]
-            eqn_size = np.max([rhs_size, lhs_size])
-            self.a.update(eqn_name, eqn_size)
-            temp = temp + eqn_size
-            self.esize[eqn_name] = eqn_size
-
-        self.state_num = temp
-
-        for eqn_name in self.g_list:
-            geval = self.g(None, *xys, eqn=eqn_name)
-            if np.max(np.abs(geval)) > 1e-5:
-                warnings.warn(
-                    f'Inconsistent initial values for algebraic equation: {eqn_name}, with deviation {np.max(np.abs(geval))}!')
-            if isinstance(geval, Number):
-                eqn_size = 1
-            else:
-                eqn_size = geval.shape[0]
-            self.a.update(eqn_name, eqn_size)
-            temp = temp + eqn_size
-            self.esize[eqn_name] = eqn_size
-
-        self.algebra_num = temp - self.state_num
-
-        if len(xys) == 1:
-            self.var_address = xys[0].a
-            self.vsize = self.var_address.total_size
-        elif len(xys) == 2:
-            x = xys[0]
-            y = xys[1]
-            if x.total_size != self.state_num:
-                raise ValueError("Length of input state variable not compatible with state equations!")
-            if y.total_size != self.algebra_num:
-                raise ValueError("Length of input algebraic variable not compatible with algebraic equations!")
-            self.var_address = combine_Address(x.a, y.a)
-
-            for var_name in self.var_address.v.keys():
-                if var_name not in self.SYMBOLS:
-                    raise ValueError(f"DAE {self.name} has no variable {var_name}")
-
-            self.vsize: int = self.var_address.total_size
-        elif len(xys) > 2:
-            raise ValueError("Accept at most two positional arguments!")
-
-        # assign dim of derivatives, which is indispensable in Jac printer
-        fg_xy = self.f_xy(0, *xys)
-        if len(self.g_list) > 0:
-            fg_xy.extend(self.g_xy(0, *xys))
-        for gy_tuple in fg_xy:
-            eqn_name = gy_tuple[0]
-            var_name = gy_tuple[1]
-            eqndiff = gy_tuple[2]
-            value = gy_tuple[3]
-            if isinstance(value, (np.ndarray, csc_array)):
-                # We use coo_array here because by default when converting to CSR or CSC format,
-                # duplicate (i,j) entries will be summed together.
-                # This facilitates efficient construction of finite element matrices and the like.
-                if value.ndim == 2:  # matrix
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
-
-                elif value.ndim == 1 and value.shape[0] != 1:  # vector
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
-                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
-                else:
-                    raise ValueError("Unknown derivative value dimension type!")
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
-            elif isinstance(value, (Number, SymNumber)):
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
-            else:
-                raise ValueError(f"Unknown derivative data type {type(value)}!")
-
-    def F(self, t, *xys) -> np.ndarray:
-        """
-        Return [f(t,x,y), g(t,x,y)]
-        :param t: time
-        :param xys: Vars
-        :return:
-        """
-        if len(self.g_list) > 0:
-            return np.concatenate([self.f(t, *xys), self.g(t, *xys)])
-        else:
-            return self.f(t, *xys)
-
-    def f(self, t, *xys, eqn=None) -> np.ndarray:
-
-        temp = []
-        if eqn:
-            if eqn in self.f_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
-                temp.append(self.eval(eqn, *args).reshape(-1, ))
-        else:
-            for eqn in self.f_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
-                temp.append(self.eval(eqn, *args).reshape(-1, ))
-
-        return np.hstack(temp)
-
-    def eval_lhs(self, t, *xys, eqn=None) -> np.ndarray:
-
-        temp = []
-        if eqn:
-            if eqn in self.f_list:
-                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
-                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
-                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
-        else:
-            for eqn in self.f_list:
-                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
-                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
-                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
-
-        return np.hstack(temp)
-
-    def g(self, t, *xys, eqn=None) -> np.ndarray:
-        """
-
-        `xys` is either:
-          - two arguments, e.g. state vars x, and numerical equation y
-          - one argument, e.g. state vars y.
-
-        """
-
-        if len(self.g_list) == 0:
-            raise ValueError(f'No AE found in {self.name}!')
-
-        temp = []
-        if eqn:
-            if eqn in self.g_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
-                temp.append(self.eval(eqn, *args).reshape(-1, ))
-        else:
-            for eqn in self.g_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
-                temp.append(self.eval(eqn, *args).reshape(-1, ))
-
-        return np.hstack(temp)
-
-    def f_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
-        """
-        generate partial derivatives of f w.r.t. vars in xys
-        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
-        """
-
-        fxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
-
-        var: List[str] = list()
-        for xy in xys:
-            var = var + xy.var_list
-
-        for eqn_name in self.f_list:
-            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
-            for var_name in var:
-                for key, value in eqn_diffs.items():
-                    if var_name == value.diff_var_name:
-                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
-                        temp = self.eval_diffs(eqn_name, key, *args)
-                        fxy = [*fxy, (eqn_name, var_name, eqn_diffs[key], temp)]
-        return fxy
-
-    def g_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
-        """
-        generate partial derivatives of f w.r.t. vars in xys
-        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
-        """
-
-        if len(self.g_list) == 0:
-            raise ValueError(f'No AE found in {self.name}!')
-
-        gxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
-
-        var: List[str] = list()
-        for xy in xys:
-            var = var + xy.var_list
-
-        for eqn_name in self.g_list:
-            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
-            for var_name in var:
-                for key, value in eqn_diffs.items():
-                    if var_name == value.diff_var_name:
-                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
-                        temp = self.eval_diffs(eqn_name, key, *args)
-                        gxy = [*gxy, (eqn_name, var_name, eqn_diffs[key], temp)]
-        return gxy
-
-    @property
-    def M(self):
-        """
-        return the singular mass matrix, M, of dae
-        Row of 1 in M corresponds to the differential equation
-        Col of 1 in M corresponds to the state variable
-        """
-        if self.state_num == 0:
-            raise ValueError("DAE address uninitialized!")
-
-        row = []
-        col = []
-        for eqn_name in self.f_list:
-            eqn = self.EQNs[eqn_name]
-            equation_address = self.a.v[eqn_name]
-            if isinstance(eqn, Ode):
-                diff_var = eqn.diff_var
-                if isinstance(diff_var, iVar):
-                    variable_address = self.var_address.v[diff_var.name]
-                elif isinstance(diff_var, IdxVar):
-                    var_idx = diff_var.index
-                    var_name = diff_var.name0
-                    if isinstance(var_idx, (np.integer, int, Integer)):
-                        variable_address = self.var_address.v[var_name][var_idx: var_idx + 1]
-                    elif isinstance(var_idx, str):
-                        variable_address = self.var_address.v[var_name][np.ix_(self.PARAM[var_idx].v.reshape((-1,)))]
-                    elif isinstance(var_idx, slice):
-                        temp = []
-                        if var_idx.start is not None:
-                            temp.append(var_idx.start)
-                        if var_idx.stop is not None:
-                            temp.append(var_idx.stop)
-                        if var_idx.step is not None:
-                            temp.append(var_idx.step)
-                        temp_func = Eqn('To evaluate var_idx of variable' + diff_var.name, Slice(*temp))
-                        variable_address = self.var_address.v[var_name][
-                            temp_func.NUM_EQN(*self.obtain_eqn_args(temp_func))]
-                    elif isinstance(var_idx, Expr):
-                        temp_func = Eqn('To evaluate var_idx of variable' + diff_var.name, var_idx)
-                        args = self.obtain_eqn_args(temp_func)
-                        variable_address = self.var_address.v[var_name][temp_func.NUM_EQN(*args).reshape(-1, )]
-                    elif isinstance(var_idx, list):
-                        variable_address = self.var_address.v[var_name][var_idx]
-                    else:
-                        raise TypeError(f"Unsupported variable index {var_idx} in equation {eqn_name}")
-                else:
-                    raise NotImplementedError
-                eqn_address_list = equation_address.tolist()
-                var_address_list = variable_address.tolist()
-                if len(eqn_address_list) != len(var_address_list):
-                    raise ValueError(f"Incompatible eqn address length {len(eqn_address_list)} and variable address length {len(var_address_list)}")
-                row.extend(eqn_address_list)
-                col.extend(var_address_list)
-            else:
-                raise ValueError("Equation in f_list is non-Ode.")
-
-        if self.matrix_container == 'scipy':
-            return csc_array((np.ones((self.state_num,)), (row, col)), (self.eqn_size, self.vsize))
-        elif self.matrix_container == 'cvxopt':
-            raise NotImplementedError("Not implemented!")
-        else:
-            raise ValueError(f"Unsupported matrix container {self.matrix_container}")
-
-    @property
-    def alg_eqn_addr(self):
-        addr_list = []
-        for eqn in self.g_list:
-            addr_list.extend(self.a.v[eqn].tolist())
-
-        return addr_list
-
-    def __repr__(self):
-        if not self.eqn_size:
-            return f"DAE {self.name} with addresses uninitialized"
-        else:
-            return f"DAE {self.name} ({self.eqn_size}×{self.vsize})"
+from __future__ import annotations
+
+import warnings
+from numbers import Number
+from typing import Union, List, Dict, Tuple
+from copy import deepcopy
+
+import numpy as np
+from sympy import Symbol, Integer, Expr, Number as SymNumber
+from scipy.sparse import csc_array, coo_array
+# from cvxopt import spmatrix, matrix
+
+from Solverz.equation.eqn import Eqn, Ode, EqnDiff
+from Solverz.equation.param import ParamBase, Param, IdxParam
+from Solverz.sym_algebra.symbols import iVar, idx, IdxVar, Para, iAliasVar
+from Solverz.sym_algebra.functions import Slice
+from Solverz.variable.variables import Vars
+from Solverz.utilities.address import Address, combine_Address
+from Solverz.num_api.Array import Array
+
+
+class Equations:
+
+    def __init__(self,
+                 eqn: Union[List[Eqn], Eqn],
+                 name: str = None,
+                 matrix_container='scipy'):
+        self.name = name
+
+        self.EQNs: Dict[str, Eqn] = dict()
+        self.SYMBOLS: Dict[str, Symbol] = dict()
+        self.a = Address()  # equation address
+        self.var_address = Address()  # variable address
+        self.esize: Dict[str, int] = dict()  # size of each equation
+        self.vsize: int = 0  # size of variables
+        self.f_list = []
+        self.g_list = []
+        self.matrix_container = matrix_container
+        self.PARAM: Dict[str, ParamBase] = dict()
+        self.triggerable_quantity: Dict[str, str] = dict()
+        self.jac_element_address = Address()
+
+        if isinstance(eqn, Eqn):
+            eqn = [eqn]
+
+        for eqn_ in eqn:
+            self.add_eqn(eqn_)
+
+    def add_eqn(self, eqn: Eqn):
+        if eqn.name in self.EQNs.keys():
+            raise ValueError(f"Equation {eqn.name} already defined!")
+        self.EQNs.update({eqn.name: eqn})
+        self.SYMBOLS.update(eqn.SYMBOLS)
+        self.a.add(eqn.name)
+        if isinstance(eqn, Eqn) and not isinstance(eqn, Ode):
+            self.g_list = self.g_list + [eqn.name]
+        elif isinstance(eqn, Ode):
+            self.f_list = self.f_list + [eqn.name]
+
+        for symbol_ in eqn.SYMBOLS.values():
+            if isinstance(symbol_, (Para, iAliasVar)):
+                # this is not fully initialize of Parameters, please use param_initializer
+                self.PARAM[symbol_.name] = Param(symbol_.name, value=symbol_.value, dim=symbol_.dim)
+            elif isinstance(symbol_, idx):
+                self.PARAM[symbol_.name] = IdxParam(symbol_.name, value=symbol_.value)
+
+        self.EQNs[eqn.name].derive_derivative()
+
+    def assign_eqn_var_address(self, *xys: Vars):
+        pass
+
+    @property
+    def eqn_size(self):
+        # total size of all the equations
+        return np.sum(np.array(list(self.esize.values())))
+
+    def is_param_defined(self, param: str) -> bool:
+
+        if param in self.SYMBOLS:
+            return True
+        else:
+            return False
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("once")
+
+    def param_initializer(self, name, param: ParamBase):
+        if not self.is_param_defined(name):
+            warnings.warn(f'Parameter {name} not defined in equations!')
+        if isinstance(param, ParamBase):
+            self.PARAM[name] = param
+            if param.triggerable:
+                self.triggerable_quantity[param.name] = param.trigger_var
+        else:
+            raise TypeError(f"Unsupported parameter type {type(param)}")
+
+    def update_param(self, *args):
+
+        if isinstance(args[0], str):
+            # Update specified params
+            param: str = args[0]
+            value: Union[np.ndarray, list, Number] = args[1]
+            try:
+                if param in self.PARAM:
+                    self.PARAM[param].v = value
+            except KeyError:
+                warnings.warn(f'Equations have no parameter: {param}')
+        elif isinstance(args[0], Vars):
+            # Update params with Vars. For example, to update x0 in trapezoid rules.
+            vars_: Vars = args[0]
+            for param_name in self.PARAM.keys():
+                if param_name in vars_.var_list:
+                    self.PARAM[param_name].v = vars_[param_name]
+
+    def eval(self, eqn_name: str, *args: Union[np.ndarray]) -> np.ndarray:
+        """
+        Evaluate equations
+        :param eqn_name:
+        :param args:
+        :return:
+        """
+        return Array(self.EQNs[eqn_name].NUM_EQN(*args), dim=1)
+
+    def trigger_param_updater(self, eqn: Eqn, *xys):
+        # update/initialize triggerable params
+        if len(xys) > 0:
+            for para_name, trigger_var in self.triggerable_quantity.items():
+                trigger_func = self.PARAM[para_name].trigger_fun
+                args = []
+                for var in trigger_var:
+                    var_value = None
+                    if var in self.PARAM:
+                        var_value = self.PARAM[var].v
+                    else:
+                        for y in xys:
+                            if var in y.var_list:
+                                var_value = y[var]
+                    if var_value is None:
+                        raise ValueError(f'Para/iVar {var} not defined')
+                    else:
+                        args.append(var_value)
+                temp = trigger_func(*args)
+                if self.PARAM[para_name].v is None:
+                    self.PARAM[para_name].v = temp
+                else:
+                    if type(temp) is not type(self.PARAM[para_name].v):
+                        raise TypeError(
+                            f"The return types of trigger func for param {para_name} must be {type(self.PARAM[para_name].v)}")
+
+    def obtain_eqn_args(self, eqn: Eqn, t=None, *xys: Vars) -> List[np.ndarray]:
+        """
+        Obtain the args of equations
+        """
+
+        self.trigger_param_updater(eqn, *xys)
+
+        args = []
+        for symbol in eqn.SYMBOLS.values():
+            value_obtained = False
+            if symbol.name in self.PARAM:
+                temp = self.PARAM[symbol.name].get_v_t(t)
+                if temp is None:
+                    raise TypeError(f'Parameter {symbol.name} uninitialized')
+                args.append(temp)
+                value_obtained = True
+            else:
+                for y in xys:
+                    if symbol.name in y.var_list:
+                        args.append(y[symbol.name])
+                        value_obtained = True
+            if not value_obtained:
+                raise ValueError(f'Cannot find the values of variable {symbol.name}')
+        return args
+
+    def eval_diffs(self, eqn_name: str, var_name: str, *args: np.ndarray) -> np.ndarray:
+        """
+        Evaluate derivative of equations
+        :param eqn_name:
+        :param var_name:
+        :param args:
+        :return:
+        """
+        return self.EQNs[eqn_name].derivatives[var_name].NUM_EQN(*args)
+
+    def parse_address(self, eqn_name, var_name, eqndiff, t=None, *xys):
+        var_idx = eqndiff.var_idx
+        var_idx_func = eqndiff.var_idx_func
+
+        equation_address = self.a.v[eqn_name]
+        if var_idx is None:
+            variable_address = self.var_address.v[var_name]
+        elif isinstance(var_idx, (float, int)):
+            variable_address = self.var_address.v[var_name][var_idx: var_idx + 1]
+        elif isinstance(var_idx, str):
+            variable_address = self.var_address.v[var_name][np.ix_(self.PARAM[var_idx].v.reshape((-1,)))]
+        elif isinstance(var_idx, slice):
+            variable_address = self.var_address.v[var_name][
+                var_idx_func.NUM_EQN(*self.obtain_eqn_args(var_idx_func, t, *xys))]
+        elif isinstance(var_idx, Expr):
+            args = self.obtain_eqn_args(var_idx_func, *xys)
+            variable_address = self.var_address.v[var_name][var_idx_func.NUM_EQN(*args).reshape(-1, )]
+        elif isinstance(var_idx, list):
+            variable_address = self.var_address.v[var_name][var_idx]
+        else:
+            raise TypeError(f"Unsupported variable index {var_idx} for equation {eqn_name}")
+
+        return equation_address, variable_address
+
+    def evalf(self, expr: Expr, t, *xys: Vars) -> np.ndarray:
+        eqn = Eqn('Solverz evalf temporal equation', expr)
+        args = self.obtain_eqn_args(eqn, t, *xys)
+        return eqn.NUM_EQN(*args)
+
+
+class AE(Equations):
+
+    def __init__(self,
+                 eqn: Union[List[Eqn], Eqn],
+                 name: str = None,
+                 matrix_container='scipy'):
+        super().__init__(eqn, name, matrix_container)
+
+        # Check if some equation in self.eqn is Eqn.
+        # If not, raise error
+        if len(self.f_list) > 0:
+            raise ValueError(f'Ode found. This object should be DAE!')
+
+    def assign_eqn_var_address(self, *xys: Vars):
+        """
+        ASSIGN ADDRESSES TO EQUATIONS
+        """
+        y = xys[0]
+
+        temp = 0
+        for eqn_name in self.EQNs.keys():
+            geval = self.g(y, eqn_name)
+            if isinstance(geval, Number):
+                eqn_size = 1
+            else:
+                eqn_size = geval.shape[0]
+            self.a.update(eqn_name, eqn_size)
+            temp = temp + eqn_size
+            self.esize[eqn_name] = eqn_size
+        self.var_address = y.a
+        self.vsize = y.total_size
+
+        # assign dim of derivatives, which is indispensable in Jac printer
+        gy = self.g_y(y)
+        for gy_tuple in gy:
+            eqn_name = gy_tuple[0]
+            var_name = gy_tuple[1]
+            eqndiff = gy_tuple[2]
+            value = gy_tuple[3]
+            if isinstance(value, (np.ndarray, csc_array)):
+                # We use coo_array here because by default when converting to CSR or CSC format,
+                # duplicate (i,j) entries will be summed together.
+                # This facilitates efficient construction of finite element matrices and the like.
+                if value.ndim == 2:  # matrix
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
+
+                elif value.ndim == 1 and value.shape[0] != 1:  # vector
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
+                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
+                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
+                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
+                else:
+                    raise ValueError("Unknown derivative value dimension type!")
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
+            elif isinstance(value, (Number, SymNumber)):
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
+            else:
+                raise ValueError(f"Unknown derivative data type {type(value)}!")
+
+    def g(self, y: Vars, eqn: str = None) -> np.ndarray:
+        """
+
+        :param y:
+        :param eqn:
+        :return:
+        """
+        temp = []
+        if not eqn:
+            for eqn_name, eqn_ in self.EQNs.items():
+                args = self.obtain_eqn_args(eqn_, None, y)
+                g_eqny = self.eval(eqn_name, *args)
+                g_eqny = g_eqny.toarray() if isinstance(g_eqny, csc_array) else g_eqny
+                temp.append(g_eqny.reshape(-1, ))
+            return np.hstack(temp)
+        else:
+            args = self.obtain_eqn_args(self.EQNs[eqn], None, y)
+            return self.eval(eqn, *args)
+
+    def g_y(self, y: Vars, eqn: List[str] = None, var: List[str] = None) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+        """
+        generate Jacobian matrices of Eqn object with respect to var object
+        :param y:
+        :param eqn:
+        :param var:
+        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
+        """
+        if not eqn:
+            eqn = list(self.EQNs.keys())
+        if not var:
+            var = list(y.var_list)
+
+        gy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
+
+        for eqn_name in eqn:
+            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
+            for var_name in var:
+                for key, value in eqn_diffs.items():
+                    if var_name == value.diff_var_name:  # f is viewed as f[k]
+                        args = self.obtain_eqn_args(eqn_diffs[key], None, y)
+                        temp = self.eval_diffs(eqn_name, key, *args)
+                        gy = [*gy, (eqn_name, var_name, eqn_diffs[key], temp)]
+        return gy
+
+    def __repr__(self):
+        if not self.eqn_size:
+            return f"Algebraic equation {self.name} with addresses uninitialized"
+        else:
+            return f"Algebraic equation {self.name} ({self.eqn_size}×{self.vsize})"
+
+
+class FDAE(AE):
+
+    def __init__(self,
+                 eqn: Union[List[Eqn], Eqn],
+                 nstep: int,
+                 name: str = None,
+                 matrix_container='scipy'):
+        super().__init__(eqn, name, matrix_container)
+
+        self.nstep = nstep
+
+    def __repr__(self):
+        if not self.eqn_size:
+            return f"FDAE {self.name} with addresses uninitialized"
+        else:
+            return f"FDAE {self.name} ({self.eqn_size}×{self.vsize})"
+
+
+class DAE(Equations):
+
+    def __init__(self,
+                 eqn: Union[List[Eqn], Eqn],
+                 name: str = None,
+                 matrix_container='scipy'
+                 ):
+
+        super().__init__(eqn, name, matrix_container)
+
+        self.state_num: int = 0  # number of state variables
+        self.algebra_num: int = 0  # number of algebraic variables
+
+        # Check if some equation in self.eqn is Ode.
+        # If not, raise error
+        if len(self.f_list) == 0:
+            raise ValueError(f'No ODE found. You should initialise AE instead!')
+
+    def assign_eqn_var_address(self, *xys: Vars):
+        """
+        ASSIGN ADDRESSES TO EQUATIONS f and g
+        """
+
+        temp = 0
+        for eqn_name in self.f_list:
+            feval = self.f(None, *xys, eqn=eqn_name)
+            lhs_eval = self.eval_lhs(None, *xys, eqn=eqn_name)
+            if isinstance(feval, Number):
+                rhs_size = 1
+            else:
+                rhs_size = feval.shape[0]
+            if isinstance(lhs_eval, Number):
+                lhs_size = 1
+            else:
+                lhs_size = lhs_eval.shape[0]
+            eqn_size = np.max([rhs_size, lhs_size])
+            self.a.update(eqn_name, eqn_size)
+            temp = temp + eqn_size
+            self.esize[eqn_name] = eqn_size
+
+        self.state_num = temp
+
+        for eqn_name in self.g_list:
+            geval = self.g(None, *xys, eqn=eqn_name)
+            if np.max(np.abs(geval)) > 1e-5:
+                warnings.warn(
+                    f'Inconsistent initial values for algebraic equation: {eqn_name}, with deviation {np.max(np.abs(geval))}!')
+            if isinstance(geval, Number):
+                eqn_size = 1
+            else:
+                eqn_size = geval.shape[0]
+            self.a.update(eqn_name, eqn_size)
+            temp = temp + eqn_size
+            self.esize[eqn_name] = eqn_size
+
+        self.algebra_num = temp - self.state_num
+
+        if len(xys) == 1:
+            self.var_address = xys[0].a
+            self.vsize = self.var_address.total_size
+        elif len(xys) == 2:
+            x = xys[0]
+            y = xys[1]
+            if x.total_size != self.state_num:
+                raise ValueError("Length of input state variable not compatible with state equations!")
+            if y.total_size != self.algebra_num:
+                raise ValueError("Length of input algebraic variable not compatible with algebraic equations!")
+            self.var_address = combine_Address(x.a, y.a)
+
+            for var_name in self.var_address.v.keys():
+                if var_name not in self.SYMBOLS:
+                    raise ValueError(f"DAE {self.name} has no variable {var_name}")
+
+            self.vsize: int = self.var_address.total_size
+        elif len(xys) > 2:
+            raise ValueError("Accept at most two positional arguments!")
+
+        # assign dim of derivatives, which is indispensable in Jac printer
+        fg_xy = self.f_xy(0, *xys)
+        if len(self.g_list) > 0:
+            fg_xy.extend(self.g_xy(0, *xys))
+        for gy_tuple in fg_xy:
+            eqn_name = gy_tuple[0]
+            var_name = gy_tuple[1]
+            eqndiff = gy_tuple[2]
+            value = gy_tuple[3]
+            if isinstance(value, (np.ndarray, csc_array)):
+                # We use coo_array here because by default when converting to CSR or CSC format,
+                # duplicate (i,j) entries will be summed together.
+                # This facilitates efficient construction of finite element matrices and the like.
+                if value.ndim == 2:  # matrix
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
+
+                elif value.ndim == 1 and value.shape[0] != 1:  # vector
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
+                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
+                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
+                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
+                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
+                else:
+                    raise ValueError("Unknown derivative value dimension type!")
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
+            elif isinstance(value, (Number, SymNumber)):
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
+                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
+            else:
+                raise ValueError(f"Unknown derivative data type {type(value)}!")
+
+    def F(self, t, *xys) -> np.ndarray:
+        """
+        Return [f(t,x,y), g(t,x,y)]
+        :param t: time
+        :param xys: Vars
+        :return:
+        """
+        if len(self.g_list) > 0:
+            return np.concatenate([self.f(t, *xys), self.g(t, *xys)])
+        else:
+            return self.f(t, *xys)
+
+    def f(self, t, *xys, eqn=None) -> np.ndarray:
+
+        temp = []
+        if eqn:
+            if eqn in self.f_list:
+                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                temp.append(self.eval(eqn, *args).reshape(-1, ))
+        else:
+            for eqn in self.f_list:
+                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                temp.append(self.eval(eqn, *args).reshape(-1, ))
+
+        return np.hstack(temp)
+
+    def eval_lhs(self, t, *xys, eqn=None) -> np.ndarray:
+
+        temp = []
+        if eqn:
+            if eqn in self.f_list:
+                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
+                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
+                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+        else:
+            for eqn in self.f_list:
+                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
+                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
+                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+
+        return np.hstack(temp)
+
+    def g(self, t, *xys, eqn=None) -> np.ndarray:
+        """
+
+        `xys` is either:
+          - two arguments, e.g. state vars x, and numerical equation y
+          - one argument, e.g. state vars y.
+
+        """
+
+        if len(self.g_list) == 0:
+            raise ValueError(f'No AE found in {self.name}!')
+
+        temp = []
+        if eqn:
+            if eqn in self.g_list:
+                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                temp.append(self.eval(eqn, *args).reshape(-1, ))
+        else:
+            for eqn in self.g_list:
+                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                temp.append(self.eval(eqn, *args).reshape(-1, ))
+
+        return np.hstack(temp)
+
+    def f_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+        """
+        generate partial derivatives of f w.r.t. vars in xys
+        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
+        """
+
+        fxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
+
+        var: List[str] = list()
+        for xy in xys:
+            var = var + xy.var_list
+
+        for eqn_name in self.f_list:
+            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
+            for var_name in var:
+                for key, value in eqn_diffs.items():
+                    if var_name == value.diff_var_name:
+                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
+                        temp = self.eval_diffs(eqn_name, key, *args)
+                        fxy = [*fxy, (eqn_name, var_name, eqn_diffs[key], temp)]
+        return fxy
+
+    def g_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+        """
+        generate partial derivatives of f w.r.t. vars in xys
+        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
+        """
+
+        if len(self.g_list) == 0:
+            raise ValueError(f'No AE found in {self.name}!')
+
+        gxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
+
+        var: List[str] = list()
+        for xy in xys:
+            var = var + xy.var_list
+
+        for eqn_name in self.g_list:
+            eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
+            for var_name in var:
+                for key, value in eqn_diffs.items():
+                    if var_name == value.diff_var_name:
+                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
+                        temp = self.eval_diffs(eqn_name, key, *args)
+                        gxy = [*gxy, (eqn_name, var_name, eqn_diffs[key], temp)]
+        return gxy
+
+    @property
+    def M(self):
+        """
+        return the singular mass matrix, M, of dae
+        Row of 1 in M corresponds to the differential equation
+        Col of 1 in M corresponds to the state variable
+        """
+        if self.state_num == 0:
+            raise ValueError("DAE address uninitialized!")
+
+        row = []
+        col = []
+        for eqn_name in self.f_list:
+            eqn = self.EQNs[eqn_name]
+            equation_address = self.a.v[eqn_name]
+            if isinstance(eqn, Ode):
+                diff_var = eqn.diff_var
+                if isinstance(diff_var, iVar):
+                    variable_address = self.var_address.v[diff_var.name]
+                elif isinstance(diff_var, IdxVar):
+                    var_idx = diff_var.index
+                    var_name = diff_var.name0
+                    if isinstance(var_idx, (np.integer, int, Integer)):
+                        variable_address = self.var_address.v[var_name][var_idx: var_idx + 1]
+                    elif isinstance(var_idx, str):
+                        variable_address = self.var_address.v[var_name][np.ix_(self.PARAM[var_idx].v.reshape((-1,)))]
+                    elif isinstance(var_idx, slice):
+                        temp = []
+                        if var_idx.start is not None:
+                            temp.append(var_idx.start)
+                        if var_idx.stop is not None:
+                            temp.append(var_idx.stop)
+                        if var_idx.step is not None:
+                            temp.append(var_idx.step)
+                        temp_func = Eqn('To evaluate var_idx of variable' + diff_var.name, Slice(*temp))
+                        variable_address = self.var_address.v[var_name][
+                            temp_func.NUM_EQN(*self.obtain_eqn_args(temp_func))]
+                    elif isinstance(var_idx, Expr):
+                        temp_func = Eqn('To evaluate var_idx of variable' + diff_var.name, var_idx)
+                        args = self.obtain_eqn_args(temp_func)
+                        variable_address = self.var_address.v[var_name][temp_func.NUM_EQN(*args).reshape(-1, )]
+                    elif isinstance(var_idx, list):
+                        variable_address = self.var_address.v[var_name][var_idx]
+                    else:
+                        raise TypeError(f"Unsupported variable index {var_idx} in equation {eqn_name}")
+                else:
+                    raise NotImplementedError
+                eqn_address_list = equation_address.tolist()
+                var_address_list = variable_address.tolist()
+                if len(eqn_address_list) != len(var_address_list):
+                    raise ValueError(f"Incompatible eqn address length {len(eqn_address_list)} and variable address length {len(var_address_list)}")
+                row.extend(eqn_address_list)
+                col.extend(var_address_list)
+            else:
+                raise ValueError("Equation in f_list is non-Ode.")
+
+        if self.matrix_container == 'scipy':
+            return csc_array((np.ones((self.state_num,)), (row, col)), (self.eqn_size, self.vsize))
+        elif self.matrix_container == 'cvxopt':
+            raise NotImplementedError("Not implemented!")
+        else:
+            raise ValueError(f"Unsupported matrix container {self.matrix_container}")
+
+    @property
+    def alg_eqn_addr(self):
+        addr_list = []
+        for eqn in self.g_list:
+            addr_list.extend(self.a.v[eqn].tolist())
+
+        return addr_list
+
+    def __repr__(self):
+        if not self.eqn_size:
+            return f"DAE {self.name} with addresses uninitialized"
+        else:
+            return f"DAE {self.name} ({self.eqn_size}×{self.vsize})"
```

### Comparing `solverz-0.0.1rc1/Solverz/equation/param.py` & `solverz-0.0.1rc2/Solverz/equation/param.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-from typing import Callable, Optional, Union, List
-from numbers import Number
-
-import numpy as np
-from scipy.interpolate import interp1d
-
-from Solverz.num_api.Array import Array
-from Solverz.variable.ssymbol import sSymBasic
-
-
-class ParamBase:
-    def __init__(self,
-                 name: str,
-                 value: Union[np.ndarray, list, Number] = None,
-                 triggerable: bool = False,
-                 trigger_var: Union[str, List[str]] = None,
-                 trigger_fun: Callable = None,
-                 dim: int = 1,
-                 dtype=float,
-                 sparse=False):
-        self.name = name
-        self.triggerable = triggerable
-        self.trigger_var = [trigger_var] if isinstance(trigger_var, str) else trigger_var
-        self.trigger_fun = trigger_fun
-        self.dim = dim
-        self.dtype = dtype
-        self.sparse = sparse
-        self.__v = None
-        self.v = value
-
-    @property
-    def v(self):
-        return self.__v
-
-    @v.setter
-    def v(self, value):
-
-        if value is None:
-            self.__v = None
-        else:
-            self.__v = Array(value, dim=self.dim, sparse=self.sparse, dtype=self.dtype)
-
-    def get_v_t(self, t):
-        return self.v
-
-    def __repr__(self):
-        return f"Param: {self.name} value: {self.v}"
-
-
-class Param(ParamBase, sSymBasic):
-
-    def __init__(self,
-                 name: str,
-                 value: Union[np.ndarray, list, Number] = None,
-                 triggerable: bool = False,
-                 trigger_var: Union[str, List[str]] = None,
-                 trigger_fun: Callable = None,
-                 dim: int = 1,
-                 dtype=float,
-                 sparse=False
-                 ):
-        ParamBase.__init__(self,
-                           name,
-                           value,
-                           triggerable,
-                           trigger_var,
-                           trigger_fun,
-                           dim,
-                           dtype,
-                           sparse)
-        sSymBasic.__init__(self, name=name, Type='Para', value=value, dim=dim)
-
-
-class IdxParam(ParamBase, sSymBasic):
-
-    def __init__(self,
-                 name: str,
-                 value: Union[np.ndarray, list, Number] = None,
-                 triggerable: bool = False,
-                 trigger_var: str = None,
-                 trigger_fun: Callable = None
-                 ):
-        ParamBase.__init__(self,
-                           name,
-                           value,
-                           triggerable,
-                           trigger_var,
-                           trigger_fun,
-                           dim=1,
-                           dtype=int,
-                           sparse=False)
-        sSymBasic.__init__(self,
-                           name=name,
-                           Type='idx',
-                           value=value,
-                           dim=1)
-
-
-class TimeSeriesParam(Param):
-    def __init__(self,
-                 name: str,
-                 v_series,
-                 time_series,
-                 index=None,
-                 value: Union[np.ndarray, list, Number] = None,
-                 dim=1,
-                 dtype=float,
-                 sparse=False
-                 ):
-        if value is None:
-            value = v_series[0]
-        super().__init__(name,
-                         value,
-                         triggerable=False,
-                         trigger_var=None,
-                         trigger_fun=None,
-                         dim=dim,
-                         dtype=dtype,
-                         sparse=sparse)
-        self.v_series = Array(v_series, dim=1)
-        self.time_series = Array(time_series, dim=1)
-        self.tend = self.time_series[-1]
-
-        if len(self.v_series) != len(self.time_series):
-            raise ValueError("Incompatible length between value series and time series!")
-        if not np.all(np.diff(self.time_series) > 0):
-            raise ValueError("Time stamp should be strictly monotonically increasing!")
-        self.index = index
-        self.vt = interp1d(self.time_series, self.v_series, kind='linear')
-
-    def get_v_t(self, t):
-        if t is None:
-            return self.v
-
-        if t < self.tend:
-            # input of interp1d is zero-dimensional, we need to reshape
-            # [0] is to eliminate the numpy DeprecationWarning in m3b9 test: Conversion of an array with ndim > 0 to a scalar is
-            # deprecated, and will error in the future, which should be resolved.
-            vt = self.vt(t).reshape((-1,))[0]
-        else:
-            vt = self.v_series[-1]
-
-        if self.index is not None:
-            temp = self.v.copy()
-
-            temp[self.index] = vt
-
-            return temp
-        else:
-            return vt
-
-    def __repr__(self):
-        return f"TimeSeriesParam: {self.name} value: {self.v}"
+from typing import Callable, Optional, Union, List
+from numbers import Number
+
+import numpy as np
+from scipy.interpolate import interp1d
+
+from Solverz.num_api.Array import Array
+from Solverz.variable.ssymbol import sSymBasic
+
+
+class ParamBase:
+    def __init__(self,
+                 name: str,
+                 value: Union[np.ndarray, list, Number] = None,
+                 triggerable: bool = False,
+                 trigger_var: Union[str, List[str]] = None,
+                 trigger_fun: Callable = None,
+                 dim: int = 1,
+                 dtype=float,
+                 sparse=False):
+        self.name = name
+        self.triggerable = triggerable
+        self.trigger_var = [trigger_var] if isinstance(trigger_var, str) else trigger_var
+        self.trigger_fun = trigger_fun
+        self.dim = dim
+        self.dtype = dtype
+        self.sparse = sparse
+        self.__v = None
+        self.v = value
+
+    @property
+    def v(self):
+        return self.__v
+
+    @v.setter
+    def v(self, value):
+
+        if value is None:
+            self.__v = None
+        else:
+            self.__v = Array(value, dim=self.dim, sparse=self.sparse, dtype=self.dtype)
+
+    def get_v_t(self, t):
+        return self.v
+
+    def __repr__(self):
+        return f"Param: {self.name} value: {self.v}"
+
+
+class Param(ParamBase, sSymBasic):
+
+    def __init__(self,
+                 name: str,
+                 value: Union[np.ndarray, list, Number] = None,
+                 triggerable: bool = False,
+                 trigger_var: Union[str, List[str]] = None,
+                 trigger_fun: Callable = None,
+                 dim: int = 1,
+                 dtype=float,
+                 sparse=False
+                 ):
+        ParamBase.__init__(self,
+                           name,
+                           value,
+                           triggerable,
+                           trigger_var,
+                           trigger_fun,
+                           dim,
+                           dtype,
+                           sparse)
+        sSymBasic.__init__(self, name=name, Type='Para', value=value, dim=dim)
+
+
+class IdxParam(ParamBase, sSymBasic):
+
+    def __init__(self,
+                 name: str,
+                 value: Union[np.ndarray, list, Number] = None,
+                 triggerable: bool = False,
+                 trigger_var: str = None,
+                 trigger_fun: Callable = None
+                 ):
+        ParamBase.__init__(self,
+                           name,
+                           value,
+                           triggerable,
+                           trigger_var,
+                           trigger_fun,
+                           dim=1,
+                           dtype=int,
+                           sparse=False)
+        sSymBasic.__init__(self,
+                           name=name,
+                           Type='idx',
+                           value=value,
+                           dim=1)
+
+
+class TimeSeriesParam(Param):
+    def __init__(self,
+                 name: str,
+                 v_series,
+                 time_series,
+                 index=None,
+                 value: Union[np.ndarray, list, Number] = None,
+                 dim=1,
+                 dtype=float,
+                 sparse=False
+                 ):
+        if value is None:
+            value = v_series[0]
+        super().__init__(name,
+                         value,
+                         triggerable=False,
+                         trigger_var=None,
+                         trigger_fun=None,
+                         dim=dim,
+                         dtype=dtype,
+                         sparse=sparse)
+        self.v_series = Array(v_series, dim=1)
+        self.time_series = Array(time_series, dim=1)
+        self.tend = self.time_series[-1]
+
+        if len(self.v_series) != len(self.time_series):
+            raise ValueError("Incompatible length between value series and time series!")
+        if not np.all(np.diff(self.time_series) > 0):
+            raise ValueError("Time stamp should be strictly monotonically increasing!")
+        self.index = index
+        self.vt = interp1d(self.time_series, self.v_series, kind='linear')
+
+    def get_v_t(self, t):
+        if t is None:
+            return self.v
+
+        if t < self.tend:
+            # input of interp1d is zero-dimensional, we need to reshape
+            # [0] is to eliminate the numpy DeprecationWarning in m3b9 test: Conversion of an array with ndim > 0 to a scalar is
+            # deprecated, and will error in the future, which should be resolved.
+            vt = self.vt(t).reshape((-1,))[0]
+        else:
+            vt = self.v_series[-1]
+
+        if self.index is not None:
+            temp = self.v.copy()
+
+            temp[self.index] = vt
+
+            return temp
+        else:
+            return vt
+
+    def __repr__(self):
+        return f"TimeSeriesParam: {self.name} value: {self.v}"
```

### Comparing `solverz-0.0.1rc1/Solverz/equation/test/test_DAE.py` & `solverz-0.0.1rc2/Solverz/equation/test/test_DAE.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from sympy import Integer
-from Solverz import Ode, iVar, DAE, as_Vars, made_numerical
-
-
-def test_zero_index():
-    # to test if index zero, being the sympy.Integer.instance, raises error when creating the singular mass mat
-    u = iVar('u', [3])
-    zero = Integer(0)
-    f = Ode('f', u[zero], u[zero])
-    sdae = DAE(f)
-    y = as_Vars(u)
-    dae = made_numerical(sdae, y)
-
-
-def test_ode():
-    # The RHS is a scalar zero, but the equation is of size 3
-    x = iVar('x', [1, 2, 3])
-    f = Ode('f', 0, x[0:3])
-    sdae = DAE(f)
-    y = as_Vars(x)
-    sdae.assign_eqn_var_address(y)
-    assert sdae.eqn_size == 3
+from sympy import Integer
+from Solverz import Ode, iVar, DAE, as_Vars, made_numerical
+
+
+def test_zero_index():
+    # to test if index zero, being the sympy.Integer.instance, raises error when creating the singular mass mat
+    u = iVar('u', [3])
+    zero = Integer(0)
+    f = Ode('f', u[zero], u[zero])
+    sdae = DAE(f)
+    y = as_Vars(u)
+    dae = made_numerical(sdae, y)
+
+
+def test_ode():
+    # The RHS is a scalar zero, but the equation is of size 3
+    x = iVar('x', [1, 2, 3])
+    f = Ode('f', 0, x[0:3])
+    sdae = DAE(f)
+    y = as_Vars(x)
+    sdae.assign_eqn_var_address(y)
+    assert sdae.eqn_size == 3
```

### Comparing `solverz-0.0.1rc1/Solverz/equation/test/test_Param.py` & `solverz-0.0.1rc2/Solverz/equation/test/test_Param.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import numpy as np
-
-from Solverz.equation.param import Param, IdxParam, TimeSeriesParam
-
-
-def test_Param():
-    # test of Param basic
-    Ts1 = Param(name='Ts')
-    try:
-        Ts1.v = [[100, 100]]
-    except ValueError as e:
-        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
-    Ts1.v = [100, 100]
-    assert Ts1.v.__str__() == '[100. 100.]'
-
-    Ts2 = Param(name='Ts', value=[1, 2, 3], dim=1)
-    assert Ts2.v.__str__() == '[1. 2. 3.]'
-
-    Ts3 = Param(name='Ts', value=[1, 2, 3], dim=2)
-    assert Ts3.v.__str__() == '[[1.]\n [2.]\n [3.]]'
-
-    Ts4 = Param(name='Ts', value=[1, 2, 3], dim=2, sparse=True)
-    assert Ts4.v.__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (2, 0)\t3.0'
-
-    Ts5 = Param(name='Ts', value=[1, 2, 3], dim=2, sparse=False)
-    assert Ts5.v.__str__() == '[[1.]\n [2.]\n [3.]]'
-
-    A = np.array([[1, 0], [2, 9], [0, 3]])
-    A = Param(name='A', value=A, dim=2, sparse=True)
-    assert A.v.__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (1, 1)\t9.0\n  (2, 1)\t3.0'
-
-    # test of IdxParam
-    f = IdxParam(name='f',
-                 value=[1, 2, 3])
-
-    try:
-        t = IdxParam(name='t',
-                     value=[[1, 2, 3]])
-    except ValueError as e:
-        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
-
-    # test of TimeSeriesParam
-    Pb = TimeSeriesParam(name='Pb',
-                         v_series=[0, 10, 100],
-                         time_series=[0, 10, 20],
-                         value=0)
-    assert Pb.get_v_t(5).__str__() == '5.0'
-
-    try:
-        Pb = TimeSeriesParam(name='Pb',
-                             v_series=[0, 10, 100],
-                             time_series=[0, -10, 20],
-                             value=0)
-    except ValueError as e:
-        assert e.args[0] == 'Time stamp should be strictly monotonically increasing!'
-
-    try:
-        Pb = TimeSeriesParam(name='Pb',
-                             v_series=[0, 10, 100, 200],
-                             time_series=[0, 10, 20],
-                             value=0)
-    except ValueError as e:
-        assert e.args[0] == 'Incompatible length between value series and time series!'
-
-    G = TimeSeriesParam(name='G',
-                        v_series=[2, 10000, 10000, 2, 2],
-                        time_series=[0, 0.002, 0.03, 0.032, 10],
-                        value=np.array([[1, 0, 3], [0, 0.1, -0.4], [1.2, -np.pi, 0]]),
-                        index=(1, 1),
-                        dim=2,
-                        sparse=True)
-    assert (G.get_v_t(0.001).toarray().__str__() ==
-            '[[ 1.00000000e+00  0.00000000e+00  3.00000000e+00]\n [ 0.00000000e+00  5.00100000e+03 -4.00000000e-01]\n [ 1.20000000e+00 -3.14159265e+00  0.00000000e+00]]')
+import numpy as np
+
+from Solverz.equation.param import Param, IdxParam, TimeSeriesParam
+
+
+def test_Param():
+    # test of Param basic
+    Ts1 = Param(name='Ts')
+    try:
+        Ts1.v = [[100, 100]]
+    except ValueError as e:
+        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
+    Ts1.v = [100, 100]
+    assert Ts1.v.__str__() == '[100. 100.]'
+
+    Ts2 = Param(name='Ts', value=[1, 2, 3], dim=1)
+    assert Ts2.v.__str__() == '[1. 2. 3.]'
+
+    Ts3 = Param(name='Ts', value=[1, 2, 3], dim=2)
+    assert Ts3.v.__str__() == '[[1.]\n [2.]\n [3.]]'
+
+    Ts4 = Param(name='Ts', value=[1, 2, 3], dim=2, sparse=True)
+    assert Ts4.v.__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (2, 0)\t3.0'
+
+    Ts5 = Param(name='Ts', value=[1, 2, 3], dim=2, sparse=False)
+    assert Ts5.v.__str__() == '[[1.]\n [2.]\n [3.]]'
+
+    A = np.array([[1, 0], [2, 9], [0, 3]])
+    A = Param(name='A', value=A, dim=2, sparse=True)
+    assert A.v.__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (1, 1)\t9.0\n  (2, 1)\t3.0'
+
+    # test of IdxParam
+    f = IdxParam(name='f',
+                 value=[1, 2, 3])
+
+    try:
+        t = IdxParam(name='t',
+                     value=[[1, 2, 3]])
+    except ValueError as e:
+        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
+
+    # test of TimeSeriesParam
+    Pb = TimeSeriesParam(name='Pb',
+                         v_series=[0, 10, 100],
+                         time_series=[0, 10, 20],
+                         value=0)
+    assert Pb.get_v_t(5).__str__() == '5.0'
+
+    try:
+        Pb = TimeSeriesParam(name='Pb',
+                             v_series=[0, 10, 100],
+                             time_series=[0, -10, 20],
+                             value=0)
+    except ValueError as e:
+        assert e.args[0] == 'Time stamp should be strictly monotonically increasing!'
+
+    try:
+        Pb = TimeSeriesParam(name='Pb',
+                             v_series=[0, 10, 100, 200],
+                             time_series=[0, 10, 20],
+                             value=0)
+    except ValueError as e:
+        assert e.args[0] == 'Incompatible length between value series and time series!'
+
+    G = TimeSeriesParam(name='G',
+                        v_series=[2, 10000, 10000, 2, 2],
+                        time_series=[0, 0.002, 0.03, 0.032, 10],
+                        value=np.array([[1, 0, 3], [0, 0.1, -0.4], [1.2, -np.pi, 0]]),
+                        index=(1, 1),
+                        dim=2,
+                        sparse=True)
+    assert (G.get_v_t(0.001).toarray().__str__() ==
+            '[[ 1.00000000e+00  0.00000000e+00  3.00000000e+00]\n [ 0.00000000e+00  5.00100000e+03 -4.00000000e-01]\n [ 1.20000000e+00 -3.14159265e+00  0.00000000e+00]]')
```

### Comparing `solverz-0.0.1rc1/Solverz/equation/test/test_jac.py` & `solverz-0.0.1rc2/Solverz/equation/test/test_jac.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from numbers import Number
-
-import numpy as np
-
-from Solverz.equation.eqn import Eqn, Ode
-from Solverz.equation.equations import DAE, AE
-from Solverz.equation.param import Param
-from Solverz.sym_algebra.symbols import iVar, idx, Para
-from Solverz.variable.variables import combine_Vars, as_Vars
-
-
-def test_jac():
-    x = iVar('x', 1)
-    y = iVar('y', 1)
-
-    f = Ode(name='f', f=-x ** 3 + 0.5 * y ** 2, diff_var=x)
-    g = Eqn(name='g', eqn=x ** 2 + y ** 2 - 2)
-    dae = DAE([f, g])
-
-    z = combine_Vars(as_Vars(x), as_Vars(y))
-    fxy = dae.f_xy(None, z)
-    gxy = dae.g_xy(None, z)
-    assert fxy[0][3].shape == (1,)
-    assert np.all(np.isclose(fxy[0][3], [-3.]))
-    assert fxy[1][3].shape == (1,)
-    assert np.all(np.isclose(fxy[1][3], [1]))
-    assert gxy[0][3].shape == (1,)
-    assert np.all(np.isclose(gxy[0][3], [2]))
-    assert gxy[1][3].shape == (1,)
-    assert np.all(np.isclose(gxy[1][3], [2]))
-
-    x = iVar('x', [1, 2, 3])
-    i = idx('i', value=[0, 2])
-
-    f = Eqn('f', eqn=x)
-    ae = AE(f)
-    gy = ae.g_y(as_Vars(x))
-    assert isinstance(gy[0][3], Number)
-    # assert gy[0][3].ndim == 0
-    assert np.all(np.isclose(gy[0][3], 1))
-
-    f = Eqn('f', eqn=x[i])
-    ae = AE(f)
-    gy = ae.g_y(as_Vars(x))
-    assert isinstance(gy[0][3], Number)
-    # assert gy[0][3].ndim == 0
-    assert np.all(np.isclose(gy[0][3], 1))
-
-    f = Eqn('f', eqn=x[i] ** 2)
-    ae = AE(f)
-    gy = ae.g_y(as_Vars(x))
-    assert isinstance(gy[0][3], np.ndarray)
-    assert gy[0][3].ndim == 1
-    assert np.all(np.isclose(gy[0][3], [2., 6.]))
-
-    A_v = np.random.rand(3, 3)
-    A = Para('A', dim=2)
-    f = Eqn('f', eqn=A * x)
-    ae = AE(f)
-    ae.param_initializer('A', Param('A', value=A_v, dim=2))
-    gy = ae.g_y(as_Vars(x))
-    assert isinstance(gy[0][3], np.ndarray)
-    assert gy[0][3].ndim == 2
-    np.testing.assert_allclose(gy[0][3], A_v)
-
+from numbers import Number
+
+import numpy as np
+
+from Solverz.equation.eqn import Eqn, Ode
+from Solverz.equation.equations import DAE, AE
+from Solverz.equation.param import Param
+from Solverz.sym_algebra.symbols import iVar, idx, Para
+from Solverz.variable.variables import combine_Vars, as_Vars
+
+
+def test_jac():
+    x = iVar('x', 1)
+    y = iVar('y', 1)
+
+    f = Ode(name='f', f=-x ** 3 + 0.5 * y ** 2, diff_var=x)
+    g = Eqn(name='g', eqn=x ** 2 + y ** 2 - 2)
+    dae = DAE([f, g])
+
+    z = combine_Vars(as_Vars(x), as_Vars(y))
+    fxy = dae.f_xy(None, z)
+    gxy = dae.g_xy(None, z)
+    assert fxy[0][3].shape == (1,)
+    assert np.all(np.isclose(fxy[0][3], [-3.]))
+    assert fxy[1][3].shape == (1,)
+    assert np.all(np.isclose(fxy[1][3], [1]))
+    assert gxy[0][3].shape == (1,)
+    assert np.all(np.isclose(gxy[0][3], [2]))
+    assert gxy[1][3].shape == (1,)
+    assert np.all(np.isclose(gxy[1][3], [2]))
+
+    x = iVar('x', [1, 2, 3])
+    i = idx('i', value=[0, 2])
+
+    f = Eqn('f', eqn=x)
+    ae = AE(f)
+    gy = ae.g_y(as_Vars(x))
+    assert isinstance(gy[0][3], Number)
+    # assert gy[0][3].ndim == 0
+    assert np.all(np.isclose(gy[0][3], 1))
+
+    f = Eqn('f', eqn=x[i])
+    ae = AE(f)
+    gy = ae.g_y(as_Vars(x))
+    assert isinstance(gy[0][3], Number)
+    # assert gy[0][3].ndim == 0
+    assert np.all(np.isclose(gy[0][3], 1))
+
+    f = Eqn('f', eqn=x[i] ** 2)
+    ae = AE(f)
+    gy = ae.g_y(as_Vars(x))
+    assert isinstance(gy[0][3], np.ndarray)
+    assert gy[0][3].ndim == 1
+    assert np.all(np.isclose(gy[0][3], [2., 6.]))
+
+    A_v = np.random.rand(3, 3)
+    A = Para('A', dim=2)
+    f = Eqn('f', eqn=A * x)
+    ae = AE(f)
+    ae.param_initializer('A', Param('A', value=A_v, dim=2))
+    gy = ae.g_y(as_Vars(x))
+    assert isinstance(gy[0][3], np.ndarray)
+    assert gy[0][3].ndim == 2
+    np.testing.assert_allclose(gy[0][3], A_v)
+
```

### Comparing `solverz-0.0.1rc1/Solverz/model/basic.py` & `solverz-0.0.1rc2/Solverz/model/basic.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from typing import Dict
-import warnings
-
-import numpy as np
-from Solverz.equation.equations import AE, FDAE, DAE
-from Solverz.equation.param import ParamBase
-from Solverz.equation.eqn import Eqn, Ode
-from Solverz.utilities.address import Address
-from Solverz.variable.variables import Vars
-from Solverz.variable.ssymbol import Var, AliasVar
-from Solverz.num_api.Array import Array
-
-
-class Model:
-
-    def __init__(self):
-        self.eqn_dict = dict()
-        self.var_dict: Dict[str, Var] = dict()
-        self.param_dict = dict()
-        self.alias_dict = dict()
-
-    def init_var(self, name):
-        init_func = Eqn(f'init_func_{name}', self.var_dict[name].init)
-        args = []
-        for arg in init_func.SYMBOLS.keys():
-            if arg in self.param_dict:
-                args += [self.param_dict[arg].value]
-            elif arg in self.var_dict:
-                if self.var_dict[arg].value is not None:
-                    args += [self.var_dict[arg].value]
-                else:
-                    args += [self.init_var(arg)]
-        self.var_dict[name].value = Array(init_func.NUM_EQN(*args), dim=1)
-
-    def create_instance(self):
-        attr_dict = vars(self)
-
-        eqn_type = 'AE'
-        nstep = None
-        for key, value in attr_dict.items():
-            if isinstance(value, (Ode, Eqn)):
-                self.eqn_dict[key] = value
-            elif isinstance(value, Var):
-                self.var_dict[key] = value
-            elif isinstance(value, ParamBase):
-                self.param_dict[key] = value
-            elif isinstance(value, AliasVar):
-                nstep = 1 if nstep is None else nstep
-                self.alias_dict[key] = value
-                nstep = np.max([nstep, value.step])
-
-        if any([isinstance(arg, Ode) for arg in self.eqn_dict.values()]):
-            if nstep is not None:
-                raise ValueError("DAE object cannot have iAliasVar!")
-            eqn_type = 'DAE'
-        elif nstep is not None:
-            eqn_type = 'FDAE'
-
-        if eqn_type == 'AE':
-            eqs = AE(list(self.eqn_dict.values()))
-        elif eqn_type == 'DAE':
-            eqs = DAE(list(self.eqn_dict.values()))
-        elif eqn_type == 'FDAE':
-            eqs = FDAE(list(self.eqn_dict.values()), nstep=nstep)
-        else:
-            raise TypeError(f"Equation type {eqn_type} not implemented!")
-
-        for name, param in self.param_dict.items():
-            if isinstance(param, ParamBase):
-                eqs.param_initializer(name, param)
-
-        a = Address()
-        # initialize variables
-        for name, var in self.var_dict.items():
-            if var.value is None and var.init is None:
-                raise ValueError(f'Variable {name} not initialized and init func not provided!')
-            elif var.value is None and var.init is not None:
-                self.init_var(name)
-            a.add(name, self.var_dict[name].value.shape[0])
-
-        array = np.zeros((a.total_size,))
-        for var in a.object_list:
-            array[a[var]] = self.var_dict[var].value
-        y0 = Vars(a, array)
-        if eqn_type == 'FDAE':
-            for i in range(nstep):
-                eqs.update_param(y0.derive_alias(f'_tag_{i}'))
-        eqs.assign_eqn_var_address(y0)
-
-        if eqs.eqn_size != eqs.vsize:
-            warnings.warn(f'Equation size {eqs.eqn_size} and variable size {eqs.vsize} not equal!')
-
-        return eqs, y0
+from typing import Dict
+import warnings
+
+import numpy as np
+from Solverz.equation.equations import AE, FDAE, DAE
+from Solverz.equation.param import ParamBase
+from Solverz.equation.eqn import Eqn, Ode
+from Solverz.utilities.address import Address
+from Solverz.variable.variables import Vars
+from Solverz.variable.ssymbol import Var, AliasVar
+from Solverz.num_api.Array import Array
+
+
+class Model:
+
+    def __init__(self):
+        self.eqn_dict = dict()
+        self.var_dict: Dict[str, Var] = dict()
+        self.param_dict = dict()
+        self.alias_dict = dict()
+
+    def init_var(self, name):
+        init_func = Eqn(f'init_func_{name}', self.var_dict[name].init)
+        args = []
+        for arg in init_func.SYMBOLS.keys():
+            if arg in self.param_dict:
+                args += [self.param_dict[arg].value]
+            elif arg in self.var_dict:
+                if self.var_dict[arg].value is not None:
+                    args += [self.var_dict[arg].value]
+                else:
+                    args += [self.init_var(arg)]
+        self.var_dict[name].value = Array(init_func.NUM_EQN(*args), dim=1)
+
+    def create_instance(self):
+        attr_dict = vars(self)
+
+        eqn_type = 'AE'
+        nstep = None
+        for key, value in attr_dict.items():
+            if isinstance(value, (Ode, Eqn)):
+                self.eqn_dict[key] = value
+            elif isinstance(value, Var):
+                self.var_dict[key] = value
+            elif isinstance(value, ParamBase):
+                self.param_dict[key] = value
+            elif isinstance(value, AliasVar):
+                nstep = 1 if nstep is None else nstep
+                self.alias_dict[key] = value
+                nstep = np.max([nstep, value.step])
+
+        if any([isinstance(arg, Ode) for arg in self.eqn_dict.values()]):
+            if nstep is not None:
+                raise ValueError("DAE object cannot have iAliasVar!")
+            eqn_type = 'DAE'
+        elif nstep is not None:
+            eqn_type = 'FDAE'
+
+        if eqn_type == 'AE':
+            eqs = AE(list(self.eqn_dict.values()))
+        elif eqn_type == 'DAE':
+            eqs = DAE(list(self.eqn_dict.values()))
+        elif eqn_type == 'FDAE':
+            eqs = FDAE(list(self.eqn_dict.values()), nstep=nstep)
+        else:
+            raise TypeError(f"Equation type {eqn_type} not implemented!")
+
+        for name, param in self.param_dict.items():
+            if isinstance(param, ParamBase):
+                eqs.param_initializer(name, param)
+
+        a = Address()
+        # initialize variables
+        for name, var in self.var_dict.items():
+            if var.value is None and var.init is None:
+                raise ValueError(f'Variable {name} not initialized and init func not provided!')
+            elif var.value is None and var.init is not None:
+                self.init_var(name)
+            a.add(name, self.var_dict[name].value.shape[0])
+
+        array = np.zeros((a.total_size,))
+        for var in a.object_list:
+            array[a[var]] = self.var_dict[var].value
+        y0 = Vars(a, array)
+        if eqn_type == 'FDAE':
+            for i in range(nstep):
+                eqs.update_param(y0.derive_alias(f'_tag_{i}'))
+        eqs.assign_eqn_var_address(y0)
+
+        if eqs.eqn_size != eqs.vsize:
+            warnings.warn(f'Equation size {eqs.eqn_size} and variable size {eqs.vsize} not equal!')
+
+        return eqs, y0
```

### Comparing `solverz-0.0.1rc1/Solverz/num_api/Array.py` & `solverz-0.0.1rc2/Solverz/num_api/Array.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import Union
-
-import numpy as np
-from numbers import Number
-from scipy.sparse import csc_array
-
-
-def type_checker(dtype):
-    if not np.issubdtype(dtype, np.integer) and not np.issubdtype(dtype, np.floating) and not np.issubdtype(dtype, np.complexfloating):
-        raise TypeError(f"Unsupported data type {dtype}")
-
-
-def Array(array: Union[np.ndarray, csc_array, list, Number],
-          dim=2,
-          sparse=False,
-          dtype=float) -> Union[np.ndarray, csc_array]:
-    type_checker(dtype)
-    if dim < 2 and sparse:
-        raise ValueError(f"Cannot create sparse matrix with dim: {dim}")
-
-    # initialize and check dtype in case of non-int/float dtypes
-    if isinstance(array, Number):
-        temp = np.array(array, dtype=dtype)
-    elif isinstance(array, list):
-        temp = np.array(array)
-        type_checker(temp.dtype)
-        if temp.ndim > dim:
-            raise ValueError(f"Input list dim {temp.ndim} higher than dim set to be {dim}")
-        temp = temp.astype(dtype)
-    elif isinstance(array, np.ndarray):
-        type_checker(array.dtype)
-        temp = array.astype(dtype)
-        if temp.ndim > dim:
-            raise ValueError(f"Input numpy.ndarray dim {temp.ndim} higher than dim set to be {dim}")
-    elif isinstance(array, csc_array):
-        type_checker(array.dtype)
-        temp = array.astype(dtype)
-        if dim != 2:
-            raise ValueError(f"csc_array input while dim set to be {dim}")
-        if not sparse:
-            raise TypeError(f"csc_array input while sparse arg set to be False")
-    else:
-        raise TypeError(f"Unsupported array type {type(array)}")
-
-    # reshape and sparsify
-    if dim == 1:
-        # This can only be np.ndarray
-        # dim of csc_array must be 2
-        return temp.reshape((-1,))
-    else:
-        # np.ndarray or csc_array
-        if temp.ndim < 2:
-            temp = temp.reshape((-1, 1))
-        if sparse:
-            return csc_array(temp)
-        else:
-            return temp
+from typing import Union
+
+import numpy as np
+from numbers import Number
+from scipy.sparse import csc_array
+
+
+def type_checker(dtype):
+    if not np.issubdtype(dtype, np.integer) and not np.issubdtype(dtype, np.floating) and not np.issubdtype(dtype, np.complexfloating):
+        raise TypeError(f"Unsupported data type {dtype}")
+
+
+def Array(array: Union[np.ndarray, csc_array, list, Number],
+          dim=2,
+          sparse=False,
+          dtype=float) -> Union[np.ndarray, csc_array]:
+    type_checker(dtype)
+    if dim < 2 and sparse:
+        raise ValueError(f"Cannot create sparse matrix with dim: {dim}")
+
+    # initialize and check dtype in case of non-int/float dtypes
+    if isinstance(array, Number):
+        temp = np.array(array, dtype=dtype)
+    elif isinstance(array, list):
+        temp = np.array(array)
+        type_checker(temp.dtype)
+        if temp.ndim > dim:
+            raise ValueError(f"Input list dim {temp.ndim} higher than dim set to be {dim}")
+        temp = temp.astype(dtype)
+    elif isinstance(array, np.ndarray):
+        type_checker(array.dtype)
+        temp = array.astype(dtype)
+        if temp.ndim > dim:
+            raise ValueError(f"Input numpy.ndarray dim {temp.ndim} higher than dim set to be {dim}")
+    elif isinstance(array, csc_array):
+        type_checker(array.dtype)
+        temp = array.astype(dtype)
+        if dim != 2:
+            raise ValueError(f"csc_array input while dim set to be {dim}")
+        if not sparse:
+            raise TypeError(f"csc_array input while sparse arg set to be False")
+    else:
+        raise TypeError(f"Unsupported array type {type(array)}")
+
+    # reshape and sparsify
+    if dim == 1:
+        # This can only be np.ndarray
+        # dim of csc_array must be 2
+        return temp.reshape((-1,))
+    else:
+        # np.ndarray or csc_array
+        if temp.ndim < 2:
+            temp = temp.reshape((-1, 1))
+        if sparse:
+            return csc_array(temp)
+        else:
+            return temp
```

### Comparing `solverz-0.0.1rc1/Solverz/num_api/custom_function.py` & `solverz-0.0.1rc2/Solverz/num_api/custom_function.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-from __future__ import annotations
-
-from functools import reduce
-
-import numpy as np
-from numpy import linalg
-from scipy.sparse import diags, csc_array, coo_array, linalg as sla
-from numba import njit
-
-# from cvxopt.umfpack import linsolve
-# from cvxopt import matrix, spmatrix
-
-numerical_interface = {'coo_array': coo_array, 'csc_array': csc_array}
-
-
-def implements_nfunc(nfunc_name: str):
-    """Register an DT function implementation for sympy Expr."""
-
-    def decorator(func):
-        numerical_interface[nfunc_name] = func
-        return func
-
-    return decorator
-
-
-@implements_nfunc('sol_slice')
-def sol_slice(*args):
-    """
-    This is used to convert the slice arguments to int
-    """
-    return slice(*[int(arg_[0]) if isinstance(arg_, np.ndarray) else arg_ for arg_ in args])
-
-
-@implements_nfunc('Slice')
-def Slice(*args):
-    """
-    This is used to evaluate the slice index of IdxVar/IdxParam/IdxConst
-    """
-    return sol_slice(*args)
-
-
-@implements_nfunc('ix_')
-def ix_(arg: np.ndarray):
-    return arg.reshape(-1, )
-
-
-@implements_nfunc('Sign')
-def _sign(arg):
-    return np.sign(arg)
-
-
-@implements_nfunc('minmod')
-def minmod(a, b, c):
-    stacked_array = np.hstack((a, b, c))
-    cd1 = (a > 0) & (b > 0) & (c > 0)
-    cd2 = (a < 0) & (b < 0) & (c < 0)
-    conditions = [cd1,
-                  cd2]
-    choice_list = [np.min(stacked_array, axis=0),
-                   np.max(stacked_array, axis=0)]
-    return np.select(conditions, choice_list, 0)
-
-
-@implements_nfunc('minmod_flag')
-def minmod_flag(*args):
-    if len(args) != 3:
-        raise ValueError("Input arg length must be 3")
-
-    shapes = [arg.shape[0] for arg in args]
-
-    a, b, c = args
-    stacked_array = np.hstack((a, b, c))
-    if all(x == shapes[0] for x in shapes):
-        cd1 = (a > 0) & (b > 0) & (c > 0)
-        cd2 = (a < 0) & (b < 0) & (c < 0)
-        conditions = [cd1,
-                      cd2]
-        choice_list = [np.argmin(stacked_array, axis=0),
-                       np.argmax(stacked_array, axis=0)]
-    else:
-        raise ValueError(f"Length of Input array not consistent {shapes}")
-    return np.select(conditions, choice_list, 3)
-
-
-@implements_nfunc('switch')
-@njit
-def switch(*args):
-    flag = args[-1]
-    flag_shape = args[-1].shape
-    v_list = list(args[0:len(args) - 1])
-
-    for i in range(len(v_list)):
-        v = v_list[i]
-        if isinstance(v, (int, float)):
-            v_list[i] = v * np.ones(flag_shape)
-        elif isinstance(v, np.ndarray):
-            if v.shape[0] == 1:
-                v_list[i] = v * np.ones(flag_shape)
-    shapes = [v.shape[0] for v in v_list]
-    if all(x.shape[0] == v_list[0].shape[0] for x in v_list):
-        conditions = [flag == i for i in range(len(args) - 1)]
-        choice_list = v_list
-    else:
-        raise ValueError(f"Length of Input array not consistent {shapes}")
-    return np.select(conditions, choice_list, 0)
-
-
-@implements_nfunc('SolIn')
-@njit(cache=True)
-def SolIn(x, xmin, xmax):
-    x = np.asarray(x).reshape((-1,))
-    return np.bitwise_and(x >= xmin, x <= xmax).astype(np.int32)
-
-
-@implements_nfunc('SolGreaterThan')
-@njit(cache=True)
-def SolGreaterThan(x, y):
-    x = np.asarray(x).reshape((-1,))
-    return (x > y).astype(np.int32)
-
-
-@implements_nfunc('SolLessThan')
-@njit(cache=True)
-def SolLessThan(x, y):
-    x = np.asarray(x).reshape((-1,))
-    return (x < y).astype(np.int32)
-
-
-@implements_nfunc('And')
-@njit(cache=True)
-def And(x, y):
-    x = np.asarray(x).reshape((-1,))
-    return x & y
-
-
-@implements_nfunc('Or')
-@njit(cache=True)
-def Or(x, y):
-    x = np.asarray(x).reshape((-1,))
-    return x | y
-
-
-@implements_nfunc('Not')
-@njit(cache=True)
-def Not(x):
-    x = np.asarray(x).reshape((-1,))
-    return np.ones_like(x) - x
-
-
-@implements_nfunc('Diag')
-def diag(x) -> np.ndarray:
-    """
-    Generate diagonal matrix of given vector X
-    :PARAM X: vector
-    :return: diagonal matrix
-    """
-    if not isinstance(x, np.ndarray):
-        return diags(x.toarray().reshape(-1, ), 0, format='csc')
-    else:
-        return np.diagflat(x)
-
-
-@implements_nfunc('dConv_s')
-def DT_conv(*args, method='conv') -> np.ndarray:
-    r"""
-    Perform the convolutions in DT computations.
-
-    Explanation
-    ===========
-
-
-
-    Parameters
-    ==========
-
-    args : np.ndarray
-
-        DT series.
-
-    method : str
-
-        the method used to compute DT convolution
-
-    """
-    if len(args) <= 2 and method == 'conv':  # if input two vectors, then use scalar multiplications and additions
-        x = args[0].reshape((1, -1))
-        y = np.flip(args[1].reshape((-1, 1)), 0)
-        return x @ y
-
-    if len(args) > 2 or method == 'fft':  # if input more than three vectors, use fft and ifft
-        k = args[0].shape[0]
-        y = []
-        m = 2 * (k - 1) + 1  # ensure that we have enough function values to recover the coefficients by ifft
-        n = np.ceil(np.log2(k))  # fft is the fastest when the length of the series is the power of 2
-        for arg in args:
-            # extend the length of the vector to the power of 2
-            arg = np.pad(arg, (0, int(np.maximum(m, n) - k)), constant_values=0)
-            y += [np.fft.fft(arg)]
-        return np.array(np.real(np.fft.ifft(reduce(lambda a, b: a * b, y))[k - 1]))
-
-
-@implements_nfunc('dLinspace')
-def linspace(start, end) -> np.ndarray:
-    r"""
-
-    Parameters
-    ==========
-
-    start:
-
-
-
-    end:
-
-
-
-    """
-    return np.arange(start, end, dtype=int)[:, np.newaxis]
+from __future__ import annotations
+
+from functools import reduce
+
+import numpy as np
+from numpy import linalg
+from scipy.sparse import diags, csc_array, coo_array, linalg as sla
+from numba import njit
+
+# from cvxopt.umfpack import linsolve
+# from cvxopt import matrix, spmatrix
+
+numerical_interface = {'coo_array': coo_array, 'csc_array': csc_array}
+
+
+def implements_nfunc(nfunc_name: str):
+    """Register an DT function implementation for sympy Expr."""
+
+    def decorator(func):
+        numerical_interface[nfunc_name] = func
+        return func
+
+    return decorator
+
+
+@implements_nfunc('sol_slice')
+def sol_slice(*args):
+    """
+    This is used to convert the slice arguments to int
+    """
+    return slice(*[int(arg_[0]) if isinstance(arg_, np.ndarray) else arg_ for arg_ in args])
+
+
+@implements_nfunc('Slice')
+def Slice(*args):
+    """
+    This is used to evaluate the slice index of IdxVar/IdxParam/IdxConst
+    """
+    return sol_slice(*args)
+
+
+@implements_nfunc('ix_')
+def ix_(arg: np.ndarray):
+    return arg.reshape(-1, )
+
+
+@implements_nfunc('Sign')
+def _sign(arg):
+    return np.sign(arg)
+
+
+@implements_nfunc('minmod')
+def minmod(a, b, c):
+    stacked_array = np.hstack((a, b, c))
+    cd1 = (a > 0) & (b > 0) & (c > 0)
+    cd2 = (a < 0) & (b < 0) & (c < 0)
+    conditions = [cd1,
+                  cd2]
+    choice_list = [np.min(stacked_array, axis=0),
+                   np.max(stacked_array, axis=0)]
+    return np.select(conditions, choice_list, 0)
+
+
+@implements_nfunc('minmod_flag')
+def minmod_flag(*args):
+    if len(args) != 3:
+        raise ValueError("Input arg length must be 3")
+
+    shapes = [arg.shape[0] for arg in args]
+
+    a, b, c = args
+    stacked_array = np.hstack((a, b, c))
+    if all(x == shapes[0] for x in shapes):
+        cd1 = (a > 0) & (b > 0) & (c > 0)
+        cd2 = (a < 0) & (b < 0) & (c < 0)
+        conditions = [cd1,
+                      cd2]
+        choice_list = [np.argmin(stacked_array, axis=0),
+                       np.argmax(stacked_array, axis=0)]
+    else:
+        raise ValueError(f"Length of Input array not consistent {shapes}")
+    return np.select(conditions, choice_list, 3)
+
+
+@implements_nfunc('switch')
+@njit
+def switch(*args):
+    flag = args[-1]
+    flag_shape = args[-1].shape
+    v_list = list(args[0:len(args) - 1])
+
+    for i in range(len(v_list)):
+        v = v_list[i]
+        if isinstance(v, (int, float)):
+            v_list[i] = v * np.ones(flag_shape)
+        elif isinstance(v, np.ndarray):
+            if v.shape[0] == 1:
+                v_list[i] = v * np.ones(flag_shape)
+    shapes = [v.shape[0] for v in v_list]
+    if all(x.shape[0] == v_list[0].shape[0] for x in v_list):
+        conditions = [flag == i for i in range(len(args) - 1)]
+        choice_list = v_list
+    else:
+        raise ValueError(f"Length of Input array not consistent {shapes}")
+    return np.select(conditions, choice_list, 0)
+
+
+@implements_nfunc('SolIn')
+@njit(cache=True)
+def SolIn(x, xmin, xmax):
+    x = np.asarray(x).reshape((-1,))
+    return np.bitwise_and(x >= xmin, x <= xmax).astype(np.int32)
+
+
+@implements_nfunc('SolGreaterThan')
+@njit(cache=True)
+def SolGreaterThan(x, y):
+    x = np.asarray(x).reshape((-1,))
+    return (x > y).astype(np.int32)
+
+
+@implements_nfunc('SolLessThan')
+@njit(cache=True)
+def SolLessThan(x, y):
+    x = np.asarray(x).reshape((-1,))
+    return (x < y).astype(np.int32)
+
+
+@implements_nfunc('And')
+@njit(cache=True)
+def And(x, y):
+    x = np.asarray(x).reshape((-1,))
+    return x & y
+
+
+@implements_nfunc('Or')
+@njit(cache=True)
+def Or(x, y):
+    x = np.asarray(x).reshape((-1,))
+    return x | y
+
+
+@implements_nfunc('Not')
+@njit(cache=True)
+def Not(x):
+    x = np.asarray(x).reshape((-1,))
+    return np.ones_like(x) - x
+
+
+@implements_nfunc('Diag')
+def diag(x) -> np.ndarray:
+    """
+    Generate diagonal matrix of given vector X
+    :PARAM X: vector
+    :return: diagonal matrix
+    """
+    if not isinstance(x, np.ndarray):
+        return diags(x.toarray().reshape(-1, ), 0, format='csc')
+    else:
+        return np.diagflat(x)
+
+
+@implements_nfunc('dConv_s')
+def DT_conv(*args, method='conv') -> np.ndarray:
+    r"""
+    Perform the convolutions in DT computations.
+
+    Explanation
+    ===========
+
+
+
+    Parameters
+    ==========
+
+    args : np.ndarray
+
+        DT series.
+
+    method : str
+
+        the method used to compute DT convolution
+
+    """
+    if len(args) <= 2 and method == 'conv':  # if input two vectors, then use scalar multiplications and additions
+        x = args[0].reshape((1, -1))
+        y = np.flip(args[1].reshape((-1, 1)), 0)
+        return x @ y
+
+    if len(args) > 2 or method == 'fft':  # if input more than three vectors, use fft and ifft
+        k = args[0].shape[0]
+        y = []
+        m = 2 * (k - 1) + 1  # ensure that we have enough function values to recover the coefficients by ifft
+        n = np.ceil(np.log2(k))  # fft is the fastest when the length of the series is the power of 2
+        for arg in args:
+            # extend the length of the vector to the power of 2
+            arg = np.pad(arg, (0, int(np.maximum(m, n) - k)), constant_values=0)
+            y += [np.fft.fft(arg)]
+        return np.array(np.real(np.fft.ifft(reduce(lambda a, b: a * b, y))[k - 1]))
+
+
+@implements_nfunc('dLinspace')
+def linspace(start, end) -> np.ndarray:
+    r"""
+
+    Parameters
+    ==========
+
+    start:
+
+
+
+    end:
+
+
+
+    """
+    return np.arange(start, end, dtype=int)[:, np.newaxis]
```

### Comparing `solverz-0.0.1rc1/Solverz/num_api/numjac.py` & `solverz-0.0.1rc2/Solverz/num_api/numjac.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import numpy as np
-from scipy.sparse import csc_array
-
-
-def numjac(F, t, y, Fty, thresh, S, g, vecon, central_diff):
-    # Add t to the end of y and adjust thresh accordingly
-    y = np.append(y, t)
-    thresh = np.append(thresh, 1.0e-8)  # For df/dt
-
-    facmax = 0.1
-    ny = len(y)
-    fac = np.sqrt(np.finfo(float).eps) + np.zeros(ny)
-    yscale = np.maximum(0.1 * np.abs(y), thresh)
-    del_ = (y + fac * yscale) - y
-    jj = np.where(del_ == 0)[0]
-
-    for j in jj:
-        while True:
-            if fac[j] < facmax:
-                fac[j] = min(100 * fac[j], facmax)
-                del_[j] = (y[j] + fac[j] * yscale[j]) - y[j]
-                if del_[j] != 0:
-                    break
-            else:
-                del_[j] = thresh[j]
-                break
-
-    if not vecon:
-        nfevals = ny
-        df = np.zeros((ny - 1, ny))
-
-        for jj in range(0, ny):
-            ydel = y.copy()
-            ydel[jj] += del_[jj]
-            t = ydel[-1]
-            ydel = ydel[:-1]
-
-            if central_diff:
-                ydel_1 = y.copy()
-                ydel_1[jj] -= del_[jj]
-                t_1 = ydel_1[-1]
-                ydel_1 = ydel_1[:-1]
-                df[:, jj] = (F(t, ydel) - F(t_1, ydel_1)) / (2 * del_[jj])
-                nfevals += 1
-            else:
-                df[:, jj] = (F(t, ydel) - Fty) / del_[jj]
-    else:
-        # Vectorized function F
-        raise NotImplementedError("Vectorized function F handling is not implemented.")
-
-    # Convert df to sparse matrix dFdyt
-    dFdyt = csc_array(df)
-
-    return Fty, dFdyt, nfevals
-
-
-def numjac_ae(F, y, thresh):
-    # Add t to the end of y and adjust thresh accordingly
-
-    facmax = 0.1
-    ny = len(y)
-    fac = np.sqrt(np.finfo(float).eps) + np.zeros(ny)
-    yscale = np.maximum(0.1 * np.abs(y), thresh)
-    del_ = (y + fac * yscale) - y
-    jj = np.where(del_ == 0)[0]
-
-    for j in jj:
-        while True:
-            if fac[j] < facmax:
-                fac[j] = min(100 * fac[j], facmax)
-                del_[j] = (y[j] + fac[j] * yscale[j]) - y[j]
-                if del_[j] != 0:
-                    break
-            else:
-                del_[j] = thresh[j]
-                break
-
-    nfevals = ny
-    df = np.zeros((ny, ny))
-
-    for jj in range(0, ny):
-        ydel = y.copy()
-        ydel[jj] += del_[jj]
-
-        ydel_1 = y.copy()
-        ydel_1[jj] -= del_[jj]
-        df[:, jj] = (F(ydel) - F(ydel_1)) / (2 * del_[jj])
-        nfevals += 1
-
-    # Convert df to sparse matrix dFdyt
-    dFdyt = csc_array(df)
-
-    return dFdyt, nfevals
+import numpy as np
+from scipy.sparse import csc_array
+
+
+def numjac(F, t, y, Fty, thresh, S, g, vecon, central_diff):
+    # Add t to the end of y and adjust thresh accordingly
+    y = np.append(y, t)
+    thresh = np.append(thresh, 1.0e-8)  # For df/dt
+
+    facmax = 0.1
+    ny = len(y)
+    fac = np.sqrt(np.finfo(float).eps) + np.zeros(ny)
+    yscale = np.maximum(0.1 * np.abs(y), thresh)
+    del_ = (y + fac * yscale) - y
+    jj = np.where(del_ == 0)[0]
+
+    for j in jj:
+        while True:
+            if fac[j] < facmax:
+                fac[j] = min(100 * fac[j], facmax)
+                del_[j] = (y[j] + fac[j] * yscale[j]) - y[j]
+                if del_[j] != 0:
+                    break
+            else:
+                del_[j] = thresh[j]
+                break
+
+    if not vecon:
+        nfevals = ny
+        df = np.zeros((ny - 1, ny))
+
+        for jj in range(0, ny):
+            ydel = y.copy()
+            ydel[jj] += del_[jj]
+            t = ydel[-1]
+            ydel = ydel[:-1]
+
+            if central_diff:
+                ydel_1 = y.copy()
+                ydel_1[jj] -= del_[jj]
+                t_1 = ydel_1[-1]
+                ydel_1 = ydel_1[:-1]
+                df[:, jj] = (F(t, ydel) - F(t_1, ydel_1)) / (2 * del_[jj])
+                nfevals += 1
+            else:
+                df[:, jj] = (F(t, ydel) - Fty) / del_[jj]
+    else:
+        # Vectorized function F
+        raise NotImplementedError("Vectorized function F handling is not implemented.")
+
+    # Convert df to sparse matrix dFdyt
+    dFdyt = csc_array(df)
+
+    return Fty, dFdyt, nfevals
+
+
+def numjac_ae(F, y, thresh):
+    # Add t to the end of y and adjust thresh accordingly
+
+    facmax = 0.1
+    ny = len(y)
+    fac = np.sqrt(np.finfo(float).eps) + np.zeros(ny)
+    yscale = np.maximum(0.1 * np.abs(y), thresh)
+    del_ = (y + fac * yscale) - y
+    jj = np.where(del_ == 0)[0]
+
+    for j in jj:
+        while True:
+            if fac[j] < facmax:
+                fac[j] = min(100 * fac[j], facmax)
+                del_[j] = (y[j] + fac[j] * yscale[j]) - y[j]
+                if del_[j] != 0:
+                    break
+            else:
+                del_[j] = thresh[j]
+                break
+
+    nfevals = ny
+    df = np.zeros((ny, ny))
+
+    for jj in range(0, ny):
+        ydel = y.copy()
+        ydel[jj] += del_[jj]
+
+        ydel_1 = y.copy()
+        ydel_1[jj] -= del_[jj]
+        df[:, jj] = (F(ydel) - F(ydel_1)) / (2 * del_[jj])
+        nfevals += 1
+
+    # Convert df to sparse matrix dFdyt
+    dFdyt = csc_array(df)
+
+    return dFdyt, nfevals
```

### Comparing `solverz-0.0.1rc1/Solverz/num_api/test/test_Array.py` & `solverz-0.0.1rc2/Solverz/num_api/test/test_Array.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import numpy as np
-from scipy.sparse import csc_array
-
-from Solverz.num_api.Array import Array
-
-
-def test_Array():
-    # input as number
-    x1 = 1
-    assert Array(x1, dim=1, dtype=float).__repr__() == 'array([1.])'
-    assert Array(x1, dim=2, dtype=float).__repr__() == 'array([[1.]])'
-    assert Array(x1, dim=2, sparse=False, dtype=float).__repr__() == 'array([[1.]])'
-    assert Array(x1, dim=2, sparse=True, dtype=float).__str__() == '  (0, 0)\t1.0'
-
-    # input as list
-    x2 = [1, 2, 3]
-    assert Array(x2, dim=1, dtype=float).__repr__() == 'array([1., 2., 3.])'
-    assert Array(x2, dim=2, dtype=int).__str__() == '[[1]\n [2]\n [3]]'
-    assert Array(x2, dim=2, sparse=False, dtype=float).__str__() == '[[1.]\n [2.]\n [3.]]'
-    try:
-        Array(x2, dim=1, sparse=True)
-    except ValueError as e:
-        assert e.args[0] == 'Cannot create sparse matrix with dim: 1'
-    assert Array(x2, dim=2, sparse=True, dtype=float).__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (2, 0)\t3.0'
-
-    x2 = [[1, 0], [2, 9], [0, 3]]
-    try:
-        Array(x2, dim=1, dtype=float)
-    except ValueError as e:
-        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
-
-    assert Array(x2, dtype=float).__str__() == '[[1. 0.]\n [2. 9.]\n [0. 3.]]'
-
-    # input as object
-    x3 = [slice]
-    try:
-        Array(x3, dim=1, dtype=float)
-    except TypeError as e:
-        assert e.args[0] == 'Unsupported data type object'
-
-    # input as csc_array
-    indptr = np.array([0, 2, 3, 6])
-    indices = np.array([0, 2, 2, 0, 1, 2])
-    data = np.array([1, 2, 3, 4, 5, 6])
-    x4 = csc_array((data, indices, indptr), shape=(3, 3))
-    try:
-        Array(x4, dim=1)
-    except ValueError as e:
-        assert e.args[0] == 'csc_array input while dim set to be 1'
-    try:
-        Array(x4, sparse=False)
-    except TypeError as e:
-        assert e.args[0] == 'csc_array input while sparse arg set to be False'
-
-    # input as numpy.ndarray
-    x4 = np.array([[1, 0], [2, 9], [0, 3]])
-    assert Array(x4, sparse=True).__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (1, 1)\t9.0\n  (2, 1)\t3.0'
-    try:
-        Array(x4, dim=1, sparse=True)
-    except ValueError as e:
-        assert e.args[0] == 'Cannot create sparse matrix with dim: 1'
-
-    assert Array(np.array([1.0, 2.0, 3.0]), dtype=int, dim=2).__str__() == '[[1]\n [2]\n [3]]'
-    assert Array(np.array([1.0, 2.0, 3.0]), dtype=int, dim=1).__str__() == '[1 2 3]'
-    assert Array(np.array([1.0, 2.0, 3.0]),
-                 dtype=int,
-                 dim=2,
-                 sparse=True).__str__() == '  (0, 0)\t1\n  (1, 0)\t2\n  (2, 0)\t3'
+import numpy as np
+from scipy.sparse import csc_array
+
+from Solverz.num_api.Array import Array
+
+
+def test_Array():
+    # input as number
+    x1 = 1
+    assert Array(x1, dim=1, dtype=float).__repr__() == 'array([1.])'
+    assert Array(x1, dim=2, dtype=float).__repr__() == 'array([[1.]])'
+    assert Array(x1, dim=2, sparse=False, dtype=float).__repr__() == 'array([[1.]])'
+    assert Array(x1, dim=2, sparse=True, dtype=float).__str__() == '  (0, 0)\t1.0'
+
+    # input as list
+    x2 = [1, 2, 3]
+    assert Array(x2, dim=1, dtype=float).__repr__() == 'array([1., 2., 3.])'
+    assert Array(x2, dim=2, dtype=int).__str__() == '[[1]\n [2]\n [3]]'
+    assert Array(x2, dim=2, sparse=False, dtype=float).__str__() == '[[1.]\n [2.]\n [3.]]'
+    try:
+        Array(x2, dim=1, sparse=True)
+    except ValueError as e:
+        assert e.args[0] == 'Cannot create sparse matrix with dim: 1'
+    assert Array(x2, dim=2, sparse=True, dtype=float).__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (2, 0)\t3.0'
+
+    x2 = [[1, 0], [2, 9], [0, 3]]
+    try:
+        Array(x2, dim=1, dtype=float)
+    except ValueError as e:
+        assert e.args[0] == 'Input list dim 2 higher than dim set to be 1'
+
+    assert Array(x2, dtype=float).__str__() == '[[1. 0.]\n [2. 9.]\n [0. 3.]]'
+
+    # input as object
+    x3 = [slice]
+    try:
+        Array(x3, dim=1, dtype=float)
+    except TypeError as e:
+        assert e.args[0] == 'Unsupported data type object'
+
+    # input as csc_array
+    indptr = np.array([0, 2, 3, 6])
+    indices = np.array([0, 2, 2, 0, 1, 2])
+    data = np.array([1, 2, 3, 4, 5, 6])
+    x4 = csc_array((data, indices, indptr), shape=(3, 3))
+    try:
+        Array(x4, dim=1)
+    except ValueError as e:
+        assert e.args[0] == 'csc_array input while dim set to be 1'
+    try:
+        Array(x4, sparse=False)
+    except TypeError as e:
+        assert e.args[0] == 'csc_array input while sparse arg set to be False'
+
+    # input as numpy.ndarray
+    x4 = np.array([[1, 0], [2, 9], [0, 3]])
+    assert Array(x4, sparse=True).__str__() == '  (0, 0)\t1.0\n  (1, 0)\t2.0\n  (1, 1)\t9.0\n  (2, 1)\t3.0'
+    try:
+        Array(x4, dim=1, sparse=True)
+    except ValueError as e:
+        assert e.args[0] == 'Cannot create sparse matrix with dim: 1'
+
+    assert Array(np.array([1.0, 2.0, 3.0]), dtype=int, dim=2).__str__() == '[[1]\n [2]\n [3]]'
+    assert Array(np.array([1.0, 2.0, 3.0]), dtype=int, dim=1).__str__() == '[1 2 3]'
+    assert Array(np.array([1.0, 2.0, 3.0]),
+                 dtype=int,
+                 dim=2,
+                 sparse=True).__str__() == '  (0, 0)\t1\n  (1, 0)\t2\n  (2, 0)\t3'
```

### Comparing `solverz-0.0.1rc1/Solverz/num_api/test/test_custom_func.py` & `solverz-0.0.1rc2/Solverz/num_api/test/test_custom_func.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import numpy as np
-
-from Solverz.num_api.custom_function import SolIn, SolLessThan, SolGreaterThan, And, Or, Not
-
-
-def test_in():
-    a = np.array([1, 2, 3.0])
-    b = np.array([3, 2, 1.0])
-    np.testing.assert_allclose(SolIn(a, 2, 2), np.array([0, 1, 0]))
-    np.testing.assert_allclose(SolIn(a, 1, 3), np.array([1, 1, 1]))
-    np.testing.assert_allclose(SolIn(a, 1, 2.5), np.array([1, 1, 0]))
-    np.testing.assert_allclose(SolIn(5, 4, 4.5), np.array([0]))
-
-
-def test_gt():
-    a = np.array([1, 2, 3.0])
-    b = np.array([3, 2, 1.0])
-    np.testing.assert_allclose(SolGreaterThan(a, b), np.array([0, 0, 1]))
-    np.testing.assert_allclose(SolGreaterThan(5, 4), np.array([1]))
-    np.testing.assert_allclose(SolGreaterThan(5, 6), np.array([0]))
-
-
-def test_lt():
-    a = np.array([1, 2, 3.0])
-    b = np.array([3, 2, 1.0])
-    np.testing.assert_allclose(SolLessThan(a, b), np.array([1, 0, 0]))
-    np.testing.assert_allclose(SolLessThan(5, 4), np.array([0]))
-    np.testing.assert_allclose(SolLessThan(5, 6), np.array([1]))
-
-
-def test_and():
-    a = np.array([1, 0, 1])
-    b = np.array([1, 1, 0])
-    np.testing.assert_allclose(And(a, b), np.array([1, 0, 0]))
-    np.testing.assert_allclose(And(1, 0), np.array([0]))
-    np.testing.assert_allclose(And(1, 1), np.array([1]))
-
-
-def test_or():
-    a = np.array([1, 0, 1])
-    b = np.array([1, 1, 0])
-    np.testing.assert_allclose(Or(a, b), np.array([1, 1, 1]))
-    np.testing.assert_allclose(Or(1, 0), np.array([1]))
-    np.testing.assert_allclose(Or(0, 0), np.array([0]))
-
-
-def test_not():
-    a = np.array([1, 0, 1])
-    np.testing.assert_allclose(Not(a), np.array([0, 1, 0]))
-    np.testing.assert_allclose(Not(1), np.array([0]))
-    np.testing.assert_allclose(Not(0), np.array([1]))
+import numpy as np
+
+from Solverz.num_api.custom_function import SolIn, SolLessThan, SolGreaterThan, And, Or, Not
+
+
+def test_in():
+    a = np.array([1, 2, 3.0])
+    b = np.array([3, 2, 1.0])
+    np.testing.assert_allclose(SolIn(a, 2, 2), np.array([0, 1, 0]))
+    np.testing.assert_allclose(SolIn(a, 1, 3), np.array([1, 1, 1]))
+    np.testing.assert_allclose(SolIn(a, 1, 2.5), np.array([1, 1, 0]))
+    np.testing.assert_allclose(SolIn(5, 4, 4.5), np.array([0]))
+
+
+def test_gt():
+    a = np.array([1, 2, 3.0])
+    b = np.array([3, 2, 1.0])
+    np.testing.assert_allclose(SolGreaterThan(a, b), np.array([0, 0, 1]))
+    np.testing.assert_allclose(SolGreaterThan(5, 4), np.array([1]))
+    np.testing.assert_allclose(SolGreaterThan(5, 6), np.array([0]))
+
+
+def test_lt():
+    a = np.array([1, 2, 3.0])
+    b = np.array([3, 2, 1.0])
+    np.testing.assert_allclose(SolLessThan(a, b), np.array([1, 0, 0]))
+    np.testing.assert_allclose(SolLessThan(5, 4), np.array([0]))
+    np.testing.assert_allclose(SolLessThan(5, 6), np.array([1]))
+
+
+def test_and():
+    a = np.array([1, 0, 1])
+    b = np.array([1, 1, 0])
+    np.testing.assert_allclose(And(a, b), np.array([1, 0, 0]))
+    np.testing.assert_allclose(And(1, 0), np.array([0]))
+    np.testing.assert_allclose(And(1, 1), np.array([1]))
+
+
+def test_or():
+    a = np.array([1, 0, 1])
+    b = np.array([1, 1, 0])
+    np.testing.assert_allclose(Or(a, b), np.array([1, 1, 1]))
+    np.testing.assert_allclose(Or(1, 0), np.array([1]))
+    np.testing.assert_allclose(Or(0, 0), np.array([0]))
+
+
+def test_not():
+    a = np.array([1, 0, 1])
+    np.testing.assert_allclose(Not(a), np.array([0, 1, 0]))
+    np.testing.assert_allclose(Not(1), np.array([0]))
+    np.testing.assert_allclose(Not(0), np.array([1]))
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/fdesolver.py` & `solverz-0.0.1rc2/Solverz/solvers/fdesolver.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-from typing import List, Union
-from numbers import Number
-import numpy as np
-import tqdm
-
-from Solverz.num_api.num_eqn import nFDAE, nAE
-from Solverz.solvers.nlaesolver import nr_method
-from Solverz.solvers.stats import Stats
-from Solverz.solvers.option import Opt
-from Solverz.solvers.parser import fdae_io_parser
-from Solverz.solvers.solution import daesol
-
-
-@fdae_io_parser
-def fdae_solver(fdae: nFDAE,
-                tspan: List | np.ndarray,
-                u0: np.ndarray,
-                opt: Opt = None):
-    r"""
-    The general solver of FDAE.
-
-    Parameters
-    ==========
-
-    fdae : nFDAE
-        Numerical FDAE object.
-
-    tspan : List | np.ndarray
-        An array specifying t0 and tend
-
-    u0 : np.ndarray
-        The initial values of variables
-
-    opt : Opt
-        The solver options, including:
-
-        - step_size: 1e-3(default)|float
-            The step size
-        - ite_tol: 1e-8(default)|float
-            The error tolerance of inner Newton iterations.
-
-    Returns
-    =======
-
-    sol : daesol
-        The daesol object.
-
-    """
-    stats = Stats(scheme='FDE solver')
-    if opt is None:
-        opt = Opt(stats=True)
-    dt = opt.step_size
-    tspan = np.array(tspan)
-    T_initial = tspan[0]
-    tend = tspan[-1]
-    if (tend / dt) > 10000:
-        nstep = np.ceil(tend / dt).astype(int) + 1000
-    else:
-        nstep = int(10000)
-    nt = 0
-    tt = T_initial
-    t0 = tt
-    uround = np.spacing(1.0)
-
-    u = np.zeros((nstep, u0.shape[0]))
-    u[0, :] = u0
-    T = np.zeros((nstep,))
-    T[0] = t0
-    if opt.pbar:
-        bar = tqdm.tqdm(total=tend)
-
-    done = False
-    p = fdae.p
-    while not done:
-
-        if tt + dt >= tend:
-            dt = tend - tt
-        else:
-            dt = np.minimum(dt, 0.5 * (tend - tt))
-
-        if done:
-            break
-
-        if fdae.nstep == 1:
-            ae = nAE(lambda y_, p_: fdae.F(t0 + dt, y_, p_, u0),
-                     lambda y_, p_: fdae.J(t0 + dt, y_, p_, u0),
-                     p)
-        else:
-            raise NotImplementedError("Multistep FDAE not implemented!")
-
-        sol = nr_method(ae, u0, Opt(ite_tol=opt.ite_tol, stats=True))
-        u1 = sol.y
-        ite = sol.stats
-        stats.ndecomp = stats.ndecomp + ite
-        stats.nfeval = stats.nfeval + ite + 1
-        if ite >= 100:
-            print(f"FDAE solver broke at time={tt} due to non-convergence")
-            break
-
-        tt = tt + dt
-        nt = nt + 1
-        u[nt] = u1
-        T[nt] = tt
-        if opt.pbar:
-            bar.update(dt)
-        t0 = tt
-        u0 = u1
-
-        if np.abs(tend - tt) < uround:
-            done = True
-
-    u = u[0:nt + 1]
-    T = T[0:nt + 1]
-    stats.nstep = nt
-    if opt.pbar:
-        bar.close()
-    return daesol(T, u, stats=stats)
-
-
-def fdae_ss_solver(fdae: nFDAE,
-                   u0: np.ndarray,
-                   dt,
-                   T0: Number = 0,
-                   opt: Opt = None):
-    stats = Stats(scheme='FDE solver')
-    if opt is None:
-        opt = Opt()
-
-    nstep = 10000
-    nt = 0
-    tt = T0
-    t0 = tt
-
-    u = np.zeros((nstep, u0.shape[0]))
-    u[0, :] = u0
-
-    done = False
-    p = fdae.p
-    dev0 = 1
-    while not done:
-
-        if done:
-            break
-
-        if fdae.nstep == 1:
-            ae = nAE(lambda y_, p_: fdae.F(t0 + dt, y_, p_, u0),
-                     lambda y_, p_: fdae.J(t0 + dt, y_, p_, u0),
-                     p)
-        else:
-            raise NotImplementedError("Multistep FDAE not implemented!")
-
-        u1, ite = nr_method(ae, u0, tol=opt.ite_tol, stats=True)
-        stats.ndecomp = stats.ndecomp + ite
-        stats.nfeval = stats.nfeval + ite + 1
-
-        tt = tt + dt
-        nt = nt + 1
-        u[nt] = u1
-
-        du = u1 - u0
-        args = u1 != 0
-        dev1 = np.max(np.abs(du[args] / u1[args]))
-        if dev1 < 1e-7:
-            done = True
-
-        u0 = u1
-        t0 = tt
-        # if dev1 <= dev0:
-        #     dt = dt * 1.1
-        dev0 = dev1
-
-    u = u[0:nt + 1]
-    stats.nstep = nt
-
-    return u, stats
+from typing import List, Union
+from numbers import Number
+import numpy as np
+import tqdm
+
+from Solverz.num_api.num_eqn import nFDAE, nAE
+from Solverz.solvers.nlaesolver import nr_method
+from Solverz.solvers.stats import Stats
+from Solverz.solvers.option import Opt
+from Solverz.solvers.parser import fdae_io_parser
+from Solverz.solvers.solution import daesol
+
+
+@fdae_io_parser
+def fdae_solver(fdae: nFDAE,
+                tspan: List | np.ndarray,
+                u0: np.ndarray,
+                opt: Opt = None):
+    r"""
+    The general solver of FDAE.
+
+    Parameters
+    ==========
+
+    fdae : nFDAE
+        Numerical FDAE object.
+
+    tspan : List | np.ndarray
+        An array specifying t0 and tend
+
+    u0 : np.ndarray
+        The initial values of variables
+
+    opt : Opt
+        The solver options, including:
+
+        - step_size: 1e-3(default)|float
+            The step size
+        - ite_tol: 1e-8(default)|float
+            The error tolerance of inner Newton iterations.
+
+    Returns
+    =======
+
+    sol : daesol
+        The daesol object.
+
+    """
+    stats = Stats(scheme='FDE solver')
+    if opt is None:
+        opt = Opt(stats=True)
+    dt = opt.step_size
+    tspan = np.array(tspan)
+    T_initial = tspan[0]
+    tend = tspan[-1]
+    if (tend / dt) > 10000:
+        nstep = np.ceil(tend / dt).astype(int) + 1000
+    else:
+        nstep = int(10000)
+    nt = 0
+    tt = T_initial
+    t0 = tt
+    uround = np.spacing(1.0)
+
+    u = np.zeros((nstep, u0.shape[0]))
+    u[0, :] = u0
+    T = np.zeros((nstep,))
+    T[0] = t0
+    if opt.pbar:
+        bar = tqdm.tqdm(total=tend)
+
+    done = False
+    p = fdae.p
+    while not done:
+
+        if tt + dt >= tend:
+            dt = tend - tt
+        else:
+            dt = np.minimum(dt, 0.5 * (tend - tt))
+
+        if done:
+            break
+
+        if fdae.nstep == 1:
+            ae = nAE(lambda y_, p_: fdae.F(t0 + dt, y_, p_, u0),
+                     lambda y_, p_: fdae.J(t0 + dt, y_, p_, u0),
+                     p)
+        else:
+            raise NotImplementedError("Multistep FDAE not implemented!")
+
+        sol = nr_method(ae, u0, Opt(ite_tol=opt.ite_tol, stats=True))
+        u1 = sol.y
+        ite = sol.stats
+        stats.ndecomp = stats.ndecomp + ite
+        stats.nfeval = stats.nfeval + ite + 1
+        if ite >= 100:
+            print(f"FDAE solver broke at time={tt} due to non-convergence")
+            break
+
+        tt = tt + dt
+        nt = nt + 1
+        u[nt] = u1
+        T[nt] = tt
+        if opt.pbar:
+            bar.update(dt)
+        t0 = tt
+        u0 = u1
+
+        if np.abs(tend - tt) < uround:
+            done = True
+
+    u = u[0:nt + 1]
+    T = T[0:nt + 1]
+    stats.nstep = nt
+    if opt.pbar:
+        bar.close()
+    return daesol(T, u, stats=stats)
+
+
+def fdae_ss_solver(fdae: nFDAE,
+                   u0: np.ndarray,
+                   dt,
+                   T0: Number = 0,
+                   opt: Opt = None):
+    stats = Stats(scheme='FDE solver')
+    if opt is None:
+        opt = Opt()
+
+    nstep = 10000
+    nt = 0
+    tt = T0
+    t0 = tt
+
+    u = np.zeros((nstep, u0.shape[0]))
+    u[0, :] = u0
+
+    done = False
+    p = fdae.p
+    dev0 = 1
+    while not done:
+
+        if done:
+            break
+
+        if fdae.nstep == 1:
+            ae = nAE(lambda y_, p_: fdae.F(t0 + dt, y_, p_, u0),
+                     lambda y_, p_: fdae.J(t0 + dt, y_, p_, u0),
+                     p)
+        else:
+            raise NotImplementedError("Multistep FDAE not implemented!")
+
+        u1, ite = nr_method(ae, u0, tol=opt.ite_tol, stats=True)
+        stats.ndecomp = stats.ndecomp + ite
+        stats.nfeval = stats.nfeval + ite + 1
+
+        tt = tt + dt
+        nt = nt + 1
+        u[nt] = u1
+
+        du = u1 - u0
+        args = u1 != 0
+        dev1 = np.max(np.abs(du[args] / u1[args]))
+        if dev1 < 1e-7:
+            done = True
+
+        u0 = u1
+        t0 = tt
+        # if dev1 <= dev0:
+        #     dt = dt * 1.1
+        dev0 = dev1
+
+    u = u[0:nt + 1]
+    stats.nstep = nt
+
+    return u, stats
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/option.py` & `solverz-0.0.1rc2/Solverz/solvers/option.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Callable
-
-
-class Opt:
-    def __init__(self,
-                 atol=1e-6,
-                 rtol=1e-3,
-                 f_savety=0.9,
-                 facmax=6,
-                 fac1=0.2,
-                 fac2=6,
-                 scheme='rodas4',
-                 ite_tol=1e-5,
-                 fix_h: bool = False,
-                 hinit=None,
-                 hmax=None,
-                 pbar=False,
-                 stats=False,
-                 step_size=1e-3,
-                 event: Callable = None,
-                 event_duration=1e-8):
-        self.atol = atol
-        self.rtol = rtol
-        self.f_savety = f_savety
-        self.facmax = facmax
-        self.fac1 = fac1
-        self.fac2 = fac2
-        self.fix_h = fix_h  # To force the step sizes to be invariant. This is not robust.
-        self.hinit = hinit
-        self.hmax = hmax
-        self.scheme = scheme
-        self.pbar = pbar
-        self.ite_tol = ite_tol  # tol for iterative solver
-        self.stats = stats
-        self.step_size = step_size
-        self.event = event
-        self.event_duration = event_duration
+from typing import Callable
+
+
+class Opt:
+    def __init__(self,
+                 atol=1e-6,
+                 rtol=1e-3,
+                 f_savety=0.9,
+                 facmax=6,
+                 fac1=0.2,
+                 fac2=6,
+                 scheme='rodas4',
+                 ite_tol=1e-5,
+                 fix_h: bool = False,
+                 hinit=None,
+                 hmax=None,
+                 pbar=False,
+                 stats=False,
+                 step_size=1e-3,
+                 event: Callable = None,
+                 event_duration=1e-8):
+        self.atol = atol
+        self.rtol = rtol
+        self.f_savety = f_savety
+        self.facmax = facmax
+        self.fac1 = fac1
+        self.fac2 = fac2
+        self.fix_h = fix_h  # To force the step sizes to be invariant. This is not robust.
+        self.hinit = hinit
+        self.hmax = hmax
+        self.scheme = scheme
+        self.pbar = pbar
+        self.ite_tol = ite_tol  # tol for iterative solver
+        self.stats = stats
+        self.step_size = step_size
+        self.event = event
+        self.event_duration = event_duration
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/daesolver/rodas.py` & `solverz-0.0.1rc2/Solverz/solvers/daesolver/rodas.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,486 +1,486 @@
-import warnings
-
-from Solverz.solvers.daesolver.utilities import *
-
-
-@dae_io_parser
-def Rodas(dae: nDAE,
-          tspan: List | np.ndarray,
-          y0: np.ndarray,
-          opt: Opt = None):
-    r"""
-    The stiffly accurate Rosenbrock methods including Rodas4 [1]_, Rodasp [2]_, Rodas5p [3]_.
-
-    Parameters
-    ==========
-
-    dae : nDAE
-        Numerical DAE object.
-
-    tspan : List | np.ndarray
-        Either
-        - a list specifying [t0, tend], or
-        - a `np.ndarray` specifying the time nodes that you are concerned about
-
-    y0 : np.ndarray
-        The initial values of variables
-
-    opt : Opt
-        The solver options, including:
-
-        - scheme: 'rodas4'(default)|'rodasp'|'rodas5p'
-            The rodas scheme
-        - rtol: 1e-3(default)|float
-            The relative error tolerance
-        - atol: 1e-6(default)|float
-            The absolute error tolerance
-        - event: Callable
-            The simulation events, with $t$ and $y$ being args,
-            and `value`, `is_terminal` and `direction` being outputs
-        - fixed_h: False(default)|bool
-            To use fixed step size
-        - hinit: None(default)|float
-            Initial step size
-        - hmax: None(default)|float
-            Maximum step size.
-
-    Returns
-    =======
-
-    sol : daesol
-        The daesol object.
-
-
-    References
-    ==========
-
-    .. [1] Hairer and Wanner, Solving Ordinary Differential Equations II , 2nd ed. Berlin, Heidelberg, Germany: Springer-Verlag, 1996.
-    .. [2] Steinebach, Order-reduction of ROW-methods for DAEs and method of lines applications. Preprint-Nr. 1741, FB Mathematik, TH Darmstadt, 1995
-    .. [3] Steinebach, “Construction of rosenbrock-wanner method rodas5p and numerical benchmarks within the julia differential equations package,” BIT, vol. 63, no. 27, Jun 2023.
-    """
-
-    if opt is None:
-        opt = Opt()
-    stats = Stats(opt.scheme)
-
-    rparam = Rodas_param(opt.scheme)
-    vsize = y0.shape[0]
-    tspan = np.array(tspan)
-    tend = tspan[-1]
-    t0 = tspan[0]
-    if opt.hmax is None:
-        opt.hmax = np.abs(tend - t0)
-    nt = 0
-    t = t0
-    hmin = 16 * np.spacing(t0)
-    uround = np.spacing(1.0)
-    T = np.zeros((10001,))
-    T[nt] = t0
-    y = np.zeros((10001, vsize))
-    y0 = DaeIc(dae, y0, t0, opt.rtol)  # check and modify initial values
-    y[0, :] = y0
-
-    dense_output = False
-    n_tspan = len(tspan)
-    told = t0
-    if n_tspan > 2:
-        dense_output = True
-        inext = 1
-        tnext = tspan[inext]
-
-    events = opt.event
-    haveEvent = True if events is not None else False
-
-    if haveEvent:
-        value, isterminal, direction = events(t, y0)
-    stop = 0
-    nevent = -1
-    te = np.zeros((10001,))
-    ye = np.zeros((10001, vsize))
-    ie = np.zeros((10001,))
-
-    # The initial step size
-    if opt.hinit is None:
-        dt = 1e-6 * (tend - t0)
-    else:
-        dt = opt.hinit
-
-    dt = np.maximum(dt, hmin)
-    dt = np.minimum(dt, opt.hmax)
-
-    M = dae.M
-    p = dae.p
-    done = False
-    reject = 0
-    while not done:
-        # step size too small
-        # pass
-
-        if np.abs(dt) < uround:
-            print(f"Error exit of RODAS at time = {t}: step size too small h = {dt}.\n")
-            stats.ret = 'failed'
-            break
-
-        if reject > 100:
-            print(f"Step rejected over 100 times at time = {t}.\n")
-            stats.ret = 'failed'
-            break
-
-        # Stretch the step if within 10% of T-t.
-        if t + dt >= tend:
-            dt = tend - t
-        else:
-            dt = np.minimum(dt, 0.5 * (tend - t))
-
-        if opt.fix_h:
-            dt = opt.hinit
-
-        if done:
-            break
-        K = np.zeros((vsize, rparam.s))
-
-        if reject == 0:
-            J = dae.J(t, y0, p)
-
-        dfdt0 = dt * dfdt(dae, t, y0)
-        rhs = dae.F(t, y0, p) + rparam.g[0] * dfdt0
-        stats.nfeval = stats.nfeval + 1
-
-        try:
-            lu = lu_decomposition(M - dt * rparam.gamma * J)
-        except RuntimeError:
-            break
-        stats.ndecomp = stats.ndecomp + 1
-        K[:, 0] = lu.solve(rhs)
-
-        for j in range(1, rparam.s):
-            sum_1 = K @ rparam.alpha[:, j]
-            sum_2 = K @ rparam.gammatilde[:, j]
-            y1 = y0 + dt * sum_1
-
-            rhs = dae.F(t + dt * rparam.a[j], y1, p) + M @ sum_2 + rparam.g[j] * dfdt0
-            stats.nfeval = stats.nfeval + 1
-            sol = lu.solve(rhs)
-            K[:, j] = sol - sum_2
-
-        sum_1 = K @ (dt * rparam.b)
-        ynew = y0 + sum_1
-        if not opt.fix_h:
-            sum_2 = K @ (dt * rparam.bd)
-            SK = (opt.atol + opt.rtol * abs(ynew)).reshape((-1,))
-            err = np.max(np.abs((sum_1 - sum_2) / SK))
-            if np.any(np.isinf(ynew)) or np.any(np.isnan(ynew)):
-                err = 1.0e6
-                print('Warning Rodas: NaN or Inf occurs.')
-            err = np.maximum(err, 1.0e-6)
-            fac = opt.f_savety / (err ** (1 / rparam.pord))
-            fac = np.minimum(opt.facmax, np.maximum(opt.fac1, fac))
-            dtnew = dt * fac
-        else:
-            err = 1.0
-            dtnew = dt
-
-        if err <= 1.0:
-            reject = 0
-            told = t
-            t = t + dt
-            stats.nstep = stats.nstep + 1
-            # events
-            if haveEvent:
-                valueold = value
-                value, isterminal, direction = events(t, ynew)
-                value_save = value
-                ff = np.where(value * valueold < 0)[0]
-                if ff.size > 0:
-                    for i in ff:
-                        v0 = valueold[i]
-                        v1 = value[i]
-                        detect = 1
-                        if direction[i] < 0 and v0 <= v1:
-                            detect = 0
-                        if direction[i] > 0 and v0 >= v1:
-                            detect = 0
-                        if detect:
-                            iterate = 1
-                            tL = told
-                            tR = t
-                            if np.abs(v1 - v0) > uround:
-                                tevent = told - v0 * dt / (v1 - v0)  # initial guess for tevent
-                            else:
-                                iterate = 0
-                                tevent = t
-                                ynext = ynew
-
-                            tol = 128 * np.max([np.spacing(told), np.spacing(t)])
-                            tol = np.min([tol, np.abs(t - told)])
-                            while iterate > 0:
-                                iterate = iterate + 1
-                                tau = (tevent - told) / dt
-                                ynext = y0 + tau * dt * K @ (
-                                        rparam.b + (tau - 1) * (rparam.c + tau * (rparam.d + tau * rparam.e)))
-                                value, isterminal, direction = events(tevent, ynext)
-                                if v1 * value[i] < 0:
-                                    tL = tevent
-                                    tevent = 0.5 * (tevent + tR)
-                                    v0 = value[i]
-                                elif v0 * value[i] < 0:
-                                    tR = tevent
-                                    tevent = 0.5 * (tL + tevent)
-                                    v1 = value[i]
-                                else:
-                                    iterate = 0
-                                if (tR - tL) < tol:
-                                    iterate = 0
-                                if iterate > 100:
-                                    print(f"Lost Event in interval [{told}, {t}].\n")
-                                    break
-                            if np.abs(tevent - told) < opt.event_duration:
-                                # We're not going to find events closer than tol.
-                                break
-                            t = tevent
-                            ynew = ynext
-                            nevent += 1
-                            te[nevent] = tevent
-                            ie[nevent] = i
-                            ye[nevent] = ynext
-                            value, isterminal, direction = events(tevent, ynext)
-                            value = value_save
-                            if isterminal[i]:
-                                if dense_output:
-                                    if tnext >= tevent:
-                                        tnext = tevent
-                                stop = 1
-                                break
-
-            if dense_output:  # dense_output
-                while t >= tnext > told:
-                    tau = (tnext - told) / dt
-                    ynext = y0 + tau * dt * K @ (rparam.b + (tau - 1) * (rparam.c + tau * (rparam.d + tau * rparam.e)))
-                    nt = nt + 1
-                    T[nt] = tnext
-                    y[nt] = ynext
-
-                    if haveEvent and stop:
-                        if tnext >= tevent:
-                            break
-
-                    inext = inext + 1
-                    if inext <= n_tspan - 1:
-                        tnext = tspan[inext]
-                        if haveEvent and stop:
-                            if tnext >= tevent:
-                                tnext = tevent
-                    else:
-                        tnext = tend + dt
-            else:
-                nt = nt + 1
-                T[nt] = t
-                y[nt] = ynew
-
-            if nt == 10000:
-                warnings.warn("Time steps more than 10000! Rodas breaks. Try input a smaller tspan!")
-                done = True
-
-            if np.abs(tend - t) < uround or stop:
-                done = True
-            y0 = ynew
-            opt.facmax = opt.fac2
-
-        else:
-            reject = reject + 1
-            stats.nreject = stats.nreject + 1
-            opt.facmax = 1
-        dt = np.min([opt.hmax, np.max([hmin, dtnew])])
-
-    T = T[0:nt + 1]
-    y = y[0:nt + 1]
-    if haveEvent:
-        te = te[0:nevent + 1]
-        ye = ye[0:nevent + 1]
-        ie = ie[0:nevent + 1]
-        return daesol(T, y, te, ye, ie, stats)
-    else:
-        return daesol(T, y, stats=stats)
-
-
-class Rodas_param:
-
-    def __init__(self,
-                 scheme: str = 'rodas4'):
-        match scheme:
-            case 'rodas4':
-                self.s = 6
-                self.pord = 4
-                self.alpha = np.zeros((self.s, self.s))
-                self.beta = np.zeros((self.s, self.s))
-                self.g = np.zeros((self.s, 1))
-                self.gamma = 0.25
-                self.alpha[1, 0] = 3.860000000000000e-01
-                self.alpha[2, 0:2] = [1.460747075254185e-01, 6.392529247458190e-02]
-                self.alpha[3, 0:3] = [-3.308115036677222e-01, 7.111510251682822e-01, 2.496604784994390e-01]
-                self.alpha[4, 0:4] = [-4.552557186318003e+00, 1.710181363241323e+00, 4.014347332103149e+00,
-                                      -1.719715090264703e-01]
-                self.alpha[5, 0:5] = [2.428633765466977e+00, -3.827487337647808e-01, -1.855720330929572e+00,
-                                      5.598352992273752e-01,
-                                      2.499999999999995e-01]
-                self.beta[1, 0] = 3.170000000000250e-02
-                self.beta[2, 0:2] = [1.247220225724355e-02, 5.102779774275723e-02]
-                self.beta[3, 0:3] = [1.196037669338736e+00, 1.774947364178279e-01, -1.029732405756564e+00]
-                self.beta[4, 0:4] = [2.428633765466977e+00, -3.827487337647810e-01, -1.855720330929572e+00,
-                                     5.598352992273752e-01]
-                self.beta[5, 0:5] = [3.484442712860512e-01, 2.130136219118989e-01, -1.541025326623184e-01,
-                                     4.713207793914960e-01,
-                                     -1.286761399271284e-01]
-                self.b = np.zeros((6,))
-                self.b[0:5] = self.beta[5, 0:5]
-                self.b[5] = self.gamma
-                self.bd = np.zeros((6,))
-                self.bd[0:4] = self.beta[4, 0:4]
-                self.bd[4] = self.gamma
-                self.c = np.array([-4.786970949443344e+00, -6.966969867338157e-01, 4.491962205414260e+00,
-                                   1.247990161586704e+00, -2.562844308238056e-01, 0])
-                self.d = np.array([1.274202171603216e+01, -1.894421984691950e+00, -1.113020959269748e+01,
-                                   -1.365987420071593e+00, 1.648597281428871e+00, 0])
-                self.e = np.zeros((6,))
-                self.gammatilde = self.beta - self.alpha
-                self.a = np.sum(self.alpha, axis=1)
-                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
-                self.gammatilde = self.gammatilde / self.gamma
-                self.alpha = self.alpha.T
-                self.gammatilde = self.gammatilde.T
-            case 'rodasp':
-                self.s = 6
-                self.pord = 4
-                self.alpha = np.zeros((self.s, self.s))
-                self.beta = np.zeros((self.s, self.s))
-                self.gamma = 0.25
-                self.alpha[1, 0] = 0.75
-                self.alpha[2, 0:2] = [0.0861204008141522, 0.123879599185848]
-                self.alpha[3, 0:3] = [0.774934535507324, 0.149265154950868, -0.294199690458192]
-                self.alpha[4, 0:4] = [5.30874668264614, 1.33089214003727, -5.37413781165556, -0.265501011027850]
-                self.alpha[5, 0:5] = [-1.76443764877448, -0.474756557206303, 2.36969184691580, 0.619502359064983,
-                                      0.250000000000000]
-                self.beta[1, 0] = 0.0
-                self.beta[2, 0:2] = [-0.0493920000000000, -0.0141120000000000]
-                self.beta[3, 0:3] = [-0.482049469387756, -0.100879555555556, 0.926729024943312]
-                self.beta[4, 0:4] = [-1.76443764877448, -0.474756557206303, 2.36969184691580, 0.619502359064983]
-                self.beta[5, 0:5] = [-0.0803683707891135, -0.0564906135924476, 0.488285630042799, 0.505716211481619,
-                                     -0.107142857142857]
-                self.b = np.zeros((6,))
-                self.b[0:5] = self.beta[5, 0:5]
-                self.b[5] = self.gamma
-                self.bd = np.zeros((6,))
-                self.bd[0:4] = self.beta[4, 0:4]
-                self.bd[4] = self.gamma
-                self.c = np.array([-40.98639964388325,
-                                   -10.36668980524365,
-                                   44.66751816647147,
-                                   4.13001572709988,
-                                   2.55555555555556,
-                                   0])
-                self.d = np.array([73.75018659483291,
-                                   18.54063799119389,
-                                   -81.66902074619779,
-                                   -6.84402606205123,
-                                   -3.77777777777778,
-                                   0])
-                self.e = np.zeros((6,))
-                self.gammatilde = self.beta - self.alpha
-                self.a = np.sum(self.alpha, axis=1)
-                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
-                self.gammatilde = self.gammatilde / self.gamma
-                self.alpha = self.alpha.T
-                self.gammatilde = self.gammatilde.T
-            case 'rodas5p':
-                self.s = 8
-                self.pord = 5
-                self.a = np.zeros((self.s,))
-                self.g = np.zeros((self.s,))
-                self.alpha = np.array([
-                    [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [0.6358126895828704, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [0.31242290829798824, 0.09715693104176527, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [1.3140825753299277, 1.8583084874257945, -2.1954603902496506, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [0.42153145792835994, 0.25386966273009, -0.2365547905326239, -0.010005969169959593, 0.0, 0.0, 0.0,
-                     0.0],
-                    [1.712028062121536, 2.4456320333807953, -3.117254839827603, -0.04680538266310614,
-                     0.006400126988377645, 0.0, 0.0, 0.0],
-                    [-0.9993030215739269, -1.5559156221686088, 3.1251564324842267, 0.24141811637172583,
-                     -0.023293468307707062, 0.21193756319429014, 0.0, 0.0],
-                    [-0.003487250199264519, -0.1299669712056423, 1.525941760806273, 1.1496140949123888,
-                     -0.7043357115882416, -1.0497034859198033, 0.21193756319429014, 0.0]
-                ])
-                self.beta = np.array([
-                    [0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [0.0, 0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [-0.10952700614965587, -0.03129343032847311, 0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0],
-                    [1.701745865188331, -0.15675801606110462, 1.024650547472829, 0.21193756319429014, 0.0, 0.0, 0.0,
-                     0.0],
-                    [3.587261990937329, 1.6112735397639253, -2.378003402448709, -0.2778036907258995,
-                     0.21193756319429014, 0.0, 0.0, 0.0],
-                    [-0.9993030215739269, -1.5559156221686088, 3.1251564324842267, 0.24141811637172583,
-                     -0.023293468307707062, 0.21193756319429014, 0.0, 0.0],
-                    [-0.003487250199264519, -0.1299669712056423, 1.525941760806273, 1.1496140949123888,
-                     -0.7043357115882416, -1.0497034859198033, 0.21193756319429014, 0.0],
-                    [0.12236007991300712, 0.050238881884191906, 1.3238392208663585, 1.2643883758622305,
-                     -0.7904031855871826, -0.9680932754194287, -0.214267660713467, 0.21193756319429014]
-                ])
-                self.c = np.array([-0.8232744916805133, 0.3181483349120214, 0.16922330104086836, -0.049879453396320994,
-                                   0.19831791977261218, 0.31488148287699225, -0.16387506167704194,
-                                   0.036457968151382296])
-                self.d = np.array([-0.6726085201965635, -1.3128972079520966, 9.467244336394248, 12.924520918142036,
-                                   -9.002714541842755, -11.404611057341922, -1.4210850083209667,
-                                   1.4221510811179898])
-                self.e = np.array([1.4025185206933914, 0.9860299407499886, -11.006871867857507, -14.112585514422294,
-                                   9.574969612795117, 12.076626078349426, 2.114222828697341,
-                                   -1.0349095990054304])
-                self.gamma = self.beta[0, 0]
-                self.b = np.append(self.beta[7, :-1], [self.gamma])
-                self.bd = np.append(self.beta[6, :-2], [self.gamma, 0])
-                self.gammatilde = self.beta - self.gamma * np.eye(self.s) - self.alpha
-                for i in range(self.s):
-                    self.a[i] = np.sum(self.alpha[i, :])
-                    self.g[i] = np.sum(self.gammatilde[i, :]) + self.gamma
-                self.gammatilde /= self.gamma
-                self.alpha = self.alpha.T
-                self.gammatilde = self.gammatilde.T
-            case 'rodas3d':
-                self.s = 4
-                self.pord = 3
-                self.alpha = np.zeros((self.s, self.s))
-                self.beta = np.zeros((self.s, self.s))
-                self.g = np.zeros((self.s, 1))
-                self.gamma = 0.57281606
-                self.alpha[1, 0] = 1.2451051999132263
-                self.alpha[2, 0:2] = [1, 0]
-                self.alpha[3, 0:3] = [0.32630307266483527, 0.10088086733516474, 0.57281606]
-                self.beta[1, 0] = -3.1474142698552949
-                self.beta[2, 0:2] = [0.32630307266483527, 0.10088086733516474]
-                self.beta[3, 0:3] = [0.69775271462407906, 0.056490613592447572, -0.32705938821652658]
-                self.b = np.zeros((self.s,))
-                self.b[0:3] = self.beta[3, 0:3]
-                self.b[self.s - 1] = self.gamma
-                self.bd = np.zeros((self.s,))
-                self.bd[0:2] = self.beta[2, 0:2]
-                self.bd[self.s - 2] = self.gamma
-                # self.c = np.array([-4.786970949443344e+00, -6.966969867338157e-01, 4.491962205414260e+00,
-                #                    1.247990161586704e+00, -2.562844308238056e-01, 0])
-                # self.d = np.array([1.274202171603216e+01, -1.894421984691950e+00, -1.113020959269748e+01,
-                #                    -1.365987420071593e+00, 1.648597281428871e+00, 0])
-                # self.e = np.zeros((6,))
-                self.gammatilde = self.beta - self.alpha
-                self.a = np.sum(self.alpha, axis=1)
-                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
-                self.gammatilde = self.gammatilde / self.gamma
-                self.alpha = self.alpha.T
-                self.gammatilde = self.gammatilde.T
-            case _:
-                raise ValueError("Not implemented")
-
-
-def dfdt(dae: nDAE, t, y):
-    tscale = np.maximum(0.1 * np.abs(t), 1e-8)
-    ddt = t + np.sqrt(np.spacing(1)) * tscale - t
-    f0 = dae.F(t, y, dae.p)
-    f1 = dae.F(t + ddt, y, dae.p)
-    return (f1 - f0) / ddt
+import warnings
+
+from Solverz.solvers.daesolver.utilities import *
+
+
+@dae_io_parser
+def Rodas(dae: nDAE,
+          tspan: List | np.ndarray,
+          y0: np.ndarray,
+          opt: Opt = None):
+    r"""
+    The stiffly accurate Rosenbrock methods including Rodas4 [1]_, Rodasp [2]_, Rodas5p [3]_.
+
+    Parameters
+    ==========
+
+    dae : nDAE
+        Numerical DAE object.
+
+    tspan : List | np.ndarray
+        Either
+        - a list specifying [t0, tend], or
+        - a `np.ndarray` specifying the time nodes that you are concerned about
+
+    y0 : np.ndarray
+        The initial values of variables
+
+    opt : Opt
+        The solver options, including:
+
+        - scheme: 'rodas4'(default)|'rodasp'|'rodas5p'
+            The rodas scheme
+        - rtol: 1e-3(default)|float
+            The relative error tolerance
+        - atol: 1e-6(default)|float
+            The absolute error tolerance
+        - event: Callable
+            The simulation events, with $t$ and $y$ being args,
+            and `value`, `is_terminal` and `direction` being outputs
+        - fixed_h: False(default)|bool
+            To use fixed step size
+        - hinit: None(default)|float
+            Initial step size
+        - hmax: None(default)|float
+            Maximum step size.
+
+    Returns
+    =======
+
+    sol : daesol
+        The daesol object.
+
+
+    References
+    ==========
+
+    .. [1] Hairer and Wanner, Solving Ordinary Differential Equations II , 2nd ed. Berlin, Heidelberg, Germany: Springer-Verlag, 1996.
+    .. [2] Steinebach, Order-reduction of ROW-methods for DAEs and method of lines applications. Preprint-Nr. 1741, FB Mathematik, TH Darmstadt, 1995
+    .. [3] Steinebach, “Construction of rosenbrock-wanner method rodas5p and numerical benchmarks within the julia differential equations package,” BIT, vol. 63, no. 27, Jun 2023.
+    """
+
+    if opt is None:
+        opt = Opt()
+    stats = Stats(opt.scheme)
+
+    rparam = Rodas_param(opt.scheme)
+    vsize = y0.shape[0]
+    tspan = np.array(tspan)
+    tend = tspan[-1]
+    t0 = tspan[0]
+    if opt.hmax is None:
+        opt.hmax = np.abs(tend - t0)
+    nt = 0
+    t = t0
+    hmin = 16 * np.spacing(t0)
+    uround = np.spacing(1.0)
+    T = np.zeros((10001,))
+    T[nt] = t0
+    y = np.zeros((10001, vsize))
+    y0 = DaeIc(dae, y0, t0, opt.rtol)  # check and modify initial values
+    y[0, :] = y0
+
+    dense_output = False
+    n_tspan = len(tspan)
+    told = t0
+    if n_tspan > 2:
+        dense_output = True
+        inext = 1
+        tnext = tspan[inext]
+
+    events = opt.event
+    haveEvent = True if events is not None else False
+
+    if haveEvent:
+        value, isterminal, direction = events(t, y0)
+    stop = 0
+    nevent = -1
+    te = np.zeros((10001,))
+    ye = np.zeros((10001, vsize))
+    ie = np.zeros((10001,))
+
+    # The initial step size
+    if opt.hinit is None:
+        dt = 1e-6 * (tend - t0)
+    else:
+        dt = opt.hinit
+
+    dt = np.maximum(dt, hmin)
+    dt = np.minimum(dt, opt.hmax)
+
+    M = dae.M
+    p = dae.p
+    done = False
+    reject = 0
+    while not done:
+        # step size too small
+        # pass
+
+        if np.abs(dt) < uround:
+            print(f"Error exit of RODAS at time = {t}: step size too small h = {dt}.\n")
+            stats.ret = 'failed'
+            break
+
+        if reject > 100:
+            print(f"Step rejected over 100 times at time = {t}.\n")
+            stats.ret = 'failed'
+            break
+
+        # Stretch the step if within 10% of T-t.
+        if t + dt >= tend:
+            dt = tend - t
+        else:
+            dt = np.minimum(dt, 0.5 * (tend - t))
+
+        if opt.fix_h:
+            dt = opt.hinit
+
+        if done:
+            break
+        K = np.zeros((vsize, rparam.s))
+
+        if reject == 0:
+            J = dae.J(t, y0, p)
+
+        dfdt0 = dt * dfdt(dae, t, y0)
+        rhs = dae.F(t, y0, p) + rparam.g[0] * dfdt0
+        stats.nfeval = stats.nfeval + 1
+
+        try:
+            lu = lu_decomposition(M - dt * rparam.gamma * J)
+        except RuntimeError:
+            break
+        stats.ndecomp = stats.ndecomp + 1
+        K[:, 0] = lu.solve(rhs)
+
+        for j in range(1, rparam.s):
+            sum_1 = K @ rparam.alpha[:, j]
+            sum_2 = K @ rparam.gammatilde[:, j]
+            y1 = y0 + dt * sum_1
+
+            rhs = dae.F(t + dt * rparam.a[j], y1, p) + M @ sum_2 + rparam.g[j] * dfdt0
+            stats.nfeval = stats.nfeval + 1
+            sol = lu.solve(rhs)
+            K[:, j] = sol - sum_2
+
+        sum_1 = K @ (dt * rparam.b)
+        ynew = y0 + sum_1
+        if not opt.fix_h:
+            sum_2 = K @ (dt * rparam.bd)
+            SK = (opt.atol + opt.rtol * abs(ynew)).reshape((-1,))
+            err = np.max(np.abs((sum_1 - sum_2) / SK))
+            if np.any(np.isinf(ynew)) or np.any(np.isnan(ynew)):
+                err = 1.0e6
+                print('Warning Rodas: NaN or Inf occurs.')
+            err = np.maximum(err, 1.0e-6)
+            fac = opt.f_savety / (err ** (1 / rparam.pord))
+            fac = np.minimum(opt.facmax, np.maximum(opt.fac1, fac))
+            dtnew = dt * fac
+        else:
+            err = 1.0
+            dtnew = dt
+
+        if err <= 1.0:
+            reject = 0
+            told = t
+            t = t + dt
+            stats.nstep = stats.nstep + 1
+            # events
+            if haveEvent:
+                valueold = value
+                value, isterminal, direction = events(t, ynew)
+                value_save = value
+                ff = np.where(value * valueold < 0)[0]
+                if ff.size > 0:
+                    for i in ff:
+                        v0 = valueold[i]
+                        v1 = value[i]
+                        detect = 1
+                        if direction[i] < 0 and v0 <= v1:
+                            detect = 0
+                        if direction[i] > 0 and v0 >= v1:
+                            detect = 0
+                        if detect:
+                            iterate = 1
+                            tL = told
+                            tR = t
+                            if np.abs(v1 - v0) > uround:
+                                tevent = told - v0 * dt / (v1 - v0)  # initial guess for tevent
+                            else:
+                                iterate = 0
+                                tevent = t
+                                ynext = ynew
+
+                            tol = 128 * np.max([np.spacing(told), np.spacing(t)])
+                            tol = np.min([tol, np.abs(t - told)])
+                            while iterate > 0:
+                                iterate = iterate + 1
+                                tau = (tevent - told) / dt
+                                ynext = y0 + tau * dt * K @ (
+                                        rparam.b + (tau - 1) * (rparam.c + tau * (rparam.d + tau * rparam.e)))
+                                value, isterminal, direction = events(tevent, ynext)
+                                if v1 * value[i] < 0:
+                                    tL = tevent
+                                    tevent = 0.5 * (tevent + tR)
+                                    v0 = value[i]
+                                elif v0 * value[i] < 0:
+                                    tR = tevent
+                                    tevent = 0.5 * (tL + tevent)
+                                    v1 = value[i]
+                                else:
+                                    iterate = 0
+                                if (tR - tL) < tol:
+                                    iterate = 0
+                                if iterate > 100:
+                                    print(f"Lost Event in interval [{told}, {t}].\n")
+                                    break
+                            if np.abs(tevent - told) < opt.event_duration:
+                                # We're not going to find events closer than tol.
+                                break
+                            t = tevent
+                            ynew = ynext
+                            nevent += 1
+                            te[nevent] = tevent
+                            ie[nevent] = i
+                            ye[nevent] = ynext
+                            value, isterminal, direction = events(tevent, ynext)
+                            value = value_save
+                            if isterminal[i]:
+                                if dense_output:
+                                    if tnext >= tevent:
+                                        tnext = tevent
+                                stop = 1
+                                break
+
+            if dense_output:  # dense_output
+                while t >= tnext > told:
+                    tau = (tnext - told) / dt
+                    ynext = y0 + tau * dt * K @ (rparam.b + (tau - 1) * (rparam.c + tau * (rparam.d + tau * rparam.e)))
+                    nt = nt + 1
+                    T[nt] = tnext
+                    y[nt] = ynext
+
+                    if haveEvent and stop:
+                        if tnext >= tevent:
+                            break
+
+                    inext = inext + 1
+                    if inext <= n_tspan - 1:
+                        tnext = tspan[inext]
+                        if haveEvent and stop:
+                            if tnext >= tevent:
+                                tnext = tevent
+                    else:
+                        tnext = tend + dt
+            else:
+                nt = nt + 1
+                T[nt] = t
+                y[nt] = ynew
+
+            if nt == 10000:
+                warnings.warn("Time steps more than 10000! Rodas breaks. Try input a smaller tspan!")
+                done = True
+
+            if np.abs(tend - t) < uround or stop:
+                done = True
+            y0 = ynew
+            opt.facmax = opt.fac2
+
+        else:
+            reject = reject + 1
+            stats.nreject = stats.nreject + 1
+            opt.facmax = 1
+        dt = np.min([opt.hmax, np.max([hmin, dtnew])])
+
+    T = T[0:nt + 1]
+    y = y[0:nt + 1]
+    if haveEvent:
+        te = te[0:nevent + 1]
+        ye = ye[0:nevent + 1]
+        ie = ie[0:nevent + 1]
+        return daesol(T, y, te, ye, ie, stats)
+    else:
+        return daesol(T, y, stats=stats)
+
+
+class Rodas_param:
+
+    def __init__(self,
+                 scheme: str = 'rodas4'):
+        match scheme:
+            case 'rodas4':
+                self.s = 6
+                self.pord = 4
+                self.alpha = np.zeros((self.s, self.s))
+                self.beta = np.zeros((self.s, self.s))
+                self.g = np.zeros((self.s, 1))
+                self.gamma = 0.25
+                self.alpha[1, 0] = 3.860000000000000e-01
+                self.alpha[2, 0:2] = [1.460747075254185e-01, 6.392529247458190e-02]
+                self.alpha[3, 0:3] = [-3.308115036677222e-01, 7.111510251682822e-01, 2.496604784994390e-01]
+                self.alpha[4, 0:4] = [-4.552557186318003e+00, 1.710181363241323e+00, 4.014347332103149e+00,
+                                      -1.719715090264703e-01]
+                self.alpha[5, 0:5] = [2.428633765466977e+00, -3.827487337647808e-01, -1.855720330929572e+00,
+                                      5.598352992273752e-01,
+                                      2.499999999999995e-01]
+                self.beta[1, 0] = 3.170000000000250e-02
+                self.beta[2, 0:2] = [1.247220225724355e-02, 5.102779774275723e-02]
+                self.beta[3, 0:3] = [1.196037669338736e+00, 1.774947364178279e-01, -1.029732405756564e+00]
+                self.beta[4, 0:4] = [2.428633765466977e+00, -3.827487337647810e-01, -1.855720330929572e+00,
+                                     5.598352992273752e-01]
+                self.beta[5, 0:5] = [3.484442712860512e-01, 2.130136219118989e-01, -1.541025326623184e-01,
+                                     4.713207793914960e-01,
+                                     -1.286761399271284e-01]
+                self.b = np.zeros((6,))
+                self.b[0:5] = self.beta[5, 0:5]
+                self.b[5] = self.gamma
+                self.bd = np.zeros((6,))
+                self.bd[0:4] = self.beta[4, 0:4]
+                self.bd[4] = self.gamma
+                self.c = np.array([-4.786970949443344e+00, -6.966969867338157e-01, 4.491962205414260e+00,
+                                   1.247990161586704e+00, -2.562844308238056e-01, 0])
+                self.d = np.array([1.274202171603216e+01, -1.894421984691950e+00, -1.113020959269748e+01,
+                                   -1.365987420071593e+00, 1.648597281428871e+00, 0])
+                self.e = np.zeros((6,))
+                self.gammatilde = self.beta - self.alpha
+                self.a = np.sum(self.alpha, axis=1)
+                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
+                self.gammatilde = self.gammatilde / self.gamma
+                self.alpha = self.alpha.T
+                self.gammatilde = self.gammatilde.T
+            case 'rodasp':
+                self.s = 6
+                self.pord = 4
+                self.alpha = np.zeros((self.s, self.s))
+                self.beta = np.zeros((self.s, self.s))
+                self.gamma = 0.25
+                self.alpha[1, 0] = 0.75
+                self.alpha[2, 0:2] = [0.0861204008141522, 0.123879599185848]
+                self.alpha[3, 0:3] = [0.774934535507324, 0.149265154950868, -0.294199690458192]
+                self.alpha[4, 0:4] = [5.30874668264614, 1.33089214003727, -5.37413781165556, -0.265501011027850]
+                self.alpha[5, 0:5] = [-1.76443764877448, -0.474756557206303, 2.36969184691580, 0.619502359064983,
+                                      0.250000000000000]
+                self.beta[1, 0] = 0.0
+                self.beta[2, 0:2] = [-0.0493920000000000, -0.0141120000000000]
+                self.beta[3, 0:3] = [-0.482049469387756, -0.100879555555556, 0.926729024943312]
+                self.beta[4, 0:4] = [-1.76443764877448, -0.474756557206303, 2.36969184691580, 0.619502359064983]
+                self.beta[5, 0:5] = [-0.0803683707891135, -0.0564906135924476, 0.488285630042799, 0.505716211481619,
+                                     -0.107142857142857]
+                self.b = np.zeros((6,))
+                self.b[0:5] = self.beta[5, 0:5]
+                self.b[5] = self.gamma
+                self.bd = np.zeros((6,))
+                self.bd[0:4] = self.beta[4, 0:4]
+                self.bd[4] = self.gamma
+                self.c = np.array([-40.98639964388325,
+                                   -10.36668980524365,
+                                   44.66751816647147,
+                                   4.13001572709988,
+                                   2.55555555555556,
+                                   0])
+                self.d = np.array([73.75018659483291,
+                                   18.54063799119389,
+                                   -81.66902074619779,
+                                   -6.84402606205123,
+                                   -3.77777777777778,
+                                   0])
+                self.e = np.zeros((6,))
+                self.gammatilde = self.beta - self.alpha
+                self.a = np.sum(self.alpha, axis=1)
+                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
+                self.gammatilde = self.gammatilde / self.gamma
+                self.alpha = self.alpha.T
+                self.gammatilde = self.gammatilde.T
+            case 'rodas5p':
+                self.s = 8
+                self.pord = 5
+                self.a = np.zeros((self.s,))
+                self.g = np.zeros((self.s,))
+                self.alpha = np.array([
+                    [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [0.6358126895828704, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [0.31242290829798824, 0.09715693104176527, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [1.3140825753299277, 1.8583084874257945, -2.1954603902496506, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [0.42153145792835994, 0.25386966273009, -0.2365547905326239, -0.010005969169959593, 0.0, 0.0, 0.0,
+                     0.0],
+                    [1.712028062121536, 2.4456320333807953, -3.117254839827603, -0.04680538266310614,
+                     0.006400126988377645, 0.0, 0.0, 0.0],
+                    [-0.9993030215739269, -1.5559156221686088, 3.1251564324842267, 0.24141811637172583,
+                     -0.023293468307707062, 0.21193756319429014, 0.0, 0.0],
+                    [-0.003487250199264519, -0.1299669712056423, 1.525941760806273, 1.1496140949123888,
+                     -0.7043357115882416, -1.0497034859198033, 0.21193756319429014, 0.0]
+                ])
+                self.beta = np.array([
+                    [0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [0.0, 0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [-0.10952700614965587, -0.03129343032847311, 0.21193756319429014, 0.0, 0.0, 0.0, 0.0, 0.0],
+                    [1.701745865188331, -0.15675801606110462, 1.024650547472829, 0.21193756319429014, 0.0, 0.0, 0.0,
+                     0.0],
+                    [3.587261990937329, 1.6112735397639253, -2.378003402448709, -0.2778036907258995,
+                     0.21193756319429014, 0.0, 0.0, 0.0],
+                    [-0.9993030215739269, -1.5559156221686088, 3.1251564324842267, 0.24141811637172583,
+                     -0.023293468307707062, 0.21193756319429014, 0.0, 0.0],
+                    [-0.003487250199264519, -0.1299669712056423, 1.525941760806273, 1.1496140949123888,
+                     -0.7043357115882416, -1.0497034859198033, 0.21193756319429014, 0.0],
+                    [0.12236007991300712, 0.050238881884191906, 1.3238392208663585, 1.2643883758622305,
+                     -0.7904031855871826, -0.9680932754194287, -0.214267660713467, 0.21193756319429014]
+                ])
+                self.c = np.array([-0.8232744916805133, 0.3181483349120214, 0.16922330104086836, -0.049879453396320994,
+                                   0.19831791977261218, 0.31488148287699225, -0.16387506167704194,
+                                   0.036457968151382296])
+                self.d = np.array([-0.6726085201965635, -1.3128972079520966, 9.467244336394248, 12.924520918142036,
+                                   -9.002714541842755, -11.404611057341922, -1.4210850083209667,
+                                   1.4221510811179898])
+                self.e = np.array([1.4025185206933914, 0.9860299407499886, -11.006871867857507, -14.112585514422294,
+                                   9.574969612795117, 12.076626078349426, 2.114222828697341,
+                                   -1.0349095990054304])
+                self.gamma = self.beta[0, 0]
+                self.b = np.append(self.beta[7, :-1], [self.gamma])
+                self.bd = np.append(self.beta[6, :-2], [self.gamma, 0])
+                self.gammatilde = self.beta - self.gamma * np.eye(self.s) - self.alpha
+                for i in range(self.s):
+                    self.a[i] = np.sum(self.alpha[i, :])
+                    self.g[i] = np.sum(self.gammatilde[i, :]) + self.gamma
+                self.gammatilde /= self.gamma
+                self.alpha = self.alpha.T
+                self.gammatilde = self.gammatilde.T
+            case 'rodas3d':
+                self.s = 4
+                self.pord = 3
+                self.alpha = np.zeros((self.s, self.s))
+                self.beta = np.zeros((self.s, self.s))
+                self.g = np.zeros((self.s, 1))
+                self.gamma = 0.57281606
+                self.alpha[1, 0] = 1.2451051999132263
+                self.alpha[2, 0:2] = [1, 0]
+                self.alpha[3, 0:3] = [0.32630307266483527, 0.10088086733516474, 0.57281606]
+                self.beta[1, 0] = -3.1474142698552949
+                self.beta[2, 0:2] = [0.32630307266483527, 0.10088086733516474]
+                self.beta[3, 0:3] = [0.69775271462407906, 0.056490613592447572, -0.32705938821652658]
+                self.b = np.zeros((self.s,))
+                self.b[0:3] = self.beta[3, 0:3]
+                self.b[self.s - 1] = self.gamma
+                self.bd = np.zeros((self.s,))
+                self.bd[0:2] = self.beta[2, 0:2]
+                self.bd[self.s - 2] = self.gamma
+                # self.c = np.array([-4.786970949443344e+00, -6.966969867338157e-01, 4.491962205414260e+00,
+                #                    1.247990161586704e+00, -2.562844308238056e-01, 0])
+                # self.d = np.array([1.274202171603216e+01, -1.894421984691950e+00, -1.113020959269748e+01,
+                #                    -1.365987420071593e+00, 1.648597281428871e+00, 0])
+                # self.e = np.zeros((6,))
+                self.gammatilde = self.beta - self.alpha
+                self.a = np.sum(self.alpha, axis=1)
+                self.g = np.sum(self.gammatilde, axis=1) + self.gamma
+                self.gammatilde = self.gammatilde / self.gamma
+                self.alpha = self.alpha.T
+                self.gammatilde = self.gammatilde.T
+            case _:
+                raise ValueError("Not implemented")
+
+
+def dfdt(dae: nDAE, t, y):
+    tscale = np.maximum(0.1 * np.abs(t), 1e-8)
+    ddt = t + np.sqrt(np.spacing(1)) * tscale - t
+    f0 = dae.F(t, y, dae.p)
+    f1 = dae.F(t + ddt, y, dae.p)
+    return (f1 - f0) / ddt
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/daesolver/trapezoidal.py` & `solverz-0.0.1rc2/Solverz/solvers/daesolver/trapezoidal.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from Solverz.solvers.daesolver.utilities import *
-
-
-@dae_io_parser
-def implicit_trapezoid(dae: nDAE,
-                       tspan: List | np.ndarray,
-                       y0: np.ndarray,
-                       opt: Opt = None):
-    r"""
-    The fixed step implicit trapezoidal method.
-
-    Parameters
-    ==========
-
-    dae : nDAE
-        Numerical DAE object.
-
-    tspan : List | np.ndarray
-        An array specifying t0 and tend
-
-    y0 : np.ndarray
-        The initial values of variables
-
-    opt : Opt
-        The solver options, including:
-
-        - step_size: 1e-3(default)|float
-            The step size
-
-    Returns
-    =======
-
-    sol : daesol
-        The daesol object.
-
-
-    References
-    ==========
-
-    .. [1] https://en.wikipedia.org/wiki/Trapezoidal_rule_(differential_equations)
-
-    """
-    stats = Stats(scheme='Trapezoidal')
-    if opt is None:
-        opt = Opt(stats=True)
-    dt = opt.step_size
-    tspan = np.array(tspan)
-    T_initial = tspan[0]
-    T_end = tspan[-1]
-    nt = 0
-    tt = T_initial
-    t0 = tt
-
-    y = np.zeros((10000, y0.shape[0]))
-    y0 = DaeIc(dae, y0, t0, opt.rtol)  # check and modify initial values
-    y[0, :] = y0
-    T = np.zeros((10000,))
-
-    p = dae.p
-    while abs(tt - T_end) > abs(dt) / 10:
-        My0 = dae.M @ y0
-        F0 = dae.F(t0, y0, p).copy()
-        ae = nAE(lambda y_, p_: dt / 2 * (dae.F(t0 + dt, y_, p_) + F0) - dae.M @ y_ + My0,
-                 lambda y_, p_: -dae.M + dt / 2 * dae.J(t0 + dt, y_, p_),
-                 p)
-
-        sol = nr_method(ae, y0, Opt(stats=True))
-        y1 = sol.y
-        ite = sol.stats
-        stats.ndecomp = stats.ndecomp + ite
-        stats.nfeval = stats.nfeval + ite
-
-        tt = tt + dt
-        nt = nt + 1
-        y[nt] = y1
-        T[nt] = tt
-        y0 = y1
-        t0 = tt
-
-    y = y[0:nt + 1]
-    T = T[0:nt + 1]
-    stats.nstep = nt
-
-    return daesol(T, y, stats=stats)
+from Solverz.solvers.daesolver.utilities import *
+
+
+@dae_io_parser
+def implicit_trapezoid(dae: nDAE,
+                       tspan: List | np.ndarray,
+                       y0: np.ndarray,
+                       opt: Opt = None):
+    r"""
+    The fixed step implicit trapezoidal method.
+
+    Parameters
+    ==========
+
+    dae : nDAE
+        Numerical DAE object.
+
+    tspan : List | np.ndarray
+        An array specifying t0 and tend
+
+    y0 : np.ndarray
+        The initial values of variables
+
+    opt : Opt
+        The solver options, including:
+
+        - step_size: 1e-3(default)|float
+            The step size
+
+    Returns
+    =======
+
+    sol : daesol
+        The daesol object.
+
+
+    References
+    ==========
+
+    .. [1] https://en.wikipedia.org/wiki/Trapezoidal_rule_(differential_equations)
+
+    """
+    stats = Stats(scheme='Trapezoidal')
+    if opt is None:
+        opt = Opt(stats=True)
+    dt = opt.step_size
+    tspan = np.array(tspan)
+    T_initial = tspan[0]
+    T_end = tspan[-1]
+    nt = 0
+    tt = T_initial
+    t0 = tt
+
+    y = np.zeros((10000, y0.shape[0]))
+    y0 = DaeIc(dae, y0, t0, opt.rtol)  # check and modify initial values
+    y[0, :] = y0
+    T = np.zeros((10000,))
+
+    p = dae.p
+    while abs(tt - T_end) > abs(dt) / 10:
+        My0 = dae.M @ y0
+        F0 = dae.F(t0, y0, p).copy()
+        ae = nAE(lambda y_, p_: dt / 2 * (dae.F(t0 + dt, y_, p_) + F0) - dae.M @ y_ + My0,
+                 lambda y_, p_: -dae.M + dt / 2 * dae.J(t0 + dt, y_, p_),
+                 p)
+
+        sol = nr_method(ae, y0, Opt(stats=True))
+        y1 = sol.y
+        ite = sol.stats
+        stats.ndecomp = stats.ndecomp + ite
+        stats.nfeval = stats.nfeval + ite
+
+        tt = tt + dt
+        nt = nt + 1
+        y[nt] = y1
+        T[nt] = tt
+        y0 = y1
+        t0 = tt
+
+    y = y[0:nt + 1]
+    T = T[0:nt + 1]
+    stats.nstep = nt
+
+    return daesol(T, y, stats=stats)
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/nlaesolver/cnr.py` & `solverz-0.0.1rc2/Solverz/solvers/nlaesolver/cnr.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from Solverz.solvers.nlaesolver.utilities import *
-
-
-@ae_io_parser
-def continuous_nr(eqn: nAE,
-                  y: np.ndarray,
-                  opt: Opt = None):
-    r"""
-    The Continuous Newton-Raphson method.
-
-    Parameters
-    ==========
-
-    eqn : nAE
-        Numerical AE object.
-
-    y : np.ndarray
-        The initial values of variables
-
-    opt : Opt
-        The solver options, including:
-
-        - ite_tol: 1e-8(default)|float
-            The iteration error tolerance.
-
-    Returns
-    =======
-
-    sol : aesol
-        The aesol object.
-
-    References
-    ==========
-
-    .. [1] F. Milano, ‘Continuous Newton’s Method for Power Flow Analysis’, IEEE Transactions on Power Systems, vol. 24,
-           no. 1, pp. 50–57, Feb. 2009, doi: 10.1109/TPWRS.2008.2004820.
-
-    """
-    p = eqn.p
-    if opt is None:
-        opt = Opt()
-
-    dt = 1
-    hmax = 1.7
-    tol = opt.ite_tol
-
-    def f(y_, p_) -> np.ndarray:
-        return -solve(eqn.J(y_, p_), eqn.F(y_, p_))
-
-    Pow = 1 / 5
-    # c2, c3, c4, c5 = 1 / 5, 3 / 10, 4 / 5, 8 / 9 for non-autonomous equations
-    a11, a21, a31, a41, a51, a61 = 1 / 5, 3 / 40, 44 / 45, 19372 / 6561, 9017 / 3168, 35 / 384
-    a22, a32, a42, a52 = 9 / 40, -56 / 15, -25360 / 2187, -355 / 33
-    a33, a43, a53, a63 = 32 / 9, 64448 / 6561, 46732 / 5247, 500 / 1113
-    a44, a54, a64 = -212 / 729, 49 / 176, 125 / 192
-    a55, a65 = -5103 / 18656, -2187 / 6784
-    a66 = 11 / 84
-    e1, e3, e4, e5, e6, e7 = 71 / 57600, -71 / 16695, 71 / 1920, -17253 / 339200, 22 / 525, -1 / 40
-
-    dt = dt
-    atol = 1e-6
-    rtol = 1e-1
-    threshold = atol / rtol
-    hmax = hmax
-    hmin = 16 * np.spacing(0)
-    # atol and rtol can not be too small
-    ite = 0
-    df = eqn.F(y, p)
-    while max(abs(df)) > tol:
-        ite = ite + 1
-        err = 2
-        nofailed = True
-        while err > rtol:
-            k1 = f(y, p)
-            k2 = f(y + dt * a11 * k1, p)
-            k3 = f(y + dt * (a21 * k1 + a22 * k2), p)
-            k4 = f(y + dt * (a31 * k1 + a32 * k2 + a33 * k3), p)
-            k5 = f(y + dt * (a41 * k1 + a42 * k2 + a43 * k3 + a44 * k4), p)
-            k6 = f(y + dt * (a51 * k1 + a52 * k2 + a53 * k3 + a54 * k4 + a55 * k5), p)
-            ynew = y + dt * (a61 * k1 + a63 * k3 + a64 * k4 + a65 * k5 + a66 * k6)  # y6 has nothing to do with k7
-            k7 = f(ynew, p)
-            kE = k1 * e1 + k3 * e3 + k4 * e4 + k5 * e5 + k6 * e6 + k7 * e7
-
-            # error control
-            # error estimation
-            err = dt * np.linalg.norm(
-                kE.reshape(-1, ) / np.maximum(np.maximum(abs(y), abs(ynew)).reshape(-1, ), threshold),
-                np.Inf)
-            if err > rtol:  # failed step
-                if dt <= hmin:
-                    raise ValueError(f'IntegrationTolNotMet step size: {dt} hmin: {hmin}')
-                if nofailed:  # There haven't been failed attempts
-                    nofailed = False
-                    dt = np.max([hmin, dt * np.max([0.1, 0.8 * (rtol / err) ** Pow])])
-                else:
-                    dt = np.max([hmin, 0.5 * dt])
-            else:  # Successful step
-                break
-
-        y = ynew
-        df = eqn.F(y, p)
-
-        if nofailed:  # Enlarge step size if no failure is met
-            temp = 1.25 * (err / rtol) ** Pow
-            if temp > 0.2:
-                dt = dt / temp
-            else:
-                dt = 5 * dt
-
-        dt = np.min([dt, hmax])
-
-        if ite > 100:
-            break
-
-    return aesol(y, ite)
+from Solverz.solvers.nlaesolver.utilities import *
+
+
+@ae_io_parser
+def continuous_nr(eqn: nAE,
+                  y: np.ndarray,
+                  opt: Opt = None):
+    r"""
+    The Continuous Newton-Raphson method.
+
+    Parameters
+    ==========
+
+    eqn : nAE
+        Numerical AE object.
+
+    y : np.ndarray
+        The initial values of variables
+
+    opt : Opt
+        The solver options, including:
+
+        - ite_tol: 1e-8(default)|float
+            The iteration error tolerance.
+
+    Returns
+    =======
+
+    sol : aesol
+        The aesol object.
+
+    References
+    ==========
+
+    .. [1] F. Milano, ‘Continuous Newton’s Method for Power Flow Analysis’, IEEE Transactions on Power Systems, vol. 24,
+           no. 1, pp. 50–57, Feb. 2009, doi: 10.1109/TPWRS.2008.2004820.
+
+    """
+    p = eqn.p
+    if opt is None:
+        opt = Opt()
+
+    dt = 1
+    hmax = 1.7
+    tol = opt.ite_tol
+
+    def f(y_, p_) -> np.ndarray:
+        return -solve(eqn.J(y_, p_), eqn.F(y_, p_))
+
+    Pow = 1 / 5
+    # c2, c3, c4, c5 = 1 / 5, 3 / 10, 4 / 5, 8 / 9 for non-autonomous equations
+    a11, a21, a31, a41, a51, a61 = 1 / 5, 3 / 40, 44 / 45, 19372 / 6561, 9017 / 3168, 35 / 384
+    a22, a32, a42, a52 = 9 / 40, -56 / 15, -25360 / 2187, -355 / 33
+    a33, a43, a53, a63 = 32 / 9, 64448 / 6561, 46732 / 5247, 500 / 1113
+    a44, a54, a64 = -212 / 729, 49 / 176, 125 / 192
+    a55, a65 = -5103 / 18656, -2187 / 6784
+    a66 = 11 / 84
+    e1, e3, e4, e5, e6, e7 = 71 / 57600, -71 / 16695, 71 / 1920, -17253 / 339200, 22 / 525, -1 / 40
+
+    dt = dt
+    atol = 1e-6
+    rtol = 1e-1
+    threshold = atol / rtol
+    hmax = hmax
+    hmin = 16 * np.spacing(0)
+    # atol and rtol can not be too small
+    ite = 0
+    df = eqn.F(y, p)
+    while max(abs(df)) > tol:
+        ite = ite + 1
+        err = 2
+        nofailed = True
+        while err > rtol:
+            k1 = f(y, p)
+            k2 = f(y + dt * a11 * k1, p)
+            k3 = f(y + dt * (a21 * k1 + a22 * k2), p)
+            k4 = f(y + dt * (a31 * k1 + a32 * k2 + a33 * k3), p)
+            k5 = f(y + dt * (a41 * k1 + a42 * k2 + a43 * k3 + a44 * k4), p)
+            k6 = f(y + dt * (a51 * k1 + a52 * k2 + a53 * k3 + a54 * k4 + a55 * k5), p)
+            ynew = y + dt * (a61 * k1 + a63 * k3 + a64 * k4 + a65 * k5 + a66 * k6)  # y6 has nothing to do with k7
+            k7 = f(ynew, p)
+            kE = k1 * e1 + k3 * e3 + k4 * e4 + k5 * e5 + k6 * e6 + k7 * e7
+
+            # error control
+            # error estimation
+            err = dt * np.linalg.norm(
+                kE.reshape(-1, ) / np.maximum(np.maximum(abs(y), abs(ynew)).reshape(-1, ), threshold),
+                np.Inf)
+            if err > rtol:  # failed step
+                if dt <= hmin:
+                    raise ValueError(f'IntegrationTolNotMet step size: {dt} hmin: {hmin}')
+                if nofailed:  # There haven't been failed attempts
+                    nofailed = False
+                    dt = np.max([hmin, dt * np.max([0.1, 0.8 * (rtol / err) ** Pow])])
+                else:
+                    dt = np.max([hmin, 0.5 * dt])
+            else:  # Successful step
+                break
+
+        y = ynew
+        df = eqn.F(y, p)
+
+        if nofailed:  # Enlarge step size if no failure is met
+            temp = 1.25 * (err / rtol) ** Pow
+            if temp > 0.2:
+                dt = dt / temp
+            else:
+                dt = 5 * dt
+
+        dt = np.min([dt, hmax])
+
+        if ite > 100:
+            break
+
+    return aesol(y, ite)
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/nlaesolver/nr.py` & `solverz-0.0.1rc2/Solverz/solvers/nlaesolver/nr.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from Solverz.solvers.nlaesolver.utilities import *
-
-
-@ae_io_parser
-def nr_method(eqn: nAE,
-              y: np.ndarray,
-              opt: Opt = None):
-    r"""
-    The Newton-Raphson method.
-
-    Parameters
-    ==========
-
-    eqn : nAE
-        Numerical AE object.
-
-    y : np.ndarray
-        The initial values of variables
-
-    opt : Opt
-        The solver options, including:
-
-        - ite_tol: 1e-8(default)|float
-            The iteration error tolerance.
-
-    Returns
-    =======
-
-    sol : aesol
-        The aesol object.
-
-    References
-    ==========
-
-    .. [1] https://en.wikipedia.org/wiki/Newton%27s_method
-
-    """
-    if opt is None:
-        opt = Opt(ite_tol=1e-8)
-
-    tol = opt.ite_tol
-    p = eqn.p
-    df = eqn.F(y, p)
-    ite = 0
-    # main loop
-    while max(abs(df)) > tol:
-        ite = ite + 1
-        y = y - solve(eqn.J(y, p), df)
-        df = eqn.F(y, p)
-        if ite >= 100:
-            print(f"Cannot converge within 100 iterations. Deviation: {max(abs(df))}!")
-            break
-
-    return aesol(y, ite)
+from Solverz.solvers.nlaesolver.utilities import *
+
+
+@ae_io_parser
+def nr_method(eqn: nAE,
+              y: np.ndarray,
+              opt: Opt = None):
+    r"""
+    The Newton-Raphson method.
+
+    Parameters
+    ==========
+
+    eqn : nAE
+        Numerical AE object.
+
+    y : np.ndarray
+        The initial values of variables
+
+    opt : Opt
+        The solver options, including:
+
+        - ite_tol: 1e-8(default)|float
+            The iteration error tolerance.
+
+    Returns
+    =======
+
+    sol : aesol
+        The aesol object.
+
+    References
+    ==========
+
+    .. [1] https://en.wikipedia.org/wiki/Newton%27s_method
+
+    """
+    if opt is None:
+        opt = Opt(ite_tol=1e-8)
+
+    tol = opt.ite_tol
+    p = eqn.p
+    df = eqn.F(y, p)
+    ite = 0
+    # main loop
+    while max(abs(df)) > tol:
+        ite = ite + 1
+        y = y - solve(eqn.J(y, p), df)
+        df = eqn.F(y, p)
+        if ite >= 100:
+            print(f"Cannot converge within 100 iterations. Deviation: {max(abs(df))}!")
+            break
+
+    return aesol(y, ite)
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/odesolver/ode45.py` & `solverz-0.0.1rc2/Solverz/solvers/odesolver/ode45.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-from __future__ import annotations
-
-from typing import Union, List
-
-import numpy as np
-from numpy import abs, linalg
-
-from Solverz.equation.equations import DAE
-from Solverz.num_api.num_eqn import nDAE, nAE
-from Solverz.solvers.laesolver import lu_decomposition
-from Solverz.solvers.nlaesolver import nr_method
-from Solverz.solvers.option import Opt
-from Solverz.solvers.parser import dae_io_parser
-from Solverz.solvers.stats import Stats
-from Solverz.variable.variables import TimeVars
-
-
-def ode45(ode: DAE,
-          y: TimeVars,
-          tspan: Union[List, np.ndarray],
-          dt=None,
-          atol=1e-6,
-          rtol=1e-3,
-          output_k=False):
-    """
-    Ode45 with dense output
-    :return:
-    """
-
-    Pow = 1 / 5
-    # c2, c3, c4, c5 = 1 / 5, 3 / 10, 4 / 5, 8 / 9 for non-autonomous equations
-    a11, a21, a31, a41, a51, a61 = 1 / 5, 3 / 40, 44 / 45, 19372 / 6561, 9017 / 3168, 35 / 384
-    a22, a32, a42, a52 = 9 / 40, -56 / 15, -25360 / 2187, -355 / 33
-    a33, a43, a53, a63 = 32 / 9, 64448 / 6561, 46732 / 5247, 500 / 1113
-    a44, a54, a64 = -212 / 729, 49 / 176, 125 / 192
-    a55, a65 = -5103 / 18656, -2187 / 6784
-    a66 = 11 / 84
-    e1, e3, e4, e5, e6, e7 = 71 / 57600, -71 / 16695, 71 / 1920, -17253 / 339200, 22 / 525, -1 / 40
-
-    tspan = np.array(tspan)
-    T = tspan[-1]
-    hmax = np.abs(T) / 10
-    i = 0
-    t = 0
-    tout = TimeVar('tout', length=100)
-    hmin = 16 * np.spacing(t)
-    threshold = atol / rtol
-    y0 = y[0]
-    if output_k:
-        kout = np.zeros((100, ode.f(y0).shape[0], 7))
-
-    # Compute an initial step size using f(y)
-    if dt is None:
-        dt = hmax
-    dt_ = linalg.norm(ode.f(y0) / np.maximum(np.abs(y0), threshold), np.Inf) / (0.8 * rtol ** Pow)
-    if dt * dt_ > 1:
-        dt = 1 / dt_
-    dt = np.maximum(dt, hmin)
-
-    done = False
-    while not done:
-        hmin = 16 * np.spacing(dt)
-        dt = np.min([hmax, np.max([hmin, dt])])
-
-        # Stretch the step if within 10% of T-t.
-        if 1.1 * dt >= np.abs(T - t):
-            dt = T - t
-            done = True
-
-        nofailed = True
-        while True:
-            k1 = ode.f(y0)
-            k2 = ode.f(y0 + dt * a11 * k1)
-            k3 = ode.f(y0 + dt * (a21 * k1 + a22 * k2))
-            k4 = ode.f(y0 + dt * (a31 * k1 + a32 * k2 + a33 * k3))
-            k5 = ode.f(y0 + dt * (a41 * k1 + a42 * k2 + a43 * k3 + a44 * k4))
-            k6 = ode.f(y0 + dt * (a51 * k1 + a52 * k2 + a53 * k3 + a54 * k4 + a55 * k5))
-            ynew = y0 + dt * (a61 * k1 + a63 * k3 + a64 * k4 + a65 * k5 + a66 * k6)  # y6 has nothing to do with k7
-            k7 = ode.f(ynew)
-            kE = k1 * e1 + k3 * e3 + k4 * e4 + k5 * e5 + k6 * e6 + k7 * e7
-            tnew = t + dt
-            if done:
-                tnew = T
-            dt = tnew - t  # purify dt
-            # error control
-            # error estimation
-            err = dt * linalg.norm(kE / np.maximum(np.maximum(abs(y0), abs(ynew)).reshape(-1, ), threshold), np.Inf)
-
-            if err > rtol:  # failed step
-                if dt <= hmin:
-                    raise ValueError(f'IntegrationTolNotMet step size: {dt} hmin: {hmin}')
-                if nofailed:  # There haven't been failed attempts
-                    nofailed = False
-                    dt = np.max([hmin, dt * np.max([0.1, 0.8 * (rtol / err) ** Pow])])
-                else:
-                    dt = np.max([hmin, 0.5 * dt])
-                done = False
-            else:  # Successful step
-                break
-        i = i + 1
-
-        # TODO: 3. Event
-
-        # Output
-        y[i] = ynew
-        tout[i] = tnew
-        if output_k:
-            kout[i - 1, :, :] = np.array([k1, k2, k3, k4, k5, k6, k7]).T
-
-        if done:
-            break
-        if nofailed:  # Enlarge step size if no failure is met
-            temp = 1.25 * (err / rtol) ** Pow
-            if temp > 0.2:
-                dt = dt / temp
-            else:
-                dt = 5 * dt
-
-        t = tnew
-        y0 = ynew
-
-    tout = tout[0:i + 1]
-    y = y[0:i + 1]
-    if output_k:
-        kout = kout[0:i]
-        return tout, y, kout
-    else:
-        return tout, y
-
-
-def nrtp45(tinterp: np.ndarray, t: float, y: np.ndarray, dt: float, k: np.ndarray) -> np.ndarray:
-    """
-    Dense output of ODE45 with continuous Runge-Kutta method
-    :return:
-    """
-    # Define the BI matrix
-    BI = np.array([
-        [1, - 183 / 64, 37 / 12, - 145 / 128],
-        [0, 0, 0, 0],
-        [0, 1500 / 371, - 1000 / 159, 1000 / 371],
-        [0, - 125 / 32, 125 / 12, - 375 / 64],
-        [0, 9477 / 3392, - 729 / 106, 25515 / 6784],
-        [0, - 11 / 7, 11 / 3, - 55 / 28],
-        [0, 3 / 2, - 4, 5 / 2]
-    ])
-    s = (tinterp - t) / dt
-    yinterp = np.repeat(y.reshape(-1, 1), tinterp.shape[0], axis=1) + k @ (dt * BI) @ np.cumprod([s, s, s, s], axis=0)
-    return yinterp
+from __future__ import annotations
+
+from typing import Union, List
+
+import numpy as np
+from numpy import abs, linalg
+
+from Solverz.equation.equations import DAE
+from Solverz.num_api.num_eqn import nDAE, nAE
+from Solverz.solvers.laesolver import lu_decomposition
+from Solverz.solvers.nlaesolver import nr_method
+from Solverz.solvers.option import Opt
+from Solverz.solvers.parser import dae_io_parser
+from Solverz.solvers.stats import Stats
+from Solverz.variable.variables import TimeVars
+
+
+def ode45(ode: DAE,
+          y: TimeVars,
+          tspan: Union[List, np.ndarray],
+          dt=None,
+          atol=1e-6,
+          rtol=1e-3,
+          output_k=False):
+    """
+    Ode45 with dense output
+    :return:
+    """
+
+    Pow = 1 / 5
+    # c2, c3, c4, c5 = 1 / 5, 3 / 10, 4 / 5, 8 / 9 for non-autonomous equations
+    a11, a21, a31, a41, a51, a61 = 1 / 5, 3 / 40, 44 / 45, 19372 / 6561, 9017 / 3168, 35 / 384
+    a22, a32, a42, a52 = 9 / 40, -56 / 15, -25360 / 2187, -355 / 33
+    a33, a43, a53, a63 = 32 / 9, 64448 / 6561, 46732 / 5247, 500 / 1113
+    a44, a54, a64 = -212 / 729, 49 / 176, 125 / 192
+    a55, a65 = -5103 / 18656, -2187 / 6784
+    a66 = 11 / 84
+    e1, e3, e4, e5, e6, e7 = 71 / 57600, -71 / 16695, 71 / 1920, -17253 / 339200, 22 / 525, -1 / 40
+
+    tspan = np.array(tspan)
+    T = tspan[-1]
+    hmax = np.abs(T) / 10
+    i = 0
+    t = 0
+    tout = TimeVar('tout', length=100)
+    hmin = 16 * np.spacing(t)
+    threshold = atol / rtol
+    y0 = y[0]
+    if output_k:
+        kout = np.zeros((100, ode.f(y0).shape[0], 7))
+
+    # Compute an initial step size using f(y)
+    if dt is None:
+        dt = hmax
+    dt_ = linalg.norm(ode.f(y0) / np.maximum(np.abs(y0), threshold), np.Inf) / (0.8 * rtol ** Pow)
+    if dt * dt_ > 1:
+        dt = 1 / dt_
+    dt = np.maximum(dt, hmin)
+
+    done = False
+    while not done:
+        hmin = 16 * np.spacing(dt)
+        dt = np.min([hmax, np.max([hmin, dt])])
+
+        # Stretch the step if within 10% of T-t.
+        if 1.1 * dt >= np.abs(T - t):
+            dt = T - t
+            done = True
+
+        nofailed = True
+        while True:
+            k1 = ode.f(y0)
+            k2 = ode.f(y0 + dt * a11 * k1)
+            k3 = ode.f(y0 + dt * (a21 * k1 + a22 * k2))
+            k4 = ode.f(y0 + dt * (a31 * k1 + a32 * k2 + a33 * k3))
+            k5 = ode.f(y0 + dt * (a41 * k1 + a42 * k2 + a43 * k3 + a44 * k4))
+            k6 = ode.f(y0 + dt * (a51 * k1 + a52 * k2 + a53 * k3 + a54 * k4 + a55 * k5))
+            ynew = y0 + dt * (a61 * k1 + a63 * k3 + a64 * k4 + a65 * k5 + a66 * k6)  # y6 has nothing to do with k7
+            k7 = ode.f(ynew)
+            kE = k1 * e1 + k3 * e3 + k4 * e4 + k5 * e5 + k6 * e6 + k7 * e7
+            tnew = t + dt
+            if done:
+                tnew = T
+            dt = tnew - t  # purify dt
+            # error control
+            # error estimation
+            err = dt * linalg.norm(kE / np.maximum(np.maximum(abs(y0), abs(ynew)).reshape(-1, ), threshold), np.Inf)
+
+            if err > rtol:  # failed step
+                if dt <= hmin:
+                    raise ValueError(f'IntegrationTolNotMet step size: {dt} hmin: {hmin}')
+                if nofailed:  # There haven't been failed attempts
+                    nofailed = False
+                    dt = np.max([hmin, dt * np.max([0.1, 0.8 * (rtol / err) ** Pow])])
+                else:
+                    dt = np.max([hmin, 0.5 * dt])
+                done = False
+            else:  # Successful step
+                break
+        i = i + 1
+
+        # TODO: 3. Event
+
+        # Output
+        y[i] = ynew
+        tout[i] = tnew
+        if output_k:
+            kout[i - 1, :, :] = np.array([k1, k2, k3, k4, k5, k6, k7]).T
+
+        if done:
+            break
+        if nofailed:  # Enlarge step size if no failure is met
+            temp = 1.25 * (err / rtol) ** Pow
+            if temp > 0.2:
+                dt = dt / temp
+            else:
+                dt = 5 * dt
+
+        t = tnew
+        y0 = ynew
+
+    tout = tout[0:i + 1]
+    y = y[0:i + 1]
+    if output_k:
+        kout = kout[0:i]
+        return tout, y, kout
+    else:
+        return tout, y
+
+
+def nrtp45(tinterp: np.ndarray, t: float, y: np.ndarray, dt: float, k: np.ndarray) -> np.ndarray:
+    """
+    Dense output of ODE45 with continuous Runge-Kutta method
+    :return:
+    """
+    # Define the BI matrix
+    BI = np.array([
+        [1, - 183 / 64, 37 / 12, - 145 / 128],
+        [0, 0, 0, 0],
+        [0, 1500 / 371, - 1000 / 159, 1000 / 371],
+        [0, - 125 / 32, 125 / 12, - 375 / 64],
+        [0, 9477 / 3392, - 729 / 106, 25515 / 6784],
+        [0, - 11 / 7, 11 / 3, - 55 / 28],
+        [0, 3 / 2, - 4, 5 / 2]
+    ])
+    s = (tinterp - t) / dt
+    yinterp = np.repeat(y.reshape(-1, 1), tinterp.shape[0], axis=1) + k @ (dt * BI) @ np.cumprod([s, s, s, s], axis=0)
+    return yinterp
```

### Comparing `solverz-0.0.1rc1/Solverz/solvers/test/test_rodas_event.py` & `solverz-0.0.1rc2/Solverz/solvers/test/test_rodas_event.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import numpy as np
-from Solverz import Ode, Var, Opt, Rodas, made_numerical, TimeVars, Model
-
-
-# %% event test
-def test_bounceball():
-    m = Model()
-    m.x = Var('x', [0, 20])
-    m.f1 = Ode('f1', m.x[1], m.x[0])
-    m.f2 = Ode('f2', -9.8, m.x[1])
-    bball, y0 = m.create_instance()
-    nbball = made_numerical(bball, y0, sparse=True)
-
-    def events(t, y):
-        value = np.array([y[0]])
-        isterminal = np.array([1])
-        direction = np.array([-1])
-        return value, isterminal, direction
-
-    opt = Opt(event=events)
-    tout = np.array([0])
-    yout = TimeVars(y0, 1)
-    teout = np.array([])
-    yeout = TimeVars(y0, 0)
-    ieout = np.array([], dtype=int)
-    tstart = 0
-    tend = 30
-    for i in range(10):
-        sol = Rodas(nbball, np.linspace(tstart, tend, 100), y0, opt)
-
-        tout = np.concatenate([tout, sol.T[1:]])
-        yout.append(sol.Y[1:])
-        teout = np.concatenate([teout, sol.te])
-        yeout.append(sol.ye)
-        ieout = np.concatenate([ieout, sol.ie])
-
-        y0['x'][0] = 0
-        y0['x'][1] = -0.9 * sol.Y[-1]['x'][1]
-        tstart = sol.T[-1]
-
-    np.testing.assert_allclose(teout,
-                               np.array([4.081633047365558, 7.755103268847604, 11.061226369910107, 14.03673684129459,
-                                         16.714695668619328, 19.124858513456523, 21.294005283692695, 23.246237159791765,
-                                         25.003245923211466, 26.584554164220997]),
-                               rtol=1e-5,
-                               atol=0)
-
-
-def test_orbit():
-    mu = 1 / 82.45
-    mustar = 1 - mu
-    m = Model()
-    m.y = Var('y', [1.2, 0, 0, -1.04935750983031990726])
-    m.f1 = Ode('f1', m.y[2], m.y[0])
-    m.f2 = Ode('f2', m.y[3], m.y[1])
-    r13 = ((m.y[0] + mu) ** 2 + m.y[1] ** 2) ** 1.5
-    r23 = ((m.y[0] - mustar) ** 2 + m.y[1] ** 2) ** 1.5
-    m.f3 = Ode('f3',
-               2 * m.y[3] + m.y[0] - mustar * ((m.y[0] + mu) / r13) - mu * ((m.y[0] - mustar) / r23),
-               m.y[2])
-    m.f4 = Ode('f4',
-               -2 * m.y[2] + m.y[1] - mustar * (m.y[1] / r13) - mu * (m.y[1] / r23),
-               m.y[3])
-    orbit, y0 = m.create_instance()
-    norbit = made_numerical(orbit, y0, sparse=True)
-
-    def events(t, y):
-        dDSQdt = 2 * (y[0:2] - np.array([1.2, 0])).dot(y[2:4])
-        value = np.array([dDSQdt, dDSQdt])
-        isterminal = np.array([1, 0])
-        direction = np.array([1, -1])
-        return value, isterminal, direction
-
-    sol = Rodas(norbit, [0, 7], y0, Opt(event=events, rtol=1e-5, atol=1e-4))
-
-    np.testing.assert_allclose(sol.te,
-                               np.array([3.09609516, 6.19215951]),
-                               rtol=1e-5,
-                               atol=0)
-    np.testing.assert_allclose(sol.ye,
-                               np.array([[-1.262468e+00, 1.162918e-05, 4.956687e-06, 1.049574e+00],
-                                         [1.200024e+00, 1.455118e-09, 6.495375e-05, -1.049349e+00]]),
-                               rtol=1e-5,
-                               atol=0)
+import numpy as np
+from Solverz import Ode, Var, Opt, Rodas, made_numerical, TimeVars, Model
+
+
+# %% event test
+def test_bounceball():
+    m = Model()
+    m.x = Var('x', [0, 20])
+    m.f1 = Ode('f1', m.x[1], m.x[0])
+    m.f2 = Ode('f2', -9.8, m.x[1])
+    bball, y0 = m.create_instance()
+    nbball = made_numerical(bball, y0, sparse=True)
+
+    def events(t, y):
+        value = np.array([y[0]])
+        isterminal = np.array([1])
+        direction = np.array([-1])
+        return value, isterminal, direction
+
+    opt = Opt(event=events)
+    tout = np.array([0])
+    yout = TimeVars(y0, 1)
+    teout = np.array([])
+    yeout = TimeVars(y0, 0)
+    ieout = np.array([], dtype=int)
+    tstart = 0
+    tend = 30
+    for i in range(10):
+        sol = Rodas(nbball, np.linspace(tstart, tend, 100), y0, opt)
+
+        tout = np.concatenate([tout, sol.T[1:]])
+        yout.append(sol.Y[1:])
+        teout = np.concatenate([teout, sol.te])
+        yeout.append(sol.ye)
+        ieout = np.concatenate([ieout, sol.ie])
+
+        y0['x'][0] = 0
+        y0['x'][1] = -0.9 * sol.Y[-1]['x'][1]
+        tstart = sol.T[-1]
+
+    np.testing.assert_allclose(teout,
+                               np.array([4.081633047365558, 7.755103268847604, 11.061226369910107, 14.03673684129459,
+                                         16.714695668619328, 19.124858513456523, 21.294005283692695, 23.246237159791765,
+                                         25.003245923211466, 26.584554164220997]),
+                               rtol=1e-5,
+                               atol=0)
+
+
+def test_orbit():
+    mu = 1 / 82.45
+    mustar = 1 - mu
+    m = Model()
+    m.y = Var('y', [1.2, 0, 0, -1.04935750983031990726])
+    m.f1 = Ode('f1', m.y[2], m.y[0])
+    m.f2 = Ode('f2', m.y[3], m.y[1])
+    r13 = ((m.y[0] + mu) ** 2 + m.y[1] ** 2) ** 1.5
+    r23 = ((m.y[0] - mustar) ** 2 + m.y[1] ** 2) ** 1.5
+    m.f3 = Ode('f3',
+               2 * m.y[3] + m.y[0] - mustar * ((m.y[0] + mu) / r13) - mu * ((m.y[0] - mustar) / r23),
+               m.y[2])
+    m.f4 = Ode('f4',
+               -2 * m.y[2] + m.y[1] - mustar * (m.y[1] / r13) - mu * (m.y[1] / r23),
+               m.y[3])
+    orbit, y0 = m.create_instance()
+    norbit = made_numerical(orbit, y0, sparse=True)
+
+    def events(t, y):
+        dDSQdt = 2 * (y[0:2] - np.array([1.2, 0])).dot(y[2:4])
+        value = np.array([dDSQdt, dDSQdt])
+        isterminal = np.array([1, 0])
+        direction = np.array([1, -1])
+        return value, isterminal, direction
+
+    sol = Rodas(norbit, [0, 7], y0, Opt(event=events, rtol=1e-5, atol=1e-4))
+
+    np.testing.assert_allclose(sol.te,
+                               np.array([3.09609516, 6.19215951]),
+                               rtol=1e-5,
+                               atol=0)
+    np.testing.assert_allclose(sol.ye,
+                               np.array([[-1.262468e+00, 1.162918e-05, 4.956687e-06, 1.049574e+00],
+                                         [1.200024e+00, 1.455118e-09, 6.495375e-05, -1.049349e+00]]),
+                               rtol=1e-5,
+                               atol=0)
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/functions.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/functions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,574 +1,574 @@
-from functools import reduce
-
-from sympy import Symbol, Function, Number, S, Integer, sin as Symsin, cos as Symcos
-from sympy.core.function import ArgumentIndexError
-
-from Solverz.variable.ssymbol import sSym2Sym
-
-
-# %% miscellaneous
-class F(Function):
-    """
-    For the usage of denoting the function being differentiated in EqnDiff object only
-    """
-    pass
-
-
-# %%
-def VarParser(cls):
-    # To convert non-sympy symbols to sympy symbols
-    original_new = cls.__new__
-
-    def new_new(cls, *args, **options):
-        # check arg types and do the conversions
-        args = [sSym2Sym(arg) for arg in args]
-        return original_new(cls, *args, **options)
-
-    cls.__new__ = new_new
-    return cls
-
-
-# %% matrix func
-@VarParser
-class MatrixFunction(Function):
-    """
-    The basic Function class of matrix computation
-    """
-    is_commutative = False
-    dim = 2
-
-
-class transpose(MatrixFunction):
-    @classmethod
-    def eval(cls, *args):
-        if len(args) > 1:
-            raise TypeError(f'Supports one operand while {len(args)} input!')
-
-
-class Mat_Mul(MatrixFunction):
-
-    @classmethod
-    def eval(cls, *args):
-        # This is to simplify the `0`, `1` and `-1` derived by matrix calculus, which shall be removed
-        # by further improvements of the matrix calculus module.
-        i = 0
-        args = list(args)
-        for arg in args:
-            if arg == S.Zero:
-                return 0
-            elif arg == S.NegativeOne:
-                del args[i]
-                if len(args) > 1:
-                    return -Mat_Mul(*args)
-                else:
-                    if i > 0:
-                        return - args[0]
-                    else:
-                        return - args[1]
-            elif arg == S.One:
-                del args[i]
-                if len(args) > 1:
-                    return Mat_Mul(*args)
-                else:
-                    if i > 0:
-                        return args[0]
-                    else:
-                        return args[1]
-            i = i + 1
-
-    def __repr__(self):
-        return self.__str__()
-
-    def _latex(self, printer, **kwargs):
-
-        arg_latex_str = []
-        for arg in self.args:
-            if isinstance(arg, Symbol):
-                arg_latex_str = [*arg_latex_str, printer._print(arg)]
-            else:
-                arg_latex_str = [*arg_latex_str, r'\left (' + printer._print(arg) + r'\right )']
-        _latex_str = arg_latex_str[0]
-        for arg_latex_str_ in arg_latex_str[1:]:
-            _latex_str = _latex_str + arg_latex_str_
-        if 'exp' in kwargs.keys():
-            return r'\left (' + _latex_str + r'\right )^{' + kwargs['exp'] + r'}'
-        else:
-            return _latex_str
-
-    def _sympystr(self, printer, **kwargs):
-        temp = printer._print(self.args[0])
-        for arg in self.args[1:]:
-            if isinstance(arg, (Symbol, Function)):
-                temp += '@{operand}'.format(operand=printer._print(arg))
-            else:
-                temp += '@({operand})'.format(operand=printer._print(arg))
-        return temp
-
-    def _numpycode(self, printer, **kwargs):
-
-        temp = printer._print(self.args[0])
-        for arg in self.args[1:]:
-            if isinstance(arg, (Symbol, Function)):
-                temp += '@{operand}'.format(operand=printer._print(arg))
-            else:
-                temp += '@({operand})'.format(operand=printer._print(arg))
-        return r'(' + temp + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Diag(MatrixFunction):
-
-    @classmethod
-    def eval(cls, *args):
-        if len(args) > 1:
-            raise TypeError(f"Diagonal takes 1 positional arguments but {len(args)} were given!")
-
-        if args[0] == S.Zero:
-            return 0
-        elif isinstance(args[0], Number):
-            return args[0]
-
-    def _sympystr(self, printer, **kwargs):
-
-        temp = 'diag({operand})'.format(operand=printer._print(self.args[0]))
-
-        return temp
-
-    def _latex(self, printer, **kwargs):
-
-        _latex_str = r'\operatorname{diag}\left (' + printer._print(self.args[0]) + r'\right )'
-        if 'exp' in kwargs.keys():
-            return r'\left (' + _latex_str + r'\right )^{' + kwargs['exp'] + r'}'
-        else:
-            return _latex_str
-
-    def _numpycode(self, printer, **kwargs):
-
-        return r'diagflat(' + printer._print(self.args[0], **kwargs) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-# %% Univariate func
-@VarParser
-class UniVarFunc(Function):
-    @classmethod
-    def eval(cls, *args):
-        if len(args) != 1:
-            raise TypeError(f'Supports one operand while {len(args)} input!')
-
-
-class Abs(UniVarFunc):
-    r"""
-    The element-wise absolute value function:
-
-        .. math::
-
-            \operatorname{Abs}(x)=|x|
-
-    with derivative
-
-        .. math::
-
-            \frac{\mathrm{d}}{\mathrm{d}x}{\operatorname{Abs}}(x)=\operatorname{Sign}(x).
-
-    """
-    def fdiff(self, argindex=1):
-        """
-        Get the first derivative of the argument to Abs().
-        """
-        if argindex == 1:
-            return Sign(self.args[0])
-        else:
-            raise ArgumentIndexError(self, argindex)
-
-    def _numpycode(self, printer, **kwargs):
-        return r'abs(' + printer._print(self.args[0]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class exp(UniVarFunc):
-    r"""
-    The exponential function, $e^x$.
-    """
-    def fdiff(self, argindex=1):
-        return exp(*self.args)
-
-    def _numpycode(self, printer, **kwargs):
-        return r'exp(' + printer._print(self.args[0]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class sin(UniVarFunc):
-    r"""
-    The sine function.
-    """
-    def fdiff(self, argindex=1):
-        if argindex == 1:
-            return Symcos(self.args[0])
-        else:
-            raise ArgumentIndexError(self, argindex)
-
-    def _numpycode(self, printer, **kwargs):
-        return r'sin(' + printer._print(self.args[0]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class cos(UniVarFunc):
-    r"""
-    The cosine function.
-    """
-    def fdiff(self, argindex=1):
-        if argindex == 1:
-            return -Symsin(self.args[0])
-        else:
-            raise ArgumentIndexError(self, argindex)
-
-    def _numpycode(self, printer, **kwargs):
-        return r'cos(' + printer._print(self.args[0]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Sign(UniVarFunc):
-    r"""
-    The element-wise indication of the sign of a number
-
-        .. math::
-
-            \operatorname{Sign}(x)=
-            \begin{cases}
-            1&x> 0\\
-            0& x==0\\
-            -1&x< 0
-            \end{cases}
-
-    """
-    def fdiff(self, argindex=1):
-        # sign function should be treated as a constant.
-        if argindex == 1:
-            return 0
-        raise ArgumentIndexError(self, argindex)
-
-    def _numpycode(self, printer, **kwargs):
-        return r'sign(' + printer._print(self.args[0], **kwargs) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-# %% multi-variate func
-@VarParser
-class MulVarFunc(Function):
-    pass
-
-
-class minmod_flag(MulVarFunc):
-    """
-    Different from `minmod`, minmod function outputs the position of args instead of the values of args.
-    """
-
-    @classmethod
-    def eval(cls, *args):
-        if len(args) != 3:
-            raise TypeError(f"minmod takes 3 positional arguments but {len(args)} were given!")
-
-
-class switch(MulVarFunc):
-    def _eval_derivative(self, s):
-        return switch(*[arg.diff(s) for arg in self.args[0:len(self.args) - 1]], self.args[-1])
-
-    def _numpycode(self, printer, **kwargs):
-        return r'switch(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Saturation(MulVarFunc):
-    r"""
-    The element-wise saturation a number
-
-        .. math::
-
-            \operatorname{Saturation}(v, v_\min, v_\max)=
-            \begin{cases}
-            v_\max&v> v_\max\\
-            v& v_\min\leq v\leq v_\max\\
-            v_\min&v< v_\min
-            \end{cases}
-    """
-    @classmethod
-    def eval(cls, v, vmin, vmax):
-        return v * In(v, vmin, vmax) + vmax * GreaterThan(v, vmax) + vmin * LessThan(v, vmin)
-
-
-class AntiWindUp(MulVarFunc):
-    r"""
-    For PI controller
-
-        .. math::
-
-            \begin{aligned}
-                \dot{z}(t) & =e(t) \\
-                u_{d e s}(t) & =K_p e(t)+K_i z(t)
-            \end{aligned},
-
-    we limit the integrator output by setting, in the $K_i>0$ case,
-
-        .. math::
-
-            \dot{z}(t)=
-            \begin{cases}
-                0 & \text { if } u_{\text {des }}(t) \geq u_{\max } \text { and } e(t) \geq 0 \\
-                0 & \text { if } u_{\text {des }}(t) \leq u_{\min } \text { and } e(t) \leq 0 \\
-                e(t) & \text { otherwise }
-            \end{cases}.
-
-    So the AntiWindUp function reads
-
-        .. math::
-
-            \dot{z}(t)=
-            \operatorname{AntiWindUp}(u_{\text {des }}(t), u_{\min }, u_{\max }, e(t)).
-
-    """
-
-    @classmethod
-    def eval(cls, u, umin, umax, e):
-        return e * Not(Or(And(GreaterThan(u, umax),
-                              GreaterThan(e, 0)),
-                          And(LessThan(u, umin),
-                              LessThan(e, 0))
-                          ))
-
-
-class Min(MulVarFunc):
-    r"""
-    The element-wise minimum of two numbers
-
-    .. math::
-
-        \begin{split}\min(x,y)=
-        \begin{cases}
-        x&x\leq y\\
-        y& x>y
-        \end{cases}\end{split}
-
-    """
-    @classmethod
-    def eval(cls, x, y):
-        return x * LessThan(x, y) + y * (1 - LessThan(x, y))
-
-
-class In(MulVarFunc):
-    """
-    In(v, vmin, vmax)
-        return True if vmin<=v<=vmax
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})<=({op2})<=({op3}))'.format(op1=printer._print(self.args[1]),
-                                                    op2=printer._print(self.args[0]),
-                                                    op3=printer._print(self.args[2]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'SolIn(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class GreaterThan(MulVarFunc):
-    """
-    Represents > operator
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})>({op2}))'.format(op1=printer._print(self.args[0]),
-                                           op2=printer._print(self.args[1]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'SolGreaterThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class LessThan(MulVarFunc):
-    """
-    Represents < operator
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})<({op2}))'.format(op1=printer._print(self.args[0]),
-                                           op2=printer._print(self.args[1]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'SolLessThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class And(MulVarFunc):
-    """
-    Represents bitwise_and
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})&({op2}))'.format(op1=printer._print(self.args[0]),
-                                          op2=printer._print(self.args[1]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'And(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Or(MulVarFunc):
-    """
-    Represents bitwise_or
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})|({op2}))'.format(op1=printer._print(self.args[0]),
-                                          op2=printer._print(self.args[1]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'Or(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Not(MulVarFunc):
-    """
-    Represents bitwise_not
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '({op1})'.format(op1=printer._print(self.args[0]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'Not(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-# %% custom func of equation printer
-class Slice(Function):
-
-    @classmethod
-    def eval(cls, *args):
-        if len(args) > 3:
-            raise TypeError(f"minmod takes at most 3 positional arguments but {len(args)} were given!")
-
-
-class zeros(Function):
-    # print zeros(6,6) as zeros((6,6))
-    # or zeros(6,) as zeros((6,))
-    def _numpycode(self, printer, **kwargs):
-        if len(self.args) == 2:
-            temp1 = printer._print(self.args[0])
-            temp2 = printer._print(self.args[1])
-            return r'zeros((' + temp1 + ', ' + temp2 + r'))'
-        elif len(self.args) == 1:
-            temp = printer._print(self.args[0])
-            return r'zeros((' + temp + ', ' + r'))'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class CSC_array(Function):
-
-    @classmethod
-    def eval(cls, *args):
-        if len(args) != 1:
-            raise TypeError(f"CSC_array takes 1 positional arguments but {len(args)} were given!")
-
-    def _numpycode(self, printer, **kwargs):
-        return r'csc_array(' + printer._print(self.args[0]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class Arange(Function):
-    """
-    Solverz' arange function
-    """
-
-    @classmethod
-    def eval(cls, *args):
-        if any([not isinstance(arg, Integer) for arg in args]):
-            raise ValueError(f"Solverz' arange object accepts only integer inputs.")
-        if len(args) > 2:
-            raise ValueError(f"Solverz' arange object takes 2 positional arguments but {len(args)} were given!")
-
-    def _numpycode(self, printer, **kwargs):
-        return r'arange(' + ', '.join([printer._print(arg) for arg in self.args]) + r')'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
+from functools import reduce
+
+from sympy import Symbol, Function, Number, S, Integer, sin as Symsin, cos as Symcos
+from sympy.core.function import ArgumentIndexError
+
+from Solverz.variable.ssymbol import sSym2Sym
+
+
+# %% miscellaneous
+class F(Function):
+    """
+    For the usage of denoting the function being differentiated in EqnDiff object only
+    """
+    pass
+
+
+# %%
+def VarParser(cls):
+    # To convert non-sympy symbols to sympy symbols
+    original_new = cls.__new__
+
+    def new_new(cls, *args, **options):
+        # check arg types and do the conversions
+        args = [sSym2Sym(arg) for arg in args]
+        return original_new(cls, *args, **options)
+
+    cls.__new__ = new_new
+    return cls
+
+
+# %% matrix func
+@VarParser
+class MatrixFunction(Function):
+    """
+    The basic Function class of matrix computation
+    """
+    is_commutative = False
+    dim = 2
+
+
+class transpose(MatrixFunction):
+    @classmethod
+    def eval(cls, *args):
+        if len(args) > 1:
+            raise TypeError(f'Supports one operand while {len(args)} input!')
+
+
+class Mat_Mul(MatrixFunction):
+
+    @classmethod
+    def eval(cls, *args):
+        # This is to simplify the `0`, `1` and `-1` derived by matrix calculus, which shall be removed
+        # by further improvements of the matrix calculus module.
+        i = 0
+        args = list(args)
+        for arg in args:
+            if arg == S.Zero:
+                return 0
+            elif arg == S.NegativeOne:
+                del args[i]
+                if len(args) > 1:
+                    return -Mat_Mul(*args)
+                else:
+                    if i > 0:
+                        return - args[0]
+                    else:
+                        return - args[1]
+            elif arg == S.One:
+                del args[i]
+                if len(args) > 1:
+                    return Mat_Mul(*args)
+                else:
+                    if i > 0:
+                        return args[0]
+                    else:
+                        return args[1]
+            i = i + 1
+
+    def __repr__(self):
+        return self.__str__()
+
+    def _latex(self, printer, **kwargs):
+
+        arg_latex_str = []
+        for arg in self.args:
+            if isinstance(arg, Symbol):
+                arg_latex_str = [*arg_latex_str, printer._print(arg)]
+            else:
+                arg_latex_str = [*arg_latex_str, r'\left (' + printer._print(arg) + r'\right )']
+        _latex_str = arg_latex_str[0]
+        for arg_latex_str_ in arg_latex_str[1:]:
+            _latex_str = _latex_str + arg_latex_str_
+        if 'exp' in kwargs.keys():
+            return r'\left (' + _latex_str + r'\right )^{' + kwargs['exp'] + r'}'
+        else:
+            return _latex_str
+
+    def _sympystr(self, printer, **kwargs):
+        temp = printer._print(self.args[0])
+        for arg in self.args[1:]:
+            if isinstance(arg, (Symbol, Function)):
+                temp += '@{operand}'.format(operand=printer._print(arg))
+            else:
+                temp += '@({operand})'.format(operand=printer._print(arg))
+        return temp
+
+    def _numpycode(self, printer, **kwargs):
+
+        temp = printer._print(self.args[0])
+        for arg in self.args[1:]:
+            if isinstance(arg, (Symbol, Function)):
+                temp += '@{operand}'.format(operand=printer._print(arg))
+            else:
+                temp += '@({operand})'.format(operand=printer._print(arg))
+        return r'(' + temp + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Diag(MatrixFunction):
+
+    @classmethod
+    def eval(cls, *args):
+        if len(args) > 1:
+            raise TypeError(f"Diagonal takes 1 positional arguments but {len(args)} were given!")
+
+        if args[0] == S.Zero:
+            return 0
+        elif isinstance(args[0], Number):
+            return args[0]
+
+    def _sympystr(self, printer, **kwargs):
+
+        temp = 'diag({operand})'.format(operand=printer._print(self.args[0]))
+
+        return temp
+
+    def _latex(self, printer, **kwargs):
+
+        _latex_str = r'\operatorname{diag}\left (' + printer._print(self.args[0]) + r'\right )'
+        if 'exp' in kwargs.keys():
+            return r'\left (' + _latex_str + r'\right )^{' + kwargs['exp'] + r'}'
+        else:
+            return _latex_str
+
+    def _numpycode(self, printer, **kwargs):
+
+        return r'diagflat(' + printer._print(self.args[0], **kwargs) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+# %% Univariate func
+@VarParser
+class UniVarFunc(Function):
+    @classmethod
+    def eval(cls, *args):
+        if len(args) != 1:
+            raise TypeError(f'Supports one operand while {len(args)} input!')
+
+
+class Abs(UniVarFunc):
+    r"""
+    The element-wise absolute value function:
+
+        .. math::
+
+            \operatorname{Abs}(x)=|x|
+
+    with derivative
+
+        .. math::
+
+            \frac{\mathrm{d}}{\mathrm{d}x}{\operatorname{Abs}}(x)=\operatorname{Sign}(x).
+
+    """
+    def fdiff(self, argindex=1):
+        """
+        Get the first derivative of the argument to Abs().
+        """
+        if argindex == 1:
+            return Sign(self.args[0])
+        else:
+            raise ArgumentIndexError(self, argindex)
+
+    def _numpycode(self, printer, **kwargs):
+        return r'abs(' + printer._print(self.args[0]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class exp(UniVarFunc):
+    r"""
+    The exponential function, $e^x$.
+    """
+    def fdiff(self, argindex=1):
+        return exp(*self.args)
+
+    def _numpycode(self, printer, **kwargs):
+        return r'exp(' + printer._print(self.args[0]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class sin(UniVarFunc):
+    r"""
+    The sine function.
+    """
+    def fdiff(self, argindex=1):
+        if argindex == 1:
+            return Symcos(self.args[0])
+        else:
+            raise ArgumentIndexError(self, argindex)
+
+    def _numpycode(self, printer, **kwargs):
+        return r'sin(' + printer._print(self.args[0]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class cos(UniVarFunc):
+    r"""
+    The cosine function.
+    """
+    def fdiff(self, argindex=1):
+        if argindex == 1:
+            return -Symsin(self.args[0])
+        else:
+            raise ArgumentIndexError(self, argindex)
+
+    def _numpycode(self, printer, **kwargs):
+        return r'cos(' + printer._print(self.args[0]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Sign(UniVarFunc):
+    r"""
+    The element-wise indication of the sign of a number
+
+        .. math::
+
+            \operatorname{Sign}(x)=
+            \begin{cases}
+            1&x> 0\\
+            0& x==0\\
+            -1&x< 0
+            \end{cases}
+
+    """
+    def fdiff(self, argindex=1):
+        # sign function should be treated as a constant.
+        if argindex == 1:
+            return 0
+        raise ArgumentIndexError(self, argindex)
+
+    def _numpycode(self, printer, **kwargs):
+        return r'sign(' + printer._print(self.args[0], **kwargs) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+# %% multi-variate func
+@VarParser
+class MulVarFunc(Function):
+    pass
+
+
+class minmod_flag(MulVarFunc):
+    """
+    Different from `minmod`, minmod function outputs the position of args instead of the values of args.
+    """
+
+    @classmethod
+    def eval(cls, *args):
+        if len(args) != 3:
+            raise TypeError(f"minmod takes 3 positional arguments but {len(args)} were given!")
+
+
+class switch(MulVarFunc):
+    def _eval_derivative(self, s):
+        return switch(*[arg.diff(s) for arg in self.args[0:len(self.args) - 1]], self.args[-1])
+
+    def _numpycode(self, printer, **kwargs):
+        return r'switch(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Saturation(MulVarFunc):
+    r"""
+    The element-wise saturation a number
+
+        .. math::
+
+            \operatorname{Saturation}(v, v_\min, v_\max)=
+            \begin{cases}
+            v_\max&v> v_\max\\
+            v& v_\min\leq v\leq v_\max\\
+            v_\min&v< v_\min
+            \end{cases}
+    """
+    @classmethod
+    def eval(cls, v, vmin, vmax):
+        return v * In(v, vmin, vmax) + vmax * GreaterThan(v, vmax) + vmin * LessThan(v, vmin)
+
+
+class AntiWindUp(MulVarFunc):
+    r"""
+    For PI controller
+
+        .. math::
+
+            \begin{aligned}
+                \dot{z}(t) & =e(t) \\
+                u_{d e s}(t) & =K_p e(t)+K_i z(t)
+            \end{aligned},
+
+    we limit the integrator output by setting, in the $K_i>0$ case,
+
+        .. math::
+
+            \dot{z}(t)=
+            \begin{cases}
+                0 & \text { if } u_{\text {des }}(t) \geq u_{\max } \text { and } e(t) \geq 0 \\
+                0 & \text { if } u_{\text {des }}(t) \leq u_{\min } \text { and } e(t) \leq 0 \\
+                e(t) & \text { otherwise }
+            \end{cases}.
+
+    So the AntiWindUp function reads
+
+        .. math::
+
+            \dot{z}(t)=
+            \operatorname{AntiWindUp}(u_{\text {des }}(t), u_{\min }, u_{\max }, e(t)).
+
+    """
+
+    @classmethod
+    def eval(cls, u, umin, umax, e):
+        return e * Not(Or(And(GreaterThan(u, umax),
+                              GreaterThan(e, 0)),
+                          And(LessThan(u, umin),
+                              LessThan(e, 0))
+                          ))
+
+
+class Min(MulVarFunc):
+    r"""
+    The element-wise minimum of two numbers
+
+    .. math::
+
+        \begin{split}\min(x,y)=
+        \begin{cases}
+        x&x\leq y\\
+        y& x>y
+        \end{cases}\end{split}
+
+    """
+    @classmethod
+    def eval(cls, x, y):
+        return x * LessThan(x, y) + y * (1 - LessThan(x, y))
+
+
+class In(MulVarFunc):
+    """
+    In(v, vmin, vmax)
+        return True if vmin<=v<=vmax
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})<=({op2})<=({op3}))'.format(op1=printer._print(self.args[1]),
+                                                    op2=printer._print(self.args[0]),
+                                                    op3=printer._print(self.args[2]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'SolIn(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class GreaterThan(MulVarFunc):
+    """
+    Represents > operator
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})>({op2}))'.format(op1=printer._print(self.args[0]),
+                                           op2=printer._print(self.args[1]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'SolGreaterThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class LessThan(MulVarFunc):
+    """
+    Represents < operator
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})<({op2}))'.format(op1=printer._print(self.args[0]),
+                                           op2=printer._print(self.args[1]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'SolLessThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class And(MulVarFunc):
+    """
+    Represents bitwise_and
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})&({op2}))'.format(op1=printer._print(self.args[0]),
+                                          op2=printer._print(self.args[1]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'And(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Or(MulVarFunc):
+    """
+    Represents bitwise_or
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})|({op2}))'.format(op1=printer._print(self.args[0]),
+                                          op2=printer._print(self.args[1]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'Or(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Not(MulVarFunc):
+    """
+    Represents bitwise_not
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '({op1})'.format(op1=printer._print(self.args[0]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'Not(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+# %% custom func of equation printer
+class Slice(Function):
+
+    @classmethod
+    def eval(cls, *args):
+        if len(args) > 3:
+            raise TypeError(f"minmod takes at most 3 positional arguments but {len(args)} were given!")
+
+
+class zeros(Function):
+    # print zeros(6,6) as zeros((6,6))
+    # or zeros(6,) as zeros((6,))
+    def _numpycode(self, printer, **kwargs):
+        if len(self.args) == 2:
+            temp1 = printer._print(self.args[0])
+            temp2 = printer._print(self.args[1])
+            return r'zeros((' + temp1 + ', ' + temp2 + r'))'
+        elif len(self.args) == 1:
+            temp = printer._print(self.args[0])
+            return r'zeros((' + temp + ', ' + r'))'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class CSC_array(Function):
+
+    @classmethod
+    def eval(cls, *args):
+        if len(args) != 1:
+            raise TypeError(f"CSC_array takes 1 positional arguments but {len(args)} were given!")
+
+    def _numpycode(self, printer, **kwargs):
+        return r'csc_array(' + printer._print(self.args[0]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class Arange(Function):
+    """
+    Solverz' arange function
+    """
+
+    @classmethod
+    def eval(cls, *args):
+        if any([not isinstance(arg, Integer) for arg in args]):
+            raise ValueError(f"Solverz' arange object accepts only integer inputs.")
+        if len(args) > 2:
+            raise ValueError(f"Solverz' arange object takes 2 positional arguments but {len(args)} were given!")
+
+    def _numpycode(self, printer, **kwargs):
+        return r'arange(' + ', '.join([printer._print(arg) for arg in self.args]) + r')'
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/matrix_calculus.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/matrix_calculus.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,455 +1,455 @@
-from __future__ import annotations
-
-from typing import List, Union, Dict, Tuple
-
-import matplotlib.pyplot as plt
-import networkx as nx
-import numpy as np
-import sympy as sp
-from sympy import Expr, Mul, Add, S, Number, Integer, Symbol
-
-from Solverz.sym_algebra.symbols import IdxVar, IdxPara, iVar, Para
-from Solverz.sym_algebra.functions import Mat_Mul, Diag, transpose, Abs, Sign
-
-
-class TMatrix:
-    def __init__(self, expr: Expr, index: TensorIndex):
-        self.name = expr.name
-        self.index = index
-        self.symbol = expr
-
-    def __repr__(self):
-        return f"{self.name}[{self.index}]"
-
-    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
-    def __hash__(self):
-        return hash(tuple([self.name, *self.index.index]))
-
-    def __eq__(self, other):
-        if not isinstance(other, TMatrix):
-            return False
-        else:
-            if self.name == other.name and self.index.index_value == other.index.index_value:
-                return True
-            else:
-                return False
-
-
-class TVector:
-    def __init__(self, expr: Expr, index: TensorIndex):
-        self.name = expr.name
-        self.index = index
-        self.symbol = expr
-
-    def __repr__(self):
-        return f"{self.name}[{self.index}]"
-
-    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
-    def __hash__(self):
-        return hash(tuple([self.name, *self.index.index]))
-
-    def __eq__(self, other):
-        if not isinstance(other, TVector):
-            return False
-        else:
-            if self.name == other.name and self.index.index_value == other.index.index_value:
-                return True
-            else:
-                return False
-
-
-class TMul:
-
-    def __init__(self, expr: Union[Mul, Mat_Mul], index: TensorIndex):
-        self.args = []
-        self.expr = expr
-        if not isinstance(expr, (Mul, Mat_Mul)):
-            raise TypeError("Unsupported input expression")
-        if len(expr.args) > 2:
-            self.args += [expr.args[0]]
-            self.args += [expr.func(*expr.args[1:])]
-        else:
-            self.args += [expr.args[0]]
-            self.args += [expr.args[1]]
-        dim1, dim2 = [obtain_dim(arg) for arg in self.args]
-        if dim1 == 0:
-            self.index = [TensorIndex(-1), index, index]
-        else:
-            if len(index.index) == 2:
-                # TMul produces a matrix
-                if isinstance(expr, Mul):
-                    # dot product of two matrices
-                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index, index]
-                elif isinstance(expr, Mat_Mul):
-                    if isinstance(expr.args[0], Diag):
-                        # diag(x)@A
-                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index[0], index]
-                    elif isinstance(expr.args[1], Diag):
-                        # A@diag(x)
-                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index[1], index]
-                    else:
-                        # A@B
-                        max_index = max(index.index_value)
-                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
-                            [TensorIndex([index.index_value[0], max_index + 1]),
-                             TensorIndex([max_index + 1, index.index_value[0]]),
-                             index]
-            elif len(index.index) == 1:
-                if dim1 == 2:
-                    # A@y
-                    max_index = max(index.index_value)
-                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
-                        [TensorIndex([index.index_value[0], max_index + 1]),
-                         TensorIndex([max_index + 1]),
-                         index]
-                elif dim1 == 1:
-                    # y*x
-                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
-                        [index, index, index]
-            else:
-                raise TypeError(f"Unsupported index length {len(index.index)}")
-
-    def __repr__(self):
-        # To add self.args here is to differentiate TMul objects with the same index, in which case, graphviz
-        # treats the nodes with the same __repr__() value as one node.
-        return r"$*%s_{%s}$" % (self.index, self.args)
-
-    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
-    def __hash__(self):
-        return hash(tuple([*self.args, self.__repr__()]))
-
-    def __eq__(self, other):
-        if not isinstance(other, TMul):
-            return False
-        else:
-            if self.args == other.args and self.__repr__() == other.__repr__():
-                return True
-            else:
-                return False
-
-
-class TAdd:
-
-    def __init__(self, expr: Add, index: TensorIndex):
-        if not isinstance(expr, Add):
-            raise TypeError("Input expression is not Add")
-
-        self.index = index
-        self.expr = expr
-        self.args = expr.args
-
-    def _eval_derivative(self, s):
-        pass
-
-    def __repr__(self):
-        return f"+[{self.index}]"
-
-    def __hash__(self):
-        return hash(tuple([*self.args, self.__repr__()]))
-
-    def __eq__(self, other):
-        if not isinstance(other, TAdd):
-            return False
-        else:
-            if self.args == other.args and self.__repr__() == other.__repr__():
-                return True
-            else:
-                return False
-
-
-class TAbs:
-
-    def __init__(self, expr: Abs, index: TensorIndex):
-        if not isinstance(expr, Abs):
-            raise TypeError("Input expression is not Abs")
-
-        self.index: TensorIndex = index
-        self.expr = expr
-        self.args = expr.args
-
-    def __repr__(self):
-        return f"$Abs_{self.index}$"
-
-    def __hash__(self):
-        return hash(tuple([*self.args, self.__repr__()]))
-
-    def __eq__(self, other):
-        if not isinstance(other, TAbs):
-            return False
-        else:
-            if self.args == other.args and self.__repr__() == other.__repr__():
-                return True
-            else:
-                return False
-
-
-class TNumber:
-
-    def __init__(self, expr: Number):
-        if not isinstance(expr, Number):
-            raise TypeError("Input expression is not Number")
-        self.name = expr.__repr__()
-        self.index: TensorIndex = TensorIndex(-1)
-        self.expr = expr
-        self.args = expr.args
-
-    def __repr__(self):
-        return self.expr.__repr__()
-
-
-index_list = [chr(ord('i') + i) for i in range(18)]
-
-
-class TensorIndex:
-
-    def __init__(self, index_value):
-        if isinstance(index_value, (int, float)):
-            index_value = [index_value]
-        self.index_value = index_value
-
-    @property
-    def index(self) -> str:
-        return ''.join([index_list[idx] if idx >= 0 else '' for idx in self.index_value])
-
-    def __getitem__(self, item):
-        if not isinstance(item, int):
-            raise TypeError(f"Unsupported index type {type(item)}")
-        else:
-            return self.index[item]
-
-    def __repr__(self):
-        return self.index
-
-    def __eq__(self, other):
-        if not isinstance(other, TensorIndex):
-            raise TypeError(f"Unsupported type {type(other)}")
-
-        if self.index_value == other.index_value:
-            return True
-        else:
-            return False
-
-
-def obtain_dim(expr) -> int:
-    """
-    # Evaluate the expr to decide its dimension
-    """
-    if expr == S.NegativeOne or isinstance(expr, Number):
-        return 0
-
-    symbol_dict = dict()
-    for symbol in list(expr.free_symbols):
-        if isinstance(symbol, (iVar, IdxVar)):
-            symbol_dict[symbol] = np.ones((2, 1))
-        elif isinstance(symbol, (Para, IdxPara)):
-            if symbol.dim == 2:
-                symbol_dict[symbol] = np.ones((2, 2))
-            elif symbol.dim == 1:
-                symbol_dict[symbol] = np.ones((2, 1))
-    temp_expr = sp.lambdify(symbol_dict.keys(), expr)
-    return temp_expr(*symbol_dict.values()).shape[1]
-
-
-def obtain_TExpr(expr: Expr, index: TensorIndex):
-    """
-    Convert Expr to TOperator and its args
-
-    """
-
-    if isinstance(expr, Add):
-        Texpr = TAdd(expr, index)
-    elif isinstance(expr, (Mat_Mul, Mul)):
-        Texpr = TMul(expr, index)
-    elif isinstance(expr, Abs):
-        Texpr = TAbs(expr, index)
-    elif isinstance(expr, (iVar, IdxVar)):
-        Texpr = TVector(expr, index)
-    elif isinstance(expr, (Para, IdxPara)):
-        if expr.dim == 2:
-            Texpr = TMatrix(expr, index)
-        elif expr.dim == 1:
-            Texpr = TVector(expr, index)
-        else:
-            TypeError(f"Unsupported dim {expr.dim}")
-    elif isinstance(expr, Number):
-        Texpr = TNumber(expr)
-    else:
-        raise NotImplementedError(f"Unsupported expression type {type(expr)}")
-    return Texpr
-
-
-def ToComGraph(expr: Expr) -> nx.DiGraph:
-    DG = nx.DiGraph()
-    output_dim = obtain_dim(expr)
-    if output_dim == 2:
-        index = TensorIndex([0, 1])
-    elif output_dim == 1:
-        index = TensorIndex([0])
-    else:
-        raise TypeError("Unsupported output dim")
-    queue = [(expr, index, None)]  # [(Expr, TensorIndex, predecessor)]
-
-    while queue:
-        current_expr, index, predecessor = queue.pop(0)
-
-        Texpr = obtain_TExpr(current_expr, index)
-
-        if predecessor is not None:
-            DG.add_edge(predecessor, Texpr)
-            DG.nodes[Texpr]['level'] = DG.nodes[predecessor]['level'] + 1
-        else:
-            DG.add_node(Texpr)
-            DG.nodes[Texpr]['level'] = 0
-
-        if isinstance(Texpr, TMul):
-            queue.append((Texpr.args[0], TensorIndex(Texpr.index[0].index_value), Texpr))
-            queue.append((Texpr.args[1], TensorIndex(Texpr.index[1].index_value), Texpr))
-        elif isinstance(Texpr, TAdd):
-            for subexpr in Texpr.args:
-                queue.append((subexpr, TensorIndex(Texpr.index.index_value), Texpr))
-        elif isinstance(Texpr, TAbs):
-            queue.append((Texpr.args[0], TensorIndex(Texpr.index.index_value), Texpr))
-
-    # Check for and remove any cycles to ensure acyclic graph
-    if not nx.is_directed_acyclic_graph(DG):
-        raise ValueError("The expression contains cycles.")
-
-    return DG
-
-
-def draw_dag_as_tree(G, pos=None):
-    # using Graphviz and pygraphviz to draw directed acyclic expression graph as a 'tree'
-
-    if pos is None:
-        pos = nx.nx_agraph.graphviz_layout(G, prog='dot')
-
-    nx.draw_networkx_nodes(G, pos, node_size=800, node_color='lightblue')
-    root_node = [node for node in G.nodes() if G.in_degree(node) == 0]
-    leaf_node = [node for node in G.nodes() if G.out_degree(node) == 0]
-    nx.draw_networkx_nodes(G, pos, nodelist=root_node, node_size=800, node_color='lightgreen')
-    nx.draw_networkx_nodes(G, pos, nodelist=leaf_node, node_size=800)
-    nx.draw_networkx_labels(G, pos)
-    nx.draw_networkx_edges(G, pos, arrowstyle='-|>', arrowsize=15)
-
-    plt.axis('off')
-    plt.show()
-
-
-def TMul2Mul(x, y, index: List[TensorIndex, TensorIndex, TensorIndex]):
-    if x is S.Zero or y is S.Zero:
-        return 0
-    s1, s2, s3 = index[:]
-    if s1 == TensorIndex(-1) or s2 == TensorIndex(-1):
-        return x * y
-    if len(s1.index) < 2:
-        if len(s2.index) < 2:
-            # i, j, ij
-            if s1.index_value[0] != s2.index_value[0]:
-                return Mat_Mul(x, transpose(y))
-            # i, i, i
-            if s1.index_value[0] == s2.index_value[0]:
-                return x * y
-        else:
-            # j, jj, jj
-            if s2.index_value[0] == s2.index_value[1] == s1.index_value[0]:
-                if isinstance(y, Diag):
-                    return Diag(x * y.args[0])
-                else:
-                    return Diag(x * y)
-            # i, ij, ij
-            if s2.index_value[0] != s2.index_value[1] and s1.index_value[0] == s2.index_value[0]:
-                return Mat_Mul(Diag(x), y)
-    else:
-        if len(s2.index) < 2:
-            # jj, j, jj
-            if s1.index_value[0] == s1.index_value[1] == s2.index_value[0]:
-                if isinstance(x, Diag):
-                    return Diag(x.args[0] * y)
-            # ij, j, i
-            if s1.index_value[0] != s1.index_value[1] and s1.index_value[1] == s2.index_value[0]:
-                return Mat_Mul(x, y)
-        else:
-            # ij, ij, ij
-            if s1.index_value == s2.index_value and s1.index_value[0] != s1.index_value[1]:
-                return x * y
-            # ij, jj, ij
-            if s1 == s3 and s2.index_value[0] == s2.index_value[1] and s1.index_value[1] == s2.index_value[0]:
-                if isinstance(y, Number):
-                    return y * x
-                elif isinstance(y, Diag):
-                    return Mat_Mul(x, y)
-            # ij, jk, ik
-            if s1.index_value != s2.index_value and s1.index_value[1] == s2.index_value[0]:
-                return Mat_Mul(x, y)
-        return NotImplementedError("Unsupport index type!")
-
-
-class TensorExpr:
-
-    def __init__(self, expr: Expr):
-        self.ComGraph = ToComGraph(expr)
-        self.index = TensorIndex([0])
-
-    def visualize(self):
-        """
-        To visualize TensorExpr
-        """
-        draw_dag_as_tree(self.ComGraph)
-
-    def diff(self, s):
-
-        leaf_node = [node for node in self.ComGraph.nodes() if self.ComGraph.out_degree(node) == 0]
-        index_s = None
-        for node in leaf_node:
-            if node.name == s.name:
-                index_s = node.index
-        if index_s is None:
-            raise TypeError(f"Cant find index of {s}")
-
-        highest_level = np.max([attr['level'] for node, attr in self.ComGraph.nodes(data=True)])
-        derivatives: Dict[Union[TMatrix, TVector, TMul, TAdd, TAbs, TNumber], Tuple[Expr, TensorIndex]] = dict()
-        for level in range(highest_level, -1, -1):
-            current_nodes = [node for node, attr in self.ComGraph.nodes(data=True) if attr['level'] == level]
-            for node in current_nodes:
-                if isinstance(node, (TMatrix, TVector)):
-                    derivatives[node] = (node.symbol.diff(s), node.index)
-                elif isinstance(node, TAdd):
-                    succ = list(self.ComGraph.successors(node))
-                    derivatives[node] = (Add(*[derivatives[arg][0] for arg in succ]), derivatives[succ[0]][1])
-                elif isinstance(node, TAbs):
-                    succ = list(self.ComGraph.successors(node))
-                    s1 = derivatives[succ[0]][1]
-                    s2 = index_s
-                    Aprime = derivatives[succ[0]][0]
-                    fprimeA = Sign(node.args[0])
-                    s1s2 = TensorIndex(s1.index_value + s2.index_value)
-
-                    derivatives[node] = (TMul2Mul(fprimeA, Aprime, [s1, s1s2, s1s2]),
-                                         s1s2)
-                elif isinstance(node, TMul):
-                    succ = list(self.ComGraph.successors(node))
-                    s4 = index_s
-                    s1 = node.index[0]
-                    s2 = node.index[1]
-                    s3 = node.index[2]
-                    A = node.args[0]
-                    B = node.args[1]
-                    Aprime = derivatives[succ[0]][0]
-                    Bprime = derivatives[succ[1]][0]
-                    s1s4 = TensorIndex(s1.index_value + s4.index_value)
-                    s3s4 = TensorIndex(s3.index_value + s4.index_value)
-                    s2s4 = TensorIndex(s2.index_value + s4.index_value)
-                    derivatives[node] = (TMul2Mul(B, Aprime, [s2, s1s4, s3s4]) + TMul2Mul(A, Bprime, [s1, s2s4, s3s4]),
-                                         s3s4)
-                elif isinstance(node, TNumber):
-                    derivatives[node] = (Integer(0), TensorIndex(-1))
-        root_node = [node for node in self.ComGraph.nodes() if self.ComGraph.in_degree(node) == 0]
-        return derivatives[root_node[0]][0]
-
-
-def MixedEquationDiff(expr: Expr, symbol: Symbol):
-    """
-    Calculate the derivatives of mixed-Matrix-Vector equations
-
-    """
-    return TensorExpr(expr).diff(symbol)
+from __future__ import annotations
+
+from typing import List, Union, Dict, Tuple
+
+import matplotlib.pyplot as plt
+import networkx as nx
+import numpy as np
+import sympy as sp
+from sympy import Expr, Mul, Add, S, Number, Integer, Symbol
+
+from Solverz.sym_algebra.symbols import IdxVar, IdxPara, iVar, Para
+from Solverz.sym_algebra.functions import Mat_Mul, Diag, transpose, Abs, Sign
+
+
+class TMatrix:
+    def __init__(self, expr: Expr, index: TensorIndex):
+        self.name = expr.name
+        self.index = index
+        self.symbol = expr
+
+    def __repr__(self):
+        return f"{self.name}[{self.index}]"
+
+    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
+    def __hash__(self):
+        return hash(tuple([self.name, *self.index.index]))
+
+    def __eq__(self, other):
+        if not isinstance(other, TMatrix):
+            return False
+        else:
+            if self.name == other.name and self.index.index_value == other.index.index_value:
+                return True
+            else:
+                return False
+
+
+class TVector:
+    def __init__(self, expr: Expr, index: TensorIndex):
+        self.name = expr.name
+        self.index = index
+        self.symbol = expr
+
+    def __repr__(self):
+        return f"{self.name}[{self.index}]"
+
+    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
+    def __hash__(self):
+        return hash(tuple([self.name, *self.index.index]))
+
+    def __eq__(self, other):
+        if not isinstance(other, TVector):
+            return False
+        else:
+            if self.name == other.name and self.index.index_value == other.index.index_value:
+                return True
+            else:
+                return False
+
+
+class TMul:
+
+    def __init__(self, expr: Union[Mul, Mat_Mul], index: TensorIndex):
+        self.args = []
+        self.expr = expr
+        if not isinstance(expr, (Mul, Mat_Mul)):
+            raise TypeError("Unsupported input expression")
+        if len(expr.args) > 2:
+            self.args += [expr.args[0]]
+            self.args += [expr.func(*expr.args[1:])]
+        else:
+            self.args += [expr.args[0]]
+            self.args += [expr.args[1]]
+        dim1, dim2 = [obtain_dim(arg) for arg in self.args]
+        if dim1 == 0:
+            self.index = [TensorIndex(-1), index, index]
+        else:
+            if len(index.index) == 2:
+                # TMul produces a matrix
+                if isinstance(expr, Mul):
+                    # dot product of two matrices
+                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index, index]
+                elif isinstance(expr, Mat_Mul):
+                    if isinstance(expr.args[0], Diag):
+                        # diag(x)@A
+                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index[0], index]
+                    elif isinstance(expr.args[1], Diag):
+                        # A@diag(x)
+                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = [index, index[1], index]
+                    else:
+                        # A@B
+                        max_index = max(index.index_value)
+                        self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
+                            [TensorIndex([index.index_value[0], max_index + 1]),
+                             TensorIndex([max_index + 1, index.index_value[0]]),
+                             index]
+            elif len(index.index) == 1:
+                if dim1 == 2:
+                    # A@y
+                    max_index = max(index.index_value)
+                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
+                        [TensorIndex([index.index_value[0], max_index + 1]),
+                         TensorIndex([max_index + 1]),
+                         index]
+                elif dim1 == 1:
+                    # y*x
+                    self.index: List[TensorIndex, TensorIndex, TensorIndex] = \
+                        [index, index, index]
+            else:
+                raise TypeError(f"Unsupported index length {len(index.index)}")
+
+    def __repr__(self):
+        # To add self.args here is to differentiate TMul objects with the same index, in which case, graphviz
+        # treats the nodes with the same __repr__() value as one node.
+        return r"$*%s_{%s}$" % (self.index, self.args)
+
+    # __hash__ and __eq__ functions ensure that TMatrix and TVector objects are unique in computation graph.
+    def __hash__(self):
+        return hash(tuple([*self.args, self.__repr__()]))
+
+    def __eq__(self, other):
+        if not isinstance(other, TMul):
+            return False
+        else:
+            if self.args == other.args and self.__repr__() == other.__repr__():
+                return True
+            else:
+                return False
+
+
+class TAdd:
+
+    def __init__(self, expr: Add, index: TensorIndex):
+        if not isinstance(expr, Add):
+            raise TypeError("Input expression is not Add")
+
+        self.index = index
+        self.expr = expr
+        self.args = expr.args
+
+    def _eval_derivative(self, s):
+        pass
+
+    def __repr__(self):
+        return f"+[{self.index}]"
+
+    def __hash__(self):
+        return hash(tuple([*self.args, self.__repr__()]))
+
+    def __eq__(self, other):
+        if not isinstance(other, TAdd):
+            return False
+        else:
+            if self.args == other.args and self.__repr__() == other.__repr__():
+                return True
+            else:
+                return False
+
+
+class TAbs:
+
+    def __init__(self, expr: Abs, index: TensorIndex):
+        if not isinstance(expr, Abs):
+            raise TypeError("Input expression is not Abs")
+
+        self.index: TensorIndex = index
+        self.expr = expr
+        self.args = expr.args
+
+    def __repr__(self):
+        return f"$Abs_{self.index}$"
+
+    def __hash__(self):
+        return hash(tuple([*self.args, self.__repr__()]))
+
+    def __eq__(self, other):
+        if not isinstance(other, TAbs):
+            return False
+        else:
+            if self.args == other.args and self.__repr__() == other.__repr__():
+                return True
+            else:
+                return False
+
+
+class TNumber:
+
+    def __init__(self, expr: Number):
+        if not isinstance(expr, Number):
+            raise TypeError("Input expression is not Number")
+        self.name = expr.__repr__()
+        self.index: TensorIndex = TensorIndex(-1)
+        self.expr = expr
+        self.args = expr.args
+
+    def __repr__(self):
+        return self.expr.__repr__()
+
+
+index_list = [chr(ord('i') + i) for i in range(18)]
+
+
+class TensorIndex:
+
+    def __init__(self, index_value):
+        if isinstance(index_value, (int, float)):
+            index_value = [index_value]
+        self.index_value = index_value
+
+    @property
+    def index(self) -> str:
+        return ''.join([index_list[idx] if idx >= 0 else '' for idx in self.index_value])
+
+    def __getitem__(self, item):
+        if not isinstance(item, int):
+            raise TypeError(f"Unsupported index type {type(item)}")
+        else:
+            return self.index[item]
+
+    def __repr__(self):
+        return self.index
+
+    def __eq__(self, other):
+        if not isinstance(other, TensorIndex):
+            raise TypeError(f"Unsupported type {type(other)}")
+
+        if self.index_value == other.index_value:
+            return True
+        else:
+            return False
+
+
+def obtain_dim(expr) -> int:
+    """
+    # Evaluate the expr to decide its dimension
+    """
+    if expr == S.NegativeOne or isinstance(expr, Number):
+        return 0
+
+    symbol_dict = dict()
+    for symbol in list(expr.free_symbols):
+        if isinstance(symbol, (iVar, IdxVar)):
+            symbol_dict[symbol] = np.ones((2, 1))
+        elif isinstance(symbol, (Para, IdxPara)):
+            if symbol.dim == 2:
+                symbol_dict[symbol] = np.ones((2, 2))
+            elif symbol.dim == 1:
+                symbol_dict[symbol] = np.ones((2, 1))
+    temp_expr = sp.lambdify(symbol_dict.keys(), expr)
+    return temp_expr(*symbol_dict.values()).shape[1]
+
+
+def obtain_TExpr(expr: Expr, index: TensorIndex):
+    """
+    Convert Expr to TOperator and its args
+
+    """
+
+    if isinstance(expr, Add):
+        Texpr = TAdd(expr, index)
+    elif isinstance(expr, (Mat_Mul, Mul)):
+        Texpr = TMul(expr, index)
+    elif isinstance(expr, Abs):
+        Texpr = TAbs(expr, index)
+    elif isinstance(expr, (iVar, IdxVar)):
+        Texpr = TVector(expr, index)
+    elif isinstance(expr, (Para, IdxPara)):
+        if expr.dim == 2:
+            Texpr = TMatrix(expr, index)
+        elif expr.dim == 1:
+            Texpr = TVector(expr, index)
+        else:
+            TypeError(f"Unsupported dim {expr.dim}")
+    elif isinstance(expr, Number):
+        Texpr = TNumber(expr)
+    else:
+        raise NotImplementedError(f"Unsupported expression type {type(expr)}")
+    return Texpr
+
+
+def ToComGraph(expr: Expr) -> nx.DiGraph:
+    DG = nx.DiGraph()
+    output_dim = obtain_dim(expr)
+    if output_dim == 2:
+        index = TensorIndex([0, 1])
+    elif output_dim == 1:
+        index = TensorIndex([0])
+    else:
+        raise TypeError("Unsupported output dim")
+    queue = [(expr, index, None)]  # [(Expr, TensorIndex, predecessor)]
+
+    while queue:
+        current_expr, index, predecessor = queue.pop(0)
+
+        Texpr = obtain_TExpr(current_expr, index)
+
+        if predecessor is not None:
+            DG.add_edge(predecessor, Texpr)
+            DG.nodes[Texpr]['level'] = DG.nodes[predecessor]['level'] + 1
+        else:
+            DG.add_node(Texpr)
+            DG.nodes[Texpr]['level'] = 0
+
+        if isinstance(Texpr, TMul):
+            queue.append((Texpr.args[0], TensorIndex(Texpr.index[0].index_value), Texpr))
+            queue.append((Texpr.args[1], TensorIndex(Texpr.index[1].index_value), Texpr))
+        elif isinstance(Texpr, TAdd):
+            for subexpr in Texpr.args:
+                queue.append((subexpr, TensorIndex(Texpr.index.index_value), Texpr))
+        elif isinstance(Texpr, TAbs):
+            queue.append((Texpr.args[0], TensorIndex(Texpr.index.index_value), Texpr))
+
+    # Check for and remove any cycles to ensure acyclic graph
+    if not nx.is_directed_acyclic_graph(DG):
+        raise ValueError("The expression contains cycles.")
+
+    return DG
+
+
+def draw_dag_as_tree(G, pos=None):
+    # using Graphviz and pygraphviz to draw directed acyclic expression graph as a 'tree'
+
+    if pos is None:
+        pos = nx.nx_agraph.graphviz_layout(G, prog='dot')
+
+    nx.draw_networkx_nodes(G, pos, node_size=800, node_color='lightblue')
+    root_node = [node for node in G.nodes() if G.in_degree(node) == 0]
+    leaf_node = [node for node in G.nodes() if G.out_degree(node) == 0]
+    nx.draw_networkx_nodes(G, pos, nodelist=root_node, node_size=800, node_color='lightgreen')
+    nx.draw_networkx_nodes(G, pos, nodelist=leaf_node, node_size=800)
+    nx.draw_networkx_labels(G, pos)
+    nx.draw_networkx_edges(G, pos, arrowstyle='-|>', arrowsize=15)
+
+    plt.axis('off')
+    plt.show()
+
+
+def TMul2Mul(x, y, index: List[TensorIndex, TensorIndex, TensorIndex]):
+    if x is S.Zero or y is S.Zero:
+        return 0
+    s1, s2, s3 = index[:]
+    if s1 == TensorIndex(-1) or s2 == TensorIndex(-1):
+        return x * y
+    if len(s1.index) < 2:
+        if len(s2.index) < 2:
+            # i, j, ij
+            if s1.index_value[0] != s2.index_value[0]:
+                return Mat_Mul(x, transpose(y))
+            # i, i, i
+            if s1.index_value[0] == s2.index_value[0]:
+                return x * y
+        else:
+            # j, jj, jj
+            if s2.index_value[0] == s2.index_value[1] == s1.index_value[0]:
+                if isinstance(y, Diag):
+                    return Diag(x * y.args[0])
+                else:
+                    return Diag(x * y)
+            # i, ij, ij
+            if s2.index_value[0] != s2.index_value[1] and s1.index_value[0] == s2.index_value[0]:
+                return Mat_Mul(Diag(x), y)
+    else:
+        if len(s2.index) < 2:
+            # jj, j, jj
+            if s1.index_value[0] == s1.index_value[1] == s2.index_value[0]:
+                if isinstance(x, Diag):
+                    return Diag(x.args[0] * y)
+            # ij, j, i
+            if s1.index_value[0] != s1.index_value[1] and s1.index_value[1] == s2.index_value[0]:
+                return Mat_Mul(x, y)
+        else:
+            # ij, ij, ij
+            if s1.index_value == s2.index_value and s1.index_value[0] != s1.index_value[1]:
+                return x * y
+            # ij, jj, ij
+            if s1 == s3 and s2.index_value[0] == s2.index_value[1] and s1.index_value[1] == s2.index_value[0]:
+                if isinstance(y, Number):
+                    return y * x
+                elif isinstance(y, Diag):
+                    return Mat_Mul(x, y)
+            # ij, jk, ik
+            if s1.index_value != s2.index_value and s1.index_value[1] == s2.index_value[0]:
+                return Mat_Mul(x, y)
+        return NotImplementedError("Unsupport index type!")
+
+
+class TensorExpr:
+
+    def __init__(self, expr: Expr):
+        self.ComGraph = ToComGraph(expr)
+        self.index = TensorIndex([0])
+
+    def visualize(self):
+        """
+        To visualize TensorExpr
+        """
+        draw_dag_as_tree(self.ComGraph)
+
+    def diff(self, s):
+
+        leaf_node = [node for node in self.ComGraph.nodes() if self.ComGraph.out_degree(node) == 0]
+        index_s = None
+        for node in leaf_node:
+            if node.name == s.name:
+                index_s = node.index
+        if index_s is None:
+            raise TypeError(f"Cant find index of {s}")
+
+        highest_level = np.max([attr['level'] for node, attr in self.ComGraph.nodes(data=True)])
+        derivatives: Dict[Union[TMatrix, TVector, TMul, TAdd, TAbs, TNumber], Tuple[Expr, TensorIndex]] = dict()
+        for level in range(highest_level, -1, -1):
+            current_nodes = [node for node, attr in self.ComGraph.nodes(data=True) if attr['level'] == level]
+            for node in current_nodes:
+                if isinstance(node, (TMatrix, TVector)):
+                    derivatives[node] = (node.symbol.diff(s), node.index)
+                elif isinstance(node, TAdd):
+                    succ = list(self.ComGraph.successors(node))
+                    derivatives[node] = (Add(*[derivatives[arg][0] for arg in succ]), derivatives[succ[0]][1])
+                elif isinstance(node, TAbs):
+                    succ = list(self.ComGraph.successors(node))
+                    s1 = derivatives[succ[0]][1]
+                    s2 = index_s
+                    Aprime = derivatives[succ[0]][0]
+                    fprimeA = Sign(node.args[0])
+                    s1s2 = TensorIndex(s1.index_value + s2.index_value)
+
+                    derivatives[node] = (TMul2Mul(fprimeA, Aprime, [s1, s1s2, s1s2]),
+                                         s1s2)
+                elif isinstance(node, TMul):
+                    succ = list(self.ComGraph.successors(node))
+                    s4 = index_s
+                    s1 = node.index[0]
+                    s2 = node.index[1]
+                    s3 = node.index[2]
+                    A = node.args[0]
+                    B = node.args[1]
+                    Aprime = derivatives[succ[0]][0]
+                    Bprime = derivatives[succ[1]][0]
+                    s1s4 = TensorIndex(s1.index_value + s4.index_value)
+                    s3s4 = TensorIndex(s3.index_value + s4.index_value)
+                    s2s4 = TensorIndex(s2.index_value + s4.index_value)
+                    derivatives[node] = (TMul2Mul(B, Aprime, [s2, s1s4, s3s4]) + TMul2Mul(A, Bprime, [s1, s2s4, s3s4]),
+                                         s3s4)
+                elif isinstance(node, TNumber):
+                    derivatives[node] = (Integer(0), TensorIndex(-1))
+        root_node = [node for node in self.ComGraph.nodes() if self.ComGraph.in_degree(node) == 0]
+        return derivatives[root_node[0]][0]
+
+
+def MixedEquationDiff(expr: Expr, symbol: Symbol):
+    """
+    Calculate the derivatives of mixed-Matrix-Vector equations
+
+    """
+    return TensorExpr(expr).diff(symbol)
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/symbols.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/symbols.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-from typing import Dict
-
-import numpy as np
-from sympy import Symbol, Expr
-
-from Solverz.num_api.Array import Array
-
-Sympify_Mapping = {}
-
-
-def IndexPrinter(index):
-    if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
-        raise TypeError(f"Unsupported idx type {type(index)}")
-
-    def print_(index_):
-        if isinstance(index_, slice):
-            start = index_.start if index_.start is not None else ''
-            stop = index_.stop if index_.stop is not None else ''
-            slice_str = f'{start}:{stop}'
-            slice_str += f':{index_.step}' if index_.step is not None else ''
-            return slice_str
-        elif isinstance(index_, (int, np.integer, list, idx, IdxSymBasic, Expr)):
-            return f'{index_}'
-
-    if isinstance(index, tuple):
-        if len(index) != 2:
-            raise ValueError("Support only two element tuples!")
-        else:
-            return print_(index[0]) + ',' + print_(index[1])
-    else:
-        return print_(index)
-
-
-def SymbolExtractor(index) -> Dict:
-    if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
-        raise TypeError(f"Unsupported idx type {type(index)}")
-
-    temp = dict()
-
-    if isinstance(index, (int, np.integer, idx, IdxSymBasic)):
-        if isinstance(index, idx):
-            temp.update({index.name: index})
-        elif isinstance(index, IdxSymBasic):
-            temp.update({index.name0: index.symbol0})
-            temp.update(index.SymInIndex)
-    elif isinstance(index, list):
-        for i in range(len(index)):
-            temp.update(SymbolExtractor(index[i]))
-    elif isinstance(index, Expr):
-        for var_ in list(index.free_symbols):
-            temp.update(SymbolExtractor(var_))
-    elif isinstance(index, slice):
-        if index.start is not None:
-            temp.update(SymbolExtractor(index.start))
-        if index.stop is not None:
-            temp.update(SymbolExtractor(index.stop))
-        if index.step is not None:
-            temp.update(SymbolExtractor(index.step))
-    elif isinstance(index, tuple):
-        if len(index) != 2:
-            raise ValueError("Support only two element tuples!")
-        else:
-            temp.update(SymbolExtractor(index[0]))
-            temp.update(SymbolExtractor(index[1]))
-
-    return temp
-
-
-Solverz_internal_name = ['y_', 'F_', 'p_', 'J_', 'row', 'col', 'data', '_F_', 'data_']
-
-
-class SolSymBasic(Symbol):
-    """
-    Basic class for Solverz Symbols
-    """
-    _iterable = False  # sp.lambdify gets into infinite loop if _iterable == True
-
-    def __new__(cls, name: str, value=None, dim: int = 1, internal_use=False):
-        if any([name == built_in_name for built_in_name in Solverz_internal_name]):
-            if not internal_use:
-                raise ValueError(f"Solverz built-in name {name}, cannot be used as variable name.")
-        obj = Symbol.__new__(cls, f'{name}')
-        obj.name = f'{name}'
-        obj.dim = dim
-        if value is not None:
-            obj.value = Array(value, dim)
-        else:
-            obj.value = None
-        obj.initialized = True if value is not None else False
-        return obj
-
-    def __getitem__(self, index):
-        pass
-
-
-class IdxSymBasic(Symbol):
-    """
-    Basic class for Solverz indexed Symbols
-    """
-
-    def __new__(cls, symbol, index, dim):
-        if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
-            raise TypeError(f"Unsupported idx type {type(index)}")
-        if not isinstance(symbol, Symbol):
-            raise TypeError(f"Invalid symbol type {type(symbol)}")
-        obj = Symbol.__new__(cls, f'{symbol.name}[{index}]')
-        obj.symbol0 = symbol
-        obj.index = index
-        obj.name0 = symbol.name
-        obj.name = obj.name0 + '[' + IndexPrinter(index) + ']'
-        obj.SymInIndex = SymbolExtractor(index)
-        obj.dim = dim
-
-        return obj
-
-    def _numpycode(self, printer, **kwargs):
-
-        def IndexCodePrinter(index, printer):
-            if isinstance(index, (int, np.integer, list)):
-                return '{i}'.format(i=printer._print(index))
-            elif isinstance(index, idx):
-                return '{i}'.format(i=printer._print(index))
-            elif isinstance(index, Expr):
-                return '{i}'.format(i=printer._print(index))
-            elif isinstance(index, slice):
-                start = index.start
-                stop = index.stop
-                step = index.step
-                if any([isinstance(arg, (idx, Expr)) for arg in [start, stop, step]]):
-                    start = IndexCodePrinter(start, printer) if start is not None else None
-                    stop = IndexCodePrinter(stop, printer) if stop is not None else None
-                    step = IndexCodePrinter(step, printer) if step is not None else None
-                    return 'sol_slice({i}, {j}, {k})'.format(i=start, j=stop, k=step)
-                else:
-                    start = IndexCodePrinter(start, printer) if start is not None else ''
-                    stop = IndexCodePrinter(stop, printer) if stop is not None else ''
-                    slice_str = '{i}:{j}'.format(i=start, j=stop)
-                    slice_str += f':{IndexCodePrinter(step, printer)}' if step is not None else ''
-                    return slice_str
-
-        if isinstance(self.index, tuple):
-            if len(self.index) != 2:
-                raise ValueError("Support only two element tuples!")
-            else:
-                temp = IndexCodePrinter(self.index[0], printer) + ',' + IndexCodePrinter(self.index[1], printer)
-        else:
-            temp = IndexCodePrinter(self.index, printer)
-
-        return self.name0 + '[' + temp + ']'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
-class iVar(SolSymBasic):
-    def __getitem__(self, index):
-        return IdxVar(self, index, self.dim)
-
-
-class iAliasVar(SolSymBasic):
-    def __getitem__(self, index):
-        return IdxAliasVar(self, index, self.dim)
-
-
-class Para(SolSymBasic):
-    def __getitem__(self, index):
-        return IdxPara(self, index, self.dim)
-
-
-class idx(SolSymBasic):
-    def __new__(cls, name: str, value=None, dim: int = 1):
-        if dim > 1:
-            raise ValueError("idx can only be one-dimensional")
-        obj = SolSymBasic.__new__(cls, name, value, dim=1)
-        if obj.value is not None:
-            obj.value = Array(value, dim=1, dtype=int)
-        return obj
-
-    def __getitem__(self, index):
-        return Idxidx(self, index, dim=1)
-
-
-class IdxVar(IdxSymBasic):
-    pass
-
-
-class IdxAliasVar(IdxSymBasic):
-    pass
-
-
-class IdxPara(IdxSymBasic):
-    pass
-
-
-class Idxidx(IdxSymBasic):
-    pass
-
-
-class SolDict(Symbol):
-    """
-    Solverz' Dict class for numerical equation code printer, which accepts only str index
-    """
-    _iterable = False  # sp.lambdify gets into infinite loop if _iterable == True
-
-    def __new__(cls, name: str):
-        obj = Symbol.__new__(cls, f'{name}')
-        obj.name = f'{name}'
-        return obj
-
-    def __getitem__(self, index):
-        return IdxDict(self, index)
-
-
-class IdxDict(Symbol):
-    """
-    Indexed Dicts
-    """
-
-    def __new__(cls, symbol, index):
-        if not isinstance(index, str):
-            raise TypeError(f"Unsupported idx type {type(index)}")
-        if not isinstance(symbol, SolDict):
-            raise TypeError(f"Invalid symbol type {type(symbol)}")
-        obj = Symbol.__new__(cls, f'{symbol.name}["{index}"]')
-        obj.index = index
-
-        return obj
-
-    def _numpycode(self, printer, **kwargs):
-        return self.name
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
+from typing import Dict
+
+import numpy as np
+from sympy import Symbol, Expr
+
+from Solverz.num_api.Array import Array
+
+Sympify_Mapping = {}
+
+
+def IndexPrinter(index):
+    if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
+        raise TypeError(f"Unsupported idx type {type(index)}")
+
+    def print_(index_):
+        if isinstance(index_, slice):
+            start = index_.start if index_.start is not None else ''
+            stop = index_.stop if index_.stop is not None else ''
+            slice_str = f'{start}:{stop}'
+            slice_str += f':{index_.step}' if index_.step is not None else ''
+            return slice_str
+        elif isinstance(index_, (int, np.integer, list, idx, IdxSymBasic, Expr)):
+            return f'{index_}'
+
+    if isinstance(index, tuple):
+        if len(index) != 2:
+            raise ValueError("Support only two element tuples!")
+        else:
+            return print_(index[0]) + ',' + print_(index[1])
+    else:
+        return print_(index)
+
+
+def SymbolExtractor(index) -> Dict:
+    if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
+        raise TypeError(f"Unsupported idx type {type(index)}")
+
+    temp = dict()
+
+    if isinstance(index, (int, np.integer, idx, IdxSymBasic)):
+        if isinstance(index, idx):
+            temp.update({index.name: index})
+        elif isinstance(index, IdxSymBasic):
+            temp.update({index.name0: index.symbol0})
+            temp.update(index.SymInIndex)
+    elif isinstance(index, list):
+        for i in range(len(index)):
+            temp.update(SymbolExtractor(index[i]))
+    elif isinstance(index, Expr):
+        for var_ in list(index.free_symbols):
+            temp.update(SymbolExtractor(var_))
+    elif isinstance(index, slice):
+        if index.start is not None:
+            temp.update(SymbolExtractor(index.start))
+        if index.stop is not None:
+            temp.update(SymbolExtractor(index.stop))
+        if index.step is not None:
+            temp.update(SymbolExtractor(index.step))
+    elif isinstance(index, tuple):
+        if len(index) != 2:
+            raise ValueError("Support only two element tuples!")
+        else:
+            temp.update(SymbolExtractor(index[0]))
+            temp.update(SymbolExtractor(index[1]))
+
+    return temp
+
+
+Solverz_internal_name = ['y_', 'F_', 'p_', 'J_', 'row', 'col', 'data', '_F_', 'data_']
+
+
+class SolSymBasic(Symbol):
+    """
+    Basic class for Solverz Symbols
+    """
+    _iterable = False  # sp.lambdify gets into infinite loop if _iterable == True
+
+    def __new__(cls, name: str, value=None, dim: int = 1, internal_use=False):
+        if any([name == built_in_name for built_in_name in Solverz_internal_name]):
+            if not internal_use:
+                raise ValueError(f"Solverz built-in name {name}, cannot be used as variable name.")
+        obj = Symbol.__new__(cls, f'{name}')
+        obj.name = f'{name}'
+        obj.dim = dim
+        if value is not None:
+            obj.value = Array(value, dim)
+        else:
+            obj.value = None
+        obj.initialized = True if value is not None else False
+        return obj
+
+    def __getitem__(self, index):
+        pass
+
+
+class IdxSymBasic(Symbol):
+    """
+    Basic class for Solverz indexed Symbols
+    """
+
+    def __new__(cls, symbol, index, dim):
+        if not isinstance(index, (int, np.integer, list, idx, IdxSymBasic, Expr, slice, tuple)):
+            raise TypeError(f"Unsupported idx type {type(index)}")
+        if not isinstance(symbol, Symbol):
+            raise TypeError(f"Invalid symbol type {type(symbol)}")
+        obj = Symbol.__new__(cls, f'{symbol.name}[{index}]')
+        obj.symbol0 = symbol
+        obj.index = index
+        obj.name0 = symbol.name
+        obj.name = obj.name0 + '[' + IndexPrinter(index) + ']'
+        obj.SymInIndex = SymbolExtractor(index)
+        obj.dim = dim
+
+        return obj
+
+    def _numpycode(self, printer, **kwargs):
+
+        def IndexCodePrinter(index, printer):
+            if isinstance(index, (int, np.integer, list)):
+                return '{i}'.format(i=printer._print(index))
+            elif isinstance(index, idx):
+                return '{i}'.format(i=printer._print(index))
+            elif isinstance(index, Expr):
+                return '{i}'.format(i=printer._print(index))
+            elif isinstance(index, slice):
+                start = index.start
+                stop = index.stop
+                step = index.step
+                if any([isinstance(arg, (idx, Expr)) for arg in [start, stop, step]]):
+                    start = IndexCodePrinter(start, printer) if start is not None else None
+                    stop = IndexCodePrinter(stop, printer) if stop is not None else None
+                    step = IndexCodePrinter(step, printer) if step is not None else None
+                    return 'sol_slice({i}, {j}, {k})'.format(i=start, j=stop, k=step)
+                else:
+                    start = IndexCodePrinter(start, printer) if start is not None else ''
+                    stop = IndexCodePrinter(stop, printer) if stop is not None else ''
+                    slice_str = '{i}:{j}'.format(i=start, j=stop)
+                    slice_str += f':{IndexCodePrinter(step, printer)}' if step is not None else ''
+                    return slice_str
+
+        if isinstance(self.index, tuple):
+            if len(self.index) != 2:
+                raise ValueError("Support only two element tuples!")
+            else:
+                temp = IndexCodePrinter(self.index[0], printer) + ',' + IndexCodePrinter(self.index[1], printer)
+        else:
+            temp = IndexCodePrinter(self.index, printer)
+
+        return self.name0 + '[' + temp + ']'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+
+class iVar(SolSymBasic):
+    def __getitem__(self, index):
+        return IdxVar(self, index, self.dim)
+
+
+class iAliasVar(SolSymBasic):
+    def __getitem__(self, index):
+        return IdxAliasVar(self, index, self.dim)
+
+
+class Para(SolSymBasic):
+    def __getitem__(self, index):
+        return IdxPara(self, index, self.dim)
+
+
+class idx(SolSymBasic):
+    def __new__(cls, name: str, value=None, dim: int = 1):
+        if dim > 1:
+            raise ValueError("idx can only be one-dimensional")
+        obj = SolSymBasic.__new__(cls, name, value, dim=1)
+        if obj.value is not None:
+            obj.value = Array(value, dim=1, dtype=int)
+        return obj
+
+    def __getitem__(self, index):
+        return Idxidx(self, index, dim=1)
+
+
+class IdxVar(IdxSymBasic):
+    pass
+
+
+class IdxAliasVar(IdxSymBasic):
+    pass
+
+
+class IdxPara(IdxSymBasic):
+    pass
+
+
+class Idxidx(IdxSymBasic):
+    pass
+
+
+class SolDict(Symbol):
+    """
+    Solverz' Dict class for numerical equation code printer, which accepts only str index
+    """
+    _iterable = False  # sp.lambdify gets into infinite loop if _iterable == True
+
+    def __new__(cls, name: str):
+        obj = Symbol.__new__(cls, f'{name}')
+        obj.name = f'{name}'
+        return obj
+
+    def __getitem__(self, index):
+        return IdxDict(self, index)
+
+
+class IdxDict(Symbol):
+    """
+    Indexed Dicts
+    """
+
+    def __new__(cls, symbol, index):
+        if not isinstance(index, str):
+            raise TypeError(f"Unsupported idx type {type(index)}")
+        if not isinstance(symbol, SolDict):
+            raise TypeError(f"Invalid symbol type {type(symbol)}")
+        obj = Symbol.__new__(cls, f'{symbol.name}["{index}"]')
+        obj.index = index
+
+        return obj
+
+    def _numpycode(self, printer, **kwargs):
+        return self.name
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/transform.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/transform.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-from sympy import simplify
-
-from Solverz.sym_algebra.symbols import Para, iAliasVar, IdxVar, iVar
-from Solverz.sym_algebra.functions import switch
-from Solverz.utilities.type_checker import is_number
-
-
-def finite_difference(diff_var, flux, source, two_dim_var, M, scheme='central diff', direction=None, dx=None):
-    M_ = M + 1  # for pretty printer of M in slice
-    if dx is None:
-        dx = Para('dx')
-    else:
-        if is_number(dx):
-            dx = dx
-        else:
-            raise TypeError(f'Input dx is not number!')
-
-    dt = Para('dt')
-    u = diff_var
-    u0 = iAliasVar(u.name + '_tag_0')
-
-    if scheme == 'central diff':
-        fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
-        fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
-        fui1j = flux.subs([(a, iAliasVar(a.name + '_tag_0')[1:M_]) for a in two_dim_var])
-        fuij = flux.subs([(a, iAliasVar(a.name + '_tag_0')[0:M_ - 1]) for a in two_dim_var])
-
-        S = source.subs([(a, (a[1:M_] + a[0:M_ - 1] + iAliasVar(a.name + '_tag_0')[1:M_] + iAliasVar(a.name + '_tag_0')[
-                                                                                          0:M_ - 1]) / 4) for a in
-                         two_dim_var])
-
-        fde = dx * (u[1:M_] - u0[1:M_] + u[0:M_ - 1] - u0[0:M_ - 1]) \
-              + simplify(dt * (fui1j1 - fuij1 + fui1j - fuij)) \
-              - simplify(2 * dx * dt * S)
-
-    elif scheme == 'euler':
-        if direction == 1:
-            fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
-            fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
-            S = source.subs([(a, a[1:M_]) for a in two_dim_var])
-            fde = dx * (u[1:M_] - u0[1:M_]) + simplify(dt * (fui1j1 - fuij1)) - simplify(dx * dt * S)
-        elif direction == -1:
-            fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
-            fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
-            S = source.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
-            fde = dx * (u[0:M_ - 1] - u0[0:M_ - 1]) + simplify(dt * (fui1j1 - fuij1)) - simplify(dx * dt * S)
-        else:
-            raise ValueError(f"Unimplemented direction {direction}!")
-    return fde
-
-
-def semi_descritize(diff_var,
-                    flux,
-                    source,
-                    two_dim_var,
-                    M,
-                    scheme='TVD1',
-                    a0=None,
-                    a1=None,
-                    dx=None):
-    M_ = M + 1  # for pretty printer of M in slice
-
-    if a0 is None:
-        a0 = Para('ajp12')
-    if a1 is None:
-        a1 = Para('ajm12')
-
-    if dx is None:
-        dx = Para('dx')
-    else:
-        if is_number(dx):
-            dx = dx
-        else:
-            raise TypeError(f'Input dx is not number!')
-
-    u = diff_var
-    if scheme == 'TVD2':
-        # j=1
-        # f(u[2])
-        fu2 = flux.subs([(var, var[2]) for var in two_dim_var])
-        # f(u[0])=f(2*uL-u[1])
-        fu0 = flux.subs([(var, var[0]) for var in two_dim_var])
-        # S(u[1])
-        Su1 = source.subs([(var, var[1]) for var in two_dim_var])
-        ode_rhs1 = -simplify((fu2 - fu0) / (2 * dx)) \
-                   + simplify((a0[0] * (u[2] - u[1]) - a1[0] * (u[1] - u[0])) / (2 * dx)) \
-                   + simplify(Su1)
-
-        # j=M-1
-        # f(u[M])=f(2*uR-u[M-1])
-        fum = flux.subs([(var, var[M]) for var in two_dim_var])
-        # f(u[M-2])
-        fum2 = flux.subs([(var, var[M - 2]) for var in two_dim_var])
-        # S(u[M-1])
-        SuM1 = source.subs([(var, var[M - 1]) for var in two_dim_var])
-        ode_rhs3 = -simplify((fum - fum2) / (2 * dx)) \
-                   + simplify((a0[-1] * (u[M] - u[M - 1]) - a1[-1] * (u[M - 1] - u[M - 2])) / (2 * dx)) \
-                   + simplify(SuM1)
-
-        # 2<=j<=M-2
-        def ujprime(U: IdxVar, v: int):
-            # for given u_j,
-            # returns
-            # u^+_{j+1/2} case v==0,
-            # u^-_{j+1/2} case 1,
-            # u^+_{j-1/2} case 2,
-            # u^-_{j-1/2} case 3
-            if not isinstance(U.index, slice):
-                raise TypeError("Index of IdxVar must be slice object")
-            start = U.index.start
-            stop = U.index.stop
-            step = U.index.step
-            U = U.symbol0
-            Ux = iVar(U.name + 'x')
-
-            # u_j
-            Uj = U[start:stop:step]
-            # (u_x)_j
-            Uxj = Ux[start:stop:step]
-            # u_{j+1}
-            Ujp1 = U[start + 1:stop + 1:step]
-            # (u_x)_{j+1}
-            Uxjp1 = Ux[start + 1:stop + 1:step]
-            # u_{j-1}
-            Ujm1 = U[start - 1:stop - 1:step]
-            # (u_x)_{j-1}
-            Uxjm1 = Ux[start - 1:stop - 1:step]
-
-            if v == 0:
-                return Ujp1 - dx / 2 * Uxjp1
-            elif v == 1:
-                return Uj + dx / 2 * Uxj
-            elif v == 2:
-                return Uj - dx / 2 * Uxj
-            elif v == 3:
-                return Ujm1 + dx / 2 * Uxjm1
-            else:
-                raise ValueError("v=0 or 1 or 2 or 3!")
-
-        # j\in [2:M_-2]
-        Suj = source.subs([(var, var[2:M_ - 2]) for var in two_dim_var])
-        Hp = (flux.subs([(var, ujprime(var[2:M_ - 2], 0)) for var in two_dim_var]) +
-              flux.subs([(var, ujprime(var[2:M_ - 2], 1)) for var in two_dim_var])) / 2 \
-             - a0[2:M_ - 2] / 2 * (ujprime(u[2:M_ - 2], 0) - ujprime(u[2:M_ - 2], 1))
-        Hm = (flux.subs([(var, ujprime(var[2:M_ - 2], 2)) for var in two_dim_var]) +
-              flux.subs([(var, ujprime(var[2:M_ - 2], 3)) for var in two_dim_var])) / 2 \
-             - a1[2:M_ - 2] / 2 * (ujprime(u[2:M_ - 2], 2) - ujprime(u[2:M_ - 2], 3))
-        ode_rhs2 = -simplify(Hp - Hm) / dx + Suj
-
-        theta = Para('theta')
-        ux = iVar(u.name + 'x')
-        minmod_flag = Para('minmod_flag_of_' + ux.name)
-        minmod_rhs = ux[1:M_ - 1] - switch(theta * (u[1:M_ - 1] - u[0:M_ - 2]) / dx,
-                                           (u[2:M_] - u[0:M_ - 2]) / (2 * dx),
-                                           theta * (u[2:M_] - u[1:M_ - 1]) / dx,
-                                           0,
-                                           minmod_flag)
-
-        return {'Ode': [(ode_rhs1, u[1]), (ode_rhs2, u[2:M_ - 2]), (ode_rhs3, u[M - 1])],
-                'Eqn': [minmod_rhs, ux[0], ux[M]]}
-    elif scheme == 'TVD1':
-        # 1<=j<=M-1
-        # f(u[j+1])
-        fu1 = flux.subs([(var, var[2:M_]) for var in two_dim_var])
-        # f(u[j-1])
-        fu2 = flux.subs([(var, var[0:M_ - 2]) for var in two_dim_var])
-        # S(u[j])
-        Su = source.subs([(var, var[1:M_ - 1]) for var in two_dim_var])
-        ode_rhs = -simplify((fu1 - fu2) / (2 * dx)) \
-                  + simplify((a0 * (u[2:M_] - u[1:M_ - 1]) - a1 * (u[1:M_ - 1] - u[0:M_ - 2])) / (2 * dx)) \
-                  + simplify(Su)
-        return {'Ode': (ode_rhs, u[1:M_ - 1])}
+from sympy import simplify
+
+from Solverz.sym_algebra.symbols import Para, iAliasVar, IdxVar, iVar
+from Solverz.sym_algebra.functions import switch
+from Solverz.utilities.type_checker import is_number
+
+
+def finite_difference(diff_var, flux, source, two_dim_var, M, scheme='central diff', direction=None, dx=None):
+    M_ = M + 1  # for pretty printer of M in slice
+    if dx is None:
+        dx = Para('dx')
+    else:
+        if is_number(dx):
+            dx = dx
+        else:
+            raise TypeError(f'Input dx is not number!')
+
+    dt = Para('dt')
+    u = diff_var
+    u0 = iAliasVar(u.name + '_tag_0')
+
+    if scheme == 'central diff':
+        fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
+        fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
+        fui1j = flux.subs([(a, iAliasVar(a.name + '_tag_0')[1:M_]) for a in two_dim_var])
+        fuij = flux.subs([(a, iAliasVar(a.name + '_tag_0')[0:M_ - 1]) for a in two_dim_var])
+
+        S = source.subs([(a, (a[1:M_] + a[0:M_ - 1] + iAliasVar(a.name + '_tag_0')[1:M_] + iAliasVar(a.name + '_tag_0')[
+                                                                                          0:M_ - 1]) / 4) for a in
+                         two_dim_var])
+
+        fde = dx * (u[1:M_] - u0[1:M_] + u[0:M_ - 1] - u0[0:M_ - 1]) \
+              + simplify(dt * (fui1j1 - fuij1 + fui1j - fuij)) \
+              - simplify(2 * dx * dt * S)
+
+    elif scheme == 'euler':
+        if direction == 1:
+            fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
+            fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
+            S = source.subs([(a, a[1:M_]) for a in two_dim_var])
+            fde = dx * (u[1:M_] - u0[1:M_]) + simplify(dt * (fui1j1 - fuij1)) - simplify(dx * dt * S)
+        elif direction == -1:
+            fui1j1 = flux.subs([(a, a[1:M_]) for a in two_dim_var])
+            fuij1 = flux.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
+            S = source.subs([(a, a[0:M_ - 1]) for a in two_dim_var])
+            fde = dx * (u[0:M_ - 1] - u0[0:M_ - 1]) + simplify(dt * (fui1j1 - fuij1)) - simplify(dx * dt * S)
+        else:
+            raise ValueError(f"Unimplemented direction {direction}!")
+    return fde
+
+
+def semi_descritize(diff_var,
+                    flux,
+                    source,
+                    two_dim_var,
+                    M,
+                    scheme='TVD1',
+                    a0=None,
+                    a1=None,
+                    dx=None):
+    M_ = M + 1  # for pretty printer of M in slice
+
+    if a0 is None:
+        a0 = Para('ajp12')
+    if a1 is None:
+        a1 = Para('ajm12')
+
+    if dx is None:
+        dx = Para('dx')
+    else:
+        if is_number(dx):
+            dx = dx
+        else:
+            raise TypeError(f'Input dx is not number!')
+
+    u = diff_var
+    if scheme == 'TVD2':
+        # j=1
+        # f(u[2])
+        fu2 = flux.subs([(var, var[2]) for var in two_dim_var])
+        # f(u[0])=f(2*uL-u[1])
+        fu0 = flux.subs([(var, var[0]) for var in two_dim_var])
+        # S(u[1])
+        Su1 = source.subs([(var, var[1]) for var in two_dim_var])
+        ode_rhs1 = -simplify((fu2 - fu0) / (2 * dx)) \
+                   + simplify((a0[0] * (u[2] - u[1]) - a1[0] * (u[1] - u[0])) / (2 * dx)) \
+                   + simplify(Su1)
+
+        # j=M-1
+        # f(u[M])=f(2*uR-u[M-1])
+        fum = flux.subs([(var, var[M]) for var in two_dim_var])
+        # f(u[M-2])
+        fum2 = flux.subs([(var, var[M - 2]) for var in two_dim_var])
+        # S(u[M-1])
+        SuM1 = source.subs([(var, var[M - 1]) for var in two_dim_var])
+        ode_rhs3 = -simplify((fum - fum2) / (2 * dx)) \
+                   + simplify((a0[-1] * (u[M] - u[M - 1]) - a1[-1] * (u[M - 1] - u[M - 2])) / (2 * dx)) \
+                   + simplify(SuM1)
+
+        # 2<=j<=M-2
+        def ujprime(U: IdxVar, v: int):
+            # for given u_j,
+            # returns
+            # u^+_{j+1/2} case v==0,
+            # u^-_{j+1/2} case 1,
+            # u^+_{j-1/2} case 2,
+            # u^-_{j-1/2} case 3
+            if not isinstance(U.index, slice):
+                raise TypeError("Index of IdxVar must be slice object")
+            start = U.index.start
+            stop = U.index.stop
+            step = U.index.step
+            U = U.symbol0
+            Ux = iVar(U.name + 'x')
+
+            # u_j
+            Uj = U[start:stop:step]
+            # (u_x)_j
+            Uxj = Ux[start:stop:step]
+            # u_{j+1}
+            Ujp1 = U[start + 1:stop + 1:step]
+            # (u_x)_{j+1}
+            Uxjp1 = Ux[start + 1:stop + 1:step]
+            # u_{j-1}
+            Ujm1 = U[start - 1:stop - 1:step]
+            # (u_x)_{j-1}
+            Uxjm1 = Ux[start - 1:stop - 1:step]
+
+            if v == 0:
+                return Ujp1 - dx / 2 * Uxjp1
+            elif v == 1:
+                return Uj + dx / 2 * Uxj
+            elif v == 2:
+                return Uj - dx / 2 * Uxj
+            elif v == 3:
+                return Ujm1 + dx / 2 * Uxjm1
+            else:
+                raise ValueError("v=0 or 1 or 2 or 3!")
+
+        # j\in [2:M_-2]
+        Suj = source.subs([(var, var[2:M_ - 2]) for var in two_dim_var])
+        Hp = (flux.subs([(var, ujprime(var[2:M_ - 2], 0)) for var in two_dim_var]) +
+              flux.subs([(var, ujprime(var[2:M_ - 2], 1)) for var in two_dim_var])) / 2 \
+             - a0[2:M_ - 2] / 2 * (ujprime(u[2:M_ - 2], 0) - ujprime(u[2:M_ - 2], 1))
+        Hm = (flux.subs([(var, ujprime(var[2:M_ - 2], 2)) for var in two_dim_var]) +
+              flux.subs([(var, ujprime(var[2:M_ - 2], 3)) for var in two_dim_var])) / 2 \
+             - a1[2:M_ - 2] / 2 * (ujprime(u[2:M_ - 2], 2) - ujprime(u[2:M_ - 2], 3))
+        ode_rhs2 = -simplify(Hp - Hm) / dx + Suj
+
+        theta = Para('theta')
+        ux = iVar(u.name + 'x')
+        minmod_flag = Para('minmod_flag_of_' + ux.name)
+        minmod_rhs = ux[1:M_ - 1] - switch(theta * (u[1:M_ - 1] - u[0:M_ - 2]) / dx,
+                                           (u[2:M_] - u[0:M_ - 2]) / (2 * dx),
+                                           theta * (u[2:M_] - u[1:M_ - 1]) / dx,
+                                           0,
+                                           minmod_flag)
+
+        return {'Ode': [(ode_rhs1, u[1]), (ode_rhs2, u[2:M_ - 2]), (ode_rhs3, u[M - 1])],
+                'Eqn': [minmod_rhs, ux[0], ux[M]]}
+    elif scheme == 'TVD1':
+        # 1<=j<=M-1
+        # f(u[j+1])
+        fu1 = flux.subs([(var, var[2:M_]) for var in two_dim_var])
+        # f(u[j-1])
+        fu2 = flux.subs([(var, var[0:M_ - 2]) for var in two_dim_var])
+        # S(u[j])
+        Su = source.subs([(var, var[1:M_ - 1]) for var in two_dim_var])
+        ode_rhs = -simplify((fu1 - fu2) / (2 * dx)) \
+                  + simplify((a0 * (u[2:M_] - u[1:M_ - 1]) - a1 * (u[1:M_ - 1] - u[0:M_ - 2])) / (2 * dx)) \
+                  + simplify(Su)
+        return {'Ode': (ode_rhs, u[1:M_ - 1])}
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/test/test_finite_difference.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/test/test_finite_difference.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from sympy import pycode, Integer
-
-from Solverz.sym_algebra.transform import finite_difference, semi_descritize
-from Solverz.sym_algebra.symbols import iVar, Para
-
-pi = iVar('pi')
-qi = iVar('qi')
-S = Para('S')
-va = Para('va')
-D = Para('D')
-lam = Para('lam')
-
-
-# finite difference of hyperbolic PDE, the gas equation
-def test_fd():
-    fde = finite_difference(qi,
-                            S * pi,
-                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
-                            [pi, qi],
-                            10,
-                            'central diff')
-    assert pycode(
-        fde) == 'S*dt*(-pi_tag_0[0:10] + pi_tag_0[1:11] - pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[0:10] - qi_tag_0[1:11] + qi[0:10] + qi[1:11]) + (1/4)*dt*dx*lam*va**2*(qi_tag_0[0:10] + qi_tag_0[1:11] + qi[0:10] + qi[1:11])**2/(D*S*(pi_tag_0[0:10] + pi_tag_0[1:11] + pi[0:10] + pi[1:11]))'
-
-    fde = finite_difference(pi,
-                            va ** 2 / S * qi,
-                            Integer(0),
-                            [pi, qi],
-                            10,
-                            'central diff')
-    assert pycode(
-        fde) == 'dx*(-pi_tag_0[0:10] - pi_tag_0[1:11] + pi[0:10] + pi[1:11]) + dt*va**2*(-qi_tag_0[0:10] + qi_tag_0[1:11] - qi[0:10] + qi[1:11])/S'
-
-    fde = finite_difference(qi,
-                            S * pi,
-                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
-                            [pi, qi],
-                            10,
-                            'euler',
-                            direction=1)
-    assert pycode(
-        fde) == 'S*dt*(-pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[1:11] + qi[1:11]) + (1/2)*qi[1:11]**2*dt*dx*lam*va**2/(pi[1:11]*D*S)'
-
-    fde = finite_difference(pi,
-                            va ** 2 / S * qi,
-                            Integer(0),
-                            [pi, qi],
-                            10,
-                            'euler',
-                            direction=1)
-    assert pycode(fde) == 'dx*(-pi_tag_0[1:11] + pi[1:11]) + dt*va**2*(-qi[0:10] + qi[1:11])/S'
-
-    fde = finite_difference(qi,
-                            S * pi,
-                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
-                            [pi, qi],
-                            10,
-                            'euler',
-                            direction=-1)
-    assert pycode(
-        fde) == 'S*dt*(-pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[0:10] + qi[0:10]) + (1/2)*qi[0:10]**2*dt*dx*lam*va**2/(pi[0:10]*D*S)'
-
-    fde = finite_difference(pi,
-                            va ** 2 / S * qi,
-                            Integer(0),
-                            [pi, qi],
-                            10,
-                            'euler',
-                            direction=-1)
-    assert pycode(fde) == 'dx*(-pi_tag_0[0:10] + pi[0:10]) + dt*va**2*(-qi[0:10] + qi[1:11])/S'
-
-
-def test_sd():
-    # semi-discretize
-    eqn_dict = semi_descritize(qi,
-                               S * pi,
-                               -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
-                               [pi, qi],
-                               11,
-                               'TVD1',
-                               a0=va,
-                               a1=va)
-
-    rhs = eqn_dict['Ode'][0]
-    diff_var = eqn_dict['Ode'][1]
-
-    assert pycode(
-        rhs) == '-1/2*S*(-pi[0:10] + pi[2:12])/dx + (1/2)*va*(qi[0:10] - 2*qi[1:11] + qi[2:12])/dx - 1/2*qi[1:11]**2*lam*va**2/(pi[1:11]*D*S)'
-    assert pycode(diff_var) == 'qi[1:11]'
-
-    eqn_dict = semi_descritize(pi,
-                               va ** 2 / S * qi,
-                               Integer(0),
-                               [pi, qi],
-                               11,
-                               'TVD1',
-                               a0=va,
-                               a1=va)
-    rhs = eqn_dict['Ode'][0]
-    diff_var = eqn_dict['Ode'][1]
-
-    assert pycode(rhs) == '(1/2)*va*(pi[0:10] - 2*pi[1:11] + pi[2:12])/dx - 1/2*va**2*(-qi[0:10] + qi[2:12])/(S*dx)'
-    assert pycode(diff_var) == 'pi[1:11]'
+from sympy import pycode, Integer
+
+from Solverz.sym_algebra.transform import finite_difference, semi_descritize
+from Solverz.sym_algebra.symbols import iVar, Para
+
+pi = iVar('pi')
+qi = iVar('qi')
+S = Para('S')
+va = Para('va')
+D = Para('D')
+lam = Para('lam')
+
+
+# finite difference of hyperbolic PDE, the gas equation
+def test_fd():
+    fde = finite_difference(qi,
+                            S * pi,
+                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
+                            [pi, qi],
+                            10,
+                            'central diff')
+    assert pycode(
+        fde) == 'S*dt*(-pi_tag_0[0:10] + pi_tag_0[1:11] - pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[0:10] - qi_tag_0[1:11] + qi[0:10] + qi[1:11]) + (1/4)*dt*dx*lam*va**2*(qi_tag_0[0:10] + qi_tag_0[1:11] + qi[0:10] + qi[1:11])**2/(D*S*(pi_tag_0[0:10] + pi_tag_0[1:11] + pi[0:10] + pi[1:11]))'
+
+    fde = finite_difference(pi,
+                            va ** 2 / S * qi,
+                            Integer(0),
+                            [pi, qi],
+                            10,
+                            'central diff')
+    assert pycode(
+        fde) == 'dx*(-pi_tag_0[0:10] - pi_tag_0[1:11] + pi[0:10] + pi[1:11]) + dt*va**2*(-qi_tag_0[0:10] + qi_tag_0[1:11] - qi[0:10] + qi[1:11])/S'
+
+    fde = finite_difference(qi,
+                            S * pi,
+                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
+                            [pi, qi],
+                            10,
+                            'euler',
+                            direction=1)
+    assert pycode(
+        fde) == 'S*dt*(-pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[1:11] + qi[1:11]) + (1/2)*qi[1:11]**2*dt*dx*lam*va**2/(pi[1:11]*D*S)'
+
+    fde = finite_difference(pi,
+                            va ** 2 / S * qi,
+                            Integer(0),
+                            [pi, qi],
+                            10,
+                            'euler',
+                            direction=1)
+    assert pycode(fde) == 'dx*(-pi_tag_0[1:11] + pi[1:11]) + dt*va**2*(-qi[0:10] + qi[1:11])/S'
+
+    fde = finite_difference(qi,
+                            S * pi,
+                            -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
+                            [pi, qi],
+                            10,
+                            'euler',
+                            direction=-1)
+    assert pycode(
+        fde) == 'S*dt*(-pi[0:10] + pi[1:11]) + dx*(-qi_tag_0[0:10] + qi[0:10]) + (1/2)*qi[0:10]**2*dt*dx*lam*va**2/(pi[0:10]*D*S)'
+
+    fde = finite_difference(pi,
+                            va ** 2 / S * qi,
+                            Integer(0),
+                            [pi, qi],
+                            10,
+                            'euler',
+                            direction=-1)
+    assert pycode(fde) == 'dx*(-pi_tag_0[0:10] + pi[0:10]) + dt*va**2*(-qi[0:10] + qi[1:11])/S'
+
+
+def test_sd():
+    # semi-discretize
+    eqn_dict = semi_descritize(qi,
+                               S * pi,
+                               -lam * va ** 2 * qi ** 2 / (2 * D * S * pi),
+                               [pi, qi],
+                               11,
+                               'TVD1',
+                               a0=va,
+                               a1=va)
+
+    rhs = eqn_dict['Ode'][0]
+    diff_var = eqn_dict['Ode'][1]
+
+    assert pycode(
+        rhs) == '-1/2*S*(-pi[0:10] + pi[2:12])/dx + (1/2)*va*(qi[0:10] - 2*qi[1:11] + qi[2:12])/dx - 1/2*qi[1:11]**2*lam*va**2/(pi[1:11]*D*S)'
+    assert pycode(diff_var) == 'qi[1:11]'
+
+    eqn_dict = semi_descritize(pi,
+                               va ** 2 / S * qi,
+                               Integer(0),
+                               [pi, qi],
+                               11,
+                               'TVD1',
+                               a0=va,
+                               a1=va)
+    rhs = eqn_dict['Ode'][0]
+    diff_var = eqn_dict['Ode'][1]
+
+    assert pycode(rhs) == '(1/2)*va*(pi[0:10] - 2*pi[1:11] + pi[2:12])/dx - 1/2*va**2*(-qi[0:10] + qi[2:12])/(S*dx)'
+    assert pycode(diff_var) == 'pi[1:11]'
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/test/test_matrix_calculus.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/test/test_matrix_calculus.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from Solverz.sym_algebra.symbols import iVar, Para, idx
-from Solverz.sym_algebra.functions import Abs, Mat_Mul
-from Solverz.sym_algebra.matrix_calculus import TensorExpr
-from Solverz.equation.eqn import Eqn
-
-mL = Para('mL', dim=2)
-K = Para(name='K')
-m = iVar(name='m')
-V = Para(name='V', dim=2)
-Ts = iVar(name='Ts')
-Vp = Para(name='Vp', dim=2)
-Touts = iVar(name='Touts')
-li = idx(name='li')
-mq = iVar(name='mq')
-rs = idx(name='rs')
-E8 = Eqn(name='E8', eqn=Mat_Mul(mL, (K * Abs(m) * m)))
-E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) - mq[rs])
-E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], (Touts * Abs(m))))
-TE8 = TensorExpr(E8.RHS)
-TE5 = TensorExpr(E5.RHS)
-TE9 = TensorExpr(E9.RHS)
-
-e = iVar(name='e', value=[1.06, 1, 1.00])
-f = iVar(name='f', value=[0, 0, 0])
-P = iVar(name='P')
-q = iVar(name='q')
-G = Para(name='G', dim=2, value=[0])
-B = Para(name='B', dim=2, value=[0])
-
-P1 = Eqn(name='Active power balance of PQ',
-         eqn=e * (Mat_Mul(G, e) - Mat_Mul(B, f)) + f * (Mat_Mul(B, e) + Mat_Mul(G, f)) - P)
-P2 = Eqn(name='Reactive power balance of PQ',
-         eqn=f * (Mat_Mul(G, e) - Mat_Mul(B, f)) - e * (Mat_Mul(B, e) + Mat_Mul(G, f)) - q)
-TP1 = TensorExpr(P1.RHS)
-TP2 = TensorExpr(P2.RHS)
-
-
-def test_matrix_calculus():
-    assert TE8.diff(m).__repr__() == 'mL@(diag(K*Abs(m)) + diag(K*m*Sign(m)))'
-    assert TE5.diff(m).__repr__() == 'V[rs,:]'
-    assert TE5.diff(mq[rs]).__repr__() == '-1'
-    assert TE9.diff(m).__repr__() == '-Vp[li,:]@diag(Touts*Sign(m)) + diag(Ts[li])@Vp[li,:]@diag(Sign(m))'
-    assert TE9.diff(Ts[li]).__repr__() == 'diag(Vp[li,:]@Abs(m))'
-    assert TE9.diff(Touts).__repr__() == '-Vp[li,:]@diag(Abs(m))'
-    assert TP1.diff(e).__repr__() == 'diag(-B@f + G@e) + diag(e)@G + diag(f)@B'
-    assert TP1.diff(f).__repr__() == 'diag(B@e + G@f) + diag(e)@(-B) + diag(f)@G'
-    assert TP2.diff(e).__repr__() == '-(diag(B@e + G@f) + diag(e)@B) + diag(f)@G'
-    assert TP2.diff(f).__repr__() == 'diag(-B@f + G@e) - diag(e)@G + diag(f)@(-B)'
+from Solverz.sym_algebra.symbols import iVar, Para, idx
+from Solverz.sym_algebra.functions import Abs, Mat_Mul
+from Solverz.sym_algebra.matrix_calculus import TensorExpr
+from Solverz.equation.eqn import Eqn
+
+mL = Para('mL', dim=2)
+K = Para(name='K')
+m = iVar(name='m')
+V = Para(name='V', dim=2)
+Ts = iVar(name='Ts')
+Vp = Para(name='Vp', dim=2)
+Touts = iVar(name='Touts')
+li = idx(name='li')
+mq = iVar(name='mq')
+rs = idx(name='rs')
+E8 = Eqn(name='E8', eqn=Mat_Mul(mL, (K * Abs(m) * m)))
+E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) - mq[rs])
+E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], (Touts * Abs(m))))
+TE8 = TensorExpr(E8.RHS)
+TE5 = TensorExpr(E5.RHS)
+TE9 = TensorExpr(E9.RHS)
+
+e = iVar(name='e', value=[1.06, 1, 1.00])
+f = iVar(name='f', value=[0, 0, 0])
+P = iVar(name='P')
+q = iVar(name='q')
+G = Para(name='G', dim=2, value=[0])
+B = Para(name='B', dim=2, value=[0])
+
+P1 = Eqn(name='Active power balance of PQ',
+         eqn=e * (Mat_Mul(G, e) - Mat_Mul(B, f)) + f * (Mat_Mul(B, e) + Mat_Mul(G, f)) - P)
+P2 = Eqn(name='Reactive power balance of PQ',
+         eqn=f * (Mat_Mul(G, e) - Mat_Mul(B, f)) - e * (Mat_Mul(B, e) + Mat_Mul(G, f)) - q)
+TP1 = TensorExpr(P1.RHS)
+TP2 = TensorExpr(P2.RHS)
+
+
+def test_matrix_calculus():
+    assert TE8.diff(m).__repr__() == 'mL@(diag(K*Abs(m)) + diag(K*m*Sign(m)))'
+    assert TE5.diff(m).__repr__() == 'V[rs,:]'
+    assert TE5.diff(mq[rs]).__repr__() == '-1'
+    assert TE9.diff(m).__repr__() == '-Vp[li,:]@diag(Touts*Sign(m)) + diag(Ts[li])@Vp[li,:]@diag(Sign(m))'
+    assert TE9.diff(Ts[li]).__repr__() == 'diag(Vp[li,:]@Abs(m))'
+    assert TE9.diff(Touts).__repr__() == '-Vp[li,:]@diag(Abs(m))'
+    assert TP1.diff(e).__repr__() == 'diag(-B@f + G@e) + diag(e)@G + diag(f)@B'
+    assert TP1.diff(f).__repr__() == 'diag(B@e + G@f) + diag(e)@(-B) + diag(f)@G'
+    assert TP2.diff(e).__repr__() == '-(diag(B@e + G@f) + diag(e)@B) + diag(f)@G'
+    assert TP2.diff(f).__repr__() == 'diag(-B@f + G@e) - diag(e)@G + diag(f)@(-B)'
```

### Comparing `solverz-0.0.1rc1/Solverz/sym_algebra/test/test_num_alg.py` & `solverz-0.0.1rc2/Solverz/sym_algebra/test/test_num_alg.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import numpy as np
-from sympy import lambdify
-import inspect
-
-from Solverz.sym_algebra.symbols import iVar, Para, idx, IdxVar, IdxPara, Idxidx
-from Solverz.num_api.custom_function import sol_slice
-
-
-# test of IndexPrinter
-def test_IndexPrinter():
-    x = iVar('x')
-    G = Para('G', dim=2)
-    k = idx('k')
-    M = idx('M')
-    j = idx('j')
-    assert x[0].__repr__() == 'x[0]'
-    assert x[k].__repr__() == 'x[k]'
-    assert x[k ** 2].__repr__() == 'x[k**2]'
-    assert x[k ** 2].SymInIndex.__repr__() == "{'k': k}"
-    assert x[[1, k, M[j]]].__repr__() == 'x[[1, k, M[j]]]'
-    assert x[[1, k, M[j]]].SymInIndex.__repr__() == "{'k': k, 'M': M, 'j': j}"
-    assert x[[1, 2, 3]].__repr__() == 'x[[1, 2, 3]]'
-    assert x[1:k - 1:2].__repr__() == 'x[1:k - 1:2]'
-    assert x[1:k - 1:2].SymInIndex.__repr__() == "{'k': k}"
-    assert x[M[j]:k[j] - 1].__repr__() == 'x[M[j]:k[j] - 1]'
-    assert x[M[j]:k[j] - 1].SymInIndex.__repr__() == "{'M': M, 'j': j, 'k': k}"
-    assert G[k, :].__repr__() == 'G[k,:]'
-    assert G[k, :].SymInIndex.__repr__() == "{'k': k}"
-    assert G[:, k[M[j]]].__repr__() == 'G[:,k[M[j]]]'
-    assert G[:, k[M[j]]].SymInIndex.__repr__() == "{'k': k, 'M': M, 'j': j}"
-    assert G[[1, 2, 3], k].__repr__() == 'G[[1, 2, 3],k]'
-
-
-modules = [{'sol_slice': sol_slice}, 'numpy']
-
-
-# test of numpy code printer
-def test_numpy_code_printer():
-    x = iVar('x')
-    k = idx('k')
-    fxk = lambdify([x, k], x[k], modules=modules)
-    assert (inspect.getsource(fxk) ==
-            "def _lambdifygenerated(x, k):\n    return x[k]\n")
-    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
-    k = np.array([0, 2, 5])
-    assert np.isclose(fxk(x, k), np.array([[1], [3], [6]])).all()
-
-    z = iVar('z')
-    fz = lambdify([z], z[1], modules=modules)
-    assert (inspect.getsource(fz) ==
-            "def _lambdifygenerated(z):\n    return z[1]\n")
-    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
-    assert fz(x) == np.array([2])
-
-    x = iVar('x')
-    yy = iVar('yy')
-    k = idx('k')
-    fxyk = lambdify([x, yy, k], x[[1, 2, 3]] + yy[k], modules=modules)
-    assert (inspect.getsource(fxyk) ==
-            "def _lambdifygenerated(x, yy, k):\n    return x[[1, 2, 3]] + yy[k]\n")
-    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
-    yy = np.array([-1, -2, -3, -7]).reshape((-1, 1))
-    k = np.array([0, 3, 3])
-    assert np.isclose(fxyk(x, yy, k), np.array([[1], [-4], [-3]])).all()
-
-    z = iVar('z')
-    k = idx('k')
-    fzk = lambdify([z, k], z[1:k], modules=modules)
-    assert (inspect.getsource(fzk) ==
-            "def _lambdifygenerated(z, k):\n    return z[sol_slice(1, k, None)]\n")
-    z = np.array([-1, -2, -3, -7]).reshape((-1, 1))
-    k = np.array([3])
-    assert np.isclose(fzk(z, k), np.array([[-2], [-3]])).all()
-
-    z = iVar('z')
-    M = idx('M')
-    j = idx('j')
-    fzMj = lambdify([z, M, j], z[1:M[j] + 2], modules=modules)
-    assert (inspect.getsource(fzMj) ==
-            "def _lambdifygenerated(z, M, j):\n    return z[sol_slice(1, M[j] + 2, None)]\n")
-    z = np.array([-1, -2, -3, -7]).reshape((-1, 1))
-    M = np.array([0, 3, 1])
-    j = np.array([1])
-    assert np.isclose(fzMj(z, M, j), np.array([[-2], [-3], [-7]])).all()
-
-    k = idx('k')
-    G = Para('G', dim=2)
-    fGk = lambdify([k, G], G[k, :], modules=modules)
-    assert (inspect.getsource(fGk) ==
-            "def _lambdifygenerated(k, G):\n    return G[k,:]\n")
-    G = np.random.randn(3, 3)
-    k = np.array([1, 2])
-    assert np.isclose(fGk(k, G), G[k, :]).all()
-
-    k = idx('k')
-    G = Para('G', dim=2)
-    j = idx('j')
-    fkjG = lambdify([k, j, G], G[:, 1:k[j] - 1:2], modules=modules)
-    assert (inspect.getsource(fkjG) ==
-            "def _lambdifygenerated(k, j, G):\n    return G[:,sol_slice(1, k[j] - 1, 2)]\n")
-    G = np.random.randn(3, 3)
-    k = np.array([0, 2])
-    j = [1]
-    assert np.isclose(fkjG(k, j, G), G[:, 1:k[j][0] - 1:2]).all()
+import numpy as np
+from sympy import lambdify
+import inspect
+
+from Solverz.sym_algebra.symbols import iVar, Para, idx, IdxVar, IdxPara, Idxidx
+from Solverz.num_api.custom_function import sol_slice
+
+
+# test of IndexPrinter
+def test_IndexPrinter():
+    x = iVar('x')
+    G = Para('G', dim=2)
+    k = idx('k')
+    M = idx('M')
+    j = idx('j')
+    assert x[0].__repr__() == 'x[0]'
+    assert x[k].__repr__() == 'x[k]'
+    assert x[k ** 2].__repr__() == 'x[k**2]'
+    assert x[k ** 2].SymInIndex.__repr__() == "{'k': k}"
+    assert x[[1, k, M[j]]].__repr__() == 'x[[1, k, M[j]]]'
+    assert x[[1, k, M[j]]].SymInIndex.__repr__() == "{'k': k, 'M': M, 'j': j}"
+    assert x[[1, 2, 3]].__repr__() == 'x[[1, 2, 3]]'
+    assert x[1:k - 1:2].__repr__() == 'x[1:k - 1:2]'
+    assert x[1:k - 1:2].SymInIndex.__repr__() == "{'k': k}"
+    assert x[M[j]:k[j] - 1].__repr__() == 'x[M[j]:k[j] - 1]'
+    assert x[M[j]:k[j] - 1].SymInIndex.__repr__() == "{'M': M, 'j': j, 'k': k}"
+    assert G[k, :].__repr__() == 'G[k,:]'
+    assert G[k, :].SymInIndex.__repr__() == "{'k': k}"
+    assert G[:, k[M[j]]].__repr__() == 'G[:,k[M[j]]]'
+    assert G[:, k[M[j]]].SymInIndex.__repr__() == "{'k': k, 'M': M, 'j': j}"
+    assert G[[1, 2, 3], k].__repr__() == 'G[[1, 2, 3],k]'
+
+
+modules = [{'sol_slice': sol_slice}, 'numpy']
+
+
+# test of numpy code printer
+def test_numpy_code_printer():
+    x = iVar('x')
+    k = idx('k')
+    fxk = lambdify([x, k], x[k], modules=modules)
+    assert (inspect.getsource(fxk) ==
+            "def _lambdifygenerated(x, k):\n    return x[k]\n")
+    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
+    k = np.array([0, 2, 5])
+    assert np.isclose(fxk(x, k), np.array([[1], [3], [6]])).all()
+
+    z = iVar('z')
+    fz = lambdify([z], z[1], modules=modules)
+    assert (inspect.getsource(fz) ==
+            "def _lambdifygenerated(z):\n    return z[1]\n")
+    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
+    assert fz(x) == np.array([2])
+
+    x = iVar('x')
+    yy = iVar('yy')
+    k = idx('k')
+    fxyk = lambdify([x, yy, k], x[[1, 2, 3]] + yy[k], modules=modules)
+    assert (inspect.getsource(fxyk) ==
+            "def _lambdifygenerated(x, yy, k):\n    return x[[1, 2, 3]] + yy[k]\n")
+    x = np.array([1, 2, 3, 4, 5, 6]).reshape((-1, 1))
+    yy = np.array([-1, -2, -3, -7]).reshape((-1, 1))
+    k = np.array([0, 3, 3])
+    assert np.isclose(fxyk(x, yy, k), np.array([[1], [-4], [-3]])).all()
+
+    z = iVar('z')
+    k = idx('k')
+    fzk = lambdify([z, k], z[1:k], modules=modules)
+    assert (inspect.getsource(fzk) ==
+            "def _lambdifygenerated(z, k):\n    return z[sol_slice(1, k, None)]\n")
+    z = np.array([-1, -2, -3, -7]).reshape((-1, 1))
+    k = np.array([3])
+    assert np.isclose(fzk(z, k), np.array([[-2], [-3]])).all()
+
+    z = iVar('z')
+    M = idx('M')
+    j = idx('j')
+    fzMj = lambdify([z, M, j], z[1:M[j] + 2], modules=modules)
+    assert (inspect.getsource(fzMj) ==
+            "def _lambdifygenerated(z, M, j):\n    return z[sol_slice(1, M[j] + 2, None)]\n")
+    z = np.array([-1, -2, -3, -7]).reshape((-1, 1))
+    M = np.array([0, 3, 1])
+    j = np.array([1])
+    assert np.isclose(fzMj(z, M, j), np.array([[-2], [-3], [-7]])).all()
+
+    k = idx('k')
+    G = Para('G', dim=2)
+    fGk = lambdify([k, G], G[k, :], modules=modules)
+    assert (inspect.getsource(fGk) ==
+            "def _lambdifygenerated(k, G):\n    return G[k,:]\n")
+    G = np.random.randn(3, 3)
+    k = np.array([1, 2])
+    assert np.isclose(fGk(k, G), G[k, :]).all()
+
+    k = idx('k')
+    G = Para('G', dim=2)
+    j = idx('j')
+    fkjG = lambdify([k, j, G], G[:, 1:k[j] - 1:2], modules=modules)
+    assert (inspect.getsource(fkjG) ==
+            "def _lambdifygenerated(k, j, G):\n    return G[:,sol_slice(1, k[j] - 1, 2)]\n")
+    G = np.random.randn(3, 3)
+    k = np.array([0, 2])
+    j = [1]
+    assert np.isclose(fkjG(k, j, G), G[:, 1:k[j][0] - 1:2]).all()
```

### Comparing `solverz-0.0.1rc1/Solverz/utilities/test/test_address.py` & `solverz-0.0.1rc2/Solverz/utilities/test/test_address.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from Solverz.utilities.address import Address, combine_Address
-
-
-def test_address():
-    a = Address()
-    a.add('x')
-
-    a.add('y', 2)
-    assert a['y'] == slice(0, 2, None)
-    a.update('x', 3)
-    assert a['x'] == slice(0, 3, None)
-
-    try:
-        a.update('z', 3)
-    except KeyError as k:
-        assert k.args[0] == "Non-existent name z, use Address.add() instead"
-
-    a.update('x', 0)
-    try:
-        a['x']
-    except IndexError as i:
-        assert i.args[0] == "index 0 is out of bounds for axis 0 with size 0"
-
-    a.update('x', 5)
-    a0 = a.derive_alias('0')
-    assert a0['x0'] == slice(0, 5, None)
-    assert a0.size['x0'] == 5
-    assert a0.size['y0'] == 2
-    assert a0.total_size == 7
-
-    a2 = combine_Address(a, a0)
-    assert a2['y0'] == slice(12, 14, None)
-
-    b = Address()
-    b.add('x')
-    b.add('y')
-    b.update('x', 5)
-    b.update('y', 2)
-
-    assert a != a0
-    assert a == b
+from Solverz.utilities.address import Address, combine_Address
+
+
+def test_address():
+    a = Address()
+    a.add('x')
+
+    a.add('y', 2)
+    assert a['y'] == slice(0, 2, None)
+    a.update('x', 3)
+    assert a['x'] == slice(0, 3, None)
+
+    try:
+        a.update('z', 3)
+    except KeyError as k:
+        assert k.args[0] == "Non-existent name z, use Address.add() instead"
+
+    a.update('x', 0)
+    try:
+        a['x']
+    except IndexError as i:
+        assert i.args[0] == "index 0 is out of bounds for axis 0 with size 0"
+
+    a.update('x', 5)
+    a0 = a.derive_alias('0')
+    assert a0['x0'] == slice(0, 5, None)
+    assert a0.size['x0'] == 5
+    assert a0.size['y0'] == 2
+    assert a0.total_size == 7
+
+    a2 = combine_Address(a, a0)
+    assert a2['y0'] == slice(12, 14, None)
+
+    b = Address()
+    b.add('x')
+    b.add('y')
+    b.update('x', 5)
+    b.update('y', 2)
+
+    assert a != a0
+    assert a == b
```

### Comparing `solverz-0.0.1rc1/Solverz/variable/ssymbol.py` & `solverz-0.0.1rc2/Solverz/variable/ssymbol.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from typing import Callable, Union, List
-from numbers import Number
-
-import numpy as np
-
-from sympy import Expr, Symbol
-
-from Solverz.sym_algebra.symbols import iVar, iAliasVar, Para, idx
-from Solverz.num_api.Array import Array
-from Solverz.utilities.type_checker import is_number
-
-
-# operator = ['__add__', '__radd__', '__sub__', '__rsub__', '__mul__', '__rmul__', '__truediv__', 'pow']
-
-
-def convert_idx_in_slice(s: slice):
-    if isinstance(s, slice):
-        start = s.start + 0 if s.start is not None else s.start
-        stop = s.stop + 0 if s.stop is not None else s.stop
-        step = s.step + 0 if s.step is not None else s.step
-        s = slice(start, stop, step)
-        return s
-
-
-class sSymBasic:
-    """
-    Basic class for Solverz sSym
-    """
-
-    def __init__(self, name: str, Type: str, value=None, dim: int = 1, init=None):
-        self.name = f'{name}'
-        self.dim = dim
-        if value is not None:
-            self.value = Array(value, dim)
-        else:
-            self.value = None
-        self.Type = Type
-        self.init = sSym2Sym(init) if init is not None else None
-        if self.Type == 'iVar':
-            self.symbol = iVar(self.name)
-        elif self.Type == 'Para':
-            self.symbol = Para(self.name, dim=self.dim)
-        elif self.Type == 'idx':
-            self.symbol = idx(self.name)
-        elif self.Type == 'iAliasVar':
-            self.symbol = iAliasVar(self.name)
-
-    def __neg__(self):
-        return -self.symbol
-
-    def __add__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__add__')(other)
-
-    def __radd__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__radd__')(other)
-
-    def __mul__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__mul__')(other)
-
-    def __rmul__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__rmul__')(other)
-
-    def __sub__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__sub__')(other)
-
-    def __rsub__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__rsub__')(other)
-
-    def __pow__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__pow__')(other)
-
-    def __rpow__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__rpow__')(other)
-
-    def __truediv__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__truediv__')(other)
-
-    def __rtruediv__(self, other):
-        other = sSym2Sym(other)
-        return getattr(self.symbol, '__rtruediv__')(other)
-
-    def __getitem__(self, index):
-        index = index.symbol if isinstance(index, sSymBasic) else index
-        if isinstance(index, tuple):
-            index = tuple([convert_idx_in_slice(arg) if isinstance(arg, slice) else arg + 0 for arg in index])
-        elif isinstance(index, slice):
-            index = convert_idx_in_slice(index)
-        elif isinstance(index, (int, np.integer, Expr)):
-            index = index + 0  # convert IdxParam to idx symbol
-        elif isinstance(index, (list, idx)):
-            index = index
-        else:
-            raise TypeError(f"Index type {type(index)} not implemented!")
-        return self.symbol[index]
-
-
-class Var(sSymBasic):
-    def __init__(self, name: str, value=None, init=None):
-        super().__init__(name=name, Type='iVar', value=value, dim=1, init=init)
-
-
-class AliasVar(sSymBasic):
-    def __init__(self, name: str, step=1, value=None, init=None):
-        name = name + '_tag_' + str(step-1)
-        super().__init__(name=name, Type='iAliasVar', value=value, dim=1, init=init)
-        self.step = step
-
-
-def sSym2Sym(x):
-    if isinstance(x, sSymBasic):
-        return x.symbol
-    elif isinstance(x, (Expr, Symbol)):
-        return x
-    elif is_number(x):
-        return x
-    else:
-        raise TypeError(f'Input type {type(x)} not supported!')
-
+from typing import Callable, Union, List
+from numbers import Number
+
+import numpy as np
+
+from sympy import Expr, Symbol
+
+from Solverz.sym_algebra.symbols import iVar, iAliasVar, Para, idx
+from Solverz.num_api.Array import Array
+from Solverz.utilities.type_checker import is_number
+
+
+# operator = ['__add__', '__radd__', '__sub__', '__rsub__', '__mul__', '__rmul__', '__truediv__', 'pow']
+
+
+def convert_idx_in_slice(s: slice):
+    if isinstance(s, slice):
+        start = s.start + 0 if s.start is not None else s.start
+        stop = s.stop + 0 if s.stop is not None else s.stop
+        step = s.step + 0 if s.step is not None else s.step
+        s = slice(start, stop, step)
+        return s
+
+
+class sSymBasic:
+    """
+    Basic class for Solverz sSym
+    """
+
+    def __init__(self, name: str, Type: str, value=None, dim: int = 1, init=None):
+        self.name = f'{name}'
+        self.dim = dim
+        if value is not None:
+            self.value = Array(value, dim)
+        else:
+            self.value = None
+        self.Type = Type
+        self.init = sSym2Sym(init) if init is not None else None
+        if self.Type == 'iVar':
+            self.symbol = iVar(self.name)
+        elif self.Type == 'Para':
+            self.symbol = Para(self.name, dim=self.dim)
+        elif self.Type == 'idx':
+            self.symbol = idx(self.name)
+        elif self.Type == 'iAliasVar':
+            self.symbol = iAliasVar(self.name)
+
+    def __neg__(self):
+        return -self.symbol
+
+    def __add__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__add__')(other)
+
+    def __radd__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__radd__')(other)
+
+    def __mul__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__mul__')(other)
+
+    def __rmul__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__rmul__')(other)
+
+    def __sub__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__sub__')(other)
+
+    def __rsub__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__rsub__')(other)
+
+    def __pow__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__pow__')(other)
+
+    def __rpow__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__rpow__')(other)
+
+    def __truediv__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__truediv__')(other)
+
+    def __rtruediv__(self, other):
+        other = sSym2Sym(other)
+        return getattr(self.symbol, '__rtruediv__')(other)
+
+    def __getitem__(self, index):
+        index = index.symbol if isinstance(index, sSymBasic) else index
+        if isinstance(index, tuple):
+            index = tuple([convert_idx_in_slice(arg) if isinstance(arg, slice) else arg + 0 for arg in index])
+        elif isinstance(index, slice):
+            index = convert_idx_in_slice(index)
+        elif isinstance(index, (int, np.integer, Expr)):
+            index = index + 0  # convert IdxParam to idx symbol
+        elif isinstance(index, (list, idx)):
+            index = index
+        else:
+            raise TypeError(f"Index type {type(index)} not implemented!")
+        return self.symbol[index]
+
+
+class Var(sSymBasic):
+    def __init__(self, name: str, value=None, init=None):
+        super().__init__(name=name, Type='iVar', value=value, dim=1, init=init)
+
+
+class AliasVar(sSymBasic):
+    def __init__(self, name: str, step=1, value=None, init=None):
+        name = name + '_tag_' + str(step-1)
+        super().__init__(name=name, Type='iAliasVar', value=value, dim=1, init=init)
+        self.step = step
+
+
+def sSym2Sym(x):
+    if isinstance(x, sSymBasic):
+        return x.symbol
+    elif isinstance(x, (Expr, Symbol)):
+        return x
+    elif is_number(x):
+        return x
+    else:
+        raise TypeError(f'Input type {type(x)} not supported!')
+
```

### Comparing `solverz-0.0.1rc1/Solverz/variable/variables.py` & `solverz-0.0.1rc2/Solverz/variable/variables.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from typing import Union, List, Dict
-import warnings
-
-import numpy as np
-
-from Solverz.sym_algebra.symbols import iVar
-from Solverz.utilities.address import Address, combine_Address
-from Solverz.num_api.Array import Array
-
-
-def as_Vars(var: Union[iVar, List[iVar]]) -> Vars:
-    var = [var] if isinstance(var, iVar) else var
-    a = Address()
-
-    for var_ in var:
-        if not isinstance(var_, iVar):
-            raise TypeError(f'Type {type(var_)} cannot be parsed as iVar object')
-        if var_.initialized:
-            a.add(var_.name, var_.value.shape[0])
-        else:
-            warnings.warn(f"Variable {var_.name} not initialized, set to zero")
-            a.add(var_.name, 1)
-
-    array = np.zeros((a.total_size, ))
-    for var_ in var:
-        if var_.initialized:
-            array[a[var_.name]] = var_.value
-        else:
-            array[a[var_.name]] = 0
-
-    return Vars(a, array)
-
-
-class VarsBasic:
-
-    def __init__(self):
-        self.a: Address = Address()
-        self.array = None
-
-    def __array__(self):
-        return self.array
-
-    @property
-    def total_size(self):
-        return self.a.total_size
-
-    @property
-    def var_size(self) -> Dict[str, int]:
-        return self.a.size
-
-    @property
-    def var_list(self):
-        return list(self.a.v.keys())
-
-
-def combine_Vars(vars1: Vars, vars2: Vars):
-    a = combine_Address(vars1.a, vars2.a)
-    array = np.concatenate([vars1.array, vars2.array], axis=0)
-    return Vars(a, array)
-
-
-class Vars(VarsBasic):
-
-    def __init__(self,
-                 a: Address,
-                 array: np.ndarray):
-        super().__init__()
-        self.a = a
-        array = Array(array, dim=1)
-        if array.shape[0] != self.a.total_size:
-            raise ValueError("Unequal address size and array size!")
-        else:
-            self.array = array
-
-    def __getitem__(self, item):
-        if isinstance(item, str):
-            return self.array[self.a[item]]
-        else:
-            return self.array[item]
-
-    def __setitem__(self, key, value):
-        if key in self.var_list:
-            temp = Array(value, dim=1)
-            if temp.shape[0] == self.array[self.a[key]].shape[0]:
-                self.array[self.a[key]] = temp
-            else:
-                raise ValueError(f'Incompatible input array shape!')
-        else:
-            raise ValueError(f'There is no variable {key}!')
-
-    def __repr__(self):
-        return f'Variables (size {self.total_size}) {list(self.var_list)}'
-
-    def __mul__(self, other: Union[int, float, Vars]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = new_vars.array * other
-            return new_vars
-        elif isinstance(other, Vars):
-            if self.a == other.a:
-                new_vars.array[:] = new_vars.array * other.array
-                return new_vars
-            else:
-                raise ValueError('Cannot multiply Vars object by another one with different variables!')
-        else:
-            raise TypeError(f'Input type {type(other)} invalid')
-
-    def __rmul__(self, other: Union[int, float, Vars]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = other * new_vars.array
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = other.array * new_vars.array
-            return new_vars
-        else:
-            raise TypeError(f'Input type {type(other)} invalid')
-
-    def __add__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        if isinstance(other, int) or isinstance(other, float):
-            return Vars(self.a, self.array+other)
-        elif isinstance(other, Vars):
-            return Vars(self.a, self.array+other.array)
-        elif isinstance(other, np.ndarray):
-            return Vars(self.a, self.array+other)
-
-    def __radd__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = other + new_vars.array
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = other.array + new_vars.array
-            return new_vars
-        elif isinstance(other, np.ndarray):
-            if new_vars.total_size != other.reshape(-1, ).shape[0]:
-                raise ValueError('Incompatible array size')
-            else:
-                new_vars.array[:] = other.reshape(-1, ) + new_vars.array
-                return new_vars
-
-    def __sub__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = new_vars.array - other
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = new_vars.array - other.array
-            return new_vars
-        elif isinstance(other, np.ndarray):
-            if new_vars.total_size != other.reshape(-1, ).shape[0]:
-                raise ValueError('Incompatible array size')
-            else:
-                new_vars.array[:] = new_vars.array - other.reshape(-1, )
-                return new_vars
-
-    def __rsub__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = other - new_vars.array
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = other.array - new_vars.array
-            return new_vars
-        elif isinstance(other, np.ndarray):
-            if new_vars.total_size != other.reshape(-1, ).shape[0]:
-                raise ValueError('Incompatible array size')
-            else:
-                new_vars.array[:] = other.reshape(-1, ) - new_vars.array
-                return new_vars
-
-    def __truediv__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = new_vars.array / other
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = new_vars.array / other.array
-            return new_vars
-        elif isinstance(other, np.ndarray):
-            if new_vars.total_size != other.reshape(-1, ).shape[0]:
-                raise ValueError('Incompatible array size')
-            else:
-                new_vars.array[:] = new_vars.array / other.reshape(-1, )
-                return new_vars
-
-    def __rtruediv__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
-        new_vars = deepcopy(self)
-        if isinstance(other, int) or isinstance(other, float):
-            new_vars.array[:] = other / new_vars.array
-            return new_vars
-        elif isinstance(other, Vars):
-            new_vars.array[:] = other.array / new_vars.array
-            return new_vars
-        elif isinstance(other, np.ndarray):
-            if new_vars.total_size != other.reshape(-1, ).shape[0]:
-                raise ValueError('Incompatible array size')
-            else:
-                new_vars.array[:] = other.reshape(-1, ) / new_vars.array
-                return new_vars
-
-    def derive_alias(self, suffix: str):
-
-        return Vars(self.a.derive_alias(suffix), self.array)
-
-
-class TimeVars(VarsBasic):
-
-    def __init__(self,
-                 Vars_: Vars,
-                 length: int = 1001
-                 ):
-
-        super().__init__()
-
-        self.a = Vars_.a
-
-        self.array = np.zeros((length, self.total_size))
-        if length > 0:
-            self.array[0, :] = Vars_.array
-
-    def __getitem__(self, item):
-        """
-        case item==str
-        case item==number
-        case item=[str, number]
-        :param item:
-        :return: Time series frame, a Vars object
-        """
-        if isinstance(item, int):
-            if item > self.len:
-                raise ValueError(f'Exceed maximum indices of Time-series Variables')
-            else:
-                return Vars(self.a, self.array[item, 0:])
-        elif isinstance(item, str):
-            return self.array[:, self.a[item]]
-        elif isinstance(item, slice):
-            temp = TimeVars(self[item.start], length=0)
-            temp.array = self.array[item, 0:]
-            return temp
-        else:
-            # not implemented
-            raise NotImplementedError(f'Unsupported indices')
-
-    def __setitem__(self, key: int, value: Vars):
-        """
-        assign the Vars object to time series frame
-        :param key:
-        :param value:
-        :return: none
-        """
-        if isinstance(key, int):
-            if key > self.len:
-                raise ValueError(f'Exceed the maximum index, which is {self.len}')
-            else:
-                self.array[key:key + 1, :] = value.array[:].T
-        else:
-            raise NotImplementedError(f'Unsupported indices')
-
-    @property
-    def T(self):
-        """
-        Transpose of TimeVars
-        :return:
-        """
-        return self.array.T
-
-    @property
-    def len(self):
-        return self.array.shape[0]
-
-    def __repr__(self):
-        return f'Time-series (size {self.len}×{self.total_size}) {list(self.var_list)}'
-
-    def append(self, other: TimeVars):
-        if self.a == other.a:
-            self.array = np.concatenate([self.array, other.array], axis=0)
-        else:
-            raise ValueError("Cannot concatenate two TimeVars with different variable addresses!")
+from __future__ import annotations
+
+from copy import deepcopy
+from typing import Union, List, Dict
+import warnings
+
+import numpy as np
+
+from Solverz.sym_algebra.symbols import iVar
+from Solverz.utilities.address import Address, combine_Address
+from Solverz.num_api.Array import Array
+
+
+def as_Vars(var: Union[iVar, List[iVar]]) -> Vars:
+    var = [var] if isinstance(var, iVar) else var
+    a = Address()
+
+    for var_ in var:
+        if not isinstance(var_, iVar):
+            raise TypeError(f'Type {type(var_)} cannot be parsed as iVar object')
+        if var_.initialized:
+            a.add(var_.name, var_.value.shape[0])
+        else:
+            warnings.warn(f"Variable {var_.name} not initialized, set to zero")
+            a.add(var_.name, 1)
+
+    array = np.zeros((a.total_size, ))
+    for var_ in var:
+        if var_.initialized:
+            array[a[var_.name]] = var_.value
+        else:
+            array[a[var_.name]] = 0
+
+    return Vars(a, array)
+
+
+class VarsBasic:
+
+    def __init__(self):
+        self.a: Address = Address()
+        self.array = None
+
+    def __array__(self):
+        return self.array
+
+    @property
+    def total_size(self):
+        return self.a.total_size
+
+    @property
+    def var_size(self) -> Dict[str, int]:
+        return self.a.size
+
+    @property
+    def var_list(self):
+        return list(self.a.v.keys())
+
+
+def combine_Vars(vars1: Vars, vars2: Vars):
+    a = combine_Address(vars1.a, vars2.a)
+    array = np.concatenate([vars1.array, vars2.array], axis=0)
+    return Vars(a, array)
+
+
+class Vars(VarsBasic):
+
+    def __init__(self,
+                 a: Address,
+                 array: np.ndarray):
+        super().__init__()
+        self.a = a
+        array = Array(array, dim=1)
+        if array.shape[0] != self.a.total_size:
+            raise ValueError("Unequal address size and array size!")
+        else:
+            self.array = array
+
+    def __getitem__(self, item):
+        if isinstance(item, str):
+            return self.array[self.a[item]]
+        else:
+            return self.array[item]
+
+    def __setitem__(self, key, value):
+        if key in self.var_list:
+            temp = Array(value, dim=1)
+            if temp.shape[0] == self.array[self.a[key]].shape[0]:
+                self.array[self.a[key]] = temp
+            else:
+                raise ValueError(f'Incompatible input array shape!')
+        else:
+            raise ValueError(f'There is no variable {key}!')
+
+    def __repr__(self):
+        return f'Variables (size {self.total_size}) {list(self.var_list)}'
+
+    def __mul__(self, other: Union[int, float, Vars]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = new_vars.array * other
+            return new_vars
+        elif isinstance(other, Vars):
+            if self.a == other.a:
+                new_vars.array[:] = new_vars.array * other.array
+                return new_vars
+            else:
+                raise ValueError('Cannot multiply Vars object by another one with different variables!')
+        else:
+            raise TypeError(f'Input type {type(other)} invalid')
+
+    def __rmul__(self, other: Union[int, float, Vars]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = other * new_vars.array
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = other.array * new_vars.array
+            return new_vars
+        else:
+            raise TypeError(f'Input type {type(other)} invalid')
+
+    def __add__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        if isinstance(other, int) or isinstance(other, float):
+            return Vars(self.a, self.array+other)
+        elif isinstance(other, Vars):
+            return Vars(self.a, self.array+other.array)
+        elif isinstance(other, np.ndarray):
+            return Vars(self.a, self.array+other)
+
+    def __radd__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = other + new_vars.array
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = other.array + new_vars.array
+            return new_vars
+        elif isinstance(other, np.ndarray):
+            if new_vars.total_size != other.reshape(-1, ).shape[0]:
+                raise ValueError('Incompatible array size')
+            else:
+                new_vars.array[:] = other.reshape(-1, ) + new_vars.array
+                return new_vars
+
+    def __sub__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = new_vars.array - other
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = new_vars.array - other.array
+            return new_vars
+        elif isinstance(other, np.ndarray):
+            if new_vars.total_size != other.reshape(-1, ).shape[0]:
+                raise ValueError('Incompatible array size')
+            else:
+                new_vars.array[:] = new_vars.array - other.reshape(-1, )
+                return new_vars
+
+    def __rsub__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = other - new_vars.array
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = other.array - new_vars.array
+            return new_vars
+        elif isinstance(other, np.ndarray):
+            if new_vars.total_size != other.reshape(-1, ).shape[0]:
+                raise ValueError('Incompatible array size')
+            else:
+                new_vars.array[:] = other.reshape(-1, ) - new_vars.array
+                return new_vars
+
+    def __truediv__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = new_vars.array / other
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = new_vars.array / other.array
+            return new_vars
+        elif isinstance(other, np.ndarray):
+            if new_vars.total_size != other.reshape(-1, ).shape[0]:
+                raise ValueError('Incompatible array size')
+            else:
+                new_vars.array[:] = new_vars.array / other.reshape(-1, )
+                return new_vars
+
+    def __rtruediv__(self, other: Union[int, float, Vars, np.ndarray]) -> Vars:
+        new_vars = deepcopy(self)
+        if isinstance(other, int) or isinstance(other, float):
+            new_vars.array[:] = other / new_vars.array
+            return new_vars
+        elif isinstance(other, Vars):
+            new_vars.array[:] = other.array / new_vars.array
+            return new_vars
+        elif isinstance(other, np.ndarray):
+            if new_vars.total_size != other.reshape(-1, ).shape[0]:
+                raise ValueError('Incompatible array size')
+            else:
+                new_vars.array[:] = other.reshape(-1, ) / new_vars.array
+                return new_vars
+
+    def derive_alias(self, suffix: str):
+
+        return Vars(self.a.derive_alias(suffix), self.array)
+
+
+class TimeVars(VarsBasic):
+
+    def __init__(self,
+                 Vars_: Vars,
+                 length: int = 1001
+                 ):
+
+        super().__init__()
+
+        self.a = Vars_.a
+
+        self.array = np.zeros((length, self.total_size))
+        if length > 0:
+            self.array[0, :] = Vars_.array
+
+    def __getitem__(self, item):
+        """
+        case item==str
+        case item==number
+        case item=[str, number]
+        :param item:
+        :return: Time series frame, a Vars object
+        """
+        if isinstance(item, int):
+            if item > self.len:
+                raise ValueError(f'Exceed maximum indices of Time-series Variables')
+            else:
+                return Vars(self.a, self.array[item, 0:])
+        elif isinstance(item, str):
+            return self.array[:, self.a[item]]
+        elif isinstance(item, slice):
+            temp = TimeVars(self[item.start], length=0)
+            temp.array = self.array[item, 0:]
+            return temp
+        else:
+            # not implemented
+            raise NotImplementedError(f'Unsupported indices')
+
+    def __setitem__(self, key: int, value: Vars):
+        """
+        assign the Vars object to time series frame
+        :param key:
+        :param value:
+        :return: none
+        """
+        if isinstance(key, int):
+            if key > self.len:
+                raise ValueError(f'Exceed the maximum index, which is {self.len}')
+            else:
+                self.array[key:key + 1, :] = value.array[:].T
+        else:
+            raise NotImplementedError(f'Unsupported indices')
+
+    @property
+    def T(self):
+        """
+        Transpose of TimeVars
+        :return:
+        """
+        return self.array.T
+
+    @property
+    def len(self):
+        return self.array.shape[0]
+
+    def __repr__(self):
+        return f'Time-series (size {self.len}×{self.total_size}) {list(self.var_list)}'
+
+    def append(self, other: TimeVars):
+        if self.a == other.a:
+            self.array = np.concatenate([self.array, other.array], axis=0)
+        else:
+            raise ValueError("Cannot concatenate two TimeVars with different variable addresses!")
```

### Comparing `solverz-0.0.1rc1/Solverz/variable/test/test_variable.py` & `solverz-0.0.1rc2/Solverz/variable/test/test_variable.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import numpy as np
-
-from Solverz.variable.variables import as_Vars, combine_Vars, Vars, TimeVars
-from Solverz.sym_algebra.symbols import iVar, Para
-
-
-def test_Vars():
-    # as_Vars
-    a = iVar('a', [1, 2, 3])
-    b = Para('b', [4, 5, 6])
-    try:
-        y = as_Vars([a, b])
-    except TypeError as e:
-        assert e.args[0] == "Type <class 'Solverz.sym_algebra.symbols.Para'> cannot be parsed as iVar object"
-
-    a = iVar('a', [1, 2, 3])
-    b = iVar('b', [4, 5, 6])
-    y = as_Vars([a, b])
-    assert np.all(np.isclose(y.array, [1, 2, 3, 4, 5, 6]))
-    assert y[0] == 1
-    assert y[2:4].tolist() == [3, 4]
-    assert y[:-1].tolist() == [1, 2, 3, 4, 5]
-    assert y[::2].tolist() == [1, 3, 5]
-
-    c = iVar('c', [0, -2, 3.0])
-    d = iVar('d', [100, 5, 6])
-    z = as_Vars([c, d])
-    assert np.all(np.isclose(z.array, [0, -2, 3.0, 100, 5, 6]))
-
-    # combine_Vars
-    x = combine_Vars(y, z)
-    assert np.all(np.isclose(x.array, [1, 2, 3, 4, 5, 6, 0, -2, 3.0, 100, 5, 6]))
-
-    # get_item
-    assert np.all(np.isclose(y['a'], [1.0, 2.0, 3.0]))
-
-    # set_item
-    y['a'] = [7, 8, 9]
-
-    try:
-        y['a'] = [1]
-    except ValueError as e:
-        assert e.args[0] == 'Incompatible input array shape!'
-
-    try:
-        y['e'] = [1]
-    except ValueError as e:
-        assert e.args[0] == 'There is no variable e!'
-
-    assert y.__repr__() == "Variables (size 6) ['a', 'b']"
-
-    # operator
-    xr = np.array([1, 2, 3, 4, 5, 6, 0, -2, 3.0, 100, 5, 6])
-    # Mul
-    assert np.all(np.isclose((x * 2).array, 2 * xr))
-    assert np.all(np.isclose((x * 2)['c'], [0, -4, 6.0]))
-    assert np.all(np.isclose((2 * x).array, 2 * xr))
-    assert np.all(np.isclose((2 * x)['c'], [0, -4, 6.0]))
-
-    try:
-        np.all(np.isclose((y * z)['c'], [0, -4, 6.0]))
-    except ValueError as v:
-        assert v.args[0] == 'Cannot multiply Vars object by another one with different variables!'
-    assert np.all(np.isclose((y * y)['a'], [49., 64., 81.]))
-
-    # Add
-    assert np.all(np.isclose((2 + x).array, 2 + xr))
-    assert np.all(np.isclose((2 + x)['c'], [2, 0, 5]))
-    assert np.all(np.isclose((x + 2).array, 2 + xr))
-    assert np.all(np.isclose((x + 2)['c'], [2, 0, 5]))
-
-    # Sub
-    assert np.all(np.isclose((2 - x).array, 2 - xr))
-    assert np.all(np.isclose((2 - x)['c'], [2, 4, -1]))
-    assert np.all(np.isclose((x - 2).array, xr - 2))
-    assert np.all(np.isclose((x - 2)['c'], [-2, -4, 1]))
-
-    # Div
-    assert np.all(np.isclose((x / 2).array, xr / 2))
-    assert np.all(np.isclose((2 / y).array, 2 / np.array([7, 8, 9, 4, 5, 6])))
-    assert np.all(np.isclose((x / 2)['d'], [50., 2.5, 3.]))
-    assert np.all(np.isclose((2 / y)['b'], [0.5, 0.4, 0.33333333]))
-
-    # derive_alias
-    x0 = x.derive_alias('0')
-    assert np.all(np.isclose(x0.array, x.array))
-    assert np.all(np.isclose(x0['a0'], x['a']))
-
-
-def test_TimeVars():
-    a = iVar('a', [1, 2, 3])
-    b = iVar('b', [4, 5, 6])
-    y = as_Vars([a, b])
-    yt = TimeVars(y, length=1001)
-    assert yt.a == y.a
-
-    # __getitem__()
-    assert np.all(np.isclose(yt[0].array, [1., 2., 3., 4., 5., 6.]))
-    assert np.all(np.isclose(yt['a'], yt.array[:, 0:3]))
-    assert np.all(np.isclose(yt[0:5].array, yt.array[0:5, :]))
-
-    # __setitem__()
-    yt[2] = 2 * y
-    assert np.all(np.isclose(yt[2].array, [2., 4., 6., 8., 10., 12.]))
-    assert yt.len == 1001
-
-    # T
-    assert np.all(np.isclose(yt.T, yt.array.T))
-
-    # __repr__()
-    assert yt.__repr__() == "Time-series (size 1001×6) ['a', 'b']"
-
-    # append
-    Y = TimeVars(y, length=5)
-    Y.append(Y)
-    assert Y.len == 10
-    np.testing.assert_allclose(Y[5], np.array([1, 2, 3, 4, 5, 6]))
-
-    Y1 = TimeVars(y, length=0)
-    Y1.append(Y)
-    assert Y1.len == 10
-    np.testing.assert_allclose(Y1[0], np.array([1, 2, 3, 4, 5, 6]))
-    np.testing.assert_allclose(Y1[-1], np.array([0, 0, 0, 0, 0, 0]))
+import numpy as np
+
+from Solverz.variable.variables import as_Vars, combine_Vars, Vars, TimeVars
+from Solverz.sym_algebra.symbols import iVar, Para
+
+
+def test_Vars():
+    # as_Vars
+    a = iVar('a', [1, 2, 3])
+    b = Para('b', [4, 5, 6])
+    try:
+        y = as_Vars([a, b])
+    except TypeError as e:
+        assert e.args[0] == "Type <class 'Solverz.sym_algebra.symbols.Para'> cannot be parsed as iVar object"
+
+    a = iVar('a', [1, 2, 3])
+    b = iVar('b', [4, 5, 6])
+    y = as_Vars([a, b])
+    assert np.all(np.isclose(y.array, [1, 2, 3, 4, 5, 6]))
+    assert y[0] == 1
+    assert y[2:4].tolist() == [3, 4]
+    assert y[:-1].tolist() == [1, 2, 3, 4, 5]
+    assert y[::2].tolist() == [1, 3, 5]
+
+    c = iVar('c', [0, -2, 3.0])
+    d = iVar('d', [100, 5, 6])
+    z = as_Vars([c, d])
+    assert np.all(np.isclose(z.array, [0, -2, 3.0, 100, 5, 6]))
+
+    # combine_Vars
+    x = combine_Vars(y, z)
+    assert np.all(np.isclose(x.array, [1, 2, 3, 4, 5, 6, 0, -2, 3.0, 100, 5, 6]))
+
+    # get_item
+    assert np.all(np.isclose(y['a'], [1.0, 2.0, 3.0]))
+
+    # set_item
+    y['a'] = [7, 8, 9]
+
+    try:
+        y['a'] = [1]
+    except ValueError as e:
+        assert e.args[0] == 'Incompatible input array shape!'
+
+    try:
+        y['e'] = [1]
+    except ValueError as e:
+        assert e.args[0] == 'There is no variable e!'
+
+    assert y.__repr__() == "Variables (size 6) ['a', 'b']"
+
+    # operator
+    xr = np.array([1, 2, 3, 4, 5, 6, 0, -2, 3.0, 100, 5, 6])
+    # Mul
+    assert np.all(np.isclose((x * 2).array, 2 * xr))
+    assert np.all(np.isclose((x * 2)['c'], [0, -4, 6.0]))
+    assert np.all(np.isclose((2 * x).array, 2 * xr))
+    assert np.all(np.isclose((2 * x)['c'], [0, -4, 6.0]))
+
+    try:
+        np.all(np.isclose((y * z)['c'], [0, -4, 6.0]))
+    except ValueError as v:
+        assert v.args[0] == 'Cannot multiply Vars object by another one with different variables!'
+    assert np.all(np.isclose((y * y)['a'], [49., 64., 81.]))
+
+    # Add
+    assert np.all(np.isclose((2 + x).array, 2 + xr))
+    assert np.all(np.isclose((2 + x)['c'], [2, 0, 5]))
+    assert np.all(np.isclose((x + 2).array, 2 + xr))
+    assert np.all(np.isclose((x + 2)['c'], [2, 0, 5]))
+
+    # Sub
+    assert np.all(np.isclose((2 - x).array, 2 - xr))
+    assert np.all(np.isclose((2 - x)['c'], [2, 4, -1]))
+    assert np.all(np.isclose((x - 2).array, xr - 2))
+    assert np.all(np.isclose((x - 2)['c'], [-2, -4, 1]))
+
+    # Div
+    assert np.all(np.isclose((x / 2).array, xr / 2))
+    assert np.all(np.isclose((2 / y).array, 2 / np.array([7, 8, 9, 4, 5, 6])))
+    assert np.all(np.isclose((x / 2)['d'], [50., 2.5, 3.]))
+    assert np.all(np.isclose((2 / y)['b'], [0.5, 0.4, 0.33333333]))
+
+    # derive_alias
+    x0 = x.derive_alias('0')
+    assert np.all(np.isclose(x0.array, x.array))
+    assert np.all(np.isclose(x0['a0'], x['a']))
+
+
+def test_TimeVars():
+    a = iVar('a', [1, 2, 3])
+    b = iVar('b', [4, 5, 6])
+    y = as_Vars([a, b])
+    yt = TimeVars(y, length=1001)
+    assert yt.a == y.a
+
+    # __getitem__()
+    assert np.all(np.isclose(yt[0].array, [1., 2., 3., 4., 5., 6.]))
+    assert np.all(np.isclose(yt['a'], yt.array[:, 0:3]))
+    assert np.all(np.isclose(yt[0:5].array, yt.array[0:5, :]))
+
+    # __setitem__()
+    yt[2] = 2 * y
+    assert np.all(np.isclose(yt[2].array, [2., 4., 6., 8., 10., 12.]))
+    assert yt.len == 1001
+
+    # T
+    assert np.all(np.isclose(yt.T, yt.array.T))
+
+    # __repr__()
+    assert yt.__repr__() == "Time-series (size 1001×6) ['a', 'b']"
+
+    # append
+    Y = TimeVars(y, length=5)
+    Y.append(Y)
+    assert Y.len == 10
+    np.testing.assert_allclose(Y[5], np.array([1, 2, 3, 4, 5, 6]))
+
+    Y1 = TimeVars(y, length=0)
+    Y1.append(Y)
+    assert Y1.len == 10
+    np.testing.assert_allclose(Y1[0], np.array([1, 2, 3, 4, 5, 6]))
+    np.testing.assert_allclose(Y1[-1], np.array([0, 0, 0, 0, 0, 0]))
```

### Comparing `solverz-0.0.1rc1/docs/Makefile` & `solverz-0.0.1rc2/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = src
-BUILDDIR      = build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = src
+BUILDDIR      = build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `solverz-0.0.1rc1/docs/ext/convert-svg-to-pdf.py` & `solverz-0.0.1rc2/docs/ext/convert-svg-to-pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,238 +1,232 @@
 00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
 00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
-00000020: 6e73 0d0a 2222 220d 0a20 2020 2043 6f6e  ns.."""..    Con
-00000030: 7665 7274 7320 5356 4720 696d 6167 6573  verts SVG images
-00000040: 2074 6f20 5044 4620 7573 696e 6720 6368   to PDF using ch
-00000050: 726f 6d65 2069 6e20 6361 7365 2074 6865  rome in case the
-00000060: 2062 7569 6c64 6572 2064 6f65 7320 6e6f   builder does no
-00000070: 740d 0a20 2020 2073 7570 706f 7274 2053  t..    support S
-00000080: 5647 2069 6d61 6765 7320 6e61 7469 7665  VG images native
-00000090: 6c79 2028 652e 672e 204c 6154 6558 292e  ly (e.g. LaTeX).
-000000a0: 0d0a 0d0a 2222 220d 0a0d 0a66 726f 6d20  ...."""....from 
-000000b0: 7370 6869 6e78 2e74 7261 6e73 666f 726d  sphinx.transform
-000000c0: 732e 706f 7374 5f74 7261 6e73 666f 726d  s.post_transform
-000000d0: 732e 696d 6167 6573 2069 6d70 6f72 7420  s.images import 
-000000e0: 496d 6167 6543 6f6e 7665 7274 6572 0d0a  ImageConverter..
-000000f0: 6672 6f6d 2073 7068 696e 782e 7574 696c  from sphinx.util
-00000100: 2069 6d70 6f72 7420 6c6f 6767 696e 670d   import logging.
-00000110: 0a69 6d70 6f72 7420 6f73 0d0a 696d 706f  .import os..impo
-00000120: 7274 2070 6c61 7466 6f72 6d0d 0a66 726f  rt platform..fro
-00000130: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000140: 416e 7920 2023 204e 4f51 410d 0a66 726f  Any  # NOQA..fro
-00000150: 6d20 7370 6869 6e78 2e61 7070 6c69 6361  m sphinx.applica
-00000160: 7469 6f6e 2069 6d70 6f72 7420 5370 6869  tion import Sphi
-00000170: 6e78 2020 2320 4e4f 5141 0d0a 0d0a 0d0a  nx  # NOQA......
-00000180: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
-00000190: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
-000001a0: 655f 5f29 0d0a 0d0a 0d0a 636c 6173 7320  e__)......class 
-000001b0: 436f 6e76 6572 7465 7228 496d 6167 6543  Converter(ImageC
-000001c0: 6f6e 7665 7274 6572 293a 0d0a 2020 2020  onverter):..    
-000001d0: 636f 6e76 6572 7369 6f6e 5f72 756c 6573  conversion_rules
-000001e0: 203d 205b 0d0a 2020 2020 2020 2020 2827   = [..        ('
-000001f0: 696d 6167 652f 7376 672b 786d 6c27 2c20  image/svg+xml', 
-00000200: 2761 7070 6c69 6361 7469 6f6e 2f70 6466  'application/pdf
-00000210: 2729 2c0d 0a20 2020 205d 0d0a 0d0a 2020  '),..    ]....  
-00000220: 2020 6465 6620 6973 5f61 7661 696c 6162    def is_availab
-00000230: 6c65 2873 656c 6629 202d 3e20 626f 6f6c  le(self) -> bool
-00000240: 3a0d 0a20 2020 2020 2020 2022 2222 436f  :..        """Co
-00000250: 6e66 6972 6d73 2069 6620 636f 6e76 6572  nfirms if conver
-00000260: 7465 7220 6973 2061 7661 696c 6162 6c65  ter is available
-00000270: 206f 7220 6e6f 742e 2222 220d 0a20 2020   or not."""..   
-00000280: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00000290: 0d0a 0d0a 2020 2020 6465 6620 6368 726f  ....    def chro
-000002a0: 6d65 5f63 6f6d 6d61 6e64 2873 656c 6629  me_command(self)
-000002b0: 202d 3e20 7374 7220 7c20 4e6f 6e65 3a0d   -> str | None:.
-000002c0: 0a20 2020 2020 2020 2069 6620 706c 6174  .        if plat
-000002d0: 666f 726d 2e77 696e 3332 5f76 6572 2829  form.win32_ver()
-000002e0: 5b30 5d3a 0d0a 2020 2020 2020 2020 2020  [0]:..          
-000002f0: 2020 6966 206f 732e 7379 7374 656d 2822    if os.system("
-00000300: 7768 6572 6520 6368 726f 6d65 2229 203d  where chrome") =
-00000310: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-00000320: 2020 2020 2020 7265 7475 726e 2022 6368        return "ch
-00000330: 726f 6d65 220d 0a20 2020 2020 2020 2020  rome"..         
-00000340: 2020 2070 6174 6820 3d20 6f73 2e70 6174     path = os.pat
-00000350: 682e 6a6f 696e 286f 732e 656e 7669 726f  h.join(os.enviro
-00000360: 6e5b 2250 524f 4752 414d 5736 3433 3222  n["PROGRAMW6432"
-00000370: 5d2c 2022 476f 6f67 6c65 5c5c 4368 726f  ], "Google\\Chro
-00000380: 6d65 5c5c 4170 706c 6963 6174 696f 6e5c  me\\Application\
-00000390: 5c63 6872 6f6d 652e 6578 6522 290d 0a20  \chrome.exe").. 
-000003a0: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
-000003b0: 2e70 6174 682e 6578 6973 7473 2870 6174  .path.exists(pat
-000003c0: 6829 3a0d 0a20 2020 2020 2020 2020 2020  h):..           
-000003d0: 2020 2020 2072 6574 7572 6e20 6627 227b       return f'"{
-000003e0: 7061 7468 7d22 270d 0a20 2020 2020 2020  path}"'..       
-000003f0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00000400: 0d0a 2020 2020 2020 2020 6966 206f 732e  ..        if os.
-00000410: 7379 7374 656d 2822 6368 726f 6d65 202d  system("chrome -
-00000420: 2d76 6572 7369 6f6e 2229 203d 3d20 303a  -version") == 0:
-00000430: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000440: 7475 726e 2022 6368 726f 6d65 220d 0a20  turn "chrome".. 
-00000450: 2020 2020 2020 2069 6620 706c 6174 666f         if platfo
-00000460: 726d 2e6d 6163 5f76 6572 2829 5b30 5d3a  rm.mac_ver()[0]:
-00000470: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000480: 7475 726e 2022 272f 4170 706c 6963 6174  turn "'/Applicat
-00000490: 696f 6e73 2f47 6f6f 676c 6520 4368 726f  ions/Google Chro
-000004a0: 6d65 2e61 7070 2f43 6f6e 7465 6e74 732f  me.app/Contents/
-000004b0: 4d61 634f 532f 476f 6f67 6c65 2043 6872  MacOS/Google Chr
-000004c0: 6f6d 6527 220d 0a20 2020 2020 2020 2065  ome'"..        e
-000004d0: 6c69 6620 706c 6174 666f 726d 2e6c 6962  lif platform.lib
-000004e0: 635f 7665 7228 295b 305d 3a0d 0a20 2020  c_ver()[0]:..   
-000004f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000500: 2267 6f6f 676c 652d 6368 726f 6d65 220d  "google-chrome".
-00000510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000520: 4e6f 6e65 0d0a 0d0a 2020 2020 6465 6620  None....    def 
-00000530: 6368 726f 6d69 756d 5f63 6f6d 6d61 6e64  chromium_command
-00000540: 2873 656c 6629 202d 3e20 7374 7220 7c20  (self) -> str | 
-00000550: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-00000560: 6620 706c 6174 666f 726d 2e77 696e 3332  f platform.win32
-00000570: 5f76 6572 2829 5b30 5d3a 0d0a 2020 2020  _ver()[0]:..    
-00000580: 2020 2020 2020 2020 6966 206f 732e 7379          if os.sy
-00000590: 7374 656d 2822 7768 6572 6520 6368 726f  stem("where chro
-000005a0: 6d69 756d 2229 203d 3d20 303a 0d0a 2020  mium") == 0:..  
-000005b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000005c0: 7475 726e 2022 6368 726f 6d69 756d 220d  turn "chromium".
-000005d0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-000005e0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-000005f0: 286f 732e 656e 7669 726f 6e5b 2250 524f  (os.environ["PRO
-00000600: 4752 414d 5736 3433 3222 5d2c 2022 4368  GRAMW6432"], "Ch
-00000610: 726f 6d69 756d 5c5c 4170 706c 6963 6174  romium\\Applicat
-00000620: 696f 6e5c 5c63 6872 6f6d 652e 6578 6522  ion\\chrome.exe"
-00000630: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00000640: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-00000650: 2870 6174 6829 3a0d 0a20 2020 2020 2020  (path):..       
-00000660: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000670: 6627 227b 7061 7468 7d22 270d 0a20 2020  f'"{path}"'..   
-00000680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000690: 4e6f 6e65 0d0a 2020 2020 2020 2020 6966  None..        if
-000006a0: 206f 732e 7379 7374 656d 2822 6368 726f   os.system("chro
-000006b0: 6d69 756d 202d 2d76 6572 7369 6f6e 2229  mium --version")
-000006c0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-000006d0: 2020 2020 7265 7475 726e 2022 6368 726f      return "chro
-000006e0: 6d69 756d 220d 0a20 2020 2020 2020 2069  mium"..        i
-000006f0: 6620 706c 6174 666f 726d 2e6d 6163 5f76  f platform.mac_v
-00000700: 6572 2829 5b30 5d3a 0d0a 2020 2020 2020  er()[0]:..      
-00000710: 2020 2020 2020 7061 7468 203d 2022 2f41        path = "/A
-00000720: 7070 6c69 6361 7469 6f6e 732f 4368 726f  pplications/Chro
-00000730: 6d69 756d 2e61 7070 2f43 6f6e 7465 6e74  mium.app/Content
-00000740: 732f 4d61 634f 532f 4368 726f 6d69 756d  s/MacOS/Chromium
-00000750: 220d 0a20 2020 2020 2020 2020 2020 2069  "..            i
-00000760: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-00000770: 2870 6174 6829 3a0d 0a20 2020 2020 2020  (path):..       
-00000780: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000790: 7061 7468 0d0a 2020 2020 2020 2020 656c  path..        el
-000007a0: 6966 2070 6c61 7466 6f72 6d2e 6c69 6263  if platform.libc
-000007b0: 5f76 6572 2829 5b30 5d3a 0d0a 2020 2020  _ver()[0]:..    
-000007c0: 2020 2020 2020 2020 6966 206f 732e 7379          if os.sy
-000007d0: 7374 656d 2822 6368 726f 6d69 756d 2d62  stem("chromium-b
-000007e0: 726f 7773 6572 202d 2d76 6572 7369 6f6e  rowser --version
-000007f0: 2229 203d 3d20 303a 0d0a 2020 2020 2020  ") == 0:..      
-00000800: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000810: 2022 6368 726f 6d69 756d 2d62 726f 7773   "chromium-brows
-00000820: 6572 220d 0a20 2020 2020 2020 2072 6574  er"..        ret
-00000830: 7572 6e20 4e6f 6e65 0d0a 0d0a 0d0a 2020  urn None......  
-00000840: 2020 6465 6620 636f 6d6d 616e 645f 7275    def command_ru
-00000850: 6e6e 6572 2873 656c 662c 2063 6872 6f6d  nner(self, chrom
-00000860: 653a 2073 7472 207c 204e 6f6e 652c 205f  e: str | None, _
-00000870: 746f 3a20 7374 722c 2074 656d 705f 6e61  to: str, temp_na
-00000880: 6d65 3a20 7374 7229 202d 3e20 696e 743a  me: str) -> int:
-00000890: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-000008a0: 2063 6872 6f6d 653a 0d0a 2020 2020 2020   chrome:..      
-000008b0: 2020 2020 2020 7265 7475 726e 2031 0d0a        return 1..
-000008c0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
-000008d0: 3d20 6627 7b63 6872 6f6d 657d 202d 2d68  = f'{chrome} --h
-000008e0: 6561 646c 6573 7320 2d2d 6469 7361 626c  eadless --disabl
-000008f0: 652d 6770 7520 2d2d 6469 7361 626c 652d  e-gpu --disable-
-00000900: 736f 6674 7761 7265 2d72 6173 7465 7269  software-rasteri
-00000910: 7a65 7220 2d2d 7072 696e 742d 746f 2d70  zer --print-to-p
-00000920: 6466 3d7b 5f74 6f7d 207b 7465 6d70 5f6e  df={_to} {temp_n
-00000930: 616d 657d 270d 0a20 2020 2020 2020 206c  ame}'..        l
-00000940: 6f67 6765 722e 6572 726f 7228 636f 6d6d  ogger.error(comm
-00000950: 616e 6429 0d0a 2020 2020 2020 2020 7265  and)..        re
-00000960: 7475 726e 206f 732e 7379 7374 656d 2863  turn os.system(c
-00000970: 6f6d 6d61 6e64 290d 0a0d 0a20 2020 2064  ommand)....    d
-00000980: 6566 2063 6f6e 7665 7274 2873 656c 662c  ef convert(self,
-00000990: 205f 6672 6f6d 3a20 7374 722c 205f 746f   _from: str, _to
-000009a0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0d  : str) -> bool:.
-000009b0: 0a20 2020 2020 2020 2022 2222 436f 6e76  .        """Conv
-000009c0: 6572 7473 2074 6865 2069 6d61 6765 2066  erts the image f
-000009d0: 726f 6d20 5356 4720 746f 2050 4446 2075  rom SVG to PDF u
-000009e0: 7369 6e67 2063 6872 6f6d 652e 2222 220d  sing chrome.""".
-000009f0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-00000a00: 656e 285f 6672 6f6d 2c20 2772 2729 2061  en(_from, 'r') a
-00000a10: 7320 663a 0d0a 2020 2020 2020 2020 2020  s f:..          
-00000a20: 2020 7376 6720 3d20 662e 7265 6164 2829    svg = f.read()
-00000a30: 0d0a 0d0a 2020 2020 2020 2020 4854 4d4c  ....        HTML
-00000a40: 203d 2022 3c68 746d 6c3e 3c68 6561 643e   = "<html><head>
-00000a50: 3c73 7479 6c65 3e62 6f64 7920 7b6d 6172  <style>body {mar
-00000a60: 6769 6e3a 2030 3b20 7d3c 2f73 7479 6c65  gin: 0; }</style
-00000a70: 3e3c 7363 7269 7074 3e66 756e 6374 696f  ><script>functio
-00000a80: 6e20 696e 6974 2829 207b 636f 6e73 7420  n init() {const 
-00000a90: 656c 656d 656e 7420 3d20 646f 6375 6d65  element = docume
-00000aa0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
-00000ab0: 2827 7376 6727 293b 636f 6e73 7420 706f  ('svg');const po
-00000ac0: 7369 7469 6f6e 496e 666f 203d 2065 6c65  sitionInfo = ele
-00000ad0: 6d65 6e74 2e67 6574 426f 756e 6469 6e67  ment.getBounding
-00000ae0: 436c 6965 6e74 5265 6374 2829 3b63 6f6e  ClientRect();con
-00000af0: 7374 2068 6569 6768 7420 3d20 706f 7369  st height = posi
-00000b00: 7469 6f6e 496e 666f 2e68 6569 6768 743b  tionInfo.height;
-00000b10: 636f 6e73 7420 7769 6474 6820 3d20 706f  const width = po
-00000b20: 7369 7469 6f6e 496e 666f 2e77 6964 7468  sitionInfo.width
-00000b30: 3b63 6f6e 7374 2073 7479 6c65 203d 2064  ;const style = d
-00000b40: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
-00000b50: 656d 656e 7428 2773 7479 6c65 2729 3b73  ement('style');s
-00000b60: 7479 6c65 2e69 6e6e 6572 4854 4d4c 203d  tyle.innerHTML =
-00000b70: 2060 4070 6167 6520 7b6d 6172 6769 6e3a   `@page {margin:
-00000b80: 2030 3b20 7369 7a65 3a20 247b 7769 6474   0; size: ${widt
-00000b90: 687d 7078 2024 7b68 6569 6768 747d 7078  h}px ${height}px
-00000ba0: 7d60 3b64 6f63 756d 656e 742e 6865 6164  }`;document.head
-00000bb0: 2e61 7070 656e 6443 6869 6c64 2873 7479  .appendChild(sty
-00000bc0: 6c65 293b 207d 7769 6e64 6f77 2e6f 6e6c  le); }window.onl
-00000bd0: 6f61 6420 3d20 696e 6974 3b3c 2f73 6372  oad = init;</scr
-00000be0: 6970 743e 3c2f 6865 6164 3e3c 626f 6479  ipt></head><body
-00000bf0: 3e25 733c 2f62 6f64 793e 3c2f 6874 6d6c  >%s</body></html
-00000c00: 3e22 2025 2028 7376 6729 0d0a 2020 2020  >" % (svg)..    
-00000c10: 2020 2020 7465 6d70 5f6e 616d 6520 3d20      temp_name = 
-00000c20: 6627 7b5f 6672 6f6d 7d2e 6874 6d6c 270d  f'{_from}.html'.
-00000c30: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-00000c40: 656e 2874 656d 705f 6e61 6d65 2c20 2777  en(temp_name, 'w
-00000c50: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
-00000c60: 2020 2020 2020 662e 7772 6974 6528 4854        f.write(HT
-00000c70: 4d4c 290d 0a0d 0a20 2020 2020 2020 2063  ML)....        c
-00000c80: 6872 6f6d 6975 6d20 3d20 7365 6c66 2e63  hromium = self.c
-00000c90: 6872 6f6d 6975 6d5f 636f 6d6d 616e 6428  hromium_command(
-00000ca0: 290d 0a20 2020 2020 2020 2063 6f64 6520  )..        code 
-00000cb0: 3d20 7365 6c66 2e63 6f6d 6d61 6e64 5f72  = self.command_r
-00000cc0: 756e 6e65 7228 6368 726f 6d69 756d 2c20  unner(chromium, 
-00000cd0: 5f74 6f2c 2074 656d 705f 6e61 6d65 290d  _to, temp_name).
-00000ce0: 0a20 2020 2020 2020 2069 6620 636f 6465  .        if code
-00000cf0: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
-00000d00: 2020 2020 6368 726f 6d65 203d 2073 656c      chrome = sel
-00000d10: 662e 6368 726f 6d65 5f63 6f6d 6d61 6e64  f.chrome_command
-00000d20: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000d30: 636f 6465 203d 2073 656c 662e 636f 6d6d  code = self.comm
-00000d40: 616e 645f 7275 6e6e 6572 2863 6872 6f6d  and_runner(chrom
-00000d50: 652c 205f 746f 2c20 7465 6d70 5f6e 616d  e, _to, temp_nam
-00000d60: 6529 0d0a 2020 2020 2020 2020 6966 2063  e)..        if c
-00000d70: 6f64 6520 213d 2030 3a0d 0a20 2020 2020  ode != 0:..     
-00000d80: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-00000d90: 726f 7228 2746 6169 6c20 746f 2063 6f6e  ror('Fail to con
-00000da0: 7665 7274 2073 7667 2074 6f20 7064 662e  vert svg to pdf.
-00000db0: 204d 616b 6520 7375 7265 2043 6872 6f6d   Make sure Chrom
-00000dc0: 6975 6d20 6f72 2043 6872 6f6d 6520 6973  ium or Chrome is
-00000dd0: 2069 6e73 7461 6c6c 6564 2e27 290d 0a20   installed.').. 
-00000de0: 2020 2020 2020 2020 2020 2065 7869 7428             exit(
-00000df0: 3129 0d0a 2020 2020 2020 2020 7265 7475  1)..        retu
-00000e00: 726e 2054 7275 650d 0a0d 0a0d 0a64 6566  rn True......def
-00000e10: 2073 6574 7570 2861 7070 3a20 5370 6869   setup(app: Sphi
-00000e20: 6e78 2920 2d3e 2064 6963 745b 7374 722c  nx) -> dict[str,
-00000e30: 2041 6e79 5d3a 0d0a 2020 2020 6170 702e   Any]:..    app.
-00000e40: 6164 645f 706f 7374 5f74 7261 6e73 666f  add_post_transfo
-00000e50: 726d 2843 6f6e 7665 7274 6572 290d 0a0d  rm(Converter)...
-00000e60: 0a20 2020 2072 6574 7572 6e20 7b0d 0a20  .    return {.. 
-00000e70: 2020 2020 2020 2027 7665 7273 696f 6e27         'version'
-00000e80: 3a20 2762 7569 6c74 696e 272c 0d0a 2020  : 'builtin',..  
-00000e90: 2020 2020 2020 2770 6172 616c 6c65 6c5f        'parallel_
-00000ea0: 7265 6164 5f73 6166 6527 3a20 5472 7565  read_safe': True
-00000eb0: 2c0d 0a20 2020 2020 2020 2027 7061 7261  ,..        'para
-00000ec0: 6c6c 656c 5f77 7269 7465 5f73 6166 6527  llel_write_safe'
-00000ed0: 3a20 5472 7565 2c0d 0a20 2020 207d       : True,..    }
+00000020: 6e73 0a22 2222 0a20 2020 2043 6f6e 7665  ns.""".    Conve
+00000030: 7274 7320 5356 4720 696d 6167 6573 2074  rts SVG images t
+00000040: 6f20 5044 4620 7573 696e 6720 6368 726f  o PDF using chro
+00000050: 6d65 2069 6e20 6361 7365 2074 6865 2062  me in case the b
+00000060: 7569 6c64 6572 2064 6f65 7320 6e6f 740a  uilder does not.
+00000070: 2020 2020 7375 7070 6f72 7420 5356 4720      support SVG 
+00000080: 696d 6167 6573 206e 6174 6976 656c 7920  images natively 
+00000090: 2865 2e67 2e20 4c61 5465 5829 2e0a 0a22  (e.g. LaTeX)..."
+000000a0: 2222 0a0a 6672 6f6d 2073 7068 696e 782e  ""..from sphinx.
+000000b0: 7472 616e 7366 6f72 6d73 2e70 6f73 745f  transforms.post_
+000000c0: 7472 616e 7366 6f72 6d73 2e69 6d61 6765  transforms.image
+000000d0: 7320 696d 706f 7274 2049 6d61 6765 436f  s import ImageCo
+000000e0: 6e76 6572 7465 720a 6672 6f6d 2073 7068  nverter.from sph
+000000f0: 696e 782e 7574 696c 2069 6d70 6f72 7420  inx.util import 
+00000100: 6c6f 6767 696e 670a 696d 706f 7274 206f  logging.import o
+00000110: 730a 696d 706f 7274 2070 6c61 7466 6f72  s.import platfor
+00000120: 6d0a 6672 6f6d 2074 7970 696e 6720 696d  m.from typing im
+00000130: 706f 7274 2041 6e79 2020 2320 4e4f 5141  port Any  # NOQA
+00000140: 0a66 726f 6d20 7370 6869 6e78 2e61 7070  .from sphinx.app
+00000150: 6c69 6361 7469 6f6e 2069 6d70 6f72 7420  lication import 
+00000160: 5370 6869 6e78 2020 2320 4e4f 5141 0a0a  Sphinx  # NOQA..
+00000170: 0a6c 6f67 6765 7220 3d20 6c6f 6767 696e  .logger = loggin
+00000180: 672e 6765 744c 6f67 6765 7228 5f5f 6e61  g.getLogger(__na
+00000190: 6d65 5f5f 290a 0a0a 636c 6173 7320 436f  me__)...class Co
+000001a0: 6e76 6572 7465 7228 496d 6167 6543 6f6e  nverter(ImageCon
+000001b0: 7665 7274 6572 293a 0a20 2020 2063 6f6e  verter):.    con
+000001c0: 7665 7273 696f 6e5f 7275 6c65 7320 3d20  version_rules = 
+000001d0: 5b0a 2020 2020 2020 2020 2827 696d 6167  [.        ('imag
+000001e0: 652f 7376 672b 786d 6c27 2c20 2761 7070  e/svg+xml', 'app
+000001f0: 6c69 6361 7469 6f6e 2f70 6466 2729 2c0a  lication/pdf'),.
+00000200: 2020 2020 5d0a 0a20 2020 2064 6566 2069      ]..    def i
+00000210: 735f 6176 6169 6c61 626c 6528 7365 6c66  s_available(self
+00000220: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00000230: 2020 2022 2222 436f 6e66 6972 6d73 2069     """Confirms i
+00000240: 6620 636f 6e76 6572 7465 7220 6973 2061  f converter is a
+00000250: 7661 696c 6162 6c65 206f 7220 6e6f 742e  vailable or not.
+00000260: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00000270: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+00000280: 2063 6872 6f6d 655f 636f 6d6d 616e 6428   chrome_command(
+00000290: 7365 6c66 2920 2d3e 2073 7472 207c 204e  self) -> str | N
+000002a0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+000002b0: 706c 6174 666f 726d 2e77 696e 3332 5f76  platform.win32_v
+000002c0: 6572 2829 5b30 5d3a 0a20 2020 2020 2020  er()[0]:.       
+000002d0: 2020 2020 2069 6620 6f73 2e73 7973 7465       if os.syste
+000002e0: 6d28 2277 6865 7265 2063 6872 6f6d 6522  m("where chrome"
+000002f0: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+00000300: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+00000310: 6368 726f 6d65 220a 2020 2020 2020 2020  chrome".        
+00000320: 2020 2020 7061 7468 203d 206f 732e 7061      path = os.pa
+00000330: 7468 2e6a 6f69 6e28 6f73 2e65 6e76 6972  th.join(os.envir
+00000340: 6f6e 5b22 5052 4f47 5241 4d57 3634 3332  on["PROGRAMW6432
+00000350: 225d 2c20 2247 6f6f 676c 655c 5c43 6872  "], "Google\\Chr
+00000360: 6f6d 655c 5c41 7070 6c69 6361 7469 6f6e  ome\\Application
+00000370: 5c5c 6368 726f 6d65 2e65 7865 2229 0a20  \\chrome.exe"). 
+00000380: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00000390: 2e70 6174 682e 6578 6973 7473 2870 6174  .path.exists(pat
+000003a0: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+000003b0: 2020 2020 7265 7475 726e 2066 2722 7b70      return f'"{p
+000003c0: 6174 687d 2227 0a20 2020 2020 2020 2020  ath}"'.         
+000003d0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+000003e0: 2020 2020 2020 2069 6620 6f73 2e73 7973         if os.sys
+000003f0: 7465 6d28 2263 6872 6f6d 6520 2d2d 7665  tem("chrome --ve
+00000400: 7273 696f 6e22 2920 3d3d 2030 3a0a 2020  rsion") == 0:.  
+00000410: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000420: 2022 6368 726f 6d65 220a 2020 2020 2020   "chrome".      
+00000430: 2020 6966 2070 6c61 7466 6f72 6d2e 6d61    if platform.ma
+00000440: 635f 7665 7228 295b 305d 3a0a 2020 2020  c_ver()[0]:.    
+00000450: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+00000460: 272f 4170 706c 6963 6174 696f 6e73 2f47  '/Applications/G
+00000470: 6f6f 676c 6520 4368 726f 6d65 2e61 7070  oogle Chrome.app
+00000480: 2f43 6f6e 7465 6e74 732f 4d61 634f 532f  /Contents/MacOS/
+00000490: 476f 6f67 6c65 2043 6872 6f6d 6527 220a  Google Chrome'".
+000004a0: 2020 2020 2020 2020 656c 6966 2070 6c61          elif pla
+000004b0: 7466 6f72 6d2e 6c69 6263 5f76 6572 2829  tform.libc_ver()
+000004c0: 5b30 5d3a 0a20 2020 2020 2020 2020 2020  [0]:.           
+000004d0: 2072 6574 7572 6e20 2267 6f6f 676c 652d   return "google-
+000004e0: 6368 726f 6d65 220a 2020 2020 2020 2020  chrome".        
+000004f0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00000500: 2064 6566 2063 6872 6f6d 6975 6d5f 636f   def chromium_co
+00000510: 6d6d 616e 6428 7365 6c66 2920 2d3e 2073  mmand(self) -> s
+00000520: 7472 207c 204e 6f6e 653a 0a20 2020 2020  tr | None:.     
+00000530: 2020 2069 6620 706c 6174 666f 726d 2e77     if platform.w
+00000540: 696e 3332 5f76 6572 2829 5b30 5d3a 0a20  in32_ver()[0]:. 
+00000550: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00000560: 2e73 7973 7465 6d28 2277 6865 7265 2063  .system("where c
+00000570: 6872 6f6d 6975 6d22 2920 3d3d 2030 3a0a  hromium") == 0:.
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 7265 7475 726e 2022 6368 726f 6d69 756d  return "chromium
+000005a0: 220a 2020 2020 2020 2020 2020 2020 7061  ".            pa
+000005b0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+000005c0: 6e28 6f73 2e65 6e76 6972 6f6e 5b22 5052  n(os.environ["PR
+000005d0: 4f47 5241 4d57 3634 3332 225d 2c20 2243  OGRAMW6432"], "C
+000005e0: 6872 6f6d 6975 6d5c 5c41 7070 6c69 6361  hromium\\Applica
+000005f0: 7469 6f6e 5c5c 6368 726f 6d65 2e65 7865  tion\\chrome.exe
+00000600: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00000610: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+00000620: 2870 6174 6829 3a0a 2020 2020 2020 2020  (path):.        
+00000630: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000640: 2722 7b70 6174 687d 2227 0a20 2020 2020  '"{path}"'.     
+00000650: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00000660: 6e65 0a20 2020 2020 2020 2069 6620 6f73  ne.        if os
+00000670: 2e73 7973 7465 6d28 2263 6872 6f6d 6975  .system("chromiu
+00000680: 6d20 2d2d 7665 7273 696f 6e22 2920 3d3d  m --version") ==
+00000690: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+000006a0: 7265 7475 726e 2022 6368 726f 6d69 756d  return "chromium
+000006b0: 220a 2020 2020 2020 2020 6966 2070 6c61  ".        if pla
+000006c0: 7466 6f72 6d2e 6d61 635f 7665 7228 295b  tform.mac_ver()[
+000006d0: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+000006e0: 7061 7468 203d 2022 2f41 7070 6c69 6361  path = "/Applica
+000006f0: 7469 6f6e 732f 4368 726f 6d69 756d 2e61  tions/Chromium.a
+00000700: 7070 2f43 6f6e 7465 6e74 732f 4d61 634f  pp/Contents/MacO
+00000710: 532f 4368 726f 6d69 756d 220a 2020 2020  S/Chromium".    
+00000720: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00000730: 7468 2e65 7869 7374 7328 7061 7468 293a  th.exists(path):
+00000740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000750: 2072 6574 7572 6e20 7061 7468 0a20 2020   return path.   
+00000760: 2020 2020 2065 6c69 6620 706c 6174 666f       elif platfo
+00000770: 726d 2e6c 6962 635f 7665 7228 295b 305d  rm.libc_ver()[0]
+00000780: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00000790: 206f 732e 7379 7374 656d 2822 6368 726f   os.system("chro
+000007a0: 6d69 756d 2d62 726f 7773 6572 202d 2d76  mium-browser --v
+000007b0: 6572 7369 6f6e 2229 203d 3d20 303a 0a20  ersion") == 0:. 
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000007d0: 6574 7572 6e20 2263 6872 6f6d 6975 6d2d  eturn "chromium-
+000007e0: 6272 6f77 7365 7222 0a20 2020 2020 2020  browser".       
+000007f0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 0a20   return None... 
+00000800: 2020 2064 6566 2063 6f6d 6d61 6e64 5f72     def command_r
+00000810: 756e 6e65 7228 7365 6c66 2c20 6368 726f  unner(self, chro
+00000820: 6d65 3a20 7374 7220 7c20 4e6f 6e65 2c20  me: str | None, 
+00000830: 5f74 6f3a 2073 7472 2c20 7465 6d70 5f6e  _to: str, temp_n
+00000840: 616d 653a 2073 7472 2920 2d3e 2069 6e74  ame: str) -> int
+00000850: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00000860: 2063 6872 6f6d 653a 0a20 2020 2020 2020   chrome:.       
+00000870: 2020 2020 2072 6574 7572 6e20 310a 2020       return 1.  
+00000880: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
+00000890: 6627 7b63 6872 6f6d 657d 202d 2d68 6561  f'{chrome} --hea
+000008a0: 646c 6573 7320 2d2d 6469 7361 626c 652d  dless --disable-
+000008b0: 6770 7520 2d2d 6469 7361 626c 652d 736f  gpu --disable-so
+000008c0: 6674 7761 7265 2d72 6173 7465 7269 7a65  ftware-rasterize
+000008d0: 7220 2d2d 7072 696e 742d 746f 2d70 6466  r --print-to-pdf
+000008e0: 3d7b 5f74 6f7d 207b 7465 6d70 5f6e 616d  ={_to} {temp_nam
+000008f0: 657d 270a 2020 2020 2020 2020 6c6f 6767  e}'.        logg
+00000900: 6572 2e65 7272 6f72 2863 6f6d 6d61 6e64  er.error(command
+00000910: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00000920: 206f 732e 7379 7374 656d 2863 6f6d 6d61   os.system(comma
+00000930: 6e64 290a 0a20 2020 2064 6566 2063 6f6e  nd)..    def con
+00000940: 7665 7274 2873 656c 662c 205f 6672 6f6d  vert(self, _from
+00000950: 3a20 7374 722c 205f 746f 3a20 7374 7229  : str, _to: str)
+00000960: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00000970: 2020 2222 2243 6f6e 7665 7274 7320 7468    """Converts th
+00000980: 6520 696d 6167 6520 6672 6f6d 2053 5647  e image from SVG
+00000990: 2074 6f20 5044 4620 7573 696e 6720 6368   to PDF using ch
+000009a0: 726f 6d65 2e22 2222 0a20 2020 2020 2020  rome.""".       
+000009b0: 2077 6974 6820 6f70 656e 285f 6672 6f6d   with open(_from
+000009c0: 2c20 2772 2729 2061 7320 663a 0a20 2020  , 'r') as f:.   
+000009d0: 2020 2020 2020 2020 2073 7667 203d 2066           svg = f
+000009e0: 2e72 6561 6428 290a 0a20 2020 2020 2020  .read()..       
+000009f0: 2048 544d 4c20 3d20 223c 6874 6d6c 3e3c   HTML = "<html><
+00000a00: 6865 6164 3e3c 7374 796c 653e 626f 6479  head><style>body
+00000a10: 207b 6d61 7267 696e 3a20 303b 207d 3c2f   {margin: 0; }</
+00000a20: 7374 796c 653e 3c73 6372 6970 743e 6675  style><script>fu
+00000a30: 6e63 7469 6f6e 2069 6e69 7428 2920 7b63  nction init() {c
+00000a40: 6f6e 7374 2065 6c65 6d65 6e74 203d 2064  onst element = d
+00000a50: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
+00000a60: 6563 746f 7228 2773 7667 2729 3b63 6f6e  ector('svg');con
+00000a70: 7374 2070 6f73 6974 696f 6e49 6e66 6f20  st positionInfo 
+00000a80: 3d20 656c 656d 656e 742e 6765 7442 6f75  = element.getBou
+00000a90: 6e64 696e 6743 6c69 656e 7452 6563 7428  ndingClientRect(
+00000aa0: 293b 636f 6e73 7420 6865 6967 6874 203d  );const height =
+00000ab0: 2070 6f73 6974 696f 6e49 6e66 6f2e 6865   positionInfo.he
+00000ac0: 6967 6874 3b63 6f6e 7374 2077 6964 7468  ight;const width
+00000ad0: 203d 2070 6f73 6974 696f 6e49 6e66 6f2e   = positionInfo.
+00000ae0: 7769 6474 683b 636f 6e73 7420 7374 796c  width;const styl
+00000af0: 6520 3d20 646f 6375 6d65 6e74 2e63 7265  e = document.cre
+00000b00: 6174 6545 6c65 6d65 6e74 2827 7374 796c  ateElement('styl
+00000b10: 6527 293b 7374 796c 652e 696e 6e65 7248  e');style.innerH
+00000b20: 544d 4c20 3d20 6040 7061 6765 207b 6d61  TML = `@page {ma
+00000b30: 7267 696e 3a20 303b 2073 697a 653a 2024  rgin: 0; size: $
+00000b40: 7b77 6964 7468 7d70 7820 247b 6865 6967  {width}px ${heig
+00000b50: 6874 7d70 787d 603b 646f 6375 6d65 6e74  ht}px}`;document
+00000b60: 2e68 6561 642e 6170 7065 6e64 4368 696c  .head.appendChil
+00000b70: 6428 7374 796c 6529 3b20 7d77 696e 646f  d(style); }windo
+00000b80: 772e 6f6e 6c6f 6164 203d 2069 6e69 743b  w.onload = init;
+00000b90: 3c2f 7363 7269 7074 3e3c 2f68 6561 643e  </script></head>
+00000ba0: 3c62 6f64 793e 2573 3c2f 626f 6479 3e3c  <body>%s</body><
+00000bb0: 2f68 746d 6c3e 2220 2520 2873 7667 290a  /html>" % (svg).
+00000bc0: 2020 2020 2020 2020 7465 6d70 5f6e 616d          temp_nam
+00000bd0: 6520 3d20 6627 7b5f 6672 6f6d 7d2e 6874  e = f'{_from}.ht
+00000be0: 6d6c 270a 2020 2020 2020 2020 7769 7468  ml'.        with
+00000bf0: 206f 7065 6e28 7465 6d70 5f6e 616d 652c   open(temp_name,
+00000c00: 2027 7727 2920 6173 2066 3a0a 2020 2020   'w') as f:.    
+00000c10: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00000c20: 4854 4d4c 290a 0a20 2020 2020 2020 2063  HTML)..        c
+00000c30: 6872 6f6d 6975 6d20 3d20 7365 6c66 2e63  hromium = self.c
+00000c40: 6872 6f6d 6975 6d5f 636f 6d6d 616e 6428  hromium_command(
+00000c50: 290a 2020 2020 2020 2020 636f 6465 203d  ).        code =
+00000c60: 2073 656c 662e 636f 6d6d 616e 645f 7275   self.command_ru
+00000c70: 6e6e 6572 2863 6872 6f6d 6975 6d2c 205f  nner(chromium, _
+00000c80: 746f 2c20 7465 6d70 5f6e 616d 6529 0a20  to, temp_name). 
+00000c90: 2020 2020 2020 2069 6620 636f 6465 2021         if code !
+00000ca0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00000cb0: 2063 6872 6f6d 6520 3d20 7365 6c66 2e63   chrome = self.c
+00000cc0: 6872 6f6d 655f 636f 6d6d 616e 6428 290a  hrome_command().
+00000cd0: 2020 2020 2020 2020 2020 2020 636f 6465              code
+00000ce0: 203d 2073 656c 662e 636f 6d6d 616e 645f   = self.command_
+00000cf0: 7275 6e6e 6572 2863 6872 6f6d 652c 205f  runner(chrome, _
+00000d00: 746f 2c20 7465 6d70 5f6e 616d 6529 0a20  to, temp_name). 
+00000d10: 2020 2020 2020 2069 6620 636f 6465 2021         if code !
+00000d20: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00000d30: 206c 6f67 6765 722e 6572 726f 7228 2746   logger.error('F
+00000d40: 6169 6c20 746f 2063 6f6e 7665 7274 2073  ail to convert s
+00000d50: 7667 2074 6f20 7064 662e 204d 616b 6520  vg to pdf. Make 
+00000d60: 7375 7265 2043 6872 6f6d 6975 6d20 6f72  sure Chromium or
+00000d70: 2043 6872 6f6d 6520 6973 2069 6e73 7461   Chrome is insta
+00000d80: 6c6c 6564 2e27 290a 2020 2020 2020 2020  lled.').        
+00000d90: 2020 2020 6578 6974 2831 290a 2020 2020      exit(1).    
+00000da0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00000db0: 0a0a 6465 6620 7365 7475 7028 6170 703a  ..def setup(app:
+00000dc0: 2053 7068 696e 7829 202d 3e20 6469 6374   Sphinx) -> dict
+00000dd0: 5b73 7472 2c20 416e 795d 3a0a 2020 2020  [str, Any]:.    
+00000de0: 6170 702e 6164 645f 706f 7374 5f74 7261  app.add_post_tra
+00000df0: 6e73 666f 726d 2843 6f6e 7665 7274 6572  nsform(Converter
+00000e00: 290a 0a20 2020 2072 6574 7572 6e20 7b0a  )..    return {.
+00000e10: 2020 2020 2020 2020 2776 6572 7369 6f6e          'version
+00000e20: 273a 2027 6275 696c 7469 6e27 2c0a 2020  ': 'builtin',.  
+00000e30: 2020 2020 2020 2770 6172 616c 6c65 6c5f        'parallel_
+00000e40: 7265 6164 5f73 6166 6527 3a20 5472 7565  read_safe': True
+00000e50: 2c0a 2020 2020 2020 2020 2770 6172 616c  ,.        'paral
+00000e60: 6c65 6c5f 7772 6974 655f 7361 6665 273a  lel_write_safe':
+00000e70: 2054 7275 652c 0a20 2020 207d             True,.    }
```

### Comparing `solverz-0.0.1rc1/docs/ext/docscrape.py` & `solverz-0.0.1rc2/docs/ext/docscrape.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,555 +1,555 @@
-"""
-Extract reference documentation from the NumPy source tree.
-"""
-
-import inspect
-import textwrap
-import re
-import pydoc
-from collections.abc import Mapping
-import sys
-
-
-class Reader:
-    """
-    A line-based string reader.
-    """
-    def __init__(self, data):
-        """
-        Parameters
-        ----------
-        data : str
-           String with lines separated by '\n'.
-
-        """
-        if isinstance(data, list):
-            self._str = data
-        else:
-            self._str = data.split('\n')  # store string as list of lines
-
-        self.reset()
-
-    def __getitem__(self, n):
-        return self._str[n]
-
-    def reset(self):
-        self._l = 0  # current line nr
-
-    def read(self):
-        if not self.eof():
-            out = self[self._l]
-            self._l += 1
-            return out
-        else:
-            return ''
-
-    def seek_next_non_empty_line(self):
-        for l in self[self._l:]:
-            if l.strip():
-                break
-            else:
-                self._l += 1
-
-    def eof(self):
-        return self._l >= len(self._str)
-
-    def read_to_condition(self, condition_func):
-        start = self._l
-        for line in self[start:]:
-            if condition_func(line):
-                return self[start:self._l]
-            self._l += 1
-            if self.eof():
-                return self[start:self._l + 1]
-        return []
-
-    def read_to_next_empty_line(self):
-        self.seek_next_non_empty_line()
-
-        def is_empty(line):
-            return not line.strip()
-
-        return self.read_to_condition(is_empty)
-
-    def read_to_next_unindented_line(self):
-        def is_unindented(line):
-            return (line.strip() and (len(line.lstrip()) == len(line)))
-        return self.read_to_condition(is_unindented)
-
-    def peek(self, n=0):
-        if self._l + n < len(self._str):
-            return self[self._l + n]
-        else:
-            return ''
-
-    def is_empty(self):
-        return not ''.join(self._str).strip()
-
-
-class NumpyDocString(Mapping):
-    def __init__(self, docstring, config={}):
-        docstring = textwrap.dedent(docstring).split('\n')
-
-        self._doc = Reader(docstring)
-        self._parsed_data = {
-            'Signature': '',
-            'Summary': [''],
-            'Extended Summary': [],
-            'Parameters': [],
-            'Returns': [],
-            'Yields': [],
-            'Raises': [],
-            'Warns': [],
-            'Other Parameters': [],
-            'Attributes': [],
-            'Methods': [],
-            'See Also': [],
-            # 'Notes': [],
-            'Warnings': [],
-            'References': '',
-            # 'Examples': '',
-            'index': {}
-        }
-        self._other_keys = []
-
-        self._parse()
-
-    def __getitem__(self, key):
-        return self._parsed_data[key]
-
-    def __setitem__(self, key, val):
-        if key not in self._parsed_data:
-            self._other_keys.append(key)
-
-        self._parsed_data[key] = val
-
-    def __iter__(self):
-        return iter(self._parsed_data)
-
-    def __len__(self):
-        return len(self._parsed_data)
-
-    def _is_at_section(self):
-        self._doc.seek_next_non_empty_line()
-
-        if self._doc.eof():
-            return False
-
-        l1 = self._doc.peek().strip()  # e.g. Parameters
-
-        if l1.startswith('.. index::'):
-            return True
-
-        l2 = self._doc.peek(1).strip()  # ---------- or ==========
-        return l2.startswith(('-' * len(l1), '=' * len(l1)))
-
-    def _strip(self, doc):
-        i = 0
-        j = 0
-        for i, line in enumerate(doc):
-            if line.strip():
-                break
-
-        for j, line in enumerate(doc[::-1]):
-            if line.strip():
-                break
-
-        return doc[i:len(doc) - j]
-
-    def _read_to_next_section(self):
-        section = self._doc.read_to_next_empty_line()
-
-        while not self._is_at_section() and not self._doc.eof():
-            if not self._doc.peek(-1).strip():  # previous line was empty
-                section += ['']
-
-            section += self._doc.read_to_next_empty_line()
-
-        return section
-
-    def _read_sections(self):
-        while not self._doc.eof():
-            data = self._read_to_next_section()
-            name = data[0].strip()
-
-            if name.startswith('..'):  # index section
-                yield name, data[1:]
-            elif len(data) < 2:
-                yield StopIteration
-            else:
-                yield name, self._strip(data[2:])
-
-    def _parse_param_list(self, content):
-        r = Reader(content)
-        params = []
-        while not r.eof():
-            header = r.read().strip()
-            if ' : ' in header:
-                arg_name, arg_type = header.split(' : ')[:2]
-            else:
-                arg_name, arg_type = header, ''
-
-            desc = r.read_to_next_unindented_line()
-            desc = dedent_lines(desc)
-
-            params.append((arg_name, arg_type, desc))
-
-        return params
-
-    _name_rgx = re.compile(r"^\s*(:(?P<role>\w+):`(?P<name>[a-zA-Z0-9_.-]+)`|"
-                           r" (?P<name2>[a-zA-Z0-9_.-]+))\s*", re.X)
-
-    def _parse_see_also(self, content):
-        """
-        func_name : Descriptive text
-            continued text
-        another_func_name : Descriptive text
-        func_name1, func_name2, :meth:`func_name`, func_name3
-
-        """
-        items = []
-
-        def parse_item_name(text):
-            """Match ':role:`name`' or 'name'"""
-            m = self._name_rgx.match(text)
-            if m:
-                g = m.groups()
-                if g[1] is None:
-                    return g[3], None
-                else:
-                    return g[2], g[1]
-            raise ValueError("%s is not an item name" % text)
-
-        def push_item(name, rest):
-            if not name:
-                return
-            name, role = parse_item_name(name)
-            if '.' not in name:
-                name = '~.' + name
-            items.append((name, list(rest), role))
-            del rest[:]
-
-        current_func = None
-        rest = []
-
-        for line in content:
-            if not line.strip():
-                continue
-
-            m = self._name_rgx.match(line)
-            if m and line[m.end():].strip().startswith(':'):
-                push_item(current_func, rest)
-                current_func, line = line[:m.end()], line[m.end():]
-                rest = [line.split(':', 1)[1].strip()]
-                if not rest[0]:
-                    rest = []
-            elif not line.startswith(' '):
-                push_item(current_func, rest)
-                current_func = None
-                if ',' in line:
-                    for func in line.split(','):
-                        if func.strip():
-                            push_item(func, [])
-                elif line.strip():
-                    current_func = line
-            elif current_func is not None:
-                rest.append(line.strip())
-        push_item(current_func, rest)
-        return items
-
-    def _parse_index(self, section, content):
-        """
-        .. index: default
-           :refguide: something, else, and more
-
-        """
-        def strip_each_in(lst):
-            return [s.strip() for s in lst]
-
-        out = {}
-        section = section.split('::')
-        if len(section) > 1:
-            out['default'] = strip_each_in(section[1].split(','))[0]
-        for line in content:
-            line = line.split(':')
-            if len(line) > 2:
-                out[line[1]] = strip_each_in(line[2].split(','))
-        return out
-
-    def _parse_summary(self):
-        """Grab signature (if given) and summary"""
-        if self._is_at_section():
-            return
-
-        # If several signatures present, take the last one
-        while True:
-            summary = self._doc.read_to_next_empty_line()
-            summary_str = " ".join([s.strip() for s in summary]).strip()
-            if re.compile(r'^([\w., ]+=)?\s*[\w\.]+\(.*\)$').match(summary_str):
-                self['Signature'] = summary_str
-                if not self._is_at_section():
-                    continue
-            break
-
-        if summary is not None:
-            self['Summary'] = summary
-
-        if not self._is_at_section():
-            self['Extended Summary'] = self._read_to_next_section()
-
-    def _parse(self):
-        self._doc.reset()
-        self._parse_summary()
-
-        sections = list(self._read_sections())
-        section_names = {section for section, content in sections}
-
-        has_returns = 'Returns' in section_names
-        has_yields = 'Yields' in section_names
-        # We could do more tests, but we are not. Arbitrarily.
-        if has_returns and has_yields:
-            msg = 'Docstring contains both a Returns and Yields section.'
-            raise ValueError(msg)
-
-        for (section, content) in sections:
-            if not section.startswith('..'):
-                section = (s.capitalize() for s in section.split(' '))
-                section = ' '.join(section)
-            if section in ('Parameters', 'Returns', 'Yields', 'Raises',
-                           'Warns', 'Other Parameters', 'Attributes',
-                           'Methods'):
-                self[section] = self._parse_param_list(content)
-            elif section.startswith('.. index::'):
-                self['index'] = self._parse_index(section, content)
-            elif section == 'See Also':
-                self['See Also'] = self._parse_see_also(content)
-            else:
-                self[section] = content
-
-    # string conversion routines
-
-    def _str_header(self, name, symbol='-'):
-        return [name, len(name)*symbol]
-
-    def _str_indent(self, doc, indent=4):
-        out = []
-        for line in doc:
-            out += [' '*indent + line]
-        return out
-
-    def _str_signature(self):
-        if self['Signature']:
-            return [self['Signature'].replace('*', r'\*')] + ['']
-        else:
-            return ['']
-
-    def _str_summary(self):
-        if self['Summary']:
-            return self['Summary'] + ['']
-        else:
-            return []
-
-    def _str_extended_summary(self):
-        if self['Extended Summary']:
-            return self['Extended Summary'] + ['']
-        else:
-            return []
-
-    def _str_param_list(self, name):
-        out = []
-        if self[name]:
-            out += self._str_header(name)
-            for param, param_type, desc in self[name]:
-                if param_type:
-                    out += ['{} : {}'.format(param, param_type)]
-                else:
-                    out += [param]
-                out += self._str_indent(desc)
-            out += ['']
-        return out
-
-    def _str_section(self, name):
-        out = []
-        if self[name]:
-            out += self._str_header(name)
-            out += self[name]
-            out += ['']
-        return out
-
-    def _str_see_also(self, func_role):
-        if not self['See Also']:
-            return []
-        out = []
-        out += self._str_header("See Also")
-        last_had_desc = True
-        for func, desc, role in self['See Also']:
-            if role:
-                link = ':{}:`{}`'.format(role, func)
-            elif func_role:
-                link = ':{}:`{}`'.format(func_role, func)
-            else:
-                link = "`%s`_" % func
-            if desc or last_had_desc:
-                out += ['']
-                out += [link]
-            else:
-                out[-1] += ", %s" % link
-            if desc:
-                out += self._str_indent([' '.join(desc)])
-                last_had_desc = True
-            else:
-                last_had_desc = False
-        out += ['']
-        return out
-
-    def _str_index(self):
-        idx = self['index']
-        out = []
-        out += ['.. index:: %s' % idx.get('default', '')]
-        for section, references in idx.items():
-            if section == 'default':
-                continue
-            out += ['   :{}: {}'.format(section, ', '.join(references))]
-        return out
-
-    def __str__(self, func_role=''):
-        out = []
-        out += self._str_signature()
-        out += self._str_summary()
-        out += self._str_extended_summary()
-        for param_list in ('Parameters', 'Returns', 'Yields',
-                           'Other Parameters', 'Raises', 'Warns'):
-            out += self._str_param_list(param_list)
-        out += self._str_section('Warnings')
-        out += self._str_see_also(func_role)
-        for s in ('Notes', 'References', 'Examples'):
-            out += self._str_section(s)
-        for param_list in ('Attributes', 'Methods'):
-            out += self._str_param_list(param_list)
-        out += self._str_index()
-        return '\n'.join(out)
-
-
-def indent(str, indent=4):
-    indent_str = ' '*indent
-    if str is None:
-        return indent_str
-    lines = str.split('\n')
-    return '\n'.join(indent_str + l for l in lines)
-
-
-def dedent_lines(lines):
-    """Deindent a list of lines maximally"""
-    return textwrap.dedent("\n".join(lines)).split("\n")
-
-
-def header(text, style='-'):
-    return text + '\n' + style*len(text) + '\n'
-
-
-class FunctionDoc(NumpyDocString):
-    def __init__(self, func, role='func', doc=None, config={}):
-        self._f = func
-        self._role = role  # e.g. "func" or "meth"
-
-        if doc is None:
-            if func is None:
-                raise ValueError("No function or docstring given")
-            doc = inspect.getdoc(func) or ''
-        NumpyDocString.__init__(self, doc)
-
-        if not self['Signature'] and func is not None:
-            func, func_name = self.get_func()
-            try:
-                # try to read signature
-                argspec = str(inspect.signature(func))
-                argspec = argspec.replace('*', r'\*')
-                signature = '{}{}'.format(func_name, argspec)
-            except TypeError as e:
-                signature = '%s()' % func_name
-            self['Signature'] = signature
-
-    def get_func(self):
-        func_name = getattr(self._f, '__name__', self.__class__.__name__)
-        if inspect.isclass(self._f):
-            func = getattr(self._f, '__call__', self._f.__init__)
-        else:
-            func = self._f
-        return func, func_name
-
-    def __str__(self):
-        out = ''
-
-        func, func_name = self.get_func()
-        signature = self['Signature'].replace('*', r'\*')
-
-        roles = {'func': 'function',
-                 'meth': 'method'}
-
-        if self._role:
-            if self._role not in roles:
-                print("Warning: invalid role %s" % self._role)
-            out += '.. {}:: {}\n    \n\n'.format(roles.get(self._role, ''),
-                                             func_name)
-
-        out += super().__str__(func_role=self._role)
-        return out
-
-
-class ClassDoc(NumpyDocString):
-
-    extra_public_methods = ['__call__']
-
-    def __init__(self, cls, doc=None, modulename='', func_doc=FunctionDoc,
-                 config={}):
-        if not inspect.isclass(cls) and cls is not None:
-            raise ValueError("Expected a class or None, but got %r" % cls)
-        self._cls = cls
-
-        self.show_inherited_members = config.get(
-                    'show_inherited_class_members', True)
-
-        if modulename and not modulename.endswith('.'):
-            modulename += '.'
-        self._mod = modulename
-
-        if doc is None:
-            if cls is None:
-                raise ValueError("No class or documentation string given")
-            doc = pydoc.getdoc(cls)
-
-        NumpyDocString.__init__(self, doc)
-
-        if config.get('show_class_members', True):
-            def splitlines_x(s):
-                if not s:
-                    return []
-                else:
-                    return s.splitlines()
-
-            for field, items in [('Methods', self.methods),
-                                 ('Attributes', self.properties)]:
-                if not self[field]:
-                    doc_list = []
-                    for name in sorted(items):
-                        clsname = getattr(self._cls, name, None)
-                        if clsname is not None:
-                            doc_item = pydoc.getdoc(clsname)
-                            doc_list.append((name, '', splitlines_x(doc_item)))
-                    self[field] = doc_list
-
-    @property
-    def methods(self):
-        if self._cls is None:
-            return []
-        return [name for name, func in inspect.getmembers(self._cls)
-                if ((not name.startswith('_')
-                     or name in self.extra_public_methods)
-                    and callable(func))]
-
-    @property
-    def properties(self):
-        if self._cls is None:
-            return []
-        return [name for name, func in inspect.getmembers(self._cls)
+"""
+Extract reference documentation from the NumPy source tree.
+"""
+
+import inspect
+import textwrap
+import re
+import pydoc
+from collections.abc import Mapping
+import sys
+
+
+class Reader:
+    """
+    A line-based string reader.
+    """
+    def __init__(self, data):
+        """
+        Parameters
+        ----------
+        data : str
+           String with lines separated by '\n'.
+
+        """
+        if isinstance(data, list):
+            self._str = data
+        else:
+            self._str = data.split('\n')  # store string as list of lines
+
+        self.reset()
+
+    def __getitem__(self, n):
+        return self._str[n]
+
+    def reset(self):
+        self._l = 0  # current line nr
+
+    def read(self):
+        if not self.eof():
+            out = self[self._l]
+            self._l += 1
+            return out
+        else:
+            return ''
+
+    def seek_next_non_empty_line(self):
+        for l in self[self._l:]:
+            if l.strip():
+                break
+            else:
+                self._l += 1
+
+    def eof(self):
+        return self._l >= len(self._str)
+
+    def read_to_condition(self, condition_func):
+        start = self._l
+        for line in self[start:]:
+            if condition_func(line):
+                return self[start:self._l]
+            self._l += 1
+            if self.eof():
+                return self[start:self._l + 1]
+        return []
+
+    def read_to_next_empty_line(self):
+        self.seek_next_non_empty_line()
+
+        def is_empty(line):
+            return not line.strip()
+
+        return self.read_to_condition(is_empty)
+
+    def read_to_next_unindented_line(self):
+        def is_unindented(line):
+            return (line.strip() and (len(line.lstrip()) == len(line)))
+        return self.read_to_condition(is_unindented)
+
+    def peek(self, n=0):
+        if self._l + n < len(self._str):
+            return self[self._l + n]
+        else:
+            return ''
+
+    def is_empty(self):
+        return not ''.join(self._str).strip()
+
+
+class NumpyDocString(Mapping):
+    def __init__(self, docstring, config={}):
+        docstring = textwrap.dedent(docstring).split('\n')
+
+        self._doc = Reader(docstring)
+        self._parsed_data = {
+            'Signature': '',
+            'Summary': [''],
+            'Extended Summary': [],
+            'Parameters': [],
+            'Returns': [],
+            'Yields': [],
+            'Raises': [],
+            'Warns': [],
+            'Other Parameters': [],
+            'Attributes': [],
+            'Methods': [],
+            'See Also': [],
+            # 'Notes': [],
+            'Warnings': [],
+            'References': '',
+            # 'Examples': '',
+            'index': {}
+        }
+        self._other_keys = []
+
+        self._parse()
+
+    def __getitem__(self, key):
+        return self._parsed_data[key]
+
+    def __setitem__(self, key, val):
+        if key not in self._parsed_data:
+            self._other_keys.append(key)
+
+        self._parsed_data[key] = val
+
+    def __iter__(self):
+        return iter(self._parsed_data)
+
+    def __len__(self):
+        return len(self._parsed_data)
+
+    def _is_at_section(self):
+        self._doc.seek_next_non_empty_line()
+
+        if self._doc.eof():
+            return False
+
+        l1 = self._doc.peek().strip()  # e.g. Parameters
+
+        if l1.startswith('.. index::'):
+            return True
+
+        l2 = self._doc.peek(1).strip()  # ---------- or ==========
+        return l2.startswith(('-' * len(l1), '=' * len(l1)))
+
+    def _strip(self, doc):
+        i = 0
+        j = 0
+        for i, line in enumerate(doc):
+            if line.strip():
+                break
+
+        for j, line in enumerate(doc[::-1]):
+            if line.strip():
+                break
+
+        return doc[i:len(doc) - j]
+
+    def _read_to_next_section(self):
+        section = self._doc.read_to_next_empty_line()
+
+        while not self._is_at_section() and not self._doc.eof():
+            if not self._doc.peek(-1).strip():  # previous line was empty
+                section += ['']
+
+            section += self._doc.read_to_next_empty_line()
+
+        return section
+
+    def _read_sections(self):
+        while not self._doc.eof():
+            data = self._read_to_next_section()
+            name = data[0].strip()
+
+            if name.startswith('..'):  # index section
+                yield name, data[1:]
+            elif len(data) < 2:
+                yield StopIteration
+            else:
+                yield name, self._strip(data[2:])
+
+    def _parse_param_list(self, content):
+        r = Reader(content)
+        params = []
+        while not r.eof():
+            header = r.read().strip()
+            if ' : ' in header:
+                arg_name, arg_type = header.split(' : ')[:2]
+            else:
+                arg_name, arg_type = header, ''
+
+            desc = r.read_to_next_unindented_line()
+            desc = dedent_lines(desc)
+
+            params.append((arg_name, arg_type, desc))
+
+        return params
+
+    _name_rgx = re.compile(r"^\s*(:(?P<role>\w+):`(?P<name>[a-zA-Z0-9_.-]+)`|"
+                           r" (?P<name2>[a-zA-Z0-9_.-]+))\s*", re.X)
+
+    def _parse_see_also(self, content):
+        """
+        func_name : Descriptive text
+            continued text
+        another_func_name : Descriptive text
+        func_name1, func_name2, :meth:`func_name`, func_name3
+
+        """
+        items = []
+
+        def parse_item_name(text):
+            """Match ':role:`name`' or 'name'"""
+            m = self._name_rgx.match(text)
+            if m:
+                g = m.groups()
+                if g[1] is None:
+                    return g[3], None
+                else:
+                    return g[2], g[1]
+            raise ValueError("%s is not an item name" % text)
+
+        def push_item(name, rest):
+            if not name:
+                return
+            name, role = parse_item_name(name)
+            if '.' not in name:
+                name = '~.' + name
+            items.append((name, list(rest), role))
+            del rest[:]
+
+        current_func = None
+        rest = []
+
+        for line in content:
+            if not line.strip():
+                continue
+
+            m = self._name_rgx.match(line)
+            if m and line[m.end():].strip().startswith(':'):
+                push_item(current_func, rest)
+                current_func, line = line[:m.end()], line[m.end():]
+                rest = [line.split(':', 1)[1].strip()]
+                if not rest[0]:
+                    rest = []
+            elif not line.startswith(' '):
+                push_item(current_func, rest)
+                current_func = None
+                if ',' in line:
+                    for func in line.split(','):
+                        if func.strip():
+                            push_item(func, [])
+                elif line.strip():
+                    current_func = line
+            elif current_func is not None:
+                rest.append(line.strip())
+        push_item(current_func, rest)
+        return items
+
+    def _parse_index(self, section, content):
+        """
+        .. index: default
+           :refguide: something, else, and more
+
+        """
+        def strip_each_in(lst):
+            return [s.strip() for s in lst]
+
+        out = {}
+        section = section.split('::')
+        if len(section) > 1:
+            out['default'] = strip_each_in(section[1].split(','))[0]
+        for line in content:
+            line = line.split(':')
+            if len(line) > 2:
+                out[line[1]] = strip_each_in(line[2].split(','))
+        return out
+
+    def _parse_summary(self):
+        """Grab signature (if given) and summary"""
+        if self._is_at_section():
+            return
+
+        # If several signatures present, take the last one
+        while True:
+            summary = self._doc.read_to_next_empty_line()
+            summary_str = " ".join([s.strip() for s in summary]).strip()
+            if re.compile(r'^([\w., ]+=)?\s*[\w\.]+\(.*\)$').match(summary_str):
+                self['Signature'] = summary_str
+                if not self._is_at_section():
+                    continue
+            break
+
+        if summary is not None:
+            self['Summary'] = summary
+
+        if not self._is_at_section():
+            self['Extended Summary'] = self._read_to_next_section()
+
+    def _parse(self):
+        self._doc.reset()
+        self._parse_summary()
+
+        sections = list(self._read_sections())
+        section_names = {section for section, content in sections}
+
+        has_returns = 'Returns' in section_names
+        has_yields = 'Yields' in section_names
+        # We could do more tests, but we are not. Arbitrarily.
+        if has_returns and has_yields:
+            msg = 'Docstring contains both a Returns and Yields section.'
+            raise ValueError(msg)
+
+        for (section, content) in sections:
+            if not section.startswith('..'):
+                section = (s.capitalize() for s in section.split(' '))
+                section = ' '.join(section)
+            if section in ('Parameters', 'Returns', 'Yields', 'Raises',
+                           'Warns', 'Other Parameters', 'Attributes',
+                           'Methods'):
+                self[section] = self._parse_param_list(content)
+            elif section.startswith('.. index::'):
+                self['index'] = self._parse_index(section, content)
+            elif section == 'See Also':
+                self['See Also'] = self._parse_see_also(content)
+            else:
+                self[section] = content
+
+    # string conversion routines
+
+    def _str_header(self, name, symbol='-'):
+        return [name, len(name)*symbol]
+
+    def _str_indent(self, doc, indent=4):
+        out = []
+        for line in doc:
+            out += [' '*indent + line]
+        return out
+
+    def _str_signature(self):
+        if self['Signature']:
+            return [self['Signature'].replace('*', r'\*')] + ['']
+        else:
+            return ['']
+
+    def _str_summary(self):
+        if self['Summary']:
+            return self['Summary'] + ['']
+        else:
+            return []
+
+    def _str_extended_summary(self):
+        if self['Extended Summary']:
+            return self['Extended Summary'] + ['']
+        else:
+            return []
+
+    def _str_param_list(self, name):
+        out = []
+        if self[name]:
+            out += self._str_header(name)
+            for param, param_type, desc in self[name]:
+                if param_type:
+                    out += ['{} : {}'.format(param, param_type)]
+                else:
+                    out += [param]
+                out += self._str_indent(desc)
+            out += ['']
+        return out
+
+    def _str_section(self, name):
+        out = []
+        if self[name]:
+            out += self._str_header(name)
+            out += self[name]
+            out += ['']
+        return out
+
+    def _str_see_also(self, func_role):
+        if not self['See Also']:
+            return []
+        out = []
+        out += self._str_header("See Also")
+        last_had_desc = True
+        for func, desc, role in self['See Also']:
+            if role:
+                link = ':{}:`{}`'.format(role, func)
+            elif func_role:
+                link = ':{}:`{}`'.format(func_role, func)
+            else:
+                link = "`%s`_" % func
+            if desc or last_had_desc:
+                out += ['']
+                out += [link]
+            else:
+                out[-1] += ", %s" % link
+            if desc:
+                out += self._str_indent([' '.join(desc)])
+                last_had_desc = True
+            else:
+                last_had_desc = False
+        out += ['']
+        return out
+
+    def _str_index(self):
+        idx = self['index']
+        out = []
+        out += ['.. index:: %s' % idx.get('default', '')]
+        for section, references in idx.items():
+            if section == 'default':
+                continue
+            out += ['   :{}: {}'.format(section, ', '.join(references))]
+        return out
+
+    def __str__(self, func_role=''):
+        out = []
+        out += self._str_signature()
+        out += self._str_summary()
+        out += self._str_extended_summary()
+        for param_list in ('Parameters', 'Returns', 'Yields',
+                           'Other Parameters', 'Raises', 'Warns'):
+            out += self._str_param_list(param_list)
+        out += self._str_section('Warnings')
+        out += self._str_see_also(func_role)
+        for s in ('Notes', 'References', 'Examples'):
+            out += self._str_section(s)
+        for param_list in ('Attributes', 'Methods'):
+            out += self._str_param_list(param_list)
+        out += self._str_index()
+        return '\n'.join(out)
+
+
+def indent(str, indent=4):
+    indent_str = ' '*indent
+    if str is None:
+        return indent_str
+    lines = str.split('\n')
+    return '\n'.join(indent_str + l for l in lines)
+
+
+def dedent_lines(lines):
+    """Deindent a list of lines maximally"""
+    return textwrap.dedent("\n".join(lines)).split("\n")
+
+
+def header(text, style='-'):
+    return text + '\n' + style*len(text) + '\n'
+
+
+class FunctionDoc(NumpyDocString):
+    def __init__(self, func, role='func', doc=None, config={}):
+        self._f = func
+        self._role = role  # e.g. "func" or "meth"
+
+        if doc is None:
+            if func is None:
+                raise ValueError("No function or docstring given")
+            doc = inspect.getdoc(func) or ''
+        NumpyDocString.__init__(self, doc)
+
+        if not self['Signature'] and func is not None:
+            func, func_name = self.get_func()
+            try:
+                # try to read signature
+                argspec = str(inspect.signature(func))
+                argspec = argspec.replace('*', r'\*')
+                signature = '{}{}'.format(func_name, argspec)
+            except TypeError as e:
+                signature = '%s()' % func_name
+            self['Signature'] = signature
+
+    def get_func(self):
+        func_name = getattr(self._f, '__name__', self.__class__.__name__)
+        if inspect.isclass(self._f):
+            func = getattr(self._f, '__call__', self._f.__init__)
+        else:
+            func = self._f
+        return func, func_name
+
+    def __str__(self):
+        out = ''
+
+        func, func_name = self.get_func()
+        signature = self['Signature'].replace('*', r'\*')
+
+        roles = {'func': 'function',
+                 'meth': 'method'}
+
+        if self._role:
+            if self._role not in roles:
+                print("Warning: invalid role %s" % self._role)
+            out += '.. {}:: {}\n    \n\n'.format(roles.get(self._role, ''),
+                                             func_name)
+
+        out += super().__str__(func_role=self._role)
+        return out
+
+
+class ClassDoc(NumpyDocString):
+
+    extra_public_methods = ['__call__']
+
+    def __init__(self, cls, doc=None, modulename='', func_doc=FunctionDoc,
+                 config={}):
+        if not inspect.isclass(cls) and cls is not None:
+            raise ValueError("Expected a class or None, but got %r" % cls)
+        self._cls = cls
+
+        self.show_inherited_members = config.get(
+                    'show_inherited_class_members', True)
+
+        if modulename and not modulename.endswith('.'):
+            modulename += '.'
+        self._mod = modulename
+
+        if doc is None:
+            if cls is None:
+                raise ValueError("No class or documentation string given")
+            doc = pydoc.getdoc(cls)
+
+        NumpyDocString.__init__(self, doc)
+
+        if config.get('show_class_members', True):
+            def splitlines_x(s):
+                if not s:
+                    return []
+                else:
+                    return s.splitlines()
+
+            for field, items in [('Methods', self.methods),
+                                 ('Attributes', self.properties)]:
+                if not self[field]:
+                    doc_list = []
+                    for name in sorted(items):
+                        clsname = getattr(self._cls, name, None)
+                        if clsname is not None:
+                            doc_item = pydoc.getdoc(clsname)
+                            doc_list.append((name, '', splitlines_x(doc_item)))
+                    self[field] = doc_list
+
+    @property
+    def methods(self):
+        if self._cls is None:
+            return []
+        return [name for name, func in inspect.getmembers(self._cls)
+                if ((not name.startswith('_')
+                     or name in self.extra_public_methods)
+                    and callable(func))]
+
+    @property
+    def properties(self):
+        if self._cls is None:
+            return []
+        return [name for name, func in inspect.getmembers(self._cls)
                 if not name.startswith('_') and func is None]
```

### Comparing `solverz-0.0.1rc1/docs/ext/docscrape_sphinx.py` & `solverz-0.0.1rc2/docs/ext/docscrape_sphinx.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-import sys
-import re
-import inspect
-import textwrap
-import pydoc
-import sphinx
-import collections
-
-from docscrape import NumpyDocString, FunctionDoc, ClassDoc
-
-
-class SphinxDocString(NumpyDocString):
-    def __init__(self, docstring, config={}):
-        NumpyDocString.__init__(self, docstring, config=config)
-        self.load_config(config)
-
-    def load_config(self, config):
-        self.use_plots = config.get('use_plots', False)
-        self.class_members_toctree = config.get('class_members_toctree', True)
-
-    # string conversion routines
-    def _str_header(self, name, symbol='`'):
-        return ['.. rubric:: ' + name, '']
-
-    def _str_field_list(self, name):
-        return [':' + name + ':']
-
-    def _str_indent(self, doc, indent=4):
-        out = []
-        for line in doc:
-            out += [' '*indent + line]
-        return out
-
-    def _str_signature(self):
-        return ['']
-        if self['Signature']:
-            return ['``%s``' % self['Signature']] + ['']
-        else:
-            return ['']
-
-    def _str_summary(self):
-        return self['Summary'] + ['']
-
-    def _str_extended_summary(self):
-        return self['Extended Summary'] + ['']
-
-    def _str_returns(self, name='Returns'):
-        out = []
-        if self[name]:
-            out += self._str_field_list(name)
-            out += ['']
-            for param, param_type, desc in self[name]:
-                if param_type:
-                    out += self._str_indent(['**{}** : {}'.format(param.strip(),
-                                                              param_type)])
-                else:
-                    out += self._str_indent([param.strip()])
-                if desc:
-                    out += ['']
-                    out += self._str_indent(desc, 8)
-                out += ['']
-        return out
-
-    def _str_param_list(self, name):
-        out = []
-        if self[name]:
-            out += self._str_field_list(name)
-            out += ['']
-            for param, param_type, desc in self[name]:
-                if param_type:
-                    out += self._str_indent(['**{}** : {}'.format(param.strip(),
-                                                              param_type)])
-                else:
-                    out += self._str_indent(['**%s**' % param.strip()])
-                if desc:
-                    out += ['']
-                    out += self._str_indent(desc, 8)
-                out += ['']
-        return out
-
-    @property
-    def _obj(self):
-        if hasattr(self, '_cls'):
-            return self._cls
-        elif hasattr(self, '_f'):
-            return self._f
-        return None
-
-    def _str_member_list(self, name):
-        """
-        Generate a member listing, autosummary:: table where possible,
-        and a table where not.
-
-        """
-        out = []
-        if self[name]:
-            out += ['.. rubric:: %s' % name, '']
-            prefix = getattr(self, '_name', '')
-
-            if prefix:
-                prefix = '~%s.' % prefix
-
-            # Lines that are commented out are used to make the
-            # autosummary:: table. Since SymPy does not use the
-            # autosummary:: functionality, it is easiest to just comment it
-            # out.
-            # autosum = []
-            others = []
-            for param, param_type, desc in self[name]:
-                param = param.strip()
-
-                # Check if the referenced member can have a docstring or not
-                param_obj = getattr(self._obj, param, None)
-                if not (callable(param_obj)
-                        or isinstance(param_obj, property)
-                        or inspect.isgetsetdescriptor(param_obj)):
-                    param_obj = None
-
-                # if param_obj and (pydoc.getdoc(param_obj) or not desc):
-                #     # Referenced object has a docstring
-                #     autosum += ["   %s%s" % (prefix, param)]
-                # else:
-                others.append((param, param_type, desc))
-
-            # if autosum:
-            #     out += ['.. autosummary::']
-            #     if self.class_members_toctree:
-            #         out += ['   :toctree:']
-            #     out += [''] + autosum
-
-            if others:
-                maxlen_0 = max(3, max([len(x[0]) for x in others]))
-                hdr = "="*maxlen_0 + "  " + "="*10
-                fmt = '%%%ds  %%s  ' % (maxlen_0,)
-                out += ['', '', hdr]
-                for param, param_type, desc in others:
-                    desc = " ".join(x.strip() for x in desc).strip()
-                    if param_type:
-                        desc = "({}) {}".format(param_type, desc)
-                    out += [fmt % (param.strip(), desc)]
-                out += [hdr]
-            out += ['']
-        return out
-
-    def _str_section(self, name):
-        out = []
-        if self[name]:
-            out += self._str_header(name)
-            out += ['']
-            content = textwrap.dedent("\n".join(self[name])).split("\n")
-            out += content
-            out += ['']
-        return out
-
-    def _str_see_also(self, func_role):
-        out = []
-        if self['See Also']:
-            see_also = super()._str_see_also(func_role)
-            out = ['.. seealso::', '']
-            out += self._str_indent(see_also[2:])
-        return out
-
-    def _str_warnings(self):
-        out = []
-        if self['Warnings']:
-            out = ['.. warning::', '']
-            out += self._str_indent(self['Warnings'])
-        return out
-
-    def _str_index(self):
-        idx = self['index']
-        out = []
-        if len(idx) == 0:
-            return out
-
-        out += ['.. index:: %s' % idx.get('default', '')]
-        for section, references in idx.items():
-            if section == 'default':
-                continue
-            elif section == 'refguide':
-                out += ['   single: %s' % (', '.join(references))]
-            else:
-                out += ['   {}: {}'.format(section, ','.join(references))]
-        return out
-
-    def _str_references(self):
-        out = []
-        if self['References']:
-            out += self._str_header('References')
-            if isinstance(self['References'], str):
-                self['References'] = [self['References']]
-            out.extend(self['References'])
-            out += ['']
-            # Latex collects all references to a separate bibliography,
-            # so we need to insert links to it
-            if sphinx.__version__ >= "0.6":
-                out += ['.. only:: latex', '']
-            else:
-                out += ['.. latexonly::', '']
-            items = []
-            for line in self['References']:
-                m = re.match(r'.. \[([a-z0-9._-]+)\]', line, re.I)
-                if m:
-                    items.append(m.group(1))
-            out += ['   ' + ", ".join(["[%s]_" % item for item in items]), '']
-        return out
-
-    def _str_examples(self):
-        examples_str = "\n".join(self['Examples'])
-
-        if (self.use_plots and 'import matplotlib' in examples_str
-                and 'plot::' not in examples_str):
-            out = []
-            out += self._str_header('Examples')
-            out += ['.. plot::', '']
-            out += self._str_indent(self['Examples'])
-            out += ['']
-            return out
-        else:
-            return self._str_section('Examples')
-
-    def __str__(self, indent=0, func_role="obj"):
-        out = []
-        out += self._str_signature()
-        out += self._str_index() + ['']
-        out += self._str_summary()
-        out += self._str_extended_summary()
-        out += self._str_param_list('Parameters')
-        out += self._str_returns('Returns')
-        out += self._str_returns('Yields')
-        for param_list in ('Other Parameters', 'Raises', 'Warns'):
-            out += self._str_param_list(param_list)
-        out += self._str_warnings()
-        for s in self._other_keys:
-            out += self._str_section(s)
-        out += self._str_see_also(func_role)
-        out += self._str_references()
-        out += self._str_member_list('Attributes')
-        out = self._str_indent(out, indent)
-        return '\n'.join(out)
-
-
-class SphinxFunctionDoc(SphinxDocString, FunctionDoc):
-    def __init__(self, obj, doc=None, config={}):
-        self.load_config(config)
-        FunctionDoc.__init__(self, obj, doc=doc, config=config)
-
-
-class SphinxClassDoc(SphinxDocString, ClassDoc):
-    def __init__(self, obj, doc=None, func_doc=None, config={}):
-        self.load_config(config)
-        ClassDoc.__init__(self, obj, doc=doc, func_doc=None, config=config)
-
-
-class SphinxObjDoc(SphinxDocString):
-    def __init__(self, obj, doc=None, config={}):
-        self._f = obj
-        self.load_config(config)
-        SphinxDocString.__init__(self, doc, config=config)
-
-
-def get_doc_object(obj, what=None, doc=None, config={}):
-    if inspect.isclass(obj):
-        what = 'class'
-    elif inspect.ismodule(obj):
-        what = 'module'
-    elif callable(obj):
-        what = 'function'
-    else:
-        what = 'object'
-
-    if what == 'class':
-        return SphinxClassDoc(obj, func_doc=SphinxFunctionDoc, doc=doc,
-                              config=config)
-    elif what in ('function', 'method'):
-        return SphinxFunctionDoc(obj, doc=doc, config=config)
-    else:
-        if doc is None:
-            doc = pydoc.getdoc(obj)
+import sys
+import re
+import inspect
+import textwrap
+import pydoc
+import sphinx
+import collections
+
+from docscrape import NumpyDocString, FunctionDoc, ClassDoc
+
+
+class SphinxDocString(NumpyDocString):
+    def __init__(self, docstring, config={}):
+        NumpyDocString.__init__(self, docstring, config=config)
+        self.load_config(config)
+
+    def load_config(self, config):
+        self.use_plots = config.get('use_plots', False)
+        self.class_members_toctree = config.get('class_members_toctree', True)
+
+    # string conversion routines
+    def _str_header(self, name, symbol='`'):
+        return ['.. rubric:: ' + name, '']
+
+    def _str_field_list(self, name):
+        return [':' + name + ':']
+
+    def _str_indent(self, doc, indent=4):
+        out = []
+        for line in doc:
+            out += [' '*indent + line]
+        return out
+
+    def _str_signature(self):
+        return ['']
+        if self['Signature']:
+            return ['``%s``' % self['Signature']] + ['']
+        else:
+            return ['']
+
+    def _str_summary(self):
+        return self['Summary'] + ['']
+
+    def _str_extended_summary(self):
+        return self['Extended Summary'] + ['']
+
+    def _str_returns(self, name='Returns'):
+        out = []
+        if self[name]:
+            out += self._str_field_list(name)
+            out += ['']
+            for param, param_type, desc in self[name]:
+                if param_type:
+                    out += self._str_indent(['**{}** : {}'.format(param.strip(),
+                                                              param_type)])
+                else:
+                    out += self._str_indent([param.strip()])
+                if desc:
+                    out += ['']
+                    out += self._str_indent(desc, 8)
+                out += ['']
+        return out
+
+    def _str_param_list(self, name):
+        out = []
+        if self[name]:
+            out += self._str_field_list(name)
+            out += ['']
+            for param, param_type, desc in self[name]:
+                if param_type:
+                    out += self._str_indent(['**{}** : {}'.format(param.strip(),
+                                                              param_type)])
+                else:
+                    out += self._str_indent(['**%s**' % param.strip()])
+                if desc:
+                    out += ['']
+                    out += self._str_indent(desc, 8)
+                out += ['']
+        return out
+
+    @property
+    def _obj(self):
+        if hasattr(self, '_cls'):
+            return self._cls
+        elif hasattr(self, '_f'):
+            return self._f
+        return None
+
+    def _str_member_list(self, name):
+        """
+        Generate a member listing, autosummary:: table where possible,
+        and a table where not.
+
+        """
+        out = []
+        if self[name]:
+            out += ['.. rubric:: %s' % name, '']
+            prefix = getattr(self, '_name', '')
+
+            if prefix:
+                prefix = '~%s.' % prefix
+
+            # Lines that are commented out are used to make the
+            # autosummary:: table. Since SymPy does not use the
+            # autosummary:: functionality, it is easiest to just comment it
+            # out.
+            # autosum = []
+            others = []
+            for param, param_type, desc in self[name]:
+                param = param.strip()
+
+                # Check if the referenced member can have a docstring or not
+                param_obj = getattr(self._obj, param, None)
+                if not (callable(param_obj)
+                        or isinstance(param_obj, property)
+                        or inspect.isgetsetdescriptor(param_obj)):
+                    param_obj = None
+
+                # if param_obj and (pydoc.getdoc(param_obj) or not desc):
+                #     # Referenced object has a docstring
+                #     autosum += ["   %s%s" % (prefix, param)]
+                # else:
+                others.append((param, param_type, desc))
+
+            # if autosum:
+            #     out += ['.. autosummary::']
+            #     if self.class_members_toctree:
+            #         out += ['   :toctree:']
+            #     out += [''] + autosum
+
+            if others:
+                maxlen_0 = max(3, max([len(x[0]) for x in others]))
+                hdr = "="*maxlen_0 + "  " + "="*10
+                fmt = '%%%ds  %%s  ' % (maxlen_0,)
+                out += ['', '', hdr]
+                for param, param_type, desc in others:
+                    desc = " ".join(x.strip() for x in desc).strip()
+                    if param_type:
+                        desc = "({}) {}".format(param_type, desc)
+                    out += [fmt % (param.strip(), desc)]
+                out += [hdr]
+            out += ['']
+        return out
+
+    def _str_section(self, name):
+        out = []
+        if self[name]:
+            out += self._str_header(name)
+            out += ['']
+            content = textwrap.dedent("\n".join(self[name])).split("\n")
+            out += content
+            out += ['']
+        return out
+
+    def _str_see_also(self, func_role):
+        out = []
+        if self['See Also']:
+            see_also = super()._str_see_also(func_role)
+            out = ['.. seealso::', '']
+            out += self._str_indent(see_also[2:])
+        return out
+
+    def _str_warnings(self):
+        out = []
+        if self['Warnings']:
+            out = ['.. warning::', '']
+            out += self._str_indent(self['Warnings'])
+        return out
+
+    def _str_index(self):
+        idx = self['index']
+        out = []
+        if len(idx) == 0:
+            return out
+
+        out += ['.. index:: %s' % idx.get('default', '')]
+        for section, references in idx.items():
+            if section == 'default':
+                continue
+            elif section == 'refguide':
+                out += ['   single: %s' % (', '.join(references))]
+            else:
+                out += ['   {}: {}'.format(section, ','.join(references))]
+        return out
+
+    def _str_references(self):
+        out = []
+        if self['References']:
+            out += self._str_header('References')
+            if isinstance(self['References'], str):
+                self['References'] = [self['References']]
+            out.extend(self['References'])
+            out += ['']
+            # Latex collects all references to a separate bibliography,
+            # so we need to insert links to it
+            if sphinx.__version__ >= "0.6":
+                out += ['.. only:: latex', '']
+            else:
+                out += ['.. latexonly::', '']
+            items = []
+            for line in self['References']:
+                m = re.match(r'.. \[([a-z0-9._-]+)\]', line, re.I)
+                if m:
+                    items.append(m.group(1))
+            out += ['   ' + ", ".join(["[%s]_" % item for item in items]), '']
+        return out
+
+    def _str_examples(self):
+        examples_str = "\n".join(self['Examples'])
+
+        if (self.use_plots and 'import matplotlib' in examples_str
+                and 'plot::' not in examples_str):
+            out = []
+            out += self._str_header('Examples')
+            out += ['.. plot::', '']
+            out += self._str_indent(self['Examples'])
+            out += ['']
+            return out
+        else:
+            return self._str_section('Examples')
+
+    def __str__(self, indent=0, func_role="obj"):
+        out = []
+        out += self._str_signature()
+        out += self._str_index() + ['']
+        out += self._str_summary()
+        out += self._str_extended_summary()
+        out += self._str_param_list('Parameters')
+        out += self._str_returns('Returns')
+        out += self._str_returns('Yields')
+        for param_list in ('Other Parameters', 'Raises', 'Warns'):
+            out += self._str_param_list(param_list)
+        out += self._str_warnings()
+        for s in self._other_keys:
+            out += self._str_section(s)
+        out += self._str_see_also(func_role)
+        out += self._str_references()
+        out += self._str_member_list('Attributes')
+        out = self._str_indent(out, indent)
+        return '\n'.join(out)
+
+
+class SphinxFunctionDoc(SphinxDocString, FunctionDoc):
+    def __init__(self, obj, doc=None, config={}):
+        self.load_config(config)
+        FunctionDoc.__init__(self, obj, doc=doc, config=config)
+
+
+class SphinxClassDoc(SphinxDocString, ClassDoc):
+    def __init__(self, obj, doc=None, func_doc=None, config={}):
+        self.load_config(config)
+        ClassDoc.__init__(self, obj, doc=doc, func_doc=None, config=config)
+
+
+class SphinxObjDoc(SphinxDocString):
+    def __init__(self, obj, doc=None, config={}):
+        self._f = obj
+        self.load_config(config)
+        SphinxDocString.__init__(self, doc, config=config)
+
+
+def get_doc_object(obj, what=None, doc=None, config={}):
+    if inspect.isclass(obj):
+        what = 'class'
+    elif inspect.ismodule(obj):
+        what = 'module'
+    elif callable(obj):
+        what = 'function'
+    else:
+        what = 'object'
+
+    if what == 'class':
+        return SphinxClassDoc(obj, func_doc=SphinxFunctionDoc, doc=doc,
+                              config=config)
+    elif what in ('function', 'method'):
+        return SphinxFunctionDoc(obj, doc=doc, config=config)
+    else:
+        if doc is None:
+            doc = pydoc.getdoc(obj)
         return SphinxObjDoc(obj, doc, config=config)
```

### Comparing `solverz-0.0.1rc1/docs/ext/numpydoc.py` & `solverz-0.0.1rc2/docs/ext/numpydoc.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-"""
-========
-numpydoc
-========
-
-Sphinx extension that handles docstrings in the Numpy standard format. [1]
-
-It will:
-
-- Convert Parameters etc. sections to field lists.
-- Convert See Also section to a See also entry.
-- Renumber references.
-- Extract the signature from the docstring, if it can't be determined
-  otherwise.
-
-.. [1] https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt
-
-"""
-
-import sys
-import re
-import pydoc
-import sphinx
-import inspect
-from collections.abc import Callable
-
-if sphinx.__version__ < '1.0.1':
-    raise RuntimeError("Sphinx 1.0.1 or newer is required")
-
-from docscrape_sphinx import get_doc_object, SphinxDocString
-
-
-def mangle_docstrings(app, what, name, obj, options, lines,
-                      reference_offset=[0]):
-
-    cfg = {'use_plots': app.config.numpydoc_use_plots,
-           'show_class_members': app.config.numpydoc_show_class_members,
-           'show_inherited_class_members':
-           app.config.numpydoc_show_inherited_class_members,
-           'class_members_toctree': app.config.numpydoc_class_members_toctree}
-
-    u_NL = '\n'
-    if what == 'module':
-        # Strip top title
-        pattern = '^\\s*[#*=]{4,}\\n[a-z0-9 -]+\\n[#*=]{4,}\\s*'
-        title_re = re.compile(pattern, re.I | re.S)
-        lines[:] = title_re.sub('', u_NL.join(lines)).split(u_NL)
-    else:
-        doc = get_doc_object(obj, what, u_NL.join(lines), config=cfg)
-        if sys.version_info[0] >= 3:
-            doc = str(doc)
-        else:
-            doc = unicode(doc)
-        lines[:] = doc.split(u_NL)
-
-    if (app.config.numpydoc_edit_link and hasattr(obj, '__name__') and
-            obj.__name__):
-        if hasattr(obj, '__module__'):
-            v = {"full_name": "{}.{}".format(obj.__module__, obj.__name__)}
-        else:
-            v = {"full_name": obj.__name__}
-        lines += ['', '.. htmlonly::', '']
-        lines += ['    %s' % x for x in
-                  (app.config.numpydoc_edit_link % v).split("\n")]
-
-    # replace reference numbers so that there are no duplicates
-    references = []
-    for line in lines:
-        line = line.strip()
-        m = re.match('^.. \\[([a-z0-9_.-])\\]', line, re.I)
-        if m:
-            references.append(m.group(1))
-
-    # start renaming from the longest string, to avoid overwriting parts
-    references.sort(key=lambda x: -len(x))
-    if references:
-        for i, line in enumerate(lines):
-            for r in references:
-                if re.match('^\\d+$', r):
-                    new_r = "R%d" % (reference_offset[0] + int(r))
-                else:
-                    new_r = "%s%d" % (r, reference_offset[0])
-                lines[i] = lines[i].replace('[%s]_' % r,
-                                            '[%s]_' % new_r)
-                lines[i] = lines[i].replace('.. [%s]' % r,
-                                            '.. [%s]' % new_r)
-
-    reference_offset[0] += len(references)
-
-
-def mangle_signature(app, what, name, obj, options, sig, retann):
-    # Do not try to inspect classes that don't define `__init__`
-    if (inspect.isclass(obj) and
-        (not hasattr(obj, '__init__') or
-            'initializes x; see ' in pydoc.getdoc(obj.__init__))):
-        return '', ''
-
-    if not (isinstance(obj, Callable) or
-            hasattr(obj, '__argspec_is_invalid_')):
-        return
-
-    if not hasattr(obj, '__doc__'):
-        return
-
-    doc = SphinxDocString(pydoc.getdoc(obj))
-    if doc['Signature']:
-        sig = re.sub("^[^(]*", "", doc['Signature'])
-        return sig, ''
-
-
-def setup(app, get_doc_object_=get_doc_object):
-    if not hasattr(app, 'add_config_value'):
-        return  # probably called by nose, better bail out
-
-    global get_doc_object
-    get_doc_object = get_doc_object_
-
-    app.connect('autodoc-process-docstring', mangle_docstrings)
-    app.connect('autodoc-process-signature', mangle_signature)
-    app.add_config_value('numpydoc_edit_link', None, False)
-    app.add_config_value('numpydoc_use_plots', None, False)
-    app.add_config_value('numpydoc_show_class_members', True, True)
-    app.add_config_value('numpydoc_show_inherited_class_members', True, True)
-    app.add_config_value('numpydoc_class_members_toctree', True, True)
-
-    # Extra mangling domains
-    app.add_domain(NumpyPythonDomain)
-    app.add_domain(NumpyCDomain)
-
-# ------------------------------------------------------------------------------
-# Docstring-mangling domains
-# ------------------------------------------------------------------------------
-
-from docutils.statemachine import ViewList
-from sphinx.domains.c import CDomain
-from sphinx.domains.python import PythonDomain
-
-
-class ManglingDomainBase:
-    directive_mangling_map = {}
-
-    def __init__(self, *a, **kw):
-        super().__init__(*a, **kw)
-        self.wrap_mangling_directives()
-
-    def wrap_mangling_directives(self):
-        for name, objtype in list(self.directive_mangling_map.items()):
-            self.directives[name] = wrap_mangling_directive(
-                self.directives[name], objtype)
-
-
-class NumpyPythonDomain(ManglingDomainBase, PythonDomain):
-    name = 'np'
-    directive_mangling_map = {
-        'function': 'function',
-        'class': 'class',
-        'exception': 'class',
-        'method': 'function',
-        'classmethod': 'function',
-        'staticmethod': 'function',
-        'attribute': 'attribute',
-    }
-    indices = []
-
-
-class NumpyCDomain(ManglingDomainBase, CDomain):
-    name = 'np-c'
-    directive_mangling_map = {
-        'function': 'function',
-        'member': 'attribute',
-        'macro': 'function',
-        'type': 'class',
-        'var': 'object',
-    }
-
-
-def wrap_mangling_directive(base_directive, objtype):
-    class directive(base_directive):
-        def run(self):
-            env = self.state.document.settings.env
-
-            name = None
-            if self.arguments:
-                m = re.match(r'^(.*\s+)?(.*?)(\(.*)?', self.arguments[0])
-                name = m.group(2).strip()
-
-            if not name:
-                name = self.arguments[0]
-
-            lines = list(self.content)
-            mangle_docstrings(env.app, objtype, name, None, None, lines)
-            self.content = ViewList(lines, self.content.parent)
-
-            return base_directive.run(self)
-
+"""
+========
+numpydoc
+========
+
+Sphinx extension that handles docstrings in the Numpy standard format. [1]
+
+It will:
+
+- Convert Parameters etc. sections to field lists.
+- Convert See Also section to a See also entry.
+- Renumber references.
+- Extract the signature from the docstring, if it can't be determined
+  otherwise.
+
+.. [1] https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt
+
+"""
+
+import sys
+import re
+import pydoc
+import sphinx
+import inspect
+from collections.abc import Callable
+
+if sphinx.__version__ < '1.0.1':
+    raise RuntimeError("Sphinx 1.0.1 or newer is required")
+
+from docscrape_sphinx import get_doc_object, SphinxDocString
+
+
+def mangle_docstrings(app, what, name, obj, options, lines,
+                      reference_offset=[0]):
+
+    cfg = {'use_plots': app.config.numpydoc_use_plots,
+           'show_class_members': app.config.numpydoc_show_class_members,
+           'show_inherited_class_members':
+           app.config.numpydoc_show_inherited_class_members,
+           'class_members_toctree': app.config.numpydoc_class_members_toctree}
+
+    u_NL = '\n'
+    if what == 'module':
+        # Strip top title
+        pattern = '^\\s*[#*=]{4,}\\n[a-z0-9 -]+\\n[#*=]{4,}\\s*'
+        title_re = re.compile(pattern, re.I | re.S)
+        lines[:] = title_re.sub('', u_NL.join(lines)).split(u_NL)
+    else:
+        doc = get_doc_object(obj, what, u_NL.join(lines), config=cfg)
+        if sys.version_info[0] >= 3:
+            doc = str(doc)
+        else:
+            doc = unicode(doc)
+        lines[:] = doc.split(u_NL)
+
+    if (app.config.numpydoc_edit_link and hasattr(obj, '__name__') and
+            obj.__name__):
+        if hasattr(obj, '__module__'):
+            v = {"full_name": "{}.{}".format(obj.__module__, obj.__name__)}
+        else:
+            v = {"full_name": obj.__name__}
+        lines += ['', '.. htmlonly::', '']
+        lines += ['    %s' % x for x in
+                  (app.config.numpydoc_edit_link % v).split("\n")]
+
+    # replace reference numbers so that there are no duplicates
+    references = []
+    for line in lines:
+        line = line.strip()
+        m = re.match('^.. \\[([a-z0-9_.-])\\]', line, re.I)
+        if m:
+            references.append(m.group(1))
+
+    # start renaming from the longest string, to avoid overwriting parts
+    references.sort(key=lambda x: -len(x))
+    if references:
+        for i, line in enumerate(lines):
+            for r in references:
+                if re.match('^\\d+$', r):
+                    new_r = "R%d" % (reference_offset[0] + int(r))
+                else:
+                    new_r = "%s%d" % (r, reference_offset[0])
+                lines[i] = lines[i].replace('[%s]_' % r,
+                                            '[%s]_' % new_r)
+                lines[i] = lines[i].replace('.. [%s]' % r,
+                                            '.. [%s]' % new_r)
+
+    reference_offset[0] += len(references)
+
+
+def mangle_signature(app, what, name, obj, options, sig, retann):
+    # Do not try to inspect classes that don't define `__init__`
+    if (inspect.isclass(obj) and
+        (not hasattr(obj, '__init__') or
+            'initializes x; see ' in pydoc.getdoc(obj.__init__))):
+        return '', ''
+
+    if not (isinstance(obj, Callable) or
+            hasattr(obj, '__argspec_is_invalid_')):
+        return
+
+    if not hasattr(obj, '__doc__'):
+        return
+
+    doc = SphinxDocString(pydoc.getdoc(obj))
+    if doc['Signature']:
+        sig = re.sub("^[^(]*", "", doc['Signature'])
+        return sig, ''
+
+
+def setup(app, get_doc_object_=get_doc_object):
+    if not hasattr(app, 'add_config_value'):
+        return  # probably called by nose, better bail out
+
+    global get_doc_object
+    get_doc_object = get_doc_object_
+
+    app.connect('autodoc-process-docstring', mangle_docstrings)
+    app.connect('autodoc-process-signature', mangle_signature)
+    app.add_config_value('numpydoc_edit_link', None, False)
+    app.add_config_value('numpydoc_use_plots', None, False)
+    app.add_config_value('numpydoc_show_class_members', True, True)
+    app.add_config_value('numpydoc_show_inherited_class_members', True, True)
+    app.add_config_value('numpydoc_class_members_toctree', True, True)
+
+    # Extra mangling domains
+    app.add_domain(NumpyPythonDomain)
+    app.add_domain(NumpyCDomain)
+
+# ------------------------------------------------------------------------------
+# Docstring-mangling domains
+# ------------------------------------------------------------------------------
+
+from docutils.statemachine import ViewList
+from sphinx.domains.c import CDomain
+from sphinx.domains.python import PythonDomain
+
+
+class ManglingDomainBase:
+    directive_mangling_map = {}
+
+    def __init__(self, *a, **kw):
+        super().__init__(*a, **kw)
+        self.wrap_mangling_directives()
+
+    def wrap_mangling_directives(self):
+        for name, objtype in list(self.directive_mangling_map.items()):
+            self.directives[name] = wrap_mangling_directive(
+                self.directives[name], objtype)
+
+
+class NumpyPythonDomain(ManglingDomainBase, PythonDomain):
+    name = 'np'
+    directive_mangling_map = {
+        'function': 'function',
+        'class': 'class',
+        'exception': 'class',
+        'method': 'function',
+        'classmethod': 'function',
+        'staticmethod': 'function',
+        'attribute': 'attribute',
+    }
+    indices = []
+
+
+class NumpyCDomain(ManglingDomainBase, CDomain):
+    name = 'np-c'
+    directive_mangling_map = {
+        'function': 'function',
+        'member': 'attribute',
+        'macro': 'function',
+        'type': 'class',
+        'var': 'object',
+    }
+
+
+def wrap_mangling_directive(base_directive, objtype):
+    class directive(base_directive):
+        def run(self):
+            env = self.state.document.settings.env
+
+            name = None
+            if self.arguments:
+                m = re.match(r'^(.*\s+)?(.*?)(\(.*)?', self.arguments[0])
+                name = m.group(2).strip()
+
+            if not name:
+                name = self.arguments[0]
+
+            lines = list(self.content)
+            mangle_docstrings(env.app, objtype, name, None, None, lines)
+            self.content = ViewList(lines, self.content.parent)
+
+            return base_directive.run(self)
+
     return directive
```

### Comparing `solverz-0.0.1rc1/docs/src/advanced.md` & `solverz-0.0.1rc2/docs/src/advanced.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-(advanced)=
-
-# Advanced Usage
-
-## Writing Custom Functions
-Sometimes one may have functions that go beyond the Solverz built-in library. This guide will describe how to create 
-such custom functions in Solverz, so that the functions can be incorporated into numerical simulations. The philosophy 
-of function customization comes from Sympy, it helps to learn the [Sympy basics](https://docs.sympy.org/latest/index.html) 
-and read the [Sympy tutorial of custom functions](https://docs.sympy.org/latest/guides/custom-functions.html) for an overview.
-
-As a motivating example for this document, let's create a custom function class representing the $\min$ function. We 
-want use $\min$ to determine the smaller one of two operands, which can be defined by
-
-```{math}
-\min(x,y)=
-\begin{cases}
-x&x\leq y\\
-y& x>y
-\end{cases}
-```
-
-We also want to extend the function to vector input, that is, capable of finding the element-wise minimum of two vectors.
-To summarize, we shall implement $\min$ that
-
-1. evaluates $\min(x,y)$ correctly
-2. can be derived proper derivatives with respect to $x$ and $y$.
-
-However, it is difficult to devise the analytical derivatives of $\min$. We should perform the trick that rewrites 
-$\min(x,y)$ as
-
-```{math}
-x*\operatorname{lessthan}(x,y)+y*(1-\operatorname{lessthan}(x,y)).
-```
-
-where the $\operatorname{lessthan}(x,y)$ function mathematically denotes the $\leq$ operator and returns 1 if 
-$x\leq y$ else 0. Since $\operatorname{lessthan}(x,y)$ can only be either 1 or 0, the above transformation holds. 
-
-If the derivatives of $\operatorname{lessthan}(x,y)$ with respect to any argument are zero, then we have
-```{math}
-\frac{\partial}{\partial x}\min(x,y)=
-\operatorname{lessthan}(x,y)
-```
-and
-```{math}
-\frac{\partial}{\partial y}\min(x,y)=
-1-\operatorname{lessthan}(x,y).
-```
-Hence, it suffices to have a custom $\operatorname{lessthan}(x,y)$ function that
-
-1. evaluates $\operatorname{lessthan}(x,y)$ correctly
-2. has zero-derivative with respect to $x$ or $y$.
-
-Let us start by subclassing `MulVarFunc`
-```python
-from Solverz.sym_algebra.functions import MulVarFunc
-class Min(MulVarFunc):
-    pass
-class LessThan(MulVarFunc):
-    pass
-```
-The `MulVarFunc` is the base class of multi-variate functions in Solverz. 
-At this point, `Min` has no behaviors defined on it. To automatically evaluate the `Min` function, we ought to define 
-the **_class method_** `eval()`. `eval()` should take the arguments of the function and return the value 
-$x*\operatorname{lessthan}(x,y)+y*(1-\operatorname{lessthan}(x,y))$:
-```python
-class Min(MulVarFunc):
-    @classmethod
-    def eval(cls, x, y):
-        return x * LessThan(x, y) + y * (1 - LessThan(x, y))
-```
-```python
->>> from Solverz import Var
->>> Min(Var('x',0),Var('y',0))
-... x*((x)<=(y)) + y*(1 - ((x)<=(y)))
-```
-To define the differentiation of  `LessThan()`, we have
-```python
-from sympy import Integer
-class LessThan(MulVarFunc):
-    """
-    Represents < operator
-    """
-
-    def _eval_derivative(self, s):
-        return Integer(0)
-
-    def _sympystr(self, printer, **kwargs):
-        return '(({op1})<=({op2}))'.format(op1=printer._print(self.args[0]),
-                                           op2=printer._print(self.args[1]))
-
-    def _numpycode(self, printer, **kwargs):
-        return r'SolLessThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
-
-    def _lambdacode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-```
-Here, the `_sympystr()` method defines its string representation:
-```python
->>> LessThan(Var('x'), Var('y'))
-... ((x)<=(y))
-```
-The `_eval_derivative()` method forces the derivatives of `LessThan()` to be zero:
-```python
-from Solverz import iVar
->>> Min(Var('x',0),Var('y',0)).diff(iVar('x'))
-... ((x)<=(y))
-```
-where `iVar` is the internal variable type of Solverz, `diff()` is the method to derive derivatives.
-
-The `_numpycode()` function defines what should `LessThan()` be printed to  in numerical codes. Here, we define the 
-`SolLessThan()` as the numerical implementation of  `LessThan()`. Given array `[0,2,-1]` and `[1,2,3]`:
-```python
->>> import numpy as np
->>> SolLessThan(np.array([0, 2, -1]), np.array([1,2,3]))
-... array([1, 0, 1])
-```
-```{note}
-In Solverz, the numerical computations are mainly dependent on the prevailing numerical libraries such as numpy and scipy. 
-It is recommended that one first gets familiar with the [numpy](https://numpy.org/doc/stable/user/index.html) and 
-[scipy](https://docs.scipy.org/doc/scipy/tutorial/index.html).
-```
-The implementation of `SolLessThan()` should be put in the `Solverz.num_api.custom_function` module:
-```python
-@implements_nfunc('SolLessThan')
-@njit(cache=True)
-def SolLessThan(x, y):
-    x = np.asarray(x).reshape((-1,))
-    return (x < y).astype(np.int32)
-```
-The `implements_nfunc()` cannot be omitted and the `njit()` decorator enables the numba-based dynamic compilation for efficiency.
-
+(advanced)=
+
+# Advanced Usage
+
+## Writing Custom Functions
+Sometimes one may have functions that go beyond the Solverz built-in library. This guide will describe how to create 
+such custom functions in Solverz, so that the functions can be incorporated into numerical simulations. The philosophy 
+of function customization comes from Sympy, it helps to learn the [Sympy basics](https://docs.sympy.org/latest/index.html) 
+and read the [Sympy tutorial of custom functions](https://docs.sympy.org/latest/guides/custom-functions.html) for an overview.
+
+As a motivating example for this document, let's create a custom function class representing the $\min$ function. We 
+want use $\min$ to determine the smaller one of two operands, which can be defined by
+
+```{math}
+\min(x,y)=
+\begin{cases}
+x&x\leq y\\
+y& x>y
+\end{cases}
+```
+
+We also want to extend the function to vector input, that is, capable of finding the element-wise minimum of two vectors.
+To summarize, we shall implement $\min$ that
+
+1. evaluates $\min(x,y)$ correctly
+2. can be derived proper derivatives with respect to $x$ and $y$.
+
+However, it is difficult to devise the analytical derivatives of $\min$. We should perform the trick that rewrites 
+$\min(x,y)$ as
+
+```{math}
+x*\operatorname{lessthan}(x,y)+y*(1-\operatorname{lessthan}(x,y)).
+```
+
+where the $\operatorname{lessthan}(x,y)$ function mathematically denotes the $\leq$ operator and returns 1 if 
+$x\leq y$ else 0. Since $\operatorname{lessthan}(x,y)$ can only be either 1 or 0, the above transformation holds. 
+
+If the derivatives of $\operatorname{lessthan}(x,y)$ with respect to any argument are zero, then we have
+```{math}
+\frac{\partial}{\partial x}\min(x,y)=
+\operatorname{lessthan}(x,y)
+```
+and
+```{math}
+\frac{\partial}{\partial y}\min(x,y)=
+1-\operatorname{lessthan}(x,y).
+```
+Hence, it suffices to have a custom $\operatorname{lessthan}(x,y)$ function that
+
+1. evaluates $\operatorname{lessthan}(x,y)$ correctly
+2. has zero-derivative with respect to $x$ or $y$.
+
+Let us start by subclassing `MulVarFunc`
+```python
+from Solverz.sym_algebra.functions import MulVarFunc
+class Min(MulVarFunc):
+    pass
+class LessThan(MulVarFunc):
+    pass
+```
+The `MulVarFunc` is the base class of multi-variate functions in Solverz. 
+At this point, `Min` has no behaviors defined on it. To automatically evaluate the `Min` function, we ought to define 
+the **_class method_** `eval()`. `eval()` should take the arguments of the function and return the value 
+$x*\operatorname{lessthan}(x,y)+y*(1-\operatorname{lessthan}(x,y))$:
+```python
+class Min(MulVarFunc):
+    @classmethod
+    def eval(cls, x, y):
+        return x * LessThan(x, y) + y * (1 - LessThan(x, y))
+```
+```python
+>>> from Solverz import Var
+>>> Min(Var('x',0),Var('y',0))
+... x*((x)<=(y)) + y*(1 - ((x)<=(y)))
+```
+To define the differentiation of  `LessThan()`, we have
+```python
+from sympy import Integer
+class LessThan(MulVarFunc):
+    """
+    Represents < operator
+    """
+
+    def _eval_derivative(self, s):
+        return Integer(0)
+
+    def _sympystr(self, printer, **kwargs):
+        return '(({op1})<=({op2}))'.format(op1=printer._print(self.args[0]),
+                                           op2=printer._print(self.args[1]))
+
+    def _numpycode(self, printer, **kwargs):
+        return r'SolLessThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
+
+    def _lambdacode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+
+    def _pythoncode(self, printer, **kwargs):
+        return self._numpycode(printer, **kwargs)
+```
+Here, the `_sympystr()` method defines its string representation:
+```python
+>>> LessThan(Var('x'), Var('y'))
+... ((x)<=(y))
+```
+The `_eval_derivative()` method forces the derivatives of `LessThan()` to be zero:
+```python
+from Solverz import iVar
+>>> Min(Var('x',0),Var('y',0)).diff(iVar('x'))
+... ((x)<=(y))
+```
+where `iVar` is the internal variable type of Solverz, `diff()` is the method to derive derivatives.
+
+The `_numpycode()` function defines what should `LessThan()` be printed to  in numerical codes. Here, we define the 
+`SolLessThan()` as the numerical implementation of  `LessThan()`. Given array `[0,2,-1]` and `[1,2,3]`:
+```python
+>>> import numpy as np
+>>> SolLessThan(np.array([0, 2, -1]), np.array([1,2,3]))
+... array([1, 0, 1])
+```
+```{note}
+In Solverz, the numerical computations are mainly dependent on the prevailing numerical libraries such as numpy and scipy. 
+It is recommended that one first gets familiar with the [numpy](https://numpy.org/doc/stable/user/index.html) and 
+[scipy](https://docs.scipy.org/doc/scipy/tutorial/index.html).
+```
+The implementation of `SolLessThan()` should be put in the `Solverz.num_api.custom_function` module:
+```python
+@implements_nfunc('SolLessThan')
+@njit(cache=True)
+def SolLessThan(x, y):
+    x = np.asarray(x).reshape((-1,))
+    return (x < y).astype(np.int32)
+```
+The `implements_nfunc()` cannot be omitted and the `njit()` decorator enables the numba-based dynamic compilation for efficiency.
+
```

### Comparing `solverz-0.0.1rc1/docs/src/conf.py` & `solverz-0.0.1rc2/docs/src/conf.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,197 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-import inspect
-import os
-import sys
-import time
-
-import sympy
-
-sys.path = ['ext'] + sys.path
-sys.path.extend(['..\\..\\Solverz'])
-# This command is for linux (Ubuntu 22.04.2 LTS), which cannot recognise relative path of Solverz library.
-sys.path.insert(0, os.path.abspath('../..'))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'Solverz'
-copyright = f'{time.localtime().tm_year}, Ruizhi Yu'
-author = 'Ruizhi Yu'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
-              'sphinx_math_dollar', 'sphinx.ext.mathjax', 'numpydoc',
-              'sphinx_reredirects', 'sphinx_copybutton',
-              'sphinx.ext.graphviz', 'sphinxcontrib.jquery',
-              'matplotlib.sphinxext.plot_directive', 'myst_parser',
-              'convert-svg-to-pdf', 'sphinx.ext.intersphinx', ]  # 'sphinx.ext.linkcode'
-
-# To stop docstrings inheritance.
-autodoc_inherit_docstrings = False
-
-# Sphinx是一个文档生成器，可以将Markdown或reStructuredText等文本格式转化为HTML、PDF等格式的文档。而MathJax是一个用于渲染数学公式的JavaScript库，它可以帮助将LaTeX或MathML格式的数学公式渲染为高质量的矢量图形。
-# 虽然Sphinx本身提供了一些对数学公式的支持，但其渲染效果不如MathJax优秀。因此，为了获得更好的数学公式渲染效果，使用MathJax插件可以帮助Sphinx在生成文档时自动渲染数学公式，从而提高文档的质量和可读性。
-
-templates_path = ['_templates']
-exclude_patterns = []
-
-source_suffix = {
-    '.rst': 'restructuredtext',
-    '.txt': 'markdown',
-    '.md': 'markdown',
-}
-
-mathjax3_config = {
-    "tex": {
-        "inlineMath": [['\\(', '\\)']],
-        "displayMath": [["\\[", "\\]"]],
-        'packages': {'[+]': ['physics']}
-    },
-    'loader': {'load': ['[tex]/physics']},
-}
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-
-html_static_path = ['_static']
-
-html_theme = 'furo'
-
-common_theme_variables = {
-    # Main "SymPy green" colors. Many things uses these colors.
-    "color-brand-primary": "#52833A",
-    "color-brand-content": "#307748",
-
-    # The left sidebar.
-    "color-sidebar-background": "#3B5526",
-    "color-sidebar-background-border": "var(--color-background-primary)",
-    "color-sidebar-link-text": "#FFFFFF",
-    "color-sidebar-brand-text": "var(--color-sidebar-link-text--top-level)",
-    "color-sidebar-link-text--top-level": "#FFFFFF",
-    "color-sidebar-item-background--hover": "var(--color-brand-primary)",
-    "color-sidebar-item-expander-background--hover": "var(--color-brand-primary)",
-
-    "color-link-underline--hover": "var(--color-link)",
-    "color-api-keyword": "#000000bd",
-    "color-api-name": "var(--color-brand-content)",
-    "color-api-pre-name": "var(--color-brand-content)",
-    "api-font-size": "var(--font-size--normal)",
-    "color-foreground-secondary": "#53555B",
-
-    # TODO: Add the other types of admonitions here if anyone uses them.
-    "color-admonition-title-background--seealso": "#CCCCCC",
-    "color-admonition-title--seealso": "black",
-    "color-admonition-title-background--note": "#CCCCCC",
-    "color-admonition-title--note": "black",
-    "color-admonition-title-background--warning": "var(--color-problematic)",
-    "color-admonition-title--warning": "white",
-    "admonition-font-size": "var(--font-size--normal)",
-    "admonition-title-font-size": "var(--font-size--normal)",
-
-    # Note: this doesn't work. If we want to change this, we have to set
-    # it as the .highlight background in custom.css.
-    "color-code-background": "hsl(80deg 100% 95%)",
-
-    "code-font-size": "var(--font-size--small)",
-    "font-stack--monospace": 'DejaVu Sans Mono,"SFMono-Regular",Menlo,Consolas,Monaco,Liberation Mono,Lucida Console,monospace;'
-}
-
-html_theme_options = {
-    "light_css_variables": common_theme_variables,
-    # The dark variables automatically inherit values from the light variables
-    "dark_css_variables": {
-        **common_theme_variables,
-        "color-brand-primary": "#33CB33",
-        "color-brand-content": "#1DBD1D",
-
-        "color-api-keyword": "#FFFFFFbd",
-        "color-api-overall": "#FFFFFF90",
-        "color-api-paren": "#FFFFFF90",
-
-        "color-sidebar-item-background--hover": "#52833A",
-        "color-sidebar-item-expander-background--hover": "#52833A",
-        # This is the color of the text in the right sidebar
-        "color-foreground-secondary": "#9DA1AC",
-
-        "color-admonition-title-background--seealso": "#555555",
-        "color-admonition-title-background--note": "#555555",
-        "color-problematic": "#B30000",
-    },
-    # See https://pradyunsg.me/furo/customisation/footer/
-    "footer_icons": [
-        {
-            "name": "GitHub",
-            "url": "https://github.com/smallbunnies/Solverz",
-            "html": """
-                <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 16 16">
-                    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
-                </svg>
-            """,
-            "class": "",
-        },
-    ],
-}
-
-html_css_files = ['custom.css']
-
-html_domain_indices = ['py-modindex']
-
-# Solverz logo on title page
-html_logo = '_static/sympylogo.png'
-latex_logo = '_static/sympylogo_big.png'
-html_favicon = '../_build/logo/sympy-notailtext-favicon.ico'
-
-
-def linkcode_resolve(domain, info):
-    """Determine the URL corresponding to Python object."""
-    if domain != 'py':
-        return
-
-    modname = info['module']
-    fullname = info['fullname']
-
-    submod = sys.modules.get(modname)
-    if submod is None:
-        return
-
-    obj = submod
-    for part in fullname.split('.'):
-        try:
-            obj = getattr(obj, part)
-        except Exception:
-            return
-
-    # strip decorators, which would resolve to the source of the decorator
-    # possibly an upstream bug in getsourcefile, bpo-1764286
-    try:
-        unwrap = inspect.unwrap
-    except AttributeError:
-        pass
-    else:
-        obj = unwrap(obj)
-
-    try:
-        fn = inspect.getsourcefile(obj)
-    except Exception:
-        fn = None
-    if not fn:
-        return
-
-    try:
-        source, lineno = inspect.getsourcelines(obj)
-    except Exception:
-        lineno = None
-
-    if lineno:
-        linespec = "#L%d-L%d" % (lineno, lineno + len(source) - 1)
-    else:
-        linespec = ""
-
-    fn = os.path.relpath(fn, start=os.path.dirname(sympy.__file__))
-    return blobpath + fn + linespec
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+import inspect
+import os
+import sys
+import time
+
+import sympy
+
+sys.path = ['ext'] + sys.path
+sys.path.extend(['..\\..\\Solverz'])
+# This command is for linux (Ubuntu 22.04.2 LTS), which cannot recognise relative path of Solverz library.
+sys.path.insert(0, os.path.abspath('../..'))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'Solverz'
+copyright = f'{time.localtime().tm_year}, Ruizhi Yu'
+author = 'Ruizhi Yu'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
+              'sphinx_math_dollar', 'sphinx.ext.mathjax', 'numpydoc',
+              'sphinx_reredirects', 'sphinx_copybutton',
+              'sphinx.ext.graphviz', 'sphinxcontrib.jquery',
+              'matplotlib.sphinxext.plot_directive', 'myst_parser',
+              'convert-svg-to-pdf', 'sphinx.ext.intersphinx', ]  # 'sphinx.ext.linkcode'
+
+# To stop docstrings inheritance.
+autodoc_inherit_docstrings = False
+
+# Sphinx是一个文档生成器，可以将Markdown或reStructuredText等文本格式转化为HTML、PDF等格式的文档。而MathJax是一个用于渲染数学公式的JavaScript库，它可以帮助将LaTeX或MathML格式的数学公式渲染为高质量的矢量图形。
+# 虽然Sphinx本身提供了一些对数学公式的支持，但其渲染效果不如MathJax优秀。因此，为了获得更好的数学公式渲染效果，使用MathJax插件可以帮助Sphinx在生成文档时自动渲染数学公式，从而提高文档的质量和可读性。
+
+templates_path = ['_templates']
+exclude_patterns = []
+
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.txt': 'markdown',
+    '.md': 'markdown',
+}
+
+mathjax3_config = {
+    "tex": {
+        "inlineMath": [['\\(', '\\)']],
+        "displayMath": [["\\[", "\\]"]],
+        'packages': {'[+]': ['physics']}
+    },
+    'loader': {'load': ['[tex]/physics']},
+}
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+
+html_static_path = ['_static']
+
+html_theme = 'furo'
+
+common_theme_variables = {
+    # Main "SymPy green" colors. Many things uses these colors.
+    "color-brand-primary": "#52833A",
+    "color-brand-content": "#307748",
+
+    # The left sidebar.
+    "color-sidebar-background": "#3B5526",
+    "color-sidebar-background-border": "var(--color-background-primary)",
+    "color-sidebar-link-text": "#FFFFFF",
+    "color-sidebar-brand-text": "var(--color-sidebar-link-text--top-level)",
+    "color-sidebar-link-text--top-level": "#FFFFFF",
+    "color-sidebar-item-background--hover": "var(--color-brand-primary)",
+    "color-sidebar-item-expander-background--hover": "var(--color-brand-primary)",
+
+    "color-link-underline--hover": "var(--color-link)",
+    "color-api-keyword": "#000000bd",
+    "color-api-name": "var(--color-brand-content)",
+    "color-api-pre-name": "var(--color-brand-content)",
+    "api-font-size": "var(--font-size--normal)",
+    "color-foreground-secondary": "#53555B",
+
+    # TODO: Add the other types of admonitions here if anyone uses them.
+    "color-admonition-title-background--seealso": "#CCCCCC",
+    "color-admonition-title--seealso": "black",
+    "color-admonition-title-background--note": "#CCCCCC",
+    "color-admonition-title--note": "black",
+    "color-admonition-title-background--warning": "var(--color-problematic)",
+    "color-admonition-title--warning": "white",
+    "admonition-font-size": "var(--font-size--normal)",
+    "admonition-title-font-size": "var(--font-size--normal)",
+
+    # Note: this doesn't work. If we want to change this, we have to set
+    # it as the .highlight background in custom.css.
+    "color-code-background": "hsl(80deg 100% 95%)",
+
+    "code-font-size": "var(--font-size--small)",
+    "font-stack--monospace": 'DejaVu Sans Mono,"SFMono-Regular",Menlo,Consolas,Monaco,Liberation Mono,Lucida Console,monospace;'
+}
+
+html_theme_options = {
+    "light_css_variables": common_theme_variables,
+    # The dark variables automatically inherit values from the light variables
+    "dark_css_variables": {
+        **common_theme_variables,
+        "color-brand-primary": "#33CB33",
+        "color-brand-content": "#1DBD1D",
+
+        "color-api-keyword": "#FFFFFFbd",
+        "color-api-overall": "#FFFFFF90",
+        "color-api-paren": "#FFFFFF90",
+
+        "color-sidebar-item-background--hover": "#52833A",
+        "color-sidebar-item-expander-background--hover": "#52833A",
+        # This is the color of the text in the right sidebar
+        "color-foreground-secondary": "#9DA1AC",
+
+        "color-admonition-title-background--seealso": "#555555",
+        "color-admonition-title-background--note": "#555555",
+        "color-problematic": "#B30000",
+    },
+    # See https://pradyunsg.me/furo/customisation/footer/
+    "footer_icons": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/smallbunnies/Solverz",
+            "html": """
+                <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 16 16">
+                    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
+                </svg>
+            """,
+            "class": "",
+        },
+    ],
+}
+
+html_css_files = ['custom.css']
+
+html_domain_indices = ['py-modindex']
+
+# Solverz logo on title page
+html_logo = '_static/sympylogo.png'
+latex_logo = '_static/sympylogo_big.png'
+html_favicon = '../_build/logo/sympy-notailtext-favicon.ico'
+
+
+def linkcode_resolve(domain, info):
+    """Determine the URL corresponding to Python object."""
+    if domain != 'py':
+        return
+
+    modname = info['module']
+    fullname = info['fullname']
+
+    submod = sys.modules.get(modname)
+    if submod is None:
+        return
+
+    obj = submod
+    for part in fullname.split('.'):
+        try:
+            obj = getattr(obj, part)
+        except Exception:
+            return
+
+    # strip decorators, which would resolve to the source of the decorator
+    # possibly an upstream bug in getsourcefile, bpo-1764286
+    try:
+        unwrap = inspect.unwrap
+    except AttributeError:
+        pass
+    else:
+        obj = unwrap(obj)
+
+    try:
+        fn = inspect.getsourcefile(obj)
+    except Exception:
+        fn = None
+    if not fn:
+        return
+
+    try:
+        source, lineno = inspect.getsourcelines(obj)
+    except Exception:
+        lineno = None
+
+    if lineno:
+        linespec = "#L%d-L%d" % (lineno, lineno + len(source) - 1)
+    else:
+        linespec = ""
+
+    fn = os.path.relpath(fn, start=os.path.dirname(sympy.__file__))
+    return blobpath + fn + linespec
```

### Comparing `solverz-0.0.1rc1/docs/src/gettingstart.md` & `solverz-0.0.1rc2/docs/src/gettingstart.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-(gettingstarted)=
-
-# Getting Started
-
-## Overview
-Solverz supports three types of equality constraints, which are respectively
-
-1. Algebraic Equations (AEs) with general formula $0=F(y,p)$
-2. Finite Difference Algebraic Equations (FDAEs) with general formula $0=F(y,p,y_0)$
-3. Differential Algebraic Equations (DAEs) with general formula $M\dot{y}=F(t,y,p)$
-
-where $y$ is the known variable, $F$ is the mapping, $p$ is the parameter set of your models, $y_0$ is the previous time node value of $y$, $M$is the singular mass matrix.
-
-If your mathematical models belong to one of the equation types above, then Solverz should be your choice, because it 
-supports an object-oriented design for the definition of these equations and can generate high-performance numerical codes. 
-
-The basic steps of a simple modeling and solution process are:
-
-1. Create model and declare components
-2. Instantiate the model and generate numerical codes
-3. Apply solver
-4. Interrogate solver results
-
-These steps and the philosophy behind Soverz are explained as follows.
-## Symbolic Modelling
-The modelling starts with declaring an empty Model with
-```python
-from Solverz import Model
-m = Model()
-```
-### Variables
-Variables represent unknown or changing parts of a model. The values taken by the variables are often referred to as a solution of the simulation. 
-In Solverz, variables can be added to the model by
-```python
-from Solverz import Var
-m.x = Var(name='x', value=[0, 1])
-m.y = Var(name='y', value=0)
-```
-We should assign two attributes to each variable, which are `name` and `value` respectively. The `name` is how variable `m.x` is represented in expressions and the `value` is the initial conditions of the `m.x`. 
-
-Solverz supports only one-dimensional variables and the length of the variables is implicitly dependent on the length of the `value` you give.
-#### Index
-Sometimes we want to access certain elements in a variable, for example, the first element of `x`, and the first to third elements of `y`. Solverz provides you with the flexibility by just calling
-```python
->>> m.x[0]
-x[0]
->>> m.y[0:3]
-y[0:3]
-```
-Currently, only `int` and `slice` indices are recommended. We are working on more complex index types such as the list. 
-Also, be careful not to exceed the maximum index that depends on the initial value you give. Otherwise, errors would be raised.
-#### Operation
-The symbolic mathematics of Solverz variables are based on [Sympy](https://www.sympy.org/en/index.html). That is, we can use the Solverz variables to perform the python operations `+`, `-`, `*`, `/`, `**`, just to name a few. 
-For example, the expressions $x_0x_1+\sin(x_2)$ can be implemented by
-```python
->>> from Solverz import Var, sin
->>> m.x = Var(name='x', value=[0, 0, 0])
->>> m.x[0]*m.x[1]+sin(m.x[2])
-x[0]*x[1] + sin(x[2])
-```
-Currently, functions like `sin`, `cos`, `Abs`, `Sign`, `exp`, just to name a few, are supported. You can refer to [api reference](https://docs.solverz.org/reference/index.html) for all supported functions and their detailed implementations.
-If you want to write your own functions, refer to [advanced usage](https://docs.solverz.org/advanced.html). And you can contact us so that we can make it a Solverz built-in funtion.
-
-A special case of Variables is the `AliasVar`, that is, the alias variables. In Solverz, the `AliasVar` is used to denote the historical value of some variable, which is useful in finite difference equations. 
-For example, one can use the following codes to declare `AliasVar`.
-```python
-from Solverz import AliasVar
-m.p = Var(name='p', value=0)
-m.p0 = AliasVar(name='p', init=m.p)
-```
-The `name` of `AliasVar` is used to denote that `m.p0` is the historical value of `m.p`. And it is initialized by `m.p`.  One can initialize the variables by assigning expressions to the `init` attribute, apart from giving the initial values.
-### Parameters
-Parameters represents the data that must be supplied to perform the simulation. Though we can use python expression `c*m.x`, where c is a number, to model the expression $cx$. But it is recommended to declare `c` as a new parameter if you want to change $c$ in simulations for different results.
-The declaration of parameters below is the same as variable declaration.
-```python
-from Solverz import Param
-m.c = Param(name='c', value=0)
-```
-The parameters can also be incorporated in operations. And it can be indexed just as the variables.
-In Solverz, it is easy to alter the parameters in simulation, which will be shown later.
-#### Parameters changing with time
-Some parameters are time-varying. For example, when simulating differential equations and the finite difference algebraic equations, you want to know the results under given boundaries. In Solverz, this is realized by using `TimeSeriesParam`.
-For example, we want the parameter `pb` to increase from 10 to 11 in the time interval [1,2]. We can do the following.
-```python
-from Solverz import TimeSeriesParam
-m.pb = TimeSeriesParam('pb',
-                       v_series=[10, 10, 11, 11],
-                       time_series=[0, 1, 2, 100])
-```
-The `v_series` and `time_series` specify the values and time nodes of the Time-series parameter. Solverz performs linear interpolation for the value of `pb` at any given $t$. If $t>100$, `pb` is assumed to be 11.
-### Equations
-Equations describe the constraints of variables. In Solverz, equations are classified into two categories:
-The basic equations 
-$0=f(y,p),$
-and the ordinary differential equation (ODE)
-$\dot{y}=f(y,p)$
-where $p$ denotes the parameters and $y$ denotes the variables.
-
-The basic equations are imposed by the `Eqn` objects. Below is the example of a `Eqn` declaration.
-```python
-from Solverz import Var, Param, Eqn, made_numerical, sin, Model, nr_method
-
-m = Model()
-m.x = Var('x', 0)
-m.t = Param('t', 0.3)
-m.x1 = Param('x1', -0.1)
-m.f = Eqn(name='f', eqn=m.x - sin(3.14 * m.x) * m.t - m.x1)
-```
-The `eqn` attribute should be the right hand size of $0=f(y,p)$.
-
-The ODEs are imposed by the `Ode` object. Below is the example of an ODE declaration.
-```python
-from Solverz import Model, Var, Ode
-
-m = Model()
-m.h = Var('h', 0)
-m.v = Var('v', 20)
-m.f1 = Ode('f1', f=m.v, diff_var=m.h)
-```
-The `f` attribute of `Ode` objects denote the right hand side of $\dot{y}=f(y,p)$ and the `diff_var` attribute denotes the left hand side
-variable.
-
-### Create Model Instance
-After adding all the elements to the `Model` object, we can create the symbolic model and the numerical variable 
-instances by calling 
-```python
-eqs, y0 = m.create_instance()
-```
-#### Symbolic Equations
-The `eqs` object is the symbolic equation, which can be either `AE`, `FDAE` or `DAE`. The type depends on the equations and variables you declare. The Solverz detects the equation and variable types, and then constructs `AE`, `FDAE` or `DAE` automatically.
-The object stores all the symbolic equations, the derivatives and the equation addresses.  Also, it can be used to check if the equation number equals the variable number, which is critical for a model to be solved.
-#### Numerical Variables
-The `y0` object is the instance of numerical variables. In Solverz, it holds the meaning of the combination of all symbolic variables `Var`. And it is used directly in simulation solutions. 
-For example, if `y0` contains variable `h` and `v`. Then we can access these variables by calling `y0['h']` and `y0['v']`. 
-If you want to set different values of `h` and `v`, you can use `y0['h']=np.array([1,2,3])`. It should be noted that the 
-new values must have the same shape compared with the original ones. 
-This is because Solverz has already allocated the addresses for the variables when creating instances.
-Moreover, by overloading operators, `y0` can be used for addition, subtraction, multiplication, and division.
-## From Symbolic to Numerical
-### Numerical Equations
-To directly use the symbolic equations for computation is too slow. Alternatively, you should use the numerical equations 
-derived by the Solverz, which are optimized for efficient simulation. 
-Specifically, Solverz prints all the symbolic expressions to well-organized python functions based on mature 
-libraries such as numpy, scipy and numba. 
-
-To derive numerical functions, just use the `made_numerical` function as follows.
-We have equation 
-$0=x-t\sin(\pi x)-x_1,$
-where $x$ is the known variabe, $t$ and $x_1$ are parameters.
-With Solverz, one has
-```python
-import numpy as np
-from Solverz import Var, Param, Eqn, made_numerical, sin, Model, nr_method, module_printer
-
-m = Model()
-m.x = Var('x', 0)
-m.t = Param('t', 0.3)
-m.x1 = Param('x1', -0.1)
-m.f = Eqn('f', m.x - sin(np.pi * m.x) * m.t - m.x1)
-sae, y0 = m.create_instance()
-ae, code = made_numerical(sae, y0, output_code=True, sparse=True)
-```
-The `ae` object is a instance of the `Solverz.nAE` class. It omit all the symbolic expressions and other redundant details, which has three attributes:
-
-1. `ae.F` that returns $F(y,p)$ if one calls `ae.F(y,p)`
-2. `ae.J` that returns  the jacobian$J(y,p)$ if one calls `ae.J(y,p)`
-3. `ae.p` that is a python dict object storing all the parameter values.
-
-In the above example, one has
-```python
->>> ae.F(y0, ae.p)
-array([0.1])
->>> ae.J(y0, ae.p).toarray()
-array([[0.0575222]])
-```
-
-One can alter the parameter values, for example to set $t=1$, by
-```python
->>> ae.p['t']=np.array([1.0])
-```
-
-You can also inspect the numerical codes generated by Solverz with
-```python
->>> print(code['F'])
-def F_(y_, p_):
-    x = y_[0:1]
-    t = p_["t"]
-    x1 = p_["x1"]
-    _F_ = zeros((1, ))
-    _F_[0:1] = -t*sin(3.14159265358979*x) - x1 + x
-    return _F_
->>> print(code['J'])
-def J_(y_, p_):
-    x = y_[0:1]
-    t = p_["t"]
-    x1 = p_["x1"]
-    row = []
-    col = []
-    data = []
-    row.extend([0])
-    col.extend(arange(0, 1))
-    data.extend(((-3.14159265358979*t*cos(3.14159265358979*x) + 1).tolist()))
-    return coo_array((data, (row,col)), (1, 1)).tocsc()
-```
-
-Similarly, `Solverz.nFDAE` and `Solverz.nDAE` are respectively the numerical equation abstraction of FDAE and DAE, with the `F` and `J` attributes being the numerical interfaces. The `Solverz.nFDAE` instance has a `nstep` attribure to denote the number of historical time steps that is required. Currently, `nstep` can only be one. 
-#### Sparse matrix
-In most cases, the Jacobian is a sparse matrix in which most of the elements are zero. 
-The sparse matrices can be decomposed very efficiently using a sparse solver. 
-It is suggested not to derive dense Jacobians because the decomposition and storage of zero elements in RAM can be very time-consuming.
-
-However, Solverz still provides both sparse and dense Jacobian options. 
-One can speficy whether to derive sparse Jacobian by setting the `sparse` argument in `made_numerical()`.
-### The Module Printer
-To model very complex systems can be slow. If one wants to avoid the repeated derivations of symbolic and numerical equations, a good way is to render an independent python module for your simulation model using `module_printer`.
-An illustrative example is
-```python
-from Solverz import Model, Var, Ode, Opt, made_numerical, Rodas, module_printer
-
-m = Model()
-m.x = Var('x', [0, 20])
-m.f1 = Ode('f1', m.x[1], m.x[0])
-m.f2 = Ode('f2', -9.8, m.x[1])
-bball, y0 = m.create_instance()
-
-pyprinter = module_printer(mdl=bball,
-                           variables=y0,
-                           name='bounceball',
-                           jit=True)
-pyprinter.render()
-```
-
-One can import the module to the codes by
-```python
-from bounceball import mdl as nbball, y as y0
-```
-
-
-The modules rendered are better optimized compared with the ones generated by `made_numerical`. In efficiency-demanding scenarios, we recommend you using the module printer. 
-### Dynamic Compilation
-The dynamic nature of Python, an interpreted-type language, brings about the efficiency decreasing compared with 
-languages like C/C++, especially in numerical computation. 
-To resolve this, Solverz uses [Numba](https://numba.pydata.org/) to accelerate your codes based on just-in-time (JIT) 
-compilation. Specifically, Numba translates Python functions to optimized machine code at runtime using the 
-industry-standard LLVM compiler library. Numba-compiled numerical algorithms in Python can approach the speeds of C or FORTRAN.
-
-If one wants to take advantage of the dynamic compilation, just set the `jit` arg in `module_printer` to be `True`. 
-Then the models will be compiled at the first time of function evaluation. 
-Though the compilation time of complex models can be of tens of minutes, the compilation results are cached locally. 
-Hence, the model should be compiled only once. 
-It is recommended to first set `jit=False` to debug the models and then perform dynamic compilation.
-Currently, dynamic compilation is not supported in `made_numerical`.
-## Solvers
-Solverz provides basic solvers for the solutions of AE, FDAE and DAE. 
-We are working hard on implementing more mature solvers. Please feel free to contact us if you have any good idea~
-
-The current solvers are summarized below. 
-### AE solvers
-
-1. `nr_method()` the Newton-Raphson method 
-2. `continuous_nr()` the continuous Newton method, which is more robust compared with the Newton-Raphson
-3. `lm()` the Levenberg-Marquardt method provided by `scipy.optimize.root`. Only dense Jacobian is allowed, which may be time-consuming.
-### FDAE solver
-`fdae_solver()`
-### DAE solvers
-
-1. `backward_euler()` the [backward Euler method](https://en.wikipedia.org/wiki/Backward_Euler_method).
-2. `implicit_trapezoid()` the [implicit trapezoidal method](https://en.wikipedia.org/wiki/Trapezoidal_rule_(differential_equations)).
-3. `Rodas()` the stiffly accurate Rosenbrock method with adaptive step size, dense output and event detection. One can use it the same as the Ode-series solvers in Matlab. This is the most stable solver in Solverz.
-
-The detailed usage of these solvers can be found in [api reference](https://docs.solverz.org/reference/index.html).
-
-It also a good idea to use solvers provided by scipy and other python packages since Solverz has derived the generic 
-numerical interfaces.
+(gettingstarted)=
+
+# Getting Started
+
+## Overview
+Solverz supports three types of equality constraints, which are respectively
+
+1. Algebraic Equations (AEs) with general formula $0=F(y,p)$
+2. Finite Difference Algebraic Equations (FDAEs) with general formula $0=F(y,p,y_0)$
+3. Differential Algebraic Equations (DAEs) with general formula $M\dot{y}=F(t,y,p)$
+
+where $y$ is the known variable, $F$ is the mapping, $p$ is the parameter set of your models, $y_0$ is the previous time node value of $y$, $M$is the singular mass matrix.
+
+If your mathematical models belong to one of the equation types above, then Solverz should be your choice, because it 
+supports an object-oriented design for the definition of these equations and can generate high-performance numerical codes. 
+
+The basic steps of a simple modeling and solution process are:
+
+1. Create model and declare components
+2. Instantiate the model and generate numerical codes
+3. Apply solver
+4. Interrogate solver results
+
+These steps and the philosophy behind Soverz are explained as follows.
+## Symbolic Modelling
+The modelling starts with declaring an empty Model with
+```python
+from Solverz import Model
+m = Model()
+```
+### Variables
+Variables represent unknown or changing parts of a model. The values taken by the variables are often referred to as a solution of the simulation. 
+In Solverz, variables can be added to the model by
+```python
+from Solverz import Var
+m.x = Var(name='x', value=[0, 1])
+m.y = Var(name='y', value=0)
+```
+We should assign two attributes to each variable, which are `name` and `value` respectively. The `name` is how variable `m.x` is represented in expressions and the `value` is the initial conditions of the `m.x`. 
+
+Solverz supports only one-dimensional variables and the length of the variables is implicitly dependent on the length of the `value` you give.
+#### Index
+Sometimes we want to access certain elements in a variable, for example, the first element of `x`, and the first to third elements of `y`. Solverz provides you with the flexibility by just calling
+```python
+>>> m.x[0]
+x[0]
+>>> m.y[0:3]
+y[0:3]
+```
+Currently, only `int` and `slice` indices are recommended. We are working on more complex index types such as the list. 
+Also, be careful not to exceed the maximum index that depends on the initial value you give. Otherwise, errors would be raised.
+#### Operation
+The symbolic mathematics of Solverz variables are based on [Sympy](https://www.sympy.org/en/index.html). That is, we can use the Solverz variables to perform the python operations `+`, `-`, `*`, `/`, `**`, just to name a few. 
+For example, the expressions $x_0x_1+\sin(x_2)$ can be implemented by
+```python
+>>> from Solverz import Var, sin
+>>> m.x = Var(name='x', value=[0, 0, 0])
+>>> m.x[0]*m.x[1]+sin(m.x[2])
+x[0]*x[1] + sin(x[2])
+```
+Currently, functions like `sin`, `cos`, `Abs`, `Sign`, `exp`, just to name a few, are supported. You can refer to [api reference](https://docs.solverz.org/reference/index.html) for all supported functions and their detailed implementations.
+If you want to write your own functions, refer to [advanced usage](https://docs.solverz.org/advanced.html). And you can contact us so that we can make it a Solverz built-in funtion.
+
+A special case of Variables is the `AliasVar`, that is, the alias variables. In Solverz, the `AliasVar` is used to denote the historical value of some variable, which is useful in finite difference equations. 
+For example, one can use the following codes to declare `AliasVar`.
+```python
+from Solverz import AliasVar
+m.p = Var(name='p', value=0)
+m.p0 = AliasVar(name='p', init=m.p)
+```
+The `name` of `AliasVar` is used to denote that `m.p0` is the historical value of `m.p`. And it is initialized by `m.p`.  One can initialize the variables by assigning expressions to the `init` attribute, apart from giving the initial values.
+### Parameters
+Parameters represents the data that must be supplied to perform the simulation. Though we can use python expression `c*m.x`, where c is a number, to model the expression $cx$. But it is recommended to declare `c` as a new parameter if you want to change $c$ in simulations for different results.
+The declaration of parameters below is the same as variable declaration.
+```python
+from Solverz import Param
+m.c = Param(name='c', value=0)
+```
+The parameters can also be incorporated in operations. And it can be indexed just as the variables.
+In Solverz, it is easy to alter the parameters in simulation, which will be shown later.
+#### Parameters changing with time
+Some parameters are time-varying. For example, when simulating differential equations and the finite difference algebraic equations, you want to know the results under given boundaries. In Solverz, this is realized by using `TimeSeriesParam`.
+For example, we want the parameter `pb` to increase from 10 to 11 in the time interval [1,2]. We can do the following.
+```python
+from Solverz import TimeSeriesParam
+m.pb = TimeSeriesParam('pb',
+                       v_series=[10, 10, 11, 11],
+                       time_series=[0, 1, 2, 100])
+```
+The `v_series` and `time_series` specify the values and time nodes of the Time-series parameter. Solverz performs linear interpolation for the value of `pb` at any given $t$. If $t>100$, `pb` is assumed to be 11.
+### Equations
+Equations describe the constraints of variables. In Solverz, equations are classified into two categories:
+The basic equations 
+$0=f(y,p),$
+and the ordinary differential equation (ODE)
+$\dot{y}=f(y,p)$
+where $p$ denotes the parameters and $y$ denotes the variables.
+
+The basic equations are imposed by the `Eqn` objects. Below is the example of a `Eqn` declaration.
+```python
+from Solverz import Var, Param, Eqn, made_numerical, sin, Model, nr_method
+
+m = Model()
+m.x = Var('x', 0)
+m.t = Param('t', 0.3)
+m.x1 = Param('x1', -0.1)
+m.f = Eqn(name='f', eqn=m.x - sin(3.14 * m.x) * m.t - m.x1)
+```
+The `eqn` attribute should be the right hand size of $0=f(y,p)$.
+
+The ODEs are imposed by the `Ode` object. Below is the example of an ODE declaration.
+```python
+from Solverz import Model, Var, Ode
+
+m = Model()
+m.h = Var('h', 0)
+m.v = Var('v', 20)
+m.f1 = Ode('f1', f=m.v, diff_var=m.h)
+```
+The `f` attribute of `Ode` objects denote the right hand side of $\dot{y}=f(y,p)$ and the `diff_var` attribute denotes the left hand side
+variable.
+
+### Create Model Instance
+After adding all the elements to the `Model` object, we can create the symbolic model and the numerical variable 
+instances by calling 
+```python
+eqs, y0 = m.create_instance()
+```
+#### Symbolic Equations
+The `eqs` object is the symbolic equation, which can be either `AE`, `FDAE` or `DAE`. The type depends on the equations and variables you declare. The Solverz detects the equation and variable types, and then constructs `AE`, `FDAE` or `DAE` automatically.
+The object stores all the symbolic equations, the derivatives and the equation addresses.  Also, it can be used to check if the equation number equals the variable number, which is critical for a model to be solved.
+#### Numerical Variables
+The `y0` object is the instance of numerical variables. In Solverz, it holds the meaning of the combination of all symbolic variables `Var`. And it is used directly in simulation solutions. 
+For example, if `y0` contains variable `h` and `v`. Then we can access these variables by calling `y0['h']` and `y0['v']`. 
+If you want to set different values of `h` and `v`, you can use `y0['h']=np.array([1,2,3])`. It should be noted that the 
+new values must have the same shape compared with the original ones. 
+This is because Solverz has already allocated the addresses for the variables when creating instances.
+Moreover, by overloading operators, `y0` can be used for addition, subtraction, multiplication, and division.
+## From Symbolic to Numerical
+### Numerical Equations
+To directly use the symbolic equations for computation is too slow. Alternatively, you should use the numerical equations 
+derived by the Solverz, which are optimized for efficient simulation. 
+Specifically, Solverz prints all the symbolic expressions to well-organized python functions based on mature 
+libraries such as numpy, scipy and numba. 
+
+To derive numerical functions, just use the `made_numerical` function as follows.
+We have equation 
+$0=x-t\sin(\pi x)-x_1,$
+where $x$ is the known variabe, $t$ and $x_1$ are parameters.
+With Solverz, one has
+```python
+import numpy as np
+from Solverz import Var, Param, Eqn, made_numerical, sin, Model, nr_method, module_printer
+
+m = Model()
+m.x = Var('x', 0)
+m.t = Param('t', 0.3)
+m.x1 = Param('x1', -0.1)
+m.f = Eqn('f', m.x - sin(np.pi * m.x) * m.t - m.x1)
+sae, y0 = m.create_instance()
+ae, code = made_numerical(sae, y0, output_code=True, sparse=True)
+```
+The `ae` object is a instance of the `Solverz.nAE` class. It omit all the symbolic expressions and other redundant details, which has three attributes:
+
+1. `ae.F` that returns $F(y,p)$ if one calls `ae.F(y,p)`
+2. `ae.J` that returns  the jacobian$J(y,p)$ if one calls `ae.J(y,p)`
+3. `ae.p` that is a python dict object storing all the parameter values.
+
+In the above example, one has
+```python
+>>> ae.F(y0, ae.p)
+array([0.1])
+>>> ae.J(y0, ae.p).toarray()
+array([[0.0575222]])
+```
+
+One can alter the parameter values, for example to set $t=1$, by
+```python
+>>> ae.p['t']=np.array([1.0])
+```
+
+You can also inspect the numerical codes generated by Solverz with
+```python
+>>> print(code['F'])
+def F_(y_, p_):
+    x = y_[0:1]
+    t = p_["t"]
+    x1 = p_["x1"]
+    _F_ = zeros((1, ))
+    _F_[0:1] = -t*sin(3.14159265358979*x) - x1 + x
+    return _F_
+>>> print(code['J'])
+def J_(y_, p_):
+    x = y_[0:1]
+    t = p_["t"]
+    x1 = p_["x1"]
+    row = []
+    col = []
+    data = []
+    row.extend([0])
+    col.extend(arange(0, 1))
+    data.extend(((-3.14159265358979*t*cos(3.14159265358979*x) + 1).tolist()))
+    return coo_array((data, (row,col)), (1, 1)).tocsc()
+```
+
+Similarly, `Solverz.nFDAE` and `Solverz.nDAE` are respectively the numerical equation abstraction of FDAE and DAE, with the `F` and `J` attributes being the numerical interfaces. The `Solverz.nFDAE` instance has a `nstep` attribure to denote the number of historical time steps that is required. Currently, `nstep` can only be one. 
+#### Sparse matrix
+In most cases, the Jacobian is a sparse matrix in which most of the elements are zero. 
+The sparse matrices can be decomposed very efficiently using a sparse solver. 
+It is suggested not to derive dense Jacobians because the decomposition and storage of zero elements in RAM can be very time-consuming.
+
+However, Solverz still provides both sparse and dense Jacobian options. 
+One can speficy whether to derive sparse Jacobian by setting the `sparse` argument in `made_numerical()`.
+### The Module Printer
+To model very complex systems can be slow. If one wants to avoid the repeated derivations of symbolic and numerical equations, a good way is to render an independent python module for your simulation model using `module_printer`.
+An illustrative example is
+```python
+from Solverz import Model, Var, Ode, Opt, made_numerical, Rodas, module_printer
+
+m = Model()
+m.x = Var('x', [0, 20])
+m.f1 = Ode('f1', m.x[1], m.x[0])
+m.f2 = Ode('f2', -9.8, m.x[1])
+bball, y0 = m.create_instance()
+
+pyprinter = module_printer(mdl=bball,
+                           variables=y0,
+                           name='bounceball',
+                           jit=True)
+pyprinter.render()
+```
+
+One can import the module to the codes by
+```python
+from bounceball import mdl as nbball, y as y0
+```
+
+
+The modules rendered are better optimized compared with the ones generated by `made_numerical`. In efficiency-demanding scenarios, we recommend you using the module printer. 
+### Dynamic Compilation
+The dynamic nature of Python, an interpreted-type language, brings about the efficiency decreasing compared with 
+languages like C/C++, especially in numerical computation. 
+To resolve this, Solverz uses [Numba](https://numba.pydata.org/) to accelerate your codes based on just-in-time (JIT) 
+compilation. Specifically, Numba translates Python functions to optimized machine code at runtime using the 
+industry-standard LLVM compiler library. Numba-compiled numerical algorithms in Python can approach the speeds of C or FORTRAN.
+
+If one wants to take advantage of the dynamic compilation, just set the `jit` arg in `module_printer` to be `True`. 
+Then the models will be compiled at the first time of function evaluation. 
+Though the compilation time of complex models can be of tens of minutes, the compilation results are cached locally. 
+Hence, the model should be compiled only once. 
+It is recommended to first set `jit=False` to debug the models and then perform dynamic compilation.
+Currently, dynamic compilation is not supported in `made_numerical`.
+## Solvers
+Solverz provides basic solvers for the solutions of AE, FDAE and DAE. 
+We are working hard on implementing more mature solvers. Please feel free to contact us if you have any good idea~
+
+The current solvers are summarized below. 
+### AE solvers
+
+1. `nr_method()` the Newton-Raphson method 
+2. `continuous_nr()` the continuous Newton method, which is more robust compared with the Newton-Raphson
+3. `lm()` the Levenberg-Marquardt method provided by `scipy.optimize.root`. Only dense Jacobian is allowed, which may be time-consuming.
+### FDAE solver
+`fdae_solver()`
+### DAE solvers
+
+1. `backward_euler()` the [backward Euler method](https://en.wikipedia.org/wiki/Backward_Euler_method).
+2. `implicit_trapezoid()` the [implicit trapezoidal method](https://en.wikipedia.org/wiki/Trapezoidal_rule_(differential_equations)).
+3. `Rodas()` the stiffly accurate Rosenbrock method with adaptive step size, dense output and event detection. One can use it the same as the Ode-series solvers in Matlab. This is the most stable solver in Solverz.
+
+The detailed usage of these solvers can be found in [api reference](https://docs.solverz.org/reference/index.html).
+
+It also a good idea to use solvers provided by scipy and other python packages since Solverz has derived the generic 
+numerical interfaces.
```

### Comparing `solverz-0.0.1rc1/docs/src/intro.md` & `solverz-0.0.1rc2/docs/src/intro.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-(intro)=
-
-# An Introductory Example
-
-Solverz aims to help you model and solve your equations more efficiently.
-
-Solverz supports three types of abstract equation types, that are
-
-- Algebraic Equations (AEs) $0=F(y,p)$
-- Finite Difference Algebraic Equations (FDAEs) $0=F(y,p,y_0)$
-- Differential Algebraic Equations (DAEs) $M\dot{y}=F(t,y,p)$
-
-where $p$ is the parameter set of your models, $y_0$ is the previous time node value of $y$.
-
-Say, we want to know how long it takes for an apple to fall from a tree to the ground. We have the 
-differential equations 
-
-```{math}
-\left\{
-\begin{aligned}
-&v'=-9.8\\
-&h'=v
-\end{aligned}
-\right.
-```
-
-with $v(0)=20$ and $h(0)=0$, we can just type the codes
-
-```python
-import matplotlib.pyplot as plt
-import numpy as np
-from Solverz import Model, Var, Ode, Opt, made_numerical, Rodas
-
-# Declare a simulation model
-m = Model()
-# Declare variables and equations
-m.h = Var('h', 0)
-m.v = Var('v', 20)
-m.f1 = Ode('f1', f=m.v, diff_var=m.h)
-m.f2 = Ode('f2', f=-9.8, diff_var=m.v)
-# Create the symbolic equation instance and the variable combination 
-bball, y0 = m.create_instance()
-# Transform symbolic equations to python numerical functions.
-nbball = made_numerical(bball, y0, sparse=True)
-
-# Define events, that is,  if the apple hits the ground then the simulation will cease.
-def events(t, y):
-    value = np.array([y[0]]) 
-    isterminal = np.array([1]) 
-    direction = np.array([-1]) 
-    return value, isterminal, direction
-
-# Solve the DAE
-sol = Rodas(nbball,
-            np.linspace(0, 30, 100), 
-            y0, 
-            Opt(event=events))
-
-# Visualize
-plt.plot(sol.T, sol.Y['h'][:, 0])
-plt.xlabel('Time/s')
-plt.ylabel('h/m')
-plt.show()
-```
-Then we have
-
-![image.png](/pics/res.png)
-
-The model is solved with the stiffly accurate Rosenbrock type method, but you can also write your own solvers by the 
-generated numerical interfaces. For example, the [multidimensional Newton method](https://en.wikipedia.org/wiki/Newton%27s_method) of 
-AEs is a scheme with formulae
-
-```{math}
-y_{k+1} = y_k - J_F(y_k)^{-1}F(y_k)\quad k=0,1,2,\cdots.
-```
-
-Its implementation using Solverz can be as simple as
-```python
-# main loop
-while max(abs(df)) > tol:
-    ite = ite + 1
-    y = y - solve(eqn.J(y, p), df)
-    df = eqn.F(y, p)
-    if ite >= 100:
-        print(f"Cannot converge within 100 iterations. Deviation: {max(abs(df))}!")
-        break
-```
-The numerical AE object `eqn` provides the $F(t,y,p)$ interface and its Jacobian $J(t,y,p)$, which grants
-your full flexibility. So that the implementation of the NR solver just resembles the formulae above.
-
-Sometimes you have very complex models and you dont want to re-derive them everytime. With Solverz, you can just use
-```python
-from Solverz import module_printer
-
-pyprinter = module_printer(bball,
-                           y0,
-                           'bounceball',
-                           jit=True)
-pyprinter.render()
-```
-to generate an independent python module of your simulation models. You can import them to your .py file by
-
-```python
-from bounceball import mdl as nbball, y as y0
-```
+(intro)=
+
+# An Introductory Example
+
+Solverz aims to help you model and solve your equations more efficiently.
+
+Solverz supports three types of abstract equation types, that are
+
+- Algebraic Equations (AEs) $0=F(y,p)$
+- Finite Difference Algebraic Equations (FDAEs) $0=F(y,p,y_0)$
+- Differential Algebraic Equations (DAEs) $M\dot{y}=F(t,y,p)$
+
+where $p$ is the parameter set of your models, $y_0$ is the previous time node value of $y$.
+
+Say, we want to know how long it takes for an apple to fall from a tree to the ground. We have the 
+differential equations 
+
+```{math}
+\left\{
+\begin{aligned}
+&v'=-9.8\\
+&h'=v
+\end{aligned}
+\right.
+```
+
+with $v(0)=20$ and $h(0)=0$, we can just type the codes
+
+```python
+import matplotlib.pyplot as plt
+import numpy as np
+from Solverz import Model, Var, Ode, Opt, made_numerical, Rodas
+
+# Declare a simulation model
+m = Model()
+# Declare variables and equations
+m.h = Var('h', 0)
+m.v = Var('v', 20)
+m.f1 = Ode('f1', f=m.v, diff_var=m.h)
+m.f2 = Ode('f2', f=-9.8, diff_var=m.v)
+# Create the symbolic equation instance and the variable combination 
+bball, y0 = m.create_instance()
+# Transform symbolic equations to python numerical functions.
+nbball = made_numerical(bball, y0, sparse=True)
+
+# Define events, that is,  if the apple hits the ground then the simulation will cease.
+def events(t, y):
+    value = np.array([y[0]]) 
+    isterminal = np.array([1]) 
+    direction = np.array([-1]) 
+    return value, isterminal, direction
+
+# Solve the DAE
+sol = Rodas(nbball,
+            np.linspace(0, 30, 100), 
+            y0, 
+            Opt(event=events))
+
+# Visualize
+plt.plot(sol.T, sol.Y['h'][:, 0])
+plt.xlabel('Time/s')
+plt.ylabel('h/m')
+plt.show()
+```
+Then we have
+
+![image.png](/pics/res.png)
+
+The model is solved with the stiffly accurate Rosenbrock type method, but you can also write your own solvers by the 
+generated numerical interfaces. For example, the [multidimensional Newton method](https://en.wikipedia.org/wiki/Newton%27s_method) of 
+AEs is a scheme with formulae
+
+```{math}
+y_{k+1} = y_k - J_F(y_k)^{-1}F(y_k)\quad k=0,1,2,\cdots.
+```
+
+Its implementation using Solverz can be as simple as
+```python
+# main loop
+while max(abs(df)) > tol:
+    ite = ite + 1
+    y = y - solve(eqn.J(y, p), df)
+    df = eqn.F(y, p)
+    if ite >= 100:
+        print(f"Cannot converge within 100 iterations. Deviation: {max(abs(df))}!")
+        break
+```
+The numerical AE object `eqn` provides the $F(t,y,p)$ interface and its Jacobian $J(t,y,p)$, which grants
+your full flexibility. So that the implementation of the NR solver just resembles the formulae above.
+
+Sometimes you have very complex models and you dont want to re-derive them everytime. With Solverz, you can just use
+```python
+from Solverz import module_printer
+
+pyprinter = module_printer(bball,
+                           y0,
+                           'bounceball',
+                           jit=True)
+pyprinter.render()
+```
+to generate an independent python module of your simulation models. You can import them to your .py file by
+
+```python
+from bounceball import mdl as nbball, y as y0
+```
```

### Comparing `solverz-0.0.1rc1/docs/src/_static/sympylogo.png` & `solverz-0.0.1rc2/docs/src/_static/sympylogo.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/docs/src/_static/sympylogo_big.png` & `solverz-0.0.1rc2/docs/src/_static/sympylogo_big.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/docs/src/pics/Hierarchy_of_equations.png` & `solverz-0.0.1rc2/docs/src/pics/Hierarchy_of_equations.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/docs/src/pics/difference_stencil.png` & `solverz-0.0.1rc2/docs/src/pics/difference_stencil.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/docs/src/pics/res.png` & `solverz-0.0.1rc2/docs/src/pics/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/docs/src/reference/index.rst` & `solverz-0.0.1rc2/docs/src/reference/index.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-.. _reference:
-
-=============
-API Reference
-=============
-
-Functions
----------
-
-.. autoclass:: Solverz.sym_algebra.functions.sin
-
-.. autoclass:: Solverz.sym_algebra.functions.cos
-
-.. autoclass:: Solverz.sym_algebra.functions.exp
-
-.. autoclass:: Solverz.sym_algebra.functions.Abs
-
-.. autoclass:: Solverz.sym_algebra.functions.Sign
-
-.. autoclass:: Solverz.sym_algebra.functions.AntiWindUp
-
-.. autoclass:: Solverz.sym_algebra.functions.Min
-
-.. autoclass:: Solverz.sym_algebra.functions.Saturation
-
-Solvers
--------
-
-AE solver
-=========
-
-.. autofunction:: Solverz.solvers.nlaesolver.nr.nr_method
-
-.. autofunction:: Solverz.solvers.nlaesolver.cnr.continuous_nr
-
-.. autofunction:: Solverz.solvers.nlaesolver.lm.lm
-
-FDAE solver
-===========
-
-.. autofunction:: Solverz.solvers.fdesolver.fdae_solver
-
-DAE solver
-==========
-
-.. autofunction:: Solverz.solvers.daesolver.beuler.backward_euler
-
-.. autofunction:: Solverz.solvers.daesolver.trapezoidal.implicit_trapezoid
-
-.. autofunction:: Solverz.solvers.daesolver.rodas.Rodas
+.. _reference:
+
+=============
+API Reference
+=============
+
+Functions
+---------
+
+.. autoclass:: Solverz.sym_algebra.functions.sin
+
+.. autoclass:: Solverz.sym_algebra.functions.cos
+
+.. autoclass:: Solverz.sym_algebra.functions.exp
+
+.. autoclass:: Solverz.sym_algebra.functions.Abs
+
+.. autoclass:: Solverz.sym_algebra.functions.Sign
+
+.. autoclass:: Solverz.sym_algebra.functions.AntiWindUp
+
+.. autoclass:: Solverz.sym_algebra.functions.Min
+
+.. autoclass:: Solverz.sym_algebra.functions.Saturation
+
+Solvers
+-------
+
+AE solver
+=========
+
+.. autofunction:: Solverz.solvers.nlaesolver.nr.nr_method
+
+.. autofunction:: Solverz.solvers.nlaesolver.cnr.continuous_nr
+
+.. autofunction:: Solverz.solvers.nlaesolver.lm.lm
+
+FDAE solver
+===========
+
+.. autofunction:: Solverz.solvers.fdesolver.fdae_solver
+
+DAE solver
+==========
+
+.. autofunction:: Solverz.solvers.daesolver.beuler.backward_euler
+
+.. autofunction:: Solverz.solvers.daesolver.trapezoidal.implicit_trapezoid
+
+.. autofunction:: Solverz.solvers.daesolver.rodas.Rodas
```

### Comparing `solverz-0.0.1rc1/instances/4node3pipe.xlsx` & `solverz-0.0.1rc2/instances/4node3pipe.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/4node3pipe_bench.xlsx` & `solverz-0.0.1rc2/instances/4node3pipe_bench.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/4node3pipe_change_sign.xlsx` & `solverz-0.0.1rc2/instances/4node3pipe_change_sign.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/4node3pipe_change_sign_bench.xlsx` & `solverz-0.0.1rc2/instances/4node3pipe_change_sign_bench.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/dae_test.xlsx` & `solverz-0.0.1rc2/instances/dae_test.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/dynamic_gas_flow_single_pipe.xlsx` & `solverz-0.0.1rc2/instances/dynamic_gas_flow_single_pipe.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/ode_test.xlsx` & `solverz-0.0.1rc2/instances/ode_test.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/test_burger.xlsx` & `solverz-0.0.1rc2/instances/test_burger.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/test_m3b9.xlsx` & `solverz-0.0.1rc2/instances/test_m3b9.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/test_ode45.xlsx` & `solverz-0.0.1rc2/instances/test_ode45.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/instances/test_sirk.xlsx` & `solverz-0.0.1rc2/instances/test_sirk.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc1/tests/test_dhspf.py` & `solverz-0.0.1rc2/tests/test_dhspf.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# import pandas as pd
-# import numpy as np
-#
-# from Solverz import Eqn, AE, nr_method, as_Vars, iVar, Para, idx, Abs, exp, Mat_Mul, made_numerical, Param, IdxParam
-#
-# # %% initialize variables and params
-# sys_df = pd.read_excel('instances/4node3pipe.xlsx',
-#                        sheet_name=None,
-#                        engine='openpyxl',
-#                        index_col=0
-#                        )
-#
-#
-# def derive_incidence_matrix(f_node, t_node):
-#     V = np.zeros((max(max(f_node), max(t_node)) + 1, len(f_node)))
-#     for pipe in range(len(f_node)):
-#         V[f_node[pipe], pipe] = -1
-#         V[t_node[pipe], pipe] = 1
-#     return V
-#
-#
-# def derive_v_plus(v: np.ndarray) -> np.ndarray:
-#     return (v + np.abs(v)) / 2
-#
-#
-# def derive_v_minus(v: np.ndarray) -> np.ndarray:
-#     return (v - np.abs(v)) / 2
-#
-#
-# # %% md
-# # Declare equations and parameters
-# # %%
-# Node = sys_df['Node']
-# i = idx(name='i', value=np.asarray(Node['type'][Node['type'] == 3].index))  # intermediate nodes
-# l = idx(name='l', value=np.asarray(Node['type'][Node['type'] == 2].index))  # load nodes
-# s = idx(name='s', value=np.asarray(Node['type'][Node['type'] == 1].index))  # non-balance source nodes
-# r = idx(name='r', value=np.asarray(Node['type'][Node['type'] == 0].index))  # balance source nodes
-# sl = idx(name='sl', value=np.concatenate((s.value, l.value)))
-# rs = idx(name='rs', value=np.concatenate((r.value, s.value)))
-# rsl = idx(name='rsl', value=np.concatenate((r.value, s.value, l.value)))
-# li = idx(name='li', value=np.concatenate((l.value, i.value)))
-# rsi = idx(name='rsi', value=np.concatenate((r.value, s.value, i.value)))
-#
-# mL = Para('mL', dim=2, value=np.asarray(sys_df['m_L']))
-# K = Para(name='K', value=np.asarray(sys_df['K']).reshape(-1, ))
-# Ts_set = Para(name='Ts_set', value=np.asarray(sys_df['Ts_set']).reshape(-1, ))
-# Tr_set = Para(name='Tr_set', value=np.asarray(sys_df['Tr_set']).reshape(-1, ))
-# phi_set = Para(name='phi_set', value=np.asarray(sys_df['phi_set']).reshape(-1, ))
-#
-# Cp = Para(name='Cp', value=np.asarray(sys_df['Cp']).reshape(-1, ))
-# L = Para(name='L', value=np.asarray(sys_df['L']).reshape(-1, ))
-# coeff_lambda = Para(name='coeff_lambda', value=np.asarray(sys_df['coeff_lambda']).reshape(-1, ))
-# Ta = Para(name='Ta', value=np.asarray(sys_df['Ta']).reshape(-1, ))
-# f_node = sys_df['Pipe']['f_node']
-# t_node = sys_df['Pipe']['t_node']
-# V = Para(name='V', dim=2, value=derive_incidence_matrix(f_node, t_node))
-# Vp = Para(name='Vp', dim=2, value=derive_v_plus(V.value))
-# Vm = Para(name='Vm', dim=2, value=derive_v_minus(V.value))
-# f_node = idx(name='f_node', value=np.asarray(f_node).reshape(-1, ))  # intermediate nodes
-# t_node = idx(name='t_node', value=np.asarray(t_node).reshape(-1, ))  # load nodes
-#
-# m = iVar(name='m', value=np.asarray(sys_df['var']['m']))
-# mq = iVar(name='mq', value=np.asarray(sys_df['var']['mq']))
-# Ts = iVar(name='Ts', value=np.asarray(sys_df['var']['Ts']))
-# Tr = iVar(name='Tr', value=np.asarray(sys_df['var']['Tr']))
-# Touts = iVar(name='Touts', value=np.asarray(sys_df['var']['Touts']))
-# Toutr = iVar(name='Toutr', value=np.asarray(sys_df['var']['Toutr']))
-# phi = iVar(name='phi', value=np.asarray(sys_df['var']['phi']))
-#
-# E1 = Eqn(name='E1', eqn=(Ts[f_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Touts)
-# E3 = Eqn(name='E3', eqn=(Tr[t_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Toutr)
-# E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) + mq[rs])
-# E6 = Eqn(name='E6', eqn=Mat_Mul(V[l, :], m) - mq[l])
-# E7 = Eqn(name='E7', eqn=Mat_Mul(V[i, :], m))
-# E8 = Eqn(name='E8', eqn=Mat_Mul(mL, K * Abs(m) * m))
-# E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], Touts * Abs(m)))
-# E10 = Eqn(name='E10', eqn=Tr[rsi] * Mat_Mul(Vm[rsi, :], Abs(m)) - Mat_Mul(Vm[rsi, :], Toutr * Abs(m)))
-# E11 = Eqn(name='E11', eqn=phi[rsl] - 4182 * mq[rsl] * (Ts[rsl] - Tr[rsl]))
-# E12 = Eqn(name='E12', eqn=Ts[rs] - Ts_set)
-# E13 = Eqn(name='E13', eqn=Tr[l] - Tr_set)
-# E14 = Eqn(name='E14', eqn=phi[sl] - phi_set)
-# E15 = Eqn(name='E15', eqn=phi[i])
-# E16 = Eqn(name='E16', eqn=mq[i])
-# E = AE(name='Pipe Equations', eqn=[E1, E3, E5, E6, E7, E8, E9, E10, E11, E12, E13, E14, E15, E16])
-# y0 = as_Vars([m, mq, Ts, Tr, Touts, Toutr, phi])
-#
-# nE, code = made_numerical(E, y0, output_code=True)
-#
-# sol = nr_method(nE, y0)
-# # y_cnr, ite = continuous_nr(nE, y0.array)
-#
-#
-# sys_df = pd.read_excel('instances/4node3pipe_bench.xlsx',
-#                        sheet_name=None,
-#                        engine='openpyxl',
-#                        header=None
-#                        )
-#
-#
-# def test_nr_method():
-#     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
-#         # find nonzero elements
-#         idx_nonzero = np.nonzero(sol.y[var_name])
-#         assert max(abs((sol.y[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) /
-#                    np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) <= 1e-8
-#
-# # def test_cnr_method():
-# #     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
-# #         # find nonzero elements
-# #         idx_nonzero = np.nonzero(y_cnr[var_name])
-# #         assert max(abs((y_cnr[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) /
-# #                        np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) <= 1e-8
+# import pandas as pd
+# import numpy as np
+#
+# from Solverz import Eqn, AE, nr_method, as_Vars, iVar, Para, idx, Abs, exp, Mat_Mul, made_numerical, Param, IdxParam
+#
+# # %% initialize variables and params
+# sys_df = pd.read_excel('instances/4node3pipe.xlsx',
+#                        sheet_name=None,
+#                        engine='openpyxl',
+#                        index_col=0
+#                        )
+#
+#
+# def derive_incidence_matrix(f_node, t_node):
+#     V = np.zeros((max(max(f_node), max(t_node)) + 1, len(f_node)))
+#     for pipe in range(len(f_node)):
+#         V[f_node[pipe], pipe] = -1
+#         V[t_node[pipe], pipe] = 1
+#     return V
+#
+#
+# def derive_v_plus(v: np.ndarray) -> np.ndarray:
+#     return (v + np.abs(v)) / 2
+#
+#
+# def derive_v_minus(v: np.ndarray) -> np.ndarray:
+#     return (v - np.abs(v)) / 2
+#
+#
+# # %% md
+# # Declare equations and parameters
+# # %%
+# Node = sys_df['Node']
+# i = idx(name='i', value=np.asarray(Node['type'][Node['type'] == 3].index))  # intermediate nodes
+# l = idx(name='l', value=np.asarray(Node['type'][Node['type'] == 2].index))  # load nodes
+# s = idx(name='s', value=np.asarray(Node['type'][Node['type'] == 1].index))  # non-balance source nodes
+# r = idx(name='r', value=np.asarray(Node['type'][Node['type'] == 0].index))  # balance source nodes
+# sl = idx(name='sl', value=np.concatenate((s.value, l.value)))
+# rs = idx(name='rs', value=np.concatenate((r.value, s.value)))
+# rsl = idx(name='rsl', value=np.concatenate((r.value, s.value, l.value)))
+# li = idx(name='li', value=np.concatenate((l.value, i.value)))
+# rsi = idx(name='rsi', value=np.concatenate((r.value, s.value, i.value)))
+#
+# mL = Para('mL', dim=2, value=np.asarray(sys_df['m_L']))
+# K = Para(name='K', value=np.asarray(sys_df['K']).reshape(-1, ))
+# Ts_set = Para(name='Ts_set', value=np.asarray(sys_df['Ts_set']).reshape(-1, ))
+# Tr_set = Para(name='Tr_set', value=np.asarray(sys_df['Tr_set']).reshape(-1, ))
+# phi_set = Para(name='phi_set', value=np.asarray(sys_df['phi_set']).reshape(-1, ))
+#
+# Cp = Para(name='Cp', value=np.asarray(sys_df['Cp']).reshape(-1, ))
+# L = Para(name='L', value=np.asarray(sys_df['L']).reshape(-1, ))
+# coeff_lambda = Para(name='coeff_lambda', value=np.asarray(sys_df['coeff_lambda']).reshape(-1, ))
+# Ta = Para(name='Ta', value=np.asarray(sys_df['Ta']).reshape(-1, ))
+# f_node = sys_df['Pipe']['f_node']
+# t_node = sys_df['Pipe']['t_node']
+# V = Para(name='V', dim=2, value=derive_incidence_matrix(f_node, t_node))
+# Vp = Para(name='Vp', dim=2, value=derive_v_plus(V.value))
+# Vm = Para(name='Vm', dim=2, value=derive_v_minus(V.value))
+# f_node = idx(name='f_node', value=np.asarray(f_node).reshape(-1, ))  # intermediate nodes
+# t_node = idx(name='t_node', value=np.asarray(t_node).reshape(-1, ))  # load nodes
+#
+# m = iVar(name='m', value=np.asarray(sys_df['var']['m']))
+# mq = iVar(name='mq', value=np.asarray(sys_df['var']['mq']))
+# Ts = iVar(name='Ts', value=np.asarray(sys_df['var']['Ts']))
+# Tr = iVar(name='Tr', value=np.asarray(sys_df['var']['Tr']))
+# Touts = iVar(name='Touts', value=np.asarray(sys_df['var']['Touts']))
+# Toutr = iVar(name='Toutr', value=np.asarray(sys_df['var']['Toutr']))
+# phi = iVar(name='phi', value=np.asarray(sys_df['var']['phi']))
+#
+# E1 = Eqn(name='E1', eqn=(Ts[f_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Touts)
+# E3 = Eqn(name='E3', eqn=(Tr[t_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Toutr)
+# E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) + mq[rs])
+# E6 = Eqn(name='E6', eqn=Mat_Mul(V[l, :], m) - mq[l])
+# E7 = Eqn(name='E7', eqn=Mat_Mul(V[i, :], m))
+# E8 = Eqn(name='E8', eqn=Mat_Mul(mL, K * Abs(m) * m))
+# E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], Touts * Abs(m)))
+# E10 = Eqn(name='E10', eqn=Tr[rsi] * Mat_Mul(Vm[rsi, :], Abs(m)) - Mat_Mul(Vm[rsi, :], Toutr * Abs(m)))
+# E11 = Eqn(name='E11', eqn=phi[rsl] - 4182 * mq[rsl] * (Ts[rsl] - Tr[rsl]))
+# E12 = Eqn(name='E12', eqn=Ts[rs] - Ts_set)
+# E13 = Eqn(name='E13', eqn=Tr[l] - Tr_set)
+# E14 = Eqn(name='E14', eqn=phi[sl] - phi_set)
+# E15 = Eqn(name='E15', eqn=phi[i])
+# E16 = Eqn(name='E16', eqn=mq[i])
+# E = AE(name='Pipe Equations', eqn=[E1, E3, E5, E6, E7, E8, E9, E10, E11, E12, E13, E14, E15, E16])
+# y0 = as_Vars([m, mq, Ts, Tr, Touts, Toutr, phi])
+#
+# nE, code = made_numerical(E, y0, output_code=True)
+#
+# sol = nr_method(nE, y0)
+# # y_cnr, ite = continuous_nr(nE, y0.array)
+#
+#
+# sys_df = pd.read_excel('instances/4node3pipe_bench.xlsx',
+#                        sheet_name=None,
+#                        engine='openpyxl',
+#                        header=None
+#                        )
+#
+#
+# def test_nr_method():
+#     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
+#         # find nonzero elements
+#         idx_nonzero = np.nonzero(sol.y[var_name])
+#         assert max(abs((sol.y[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) /
+#                    np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) <= 1e-8
+#
+# # def test_cnr_method():
+# #     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
+# #         # find nonzero elements
+# #         idx_nonzero = np.nonzero(y_cnr[var_name])
+# #         assert max(abs((y_cnr[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) /
+# #                        np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) <= 1e-8
```

### Comparing `solverz-0.0.1rc1/tests/test_dhspf_change_sign.py` & `solverz-0.0.1rc2/tests/test_dhspf_change_sign.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-# import pandas as pd
-# import numpy as np
-# from functools import partial
-#
-# from Solverz import Eqn, AE, nr_method, as_Vars, iVar, Param, continuous_nr, Para, idx, Abs, exp, Mat_Mul, \
-#     made_numerical
-#
-# # %% initialize variables and params
-# sys_df = pd.read_excel('instances/4node3pipe_change_sign.xlsx',
-#                        sheet_name=None,
-#                        engine='openpyxl',
-#                        index_col=0
-#                        )
-#
-#
-# def derive_incidence_matrix(f_node, t_node):
-#     V = np.zeros((max(max(f_node), max(t_node)) + 1, len(f_node)))
-#     for pipe in range(len(f_node)):
-#         V[f_node[pipe], pipe] = -1
-#         V[t_node[pipe], pipe] = 1
-#     return V
-#
-#
-# def derive_v_plus(v: np.ndarray) -> np.ndarray:
-#     return (v + np.abs(v)) / 2
-#
-#
-# def derive_v_minus(v: np.ndarray) -> np.ndarray:
-#     return (v - np.abs(v)) / 2
-#
-#
-# def v_p_reverse_pipe(V0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
-#     """
-#     Trigger function of v_p
-#     if some element of m changes its sign, then related column of V0 changes its sign
-#     :param V0:
-#     :param m0: initial mass flow rate
-#     :param m:
-#     :return: $V_0*(I-diag(sign(m0)-sign(m)))$
-#     """
-#     # pipe i changes sign then m_sign[i]=2
-#     m_sign = np.abs(np.sign(m0) - np.sign(m))
-#     return derive_v_plus(V0 @ (np.eye(m.shape[0]) - np.diagflat(m_sign)))
-#
-#
-# def v_m_reverse_pipe(V0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
-#     # pipe i changes sign then m_sign[i]=2
-#     m_sign = np.abs(np.sign(m0) - np.sign(m))
-#     return derive_v_minus(V0 @ (np.eye(m.shape[0]) - np.diagflat(np.abs(m_sign))))
-#
-#
-# def f_node_calculator(f_node0: np.ndarray, t_node0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
-#     # pipe i changes sign then m_sign[i]=2
-#     m_sign = np.abs(np.sign(m0) - np.sign(m))
-#     flag_change_sign = m_sign > 0
-#     return np.where(flag_change_sign.reshape((-1,)), t_node0, f_node0)
-#
-#
-# def t_node_calculator(f_node0: np.ndarray, t_node0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
-#     # pipe i changes sign then m_sign[i]=2
-#     m_sign = np.abs(np.sign(m0) - np.sign(m))
-#     flag_change_sign = m_sign > 0
-#     return np.where(flag_change_sign.reshape((-1,)), f_node0, t_node0)
-#
-#
-# # %% md
-# # Declare equations and parameters
-# # %%
-# Node = sys_df['Node']
-# i = idx(name='i', value=np.asarray(Node['type'][Node['type'] == 3].index))  # intermediate nodes
-# l = idx(name='l', value=np.asarray(Node['type'][Node['type'] == 2].index))  # load nodes
-# s = idx(name='s', value=np.asarray(Node['type'][Node['type'] == 1].index))  # non-balance source nodes
-# r = idx(name='r', value=np.asarray(Node['type'][Node['type'] == 0].index))  # balance source nodes
-# sl = idx(name='sl', value=np.concatenate((s.value, l.value)))
-# rs = idx(name='rs', value=np.concatenate((r.value, s.value)))
-# rsl = idx(name='rsl', value=np.concatenate((r.value, s.value, l.value)))
-# li = idx(name='li', value=np.concatenate((l.value, i.value)))
-# rsi = idx(name='rsi', value=np.concatenate((r.value, s.value, i.value)))
-#
-# mL = Para('mL', dim=2, value=np.asarray(sys_df['m_L']))
-# K = Para(name='K', value=np.asarray(sys_df['K']).reshape(-1, ))
-# phi_set = Para(name='phi_set', value=np.asarray(sys_df['phi_set']).reshape(-1, ))
-#
-# Cp = Para(name='Cp', value=np.asarray(sys_df['Cp']).reshape(-1, ))
-# L = Para(name='L', value=np.asarray(sys_df['L']).reshape(-1, ))
-# coeff_lambda = Para(name='coeff_lambda', value=np.asarray(sys_df['coeff_lambda']).reshape(-1, ))
-# Ta = Para(name='Ta', value=np.asarray(sys_df['Ta']).reshape(-1, ))
-# f_node = sys_df['Pipe']['f_node']
-# t_node = sys_df['Pipe']['t_node']
-# V = Para(name='V', dim=2, value=derive_incidence_matrix(f_node, t_node))
-# Vp = Para(name='Vp', dim=2, value=derive_v_plus(V.value))
-# Vm = Para(name='Vm', dim=2, value=derive_v_minus(V.value))
-# f_node = idx(name='f_node', value=np.asarray(f_node).reshape(-1, ))  # intermediate nodes
-# t_node = idx(name='t_node', value=np.asarray(t_node).reshape(-1, ))  # load nodes
-#
-# m = iVar(name='m', value=np.asarray(sys_df['var']['m']))
-# mq = iVar(name='mq', value=np.asarray(sys_df['var']['mq']))
-# Ts = iVar(name='Ts', value=np.asarray(sys_df['var']['Ts']))
-# Tr = iVar(name='Tr', value=np.asarray(sys_df['var']['Tr']))
-# Touts = iVar(name='Touts', value=np.asarray(sys_df['var']['Touts']))
-# Toutr = iVar(name='Toutr', value=np.asarray(sys_df['var']['Toutr']))
-# phi = iVar(name='phi', value=np.asarray(sys_df['var']['phi']))
-#
-# E1 = Eqn(name='E1', eqn=(Ts[f_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Touts)
-# E3 = Eqn(name='E3', eqn=(Tr[t_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Toutr)
-# E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) + mq[rs])
-# E6 = Eqn(name='E6', eqn=Mat_Mul(V[l, :], m) - mq[l])
-# E7 = Eqn(name='E7', eqn=Mat_Mul(V[i, :], m))
-# E8 = Eqn(name='E8', eqn=Mat_Mul(mL, K * Abs(m) * m))
-# E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], Touts * Abs(m)))
-# E10 = Eqn(name='E10', eqn=Tr[rsi] * Mat_Mul(Vm[rsi, :], Abs(m)) - Mat_Mul(Vm[rsi, :], Toutr * Abs(m)))
-# E11 = Eqn(name='E11', eqn=phi[rsl] - 4182 * mq[rsl] * (Ts[rsl] - Tr[rsl]))
-# E12 = Eqn(name='E12', eqn=Ts[rs] - 100)
-# E13 = Eqn(name='E13', eqn=Tr[l] - 50)
-# E14 = Eqn(name='E14', eqn=phi[sl] - phi_set)
-# E15 = Eqn(name='E15', eqn=phi[i])
-# E16 = Eqn(name='E16', eqn=mq[i])
-# E = AE(name='Pipe Equations', eqn=[E1, E3, E5, E6, E7, E8, E9, E10, E11, E12, E13, E14, E15, E16])
-#
-# E.param_initializer('Vp', param=Param('Vp', value=Vp.value, triggerable=True, trigger_var='m',
-#                                       trigger_fun=partial(v_p_reverse_pipe, V.value, m.value), dim=2))
-#
-# E.param_initializer('Vm', param=Param('Vm', value=Vm.value, triggerable=True, trigger_var='m',
-#                                       trigger_fun=partial(v_m_reverse_pipe, V.value, m.value), dim=2))
-#
-# E.param_initializer('f_node', param=Param('f_node', value=f_node.value, triggerable=True, trigger_var='m',
-#                                           trigger_fun=partial(f_node_calculator,
-#                                                               f_node.value, t_node.value, m.value), dtype=int))
-#
-# E.param_initializer('t_node', param=Param('t_node', value=t_node.value, triggerable=True, trigger_var='m',
-#                                           trigger_fun=partial(t_node_calculator,
-#                                                               f_node.value, t_node.value, m.value), dtype=int))
-#
-# y0 = as_Vars([m, mq, Ts, Tr, Touts, Toutr, phi])
-# nE, code = made_numerical(E, y0, output_code=True)
-#
-# sol_nr = nr_method(nE, y0)
-# # y_cnr, ite = continuous_nr(nE, y0.array)
-#
-#
-# sys_df = pd.read_excel('instances/4node3pipe_change_sign_bench.xlsx',
-#                        sheet_name=None,
-#                        engine='openpyxl',
-#                        header=None)
-#
-#
-# def test_nr_method():
-#     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
-#         # find nonzero elements
-#         idx_nonzero = np.nonzero(sol_nr.y[var_name])
-#         assert max(abs((sol_nr.y[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) /
-#                    np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) <= 1e-8
-#
-#
-# # def test_cnr_method():
-# #     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
-# #         # find nonzero elements
-# #         idx_nonzero = np.nonzero(y_cnr[var_name])
-# #         assert max(abs((y_cnr[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) /
-# #                        np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) <= 1e-8
+# import pandas as pd
+# import numpy as np
+# from functools import partial
+#
+# from Solverz import Eqn, AE, nr_method, as_Vars, iVar, Param, continuous_nr, Para, idx, Abs, exp, Mat_Mul, \
+#     made_numerical
+#
+# # %% initialize variables and params
+# sys_df = pd.read_excel('instances/4node3pipe_change_sign.xlsx',
+#                        sheet_name=None,
+#                        engine='openpyxl',
+#                        index_col=0
+#                        )
+#
+#
+# def derive_incidence_matrix(f_node, t_node):
+#     V = np.zeros((max(max(f_node), max(t_node)) + 1, len(f_node)))
+#     for pipe in range(len(f_node)):
+#         V[f_node[pipe], pipe] = -1
+#         V[t_node[pipe], pipe] = 1
+#     return V
+#
+#
+# def derive_v_plus(v: np.ndarray) -> np.ndarray:
+#     return (v + np.abs(v)) / 2
+#
+#
+# def derive_v_minus(v: np.ndarray) -> np.ndarray:
+#     return (v - np.abs(v)) / 2
+#
+#
+# def v_p_reverse_pipe(V0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
+#     """
+#     Trigger function of v_p
+#     if some element of m changes its sign, then related column of V0 changes its sign
+#     :param V0:
+#     :param m0: initial mass flow rate
+#     :param m:
+#     :return: $V_0*(I-diag(sign(m0)-sign(m)))$
+#     """
+#     # pipe i changes sign then m_sign[i]=2
+#     m_sign = np.abs(np.sign(m0) - np.sign(m))
+#     return derive_v_plus(V0 @ (np.eye(m.shape[0]) - np.diagflat(m_sign)))
+#
+#
+# def v_m_reverse_pipe(V0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
+#     # pipe i changes sign then m_sign[i]=2
+#     m_sign = np.abs(np.sign(m0) - np.sign(m))
+#     return derive_v_minus(V0 @ (np.eye(m.shape[0]) - np.diagflat(np.abs(m_sign))))
+#
+#
+# def f_node_calculator(f_node0: np.ndarray, t_node0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
+#     # pipe i changes sign then m_sign[i]=2
+#     m_sign = np.abs(np.sign(m0) - np.sign(m))
+#     flag_change_sign = m_sign > 0
+#     return np.where(flag_change_sign.reshape((-1,)), t_node0, f_node0)
+#
+#
+# def t_node_calculator(f_node0: np.ndarray, t_node0: np.ndarray, m0: np.ndarray, m: np.ndarray) -> np.ndarray:
+#     # pipe i changes sign then m_sign[i]=2
+#     m_sign = np.abs(np.sign(m0) - np.sign(m))
+#     flag_change_sign = m_sign > 0
+#     return np.where(flag_change_sign.reshape((-1,)), f_node0, t_node0)
+#
+#
+# # %% md
+# # Declare equations and parameters
+# # %%
+# Node = sys_df['Node']
+# i = idx(name='i', value=np.asarray(Node['type'][Node['type'] == 3].index))  # intermediate nodes
+# l = idx(name='l', value=np.asarray(Node['type'][Node['type'] == 2].index))  # load nodes
+# s = idx(name='s', value=np.asarray(Node['type'][Node['type'] == 1].index))  # non-balance source nodes
+# r = idx(name='r', value=np.asarray(Node['type'][Node['type'] == 0].index))  # balance source nodes
+# sl = idx(name='sl', value=np.concatenate((s.value, l.value)))
+# rs = idx(name='rs', value=np.concatenate((r.value, s.value)))
+# rsl = idx(name='rsl', value=np.concatenate((r.value, s.value, l.value)))
+# li = idx(name='li', value=np.concatenate((l.value, i.value)))
+# rsi = idx(name='rsi', value=np.concatenate((r.value, s.value, i.value)))
+#
+# mL = Para('mL', dim=2, value=np.asarray(sys_df['m_L']))
+# K = Para(name='K', value=np.asarray(sys_df['K']).reshape(-1, ))
+# phi_set = Para(name='phi_set', value=np.asarray(sys_df['phi_set']).reshape(-1, ))
+#
+# Cp = Para(name='Cp', value=np.asarray(sys_df['Cp']).reshape(-1, ))
+# L = Para(name='L', value=np.asarray(sys_df['L']).reshape(-1, ))
+# coeff_lambda = Para(name='coeff_lambda', value=np.asarray(sys_df['coeff_lambda']).reshape(-1, ))
+# Ta = Para(name='Ta', value=np.asarray(sys_df['Ta']).reshape(-1, ))
+# f_node = sys_df['Pipe']['f_node']
+# t_node = sys_df['Pipe']['t_node']
+# V = Para(name='V', dim=2, value=derive_incidence_matrix(f_node, t_node))
+# Vp = Para(name='Vp', dim=2, value=derive_v_plus(V.value))
+# Vm = Para(name='Vm', dim=2, value=derive_v_minus(V.value))
+# f_node = idx(name='f_node', value=np.asarray(f_node).reshape(-1, ))  # intermediate nodes
+# t_node = idx(name='t_node', value=np.asarray(t_node).reshape(-1, ))  # load nodes
+#
+# m = iVar(name='m', value=np.asarray(sys_df['var']['m']))
+# mq = iVar(name='mq', value=np.asarray(sys_df['var']['mq']))
+# Ts = iVar(name='Ts', value=np.asarray(sys_df['var']['Ts']))
+# Tr = iVar(name='Tr', value=np.asarray(sys_df['var']['Tr']))
+# Touts = iVar(name='Touts', value=np.asarray(sys_df['var']['Touts']))
+# Toutr = iVar(name='Toutr', value=np.asarray(sys_df['var']['Toutr']))
+# phi = iVar(name='phi', value=np.asarray(sys_df['var']['phi']))
+#
+# E1 = Eqn(name='E1', eqn=(Ts[f_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Touts)
+# E3 = Eqn(name='E3', eqn=(Tr[t_node] - Ta) * exp(-coeff_lambda * L / (Cp * Abs(m))) + Ta - Toutr)
+# E5 = Eqn(name='E5', eqn=Mat_Mul(V[rs, :], m) + mq[rs])
+# E6 = Eqn(name='E6', eqn=Mat_Mul(V[l, :], m) - mq[l])
+# E7 = Eqn(name='E7', eqn=Mat_Mul(V[i, :], m))
+# E8 = Eqn(name='E8', eqn=Mat_Mul(mL, K * Abs(m) * m))
+# E9 = Eqn(name='E9', eqn=Ts[li] * Mat_Mul(Vp[li, :], Abs(m)) - Mat_Mul(Vp[li, :], Touts * Abs(m)))
+# E10 = Eqn(name='E10', eqn=Tr[rsi] * Mat_Mul(Vm[rsi, :], Abs(m)) - Mat_Mul(Vm[rsi, :], Toutr * Abs(m)))
+# E11 = Eqn(name='E11', eqn=phi[rsl] - 4182 * mq[rsl] * (Ts[rsl] - Tr[rsl]))
+# E12 = Eqn(name='E12', eqn=Ts[rs] - 100)
+# E13 = Eqn(name='E13', eqn=Tr[l] - 50)
+# E14 = Eqn(name='E14', eqn=phi[sl] - phi_set)
+# E15 = Eqn(name='E15', eqn=phi[i])
+# E16 = Eqn(name='E16', eqn=mq[i])
+# E = AE(name='Pipe Equations', eqn=[E1, E3, E5, E6, E7, E8, E9, E10, E11, E12, E13, E14, E15, E16])
+#
+# E.param_initializer('Vp', param=Param('Vp', value=Vp.value, triggerable=True, trigger_var='m',
+#                                       trigger_fun=partial(v_p_reverse_pipe, V.value, m.value), dim=2))
+#
+# E.param_initializer('Vm', param=Param('Vm', value=Vm.value, triggerable=True, trigger_var='m',
+#                                       trigger_fun=partial(v_m_reverse_pipe, V.value, m.value), dim=2))
+#
+# E.param_initializer('f_node', param=Param('f_node', value=f_node.value, triggerable=True, trigger_var='m',
+#                                           trigger_fun=partial(f_node_calculator,
+#                                                               f_node.value, t_node.value, m.value), dtype=int))
+#
+# E.param_initializer('t_node', param=Param('t_node', value=t_node.value, triggerable=True, trigger_var='m',
+#                                           trigger_fun=partial(t_node_calculator,
+#                                                               f_node.value, t_node.value, m.value), dtype=int))
+#
+# y0 = as_Vars([m, mq, Ts, Tr, Touts, Toutr, phi])
+# nE, code = made_numerical(E, y0, output_code=True)
+#
+# sol_nr = nr_method(nE, y0)
+# # y_cnr, ite = continuous_nr(nE, y0.array)
+#
+#
+# sys_df = pd.read_excel('instances/4node3pipe_change_sign_bench.xlsx',
+#                        sheet_name=None,
+#                        engine='openpyxl',
+#                        header=None)
+#
+#
+# def test_nr_method():
+#     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
+#         # find nonzero elements
+#         idx_nonzero = np.nonzero(sol_nr.y[var_name])
+#         assert max(abs((sol_nr.y[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) /
+#                    np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) <= 1e-8
+#
+#
+# # def test_cnr_method():
+# #     for var_name in ['Ts', 'Tr', 'm', 'mq', 'phi']:
+# #         # find nonzero elements
+# #         idx_nonzero = np.nonzero(y_cnr[var_name])
+# #         assert max(abs((y_cnr[var_name][idx_nonzero] - np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, )) /
+# #                        np.asarray(sys_df[var_name])[idx_nonzero].reshape(-1, ))) <= 1e-8
```

### Comparing `solverz-0.0.1rc1/tests/test_dyn_gas_flow_single_pipe.py` & `solverz-0.0.1rc2/tests/test_dyn_gas_flow_single_pipe.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import numpy as np
-import pandas as pd
-
-from Solverz import idx, iVar, Para, as_Vars, HyperbolicPde, fdae_solver, Eqn, Param, IdxParam, FDAE, made_numerical, Opt
-
-results = pd.read_excel('instances/dynamic_gas_flow_single_pipe.xlsx',
-                        sheet_name=None,
-                        engine='openpyxl'
-                        )
-
-Pie = iVar('Pie', value=np.linspace(9, 8.728, 11) * 1e6)
-q = iVar('q', value=7.3125 * np.ones((11,)))
-va = Para('va', value=340)
-D = Para('D', value=0.5)
-S = Para('S', value=np.pi * (D.value / 2) ** 2)
-lam = Para('lam', 0.3)
-pb = Para('pb', 9e6)
-qb = Para('qb', 7.3125)
-M = idx('M')
-L = 3000
-
-gas_pde1 = HyperbolicPde('mass conservation',
-                         diff_var=Pie,
-                         flux=va ** 2 / S * q,
-                         two_dim_var=[Pie, q])
-gas_pde2 = HyperbolicPde('momentum conservation',
-                         diff_var=q,
-                         flux=S * Pie,
-                         source=-lam * va ** 2 * q ** 2 / (2 * D * S * Pie),
-                         two_dim_var=[Pie, q])
-
-ae1 = gas_pde1.finite_difference()
-ae2 = gas_pde2.finite_difference()
-ae3 = Eqn(name='boundary condition Pie', eqn=Pie[0] - pb)
-ae4 = Eqn(name='boundary condition q', eqn=q[M] - qb)
-
-gas_FDE = FDAE([ae1, ae2, ae3, ae4], name='gas FDE', nstep=1)
-u0 = as_Vars([Pie, q])
-gas_FDE.update_param(u0.derive_alias('_tag_0'))
-
-gas_FDE.param_initializer('M', IdxParam('M', value=np.array(10)))
-gas_FDE.param_initializer('dx', Param('dx', value=np.array(300)))
-gas_FDE.param_initializer('dt', Param('dt', value=5))
-
-ngas = made_numerical(gas_FDE, u0)
-sol1 = fdae_solver(ngas, [0, 3600], u0, Opt(step_size=5, ite_tol=1e-3))
-ngas_sparse, code = made_numerical(gas_FDE, u0, sparse=True, output_code=True)
-
-sol2 = fdae_solver(ngas_sparse, [0, 3600], u0, Opt(step_size=5, ite_tol=1e-3))
-
-
-def test_fde_solver():
-    pout = np.asarray(results['results']['pout'])
-    qin = np.asarray(results['results']['qin'])
-
-    # if matrix container is cvxopt.spmatrix
-    # assert np.mean(abs(pout - u['Pie'][:, -1] / 1e6)) < 5e-6
-    # assert np.mean(abs(qin - u['q'][:, 0])) < 1.2e-4
-
-    # if matrix container is scipy.sparse.csc_array
-    assert np.mean(abs(pout - sol1.Y['Pie'][:, -1] / 1e6)) < 1e-10
-    assert np.mean(abs(qin - sol1.Y['q'][:, 0])) < 1e-7
-    assert np.mean(abs(pout - sol2.Y['Pie'][:, -1] / 1e6)) < 1e-10
-    assert np.mean(abs(qin - sol2.Y['q'][:, 0])) < 1e-7
+import numpy as np
+import pandas as pd
+
+from Solverz import idx, iVar, Para, as_Vars, HyperbolicPde, fdae_solver, Eqn, Param, IdxParam, FDAE, made_numerical, Opt
+
+results = pd.read_excel('instances/dynamic_gas_flow_single_pipe.xlsx',
+                        sheet_name=None,
+                        engine='openpyxl'
+                        )
+
+Pie = iVar('Pie', value=np.linspace(9, 8.728, 11) * 1e6)
+q = iVar('q', value=7.3125 * np.ones((11,)))
+va = Para('va', value=340)
+D = Para('D', value=0.5)
+S = Para('S', value=np.pi * (D.value / 2) ** 2)
+lam = Para('lam', 0.3)
+pb = Para('pb', 9e6)
+qb = Para('qb', 7.3125)
+M = idx('M')
+L = 3000
+
+gas_pde1 = HyperbolicPde('mass conservation',
+                         diff_var=Pie,
+                         flux=va ** 2 / S * q,
+                         two_dim_var=[Pie, q])
+gas_pde2 = HyperbolicPde('momentum conservation',
+                         diff_var=q,
+                         flux=S * Pie,
+                         source=-lam * va ** 2 * q ** 2 / (2 * D * S * Pie),
+                         two_dim_var=[Pie, q])
+
+ae1 = gas_pde1.finite_difference()
+ae2 = gas_pde2.finite_difference()
+ae3 = Eqn(name='boundary condition Pie', eqn=Pie[0] - pb)
+ae4 = Eqn(name='boundary condition q', eqn=q[M] - qb)
+
+gas_FDE = FDAE([ae1, ae2, ae3, ae4], name='gas FDE', nstep=1)
+u0 = as_Vars([Pie, q])
+gas_FDE.update_param(u0.derive_alias('_tag_0'))
+
+gas_FDE.param_initializer('M', IdxParam('M', value=np.array(10)))
+gas_FDE.param_initializer('dx', Param('dx', value=np.array(300)))
+gas_FDE.param_initializer('dt', Param('dt', value=5))
+
+ngas = made_numerical(gas_FDE, u0)
+sol1 = fdae_solver(ngas, [0, 3600], u0, Opt(step_size=5, ite_tol=1e-3))
+ngas_sparse, code = made_numerical(gas_FDE, u0, sparse=True, output_code=True)
+
+sol2 = fdae_solver(ngas_sparse, [0, 3600], u0, Opt(step_size=5, ite_tol=1e-3))
+
+
+def test_fde_solver():
+    pout = np.asarray(results['results']['pout'])
+    qin = np.asarray(results['results']['qin'])
+
+    # if matrix container is cvxopt.spmatrix
+    # assert np.mean(abs(pout - u['Pie'][:, -1] / 1e6)) < 5e-6
+    # assert np.mean(abs(qin - u['q'][:, 0])) < 1.2e-4
+
+    # if matrix container is scipy.sparse.csc_array
+    assert np.mean(abs(pout - sol1.Y['Pie'][:, -1] / 1e6)) < 1e-10
+    assert np.mean(abs(qin - sol1.Y['q'][:, 0])) < 1e-7
+    assert np.mean(abs(pout - sol2.Y['Pie'][:, -1] / 1e6)) < 1e-10
+    assert np.mean(abs(qin - sol2.Y['q'][:, 0])) < 1e-7
```

### Comparing `solverz-0.0.1rc1/tests/test_gasflow.py` & `solverz-0.0.1rc2/tests/test_gasflow.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import numpy as np
-
-from Solverz import idx, iVar, Para, Sign, as_Vars, nr_method, Eqn, AE, Mat_Mul, made_numerical
-
-k = idx('k', value=[0, 1, 2])
-i = idx('i', value=[0, 0, 3])
-j = idx('j', value=[1, 2, 2])
-m = idx('m', value=[1, 2, 3])
-
-Pi = iVar('Pi', value=[50, 49, 45, 1.3 * 49])  # 50, 40.8160, 49.7827, 1.3 * 40.8160
-fin = iVar('fin', value=[34.6406, 10.8650, 23.7756, 0])  # 29.8308, 4.8098, 18.9658
-finset = Para('finset', value=[10.8650, 23.7756, 0])
-f = iVar('f', value=[10, 5, 25, 25])
-c = Para('c', value=[1.0329225961928894, 1.0329267609699861, 1.032931789457253, 1])
-A = Para('A', dim=2, value=[[-1, -1, 0, 0], [1, 0, 0, -1], [0, 1, 1, 0], [0, 0, -1, 1]])
-
-eqn1 = Eqn(name='mass flow continuity', eqn=finset - Mat_Mul(A[m, :], f))
-eqn2 = Eqn(name='mass flow1',
-           eqn=f[k] - c[k] * Sign(Pi[i] - Pi[j]) * (Sign(Pi[i] - Pi[j]) * (Pi[i] ** 2 - Pi[j] ** 2)) ** (1 / 2))
-eqn3 = Eqn(name='pressure', eqn=Pi[0] - 50)
-eqn4 = Eqn(name='pressure1', eqn=Pi[3] - 1.3 * Pi[1])
-
-gas_flow = AE(eqn=[eqn1, eqn2, eqn3, eqn4])
-y0 = as_Vars([f, Pi])
-
-ngas_flow = made_numerical(gas_flow, y0)
-sol = nr_method(ngas_flow, y0)
-
-
-def test_nr_method():
-    bench = np.array([29.830799999999996, 4.809800000000001, 18.965799999999998,
-                      18.965799999999998, 50.0, 40.816, 49.78269999999999, 53.06080000000001])
-    assert np.max(np.abs((sol.y - bench) / bench)) <= 1e-8
+import numpy as np
+
+from Solverz import idx, iVar, Para, Sign, as_Vars, nr_method, Eqn, AE, Mat_Mul, made_numerical
+
+k = idx('k', value=[0, 1, 2])
+i = idx('i', value=[0, 0, 3])
+j = idx('j', value=[1, 2, 2])
+m = idx('m', value=[1, 2, 3])
+
+Pi = iVar('Pi', value=[50, 49, 45, 1.3 * 49])  # 50, 40.8160, 49.7827, 1.3 * 40.8160
+fin = iVar('fin', value=[34.6406, 10.8650, 23.7756, 0])  # 29.8308, 4.8098, 18.9658
+finset = Para('finset', value=[10.8650, 23.7756, 0])
+f = iVar('f', value=[10, 5, 25, 25])
+c = Para('c', value=[1.0329225961928894, 1.0329267609699861, 1.032931789457253, 1])
+A = Para('A', dim=2, value=[[-1, -1, 0, 0], [1, 0, 0, -1], [0, 1, 1, 0], [0, 0, -1, 1]])
+
+eqn1 = Eqn(name='mass flow continuity', eqn=finset - Mat_Mul(A[m, :], f))
+eqn2 = Eqn(name='mass flow1',
+           eqn=f[k] - c[k] * Sign(Pi[i] - Pi[j]) * (Sign(Pi[i] - Pi[j]) * (Pi[i] ** 2 - Pi[j] ** 2)) ** (1 / 2))
+eqn3 = Eqn(name='pressure', eqn=Pi[0] - 50)
+eqn4 = Eqn(name='pressure1', eqn=Pi[3] - 1.3 * Pi[1])
+
+gas_flow = AE(eqn=[eqn1, eqn2, eqn3, eqn4])
+y0 = as_Vars([f, Pi])
+
+ngas_flow = made_numerical(gas_flow, y0)
+sol = nr_method(ngas_flow, y0)
+
+
+def test_nr_method():
+    bench = np.array([29.830799999999996, 4.809800000000001, 18.965799999999998,
+                      18.965799999999998, 50.0, 40.816, 49.78269999999999, 53.06080000000001])
+    assert np.max(np.abs((sol.y - bench) / bench)) <= 1e-8
```

### Comparing `solverz-0.0.1rc1/tests/test_m3b9.py` & `solverz-0.0.1rc2/tests/test_m3b9.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import numpy as np
-import pandas as pd
-
-from Solverz import DAE, Eqn, Ode, iVar, Para, idx, sin, cos, Rodas, as_Vars, Mat_Mul, \
-    implicit_trapezoid, Opt, TimeSeriesParam, made_numerical
-
-omega = iVar(name='omega')
-delta = iVar(name='delta')
-Ux = iVar(name='Ux')
-Uy = iVar(name='Uy')
-Ixg = iVar(name='Ixg')
-Iyg = iVar(name='Iyg')
-g = idx('g', value=[0, 1, 2])
-ng = idx('ng', value=[3, 4, 5, 6, 7, 8])
-Pm = Para(name='Pm')
-G = Para(name='G', dim=2)
-B = Para(name='B', dim=2)
-D = Para(name='D')
-Tj = Para(name='Tj')
-ra = Para(name='ra')
-omega_b = Para(name='omega_b')
-Edp = Para(name='Edp')
-Eqp = Para(name='Eqp')
-Xdp = Para(name='Xdp')
-Xqp = Para(name='Xqp')
-
-rotator_eqn = Ode(name='rotator speed',
-                  f=(Pm - (Ux[g] * Ixg + Uy[g] * Iyg + (Ixg ** 2 + Iyg ** 2) * ra) - D * (omega - 1)) / Tj,
-                  diff_var=omega)
-delta_eqn = Ode(name='delta', f=(omega - 1) * omega_b, diff_var=delta)
-Ed_prime = Eqn(name='Ed_prime', eqn=Edp - sin(delta) * (Ux[g] + ra * Ixg - Xqp * Iyg) + cos(delta) * (
-        Uy[g] + ra * Iyg + Xqp * Ixg))
-Eq_prime = Eqn(name='Eq_prime', eqn=Eqp - cos(delta) * (Ux[g] + ra * Ixg - Xdp * Iyg) - sin(delta) * (
-        Uy[g] + ra * Iyg + Xdp * Ixg))
-Ix_inject = Eqn(name='Ixg_inject', eqn=Ixg - (Mat_Mul(G[g, :], Ux) - Mat_Mul(B[g, :], Uy)))
-Iy_inject = Eqn(name='Iyg_inject', eqn=Iyg - (Mat_Mul(G[g, :], Uy) + Mat_Mul(B[g, :], Ux)))
-Ixng_inject = Eqn(name='Ixng_inject', eqn=Mat_Mul(G[ng, :], Ux) - Mat_Mul(B[ng, :], Uy))
-Iyng_inject = Eqn(name='Iyng_inject', eqn=Mat_Mul(G[ng, :], Uy) + Mat_Mul(B[ng, :], Ux))
-
-dt = np.array(0.002)
-T = np.array(10)
-
-m3b9 = DAE([delta_eqn, rotator_eqn, Ed_prime, Eq_prime, Ix_inject, Iy_inject, Ixng_inject, Iyng_inject],
-           name='m3b9')
-m3b9.update_param('Pm', [0.7164, 1.6300, 0.8500])
-m3b9.update_param('ra', [0.0000, 0.0000, 0.0000])
-m3b9.update_param('D', [10, 10, 10])
-m3b9.update_param('Tj', [47.2800, 12.8000, 6.0200])
-m3b9.update_param('omega_b', [376.991118430775])
-m3b9.update_param('g', [0, 1, 2])
-m3b9.update_param('ng', [3, 4, 5, 6, 7, 8])
-m3b9.update_param('Edp', [0.0000, 0.0000, 0.0000])
-m3b9.update_param('Eqp', [1.05636632091501, 0.788156757672709, 0.767859471854610])
-m3b9.update_param('Xdp', [0.0608, 0.1198, 0.1813])
-m3b9.update_param('Xqp', [0.0969, 0.8645, 1.2578])
-df = pd.read_excel('instances/test_m3b9.xlsx',
-                   sheet_name=None,
-                   engine='openpyxl',
-                   header=None
-                   )
-Gvalue = np.asarray(df['G'])
-m3b9.param_initializer('G', TimeSeriesParam(name='G',
-                                            v_series=[Gvalue[6, 6], 10000, 10000, Gvalue[6, 6], Gvalue[6, 6]],
-                                            time_series=[0, 0.002, 0.03, 0.032, T],
-                                            value=Gvalue,
-                                            index=(6, 6),
-                                            dim=2))
-m3b9.update_param('B', np.asarray(df['B']))
-
-delta = iVar('delta', [0.0625815077879868, 1.06638275203221, 0.944865048677501])
-omega = iVar('omega', [1, 1, 1])
-Ixg = iVar('Ixg', [0.688836021737262, 1.57988988391346, 0.817891311823357])
-Iyg = iVar('Iyg', [-0.260077644814056, 0.192406178191528, 0.173047791590276])
-Ux = iVar('Ux',
-          [1.04000110267534, 1.01157932564567, 1.02160343921907,
-          1.02502063033405, 0.993215117729926, 1.01056073782038,
-          1.02360471178264, 1.01579907336413, 1.03174403980626])
-Uy = iVar('Uy',
-          [9.38510394478286e-07, 0.165293826097057, 0.0833635520284917,
-          -0.0396760163416718, -0.0692587531054159, -0.0651191654677445,
-          0.0665507083524658, 0.0129050646926083, 0.0354351211556429])
-
-y0 = as_Vars([delta, omega, Ixg, Iyg, Ux, Uy])
-
-m3b9_dae, code = made_numerical(m3b9, y0, sparse=False, output_code=True)
-sol_rodas = Rodas(m3b9_dae,
-                  np.linspace(0, 10, 5001).reshape(-1, ),
-                  y0,
-                  Opt(hinit=1e-5))
-
-sol_trape = implicit_trapezoid(m3b9_dae,
-                               [0, 10],
-                               y0,
-                               Opt(step_size=dt))
-
-
-def test_m3b9():
-    assert np.abs(np.asarray(df['omega']) - sol_rodas.Y['omega']).max() <= 5e-5
-    assert np.abs(np.asarray(df['omega']) - sol_trape.Y['omega']).max() <= 2.48e-4
-    assert np.abs(np.asarray(df['delta']) - sol_rodas.Y['delta']).max() <= 9.6e-4
-    assert np.abs(np.asarray(df['delta']) - sol_trape.Y['delta']).max() <= 7.8e-2
+import numpy as np
+import pandas as pd
+
+from Solverz import DAE, Eqn, Ode, iVar, Para, idx, sin, cos, Rodas, as_Vars, Mat_Mul, \
+    implicit_trapezoid, Opt, TimeSeriesParam, made_numerical
+
+omega = iVar(name='omega')
+delta = iVar(name='delta')
+Ux = iVar(name='Ux')
+Uy = iVar(name='Uy')
+Ixg = iVar(name='Ixg')
+Iyg = iVar(name='Iyg')
+g = idx('g', value=[0, 1, 2])
+ng = idx('ng', value=[3, 4, 5, 6, 7, 8])
+Pm = Para(name='Pm')
+G = Para(name='G', dim=2)
+B = Para(name='B', dim=2)
+D = Para(name='D')
+Tj = Para(name='Tj')
+ra = Para(name='ra')
+omega_b = Para(name='omega_b')
+Edp = Para(name='Edp')
+Eqp = Para(name='Eqp')
+Xdp = Para(name='Xdp')
+Xqp = Para(name='Xqp')
+
+rotator_eqn = Ode(name='rotator speed',
+                  f=(Pm - (Ux[g] * Ixg + Uy[g] * Iyg + (Ixg ** 2 + Iyg ** 2) * ra) - D * (omega - 1)) / Tj,
+                  diff_var=omega)
+delta_eqn = Ode(name='delta', f=(omega - 1) * omega_b, diff_var=delta)
+Ed_prime = Eqn(name='Ed_prime', eqn=Edp - sin(delta) * (Ux[g] + ra * Ixg - Xqp * Iyg) + cos(delta) * (
+        Uy[g] + ra * Iyg + Xqp * Ixg))
+Eq_prime = Eqn(name='Eq_prime', eqn=Eqp - cos(delta) * (Ux[g] + ra * Ixg - Xdp * Iyg) - sin(delta) * (
+        Uy[g] + ra * Iyg + Xdp * Ixg))
+Ix_inject = Eqn(name='Ixg_inject', eqn=Ixg - (Mat_Mul(G[g, :], Ux) - Mat_Mul(B[g, :], Uy)))
+Iy_inject = Eqn(name='Iyg_inject', eqn=Iyg - (Mat_Mul(G[g, :], Uy) + Mat_Mul(B[g, :], Ux)))
+Ixng_inject = Eqn(name='Ixng_inject', eqn=Mat_Mul(G[ng, :], Ux) - Mat_Mul(B[ng, :], Uy))
+Iyng_inject = Eqn(name='Iyng_inject', eqn=Mat_Mul(G[ng, :], Uy) + Mat_Mul(B[ng, :], Ux))
+
+dt = np.array(0.002)
+T = np.array(10)
+
+m3b9 = DAE([delta_eqn, rotator_eqn, Ed_prime, Eq_prime, Ix_inject, Iy_inject, Ixng_inject, Iyng_inject],
+           name='m3b9')
+m3b9.update_param('Pm', [0.7164, 1.6300, 0.8500])
+m3b9.update_param('ra', [0.0000, 0.0000, 0.0000])
+m3b9.update_param('D', [10, 10, 10])
+m3b9.update_param('Tj', [47.2800, 12.8000, 6.0200])
+m3b9.update_param('omega_b', [376.991118430775])
+m3b9.update_param('g', [0, 1, 2])
+m3b9.update_param('ng', [3, 4, 5, 6, 7, 8])
+m3b9.update_param('Edp', [0.0000, 0.0000, 0.0000])
+m3b9.update_param('Eqp', [1.05636632091501, 0.788156757672709, 0.767859471854610])
+m3b9.update_param('Xdp', [0.0608, 0.1198, 0.1813])
+m3b9.update_param('Xqp', [0.0969, 0.8645, 1.2578])
+df = pd.read_excel('instances/test_m3b9.xlsx',
+                   sheet_name=None,
+                   engine='openpyxl',
+                   header=None
+                   )
+Gvalue = np.asarray(df['G'])
+m3b9.param_initializer('G', TimeSeriesParam(name='G',
+                                            v_series=[Gvalue[6, 6], 10000, 10000, Gvalue[6, 6], Gvalue[6, 6]],
+                                            time_series=[0, 0.002, 0.03, 0.032, T],
+                                            value=Gvalue,
+                                            index=(6, 6),
+                                            dim=2))
+m3b9.update_param('B', np.asarray(df['B']))
+
+delta = iVar('delta', [0.0625815077879868, 1.06638275203221, 0.944865048677501])
+omega = iVar('omega', [1, 1, 1])
+Ixg = iVar('Ixg', [0.688836021737262, 1.57988988391346, 0.817891311823357])
+Iyg = iVar('Iyg', [-0.260077644814056, 0.192406178191528, 0.173047791590276])
+Ux = iVar('Ux',
+          [1.04000110267534, 1.01157932564567, 1.02160343921907,
+          1.02502063033405, 0.993215117729926, 1.01056073782038,
+          1.02360471178264, 1.01579907336413, 1.03174403980626])
+Uy = iVar('Uy',
+          [9.38510394478286e-07, 0.165293826097057, 0.0833635520284917,
+          -0.0396760163416718, -0.0692587531054159, -0.0651191654677445,
+          0.0665507083524658, 0.0129050646926083, 0.0354351211556429])
+
+y0 = as_Vars([delta, omega, Ixg, Iyg, Ux, Uy])
+
+m3b9_dae, code = made_numerical(m3b9, y0, sparse=False, output_code=True)
+sol_rodas = Rodas(m3b9_dae,
+                  np.linspace(0, 10, 5001).reshape(-1, ),
+                  y0,
+                  Opt(hinit=1e-5))
+
+sol_trape = implicit_trapezoid(m3b9_dae,
+                               [0, 10],
+                               y0,
+                               Opt(step_size=dt))
+
+
+def test_m3b9():
+    assert np.abs(np.asarray(df['omega']) - sol_rodas.Y['omega']).max() <= 5e-5
+    assert np.abs(np.asarray(df['omega']) - sol_trape.Y['omega']).max() <= 2.48e-4
+    assert np.abs(np.asarray(df['delta']) - sol_rodas.Y['delta']).max() <= 9.6e-4
+    assert np.abs(np.asarray(df['delta']) - sol_trape.Y['delta']).max() <= 7.8e-2
```

### Comparing `solverz-0.0.1rc1/README.md` & `solverz-0.0.1rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,13 +99,19 @@
 
 ```python
 from bounceball import mdl as nbball, y as y0
 ```
 
 # Installation
 
+Solverz requires ```python>=3.10```, and can be installed locally with
+
+```shell
+pip install Solverz
+```
+
 # Useful Resources
 
 - [Solverz Documentation](https://docs.solverz.org)
 - [Solverz Cookbook](https://cookbook.solverz.org)
```

### Comparing `solverz-0.0.1rc1/PKG-INFO` & `solverz-0.0.1rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.3
 Name: Solverz
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A simulation modelling language
 Project-URL: Homepage, https://github.com/smallbunnies/Solverz
 Project-URL: Issues, https://github.com/smallbunnies/Solverz/issues
 Author-email: Ruizhi Yu <rz.yu@foxmail.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Requires-Dist: dill>=0.3.7
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: networkx>=3.1
 Requires-Dist: numba==0.58.1
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: openpyxl>=3.0.10
 Requires-Dist: pandas>=1.4.2
@@ -124,13 +126,19 @@
 
 ```python
 from bounceball import mdl as nbball, y as y0
 ```
 
 # Installation
 
+Solverz requires ```python>=3.10```, and can be installed locally with
+
+```shell
+pip install Solverz
+```
+
 # Useful Resources
 
 - [Solverz Documentation](https://docs.solverz.org)
 - [Solverz Cookbook](https://cookbook.solverz.org)
```

