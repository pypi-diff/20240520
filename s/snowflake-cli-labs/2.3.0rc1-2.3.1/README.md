# Comparing `tmp/snowflake_cli_labs-2.3.0rc1.tar.gz` & `tmp/snowflake_cli_labs-2.3.1.tar.gz`

## Comparing `snowflake_cli_labs-2.3.0rc1.tar` & `snowflake_cli_labs-2.3.1.tar`

### file list

```diff
@@ -1,581 +1,582 @@
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/RELEASE-NOTES.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/SECURITY.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/conftest.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/performance_history_analysis.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/docs/images/coverage_5.png
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/scripts/main.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/snyk/dependency-sync.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/snyk/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/cli_global_context.py
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/config.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/constants.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/exceptions.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/feature_flags.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/secure_path.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/secure_utils.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/sql_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/alias.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/decorators.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/experimental_behaviour.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/flags.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/project_initialisation.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/snow_typer.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/abc.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/console.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/output/formats.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/output/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/plugins/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/plugins/plugin_config.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/plugins/command/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/__init__.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/definition.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/definition_manager.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/errors.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/project_definition.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/updatable_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/__init__.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/application.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/native_app.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/package.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/argument.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/callable.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/cursor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/error_handling.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/naming_utils.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/path_utils.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/rendering.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/types.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/__main__.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/cli_app.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/constants.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/loggers.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/main_typer.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/printing.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/snow_connector.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/api_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/api_impl/plugin/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/builtin_plugins.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/exception_logging.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/threadsafe.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/typer_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/commands_structure.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/pycharm_remote_debug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/generator.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/__init__.py
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/commands.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/plugin_spec.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/__init__.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/commands.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/manager.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/__init__.py
--rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/artifacts.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/commands.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/common_flags.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/constants.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/exceptions.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/feature_flags.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/init.py
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/policy.py
--rw-r--r--   0        0        0    12493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/run_processor.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/codegen/__init__.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/version/__init__.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/version/commands.py
--rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/notebook/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/notebook/commands.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/notebook/manager.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/notebook/plugin_spec.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/__init__.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/commands.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/common.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/plugin_spec.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/__init__.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/commands.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/common.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/manager.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/models.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package_utils.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/plugin_spec.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/zipper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/__init__.py
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/commands.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/manager.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/utils.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/common.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_registry/commands.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_registry/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_repository/commands.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_repository/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/jobs/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/jobs/commands.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/jobs/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/services/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/services/commands.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/services/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/__init__.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/commands.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/manager.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/plugin_spec.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/snowsql_templating.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/__init__.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/commands.py
--rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/diff.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/manager.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/commands.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/plugin_spec.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/environment.yml.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/.gitignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/app/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/app/common.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/app/functions.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/app/procedures.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/.gitignore
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/environment.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/snowflake.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/common/hello.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/broken_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/failing_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/override_build_in_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/empty_config.toml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_cli.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_command_registration.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_common_decorators.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_common_global_context.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_config.py
--rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_connection.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_experimental_behaviour.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_help_messages.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_loaded_modules.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_logs.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_main.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_performance.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_project_initialisation.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_snow_connector.py
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_sql.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_utils.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_zipper.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0   554299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_help_messages.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/test_feature_flags.py
--rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/test_secure_path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/commands/__init__.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/commands/test_flags.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/commands/test_snow_typer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/commands/__snapshots__/test_flags.ambr
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/commands/__snapshots__/test_snow_typer.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/console/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/console/test_cli_console_output.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/console/test_console_abc.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/console/test_intermediate_output.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/utils/test_naming_utils.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/api/utils/test_rendering.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/app/test_telemetry.py
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/git/test_git_commands.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/git/__snapshots__/test_git_commands.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/patch_utils.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_annotation_processor_config.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_artifacts.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_commands.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_feature_flags.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_init.py
--rw-r--r--   0        0        0    26124 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_manager.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_package_scripts.py
--rw-r--r--   0        0        0    43940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_run_processor.py
--rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_teardown_processor.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_utils.py
--rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_version_create_processor.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_version_drop_processor.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/utils.py
--rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/__snapshots__/test_commands.ambr
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/__snapshots__/test_init.ambr
--rw-r--r--   0        0        0    21526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/nativeapp/codegen/test_sandbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/notebook/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/notebook/test_notebook_commands.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/notebook/test_notebook_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/object/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/object/test_common.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/object/test_object.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/object/test_stage.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/object/__snapshots__/test_object.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/output/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/output/test_format_silent_enforcement.py
--rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/output/test_printing.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/output/test_silent_output.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/plugin/test_broken_plugin.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/plugin/test_failing_plugin.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/plugin/test_override_by_external_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/fixtures.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/test_config.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/test_definition_manager.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/test_project_schemas.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/test_util.py
--rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/project/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/mocks.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_anaconda.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_build.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_common.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_function.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_models.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_package.py
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_procedure.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_procedure.ambr
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_common.py
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_image_repository.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_jobs.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_registry.py
--rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/test_services.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/__snapshots__/test_image_repository.ambr
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/spcs/__snapshots__/test_registry.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/stage/__init__.py
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/stage/test_diff.py
--rw-r--r--   0        0        0    30692 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/stage/test_stage.py
--rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/stage/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/streamlit/test_commands.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/streamlit/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/test_data.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/configs/broken_plugin_config.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/configs/disabled_override_plugin_config.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/configs/failing_plugin_config.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/configs/override_plugin_config.toml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure/core/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
--rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
--rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/empty_project/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit/environment.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit/pages/my_page.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_defaults/main.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_stage/environment.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/snowflake.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/package/002-shared.sql
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/snowflake.local.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/snowflake.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/package/002-shared.sql
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/minimal/snowflake.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/setup.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_1/app/streamlit/main.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/no_definition_version/snowflake.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_external_access/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_external_access/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_external_access/requirements.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_functions/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_functions/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_functions/requirements.txt
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_functions/snowflake.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_external_access/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_external_access/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/requirements.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures_coverage/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures_coverage/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/streamlit_full_definition/environment.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/streamlit_full_definition/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/streamlit_full_definition/utils/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/underspecified/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/unknown_fields/snowflake.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/streamlit/another_file_with_list.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/streamlit/another_file_with_single_item.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/streamlit/with_list_in_source_file.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/test_data/streamlit/with_single_item.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/testing_utils/conversion.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/testing_utils/files_and_dirs.py
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/testing_utils/fixtures.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/conftest.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/test_error_handling.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/test_installation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/test_snowpark_examples.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/__snapshots__/test_installation.ambr
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/config/config.toml
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_e2e/config/malformatted_config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/conftest.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_config.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_connection.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_external_plugins.py
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_git.py
--rw-r--r--   0        0        0    30602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_nativeapp.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_notebooks.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_object.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_package.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_session_token.py
--rw-r--r--   0        0        0    28873 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_snowpark.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_snowpark_external_access.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_sql.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_stage.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_streamlit.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_temporary_connection.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_utils.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_git.ambr
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_sql.ambr
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/config/config_with_enabled_all_external_plugins.toml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/scripts/integration_account_setup.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_image_repository.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_jobs.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_registry.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_services.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/docker/Dockerfile
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/docker/bootstrap_containers_setup.sh
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/docker/echo_service.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/spec/spec.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/spec/spec_upgrade.yml
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/compute_pool_utils.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/spcs_services_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/sql_multi_queries.sql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/requirements.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_version_check/.gitignore
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_version_check/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_import/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_execute/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_execute/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_execute/script3.sql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_execute/script_template.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/streamlit/environment.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/streamlit/snowflake.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/streamlit/pages/my_page.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/streamlit/utils/utils.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/naming_utils.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/snowpark_utils.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/sql_utils.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/working_directory_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/assertions/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/assertions/test_file_assertions.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/assertions/test_result_assertions.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/LICENSE
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/README.md
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17608 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/RELEASE-NOTES.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/SECURITY.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/conftest.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/performance_history_analysis.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/docs/images/coverage_5.png
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/scripts/main.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/snyk/dependency-sync.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/snyk/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/cli_global_context.py
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/config.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/constants.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/exceptions.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/feature_flags.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_path.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_utils.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/sql_execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/alias.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/decorators.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/experimental_behaviour.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/flags.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/project_initialisation.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/snow_typer.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/abc.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/console.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/formats.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/plugin_config.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/__init__.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition_manager.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/errors.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/project_definition.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/updatable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/application.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/native_app.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/package.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/argument.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/callable.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/cursor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/error_handling.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/naming_utils.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/path_utils.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/rendering.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/types.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/__main__.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/cli_app.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/constants.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/loggers.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/main_typer.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/printing.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/snow_connector.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/builtin_plugins.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/exception_logging.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/threadsafe.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/typer_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/commands_structure.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/pycharm_remote_debug.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/generator.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/__init__.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/commands.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/plugin_spec.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/commands.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/manager.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/__init__.py
+-rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/artifacts.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/commands.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/common_flags.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/constants.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/exceptions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/feature_flags.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/init.py
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/policy.py
+-rw-r--r--   0        0        0    13103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/run_processor.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/__init__.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/__init__.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/commands.py
+-rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/commands.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/manager.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/plugin_spec.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/__init__.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/commands.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/common.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/plugin_spec.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/__init__.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/commands.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/common.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/manager.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/models.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package_utils.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/plugin_spec.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/zipper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/__init__.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/commands.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/utils.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/common.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/commands.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/commands.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/commands.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/commands.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/__init__.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/commands.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/manager.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/plugin_spec.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/snowsql_templating.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/__init__.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/commands.py
+-rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/diff.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/manager.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/__init__.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/commands.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/plugin_spec.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/environment.yml.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/.gitignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/common.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/functions.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/procedures.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/.gitignore
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/environment.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/snowflake.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/common/hello.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/empty_config.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_command_registration.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_common_decorators.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_common_global_context.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_config.py
+-rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_connection.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_experimental_behaviour.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_help_messages.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_loaded_modules.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_logs.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_main.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_performance.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_project_initialisation.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_snow_connector.py
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_sql.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_zipper.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0   554299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/__snapshots__/test_help_messages.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/test_feature_flags.py
+-rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/test_secure_path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__init__.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/test_flags.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/test_snow_typer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_flags.ambr
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_snow_typer.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_cli_console_output.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_console_abc.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/console/test_intermediate_output.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/utils/test_naming_utils.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/api/utils/test_rendering.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/app/test_telemetry.py
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/git/test_git_commands.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/git/__snapshots__/test_git_commands.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/patch_utils.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_annotation_processor_config.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_artifacts.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_commands.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_feature_flags.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_init.py
+-rw-r--r--   0        0        0    26124 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_manager.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_package_scripts.py
+-rw-r--r--   0        0        0    43980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_run_processor.py
+-rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_teardown_processor.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_utils.py
+-rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_create_processor.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_drop_processor.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/utils.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_commands.ambr
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_init.ambr
+-rw-r--r--   0        0        0    21526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/nativeapp/codegen/test_sandbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_commands.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_common.py
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_object.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/test_stage.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/object/__snapshots__/test_object.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_format_silent_enforcement.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/output/test_silent_output.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_broken_plugin.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_failing_plugin.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/plugin/test_override_by_external_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/fixtures.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_config.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_definition_manager.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_project_schemas.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/test_util.py
+-rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/project/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/mocks.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_anaconda.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_build.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_common.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_function.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_models.py
+-rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_package.py
+-rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/test_procedure.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure.ambr
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_common.py
+-rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_image_repository.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_jobs.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_registry.py
+-rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/test_services.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_image_repository.ambr
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_registry.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/__init__.py
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/test_diff.py
+-rw-r--r--   0        0        0    30692 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/test_stage.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/stage/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/streamlit/test_commands.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/streamlit/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/broken_plugin_config.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/disabled_override_plugin_config.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/failing_plugin_config.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/configs/override_plugin_config.toml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure/core/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/empty_project/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/environment.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/main.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/environment.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/snowflake.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/package/002-shared.sql
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/snowflake.local.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/snowflake.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/package/002-shared.sql
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/minimal/snowflake.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/setup.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_1/app/streamlit/main.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/no_definition_version/snowflake.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/requirements.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/requirements.txt
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/snowflake.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/environment.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/streamlit_full_definition/utils/utils.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/underspecified/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/projects/unknown_fields/snowflake.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/another_file_with_list.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/another_file_with_single_item.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/with_list_in_source_file.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/test_data/streamlit/with_single_item.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/conversion.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/fixtures.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/conftest.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_error_handling.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_installation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/test_snowpark_examples.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/__snapshots__/test_installation.ambr
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/config/config.toml
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_e2e/config/malformatted_config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/conftest.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_config.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_connection.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_external_plugins.py
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_git.py
+-rw-r--r--   0        0        0    30602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_nativeapp.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_notebooks.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_object.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_package.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_session_token.py
+-rw-r--r--   0        0        0    28873 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_snowpark.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_snowpark_external_access.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_temporary_connection.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_git.ambr
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/config_with_enabled_all_external_plugins.toml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/nativeapp/test_version.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/scripts/integration_account_setup.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_image_repository.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_jobs.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_registry.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/test_services.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/Dockerfile
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/bootstrap_containers_setup.sh
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/echo_service.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/spec/spec.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/spec/spec_upgrade.yml
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/compute_pool_utils.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_services_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/sql_multi_queries.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/requirements.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_version_check/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script3.sql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_execute/script_template.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/environment.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/snowflake.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/streamlit/utils/utils.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/snowpark_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/README.md
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.1/PKG-INFO
```

### Comparing `snowflake_cli_labs-2.3.0rc1/.pre-commit-config.yaml` & `snowflake_cli_labs-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/CONTRIBUTING.md` & `snowflake_cli_labs-2.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/RELEASE-NOTES.md` & `snowflake_cli_labs-2.3.1/RELEASE-NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Unreleased version
-
+# v2.3.1
 ## Backward incompatibility
 
 ## Deprecations
 
 ## New additions
 
 ## Fixes and improvements
-
+* Improved support for quoted identifiers.
+* Fixed bugs in source artifact mapping logic for native applications
 
 # v2.3.0
 
 ## Backward incompatibility
 
 ## Deprecations
```

### Comparing `snowflake_cli_labs-2.3.0rc1/conftest.py` & `snowflake_cli_labs-2.3.1/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/performance_history_analysis.py` & `snowflake_cli_labs-2.3.1/performance_history_analysis.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/docs/images/coverage_1.png` & `snowflake_cli_labs-2.3.1/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/docs/images/coverage_2.png` & `snowflake_cli_labs-2.3.1/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/docs/images/coverage_3.png` & `snowflake_cli_labs-2.3.1/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/docs/images/coverage_4.png` & `snowflake_cli_labs-2.3.1/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/docs/images/coverage_5.png` & `snowflake_cli_labs-2.3.1/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/scripts/main.py` & `snowflake_cli_labs-2.3.1/scripts/main.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/__init__.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/cli_global_context.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/cli_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/config.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/constants.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/exceptions.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/feature_flags.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/secure_path.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/secure_utils.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/secure_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/sql_execution.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/sql_execution.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/decorators.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/flags.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/project_initialisation.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/commands/snow_typer.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/commands/snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/abc.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/console/console.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/console/console.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/output/types.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/output/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/plugins/command/__init__.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/plugins/command/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/definition.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/definition_manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/errors.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/util.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/project_definition.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/project_definition.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/updatable_model.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/updatable_model.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/application.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/application.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/native_app.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/native_app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/package.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/callable.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/callable.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/cursor.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/naming_utils.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/path_utils.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/rendering.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/api/utils/types.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/api/utils/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/cli_app.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/loggers.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/loggers.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/main_typer.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/main_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/printing.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/snow_connector.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/telemetry.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/builtin_plugins.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/builtin_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/command_plugins_loader.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/threadsafe.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/threadsafe.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/commands_registration/typer_registration.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/commands_registration/typer_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/commands_structure.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/commands_structure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/pycharm_remote_debug.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/pycharm_remote_debug.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/generator.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/connection/util.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/connection/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/git/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/git/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/artifacts.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/artifacts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/common_flags.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/common_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/constants.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 ALLOWED_SPECIAL_COMMENTS = {SPECIAL_COMMENT, SPECIAL_COMMENT_OLD}
 LOOSE_FILES_MAGIC_VERSION = "UNVERSIONED"
 
 NAME_COL = "name"
 COMMENT_COL = "comment"
 OWNER_COL = "owner"
 VERSION_COL = "version"
+PATCH_COL = "patch"
 
 INTERNAL_DISTRIBUTION = "internal"
 EXTERNAL_DISTRIBUTION = "external"
 
 ERROR_MESSAGE_2043 = "Object does not exist, or operation cannot be performed."
 ERROR_MESSAGE_606 = "No active warehouse selected in the current session."
```

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/exceptions.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/init.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/policy.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/policy.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/run_processor.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/run_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 from typing import Optional
 
 import typer
 from click import UsageError
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
 from snowflake.cli.api.project.schemas.native_app.native_app import NativeApp
+from snowflake.cli.api.project.util import (
+    identifier_to_show_like_pattern,
+    unquote_identifier,
+)
+from snowflake.cli.api.utils.cursor import find_all_rows
 from snowflake.cli.plugins.nativeapp.constants import (
     ALLOWED_SPECIAL_COMMENTS,
     COMMENT_COL,
     LOOSE_FILES_MAGIC_VERSION,
+    PATCH_COL,
     SPECIAL_COMMENT,
     VERSION_COL,
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationAlreadyExistsError,
     ApplicationPackageDoesNotExistError,
 )
@@ -24,15 +30,15 @@
     ensure_correct_owner,
     generic_sql_error_handler,
 )
 from snowflake.cli.plugins.nativeapp.policy import PolicyBase
 from snowflake.cli.plugins.stage.diff import DiffResult
 from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector import ProgrammingError
-from snowflake.connector.cursor import SnowflakeCursor
+from snowflake.connector.cursor import DictCursor, SnowflakeCursor
 
 UPGRADE_RESTRICTION_CODES = {93044, 93055, 93045, 93046}
 
 
 class NativeAppRunProcessor(NativeAppManager, NativeAppCommandProcessor):
     def __init__(self, project_definition: NativeApp, project_root: Path):
         super().__init__(project_definition, project_root)
@@ -130,32 +136,42 @@
             if show_obj_cursor.rowcount is None:
                 raise SnowflakeSQLExecutionError(show_obj_query)
 
             return show_obj_cursor
 
     def get_existing_version_info(self, version: str) -> Optional[dict]:
         """
-        Get an existing version, if defined, by the same name in an application package.
-        It executes a 'show versions like ... in application package' query and returns the result as single row, if one exists.
+        Get the latest patch on an existing version by name in the application package.
+        Executes 'show versions like ... in application package' query and returns
+        the latest patch in the version as a single row, if one exists. Otherwise,
+        returns None.
         """
         with self.use_role(self.package_role):
             try:
-                version_obj = self.show_specific_object(
-                    "versions",
-                    version,
-                    name_col=VERSION_COL,
-                    in_clause=f"in application package {self.package_name}",
+                query = f"show versions like {identifier_to_show_like_pattern(version)} in application package {self.package_name}"
+                cursor = self._execute_query(query, cursor_class=DictCursor)
+
+                if cursor.rowcount is None:
+                    raise SnowflakeSQLExecutionError(query)
+
+                matching_rows = find_all_rows(
+                    cursor, lambda row: row[VERSION_COL] == unquote_identifier(version)
                 )
+
+                if not matching_rows:
+                    return None
+
+                return max(matching_rows, key=lambda row: row[PATCH_COL])
+
             except ProgrammingError as err:
                 if err.msg.__contains__("does not exist or not authorized"):
                     raise ApplicationPackageDoesNotExistError(self.package_name)
                 else:
                     generic_sql_error_handler(err=err, role=self.package_role)
-
-            return version_obj
+                    return None
 
     def drop_application_before_upgrade(self, policy: PolicyBase, is_interactive: bool):
         """
         This method will attempt to drop an application object if a previous upgrade fails.
         """
         user_prompt = "Do you want the Snowflake CLI to drop the existing application object and recreate it?"
         if not policy.should_proceed(user_prompt):
```

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/utils.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/version/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/nativeapp/version/version_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/notebook/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/notebook/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/common.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/object/stage_deprecated/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/common.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/models.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package_utils.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/zipper.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/snowpark/package/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/snowpark/package/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/__init__.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/common.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/compute_pool/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_registry/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_registry/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_registry/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_repository/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/image_repository/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/image_repository/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/jobs/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/jobs/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/services/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/spcs/services/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/spcs/services/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/sql/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/sql/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/diff.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/diff.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/stage/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/stage/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/commands.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/plugins/streamlit/manager.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/plugins/streamlit/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/snowflake.yml` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/src/snowflake/cli/templates/default_snowpark/app/procedures.py` & `snowflake_cli_labs-2.3.1/src/snowflake/cli/templates/default_snowpark/app/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py` & `snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py` & `snowflake_cli_labs-2.3.1/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py` & `snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py` & `snowflake_cli_labs-2.3.1/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/conftest.py` & `snowflake_cli_labs-2.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_cli.py` & `snowflake_cli_labs-2.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_command_registration.py` & `snowflake_cli_labs-2.3.1/tests/test_command_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_common_decorators.py` & `snowflake_cli_labs-2.3.1/tests/test_common_decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_common_global_context.py` & `snowflake_cli_labs-2.3.1/tests/test_common_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_config.py` & `snowflake_cli_labs-2.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_connection.py` & `snowflake_cli_labs-2.3.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_experimental_behaviour.py` & `snowflake_cli_labs-2.3.1/tests/test_experimental_behaviour.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_help_messages.py` & `snowflake_cli_labs-2.3.1/tests/test_help_messages.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_logs.py` & `snowflake_cli_labs-2.3.1/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_main.py` & `snowflake_cli_labs-2.3.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_project_initialisation.py` & `snowflake_cli_labs-2.3.1/tests/test_project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_snow_connector.py` & `snowflake_cli_labs-2.3.1/tests/test_snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_sql.py` & `snowflake_cli_labs-2.3.1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_utils.py` & `snowflake_cli_labs-2.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_zipper.py` & `snowflake_cli_labs-2.3.1/tests/test_zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_config.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_connection.ambr` & `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_connection.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/__snapshots__/test_help_messages.ambr` & `snowflake_cli_labs-2.3.1/tests/__snapshots__/test_help_messages.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/test_feature_flags.py` & `snowflake_cli_labs-2.3.1/tests/api/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/test_secure_path.py` & `snowflake_cli_labs-2.3.1/tests/api/test_secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/commands/test_flags.py` & `snowflake_cli_labs-2.3.1/tests/api/commands/test_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/commands/test_snow_typer.py` & `snowflake_cli_labs-2.3.1/tests/api/commands/test_snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/commands/__snapshots__/test_flags.ambr` & `snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_flags.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/commands/__snapshots__/test_snow_typer.ambr` & `snowflake_cli_labs-2.3.1/tests/api/commands/__snapshots__/test_snow_typer.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/console/test_cli_console_output.py` & `snowflake_cli_labs-2.3.1/tests/api/console/test_cli_console_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/console/test_console_abc.py` & `snowflake_cli_labs-2.3.1/tests/api/console/test_console_abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/console/test_intermediate_output.py` & `snowflake_cli_labs-2.3.1/tests/api/console/test_intermediate_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/api/utils/test_rendering.py` & `snowflake_cli_labs-2.3.1/tests/api/utils/test_rendering.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/app/test_telemetry.py` & `snowflake_cli_labs-2.3.1/tests/app/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/git/test_git_commands.py` & `snowflake_cli_labs-2.3.1/tests/git/test_git_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/git/__snapshots__/test_git_commands.ambr` & `snowflake_cli_labs-2.3.1/tests/git/__snapshots__/test_git_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/patch_utils.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/patch_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_annotation_processor_config.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_annotation_processor_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_artifacts.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_commands.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_feature_flags.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_init.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_manager.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_package_scripts.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_package_scripts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_run_processor.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_run_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1238,14 +1238,15 @@
                 mock_cursor(
                     [
                         {
                             "name": "My Package",
                             "comment": "some comment",
                             "owner": "PACKAGE_ROLE",
                             "version": version,
+                            "patch": 0,
                         }
                     ],
                     [],
                 ),
                 mock.call(
                     f"show versions like 'V1' in application package app_pkg",
                     cursor_class=DictCursor,
```

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_teardown_processor.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_utils.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_version_create_processor.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_create_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/test_version_drop_processor.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/test_version_drop_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/utils.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/__snapshots__/test_commands.ambr` & `snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/__snapshots__/test_init.ambr` & `snowflake_cli_labs-2.3.1/tests/nativeapp/__snapshots__/test_init.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/nativeapp/codegen/test_sandbox.py` & `snowflake_cli_labs-2.3.1/tests/nativeapp/codegen/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/notebook/test_notebook_commands.py` & `snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/notebook/test_notebook_manager.py` & `snowflake_cli_labs-2.3.1/tests/notebook/test_notebook_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/object/test_common.py` & `snowflake_cli_labs-2.3.1/tests/object/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/object/test_object.py` & `snowflake_cli_labs-2.3.1/tests/object/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/object/test_stage.py` & `snowflake_cli_labs-2.3.1/tests/object/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/object/__snapshots__/test_object.ambr` & `snowflake_cli_labs-2.3.1/tests/object/__snapshots__/test_object.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/output/test_format_silent_enforcement.py` & `snowflake_cli_labs-2.3.1/tests/output/test_format_silent_enforcement.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/output/test_printing.py` & `snowflake_cli_labs-2.3.1/tests/output/test_printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/output/test_silent_output.py` & `snowflake_cli_labs-2.3.1/tests/output/test_silent_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/plugin/test_broken_plugin.py` & `snowflake_cli_labs-2.3.1/tests/plugin/test_broken_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/plugin/test_failing_plugin.py` & `snowflake_cli_labs-2.3.1/tests/plugin/test_failing_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/plugin/test_override_by_external_plugins.py` & `snowflake_cli_labs-2.3.1/tests/plugin/test_override_by_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/fixtures.py` & `snowflake_cli_labs-2.3.1/tests/project/fixtures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/test_config.py` & `snowflake_cli_labs-2.3.1/tests/project/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/test_definition_manager.py` & `snowflake_cli_labs-2.3.1/tests/project/test_definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/test_project_schemas.py` & `snowflake_cli_labs-2.3.1/tests/project/test_project_schemas.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/test_util.py` & `snowflake_cli_labs-2.3.1/tests/project/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/project/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.3.1/tests/project/__snapshots__/test_config.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/mocks.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/mocks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_anaconda.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_anaconda.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_build.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_build.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_common.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_function.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_models.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_package.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/test_procedure.py` & `snowflake_cli_labs-2.3.1/tests/snowpark/test_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_package.ambr` & `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_package.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/snowpark/__snapshots__/test_procedure.ambr` & `snowflake_cli_labs-2.3.1/tests/snowpark/__snapshots__/test_procedure.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_common.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_image_repository.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_jobs.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_registry.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/test_services.py` & `snowflake_cli_labs-2.3.1/tests/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/__snapshots__/test_image_repository.ambr` & `snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_image_repository.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/spcs/__snapshots__/test_registry.ambr` & `snowflake_cli_labs-2.3.1/tests/spcs/__snapshots__/test_registry.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/stage/test_diff.py` & `snowflake_cli_labs-2.3.1/tests/stage/test_diff.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/stage/test_stage.py` & `snowflake_cli_labs-2.3.1/tests/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/stage/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.3.1/tests/stage/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/streamlit/test_commands.py` & `snowflake_cli_labs-2.3.1/tests/streamlit/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/streamlit/test_config.py` & `snowflake_cli_labs-2.3.1/tests/streamlit/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-2.3.1/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json` & `snowflake_cli_labs-2.3.1/tests/test_data/packages_available_in_snowflake_sql_result_rows.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/test_data.py` & `snowflake_cli_labs-2.3.1/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-2.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration/app/manifest.yml` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/integration/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/integration_external/app/manifest.yml` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/integration_external/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_external_access/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_functions/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_functions/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_external_access/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/app.py` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures/app.zip` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/test_data/projects/snowpark_procedures_coverage/app.py` & `snowflake_cli_labs-2.3.1/tests/test_data/projects/snowpark_procedures_coverage/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/testing_utils/files_and_dirs.py` & `snowflake_cli_labs-2.3.1/tests/testing_utils/files_and_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests/testing_utils/fixtures.py` & `snowflake_cli_labs-2.3.1/tests/testing_utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_e2e/conftest.py` & `snowflake_cli_labs-2.3.1/tests_e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_e2e/test_error_handling.py` & `snowflake_cli_labs-2.3.1/tests_e2e/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_e2e/test_installation.py` & `snowflake_cli_labs-2.3.1/tests_e2e/test_installation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_e2e/test_snowpark_examples.py` & `snowflake_cli_labs-2.3.1/tests_e2e/test_snowpark_examples.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_e2e/__snapshots__/test_installation.ambr` & `snowflake_cli_labs-2.3.1/tests_e2e/__snapshots__/test_installation.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/conftest.py` & `snowflake_cli_labs-2.3.1/tests_integration/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/snowflake_connector.py` & `snowflake_cli_labs-2.3.1/tests_integration/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_config.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_connection.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_external_plugins.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_git.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_git.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_nativeapp.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_nativeapp.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_notebooks.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_object.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_package.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_session_token.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_session_token.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_snowpark.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_snowpark_external_access.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_snowpark_external_access.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_sql.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_stage.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_streamlit.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_temporary_connection.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_temporary_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import datetime
+import os
+from contextlib import contextmanager
+from pathlib import Path
 from typing import Any, Dict, List
 
 from snowflake.connector.cursor import SnowflakeCursor
 
 
 def row_from_mock(mock_print) -> List[Dict[str, Any]]:
     return row_from_cursor(mock_print.call_args.args[0])
@@ -47,7 +50,17 @@
 
 def not_contains_row_with(rows: List[Dict[str, Any]], values: Dict[str, Any]) -> bool:
     values_items = values.items()
     for row in rows:
         if row.items() >= values_items:
             return False
     return True
+
+
+@contextmanager
+def pushd(directory: Path):
+    cwd = os.getcwd()
+    os.chdir(directory)
+    try:
+        yield directory
+    finally:
+        os.chdir(cwd)
```

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.3.1/tests_integration/__snapshots__/test_stage.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/scripts/integration_account_setup.sql` & `snowflake_cli_labs-2.3.1/tests_integration/scripts/integration_account_setup.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_image_repository.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_jobs.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_registry.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/test_services.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/docker/echo_service.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/docker/echo_service.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/compute_pool_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/compute_pool_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/spcs/testing_utils/spcs_services_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/spcs/testing_utils/spcs_services_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark/app/app.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_external_access/app/app.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_external_access/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml` & `snowflake_cli_labs-2.3.1/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/naming_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/snowpark_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/snowpark_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/sql_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/working_directory_utils.py` & `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/working_directory_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/tests_integration/testing_utils/assertions/test_result_assertions.py` & `snowflake_cli_labs-2.3.1/tests_integration/testing_utils/assertions/test_result_assertions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/LICENSE` & `snowflake_cli_labs-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/README.md` & `snowflake_cli_labs-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/pyproject.toml` & `snowflake_cli_labs-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.3.0rc1/PKG-INFO` & `snowflake_cli_labs-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake-cli-labs
-Version: 2.3.0rc1
+Version: 2.3.1
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/snowflakedb/snowflake-cli
 Project-URL: Bug Tracker, https://github.com/snowflakedb/snowflake-cli/issues
 Author: Snowflake Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

