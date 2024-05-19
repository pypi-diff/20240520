# Comparing `tmp/amazon-orders-1.1.1.tar.gz` & `tmp/amazon_orders-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-orders-1.1.1.tar", last modified: Wed Apr 10 03:46:20 2024, max compression
+gzip compressed data, was "amazon_orders-1.1.2.tar", last modified: Sun May 19 23:20:59 2024, max compression
```

## Comparing `amazon-orders-1.1.1.tar` & `amazon_orders-1.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:46:20.399515 amazon-orders-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-10 03:46:20.399515 amazon-orders-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:46:20.395515 amazon-orders-1.1.1/amazon_orders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 03:46:20.000000 amazon-orders-1.1.1/amazon_orders.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:46:20.395515 amazon-orders-1.1.1/amazonorders/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/banner.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:46:20.395515 amazon-orders-1.1.1/amazonorders/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/parsable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/seller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/entity/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/amazonorders/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:46:20.399515 amazon-orders-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:46:20.395515 amazon-orders-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/tests/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-04-10 03:45:34.000000 amazon-orders-1.1.1/tests/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/amazon_orders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 23:20:59.000000 amazon_orders-1.1.2/amazon_orders.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/amazonorders/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/banner.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/amazonorders/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/parsable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/seller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/entity/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/amazonorders/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:20:59.208112 amazon_orders-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/tests/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-19 23:20:10.000000 amazon_orders-1.1.2/tests/testcase.py
```

### Comparing `amazon-orders-1.1.1/CHANGELOG.md` & `amazon_orders-1.1.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,144 +1,226 @@
 # Changelog
+
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased](https://github.com/alexdlaird/amazon-orders/compare/1.1.1...HEAD)
+## [Unreleased](https://github.com/alexdlaird/amazon-orders/compare/1.1.2...HEAD)
+
+## [1.1.2](https://github.com/alexdlaird/amazon-orders/compare/1.1.1...1.1.2) - 2024-05-18
+
+### Added
+- Build improvements.
+- Documentation improvements.
+- Test improvements (Amazon no longer provides the `condition` field in many cases).
+
+### Fixed
+
+- Raise `AmazonOrdersNotFoundError` when Order is not found.
+- Prices with thousands separator now parse properly.
+
+### Changed
+
+- [AmazonOrder.debug](https://amazon-orders.readthedocs.io/en/1.1.2/api.html#amazonorders.orders.AmazonOrders.debug)
+  defaults to the value
+  of [AmazonSession.debug](https://amazon-orders.readthedocs.io/en/1.1.2/api.html#amazonorders.session.AmazonSession.debug)
+  if an override is not passed.
 
 ## [1.1.1](https://github.com/alexdlaird/amazon-orders/compare/1.0.16...1.1.1) - 2024-04-09
+
 ### Added
+
 - Build improvements.
 - Test improvements.
 
 ### Changed
+
 - Renamed `kwarg` passed to `IODefault.prompt()` from `captcha_img_url` to `img_url`.
 - Renamed `kwarg` passed to `IODefault.prompt()` from `mfa_device_select_choices` to `choices`.
 
 ## [1.0.16](https://github.com/alexdlaird/amazon-orders/compare/1.0.15...1.0.16) - 2024-03-24
+
 ### Added
-- `constants.BASE_URL` will look for the environment variable `AMAZON_BASE_URL` before defaulting to "https://www.amazon.com".
+
+- `constants.BASE_URL` will look for the environment variable `AMAZON_BASE_URL` before defaulting
+  to "https://www.amazon.com".
 - Build and stability improvements.
 
 ## [1.0.15](https://github.com/alexdlaird/amazon-orders/compare/1.0.14...1.0.15) - 2024-03-05
+
 ### Added
+
 - Build and style improvements.
 - Documentation improvements.
 - `pytest` to streamline running unit and integration tests.
 
 ### Removed
-- `conf.VERSION`, moved all version information to `amazonorders/__init__.py`. Get package version with `from amazonorders import __version__` instead.
+
+- `conf.VERSION`, moved all version information to `amazonorders/__init__.py`. Get package version
+  with `from amazonorders import __version__` instead.
 
 ## [1.0.14](https://github.com/alexdlaird/amazon-orders/compare/1.0.13...1.0.14) - 2024-02-26
+
 ### Added
+
 - Build improvements.
 
 ### Changed
+
 - Renamed `make check-style` to `make check`.
 
 ## [1.0.13](https://github.com/alexdlaird/amazon-orders/compare/1.0.12...1.0.13) - 2024-02-20
+
 ### Added
+
 - `login` command to CLI.
 - If `--username` or `--password` are not given and no stored session, CLI will prompt.
 - Build improvements.
 
 ### Fixed
+
 - Issue where `Parsable` objects could not be pickled due to BeautifulSoup `Tag` objects.
 
 ## [1.0.12](https://github.com/alexdlaird/amazon-orders/compare/1.0.11...1.0.12) - 2024-02-11
+
 ### Added
+
 - Relative dependency pinning in `pyproject.toml`.
 - Style and stability improvements (check `flake8` with `make check-style`).
 
 ### Removed
+
 - `requirements.txt` files to streamline in to `pyproject.toml`.
 
 ## [1.0.11](https://github.com/alexdlaird/amazon-orders/compare/1.0.10...1.0.11) - 2024-02-09
+
 ### Changed
+
 - `version` command now includes Python version and doesn't printer banner, for easy parsing.
 
 ## [1.0.10](https://github.com/alexdlaird/amazon-orders/compare/1.0.9...1.0.10) - 2024-02-08
+
 ### Added
+
 - Migrated to `pyproject.toml`.
 
 ## [1.0.9](https://github.com/alexdlaird/amazon-orders/compare/1.0.8...1.0.9) - 2024-02-07
+
 ### Added
-- [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.AuthForm)'s now passes `captcha_img_url` to its `prompt()` fallback for Captcha, useful for overriding [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
-- [MfaDeviceSelectForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.MfaDeviceSelectForm) now passes `mfa_device_select_choices` to `prompt()`, useful for overrides [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
+
+- [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.AuthForm)'s now
+  passes `captcha_img_url` to its `prompt()` fallback for Captcha, useful for
+  overriding [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
+- [MfaDeviceSelectForm](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.forms.MfaDeviceSelectForm)
+  now passes `mfa_device_select_choices` to `prompt()`, useful for
+  overrides [IODefault](https://amazon-orders.readthedocs.io/en/1.0.9/api.html#amazonorders.session.IODefault).
 - Documentation improvements.
 
 ## [1.0.8](https://github.com/alexdlaird/amazon-orders/compare/1.0.7...1.0.8) - 2024-01-30
+
 ### Added
+
 - Stability improvements.
 
 ## [1.0.7](https://github.com/alexdlaird/amazon-orders/compare/1.0.6...1.0.7) - 2024-01-29
+
 ### Added
-- [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.forms.AuthForm) abstract class, and migrated all auth flow items to subclasses of this class.
-- [Parsable.simple_parse()](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.entities.parsable.Parsable.simple_parse), which can handle most basic fields when parised with CSS selectors.
+
+- [AuthForm](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.forms.AuthForm) abstract class, and
+  migrated all auth flow items to subclasses of this class.
+- [Parsable.simple_parse()](https://amazon-orders.readthedocs.io/en/1.0.7/api.html#amazonorders.entities.parsable.Parsable.simple_parse),
+  which can handle most basic fields when parised with CSS selectors.
 - Stability improvements.
 - Test improvements.
 
 ### Changed
+
 - Moved all constant variables (URLs, CSS selectors, etc.) to `constants.py`.
 - Migrated entities to use CSS selector constants.
-- `constants.SIGN_IN_URL` is now the landing page for login, the old value has been moved to `constants.SIGN_IN_REDIRECT_URL`.
+- `constants.SIGN_IN_URL` is now the landing page for login, the old value has been moved
+  to `constants.SIGN_IN_REDIRECT_URL`.
 
 ## [1.0.6](https://github.com/alexdlaird/amazon-orders/compare/1.0.5...1.0.6) - 2024-01-25
+
 ### Added
+
 - Support for when local session data is stale (Amazon prompts us to login again).
 - Documentation improvements.
 
 ### Fixed
+
 - Regression in the Captcha flow introduced in `1.0.5`.
 
 ## [1.0.5](https://github.com/alexdlaird/amazon-orders/compare/1.0.4...1.0.5) - 2024-01-25
+
 ### Added
+
 - [Item.image_link](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.entity.item.Item.image_link).
 - [Item.quantity](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.entity.item.Item.quantity).
 - `version` command to CLI.
 - Test improvements.
 
 ### Changed
-- Migrated to using CSS selectors in [`AmazonSession`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.session.AmazonSession)
-- Migrated to using CSS selectors in [`AmazonOrders`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.orders.AmazonOrders)
+
+- Migrated to using CSS selectors
+  in [`AmazonSession`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.session.AmazonSession)
+- Migrated to using CSS selectors
+  in [`AmazonOrders`](https://amazon-orders.readthedocs.io/en/1.0.5/api.html#amazonorders.orders.AmazonOrders)
 
 ## [1.0.4](https://github.com/alexdlaird/amazon-orders/compare/1.0.3...1.0.4) - 2024-01-24
+
 ### Added
+
 - A new OTP auth flow from Amazon that can occur after Captcha.
 - Parameters `--max-auth-attempts` and `--output-dir` to CLI.
 - `DEFAULT_OUTPUT_DIR`, which defaults to `os.getcwd()`, but allows users to change where output files are written.
 - [`Troubleshooting`](https://amazon-orders.readthedocs.io/en/1.0.4/troubleshooting.html) section to the docs.
 - Test improvements, including the ability to run dynamic tests using private order data from JSON files.
 
 ### Changed
-- Improved string representations of entities, including [`Order`](https://amazon-orders.readthedocs.io/en/1.0.4/api.html#amazonorders.entity.order.Order), moved string representation of all fields back to `cli.py` out of the `__str__` method.
+
+- Improved string representations of entities,
+  including [`Order`](https://amazon-orders.readthedocs.io/en/1.0.4/api.html#amazonorders.entity.order.Order), moved
+  string representation of all fields back to `cli.py` out of the `__str__` method.
 - Moved `DEFAULT_COOKIE_JAR_PATH` to `conf.py`.
 
 ## [1.0.3](https://github.com/alexdlaird/amazon-orders/compare/1.0.2...1.0.3) - 2024-01-18
+
 ### Added
+
 - CLI improvements.
 - Documentation improvements.
 
 ## [1.0.2](https://github.com/alexdlaird/amazon-orders/compare/1.0.1...1.0.2) - 2024-01-18
+
 ### Added
+
 - `IODefault` for I/O operations, which can be extended to use something other than `print()` and `input()`.
 - Documentation improvements.
 - Test improvements.
 
 ### Removed
-- `Orders.print_output` variable, `cli.py` now handles output. 
+
+- `Orders.print_output` variable, `cli.py` now handles output.
 
 ## [1.0.1](https://github.com/alexdlaird/amazon-orders/compare/1.0.0...1.0.1) - 2024-01-17
+
 ### Added
+
 - Auth flow now also checks session cookies in addition to parsing the page for signs of login.
-- All fields to string representation of [`Order`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order), so they are not output on the CLI.
+- All fields to string representation
+  of [`Order`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order), so they are not
+  output on the CLI.
 - `logout` command to CLI.
 - Documentation improvements.
 - Test improvements.
 
 ### Fixed
+
 - Improvements to CLI, including error message cleanup on auth exceptions.
-- [`Order.order_details_link`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order.order_details_link) is now properly populated even on the details page.
+- [`Order.order_details_link`](https://amazon-orders.readthedocs.io/en/1.0.1/api.html#amazonorders.entity.order.Order.order_details_link)
+  is now properly populated even on the details page.
 - `.gitattributes` to HTML files are now ignore by Linguist.
 
 ## [1.0.0](https://github.com/alexdlaird/amazon-orders/releases/tag/1.0.0) - 2024-01-16
+
 - First stable release of `amazon-orders`.
```

### Comparing `amazon-orders-1.1.1/LICENSE` & `amazon_orders-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/PKG-INFO` & `amazon_orders-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-orders
-Version: 1.1.1
+Version: 1.1.2
 Summary: A CLI and library for interacting with Amazon order history.
 Maintainer-email: Alex Laird <contact@alexlaird.com>
 License: MIT License
         
         Copyright (c) 2024 Alex Laird
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 License-File: LICENSE
 Requires-Dist: click>=7.1
 Requires-Dist: requests>=2.23
 Requires-Dist: amazoncaptcha>=0.4
 Requires-Dist: beautifulsoup4>=4.8
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-pyproject; extra == "dev"
 Requires-Dist: pep8-naming; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: flask; extra == "dev"
 Requires-Dist: twilio; extra == "dev"
@@ -117,15 +118,18 @@
 
 for order in orders:
     print(f"{order.order_number} - {order.grand_total}")
 ```
 
 ## Documentation
 
-For more advanced usage, `amazon-orders`'s official documentation is available at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
+For more advanced usage, `amazon-orders`'s official documentation is available
+at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
 
 ## Contributing
 
-If you would like to get involved, be sure to review the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
+If you would like to get involved, be sure to review
+the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
 
-Want to contribute financially? If you've found `amazon-orders` useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
+Want to contribute financially? If you've found `amazon-orders`
+useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
 also be greatly appreciated!
```

### Comparing `amazon-orders-1.1.1/README.md` & `amazon_orders-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,18 @@
 
 for order in orders:
     print(f"{order.order_number} - {order.grand_total}")
 ```
 
 ## Documentation
 
-For more advanced usage, `amazon-orders`'s official documentation is available at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
+For more advanced usage, `amazon-orders`'s official documentation is available
+at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
 
 ## Contributing
 
-If you would like to get involved, be sure to review the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
+If you would like to get involved, be sure to review
+the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
 
-Want to contribute financially? If you've found `amazon-orders` useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
+Want to contribute financially? If you've found `amazon-orders`
+useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
 also be greatly appreciated!
```

### Comparing `amazon-orders-1.1.1/amazon_orders.egg-info/PKG-INFO` & `amazon_orders-1.1.2/amazon_orders.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-orders
-Version: 1.1.1
+Version: 1.1.2
 Summary: A CLI and library for interacting with Amazon order history.
 Maintainer-email: Alex Laird <contact@alexlaird.com>
 License: MIT License
         
         Copyright (c) 2024 Alex Laird
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 License-File: LICENSE
 Requires-Dist: click>=7.1
 Requires-Dist: requests>=2.23
 Requires-Dist: amazoncaptcha>=0.4
 Requires-Dist: beautifulsoup4>=4.8
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: parameterized; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-pyproject; extra == "dev"
 Requires-Dist: pep8-naming; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: flask; extra == "dev"
 Requires-Dist: twilio; extra == "dev"
@@ -117,15 +118,18 @@
 
 for order in orders:
     print(f"{order.order_number} - {order.grand_total}")
 ```
 
 ## Documentation
 
-For more advanced usage, `amazon-orders`'s official documentation is available at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
+For more advanced usage, `amazon-orders`'s official documentation is available
+at [http://amazon-orders.readthedocs.io](http://amazon-orders.readthedocs.io).
 
 ## Contributing
 
-If you would like to get involved, be sure to review the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
+If you would like to get involved, be sure to review
+the [Contribution Guide](https://github.com/alexdlaird/amazon-orders/blob/main/CONTRIBUTING.rst).
 
-Want to contribute financially? If you've found `amazon-orders` useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
+Want to contribute financially? If you've found `amazon-orders`
+useful, [sponsorship](https://github.com/sponsors/alexdlaird) would
 also be greatly appreciated!
```

### Comparing `amazon-orders-1.1.1/amazon_orders.egg-info/SOURCES.txt` & `amazon_orders-1.1.2/amazon_orders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/banner.txt` & `amazon_orders-1.1.2/amazonorders/banner.txt`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/cli.py` & `amazon_orders-1.1.2/amazonorders/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 -----------------------------------------------------------------------\n"""
                    .format(year=year,
                            optional_start_index=optional_start_index,
                            optional_full_details=optional_full_details))
         click.echo("Info: This might take a minute ...\n")
 
         amazon_orders = AmazonOrders(amazon_session,
-                                     debug=amazon_session.debug,
                                      output_dir=ctx.obj["output_dir"])
 
         orders = amazon_orders.get_order_history(year=kwargs["year"],
                                                  start_index=kwargs[
                                                      "start_index"],
                                                  full_details=kwargs[
                                                      "full_details"], )
@@ -154,15 +153,14 @@
     """
     amazon_session = ctx.obj["amazon_session"]
 
     try:
         _authenticate(ctx, amazon_session)
 
         amazon_orders = AmazonOrders(amazon_session,
-                                     debug=amazon_session.debug,
                                      output_dir=ctx.obj["output_dir"])
 
         order = amazon_orders.get_order(order_id)
 
         click.echo(f"{_order_output(order)}\n")
     except AmazonOrdersError as e:
         logger.debug("An error occurred.", exc_info=True)
```

### Comparing `amazon-orders-1.1.1/amazonorders/constants.py` & `amazon_orders-1.1.2/amazonorders/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/entity/item.py` & `amazon_orders-1.1.2/amazonorders/entity/item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 import logging
-from datetime import datetime, date
+from datetime import date, datetime
 from typing import Optional
 
 from bs4 import Tag
 
 from amazonorders import constants
 from amazonorders.entity.parsable import Parsable
 from amazonorders.entity.seller import Seller
@@ -53,15 +53,15 @@
 
     def _parse_price(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ITEM_TAG_ITERATOR_SELECTOR):
             price = tag.text.strip()
             if price.startswith("$"):
-                value = float(price.replace("$", ""))
+                value = float(price.replace("$", "").replace(",", ""))
 
         return value
 
     def _parse_seller(self) -> Optional[Seller]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ITEM_TAG_ITERATOR_SELECTOR):
```

### Comparing `amazon-orders-1.1.1/amazonorders/entity/order.py` & `amazon_orders-1.1.2/amazonorders/entity/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 import json
 import logging
-from datetime import datetime, date
+from datetime import date, datetime
 from typing import List, Optional, TypeVar
-from urllib.parse import urlparse, parse_qs
+from urllib.parse import parse_qs, urlparse
 
 from bs4 import BeautifulSoup, Tag
 
 from amazonorders import constants
 from amazonorders.entity.item import Item
 from amazonorders.entity.parsable import Parsable
 from amazonorders.entity.recipient import Recipient
@@ -120,15 +120,15 @@
             for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
                 if "grand total" in tag.text.lower():
                     inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                     if inner_tag:
                         value = inner_tag.text.strip()
                         break
 
-        value = float(value.replace("$", ""))
+        value = float(value.replace("$", "").replace(",", ""))
 
         return value
 
     def _parse_order_placed_date(self) -> date:
         value = self.simple_parse(constants.FIELD_ORDER_PLACED_DATE_SELECTOR)
 
         if "Ordered on" in value:
@@ -184,75 +184,75 @@
     def _parse_subtotal(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "subtotal" in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_shipping_total(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "shipping" in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_subscription_discount(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "subscribe" in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_total_before_tax(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "before tax" in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_estimated_tax(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "estimated tax" in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_refund_total(self) -> Optional[float]:
         value = None
 
         for tag in self.parsed.select(constants.FIELD_ORDER_SUBTOTALS_TAG_ITERATOR_SELECTOR):
             if "refund total" in tag.text.lower() and "tax refund" not in tag.text.lower():
                 inner_tag = tag.select_one(constants.FIELD_ORDER_SUBTOTALS_INNER_TAG_SELECTOR)
                 if inner_tag:
-                    value = float(inner_tag.text.strip().replace("$", ""))
+                    value = float(inner_tag.text.strip().replace("$", "").replace(",", ""))
                     break
 
         return value
 
     def _parse_order_shipping_date(self) -> Optional[date]:
         match_text = "Items shipped:"
         value = self.simple_parse(constants.FIELD_ORDER_SHIPPED_DATE_SELECTOR, text_contains=match_text)
```

### Comparing `amazon-orders-1.1.1/amazonorders/entity/parsable.py` & `amazon_orders-1.1.2/amazonorders/entity/parsable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 import logging
-from typing import Callable, Any, Optional, Type, Union
+from typing import Any, Callable, Optional, Type, Union
 
 from bs4 import Tag
 
 from amazonorders.constants import BASE_URL
-from amazonorders.exception import AmazonOrdersError, AmazonOrderEntityError
+from amazonorders.exception import AmazonOrderEntityError, AmazonOrdersError
 
 logger = logging.getLogger(__name__)
 
 
 class Parsable:
     """
     A base class that contains a parsed representation of the entity, and can be extended to
```

### Comparing `amazon-orders-1.1.1/amazonorders/entity/recipient.py` & `amazon_orders-1.1.2/amazonorders/entity/recipient.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/entity/seller.py` & `amazon_orders-1.1.2/amazonorders/entity/seller.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/entity/shipment.py` & `amazon_orders-1.1.2/amazonorders/entity/shipment.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/amazonorders/forms.py` & `amazon_orders-1.1.2/amazonorders/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 from abc import ABC
 from io import BytesIO
-from typing import Optional, Dict, Any
+from typing import Any, Dict, Optional
 from urllib.parse import urlparse
 
 from PIL import Image
 from amazoncaptcha import AmazonCaptcha
 from bs4 import Tag
 
 from amazonorders import constants
-from amazonorders.exception import AmazonOrdersError, AmazonOrdersAuthError
+from amazonorders.exception import AmazonOrdersAuthError, AmazonOrdersError
 
 
 class AuthForm(ABC):
     """
     The base class of an authentication ``<form>`` that can be submitted.
 
     The base implementation will attempt to auto-solve Captcha. If this fails, it will
```

### Comparing `amazon-orders-1.1.1/amazonorders/orders.py` & `amazon_orders-1.1.2/amazonorders/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 import datetime
 import logging
 from typing import List, Optional
 
 from amazonorders import constants
 from amazonorders.conf import DEFAULT_OUTPUT_DIR
 from amazonorders.entity.order import Order
-from amazonorders.exception import AmazonOrdersError
+from amazonorders.exception import AmazonOrdersError, AmazonOrdersNotFoundError
 from amazonorders.session import AmazonSession
 
 logger = logging.getLogger(__name__)
 
 
 class AmazonOrders:
     """
     Using an authenticated :class:`~amazonorders.session.AmazonSession`, can be used to query Amazon
     for Order details and history.
     """
 
     def __init__(self,
                  amazon_session: AmazonSession,
-                 debug: bool = False,
+                 debug: Optional[bool] = None,
                  output_dir: Optional[str] = None) -> None:
+        if not debug:
+            debug = amazon_session.debug
         if not output_dir:
             output_dir = DEFAULT_OUTPUT_DIR
 
         #: The AmazonSession to use for requests.
         self.amazon_session: AmazonSession = amazon_session
 
         #: Set logger ``DEBUG`` and send output to ``stderr``.
@@ -101,13 +103,15 @@
         :param order_id: The Amazon Order ID to lookup.
         :return: The requested Order.
         """
         if not self.amazon_session.is_authenticated:
             raise AmazonOrdersError("Call AmazonSession.login() to authenticate first.")
 
         self.amazon_session.get(f"{constants.ORDER_DETAILS_URL}?orderID={order_id}")
+        if not self.amazon_session.last_response.url.startswith(constants.ORDER_DETAILS_URL):
+            raise AmazonOrdersNotFoundError(f"Amazon redirected, which likely means Order {order_id} was not found")
 
         order_details_tag = self.amazon_session.last_response_parsed.select_one(
             constants.ORDER_DETAILS_ENTITY_SELECTOR)
         order = Order(order_details_tag, full_details=True)
 
         return order
```

### Comparing `amazon-orders-1.1.1/amazonorders/session.py` & `amazon_orders-1.1.2/amazonorders/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 import json
 import logging
 import os
-from typing import Optional, Any
+from typing import Any, Optional
 from urllib.parse import urlparse
 
 import requests
 from bs4 import BeautifulSoup, Tag
-from requests import Session, Response
+from requests import Response, Session
 from requests.utils import dict_from_cookiejar
 
 from amazonorders import constants
 from amazonorders.conf import DEFAULT_COOKIE_JAR_PATH, DEFAULT_OUTPUT_DIR
 from amazonorders.exception import AmazonOrdersAuthError
-from amazonorders.forms import SignInForm, MfaDeviceSelectForm, MfaForm, CaptchaForm
+from amazonorders.forms import CaptchaForm, MfaDeviceSelectForm, MfaForm, SignInForm
 
 logger = logging.getLogger(__name__)
 
 AUTH_FORMS = [SignInForm(),
               MfaDeviceSelectForm(),
               MfaForm(),
               CaptchaForm(),
```

### Comparing `amazon-orders-1.1.1/pyproject.toml` & `amazon_orders-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
+    "parameterized",
     "coverage[toml]",
     "flake8",
     "flake8-pyproject",
     "pep8-naming",
     "responses",
     "flask",
     "twilio",
```

### Comparing `amazon-orders-1.1.1/tests/test_cli.py` & `amazon_orders-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/tests/test_orders.py` & `amazon_orders-1.1.2/tests/test_orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __copyright__ = "Copyright (c) 2024 Alex Laird"
 __license__ = "MIT"
 
 import os
 
 import responses
 
-from amazonorders.constants import ORDER_HISTORY_URL, ORDER_DETAILS_URL
+from amazonorders.constants import ORDER_DETAILS_URL, ORDER_HISTORY_URL
 from amazonorders.exception import AmazonOrdersError
 from amazonorders.orders import AmazonOrders
 from amazonorders.session import AmazonSession
 from tests.unittestcase import UnitTestCase
 
 
 class TestOrders(UnitTestCase):
```

### Comparing `amazon-orders-1.1.1/tests/test_session.py` & `amazon_orders-1.1.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `amazon-orders-1.1.1/tests/testcase.py` & `amazon_orders-1.1.2/tests/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             self.assertEqual(4, len(order.payment_method_last_4))
             self.assertEqual(30.99, order.subtotal)
             self.assertEqual(0.00, order.shipping_total)
             self.assertIsNone(order.subscription_discount)
             self.assertEqual(30.99, order.total_before_tax)
             self.assertEqual(3.02, order.estimated_tax)
             self.assertEqual(date(2018, 12, 28), order.order_shipped_date)
-            self.assertEqual("New", order.items[0].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertEqual("New", order.items[0].condition)
             self.assertEqual(30.99, order.items[0].price)
             self.assertEqual("Amazon.com Services, Inc",
                              order.items[0].seller.name)
             self.assertIsNone(order.items[0].seller.link)
 
     def assert_order_114_9460922_7737063(self, order, full_details):
         self.assertEqual(35.90, order.grand_total)
@@ -69,15 +70,16 @@
             self.assertEqual(4, len(order.payment_method_last_4))
             self.assertEqual(38.84, order.subtotal)
             self.assertEqual(0.00, order.shipping_total)
             self.assertEqual(-5.83, order.subscription_discount)
             self.assertEqual(33.01, order.total_before_tax)
             self.assertEqual(2.89, order.estimated_tax)
             self.assertEqual(date(2020, 10, 28), order.order_shipped_date)
-            self.assertEqual("New", order.items[0].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertEqual("New", order.items[0].condition)
             self.assertEqual(38.84, order.items[0].price)
             self.assertEqual("Amazon.com Services, Inc",
                              order.items[0].seller.name)
             self.assertIsNone(order.items[0].seller.link)
 
     def assert_order_112_2961628_4757846_return(self, order, full_details):
         self.assertEqual(76.11, order.grand_total)
@@ -107,15 +109,16 @@
             self.assertEqual(0.00, order.shipping_total)
             self.assertIsNone(order.subscription_discount)
             self.assertEqual(69.99, order.total_before_tax)
             self.assertEqual(6.12, order.estimated_tax)
             self.assertEqual(76.11, order.refund_total)
             self.assertEqual(date(2020, 10, 19), order.order_shipped_date)
             self.assertTrue(date(2020, 11, 2), order.refund_completed_date)
-            self.assertEqual("New", order.items[0].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertEqual("New", order.items[0].condition)
             self.assertEqual(69.99, order.items[0].price)
             self.assertEqual("Amazon.com Services, Inc",
                              order.items[0].seller.name)
             self.assertIsNone(order.items[0].seller.link)
 
     def assert_order_112_8888666_5244209_quantity(self, order):
         self.assertEqual("112-8888666-5244209", order.order_number)
@@ -180,17 +183,19 @@
             self.assertEqual(4, len(order.payment_method_last_4))
             self.assertEqual(43.23, order.subtotal)
             self.assertEqual(0.00, order.shipping_total)
             self.assertIsNone(order.subscription_discount)
             self.assertEqual(43.23, order.total_before_tax)
             self.assertEqual(3.38, order.estimated_tax)
             self.assertEqual(date(2023, 12, 7), order.order_shipped_date)
-            self.assertEqual("New", order.items[0].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertEqual("New", order.items[0].condition)
             self.assertEqual(14.99, order.items[0].price)
-            self.assertEqual("New", order.items[1].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertEqual("New", order.items[1].condition)
             self.assertEqual(28.24, order.items[1].price)
             found_cadeya = False
             found_amazon = False
             for order_item in order.items:
                 seller = order_item.seller
                 if "Cadeya" in seller.name:
                     found_cadeya = True
@@ -247,22 +252,24 @@
             self.assertEqual(2.32, order.estimated_tax)
             self.assertEqual(date(2020, 10, 27), order.order_shipped_date)
             found_aa = False
             found_aaa = False
             for item in order.items:
                 if "AAA" in item.title:
                     found_aa = True
-                    self.assertEqual("New", item.condition)
+                    # As of April 2024, this is no longer shown in Order History
+                    # self.assertEqual("New", item.condition)
                     self.assertEqual(10.99, item.price)
                     self.assertEqual("Amazon.com Services, Inc",
                                      item.seller.name)
                     self.assertIsNone(item.seller.link)
                 else:
                     found_aaa = True
-                    self.assertEqual("New", item.condition)
+                    # As of April 2024, this is no longer shown in Order History
+                    # self.assertEqual("New", item.condition)
                     self.assertEqual(15.49, item.price)
                     self.assertEqual("Amazon.com Services, Inc",
                                      item.seller.name)
                     self.assertIsNone(item.seller.link)
             self.assertTrue(found_aa)
             self.assertTrue(found_aaa)
 
@@ -284,10 +291,11 @@
         if full_details:
             self.assertIsNotNone(order.payment_method)
             self.assertEqual(4, len(order.payment_method_last_4))
             self.assertIsNotNone(order.subtotal)
             self.assertIsNotNone(order.shipping_total)
             self.assertIsNotNone(order.total_before_tax)
             self.assertIsNotNone(order.estimated_tax)
-            self.assertIsNotNone(order.items[0].condition)
+            # As of April 2024, this is no longer shown in Order History
+            # self.assertIsNotNone(order.items[0].condition)
             self.assertIsNotNone(order.items[0].price)
             self.assertIsNotNone(order.items[0].seller.name)
```

