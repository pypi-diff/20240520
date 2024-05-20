# Comparing `tmp/skforecast-0.9.0.tar.gz` & `tmp/skforecast-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skforecast-0.9.0.tar", last modified: Sun Jul  9 15:19:01 2023, max compression
+gzip compressed data, was "skforecast-0.9.1.tar", last modified: Fri Jul 14 16:58:05 2023, max compression
```

## Comparing `skforecast-0.9.0.tar` & `skforecast-0.9.1.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.074696 skforecast-0.9.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1508 2023-05-31 16:50:11.000000 skforecast-0.9.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15589 2023-07-09 15:19:01.074696 skforecast-0.9.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14689 2023-07-09 14:30:47.000000 skforecast-0.9.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-09 15:19:01.074696 skforecast-0.9.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2613 2023-07-09 14:46:06.000000 skforecast-0.9.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.034695 skforecast-0.9.0/skforecast/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.034695 skforecast-0.9.0/skforecast/ForecasterAutoreg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48408 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/ForecasterAutoreg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.038695 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2430 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/fixtures_ForecasterAutoreg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2195 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4559 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20218 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6884 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12687 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7436 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3098 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7318 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_recursive_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      729 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5955 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.038695 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49395 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/ForecasterAutoregCustom.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.042695 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/fixtures_ForecasterAutoregCustom.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9076 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3081 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13005 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8438 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1937 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_recursive_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      973 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7708 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.042695 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    60187 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/ForecasterAutoregDirect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.046696 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/fixtures_ForecasterAutoregDirect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3908 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4771 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43045 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5368 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_filter_train_X_y_for_step.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5118 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9213 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1633 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15709 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8426 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3221 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1485 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8514 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.046696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    66458 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/ForecasterAutoregMultiSeries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.050696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-06-08 08:44:59.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/fixtures_ForecasterAutoregMultiSeries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-06-08 08:44:59.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12418 2023-06-08 08:44:59.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45392 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9693 2023-06-08 08:44:59.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7720 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19850 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14060 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15631 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_recursive_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7865 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.054696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67704 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/ForecasterAutoregMultiSeriesCustom.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.054696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3607 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/fixtures_ForecasterAutoregMultiSeriesCustom.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13459 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54461 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9113 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2799 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20939 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15783 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4430 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16918 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_recursive_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9355 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.054696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68323 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/ForecasterAutoregMultiVariate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.058696 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3596 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/fixtures_ForecasterAutoregMultiVariate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4408 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6104 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_sample_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58763 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_train_X_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6653 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_filter_train_X_y_for_step.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10059 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10671 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17408 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9545 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_bootstrapping.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3800 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_dist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3795 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      854 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9524 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_out_sample_residuals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.058696 skforecast-0.9.0/skforecast/ForecasterBase/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4836 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterBase/ForecasterBase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterBase/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.058696 skforecast-0.9.0/skforecast/ForecasterBase/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterBase/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.058696 skforecast-0.9.0/skforecast/ForecasterSarimax/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31808 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/ForecasterSarimax.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.062696 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3742 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/fixtures_ForecasterSarimax.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_fit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_get_feature_importances.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_init.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16735 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_predict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19506 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_predict_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_set_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1049 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_set_params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2023-06-06 16:38:44.000000 skforecast-0.9.0/skforecast/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.062696 skforecast-0.9.0/skforecast/exceptions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/exceptions/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2838 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/exceptions/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.062696 skforecast-0.9.0/skforecast/exceptions/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/exceptions/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.062696 skforecast-0.9.0/skforecast/model_selection/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-06-09 13:16:39.000000 skforecast-0.9.0/skforecast/model_selection/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68298 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection/model_selection.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.066696 skforecast-0.9.0/skforecast/model_selection/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2773 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/fixtures_model_selection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3589 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39617 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster_no_refit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54019 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster_refit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9274 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_forecaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26850 2023-06-08 08:29:02.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_optuna.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25188 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_skopt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48981 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_create_backtesting_folds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13396 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_evaluate_grid_hyperparameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2705 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_get_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2479 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_grid_search_forecaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2752 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection/tests/test_random_search_forecaster.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.066696 skforecast-0.9.0/skforecast/model_selection_multiseries/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      262 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    60572 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/model_selection_multiseries.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.066696 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2370 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/fixtures_model_selection_multiseries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   116060 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_backtesting_forecaster_multiseries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37744 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_evaluate_grid_hyperparameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7318 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_grid_search_forecaster_multiseries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8022 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_random_search_forecaster_multiseries.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.066696 skforecast-0.9.0/skforecast/model_selection_sarimax/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32390 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/model_selection_sarimax.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.070696 skforecast-0.9.0/skforecast/model_selection_sarimax/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38950 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_backtesting_sarimax.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9764 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_evaluate_grid_hyperparameters_sarimax.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_grid_search_sarimax.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_random_search_sarimax.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.070696 skforecast-0.9.0/skforecast/plot/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/plot/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5967 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/plot/plot.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.070696 skforecast-0.9.0/skforecast/plot/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/plot/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      573 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/plot/tests/test_plot_residuals.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.070696 skforecast-0.9.0/skforecast/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.074696 skforecast-0.9.0/skforecast/utils/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29590 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_backtesting_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1545 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_exog.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3793 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_exog_dtypes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4875 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_interval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_optional_dependency.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40682 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_predict_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3029 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_select_fit_kwargs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_check_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11595 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_exog_to_direct.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5051 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_exog_to_direct_numpy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_expand_index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3505 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_initialize_lags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8156 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_initialize_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2459 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_multivariate_time_series_corr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2470 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_preproces_exog.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2648 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_preproces_last_window.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2384 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_preproces_y.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_save_load_forecaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2687 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/utils/tests/test_select_n_jobs_backtesting.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1244 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/utils/tests/test_select_n_jobs_fit_forecaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5889 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_transform_dataframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-05-31 16:50:11.000000 skforecast-0.9.0/skforecast/utils/tests/test_transform_series.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    62300 2023-07-09 14:30:47.000000 skforecast-0.9.0/skforecast/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.034695 skforecast-0.9.0/skforecast.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15589 2023-07-09 15:19:00.000000 skforecast-0.9.0/skforecast.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11663 2023-07-09 15:19:01.000000 skforecast-0.9.0/skforecast.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-09 15:19:00.000000 skforecast-0.9.0/skforecast.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-07-09 15:19:00.000000 skforecast-0.9.0/skforecast.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-09 15:19:00.000000 skforecast-0.9.0/skforecast.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-09 15:19:01.074696 skforecast-0.9.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-05-31 16:50:11.000000 skforecast-0.9.0/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-06-08 08:06:18.000000 skforecast-0.9.0/tests/test_skforecast_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.257990 skforecast-0.9.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1508 2023-05-31 16:50:11.000000 skforecast-0.9.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15589 2023-07-14 16:58:05.257990 skforecast-0.9.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14689 2023-07-14 15:11:11.000000 skforecast-0.9.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-14 16:58:05.257990 skforecast-0.9.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2613 2023-07-14 15:11:11.000000 skforecast-0.9.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.113988 skforecast-0.9.1/skforecast/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.113988 skforecast-0.9.1/skforecast/ForecasterAutoreg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48408 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/ForecasterAutoreg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.125989 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2430 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/fixtures_ForecasterAutoreg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2195 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4559 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20218 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6884 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12687 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7436 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3098 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7318 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_recursive_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      729 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5955 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.129989 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49395 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/ForecasterAutoregCustom.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.141989 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/fixtures_ForecasterAutoregCustom.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9076 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3081 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13005 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8438 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1937 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_recursive_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      973 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7708 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.141989 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    60187 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/ForecasterAutoregDirect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.153989 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/fixtures_ForecasterAutoregDirect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3908 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4771 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43045 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5368 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_filter_train_X_y_for_step.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5118 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9213 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1633 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15709 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8426 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3221 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1485 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8514 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.157989 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    66458 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/ForecasterAutoregMultiSeries.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.169989 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-06-08 08:44:59.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/fixtures_ForecasterAutoregMultiSeries.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-06-08 08:44:59.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12418 2023-06-08 08:44:59.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45392 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9693 2023-06-08 08:44:59.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7720 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19850 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14060 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15631 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_recursive_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7865 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.173989 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67704 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/ForecasterAutoregMultiSeriesCustom.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.185989 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3607 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/fixtures_ForecasterAutoregMultiSeriesCustom.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13459 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54461 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9113 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2799 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20939 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15783 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4430 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16918 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_recursive_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9355 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.185989 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68323 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/ForecasterAutoregMultiVariate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.197990 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3596 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/fixtures_ForecasterAutoregMultiVariate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4408 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6104 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_sample_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58763 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_train_X_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6653 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_filter_train_X_y_for_step.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10059 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10671 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17408 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9545 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_bootstrapping.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3800 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_dist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3795 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      854 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9524 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_out_sample_residuals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.197990 skforecast-0.9.1/skforecast/ForecasterBase/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4836 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterBase/ForecasterBase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterBase/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.201990 skforecast-0.9.1/skforecast/ForecasterBase/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterBase/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.201990 skforecast-0.9.1/skforecast/ForecasterSarimax/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31808 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/ForecasterSarimax.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.205990 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3742 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/fixtures_ForecasterSarimax.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_fit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_get_feature_importances.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_init.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16735 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_predict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19506 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_predict_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_set_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1049 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_set_params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2023-07-14 15:11:11.000000 skforecast-0.9.1/skforecast/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.209990 skforecast-0.9.1/skforecast/exceptions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/exceptions/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2838 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/exceptions/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.209990 skforecast-0.9.1/skforecast/exceptions/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/exceptions/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.209990 skforecast-0.9.1/skforecast/model_selection/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-06-09 13:16:39.000000 skforecast-0.9.1/skforecast/model_selection/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68289 2023-07-13 15:25:28.000000 skforecast-0.9.1/skforecast/model_selection/model_selection.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.221990 skforecast-0.9.1/skforecast/model_selection/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2773 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/fixtures_model_selection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3589 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39617 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster_no_refit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54019 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster_refit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9274 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_forecaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26850 2023-06-08 08:29:02.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_optuna.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25188 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_skopt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48981 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_create_backtesting_folds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13396 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_evaluate_grid_hyperparameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2705 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_get_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2479 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_grid_search_forecaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2752 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection/tests/test_random_search_forecaster.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.221990 skforecast-0.9.1/skforecast/model_selection_multiseries/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      262 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    60542 2023-07-13 15:25:28.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/model_selection_multiseries.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.229990 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2370 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/fixtures_model_selection_multiseries.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   116060 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_backtesting_forecaster_multiseries.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37744 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_evaluate_grid_hyperparameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7318 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_grid_search_forecaster_multiseries.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8022 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_random_search_forecaster_multiseries.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.229990 skforecast-0.9.1/skforecast/model_selection_sarimax/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32379 2023-07-13 15:25:28.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/model_selection_sarimax.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.233990 skforecast-0.9.1/skforecast/model_selection_sarimax/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38950 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_backtesting_sarimax.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9764 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_evaluate_grid_hyperparameters_sarimax.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_grid_search_sarimax.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_random_search_sarimax.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.237990 skforecast-0.9.1/skforecast/plot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/plot/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5967 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/plot/plot.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.237990 skforecast-0.9.1/skforecast/plot/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/plot/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      573 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/plot/tests/test_plot_residuals.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.237990 skforecast-0.9.1/skforecast/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.253991 skforecast-0.9.1/skforecast/utils/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29590 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_backtesting_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1545 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_exog.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3793 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_exog_dtypes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4875 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_interval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_optional_dependency.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40682 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_predict_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3029 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_select_fit_kwargs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_check_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11595 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_exog_to_direct.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5051 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_exog_to_direct_numpy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_expand_index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3505 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_initialize_lags.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8156 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_initialize_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2459 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_multivariate_time_series_corr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2470 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_preproces_exog.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2648 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_preproces_last_window.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2384 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_preproces_y.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1477 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_save_load_forecaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2687 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/utils/tests/test_select_n_jobs_backtesting.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1244 2023-07-09 14:30:47.000000 skforecast-0.9.1/skforecast/utils/tests/test_select_n_jobs_fit_forecaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5889 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_transform_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-05-31 16:50:11.000000 skforecast-0.9.1/skforecast/utils/tests/test_transform_series.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    62328 2023-07-13 15:26:06.000000 skforecast-0.9.1/skforecast/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.113988 skforecast-0.9.1/skforecast.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15589 2023-07-14 16:58:05.000000 skforecast-0.9.1/skforecast.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11663 2023-07-14 16:58:05.000000 skforecast-0.9.1/skforecast.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-14 16:58:05.000000 skforecast-0.9.1/skforecast.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-07-14 16:58:05.000000 skforecast-0.9.1/skforecast.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-14 16:58:05.000000 skforecast-0.9.1/skforecast.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 16:58:05.253991 skforecast-0.9.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-05-31 16:50:11.000000 skforecast-0.9.1/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-07-14 15:11:11.000000 skforecast-0.9.1/tests/test_skforecast_version.py
```

### Comparing `skforecast-0.9.0/LICENSE` & `skforecast-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/PKG-INFO` & `skforecast-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skforecast
-Version: 0.9.0
+Version: 0.9.1
 Summary: Forecasting time series with scikit-learn regressors. It also works with any regressor compatible with the scikit-learn API (pipelines, CatBoost, LightGBM, XGBoost, Ranger...).
 Home-page: https://github.com/JoaquinAmatRodrigo/skforecast
 Author: Joaquin Amat Rodrigo and Javier Escobar Ortiz
 Author-email: j.amatrodrigo@gmail.com, javier.escobar.ortiz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -65,15 +65,15 @@
 ```bash
 pip install skforecast
 ```
 
 Specific version:
 
 ```bash
-pip install skforecast==0.9.0
+pip install skforecast==0.9.1
 ```
 
 Latest (unstable):
 
 ```bash
 pip install git+https://github.com/JoaquinAmatRodrigo/skforecast#master
 ```
@@ -110,15 +110,15 @@
 ## Optional dependencies
 
 + matplotlib>=3.3, <3.8
 + seaborn>=0.11, <0.13
 + statsmodels>=0.12, <0.15
 + pmdarima>=2.0, <2.1
 
-# What is new in skforecast 0.9.0?
+# What is new in skforecast 0.9.1?
 
 Visit the [release notes](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/changelog.md) to view all notable changes.
 
 - [x] `ForecasterAutoregDirect` and `ForecasterAutoregMultiVariate` include the `n_jobs` argument in their `fit` method, allowing multi-process parallelization for improved performance.
 - [x] All backtesting and grid search functions have been extended to include the `n_jobs` argument, allowing multi-process parallelization for improved performance.
 - [x] Argument `refit` now can be also an `integer` in all backtesting dependent functions in modules `model_selection`, `model_selection_multiseries`, and `model_selection_sarimax`. This allows the Forecaster to be trained every this number of iterations.
 - [x] `ForecasterAutoregMultiSeries` and `ForecasterAutoregMultiSeriesCustom` can be trained using series of different lengths. This means that the model can handle datasets with different numbers of data points in each series.
@@ -225,25 +225,25 @@
 
 # Citation
 
 If you use this software, please cite it using the following metadata.
 
 **APA**:
 ```
-Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.0) [Computer software]
+Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.1) [Computer software]
 ```
 
 **BibTeX**:
 ```
 @software{skforecast,
 author = {Amat Rodrigo, Joaquin and Escobar Ortiz, Javier},
 license = {BSD 3-Clause License},
 month = {7},
 title = {{skforecast}},
-version = {0.9.0},
+version = {0.9.1},
 year = {2023}
 }
 ```
 
 View the [citation file](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/CITATION.cff).
```

### Comparing `skforecast-0.9.0/README.md` & `skforecast-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```bash
 pip install skforecast
 ```
 
 Specific version:
 
 ```bash
-pip install skforecast==0.9.0
+pip install skforecast==0.9.1
 ```
 
 Latest (unstable):
 
 ```bash
 pip install git+https://github.com/JoaquinAmatRodrigo/skforecast#master
 ```
@@ -89,15 +89,15 @@
 ## Optional dependencies
 
 + matplotlib>=3.3, <3.8
 + seaborn>=0.11, <0.13
 + statsmodels>=0.12, <0.15
 + pmdarima>=2.0, <2.1
 
-# What is new in skforecast 0.9.0?
+# What is new in skforecast 0.9.1?
 
 Visit the [release notes](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/changelog.md) to view all notable changes.
 
 - [x] `ForecasterAutoregDirect` and `ForecasterAutoregMultiVariate` include the `n_jobs` argument in their `fit` method, allowing multi-process parallelization for improved performance.
 - [x] All backtesting and grid search functions have been extended to include the `n_jobs` argument, allowing multi-process parallelization for improved performance.
 - [x] Argument `refit` now can be also an `integer` in all backtesting dependent functions in modules `model_selection`, `model_selection_multiseries`, and `model_selection_sarimax`. This allows the Forecaster to be trained every this number of iterations.
 - [x] `ForecasterAutoregMultiSeries` and `ForecasterAutoregMultiSeriesCustom` can be trained using series of different lengths. This means that the model can handle datasets with different numbers of data points in each series.
@@ -204,25 +204,25 @@
 
 # Citation
 
 If you use this software, please cite it using the following metadata.
 
 **APA**:
 ```
-Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.0) [Computer software]
+Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.1) [Computer software]
 ```
 
 **BibTeX**:
 ```
 @software{skforecast,
 author = {Amat Rodrigo, Joaquin and Escobar Ortiz, Javier},
 license = {BSD 3-Clause License},
 month = {7},
 title = {{skforecast}},
-version = {0.9.0},
+version = {0.9.1},
 year = {2023}
 }
 ```
 
 View the [citation file](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/CITATION.cff).
```

### Comparing `skforecast-0.9.0/setup.py` & `skforecast-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 if sys.version_info[:2] < (3, 8):
     raise RuntimeError("Python version >= 3.8 required.")
 
 if sys.version_info[:2] > (3, 11):
-    fmt = "Skforecast {} may not yet support Python {}.{}."
+    fmt = "skforecast {} may not yet support Python {}.{}."
     warnings.warn(
         fmt.format(VERSION, *sys.version_info[:2]),
         RuntimeWarning)
     del fmt
 
 
 setuptools.setup(
```

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/ForecasterAutoreg.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/ForecasterAutoreg.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/fixtures_ForecasterAutoreg.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/fixtures_ForecasterAutoreg.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_recursive_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_recursive_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoreg/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoreg/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/ForecasterAutoregCustom.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/ForecasterAutoregCustom.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/fixtures_ForecasterAutoregCustom.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/fixtures_ForecasterAutoregCustom.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_init.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_recursive_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_recursive_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregCustom/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregCustom/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/ForecasterAutoregDirect.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/ForecasterAutoregDirect.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/fixtures_ForecasterAutoregDirect.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/fixtures_ForecasterAutoregDirect.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_filter_train_X_y_for_step.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_filter_train_X_y_for_step.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_init.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregDirect/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregDirect/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/ForecasterAutoregMultiSeries.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/ForecasterAutoregMultiSeries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/fixtures_ForecasterAutoregMultiSeries.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/fixtures_ForecasterAutoregMultiSeries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_recursive_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_recursive_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeries/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeries/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/ForecasterAutoregMultiSeriesCustom.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/ForecasterAutoregMultiSeriesCustom.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/fixtures_ForecasterAutoregMultiSeriesCustom.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/fixtures_ForecasterAutoregMultiSeriesCustom.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_init.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_recursive_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_recursive_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiSeriesCustom/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/ForecasterAutoregMultiVariate.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/ForecasterAutoregMultiVariate.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/fixtures_ForecasterAutoregMultiVariate.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/fixtures_ForecasterAutoregMultiVariate.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_sample_weights.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_sample_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_create_train_X_y.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_create_train_X_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_filter_train_X_y_for_step.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_filter_train_X_y_for_step.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_init.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_bootstrapping.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_dist.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_dist.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_lags.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_out_sample_residuals.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_out_sample_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterAutoregMultiVariate/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterAutoregMultiVariate/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterBase/ForecasterBase.py` & `skforecast-0.9.1/skforecast/ForecasterBase/ForecasterBase.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/ForecasterSarimax.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/ForecasterSarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/fixtures_ForecasterSarimax.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/fixtures_ForecasterSarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_fit.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_get_feature_importances.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_init.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_predict.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_predict_interval.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_predict_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_set_fit_kwargs.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_set_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/ForecasterSarimax/tests/test_set_params.py` & `skforecast-0.9.1/skforecast/ForecasterSarimax/tests/test_set_params.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/exceptions/exceptions.py` & `skforecast-0.9.1/skforecast/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/model_selection.py` & `skforecast-0.9.1/skforecast/model_selection/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -818,17 +818,17 @@
     """
     Exhaustive search over specified parameter values for a Forecaster object.
     Validation is done using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterAutoreg, ForecasterAutoregCustom, ForecasterAutoregDirect
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
-        Training time series values. 
+        Training time series. 
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -929,15 +929,15 @@
     """
     Random search over specified parameter values or distributions for a Forecaster 
     object. Validation is done using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterAutoreg, ForecasterAutoregCustom, ForecasterAutoregDirect
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
         Training time series. 
     param_distributions : dict
         Dictionary with parameters names (`str`) as keys and 
         distributions or lists of parameters to try.
     steps : int
         Number of steps to predict.
@@ -1042,17 +1042,17 @@
 ) -> pd.DataFrame:
     """
     Evaluate parameter values for a Forecaster object using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterAutoreg, ForecasterAutoregCustom, ForecasterAutoregDirect
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
-        Training time series values. 
+        Training time series. 
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -1228,15 +1228,15 @@
     """
     Bayesian optimization for a Forecaster object using time series backtesting and 
     optuna library.
     
     Parameters
     ----------
     forecaster : ForecasterAutoreg, ForecasterAutoregCustom, ForecasterAutoregDirect
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
         Training time series. 
     search_space : Callable (optuna)
         Function with argument `trial` which returns a dictionary with parameters names 
         (`str`) as keys and Trial object from optuna (trial.suggest_float, 
         trial.suggest_int, trial.suggest_categorical) as values.
     steps : int
@@ -1377,15 +1377,15 @@
     """
     Bayesian optimization for a Forecaster object using time series backtesting 
     and optuna library.
     
     Parameters
     ----------
     forecaster : ForecasterAutoreg, ForecasterAutoregCustom, ForecasterAutoregDirect
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
         Training time series. 
     search_space : Callable
         Function with argument `trial` which returns a dictionary with parameters names 
         (`str`) as keys and Trial object from optuna (trial.suggest_float, 
         trial.suggest_int, trial.suggest_categorical) as values.
     steps : int
```

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/fixtures_model_selection.py` & `skforecast-0.9.1/skforecast/model_selection/tests/fixtures_model_selection.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster_no_refit.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster_no_refit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_backtesting_forecaster_refit.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_backtesting_forecaster_refit.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_forecaster.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_optuna.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_optuna.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_bayesian_search_skopt.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_bayesian_search_skopt.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_create_backtesting_folds.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_create_backtesting_folds.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_evaluate_grid_hyperparameters.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_evaluate_grid_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_get_metric.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_get_metric.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_grid_search_forecaster.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_grid_search_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection/tests/test_random_search_forecaster.py` & `skforecast-0.9.1/skforecast/model_selection/tests/test_random_search_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/model_selection_multiseries.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/model_selection_multiseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,15 @@
     to create the initial predictors, so no predictions are calculated for them.
     
     A copy of the original forecaster is created so that it is not modified during 
     the process.
     
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom,
-    ForecasterAutoregMultiVariate
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
         Forecaster model.
     series : pandas DataFrame
         Training time series.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -358,16 +357,15 @@
     to create the initial predictors, so no predictions are calculated for them.
     
     A copy of the original forecaster is created so that it is not modified during 
     the process.
 
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom,
-    ForecasterAutoregMultiVariate
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
         Forecaster model.
     series : pandas DataFrame
         Training time series.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -535,17 +533,16 @@
 ) -> pd.DataFrame:
     """
     Exhaustive search over specified parameter values for a Forecaster object.
     Validation is done using multi-series backtesting.
     
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom,
-    ForecasterAutoregMultiVariate
-        Forcaster model.
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
+        Forecaster model.
     series : pandas DataFrame
         Training time series.
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
@@ -655,17 +652,16 @@
 ) -> pd.DataFrame:
     """
     Random search over specified parameter values or distributions for a Forecaster 
     object. Validation is done using multi-series backtesting.
     
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, 
-    ForecasterAutoregMultiVariate
-        Forcaster model.
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
+        Forecaster model.
     series : pandas DataFrame
         Training time series.
     param_distributions : dict
         Dictionary with parameters names (`str`) as keys and distributions or 
         lists of parameters to try.
     steps : int
         Number of steps to predict.
@@ -778,17 +774,16 @@
     show_progress: bool=True
 ) -> pd.DataFrame:
     """
     Evaluate parameter values for a Forecaster object using multi-series backtesting.
     
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom,
-    ForecasterAutoregMultiVariate
-        Forcaster model.
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
+        Forecaster model.
     series : pandas DataFrame
         Training time series.
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
@@ -1003,16 +998,15 @@
     If `refit` is False, the model is trained only once using the `initial_train_size`
     first observations. If `refit` is True, the model is trained in each iteration
     increasing the training set. A copy of the original forecaster is created so 
     it is not modified during the process.
 
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, 
-    ForecasterAutoregMultiVariate
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
         Forecaster model.
     series : pandas DataFrame
         Training time series.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -1134,17 +1128,16 @@
     This function is an alias of grid_search_forecaster_multiseries.
 
     Exhaustive search over specified parameter values for a Forecaster object.
     Validation is done using multi-series backtesting.
     
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, 
-    ForecasterAutoregMultiVariate
-        Forcaster model.
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
+        Forecaster model.
     series : pandas DataFrame
         Training time series.
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
@@ -1254,17 +1247,16 @@
     This function is an alias of random_search_forecaster_multiseries.
 
     Random search over specified parameter values or distributions for a Forecaster 
     object. Validation is done using multi-series backtesting.
 
     Parameters
     ----------
-    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom,
-    ForecasterAutoregMultiVariate
-        Forcaster model.
+    forecaster : ForecasterAutoregMultiSeries, ForecasterAutoregMultiSeriesCustom, ForecasterAutoregMultiVariate
+        Forecaster model.
     series : pandas DataFrame
         Training time series.
     param_distributions : dict
         Dictionary with parameters names (`str`) as keys and distributions or 
         lists of parameters to try.
     steps : int
         Number of steps to predict.
```

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/tests/fixtures_model_selection_multiseries.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/tests/fixtures_model_selection_multiseries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_backtesting_forecaster_multiseries.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_backtesting_forecaster_multiseries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_evaluate_grid_hyperparameters.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_evaluate_grid_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_grid_search_forecaster_multiseries.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_grid_search_forecaster_multiseries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_multiseries/tests/test_random_search_forecaster_multiseries.py` & `skforecast-0.9.1/skforecast/model_selection_multiseries/tests/test_random_search_forecaster_multiseries.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_sarimax/model_selection_sarimax.py` & `skforecast-0.9.1/skforecast/model_selection_sarimax/model_selection_sarimax.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,17 +441,17 @@
     """
     Exhaustive search over specified parameter values for a ForecasterSarimax object.
     Validation is done using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterSarimax
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
-        Training time series values. 
+        Training time series. 
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
@@ -547,15 +547,15 @@
     """
     Random search over specified parameter values or distributions for a Forecaster 
     object. Validation is done using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterSarimax
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
         Training time series. 
     param_distributions : dict
         Dictionary with parameters names (`str`) as keys and 
         distributions or lists of parameters to try.
     steps : int
         Number of steps to predict.
@@ -655,17 +655,17 @@
 ) -> pd.DataFrame:
     """
     Evaluate parameter values for a Forecaster object using time series backtesting.
     
     Parameters
     ----------
     forecaster : ForecasterSarimax
-        Forcaster model.
+        Forecaster model.
     y : pandas Series
-        Training time series values. 
+        Training time series. 
     param_grid : dict
         Dictionary with parameters names (`str`) as keys and lists of parameter
         settings to try as values.
     steps : int
         Number of steps to predict.
     metric : str, Callable, list
         Metric used to quantify the goodness of fit of the model.
```

### Comparing `skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_backtesting_sarimax.py` & `skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_backtesting_sarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_evaluate_grid_hyperparameters_sarimax.py` & `skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_evaluate_grid_hyperparameters_sarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_grid_search_sarimax.py` & `skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_grid_search_sarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/model_selection_sarimax/test/test_random_search_sarimax.py` & `skforecast-0.9.1/skforecast/model_selection_sarimax/test/test_random_search_sarimax.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/plot/plot.py` & `skforecast-0.9.1/skforecast/plot/plot.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/plot/tests/test_plot_residuals.py` & `skforecast-0.9.1/skforecast/plot/tests/test_plot_residuals.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_backtesting_input.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_backtesting_input.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_exog.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_exog.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_exog_dtypes.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_exog_dtypes.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_interval.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_interval.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_optional_dependency.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_predict_input.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_predict_input.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_select_fit_kwargs.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_select_fit_kwargs.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_check_y.py` & `skforecast-0.9.1/skforecast/utils/tests/test_check_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_exog_to_direct.py` & `skforecast-0.9.1/skforecast/utils/tests/test_exog_to_direct.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_exog_to_direct_numpy.py` & `skforecast-0.9.1/skforecast/utils/tests/test_exog_to_direct_numpy.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_expand_index.py` & `skforecast-0.9.1/skforecast/utils/tests/test_expand_index.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_initialize_lags.py` & `skforecast-0.9.1/skforecast/utils/tests/test_initialize_lags.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_initialize_weights.py` & `skforecast-0.9.1/skforecast/utils/tests/test_initialize_weights.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_multivariate_time_series_corr.py` & `skforecast-0.9.1/skforecast/utils/tests/test_multivariate_time_series_corr.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_preproces_exog.py` & `skforecast-0.9.1/skforecast/utils/tests/test_preproces_exog.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_preproces_last_window.py` & `skforecast-0.9.1/skforecast/utils/tests/test_preproces_last_window.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_preproces_y.py` & `skforecast-0.9.1/skforecast/utils/tests/test_preproces_y.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_save_load_forecaster.py` & `skforecast-0.9.1/skforecast/utils/tests/test_save_load_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_select_n_jobs_backtesting.py` & `skforecast-0.9.1/skforecast/utils/tests/test_select_n_jobs_backtesting.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_select_n_jobs_fit_forecaster.py` & `skforecast-0.9.1/skforecast/utils/tests/test_select_n_jobs_fit_forecaster.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_transform_dataframe.py` & `skforecast-0.9.1/skforecast/utils/tests/test_transform_dataframe.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/tests/test_transform_series.py` & `skforecast-0.9.1/skforecast/utils/tests/test_transform_series.py`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast/utils/utils.py` & `skforecast-0.9.1/skforecast/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Union, Any, Optional, Tuple, Callable
 import warnings
 import importlib
 import joblib
 import numpy as np
 import pandas as pd
 import sklearn
+import sklearn.linear_model
 from sklearn.compose import ColumnTransformer
 from sklearn.exceptions import NotFittedError
 import inspect
 from copy import deepcopy
 
 from ..exceptions import MissingValuesExogWarning
 from ..exceptions import DataTypeWarning
```

### Comparing `skforecast-0.9.0/skforecast.egg-info/PKG-INFO` & `skforecast-0.9.1/skforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skforecast
-Version: 0.9.0
+Version: 0.9.1
 Summary: Forecasting time series with scikit-learn regressors. It also works with any regressor compatible with the scikit-learn API (pipelines, CatBoost, LightGBM, XGBoost, Ranger...).
 Home-page: https://github.com/JoaquinAmatRodrigo/skforecast
 Author: Joaquin Amat Rodrigo and Javier Escobar Ortiz
 Author-email: j.amatrodrigo@gmail.com, javier.escobar.ortiz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -65,15 +65,15 @@
 ```bash
 pip install skforecast
 ```
 
 Specific version:
 
 ```bash
-pip install skforecast==0.9.0
+pip install skforecast==0.9.1
 ```
 
 Latest (unstable):
 
 ```bash
 pip install git+https://github.com/JoaquinAmatRodrigo/skforecast#master
 ```
@@ -110,15 +110,15 @@
 ## Optional dependencies
 
 + matplotlib>=3.3, <3.8
 + seaborn>=0.11, <0.13
 + statsmodels>=0.12, <0.15
 + pmdarima>=2.0, <2.1
 
-# What is new in skforecast 0.9.0?
+# What is new in skforecast 0.9.1?
 
 Visit the [release notes](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/changelog.md) to view all notable changes.
 
 - [x] `ForecasterAutoregDirect` and `ForecasterAutoregMultiVariate` include the `n_jobs` argument in their `fit` method, allowing multi-process parallelization for improved performance.
 - [x] All backtesting and grid search functions have been extended to include the `n_jobs` argument, allowing multi-process parallelization for improved performance.
 - [x] Argument `refit` now can be also an `integer` in all backtesting dependent functions in modules `model_selection`, `model_selection_multiseries`, and `model_selection_sarimax`. This allows the Forecaster to be trained every this number of iterations.
 - [x] `ForecasterAutoregMultiSeries` and `ForecasterAutoregMultiSeriesCustom` can be trained using series of different lengths. This means that the model can handle datasets with different numbers of data points in each series.
@@ -225,25 +225,25 @@
 
 # Citation
 
 If you use this software, please cite it using the following metadata.
 
 **APA**:
 ```
-Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.0) [Computer software]
+Amat Rodrigo, J., & Escobar Ortiz, J. skforecast (Version 0.9.1) [Computer software]
 ```
 
 **BibTeX**:
 ```
 @software{skforecast,
 author = {Amat Rodrigo, Joaquin and Escobar Ortiz, Javier},
 license = {BSD 3-Clause License},
 month = {7},
 title = {{skforecast}},
-version = {0.9.0},
+version = {0.9.1},
 year = {2023}
 }
 ```
 
 View the [citation file](https://github.com/JoaquinAmatRodrigo/skforecast/blob/master/CITATION.cff).
```

### Comparing `skforecast-0.9.0/skforecast.egg-info/SOURCES.txt` & `skforecast-0.9.1/skforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skforecast-0.9.0/skforecast.egg-info/requires.txt` & `skforecast-0.9.1/skforecast.egg-info/requires.txt`

 * *Files identical despite different names*

