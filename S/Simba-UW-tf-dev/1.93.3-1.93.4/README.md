# Comparing `tmp/Simba-UW-tf-dev-1.93.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.93.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.93.3.tar", last modified: Sun May 19 20:36:16 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.93.4.tar", last modified: Mon May 20 14:22:53 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.93.3.tar` & `Simba-UW-tf-dev-1.93.4.tar`

### file list

```diff
@@ -1,686 +1,688 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.93.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)   130051 2024-05-19 17:50:50.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.93.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.93.3/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.93.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.93.3/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1173 2024-05-19 16:18:01.000000 Simba-UW-tf-dev-1.93.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.93.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.3/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.93.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.93.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.93.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    17201 2024-05-14 11:12:57.000000 Simba-UW-tf-dev-1.93.3/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.93.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/CLAHE.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/ffmpeg_progress_bar.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/detect_scene_changes.py
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/watermark.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/clean_sleap_filename.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/downsample_video_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/crossfade.py
--rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/shift_geometries.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/downsample_multiple_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/mahalanobis.py
--rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/superpixels.py
--rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/img_conv.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/blurbox.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/superimpose_frame_count.py
--rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/inset_overlay_video.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/lbp.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/eta_squared.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_mp4.py
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/change_img_file_format.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/bg_substraction.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fleiss_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/jaccard_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/profiler.py
--rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/manhattan_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/seekable.py
--rw-r--r--   0 simon      (501) staff       (20)    12182 2024-05-19 17:38:25.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/superimpose_popups.py
--rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/superimpose_elapsed_time.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/relative_risk.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/contrast.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/youden_j.py
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/color_filtering.py
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.93.3/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.93.3/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.93.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.93.3/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   190387 2024-05-19 17:29:59.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/brightness_contrast_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.93.3/simba/video_processors/clahe_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    83726 2024-05-19 17:49:14.000000 Simba-UW-tf-dev-1.93.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.93.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.93.3/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/brightness.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-19 20:36:14.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    24636 2024-05-19 20:36:15.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-19 20:36:14.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)     1078 2024-05-19 20:36:14.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-19 20:36:14.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-19 20:36:14.000000 Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.93.3/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.93.3/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.93.3/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.93.3/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.93.3/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.3/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.3/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.93.3/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.93.3/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.3/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-19 20:36:13.000000 Simba-UW-tf-dev-1.93.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-19 20:36:16.000000 Simba-UW-tf-dev-1.93.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.93.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)   143776 2024-05-20 14:18:40.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.93.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.93.4/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-20 14:20:14.000000 Simba-UW-tf-dev-1.93.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.93.4/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1173 2024-05-19 16:18:01.000000 Simba-UW-tf-dev-1.93.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.93.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.4/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.93.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.93.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.93.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    17201 2024-05-14 11:12:57.000000 Simba-UW-tf-dev-1.93.4/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.93.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/CLAHE.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/ffmpeg_progress_bar.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     9124 2024-05-20 13:37:45.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_text.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/detect_scene_changes.py
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/watermark.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/clean_sleap_filename.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/downsample_video_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/crossfade.py
+-rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/shift_geometries.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/downsample_multiple_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/mahalanobis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/superpixels.py
+-rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/img_conv.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/blurbox.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_frame_count.py
+-rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/inset_overlay_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/lbp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/eta_squared.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_mp4.py
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/change_img_file_format.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/bg_substraction.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fleiss_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/jaccard_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/profiler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/manhattan_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/seekable.py
+-rw-r--r--   0 simon      (501) staff       (20)    26677 2024-05-20 14:18:40.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_popups.py
+-rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_elapsed_time.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/relative_risk.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/contrast.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/youden_j.py
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/color_filtering.py
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.93.4/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.93.4/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.93.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.93.4/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   201425 2024-05-20 14:13:50.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/brightness_contrast_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.93.4/simba/video_processors/clahe_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    84226 2024-05-20 14:20:25.000000 Simba-UW-tf-dev-1.93.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.93.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.93.4/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:52.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     4267 2024-05-20 14:19:55.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/blur.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/brightness.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    24698 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1078 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-20 14:22:51.000000 Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.93.4/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.93.4/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.93.4/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.93.4/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.93.4/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.4/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.4/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.93.4/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.93.4/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.4/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-20 14:22:49.000000 Simba-UW-tf-dev-1.93.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-20 14:22:53.000000 Simba-UW-tf-dev-1.93.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.93.3/PKG-INFO` & `Simba-UW-tf-dev-1.93.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.93.3
+Version: 1.93.4
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     convert_video_powerpoint_compatible_format, copy_img_folder,
     crop_multiple_videos, crop_multiple_videos_circles,
     crop_multiple_videos_polygons, crop_single_video, crop_single_video_circle,
     crop_single_video_polygon, downsample_video, extract_frame_range,
     extract_frames_single_video, frames_to_movie, gif_creator,
     multi_split_video, remove_beginning_of_video, resize_videos_by_height,
     resize_videos_by_width, superimpose_frame_count, video_concatenator,
-    video_to_greyscale, watermark_video, superimpose_video_progressbar, superimpose_elapsed_time)
+    video_to_greyscale, watermark_video, superimpose_video_progressbar, superimpose_elapsed_time, superimpose_overlay_video, superimpose_video_names, superimpose_freetext, roi_blurbox)
 
 sys.setrecursionlimit(10**7)
 
 
 class CLAHEPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title="CLAHE VIDEO CONVERSION")
@@ -2577,15 +2577,15 @@
         opacities = [round(x, 1) for x in list(np.arange(0.1, 1.1, 0.1))]
         self.selected_img = FileSelect(settings_frm, "WATERMARK IMAGE PATH:", title="Select an image file", file_types=[("VIDEO", Options.ALL_IMAGE_FORMAT_OPTIONS.value)], lblwidth=25)
         self.location_dropdown = DropDownMenu(settings_frm, "WATERMARK LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
         self.opacity_dropdown = DropDownMenu(settings_frm, "WATERMARK OPACITY:", opacities, labelwidth=25)
         self.size_dropdown = DropDownMenu(settings_frm, "WATERMARK SCALE %:", list(range(5, 100, 5)), labelwidth=25)
 
         self.location_dropdown.setChoices('TOP LEFT')
-        self.opacity_dropdown.setChoices(50)
+        self.opacity_dropdown.setChoices(0.5)
         self.size_dropdown.setChoices(5)
 
         settings_frm.grid(row=0, column=0, sticky=NW)
         self.selected_img.grid(row=0, column=0, sticky=NW)
         self.location_dropdown.grid(row=1, column=0, sticky=NW)
         self.opacity_dropdown.grid(row=2, column=0, sticky=NW)
         self.size_dropdown.grid(row=3, column=0, sticky=NW)
@@ -2744,12 +2744,218 @@
             check_if_dir_exists(in_dir=data_path)
 
         threading.Thread(target=superimpose_video_progressbar(video_path=data_path,
                                                               bar_height=bar_size,
                                                               color=bar_clr,
                                                               position=loc)).start()
 
+class SuperimposeVideoPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="SUPER-IMPOSE VIDEO ON VIDEO")
+        self.LOCATIONS = {'TOP LEFT': 'top_left', 'TOP RIGHT': 'top_right', 'BOTTOM LEFT': 'bottom_left', 'BOTTOM RIGHT': 'bottom_right', 'CENTER': 'center'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        opacities = [round(x, 1) for x in list(np.arange(0.1, 1.1, 0.1))]
+        scales = [round(x, 2) for x in list(np.arange(0.05, 1.0, 0.05))]
+        self.main_video_path = FileSelect(settings_frm, "MAIN VIDEO PATH:", title="Select a video file", file_types=[("VIDEO", Options.ALL_VIDEO_FORMAT_OPTIONS.value)], lblwidth=25)
+        self.overlay_video_path = FileSelect(settings_frm, "OVERLAY VIDEO PATH:", title="Select a video file", file_types=[("VIDEO", Options.ALL_VIDEO_FORMAT_OPTIONS.value)], lblwidth=25)
+        self.location_dropdown = DropDownMenu(settings_frm, "OVERLAY VIDEO LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.opacity_dropdown = DropDownMenu(settings_frm, "OVERLAY VIDEO OPACITY:", opacities, labelwidth=25)
+        self.size_dropdown = DropDownMenu(settings_frm, "OVERLAY VIDEO SCALE (%):", scales, labelwidth=25)
+
+        self.location_dropdown.setChoices('TOP LEFT')
+        self.opacity_dropdown.setChoices(0.5)
+        self.size_dropdown.setChoices(0.05)
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.main_video_path.grid(row=0, column=0, sticky=NW)
+        self.overlay_video_path.grid(row=1, column=0, sticky=NW)
+        self.location_dropdown.grid(row=2, column=0, sticky=NW)
+        self.opacity_dropdown.grid(row=3, column=0, sticky=NW)
+        self.size_dropdown.grid(row=4, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
+        self.main_frm.mainloop()
+
+    def run(self):
+        loc = self.location_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        opacity = float(self.opacity_dropdown.getChoices())
+        size = float(self.size_dropdown.getChoices())
+        video_path = self.main_video_path.file_path
+        overlay_path = self.overlay_video_path.file_path
+        check_file_exist_and_readable(file_path=video_path)
+        check_file_exist_and_readable(file_path=overlay_path)
+        threading.Thread(target=superimpose_overlay_video(video_path=video_path,
+                                                          overlay_video_path=overlay_path,
+                                                          position=loc,
+                                                          opacity=opacity,
+                                                          scale=size)).start()
+
+class SuperimposeVideoNamesPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="SUPER-IMPOSE VIDEO NAMES ON VIDEOS")
+        self.LOCATIONS = {'TOP LEFT': 'top_left', 'TOP RIGHT': 'top_right', 'TOP MIDDLE': 'top_middle', 'BOTTOM LEFT': 'bottom_left', 'BOTTOM RIGHT': 'bottom_right', 'BOTTOM MIDDLE': 'bottom_middle'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.color_dict = get_color_dict()
+
+        self.location_dropdown = DropDownMenu(settings_frm, "VIDEO NAME TEXT LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.font_size_dropdown = DropDownMenu(settings_frm, "FONT SIZE:", list(range(5, 105, 5)), labelwidth=25)
+        self.font_color_dropdown = DropDownMenu(settings_frm, "FONT COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_dropdown = DropDownMenu(settings_frm, "FONT BORDER COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_width_dropdown = DropDownMenu(settings_frm, "FONT BORDER WIDTH:", list(range(2, 52, 2)), labelwidth=25)
+
+        self.location_dropdown.setChoices('TOP LEFT')
+        self.font_size_dropdown.setChoices(20)
+        self.font_color_dropdown.setChoices('White')
+        self.font_border_dropdown.setChoices('Black')
+        self.font_border_width_dropdown.setChoices(2)
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.location_dropdown.grid(row=0, column=0, sticky=NW)
+        self.font_size_dropdown.grid(row=1, column=0, sticky=NW)
+        self.font_color_dropdown.grid(row=2, column=0, sticky=NW)
+        self.font_border_dropdown.grid(row=3, column=0, sticky=NW)
+        self.font_border_width_dropdown.grid(row=4, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SINGLE VIDEO - SUPERIMPOSE VIDEO NAME", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN - SINGLE VIDEO", command=lambda: self.run(multiple=False))
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="MULTIPLE VIDEOS - SUPERIMPOSE VIDEO NAME", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video_dir = FolderSelect(multiple_videos_frm, "VIDEO DIRECTORY PATH:", title="Select a video directory", lblwidth=25)
+        multiple_videos_run = Button(multiple_videos_frm, text="RUN - MULTIPLE VIDEOS", command=lambda: self.run(multiple=True))
+
+        multiple_videos_frm.grid(row=2, column=0, sticky="NW")
+        self.selected_video_dir.grid(row=0, column=0, sticky="NW")
+        multiple_videos_run.grid(row=1, column=0, sticky="NW")
+        self.main_frm.mainloop()
+
+    def run(self, multiple: bool):
+        loc = self.location_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        font_size = int(self.font_size_dropdown.getChoices())
+        font_clr = self.font_color_dropdown.getChoices()
+        font_border_clr = self.font_border_dropdown.getChoices()
+        font_border_width = int(self.font_border_width_dropdown.getChoices())
+        if not multiple:
+            data_path = self.selected_video.file_path
+            check_file_exist_and_readable(file_path=data_path)
+        else:
+            data_path = self.selected_video_dir.folder_path
+            check_if_dir_exists(in_dir=data_path)
+
+        threading.Thread(target=superimpose_video_names(video_path=data_path,
+                                                         font_size=font_size,
+                                                         font_color=font_clr,
+                                                         font_border_color=font_border_clr,
+                                                         font_border_width=font_border_width,
+                                                         position=loc)).start()
+
+class SuperimposeTextPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="SUPER-IMPOSE TEXT ON VIDEOS")
+        self.LOCATIONS = {'TOP LEFT': 'top_left', 'TOP RIGHT': 'top_right', 'TOP MIDDLE': 'top_middle', 'BOTTOM LEFT': 'bottom_left', 'BOTTOM RIGHT': 'bottom_right', 'BOTTOM MIDDLE': 'bottom_middle'}
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.color_dict = get_color_dict()
+
+        self.location_dropdown = DropDownMenu(settings_frm, "TEXT LOCATION:", list(self.LOCATIONS.keys()), labelwidth=25)
+        self.text_eb = Entry_Box(parent=settings_frm, labelwidth=25, entry_box_width=50, fileDescription='TEXT:')
+        self.font_size_dropdown = DropDownMenu(settings_frm, "FONT SIZE:", list(range(5, 105, 5)), labelwidth=25)
+        self.font_color_dropdown = DropDownMenu(settings_frm, "FONT COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_dropdown = DropDownMenu(settings_frm, "FONT BORDER COLOR:", list(self.color_dict.keys()), labelwidth=25)
+        self.font_border_width_dropdown = DropDownMenu(settings_frm, "FONT BORDER WIDTH:", list(range(2, 52, 2)), labelwidth=25)
+
+        self.location_dropdown.setChoices('TOP LEFT')
+        self.font_size_dropdown.setChoices(20)
+        self.font_color_dropdown.setChoices('White')
+        self.font_border_dropdown.setChoices('Black')
+        self.font_border_width_dropdown.setChoices(2)
+
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.location_dropdown.grid(row=0, column=0, sticky=NW)
+        self.text_eb.grid(row=1, column=0, sticky=NW)
+        self.font_size_dropdown.grid(row=2, column=0, sticky=NW)
+        self.font_color_dropdown.grid(row=3, column=0, sticky=NW)
+        self.font_border_dropdown.grid(row=4, column=0, sticky=NW)
+        self.font_border_width_dropdown.grid(row=5, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SINGLE VIDEO - SUPERIMPOSE TEXT", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN - SINGLE VIDEO", command=lambda: self.run(multiple=False))
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="MULTIPLE VIDEOS - SUPERIMPOSE TEXT", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video_dir = FolderSelect(multiple_videos_frm, "VIDEO DIRECTORY PATH:", title="Select a video directory", lblwidth=25)
+        multiple_videos_run = Button(multiple_videos_frm, text="RUN - MULTIPLE VIDEOS", command=lambda: self.run(multiple=True))
+
+        multiple_videos_frm.grid(row=2, column=0, sticky="NW")
+        self.selected_video_dir.grid(row=0, column=0, sticky="NW")
+        multiple_videos_run.grid(row=1, column=0, sticky="NW")
+        self.main_frm.mainloop()
+
+    def run(self, multiple: bool):
+        loc = self.location_dropdown.getChoices()
+        loc = self.LOCATIONS[loc]
+        text = self.text_eb.entry_get
+        check_str(name='text', value=text)
+        font_size = int(self.font_size_dropdown.getChoices())
+        font_clr = self.font_color_dropdown.getChoices()
+        font_border_clr = self.font_border_dropdown.getChoices()
+        font_border_width = int(self.font_border_width_dropdown.getChoices())
+        if not multiple:
+            data_path = self.selected_video.file_path
+            check_file_exist_and_readable(file_path=data_path)
+        else:
+            data_path = self.selected_video_dir.folder_path
+            check_if_dir_exists(in_dir=data_path)
+
+        threading.Thread(target=superimpose_freetext(video_path=data_path,
+                                                     text=text,
+                                                     font_size=font_size,
+                                                     font_color=font_clr,
+                                                     font_border_color=font_border_clr,
+                                                     font_border_width=font_border_width,
+                                                     position=loc)).start()
+
+
+class BoxBlurPopUp(PopUpMixin):
+    def __init__(self):
+        PopUpMixin.__init__(self, title="BOX BLUR VIDEOS")
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="SETTINGS", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        blur_lvl = [round(x, 2) for x in list(np.arange(0.05, 1.0, 0.05))]
+        self.blur_lvl_dropdown = DropDownMenu(settings_frm, "BLUR LEVEL:", blur_lvl, labelwidth=25)
+        self.invert_dropdown = DropDownMenu(settings_frm, "INVERT BLUR REGION:", ['TRUE', 'FALSE'], labelwidth=25)
+
+        self.blur_lvl_dropdown.setChoices(0.02)
+        self.invert_dropdown.setChoices('FALSE')
+        settings_frm.grid(row=0, column=0, sticky=NW)
+        self.blur_lvl_dropdown.grid(row=0, column=0, sticky=NW)
+        self.invert_dropdown.grid(row=1, column=0, sticky=NW)
+
+        single_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header="APPLY BOX-BLUR", icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(single_video_frm, "VIDEO PATH:", title="Select a video file", lblwidth=25, file_types=[("VIDEO FILE", Options.ALL_VIDEO_FORMAT_STR_OPTIONS.value)])
+        single_video_run = Button(single_video_frm, text="RUN", command=lambda: self.run())
+
+        single_video_frm.grid(row=1, column=0, sticky="NW")
+        self.selected_video.grid(row=0, column=0, sticky="NW")
+        single_video_run.grid(row=1, column=0, sticky="NW")
+
+        self.main_frm.mainloop()
+
+    def run(self):
+        video_path = self.selected_video.file_path
+        check_file_exist_and_readable(file_path=video_path)
+        blur_lvl = float(self.blur_lvl_dropdown.getChoices())
+        invert = str_2_bool(self.invert_dropdown.getChoices())
+        threading.Thread(target=roi_blurbox(video_path=video_path, blur_level=blur_lvl, invert=invert)).start()
+
 
 
 
 # ClipMultipleVideosByFrameNumbers
 # ClipMultipleVideosByFrameNumbers(data_dir='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/videos/test', save_dir='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/videos/clipped')
```

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.93.4/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.93.4/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.93.4/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.93.4/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.93.4/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.93.4/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.93.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.93.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -292,20 +292,20 @@
 00001230: 4c01 4d01 4f01 5001 5201 5b01 5c01 5e01  L.M.O.P.R.[.\.^.
 00001240: 5f01 6101 6a01 6b01 6c01 6e01 7701 7801  _.a.j.k.l.n.w.x.
 00001250: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
 00001260: 9501 9601 9801 9901 9b01 9c01 a501 b200  ................
 00001270: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
 00001280: 0000 0000 0000 0000 0000 0000 0001 b300  ................
 00001290: 0000 0700 7300 6100 6e00 6400 6200 6f00  ....s.a.n.d.b.o.
-000012a0: 786d 6f44 4462 6c6f 6200 0000 086c f80f  xmoDDblob....l..
-000012b0: 62bf fac5 4100 0000 0700 7300 6100 6e00  b...A.....s.a.n.
+000012a0: 786d 6f44 4462 6c6f 6200 0000 08c1 9c4b  xmoDDblob......K
+000012b0: a0c9 fdc5 4100 0000 0700 7300 6100 6e00  ....A.....s.a.n.
 000012c0: 6400 6200 6f00 786d 6f64 4462 6c6f 6200  d.b.o.xmodDblob.
-000012d0: 0000 08ca 7696 58bf fac5 4100 0000 0700  ....v.X...A.....
+000012d0: 0000 08c1 9c4b a0c9 fdc5 4100 0000 0700  .....K....A.....
 000012e0: 7300 6100 6e00 6400 6200 6f00 7870 6831  s.a.n.d.b.o.xph1
-000012f0: 5363 6f6d 7000 0000 0000 1420 0000 0000  Scomp...... ....
+000012f0: 5363 6f6d 7000 0000 0000 1510 0000 0000  Scomp...........
 00001300: 0700 7300 6100 6e00 6400 6200 6f00 7876  ..s.a.n.d.b.o.xv
 00001310: 5372 6e6c 6f6e 6700 0000 0100 0000 1b00  Srnlong.........
 00001320: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
 00001330: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
 00001340: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
 00001350: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
 00001360: 0000 0347 a400 0000 1b00 7400 6800 6900  ...G......t.h.i.
@@ -320,20 +320,20 @@
 000013f0: 4462 6c6f 6200 0000 08e4 2b79 2913 eec5  Dblob.....+y)...
 00001400: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
 00001410: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
 00001420: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 00001430: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
 00001440: 6f6d 7000 0000 0000 0440 0000 0000 0200  omp......@......
 00001450: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
-00001460: 0dd7 0f00 0000 0200 7500 696d 6f44 4462  ........u.imoDDb
+00001460: 0e78 3600 0000 0200 7500 696d 6f44 4462  .x6.....u.imoDDb
 00001470: 6c6f 6200 0000 0874 394b 535b e7c5 4100  lob....t9KS[..A.
 00001480: 0000 0200 7500 696d 6f64 4462 6c6f 6200  ....u.imodDblob.
 00001490: 0000 0874 394b 535b e7c5 4100 0000 0200  ...t9KS[..A.....
 000014a0: 7500 6970 6831 5363 6f6d 7000 0000 0000  u.iph1Scomp.....
-000014b0: 1180 0000 0000 0c00 7500 6e00 7300 7500  ........u.n.s.u.
+000014b0: 1230 0000 0000 0c00 7500 6e00 7300 7500  .0......u.n.s.u.
 000014c0: 7000 6500 7200 7600 6900 7300 6500 6462  p.e.r.v.i.s.e.db
 000014d0: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
 000014e0: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
 000014f0: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
 00001500: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
 00001510: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
 00001520: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
@@ -459,19 +459,19 @@
 00001ca0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00001cb0: 6261 7208 0908 095f 1018 7b7b 3135 312c  bar...._..{{151,
 00001cc0: 2039 367d 2c20 7b31 3138 302c 2035 3638   96}, {1180, 568
 00001cd0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 00001ce0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001d00: 0000 0005 0075 0074 0069 006c 0073 6c67  .....u.t.i.l.slg
-00001d10: 3153 636f 6d70 0000 0000 0008 37ec 0000  1Scomp......7...
+00001d10: 3153 636f 6d70 0000 0000 0008 38bd 0000  1Scomp......8...
 00001d20: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001d30: 626c 6f62 0000 0008 a947 2063 d3f9 c541  blob.....G c...A
+00001d30: 626c 6f62 0000 0008 ab4e e1ff 1efb c541  blob.....N.....A
 00001d40: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
-00001d50: 6444 626c 6f62 0000 0008 a947 2063 d3f9  dDblob.....G c..
+00001d50: 6444 626c 6f62 0000 0008 ab4e e1ff 1efb  dDblob.....N....
 00001d60: c541 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
 00001d70: 7068 3153 636f 6d70 0000 0000 0009 4000  ph1Scomp......@.
 00001d80: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
 00001d90: 726e 6c6f 6e67 0000 0001 0000 0010 0076  rnlong.........v
 00001da0: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
 00001db0: 0063 0065 0073 0073 006f 0072 0073 6277  .c.e.s.s.o.r.sbw
 00001dc0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
@@ -485,44 +485,44 @@
 00001e40: 392c 2033 3030 7d2c 207b 3932 302c 2034  9, 300}, {920, 4
 00001e50: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
 00001e60: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
 00001e70: 000d 0000 0000 0000 0000 0000 0000 0000  ................
 00001e80: 008b 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00001e90: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00001ea0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00001eb0: 0000 0007 7707 0000 0010 0076 0069 0064  ....w......v.i.d
+00001eb0: 0000 0008 39d4 0000 0010 0076 0069 0064  ....9......v.i.d
 00001ec0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00001ed0: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00001ee0: 6f62 0000 0008 297b 803c a0fa c541 0000  ob....){.<...A..
+00001ee0: 6f62 0000 0008 818d 2d0f c9fd c541 0000  ob......-....A..
 00001ef0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00001f00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00001f10: 0073 6d6f 6444 626c 6f62 0000 0008 297b  .smodDblob....){
-00001f20: 803c a0fa c541 0000 0010 0076 0069 0064  .<...A.....v.i.d
+00001f10: 0073 6d6f 6444 626c 6f62 0000 0008 818d  .smodDblob......
+00001f20: 2d0f c9fd c541 0000 0010 0076 0069 0064  -....A.....v.i.d
 00001f30: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00001f40: 0073 0073 006f 0072 0073 7068 3153 636f  .s.s.o.r.sph1Sco
-00001f50: 6d70 0000 0000 0008 6000 0000 0010 0076  mp......`......v
+00001f50: 6d70 0000 0000 0009 2000 0000 0010 0076  mp...... ......v
 00001f60: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
 00001f70: 0063 0065 0073 0073 006f 0072 0073 7653  .c.e.s.s.o.r.svS
 00001f80: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 002f 0000 000b  .........../....
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0000 e6d2 0000 000b 005f 005f 0070  ..........._._.p
+00002030: 0000 0000 e8f5 0000 000b 005f 005f 0070  ..........._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 f19f 2831  moDDblob......(1
-00002060: 57f9 c541 0000 000b 005f 005f 0070 0079  W..A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 0d7a de28  moDDblob.....z.(
+00002060: c7fd c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00002080: 6444 626c 6f62 0000 0008 f19f 2831 57f9  dDblob......(1W.
+00002080: 6444 626c 6f62 0000 0008 0d7a de28 c7fd  dDblob.....z.(..
 00002090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0001 0000 0000 0006  comp............
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00b7 6270 6c69 7374 3030  blob....bplist00
 000020e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 000020f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
@@ -648,15 +648,15 @@
 00002870: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00002880: 6261 7208 0908 095f 1018 7b7b 3238 392c  bar...._..{{289,
 00002890: 2033 3030 7d2c 207b 3932 302c 2034 3336   300}, {920, 436
 000028a0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 000028b0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 000028c0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 000028d0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-000028e0: 6c67 3153 636f 6d70 0000 0000 01ce c559  lg1Scomp.......Y
+000028e0: 6c67 3153 636f 6d70 0000 0000 01ce c54f  lg1Scomp.......O
 000028f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00002900: 6c73 7643 626c 6f62 0000 030a 6270 6c69  lsvCblob....bpli
 00002910: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 00002920: 1b55 560a 5858 6963 6f6e 5369 7a65 5f10  .UV.XXiconSize_.
 00002930: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 00002940: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 00002950: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
@@ -740,18 +740,18 @@
 00002e30: 4101 4201 4301 4c01 4e01 5001 5101 5201  A.B.C.L.N.P.Q.R.
 00002e40: 5b01 5d01 5f01 6001 6101 6a01 6c01 6d01  [.]._.`.a.j.l.m.
 00002e50: 6e01 7701 7901 7b01 7c01 7d01 8601 8801  n.w.y.{.|.}.....
 00002e60: 8901 8a01 9301 9501 9701 9801 9901 9a01  ................
 00002e70: a301 b000 0000 0000 0002 0100 0000 0000  ................
 00002e80: 0000 4800 0000 0000 0000 0000 0000 0000  ..H.............
 00002e90: 0001 b100 0000 0600 6d00 6900 7800 6900  ........m.i.x.i.
-00002ea0: 6e00 736d 6f44 4462 6c6f 6200 0000 0821  n.smoDDblob....!
-00002eb0: bf0c 4ded f9c5 4100 0000 0600 6d00 6900  ..M...A.....m.i.
+00002ea0: 6e00 736d 6f44 4462 6c6f 6200 0000 0835  n.smoDDblob....5
+00002eb0: 9f8d 57fc fbc5 4100 0000 0600 6d00 6900  ..W...A.....m.i.
 00002ec0: 7800 6900 6e00 736d 6f64 4462 6c6f 6200  x.i.n.smodDblob.
-00002ed0: 0000 08f8 f68e 7999 f6c5 4100 0000 0600  ......y...A.....
+00002ed0: 0000 0835 9f8d 57fc fbc5 4100 0000 0600  ...5..W...A.....
 00002ee0: 6d00 6900 7800 6900 6e00 7370 6831 5363  m.i.x.i.n.sph1Sc
 00002ef0: 6f6d 7000 0000 0001 e1e0 0000 0000 0600  omp.............
 00002f00: 6d00 6900 7800 6900 6e00 7376 5372 6e6c  m.i.x.i.n.svSrnl
 00002f10: 6f6e 6700 0000 0100 0000 0500 6d00 6f00  ong.........m.o.
 00002f20: 6400 6500 6c6c 6731 5363 6f6d 7000 0000  d.e.llg1Scomp...
 00002f30: 0000 0217 c200 0000 0500 6d00 6f00 6400  ..........m.o.d.
 00002f40: 6500 6c6d 6f44 4462 6c6f 6200 0000 0899  e.lmoDDblob.....
@@ -951,21 +951,21 @@
 00003b60: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
 00003b70: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
 00003b80: 7300 5f00 6100 7200 6300 6800 6900 7600  s._.a.r.c.h.i.v.
 00003b90: 6570 6831 5363 6f6d 7000 0000 0000 3240  eph1Scomp.....2@
 00003ba0: 0000 0000 0e00 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
 00003bb0: 6900 6d00 7000 6f00 7200 7400 6500 7200  i.m.p.o.r.t.e.r.
 00003bc0: 736c 6731 5363 6f6d 7000 0000 0000 0403  slg1Scomp.......
-00003bd0: 8100 0000 0e00 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
+00003bd0: c500 0000 0e00 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
 00003be0: 6900 6d00 7000 6f00 7200 7400 6500 7200  i.m.p.o.r.t.e.r.
-00003bf0: 736d 6f44 4462 6c6f 6200 0000 0839 ed30  smoDDblob....9.0
-00003c00: 4da9 c2c5 4100 0000 0e00 7000 6f00 7300  M...A.....p.o.s.
+00003bf0: 736d 6f44 4462 6c6f 6200 0000 0899 dcd9  smoDDblob.......
+00003c00: 7343 fbc5 4100 0000 0e00 7000 6f00 7300  sC..A.....p.o.s.
 00003c10: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00003c20: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
-00003c30: 0839 ed30 4da9 c2c5 4100 0000 0e00 7000  .9.0M...A.....p.
+00003c30: 0899 dcd9 7343 fbc5 4100 0000 0e00 7000  ....sC..A.....p.
 00003c40: 6f00 7300 6500 5f00 6900 6d00 7000 6f00  o.s.e._.i.m.p.o.
 00003c50: 7200 7400 6500 7200 7370 6831 5363 6f6d  r.t.e.r.sph1Scom
 00003c60: 7000 0000 0000 0510 0000 0000 0f00 7000  p.............p.
 00003c70: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00003c80: 6500 7300 7300 6f00 7200 736c 6731 5363  e.s.s.o.r.slg1Sc
 00003c90: 6f6d 7000 0000 0000 00e1 e500 0000 0f00  omp.............
 00003ca0: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
@@ -989,20 +989,20 @@
 00003dc0: 6964 6562 6172 0809 0809 5f10 187b 7b31  idebar...._..{{1
 00003dd0: 3531 2c20 3936 7d2c 207b 3131 3830 2c20  51, 96}, {1180, 
 00003de0: 3536 387d 7d09 0815 232f 3b52 5f6b 6c6d  568}}...#/;R_klm
 00003df0: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
 00003e00: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
 00003e10: 0000 8b00 0000 0900 7200 6f00 6900 5f00  ........r.o.i._.
 00003e20: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
-00003e30: 7000 0000 0000 0697 3a00 0000 0900 7200  p.......:.....r.
+00003e30: 7000 0000 0000 0698 1200 0000 0900 7200  p.............r.
 00003e40: 6f00 6900 5f00 7400 6f00 6f00 6c00 736d  o.i._.t.o.o.l.sm
-00003e50: 6f44 4462 6c6f 6200 0000 08f7 0c7c 0e99  oDDblob......|..
-00003e60: f6c5 4100 0000 0900 7200 6f00 6900 5f00  ..A.....r.o.i._.
+00003e50: 6f44 4462 6c6f 6200 0000 082b c8fc 62c8  oDDblob....+..b.
+00003e60: fbc5 4100 0000 0900 7200 6f00 6900 5f00  ..A.....r.o.i._.
 00003e70: 7400 6f00 6f00 6c00 736d 6f64 4462 6c6f  t.o.o.l.smodDblo
-00003e80: 6200 0000 08f7 0c7c 0e99 f6c5 4100 0000  b......|....A...
+00003e80: 6200 0000 082b c8fc 62c8 fbc5 4100 0000  b....+..b...A...
 00003e90: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
 00003ea0: 6c00 7370 6831 5363 6f6d 7000 0000 0000  l.sph1Scomp.....
 00003eb0: 0820 0000 0000 0900 7200 6f00 6900 5f00  . ......r.o.i._.
 00003ec0: 7400 6f00 6f00 6c00 7376 5372 6e6c 6f6e  t.o.o.l.svSrnlon
 00003ed0: 6700 0000 0100 0000 0700 7300 6100 6e00  g.........s.a.n.
 00003ee0: 6400 6200 6f00 7862 7773 7062 6c6f 6200  d.b.o.xbwspblob.
 00003ef0: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
@@ -1014,15 +1014,15 @@
 00003f50: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
 00003f60: 0809 5f10 187b 7b31 3531 2c20 3936 7d2c  .._..{{151, 96},
 00003f70: 207b 3131 3830 2c20 3536 387d 7d09 0815   {1180, 568}}...
 00003f80: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
 00003f90: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00003fa0: 0000 0000 0000 0000 0000 8b00 0000 0700  ................
 00003fb0: 7300 6100 6e00 6400 6200 6f00 786c 6731  s.a.n.d.b.o.xlg1
-00003fc0: 5363 6f6d 7000 0000 0000 0e62 2c00 0000  Scomp......b,...
+00003fc0: 5363 6f6d 7000 0000 0000 0f2d b300 0000  Scomp......-....
 00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004000: 0000 0000 0000 0006 0000 0000 0000 400b  ..............@.
 00004010: 0000 0045 0000 100c 0000 040a 0000 200c  ...E.......... .
 00004020: 0000 300c 0000 0000 0000 0000 0000 0000  ..0.............
 00004030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.93.4/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.93.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.93.4/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.93.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.93.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.93.4/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/CLAHE.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/CLAHE.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/ffmpeg_progress_bar.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/ffmpeg_progress_bar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/detect_scene_changes.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/detect_scene_changes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/watermark.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/watermark.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/clean_sleap_filename.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/clean_sleap_filename.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/downsample_video_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/downsample_video_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/crossfade.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/crossfade.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/shift_geometries.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/shift_geometries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_bw.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/downsample_multiple_videos_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/downsample_multiple_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/mahalanobis.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/mahalanobis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/superpixels.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/superpixels.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/img_conv.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/img_conv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/blurbox.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/blurbox.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/superimpose_frame_count.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_frame_count.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/inset_overlay_video.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/inset_overlay_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/eta_squared.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/eta_squared.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_mp4.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_mp4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/change_img_file_format.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/change_img_file_format.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/bg_substraction.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/bg_substraction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fleiss_kappa.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convert_to_popup.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convert_to_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/jaccard_distance.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/jaccard_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/manhattan_distance.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/seekable.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/seekable.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/superimpose_elapsed_time.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/superimpose_elapsed_time.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/relative_risk.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/relative_risk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/contrast.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/contrast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/youden_j.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/youden_j.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.93.4/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.93.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.93.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.93.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.93.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.93.4/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.93.4/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.93.4/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.93.4/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.93.4/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.93.4/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.93.4/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.93.4/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.93.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.93.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.93.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/video_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9755,2146 +9755,2836 @@
 000261a0: 5f73 7563 6365 7373 286d 7367 3d66 277b  _success(msg=f'{
 000261b0: 6c65 6e28 7669 6465 6f5f 7061 7468 7329  len(video_paths)
 000261c0: 7d20 7761 7465 726d 6172 6b65 6420 7669  } watermarked vi
 000261d0: 6465 6f28 7329 2073 6176 6564 2069 6e20  deo(s) saved in 
 000261e0: 7b73 6176 655f 6469 727d 272c 2065 6c61  {save_dir}', ela
 000261f0: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
 00026200: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
-00026210: 290a 0a64 6566 2069 6e73 6574 5f6f 7665  )..def inset_ove
-00026220: 726c 6179 5f76 6964 656f 2876 6964 656f  rlay_video(video
-00026230: 5f70 6174 683a 2055 6e69 6f6e 5b73 7472  _path: Union[str
-00026240: 2c20 6f73 2e50 6174 684c 696b 655d 2c0a  , os.PathLike],.
-00026250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026260: 2020 2020 2020 2020 6f76 6572 6c61 795f          overlay_
-00026270: 7669 6465 6f5f 7061 7468 3a20 556e 696f  video_path: Unio
-00026280: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00026290: 6b65 5d2c 0a20 2020 2020 2020 2020 2020  ke],.           
-000262a0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-000262b0: 6974 696f 6e3a 204f 7074 696f 6e61 6c5b  ition: Optional[
-000262c0: 4c69 7465 7261 6c5b 2774 6f70 5f6c 6566  Literal['top_lef
-000262d0: 7427 2c20 2762 6f74 746f 6d5f 7269 6768  t', 'bottom_righ
-000262e0: 7427 2c20 2774 6f70 5f72 6967 6874 272c  t', 'top_right',
-000262f0: 2027 626f 7474 6f6d 5f6c 6566 7427 2c20   'bottom_left', 
-00026300: 2763 656e 7465 7227 5d5d 203d 2027 746f  'center']] = 'to
-00026310: 705f 6c65 6674 272c 0a20 2020 2020 2020  p_left',.       
-00026320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026330: 206f 7061 6369 7479 3a20 4f70 7469 6f6e   opacity: Option
-00026340: 616c 5b66 6c6f 6174 5d20 3d20 302e 352c  al[float] = 0.5,
-00026350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026360: 2020 2020 2020 2020 2073 6361 6c65 3a20           scale: 
-00026370: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00026380: 3d20 302e 3035 2c0a 2020 2020 2020 2020  = 0.05,.        
-00026390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263a0: 7361 7665 5f64 6972 3a20 4f70 7469 6f6e  save_dir: Option
-000263b0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
-000263c0: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
-000263d0: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
-000263e0: 2022 2222 0a20 2020 2049 6e73 6574 2061   """.    Inset a
-000263f0: 2076 6964 656f 206f 7665 726c 6179 206f   video overlay o
-00026400: 6e20 6120 7365 636f 6e64 2076 6964 656f  n a second video
-00026410: 2077 6974 6820 7370 6563 6966 6965 6420   with specified 
-00026420: 7369 7a65 2c20 6f70 6163 6974 792c 2061  size, opacity, a
-00026430: 6e64 206c 6f63 6174 696f 6e2e 0a0a 2020  nd location...  
-00026440: 2020 2e2e 2076 6964 656f 3a3a 205f 7374    .. video:: _st
-00026450: 6174 6963 2f69 6d67 2f69 6e73 6574 5f6f  atic/img/inset_o
-00026460: 7665 726c 6179 5f76 6964 656f 2e77 6562  verlay_video.web
-00026470: 6d0a 2020 2020 2020 203a 7769 6474 683a  m.       :width:
-00026480: 2037 3030 0a20 2020 2020 2020 3a6c 6f6f   700.       :loo
-00026490: 703a 0a0a 2020 2020 3a70 6172 616d 2055  p:..    :param U
-000264a0: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-000264b0: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
-000264c0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
-000264d0: 6865 2076 6964 656f 2066 696c 652e 0a20  he video file.. 
-000264e0: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
-000264f0: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
-00026500: 5d20 6f76 6572 6c61 795f 7669 6465 6f5f  ] overlay_video_
-00026510: 7061 7468 3a20 5468 6520 7061 7468 2074  path: The path t
-00026520: 6f20 7669 6465 6f20 746f 2062 6520 696e  o video to be in
-00026530: 7365 7274 6564 2069 6e74 6f20 7468 6520  serted into the 
-00026540: 6060 7669 6465 6f5f 7061 7468 6060 2076  ``video_path`` v
-00026550: 6964 656f 2e0a 2020 2020 3a70 6172 616d  ideo..    :param
-00026560: 204f 7074 696f 6e61 6c5b 7374 725d 2070   Optional[str] p
-00026570: 6f73 6974 696f 6e3a 2054 6865 2070 6f73  osition: The pos
-00026580: 6974 696f 6e20 6f66 2074 6865 2069 6e73  ition of the ins
-00026590: 6574 206f 7665 726c 6179 2076 6964 656f  et overlay video
-000265a0: 2e20 4f70 7469 6f6e 733a 2027 746f 705f  . Options: 'top_
-000265b0: 6c65 6674 272c 2027 626f 7474 6f6d 5f72  left', 'bottom_r
-000265c0: 6967 6874 272c 2027 746f 705f 7269 6768  ight', 'top_righ
-000265d0: 7427 2c20 2762 6f74 746f 6d5f 6c65 6674  t', 'bottom_left
-000265e0: 272c 2027 6365 6e74 6572 270a 2020 2020  ', 'center'.    
-000265f0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00026600: 666c 6f61 745d 206f 7061 6369 7479 3a20  float] opacity: 
-00026610: 5468 6520 6f70 6163 6974 7920 6f66 2074  The opacity of t
-00026620: 6865 2069 6e73 6574 206f 7665 726c 6179  he inset overlay
-00026630: 2076 6964 656f 2061 7320 6120 7661 6c75   video as a valu
-00026640: 6520 6265 7477 6565 6e20 302d 312e 302e  e between 0-1.0.
-00026650: 2031 2e30 206d 6561 6e69 6e67 2074 6865   1.0 meaning the
-00026660: 2073 616d 6520 6173 2069 6e70 7574 2069   same as input i
-00026670: 6d61 6765 2e20 4465 6661 756c 743a 2030  mage. Default: 0
-00026680: 2e35 2e0a 2020 2020 3a70 6172 616d 204f  .5..    :param O
-00026690: 7074 696f 6e61 6c5b 666c 6f61 745d 2073  ptional[float] s
-000266a0: 6361 6c65 3a20 5468 6520 7363 616c 6520  cale: The scale 
-000266b0: 6f66 2074 6865 2069 6e73 6574 206f 7665  of the inset ove
-000266c0: 726c 6179 2076 6964 656f 2061 7320 6120  rlay video as a 
-000266d0: 7261 7469 6f20 6f73 2074 6865 2069 6d61  ratio os the ima
-000266e0: 6765 2073 697a 652e 2044 6566 6175 6c74  ge size. Default
-000266f0: 3a20 302e 3035 2e0a 2020 2020 3a70 6172  : 0.05..    :par
-00026700: 616d 204f 7074 696f 6e61 6c5b 556e 696f  am Optional[Unio
-00026710: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-00026720: 6b65 5d5d 2073 6176 655f 6469 723a 2054  ke]] save_dir: T
-00026730: 6865 206c 6f63 6174 696f 6e20 7768 6572  he location wher
-00026740: 6520 746f 2073 6176 6520 7468 6520 6f75  e to save the ou
-00026750: 7470 7574 2076 6964 656f 2e20 4966 204e  tput video. If N
-00026760: 6f6e 652c 2074 6865 6e20 7361 7665 7320  one, then saves 
-00026770: 7468 6520 7669 6465 6f20 696e 2074 6865  the video in the
-00026780: 2073 616d 6520 6469 7265 6374 6f72 7920   same directory 
-00026790: 6173 2074 6865 2066 6972 7374 2076 6964  as the first vid
-000267a0: 656f 2e0a 2020 2020 3a72 6574 7572 6e3a  eo..    :return:
-000267b0: 204e 6f6e 650a 0a20 2020 203a 6578 616d   None..    :exam
-000267c0: 706c 653a 0a20 2020 203e 3e3e 2069 6e73  ple:.    >>> ins
-000267d0: 6574 5f6f 7665 726c 6179 5f76 6964 656f  et_overlay_video
-000267e0: 2876 6964 656f 5f70 6174 683d 272f 5573  (video_path='/Us
-000267f0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-00026800: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-00026810: 7562 6c65 7368 6f6f 7469 6e67 2f6d 756c  ubleshooting/mul
-00026820: 7469 5f61 6e69 6d61 6c5f 646c 635f 7477  ti_animal_dlc_tw
-00026830: 6f5f 6335 372f 7072 6f6a 6563 745f 666f  o_c57/project_fo
-00026840: 6c64 6572 2f76 6964 656f 732f 7761 7465  lder/videos/wate
-00026850: 726d 6172 6b2f 546f 6765 7468 6572 5f31  rmark/Together_1
-00026860: 5f70 6f77 6572 706f 696e 7472 6561 6479  _powerpointready
-00026870: 2e6d 7034 272c 206f 7665 726c 6179 5f76  .mp4', overlay_v
-00026880: 6964 656f 5f70 6174 683d 272f 5573 6572  ideo_path='/User
-00026890: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
-000268a0: 7370 6c61 7368 2e70 6e67 272c 2070 6f73  splash.png', pos
-000268b0: 6974 696f 6e3d 2774 6f70 5f6c 6566 7427  ition='top_left'
-000268c0: 2c20 6f70 6163 6974 793d 312e 302c 2073  , opacity=1.0, s
-000268d0: 6361 6c65 3d30 2e32 290a 2020 2020 2222  cale=0.2).    ""
-000268e0: 220a 0a20 2020 2074 696d 6572 203d 2053  "..    timer = S
-000268f0: 696d 6261 5469 6d65 7228 7374 6172 743d  imbaTimer(start=
-00026900: 5472 7565 290a 2020 2020 504f 5349 5449  True).    POSITI
-00026910: 4f4e 5320 3d20 5b27 746f 705f 6c65 6674  ONS = ['top_left
-00026920: 272c 2027 626f 7474 6f6d 5f72 6967 6874  ', 'bottom_right
-00026930: 272c 2027 746f 705f 7269 6768 7427 2c20  ', 'top_right', 
-00026940: 2762 6f74 746f 6d5f 6c65 6674 272c 2027  'bottom_left', '
-00026950: 6365 6e74 6572 275d 0a20 2020 2063 6865  center'].    che
-00026960: 636b 5f66 6c6f 6174 286e 616d 653d 6627  ck_float(name=f'
-00026970: 7b69 6e73 6574 5f6f 7665 726c 6179 5f76  {inset_overlay_v
-00026980: 6964 656f 2e5f 5f6e 616d 655f 5f7d 206f  ideo.__name__} o
-00026990: 7061 6369 7479 272c 2076 616c 7565 3d6f  pacity', value=o
-000269a0: 7061 6369 7479 2c20 6d69 6e5f 7661 6c75  pacity, min_valu
-000269b0: 653d 302e 3030 312c 206d 6178 5f76 616c  e=0.001, max_val
-000269c0: 7565 3d31 2e30 290a 2020 2020 6368 6563  ue=1.0).    chec
-000269d0: 6b5f 666c 6f61 7428 6e61 6d65 3d66 277b  k_float(name=f'{
-000269e0: 696e 7365 745f 6f76 6572 6c61 795f 7669  inset_overlay_vi
-000269f0: 6465 6f2e 5f5f 6e61 6d65 5f5f 7d20 7363  deo.__name__} sc
-00026a00: 616c 6527 2c20 7661 6c75 653d 7363 616c  ale', value=scal
-00026a10: 652c 206d 696e 5f76 616c 7565 3d30 2e30  e, min_value=0.0
-00026a20: 3031 2c20 6d61 785f 7661 6c75 653d 302e  01, max_value=0.
-00026a30: 3939 3929 0a20 2020 2063 6865 636b 5f73  999).    check_s
-00026a40: 7472 286e 616d 653d 6627 7b69 6e73 6574  tr(name=f'{inset
-00026a50: 5f6f 7665 726c 6179 5f76 6964 656f 2e5f  _overlay_video._
-00026a60: 5f6e 616d 655f 5f7d 2070 6f73 6974 696f  _name__} positio
-00026a70: 6e27 2c20 7661 6c75 653d 706f 7369 7469  n', value=positi
-00026a80: 6f6e 2c20 6f70 7469 6f6e 733d 504f 5349  on, options=POSI
-00026a90: 5449 4f4e 5329 0a20 2020 2063 6865 636b  TIONS).    check
-00026aa0: 5f66 696c 655f 6578 6973 745f 616e 645f  _file_exist_and_
-00026ab0: 7265 6164 6162 6c65 2866 696c 655f 7061  readable(file_pa
-00026ac0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
-00026ad0: 2020 2063 6865 636b 5f66 696c 655f 6578     check_file_ex
-00026ae0: 6973 745f 616e 645f 7265 6164 6162 6c65  ist_and_readable
-00026af0: 2866 696c 655f 7061 7468 3d6f 7665 726c  (file_path=overl
-00026b00: 6179 5f76 6964 656f 5f70 6174 6829 0a0a  ay_video_path)..
-00026b10: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
-00026b20: 7366 696c 6528 7669 6465 6f5f 7061 7468  sfile(video_path
-00026b30: 293a 0a20 2020 2020 2020 2076 6964 656f  ):.        video
-00026b40: 5f70 6174 6873 203d 205b 7669 6465 6f5f  _paths = [video_
-00026b50: 7061 7468 5d0a 2020 2020 656c 6966 206f  path].    elif o
-00026b60: 732e 7061 7468 2e69 7364 6972 2876 6964  s.path.isdir(vid
-00026b70: 656f 5f70 6174 6829 3a0a 2020 2020 2020  eo_path):.      
-00026b80: 2020 7669 6465 6f5f 7061 7468 7320 3d20    video_paths = 
-00026b90: 6c69 7374 2866 696e 645f 616c 6c5f 7669  list(find_all_vi
-00026ba0: 6465 6f73 5f69 6e5f 6469 7265 6374 6f72  deos_in_director
-00026bb0: 7928 6469 7265 6374 6f72 793d 7669 6465  y(directory=vide
-00026bc0: 6f5f 7061 7468 2c20 6173 5f64 6963 743d  o_path, as_dict=
-00026bd0: 5472 7565 2c20 7261 6973 655f 6572 726f  True, raise_erro
-00026be0: 723d 5472 7565 292e 7661 6c75 6573 2829  r=True).values()
-00026bf0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00026c00: 2020 2020 7261 6973 6520 496e 7661 6c69      raise Invali
-00026c10: 6449 6e70 7574 4572 726f 7228 6d73 673d  dInputError(msg=
-00026c20: 6627 7b76 6964 656f 5f70 6174 687d 2069  f'{video_path} i
-00026c30: 7320 6e6f 7420 6120 7661 6c69 6420 6669  s not a valid fi
-00026c40: 6c65 2070 6174 6820 6f72 2061 2076 616c  le path or a val
-00026c50: 6964 2064 6972 6563 746f 7279 2070 6174  id directory pat
-00026c60: 6827 2c0a 2020 2020 2020 2020 2020 2020  h',.            
-00026c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c80: 2020 2020 736f 7572 6365 3d69 6e73 6574      source=inset
-00026c90: 5f6f 7665 726c 6179 5f76 6964 656f 2e5f  _overlay_video._
-00026ca0: 5f6e 616d 655f 5f29 0a20 2020 2069 6620  _name__).    if 
-00026cb0: 7361 7665 5f64 6972 2069 7320 6e6f 7420  save_dir is not 
-00026cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
-00026cd0: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
-00026ce0: 7328 696e 5f64 6972 3d73 6176 655f 6469  s(in_dir=save_di
-00026cf0: 7229 0a20 2020 2065 6c73 653a 0a20 2020  r).    else:.   
-00026d00: 2020 2020 2073 6176 655f 6469 7220 3d20       save_dir = 
-00026d10: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00026d20: 7669 6465 6f5f 7061 7468 735b 305d 290a  video_paths[0]).
-00026d30: 2020 2020 666f 7220 6669 6c65 5f63 6e74      for file_cnt
-00026d40: 2c20 7669 6465 6f5f 7061 7468 2069 6e20  , video_path in 
-00026d50: 656e 756d 6572 6174 6528 7669 6465 6f5f  enumerate(video_
-00026d60: 7061 7468 7329 3a0a 2020 2020 2020 2020  paths):.        
-00026d70: 5f2c 2076 6964 656f 5f6e 616d 652c 2076  _, video_name, v
-00026d80: 6964 656f 5f65 7874 203d 2067 6574 5f66  ideo_ext = get_f
-00026d90: 6e5f 6578 7428 7669 6465 6f5f 7061 7468  n_ext(video_path
-00026da0: 290a 2020 2020 2020 2020 5f20 3d20 6765  ).        _ = ge
-00026db0: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
-00026dc0: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
-00026dd0: 656f 5f70 6174 6829 0a20 2020 2020 2020  eo_path).       
-00026de0: 2070 7269 6e74 2866 2749 6e73 6572 7469   print(f'Inserti
-00026df0: 6e67 206f 7665 726c 6179 206f 6e74 6f20  ng overlay onto 
-00026e00: 7b76 6964 656f 5f6e 616d 657d 2028 5669  {video_name} (Vi
-00026e10: 6465 6f20 7b66 696c 655f 636e 7420 2b20  deo {file_cnt + 
-00026e20: 317d 2f7b 6c65 6e28 7669 6465 6f5f 7061  1}/{len(video_pa
-00026e30: 7468 7329 7d29 2e2e 2e27 290a 2020 2020  ths)})...').    
-00026e40: 2020 2020 6f75 745f 7061 7468 203d 206f      out_path = o
-00026e50: 732e 7061 7468 2e6a 6f69 6e28 7361 7665  s.path.join(save
-00026e60: 5f64 6972 2c20 6627 7b76 6964 656f 5f6e  _dir, f'{video_n
-00026e70: 616d 657d 5f69 6e73 6574 5f6f 7665 726c  ame}_inset_overl
-00026e80: 6179 7b76 6964 656f 5f65 7874 7d27 290a  ay{video_ext}').
-00026e90: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
-00026ea0: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
-00026eb0: 6966 2070 6f73 6974 696f 6e20 3d3d 2050  if position == P
-00026ec0: 4f53 4954 494f 4e53 5b30 5d3a 0a20 2020  OSITIONS[0]:.   
-00026ed0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
-00026ee0: 2766 666d 7065 6720 2d69 2022 7b76 6964  'ffmpeg -i "{vid
-00026ef0: 656f 5f70 6174 687d 2220 2d69 2022 7b6f  eo_path}" -i "{o
-00026f00: 7665 726c 6179 5f76 6964 656f 5f70 6174  verlay_video_pat
-00026f10: 687d 2220 2d66 696c 7465 725f 636f 6d70  h}" -filter_comp
-00026f20: 6c65 7820 225b 313a 765d 7363 616c 653d  lex "[1:v]scale=
-00026f30: 6977 2a7b 7363 616c 657d 3a2d 312c 666f  iw*{scale}:-1,fo
-00026f40: 726d 6174 3d72 6762 612c 636f 6c6f 7263  rmat=rgba,colorc
-00026f50: 6861 6e6e 656c 6d69 7865 723d 6161 3d7b  hannelmixer=aa={
-00026f60: 6f70 6163 6974 797d 5b69 6e73 6574 5d3b  opacity}[inset];
-00026f70: 5b30 3a76 5d5b 696e 7365 745d 6f76 6572  [0:v][inset]over
-00026f80: 6c61 793d 303a 3022 2022 7b6f 7574 5f70  lay=0:0" "{out_p
-00026f90: 6174 687d 2220 2d79 270a 2020 2020 2020  ath}" -y'.      
-00026fa0: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
-00026fb0: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
-00026fc0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00026fd0: 203d 2066 2766 666d 7065 6720 2d69 2022   = f'ffmpeg -i "
-00026fe0: 7b76 6964 656f 5f70 6174 687d 2220 2d69  {video_path}" -i
-00026ff0: 2022 7b6f 7665 726c 6179 5f76 6964 656f   "{overlay_video
-00027000: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
-00027010: 636f 6d70 6c65 7820 225b 313a 765d 7363  complex "[1:v]sc
-00027020: 616c 653d 6977 2a7b 7363 616c 657d 3a2d  ale=iw*{scale}:-
-00027030: 312c 666f 726d 6174 3d72 6762 612c 636f  1,format=rgba,co
-00027040: 6c6f 7263 6861 6e6e 656c 6d69 7865 723d  lorchannelmixer=
-00027050: 6161 3d7b 6f70 6163 6974 797d 5b69 6e73  aa={opacity}[ins
-00027060: 6574 5d3b 5b30 3a76 5d5b 696e 7365 745d  et];[0:v][inset]
-00027070: 6f76 6572 6c61 793d 572d 773a 482d 6822  overlay=W-w:H-h"
-00027080: 2022 7b6f 7574 5f70 6174 687d 2220 2d79   "{out_path}" -y
-00027090: 270a 2020 2020 2020 2020 656c 6966 2070  '.        elif p
-000270a0: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
-000270b0: 494f 4e53 5b32 5d3a 0a20 2020 2020 2020  IONS[2]:.       
-000270c0: 2020 2020 2063 6d64 203d 2066 2766 666d       cmd = f'ffm
-000270d0: 7065 6720 2d69 2022 7b76 6964 656f 5f70  peg -i "{video_p
-000270e0: 6174 687d 2220 2d69 2022 7b6f 7665 726c  ath}" -i "{overl
-000270f0: 6179 5f76 6964 656f 5f70 6174 687d 2220  ay_video_path}" 
-00027100: 2d66 696c 7465 725f 636f 6d70 6c65 7820  -filter_complex 
-00027110: 225b 313a 765d 7363 616c 653d 6977 2a7b  "[1:v]scale=iw*{
-00027120: 7363 616c 657d 3a2d 312c 666f 726d 6174  scale}:-1,format
-00027130: 3d72 6762 612c 636f 6c6f 7263 6861 6e6e  =rgba,colorchann
-00027140: 656c 6d69 7865 723d 6161 3d7b 6f70 6163  elmixer=aa={opac
-00027150: 6974 797d 5b69 6e73 6574 5d3b 5b30 3a76  ity}[inset];[0:v
-00027160: 5d5b 696e 7365 745d 6f76 6572 6c61 793d  ][inset]overlay=
-00027170: 572d 773a 3022 2022 7b6f 7574 5f70 6174  W-w:0" "{out_pat
-00027180: 687d 2220 2d79 270a 2020 2020 2020 2020  h}" -y'.        
-00027190: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
-000271a0: 2050 4f53 4954 494f 4e53 5b33 5d3a 0a20   POSITIONS[3]:. 
-000271b0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-000271c0: 2066 2766 666d 7065 6720 2d69 2022 7b76   f'ffmpeg -i "{v
-000271d0: 6964 656f 5f70 6174 687d 2220 2d69 2022  ideo_path}" -i "
-000271e0: 7b6f 7665 726c 6179 5f76 6964 656f 5f70  {overlay_video_p
-000271f0: 6174 687d 2220 2d66 696c 7465 725f 636f  ath}" -filter_co
-00027200: 6d70 6c65 7820 225b 313a 765d 7363 616c  mplex "[1:v]scal
-00027210: 653d 6977 2a7b 7363 616c 657d 3a2d 312c  e=iw*{scale}:-1,
-00027220: 666f 726d 6174 3d72 6762 612c 636f 6c6f  format=rgba,colo
-00027230: 7263 6861 6e6e 656c 6d69 7865 723d 6161  rchannelmixer=aa
-00027240: 3d7b 6f70 6163 6974 797d 5b69 6e73 6574  ={opacity}[inset
-00027250: 5d3b 5b30 3a76 5d5b 696e 7365 745d 6f76  ];[0:v][inset]ov
-00027260: 6572 6c61 793d 303a 482d 6822 2022 7b6f  erlay=0:H-h" "{o
-00027270: 7574 5f70 6174 687d 2220 2d79 270a 2020  ut_path}" -y'.  
-00027280: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00027290: 2020 2020 2020 2020 636d 6420 3d20 6627          cmd = f'
-000272a0: 6666 6d70 6567 202d 6920 227b 7669 6465  ffmpeg -i "{vide
-000272b0: 6f5f 7061 7468 7d22 202d 6920 227b 6f76  o_path}" -i "{ov
-000272c0: 6572 6c61 795f 7669 6465 6f5f 7061 7468  erlay_video_path
-000272d0: 7d22 202d 6669 6c74 6572 5f63 6f6d 706c  }" -filter_compl
-000272e0: 6578 2022 5b31 3a76 5d73 6361 6c65 3d69  ex "[1:v]scale=i
-000272f0: 772a 7b73 6361 6c65 7d3a 2d31 2c66 6f72  w*{scale}:-1,for
-00027300: 6d61 743d 7267 6261 2c63 6f6c 6f72 6368  mat=rgba,colorch
-00027310: 616e 6e65 6c6d 6978 6572 3d61 613d 7b6f  annelmixer=aa={o
-00027320: 7061 6369 7479 7d5b 696e 7365 745d 3b5b  pacity}[inset];[
-00027330: 303a 765d 5b69 6e73 6574 5d6f 7665 726c  0:v][inset]overl
-00027340: 6179 3d28 572d 7729 2f32 3a28 482d 6829  ay=(W-w)/2:(H-h)
-00027350: 2f32 2220 227b 6f75 745f 7061 7468 7d22  /2" "{out_path}"
-00027360: 202d 7927 0a20 2020 2020 2020 2073 7562   -y'.        sub
-00027370: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
-00027380: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
-00027390: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
-000273a0: 5049 5045 290a 2020 2020 7469 6d65 722e  PIPE).    timer.
-000273b0: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
-000273c0: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
-000273d0: 6d73 673d 6627 7b6c 656e 2876 6964 656f  msg=f'{len(video
-000273e0: 5f70 6174 6873 297d 206f 7665 726c 6179  _paths)} overlay
-000273f0: 2076 6964 656f 2873 2920 7361 7665 6420   video(s) saved 
-00027400: 696e 207b 7361 7665 5f64 6972 7d27 2c20  in {save_dir}', 
-00027410: 656c 6170 7365 645f 7469 6d65 3d74 696d  elapsed_time=tim
-00027420: 6572 2e65 6c61 7073 6564 5f74 696d 655f  er.elapsed_time_
-00027430: 7374 7229 0a0a 6465 6620 726f 695f 626c  str)..def roi_bl
-00027440: 7572 626f 7828 7669 6465 6f5f 7061 7468  urbox(video_path
-00027450: 3a20 556e 696f 6e5b 7374 722c 206f 732e  : Union[str, os.
-00027460: 5061 7468 4c69 6b65 5d2c 0a20 2020 2020  PathLike],.     
-00027470: 2020 2020 2020 2020 2020 2062 6c75 725f             blur_
-00027480: 6c65 7665 6c3a 204f 7074 696f 6e61 6c5b  level: Optional[
-00027490: 666c 6f61 745d 203d 2030 2e30 322c 0a20  float] = 0.02,. 
-000274a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000274b0: 6e76 6572 743a 204f 7074 696f 6e61 6c5b  nvert: Optional[
-000274c0: 626f 6f6c 5d20 3d20 4661 6c73 652c 0a20  bool] = False,. 
-000274d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000274e0: 6176 655f 7061 7468 3a20 4f70 7469 6f6e  ave_path: Option
-000274f0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
-00027500: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
-00027510: 6e65 2920 2d3e 204e 6f6e 653a 0a0a 2020  ne) -> None:..  
-00027520: 2020 2222 220a 2020 2020 426c 7572 7320    """.    Blurs 
-00027530: 6569 7468 6572 2074 6865 2073 656c 6563  either the selec
-00027540: 7465 6420 6f72 2075 6e73 656c 6563 7465  ted or unselecte
-00027550: 6420 706f 7274 696f 6e20 6f66 2061 2075  d portion of a u
-00027560: 7365 722d 7370 6563 6966 6965 6420 7265  ser-specified re
-00027570: 6769 6f6e 2d6f 662d 696e 7465 7265 7374  gion-of-interest
-00027580: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
-00027590: 6520 7061 7373 6564 2062 6c75 7220 6c65  e passed blur le
-000275a0: 7665 6c2e 0a20 2020 2048 6967 6865 7220  vel..    Higher 
-000275b0: 626c 7572 206c 6576 656c 7320 7072 6f64  blur levels prod
-000275c0: 7563 6573 206d 6f72 6520 6f70 6171 7565  uces more opaque
-000275d0: 2072 6567 696f 6e73 2e0a 0a20 2020 202e   regions...    .
-000275e0: 2e20 7669 6465 6f3a 3a20 5f73 7461 7469  . video:: _stati
-000275f0: 632f 696d 672f 726f 695f 626c 7572 626f  c/img/roi_blurbo
-00027600: 782e 7765 626d 0a20 2020 2020 2020 3a6c  x.webm.       :l
-00027610: 6f6f 703a 0a0a 2020 2020 3a70 6172 616d  oop:..    :param
-00027620: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-00027630: 6174 684c 696b 655d 2076 6964 656f 5f70  athLike] video_p
-00027640: 6174 683a 2054 6865 2070 6174 6820 746f  ath: The path to
-00027650: 2074 6865 2076 6964 656f 206f 6e20 6469   the video on di
-00027660: 736b 0a20 2020 203a 7061 7261 6d20 4f70  sk.    :param Op
-00027670: 7469 6f6e 616c 5b66 6c6f 6174 5d20 626c  tional[float] bl
-00027680: 7572 5f6c 6576 656c 3a20 5468 6520 6c65  ur_level: The le
-00027690: 7665 6c20 6f66 2074 6865 2062 6c75 7220  vel of the blur 
-000276a0: 6173 2061 2072 6174 696f 2030 2d31 2e30  as a ratio 0-1.0
-000276b0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-000276c0: 696f 6e61 6c5b 626f 6f6c 5d20 696e 7665  ional[bool] inve
-000276d0: 7274 3a20 4966 2054 7275 652c 2062 6c75  rt: If True, blu
-000276e0: 7273 2074 6865 2075 6e73 656c 6563 7465  rs the unselecte
-000276f0: 6420 7265 6769 6f6e 2e20 4966 2046 616c  d region. If Fal
-00027700: 7365 2c20 626c 7572 7320 7468 6520 7365  se, blurs the se
-00027710: 6c65 6374 6564 2072 6567 696f 6e2e 0a20  lected region.. 
-00027720: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
-00027730: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
-00027740: 2e50 6174 684c 696b 655d 5d20 7361 7665  .PathLike]] save
-00027750: 5f70 6174 683a 2054 6865 206c 6f63 6174  _path: The locat
-00027760: 696f 6e20 7768 6572 6520 746f 2073 6176  ion where to sav
-00027770: 6520 7468 6520 626c 7572 7265 6420 7669  e the blurred vi
-00027780: 6465 6f2e 2049 6620 4e6f 6e65 2c20 7468  deo. If None, th
-00027790: 656e 2073 6176 6573 2074 6865 2062 6c75  en saves the blu
-000277a0: 7272 6564 2076 6964 656f 2069 6e20 7468  rred video in th
-000277b0: 6520 7361 6d65 2064 6972 6563 746f 7279  e same directory
-000277c0: 2061 7320 7468 6520 696e 7075 7420 7669   as the input vi
-000277d0: 6465 6f20 7769 7468 2074 6865 2060 605f  deo with the ``_
-000277e0: 626c 7572 7265 6460 6020 7375 6666 6978  blurred`` suffix
-000277f0: 2e0a 2020 2020 3a72 6574 7572 6e3a 204e  ..    :return: N
-00027800: 6f6e 650a 0a20 2020 203a 6578 616d 706c  one..    :exampl
-00027810: 653a 0a20 2020 203e 3e3e 2072 6f69 5f62  e:.    >>> roi_b
-00027820: 6c75 7262 6f78 2876 6964 656f 5f70 6174  lurbox(video_pat
-00027830: 683d 272f 5573 6572 732f 7369 6d6f 6e2f  h='/Users/simon/
-00027840: 446f 776e 6c6f 6164 732f 315f 4c48 5f63  Downloads/1_LH_c
-00027850: 6c69 7070 6564 5f64 6f77 6e73 616d 706c  lipped_downsampl
-00027860: 6564 2e6d 7034 272c 2062 6c75 725f 6c65  ed.mp4', blur_le
-00027870: 7665 6c3d 302e 322c 2069 6e76 6572 743d  vel=0.2, invert=
-00027880: 5472 7565 290a 2020 2020 2222 220a 0a20  True).    """.. 
-00027890: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
-000278a0: 6176 6169 6c61 626c 6528 7261 6973 655f  available(raise_
-000278b0: 6572 726f 723d 5472 7565 290a 2020 2020  error=True).    
-000278c0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
-000278d0: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
-000278e0: 2020 2063 6865 636b 5f66 6c6f 6174 286e     check_float(n
-000278f0: 616d 653d 6627 7b72 6f69 5f62 6c75 7262  ame=f'{roi_blurb
-00027900: 6f78 2e5f 5f6e 616d 655f 5f7d 2062 6c75  ox.__name__} blu
-00027910: 725f 6c65 7665 6c27 2c20 7661 6c75 653d  r_level', value=
-00027920: 626c 7572 5f6c 6576 656c 2c20 6d69 6e5f  blur_level, min_
-00027930: 7661 6c75 653d 302e 3030 312c 206d 6178  value=0.001, max
-00027940: 5f76 616c 7565 3d31 2e30 290a 2020 2020  _value=1.0).    
-00027950: 6368 6563 6b5f 6669 6c65 5f65 7869 7374  check_file_exist
-00027960: 5f61 6e64 5f72 6561 6461 626c 6528 6669  _and_readable(fi
-00027970: 6c65 5f70 6174 683d 7669 6465 6f5f 7061  le_path=video_pa
-00027980: 7468 290a 2020 2020 6469 722c 2076 6964  th).    dir, vid
-00027990: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
-000279a0: 6574 5f66 6e5f 6578 7428 7669 6465 6f5f  et_fn_ext(video_
-000279b0: 7061 7468 290a 2020 2020 5f20 3d20 6765  path).    _ = ge
-000279c0: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
-000279d0: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
-000279e0: 656f 5f70 6174 6829 0a20 2020 2069 6620  eo_path).    if 
-000279f0: 7361 7665 5f70 6174 6820 6973 206e 6f74  save_path is not
-00027a00: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
-00027a10: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
-00027a20: 7473 2869 6e5f 6469 723d 6f73 2e70 6174  ts(in_dir=os.pat
-00027a30: 682e 6469 726e 616d 6528 7361 7665 5f70  h.dirname(save_p
-00027a40: 6174 6829 2c20 736f 7572 6365 3d72 6f69  ath), source=roi
-00027a50: 5f62 6c75 7262 6f78 2e5f 5f6e 616d 655f  _blurbox.__name_
-00027a60: 5f29 0a20 2020 2065 6c73 653a 0a20 2020  _).    else:.   
-00027a70: 2020 2020 2073 6176 655f 7061 7468 203d       save_path =
-00027a80: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
-00027a90: 722c 2066 277b 7669 6465 6f5f 6e61 6d65  r, f'{video_name
-00027aa0: 7d5f 626c 7572 7265 647b 6578 747d 2729  }_blurred{ext}')
-00027ab0: 0a20 2020 2072 6f69 5f73 656c 6563 746f  .    roi_selecto
-00027ac0: 7220 3d20 524f 4953 656c 6563 746f 7228  r = ROISelector(
-00027ad0: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
-00027ae0: 0a20 2020 2072 6f69 5f73 656c 6563 746f  .    roi_selecto
-00027af0: 722e 7275 6e28 290a 2020 2020 772c 2068  r.run().    w, h
-00027b00: 203d 2072 6f69 5f73 656c 6563 746f 722e   = roi_selector.
-00027b10: 7769 6474 682c 2072 6f69 5f73 656c 6563  width, roi_selec
-00027b20: 746f 722e 6865 6967 6874 0a20 2020 2074  tor.height.    t
-00027b30: 6f70 5f6c 6566 745f 782c 2074 6f70 5f6c  op_left_x, top_l
-00027b40: 6566 745f 7920 3d20 726f 695f 7365 6c65  eft_y = roi_sele
-00027b50: 6374 6f72 2e74 6f70 5f6c 6566 740a 2020  ctor.top_left.  
-00027b60: 2020 6d61 785f 626c 7572 5f76 616c 7565    max_blur_value
-00027b70: 203d 2069 6e74 286d 696e 2877 2c20 6829   = int(min(w, h)
-00027b80: 202f 2032 2920 2f20 320a 2020 2020 626c   / 2) / 2.    bl
-00027b90: 7572 5f6c 6576 656c 203d 2069 6e74 286d  ur_level = int(m
-00027ba0: 6178 5f62 6c75 725f 7661 6c75 6520 2a20  ax_blur_value * 
-00027bb0: 626c 7572 5f6c 6576 656c 290a 2020 2020  blur_level).    
-00027bc0: 6966 206e 6f74 2069 6e76 6572 743a 0a20  if not invert:. 
-00027bd0: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
-00027be0: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
-00027bf0: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
-00027c00: 636f 6d70 6c65 7820 225b 303a 765d 6372  complex "[0:v]cr
-00027c10: 6f70 3d7b 777d 3a7b 687d 3a7b 746f 705f  op={w}:{h}:{top_
-00027c20: 6c65 6674 5f78 7d3a 7b74 6f70 5f6c 6566  left_x}:{top_lef
-00027c30: 745f 797d 2c62 6f78 626c 7572 3d7b 696e  t_y},boxblur={in
-00027c40: 7428 626c 7572 5f6c 6576 656c 297d 3a31  t(blur_level)}:1
-00027c50: 305b 6667 5d3b 205b 303a 765d 5b66 675d  0[fg]; [0:v][fg]
-00027c60: 6f76 6572 6c61 793d 7b74 6f70 5f6c 6566  overlay={top_lef
-00027c70: 745f 787d 3a7b 746f 705f 6c65 6674 5f79  t_x}:{top_left_y
-00027c80: 7d5b 765d 2220 2d6d 6170 2022 5b76 5d22  }[v]" -map "[v]"
-00027c90: 2022 7b73 6176 655f 7061 7468 7d22 202d   "{save_path}" -
-00027ca0: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-00027cb0: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-00027cc0: 6572 202d 7927 0a20 2020 2065 6c73 653a  er -y'.    else:
-00027cd0: 0a20 2020 2020 2020 2063 6d64 203d 2066  .        cmd = f
-00027ce0: 2766 666d 7065 6720 2d69 2022 7b76 6964  'ffmpeg -i "{vid
-00027cf0: 656f 5f70 6174 687d 2220 2d66 696c 7465  eo_path}" -filte
-00027d00: 725f 636f 6d70 6c65 7820 225b 303a 765d  r_complex "[0:v]
-00027d10: 626f 7862 6c75 723d 7b62 6c75 725f 6c65  boxblur={blur_le
-00027d20: 7665 6c7d 5b62 675d 3b5b 303a 765d 6372  vel}[bg];[0:v]cr
-00027d30: 6f70 3d7b 777d 3a7b 687d 3a7b 746f 705f  op={w}:{h}:{top_
-00027d40: 6c65 6674 5f78 7d3a 7b74 6f70 5f6c 6566  left_x}:{top_lef
-00027d50: 745f 797d 5b66 675d 3b5b 6267 5d5b 6667  t_y}[fg];[bg][fg
-00027d60: 5d6f 7665 726c 6179 3d7b 746f 705f 6c65  ]overlay={top_le
-00027d70: 6674 5f78 7d3a 7b74 6f70 5f6c 6566 745f  ft_x}:{top_left_
-00027d80: 797d 2220 2d63 3a61 2063 6f70 7920 227b  y}" -c:a copy "{
-00027d90: 7361 7665 5f70 6174 687d 2220 2d6c 6f67  save_path}" -log
-00027da0: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
-00027db0: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
-00027dc0: 2d79 270a 2020 2020 7375 6270 726f 6365  -y'.    subproce
-00027dd0: 7373 2e63 616c 6c28 636d 642c 2073 6865  ss.call(cmd, she
-00027de0: 6c6c 3d54 7275 652c 2073 7464 6f75 743d  ll=True, stdout=
-00027df0: 7375 6270 726f 6365 7373 2e50 4950 4529  subprocess.PIPE)
-00027e00: 0a20 2020 2074 696d 6572 2e73 746f 705f  .    timer.stop_
-00027e10: 7469 6d65 7228 290a 2020 2020 7374 646f  timer().    stdo
-00027e20: 7574 5f73 7563 6365 7373 286d 7367 3d66  ut_success(msg=f
-00027e30: 2742 6c75 7272 6564 207b 7669 6465 6f5f  'Blurred {video_
-00027e40: 6e61 6d65 7d20 7669 6465 6f20 7361 7665  name} video save
-00027e50: 6420 696e 207b 7361 7665 5f70 6174 687d  d in {save_path}
-00027e60: 272c 2065 6c61 7073 6564 5f74 696d 653d  ', elapsed_time=
-00027e70: 7469 6d65 722e 656c 6170 7365 645f 7469  timer.elapsed_ti
-00027e80: 6d65 5f73 7472 290a 0a0a 6465 6620 7375  me_str)...def su
-00027e90: 7065 7269 6d70 6f73 655f 656c 6170 7365  perimpose_elapse
-00027ea0: 645f 7469 6d65 2876 6964 656f 5f70 6174  d_time(video_pat
-00027eb0: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
-00027ec0: 2e50 6174 684c 696b 655d 2c0a 2020 2020  .PathLike],.    
-00027ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ee0: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
-00027ef0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
-00027f00: 5d20 3d20 3330 2c0a 2020 2020 2020 2020  ] = 30,.        
-00027f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f20: 2020 2020 2066 6f6e 745f 636f 6c6f 723a       font_color:
-00027f30: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00027f40: 2027 7768 6974 6527 2c0a 2020 2020 2020   'white',.      
-00027f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f60: 2020 2020 2020 2066 6f6e 745f 626f 7264         font_bord
-00027f70: 6572 5f63 6f6c 6f72 3a20 4f70 7469 6f6e  er_color: Option
-00027f80: 616c 5b73 7472 5d20 3d20 2762 6c61 636b  al[str] = 'black
-00027f90: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00027fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fb0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
-00027fc0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-00027fd0: 203d 2032 2c0a 2020 2020 2020 2020 2020   = 2,.          
-00027fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027ff0: 2020 2070 6f73 6974 696f 6e3a 204f 7074     position: Opt
-00028000: 696f 6e61 6c5b 4c69 7465 7261 6c5b 2774  ional[Literal['t
-00028010: 6f70 5f6c 6566 7427 2c20 2774 6f70 5f72  op_left', 'top_r
-00028020: 6967 6874 272c 2027 626f 7474 6f6d 5f6c  ight', 'bottom_l
-00028030: 6566 7427 2c20 2762 6f74 746f 6d5f 7269  eft', 'bottom_ri
-00028040: 6768 7427 2c20 276d 6964 646c 655f 746f  ght', 'middle_to
-00028050: 7027 2c20 276d 6964 646c 655f 626f 7474  p', 'middle_bott
-00028060: 6f6d 275d 5d20 3d20 2774 6f70 5f6c 6566  om']] = 'top_lef
-00028070: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-00028080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028090: 2073 6176 655f 6469 723a 204f 7074 696f   save_dir: Optio
-000280a0: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
-000280b0: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
-000280c0: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
-000280d0: 2020 2222 220a 2020 2020 5375 7065 7269    """.    Superi
-000280e0: 6d70 6f73 6573 2065 6c61 7073 6564 2074  mposes elapsed t
-000280f0: 696d 6520 6f6e 2074 6865 2067 6976 656e  ime on the given
-00028100: 2076 6964 656f 2066 696c 6528 7329 2061   video file(s) a
-00028110: 6e64 2073 6176 6573 2074 6865 206d 6f64  nd saves the mod
-00028120: 6966 6965 6420 7669 6465 6f28 7329 2e0a  ified video(s)..
-00028130: 0a20 2020 202e 2e20 7669 6465 6f3a 3a20  .    .. video:: 
-00028140: 5f73 7461 7469 632f 696d 672f 7375 7065  _static/img/supe
-00028150: 7269 6d70 6f73 655f 656c 6170 7365 645f  rimpose_elapsed_
-00028160: 7469 6d65 2e77 6562 6d0a 2020 2020 2020  time.webm.      
-00028170: 203a 7769 6474 683a 2039 3030 0a20 2020   :width: 900.   
-00028180: 2020 2020 3a6c 6f6f 703a 0a0a 2020 2020      :loop:..    
-00028190: 3a70 6172 616d 2055 6e69 6f6e 5b73 7472  :param Union[str
-000281a0: 2c20 6f73 2e50 6174 684c 696b 655d 2076  , os.PathLike] v
-000281b0: 6964 656f 5f70 6174 683a 2050 6174 6820  ideo_path: Path 
-000281c0: 746f 2074 6865 2069 6e70 7574 2076 6964  to the input vid
-000281d0: 656f 2066 696c 6520 6f72 2064 6972 6563  eo file or direc
-000281e0: 746f 7279 2063 6f6e 7461 696e 696e 6720  tory containing 
-000281f0: 7669 6465 6f20 6669 6c65 732e 0a20 2020  video files..   
-00028200: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-00028210: 5b69 6e74 5d20 666f 6e74 5f73 697a 653a  [int] font_size:
-00028220: 2046 6f6e 7420 7369 7a65 2066 6f72 2074   Font size for t
-00028230: 6865 2065 6c61 7073 6564 2074 696d 6520  he elapsed time 
-00028240: 7465 7874 2e20 4465 6661 756c 7420 3330  text. Default 30
-00028250: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00028260: 696f 6e61 6c5b 7374 725d 2066 6f6e 745f  ional[str] font_
-00028270: 636f 6c6f 723a 2020 466f 6e74 2063 6f6c  color:  Font col
-00028280: 6f72 2066 6f72 2074 6865 2065 6c61 7073  or for the elaps
-00028290: 6564 2074 696d 6520 7465 7874 2e20 4465  ed time text. De
-000282a0: 6661 756c 7420 7768 6974 650a 2020 2020  fault white.    
-000282b0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-000282c0: 7374 725d 2066 6f6e 745f 626f 7264 6572  str] font_border
-000282d0: 5f63 6f6c 6f72 3a20 466f 6e74 2062 6f72  _color: Font bor
-000282e0: 6465 7220 636f 6c6f 7220 666f 7220 7468  der color for th
-000282f0: 6520 656c 6170 7365 6420 7469 6d65 2074  e elapsed time t
-00028300: 6578 742e 2044 6566 6175 6c74 2062 6c61  ext. Default bla
-00028310: 636b 2e0a 2020 2020 3a70 6172 616d 204f  ck..    :param O
-00028320: 7074 696f 6e61 6c5b 696e 745d 2066 6f6e  ptional[int] fon
-00028330: 745f 626f 7264 6572 5f77 6964 7468 3a20  t_border_width: 
-00028340: 466f 6e74 2062 6f72 6465 7220 7769 6474  Font border widt
-00028350: 6820 666f 7220 7468 6520 656c 6170 7365  h for the elapse
-00028360: 6420 7469 6d65 2074 6578 7420 696e 2070  d time text in p
-00028370: 6978 656c 732e 2044 6566 6175 6c74 2032  ixels. Default 2
-00028380: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00028390: 696f 6e61 6c5b 4c69 7465 7261 6c5b 2774  ional[Literal['t
-000283a0: 6f70 5f6c 6566 7427 2c20 2774 6f70 5f72  op_left', 'top_r
-000283b0: 6967 6874 272c 2027 626f 7474 6f6d 5f6c  ight', 'bottom_l
-000283c0: 6566 7427 2c20 2762 6f74 746f 6d5f 7269  eft', 'bottom_ri
-000283d0: 6768 7427 2c20 276d 6964 646c 655f 746f  ght', 'middle_to
-000283e0: 7027 2c20 276d 6964 646c 655f 626f 7474  p', 'middle_bott
-000283f0: 6f6d 275d 5d20 706f 7369 7469 6f6e 3a20  om']] position: 
-00028400: 506f 7369 7469 6f6e 2077 6865 7265 2074  Position where t
-00028410: 6865 2065 6c61 7073 6564 2074 696d 6520  he elapsed time 
-00028420: 7465 7874 2077 696c 6c20 6265 2073 7570  text will be sup
-00028430: 6572 696d 706f 7365 642e 2044 6566 6175  erimposed. Defau
-00028440: 6c74 2060 6074 6f70 5f6c 6566 7460 602e  lt ``top_left``.
-00028450: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-00028460: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-00028470: 6f73 2e50 6174 684c 696b 655d 5d20 7361  os.PathLike]] sa
-00028480: 7665 5f64 6972 3a20 4469 7265 6374 6f72  ve_dir: Director
-00028490: 7920 7768 6572 6520 7468 6520 6d6f 6469  y where the modi
-000284a0: 6669 6564 2076 6964 656f 2873 2920 7769  fied video(s) wi
-000284b0: 6c6c 2062 6520 7361 7665 642e 2049 6620  ll be saved. If 
-000284c0: 6e6f 7420 7072 6f76 6964 6564 2c20 7468  not provided, th
-000284d0: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
-000284e0: 6865 2069 6e70 7574 2076 6964 656f 2873  he input video(s
-000284f0: 2920 7769 6c6c 2062 6520 7573 6564 2e0a  ) will be used..
-00028500: 2020 2020 3a72 6574 7572 6e3a 204e 6f6e      :return: Non
-00028510: 650a 0a20 2020 203a 6578 616d 706c 653a  e..    :example:
-00028520: 0a20 2020 203e 3e3e 2073 7570 6572 696d  .    >>> superim
-00028530: 706f 7365 5f65 6c61 7073 6564 5f74 696d  pose_elapsed_tim
-00028540: 6528 7669 6465 6f5f 7061 7468 3d27 2f55  e(video_path='/U
-00028550: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-00028560: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-00028570: 6f75 626c 6573 686f 6f74 696e 672f 6d6f  oubleshooting/mo
-00028580: 7573 655f 6f70 656e 5f66 6965 6c64 2f70  use_open_field/p
-00028590: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-000285a0: 6465 6f73 2f74 6573 745f 342f 312e 6d70  deos/test_4/1.mp
-000285b0: 3427 2c20 706f 7369 7469 6f6e 3d27 6d69  4', position='mi
-000285c0: 6464 6c65 5f74 6f70 272c 2066 6f6e 745f  ddle_top', font_
-000285d0: 636f 6c6f 723d 2762 6c61 636b 272c 2066  color='black', f
-000285e0: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-000285f0: 3d27 7069 6e6b 272c 2066 6f6e 745f 626f  ='pink', font_bo
-00028600: 7264 6572 5f77 6964 7468 3d35 2c20 666f  rder_width=5, fo
-00028610: 6e74 5f73 697a 653d 3330 290a 2020 2020  nt_size=30).    
-00028620: 2222 220a 0a20 2020 2063 6865 636b 5f66  """..    check_f
-00028630: 666d 7065 675f 6176 6169 6c61 626c 6528  fmpeg_available(
-00028640: 7261 6973 655f 6572 726f 723d 5472 7565  raise_error=True
-00028650: 290a 2020 2020 7469 6d65 7220 3d20 5369  ).    timer = Si
-00028660: 6d62 6154 696d 6572 2873 7461 7274 3d54  mbaTimer(start=T
-00028670: 7275 6529 0a20 2020 2050 4f53 4954 494f  rue).    POSITIO
-00028680: 4e53 203d 205b 2774 6f70 5f6c 6566 7427  NS = ['top_left'
-00028690: 2c20 2774 6f70 5f72 6967 6874 272c 2027  , 'top_right', '
-000286a0: 626f 7474 6f6d 5f6c 6566 7427 2c20 2762  bottom_left', 'b
-000286b0: 6f74 746f 6d5f 7269 6768 7427 2c20 2774  ottom_right', 't
-000286c0: 6f70 5f6d 6964 646c 6527 2c20 2762 6f74  op_middle', 'bot
-000286d0: 746f 6d5f 6d69 6464 6c65 275d 0a20 2020  tom_middle'].   
-000286e0: 2063 6865 636b 5f73 7472 286e 616d 653d   check_str(name=
-000286f0: 6627 7b73 7570 6572 696d 706f 7365 5f65  f'{superimpose_e
-00028700: 6c61 7073 6564 5f74 696d 652e 5f5f 6e61  lapsed_time.__na
-00028710: 6d65 5f5f 7d20 706f 7369 7469 6f6e 272c  me__} position',
-00028720: 2076 616c 7565 3d70 6f73 6974 696f 6e2c   value=position,
-00028730: 206f 7074 696f 6e73 3d50 4f53 4954 494f   options=POSITIO
-00028740: 4e53 290a 2020 2020 6368 6563 6b5f 696e  NS).    check_in
-00028750: 7428 6e61 6d65 3d66 277b 7375 7065 7269  t(name=f'{superi
-00028760: 6d70 6f73 655f 656c 6170 7365 645f 7469  mpose_elapsed_ti
-00028770: 6d65 2e5f 5f6e 616d 655f 5f7d 2066 6f6e  me.__name__} fon
-00028780: 745f 7369 7a65 272c 2076 616c 7565 3d66  t_size', value=f
-00028790: 6f6e 745f 7369 7a65 2c20 6d69 6e5f 7661  ont_size, min_va
-000287a0: 6c75 653d 3129 0a20 2020 2063 6865 636b  lue=1).    check
-000287b0: 5f69 6e74 286e 616d 653d 6627 7b73 7570  _int(name=f'{sup
-000287c0: 6572 696d 706f 7365 5f65 6c61 7073 6564  erimpose_elapsed
-000287d0: 5f74 696d 652e 5f5f 6e61 6d65 5f5f 7d20  _time.__name__} 
-000287e0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
-000287f0: 6827 2c20 7661 6c75 653d 666f 6e74 5f62  h', value=font_b
-00028800: 6f72 6465 725f 7769 6474 682c 206d 696e  order_width, min
-00028810: 5f76 616c 7565 3d31 290a 2020 2020 666f  _value=1).    fo
-00028820: 6e74 5f63 6f6c 6f72 203d 2027 272e 6a6f  nt_color = ''.jo
-00028830: 696e 2866 696c 7465 7228 7374 722e 6973  in(filter(str.is
-00028840: 616c 6e75 6d2c 2066 6f6e 745f 636f 6c6f  alnum, font_colo
-00028850: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
-00028860: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-00028870: 7220 3d20 2727 2e6a 6f69 6e28 6669 6c74  r = ''.join(filt
-00028880: 6572 2873 7472 2e69 7361 6c6e 756d 2c20  er(str.isalnum, 
-00028890: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-000288a0: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
-000288b0: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
-000288c0: 6528 7669 6465 6f5f 7061 7468 293a 0a20  e(video_path):. 
-000288d0: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
-000288e0: 6873 203d 205b 7669 6465 6f5f 7061 7468  hs = [video_path
-000288f0: 5d0a 2020 2020 656c 6966 206f 732e 7061  ].    elif os.pa
-00028900: 7468 2e69 7364 6972 2876 6964 656f 5f70  th.isdir(video_p
-00028910: 6174 6829 3a0a 2020 2020 2020 2020 7669  ath):.        vi
-00028920: 6465 6f5f 7061 7468 7320 3d20 6c69 7374  deo_paths = list
-00028930: 2866 696e 645f 616c 6c5f 7669 6465 6f73  (find_all_videos
-00028940: 5f69 6e5f 6469 7265 6374 6f72 7928 6469  _in_directory(di
-00028950: 7265 6374 6f72 793d 7669 6465 6f5f 7061  rectory=video_pa
-00028960: 7468 2c20 6173 5f64 6963 743d 5472 7565  th, as_dict=True
-00028970: 2c20 7261 6973 655f 6572 726f 723d 5472  , raise_error=Tr
-00028980: 7565 292e 7661 6c75 6573 2829 290a 2020  ue).values()).  
-00028990: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000289a0: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
-000289b0: 7574 4572 726f 7228 6d73 673d 6627 7b76  utError(msg=f'{v
-000289c0: 6964 656f 5f70 6174 687d 2069 7320 6e6f  ideo_path} is no
-000289d0: 7420 6120 7661 6c69 6420 6669 6c65 2070  t a valid file p
-000289e0: 6174 6820 6f72 2061 2076 616c 6964 2064  ath or a valid d
-000289f0: 6972 6563 746f 7279 2070 6174 6827 2c0a  irectory path',.
-00028a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028a20: 736f 7572 6365 3d73 7570 6572 696d 706f  source=superimpo
-00028a30: 7365 5f65 6c61 7073 6564 5f74 696d 652e  se_elapsed_time.
-00028a40: 5f5f 6e61 6d65 5f5f 290a 2020 2020 6966  __name__).    if
-00028a50: 2073 6176 655f 6469 7220 6973 206e 6f74   save_dir is not
-00028a60: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
-00028a70: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
-00028a80: 7473 2869 6e5f 6469 723d 7361 7665 5f64  ts(in_dir=save_d
-00028a90: 6972 290a 2020 2020 656c 7365 3a0a 2020  ir).    else:.  
-00028aa0: 2020 2020 2020 7361 7665 5f64 6972 203d        save_dir =
-00028ab0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-00028ac0: 2876 6964 656f 5f70 6174 6873 5b30 5d29  (video_paths[0])
-00028ad0: 0a20 2020 2066 6f72 2066 696c 655f 636e  .    for file_cn
-00028ae0: 742c 2076 6964 656f 5f70 6174 6820 696e  t, video_path in
-00028af0: 2065 6e75 6d65 7261 7465 2876 6964 656f   enumerate(video
-00028b00: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
-00028b10: 205f 2c20 7669 6465 6f5f 6e61 6d65 2c20   _, video_name, 
-00028b20: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
-00028b30: 2876 6964 656f 5f70 6174 6829 0a20 2020  (video_path).   
-00028b40: 2020 2020 2070 7269 6e74 2866 2753 7570       print(f'Sup
-00028b50: 6572 696d 706f 7369 6e67 2074 696d 6520  erimposing time 
-00028b60: 7b76 6964 656f 5f6e 616d 657d 2028 5669  {video_name} (Vi
-00028b70: 6465 6f20 7b66 696c 655f 636e 7420 2b20  deo {file_cnt + 
-00028b80: 317d 2f7b 6c65 6e28 7669 6465 6f5f 7061  1}/{len(video_pa
-00028b90: 7468 7329 7d29 2e2e 2e27 290a 2020 2020  ths)})...').    
-00028ba0: 2020 2020 7361 7665 5f70 6174 6820 3d20      save_path = 
-00028bb0: 6f73 2e70 6174 682e 6a6f 696e 2873 6176  os.path.join(sav
-00028bc0: 655f 6469 722c 2066 277b 7669 6465 6f5f  e_dir, f'{video_
-00028bd0: 6e61 6d65 7d5f 7469 6d65 5f73 7570 6572  name}_time_super
-00028be0: 696d 706f 7365 647b 6578 747d 2729 0a20  imposed{ext}'). 
-00028bf0: 2020 2020 2020 2069 6620 706f 7369 7469         if positi
-00028c00: 6f6e 203d 3d20 504f 5349 5449 4f4e 535b  on == POSITIONS[
-00028c10: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
-00028c20: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
-00028c30: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
-00028c40: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
-00028c50: 666f 6e74 6669 6c65 3d41 7269 616c 2e74  fontfile=Arial.t
-00028c60: 7466 3a74 6578 743d 2725 7b7b 7074 735c  tf:text='%{{pts\
-00028c70: 3a68 6d73 7d7d 2e25 7b7b 6569 665c 3a6d  :hms}}.%{{eif\:m
-00028c80: 6f64 286e 5c5c 2c31 3030 3029 5c5c 3a64  od(n\\,1000)\\:d
-00028c90: 5c5c 3a33 7d7d 273a 783d 353a 793d 353a  \\:3}}':x=5:y=5:
-00028ca0: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
-00028cb0: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
-00028cc0: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
-00028cd0: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
-00028ce0: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
-00028cf0: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
-00028d00: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
-00028d10: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
-00028d20: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
-00028d30: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
-00028d40: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
-00028d50: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
-00028d60: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
-00028d70: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00028d80: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
-00028d90: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
-00028da0: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
-00028db0: 7466 696c 653d 4172 6961 6c2e 7474 663a  tfile=Arial.ttf:
-00028dc0: 7465 7874 3d27 257b 7b70 7473 5c3a 686d  text='%{{pts\:hm
-00028dd0: 737d 7d2e 257b 7b65 6966 5c3a 6d6f 6428  s}}.%{{eif\:mod(
-00028de0: 6e5c 5c2c 3130 3030 295c 5c3a 645c 5c3a  n\\,1000)\\:d\\:
-00028df0: 337d 7d27 3a78 3d28 772d 7477 2d35 293a  3}}':x=(w-tw-5):
-00028e00: 793d 353a 666f 6e74 7369 7a65 3d7b 666f  y=5:fontsize={fo
-00028e10: 6e74 5f73 697a 657d 3a66 6f6e 7463 6f6c  nt_size}:fontcol
-00028e20: 6f72 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a  or={font_color}:
-00028e30: 626f 7264 6572 773d 7b66 6f6e 745f 626f  borderw={font_bo
-00028e40: 7264 6572 5f77 6964 7468 7d3a 626f 7264  rder_width}:bord
-00028e50: 6572 636f 6c6f 723d 7b66 6f6e 745f 626f  ercolor={font_bo
-00028e60: 7264 6572 5f63 6f6c 6f72 7d5c 2220 2d63  rder_color}\" -c
-00028e70: 3a61 2063 6f70 7920 277b 7361 7665 5f70  :a copy '{save_p
-00028e80: 6174 687d 2720 2d6c 6f67 6c65 7665 6c20  ath}' -loglevel 
-00028e90: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
-00028ea0: 6465 5f62 616e 6e65 7220 2d79 220a 2020  de_banner -y".  
-00028eb0: 2020 2020 2020 656c 6966 2070 6f73 6974        elif posit
-00028ec0: 696f 6e20 3d3d 2050 4f53 4954 494f 4e53  ion == POSITIONS
-00028ed0: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
-00028ee0: 2063 6d64 203d 2066 2266 666d 7065 6720   cmd = f"ffmpeg 
-00028ef0: 2d69 2027 7b76 6964 656f 5f70 6174 687d  -i '{video_path}
-00028f00: 2720 2d76 6620 5c22 6472 6177 7465 7874  ' -vf \"drawtext
-00028f10: 3d66 6f6e 7466 696c 653d 4172 6961 6c2e  =fontfile=Arial.
-00028f20: 7474 663a 7465 7874 3d27 257b 7b70 7473  ttf:text='%{{pts
-00028f30: 5c3a 686d 737d 7d2e 257b 7b65 6966 5c3a  \:hms}}.%{{eif\:
-00028f40: 6d6f 6428 6e5c 5c2c 3130 3030 295c 5c3a  mod(n\\,1000)\\:
-00028f50: 645c 5c3a 337d 7d27 3a78 3d35 3a79 3d28  d\\:3}}':x=5:y=(
-00028f60: 682d 7468 2d35 293a 666f 6e74 7369 7a65  h-th-5):fontsize
-00028f70: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
-00028f80: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
-00028f90: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
-00028fa0: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
-00028fb0: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
-00028fc0: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
-00028fd0: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
-00028fe0: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
-00028ff0: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
-00029000: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
-00029010: 220a 2020 2020 2020 2020 656c 6966 2070  ".        elif p
-00029020: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
-00029030: 494f 4e53 5b33 5d3a 0a20 2020 2020 2020  IONS[3]:.       
-00029040: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
-00029050: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
-00029060: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
-00029070: 7465 7874 3d66 6f6e 7466 696c 653d 4172  text=fontfile=Ar
-00029080: 6961 6c2e 7474 663a 7465 7874 3d27 257b  ial.ttf:text='%{
-00029090: 7b70 7473 5c3a 686d 737d 7d2e 257b 7b65  {pts\:hms}}.%{{e
-000290a0: 6966 5c3a 6d6f 6428 6e5c 5c2c 3130 3030  if\:mod(n\\,1000
-000290b0: 295c 5c3a 645c 5c3a 337d 7d27 3a78 3d28  )\\:d\\:3}}':x=(
-000290c0: 772d 7477 2d35 293a 793d 2868 2d74 682d  w-tw-5):y=(h-th-
-000290d0: 3529 3a66 6f6e 7473 697a 653d 7b66 6f6e  5):fontsize={fon
-000290e0: 745f 7369 7a65 7d3a 666f 6e74 636f 6c6f  t_size}:fontcolo
-000290f0: 723d 7b66 6f6e 745f 636f 6c6f 727d 3a62  r={font_color}:b
-00029100: 6f72 6465 7277 3d7b 666f 6e74 5f62 6f72  orderw={font_bor
-00029110: 6465 725f 7769 6474 687d 3a62 6f72 6465  der_width}:borde
-00029120: 7263 6f6c 6f72 3d7b 666f 6e74 5f62 6f72  rcolor={font_bor
-00029130: 6465 725f 636f 6c6f 727d 5c22 202d 633a  der_color}\" -c:
-00029140: 6120 636f 7079 2027 7b73 6176 655f 7061  a copy '{save_pa
-00029150: 7468 7d27 202d 6c6f 676c 6576 656c 2065  th}' -loglevel e
-00029160: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
-00029170: 655f 6261 6e6e 6572 202d 7922 0a20 2020  e_banner -y".   
-00029180: 2020 2020 2065 6c69 6620 706f 7369 7469       elif positi
-00029190: 6f6e 203d 3d20 504f 5349 5449 4f4e 535b  on == POSITIONS[
-000291a0: 345d 3a0a 2020 2020 2020 2020 2020 2020  4]:.            
-000291b0: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
-000291c0: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
-000291d0: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
-000291e0: 666f 6e74 6669 6c65 3d41 7269 616c 2e74  fontfile=Arial.t
-000291f0: 7466 3a74 6578 743d 2725 7b7b 7074 735c  tf:text='%{{pts\
-00029200: 3a68 6d73 7d7d 2e25 7b7b 6569 665c 3a6d  :hms}}.%{{eif\:m
-00029210: 6f64 286e 5c5c 2c31 3030 3029 5c5c 3a64  od(n\\,1000)\\:d
-00029220: 5c5c 3a33 7d7d 273a 783d 2877 2d74 7729  \\:3}}':x=(w-tw)
-00029230: 2f32 3a79 3d31 303a 666f 6e74 7369 7a65  /2:y=10:fontsize
-00029240: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
-00029250: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
-00029260: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
-00029270: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
-00029280: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
-00029290: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
-000292a0: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
-000292b0: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
-000292c0: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
-000292d0: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
-000292e0: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-000292f0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00029300: 3d20 6622 6666 6d70 6567 202d 6920 277b  = f"ffmpeg -i '{
-00029310: 7669 6465 6f5f 7061 7468 7d27 202d 7666  video_path}' -vf
-00029320: 205c 2264 7261 7774 6578 743d 666f 6e74   \"drawtext=font
-00029330: 6669 6c65 3d41 7269 616c 2e74 7466 3a74  file=Arial.ttf:t
-00029340: 6578 743d 2725 7b7b 7074 735c 3a68 6d73  ext='%{{pts\:hms
-00029350: 7d7d 2e25 7b7b 6569 665c 3a6d 6f64 286e  }}.%{{eif\:mod(n
-00029360: 5c5c 2c31 3030 3029 5c5c 3a64 5c5c 3a33  \\,1000)\\:d\\:3
-00029370: 7d7d 273a 783d 2877 2d74 7729 2f32 3a79  }}':x=(w-tw)/2:y
-00029380: 3d28 682d 7468 2d31 3029 3a66 6f6e 7473  =(h-th-10):fonts
-00029390: 697a 653d 7b66 6f6e 745f 7369 7a65 7d3a  ize={font_size}:
-000293a0: 666f 6e74 636f 6c6f 723d 7b66 6f6e 745f  fontcolor={font_
-000293b0: 636f 6c6f 727d 3a62 6f72 6465 7277 3d7b  color}:borderw={
-000293c0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
-000293d0: 687d 3a62 6f72 6465 7263 6f6c 6f72 3d7b  h}:bordercolor={
-000293e0: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-000293f0: 727d 5c22 202d 633a 6120 636f 7079 2027  r}\" -c:a copy '
-00029400: 7b73 6176 655f 7061 7468 7d27 202d 6c6f  {save_path}' -lo
-00029410: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
-00029420: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
-00029430: 202d 7922 0a20 2020 2020 2020 2073 7562   -y".        sub
-00029440: 7072 6f63 6573 732e 6361 6c6c 2863 6d64  process.call(cmd
-00029450: 2c20 7368 656c 6c3d 5472 7565 2c20 7374  , shell=True, st
-00029460: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
-00029470: 5049 5045 290a 2020 2020 7469 6d65 722e  PIPE).    timer.
-00029480: 7374 6f70 5f74 696d 6572 2829 0a20 2020  stop_timer().   
-00029490: 2073 7464 6f75 745f 7375 6363 6573 7328   stdout_success(
-000294a0: 6d73 673d 6627 5375 7065 722d 696d 706f  msg=f'Super-impo
-000294b0: 7365 6420 7469 6d65 206f 6e20 7b6c 656e  sed time on {len
-000294c0: 2876 6964 656f 5f70 6174 6873 297d 2076  (video_paths)} v
-000294d0: 6964 656f 2873 292c 2073 6176 6564 2069  ideo(s), saved i
-000294e0: 6e20 7b73 6176 655f 6469 727d 272c 2065  n {save_dir}', e
-000294f0: 6c61 7073 6564 5f74 696d 653d 7469 6d65  lapsed_time=time
-00029500: 722e 656c 6170 7365 645f 7469 6d65 5f73  r.elapsed_time_s
-00029510: 7472 290a 0a0a 6465 6620 7669 6465 6f5f  tr)...def video_
-00029520: 746f 5f62 7728 7669 6465 6f5f 7061 7468  to_bw(video_path
-00029530: 3a20 556e 696f 6e5b 7374 722c 206f 732e  : Union[str, os.
-00029540: 5061 7468 4c69 6b65 5d2c 0a20 2020 2020  PathLike],.     
-00029550: 2020 2020 2020 2020 2020 2074 6872 6573             thres
-00029560: 686f 6c64 3a20 4f70 7469 6f6e 616c 5b66  hold: Optional[f
-00029570: 6c6f 6174 5d20 3d20 302e 3529 202d 3e20  loat] = 0.5) -> 
-00029580: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-00029590: 2020 436f 6e76 6572 7420 7669 6465 6f20    Convert video 
-000295a0: 746f 2062 6c61 636b 2061 6e64 2077 6869  to black and whi
-000295b0: 7465 2075 7369 6e67 2070 6173 7365 6420  te using passed 
-000295c0: 7468 7265 7368 6f6c 642e 0a0a 2020 2020  threshold...    
-000295d0: 2e2e 2076 6964 656f 3a3a 205f 7374 6174  .. video:: _stat
-000295e0: 6963 2f69 6d67 2f76 6964 656f 5f74 6f5f  ic/img/video_to_
-000295f0: 6277 2e77 6562 6d0a 2020 2020 2020 203a  bw.webm.       :
-00029600: 6c6f 6f70 3a0a 0a20 2020 203a 7061 7261  loop:..    :para
-00029610: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
-00029620: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
-00029630: 7061 7468 3a20 5061 7468 2074 6f20 7468  path: Path to th
-00029640: 6520 7669 6465 6f0a 2020 2020 3a70 6172  e video.    :par
-00029650: 616d 204f 7074 696f 6e61 6c5b 666c 6f61  am Optional[floa
-00029660: 745d 2074 6872 6573 686f 6c64 3a20 5661  t] threshold: Va
-00029670: 6c75 6520 6265 7477 6565 6e20 3020 616e  lue between 0 an
-00029680: 6420 312e 204c 6f77 6572 2076 616c 7565  d 1. Lower value
-00029690: 7320 6769 7665 7320 6d6f 7265 2077 6869  s gives more whi
-000296a0: 7465 2061 6e64 2076 6963 6520 7665 7273  te and vice vers
-000296b0: 612e 0a20 2020 203a 7265 7475 726e 3a20  a..    :return: 
-000296c0: 4e6f 6e65 2e0a 0a20 2020 203a 6578 616d  None...    :exam
-000296d0: 706c 653a 0a20 2020 203e 3e3e 2076 6964  ple:.    >>> vid
-000296e0: 656f 5f74 6f5f 6277 2876 6964 656f 5f70  eo_to_bw(video_p
-000296f0: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
-00029700: 6e2f 446f 776e 6c6f 6164 732f 315f 4c48  n/Downloads/1_LH
-00029710: 5f63 6c69 7070 6564 5f63 726f 7070 6564  _clipped_cropped
-00029720: 5f65 715f 3230 3234 3035 3135 3133 3539  _eq_202405151359
-00029730: 3236 2e6d 7034 272c 2074 6872 6573 686f  26.mp4', thresho
-00029740: 6c64 3d30 2e30 3229 0a20 2020 2022 2222  ld=0.02).    """
-00029750: 0a0a 2020 2020 6368 6563 6b5f 666c 6f61  ..    check_floa
-00029760: 7428 6e61 6d65 3d66 277b 7669 6465 6f5f  t(name=f'{video_
-00029770: 746f 5f62 772e 5f5f 6e61 6d65 5f5f 7d20  to_bw.__name__} 
-00029780: 7468 7265 7368 6f6c 6427 2c20 7661 6c75  threshold', valu
-00029790: 653d 7468 7265 7368 6f6c 642c 206d 696e  e=threshold, min
-000297a0: 5f76 616c 7565 3d30 2c20 6d61 785f 7661  _value=0, max_va
-000297b0: 6c75 653d 312e 3029 0a20 2020 2074 6872  lue=1.0).    thr
-000297c0: 6573 686f 6c64 203d 2069 6e74 2832 3535  eshold = int(255
-000297d0: 202a 2074 6872 6573 686f 6c64 290a 2020   * threshold).  
-000297e0: 2020 6368 6563 6b5f 6666 6d70 6567 5f61    check_ffmpeg_a
-000297f0: 7661 696c 6162 6c65 2872 6169 7365 5f65  vailable(raise_e
-00029800: 7272 6f72 3d54 7275 6529 0a20 2020 2074  rror=True).    t
-00029810: 696d 6572 203d 2053 696d 6261 5469 6d65  imer = SimbaTime
-00029820: 7228 7374 6172 743d 5472 7565 290a 2020  r(start=True).  
-00029830: 2020 5f20 3d20 6765 745f 7669 6465 6f5f    _ = get_video_
-00029840: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
-00029850: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
-00029860: 0a20 2020 2064 6972 2c20 7669 6465 6f5f  .    dir, video_
-00029870: 6e61 6d65 2c20 6578 7420 3d20 6765 745f  name, ext = get_
-00029880: 666e 5f65 7874 2876 6964 656f 5f70 6174  fn_ext(video_pat
-00029890: 6829 0a20 2020 2073 6176 655f 7061 7468  h).    save_path
-000298a0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000298b0: 6469 722c 2066 277b 7669 6465 6f5f 6e61  dir, f'{video_na
-000298c0: 6d65 7d5f 6277 7b65 7874 7d27 290a 2020  me}_bw{ext}').  
-000298d0: 2020 636d 6420 3d20 6622 6666 6d70 6567    cmd = f"ffmpeg
-000298e0: 202d 6920 277b 7669 6465 6f5f 7061 7468   -i '{video_path
-000298f0: 7d27 202d 7666 205c 2266 6f72 6d61 743d  }' -vf \"format=
-00029900: 6772 6179 2c67 6571 3d6c 756d 5f65 7870  gray,geq=lum_exp
-00029910: 723d 2769 6628 6c74 286c 756d 2858 2c59  r='if(lt(lum(X,Y
-00029920: 292c 7b74 6872 6573 686f 6c64 7d29 2c30  ),{threshold}),0
-00029930: 2c32 3535 2927 5c22 202d 7069 785f 666d  ,255)'\" -pix_fm
-00029940: 7420 7975 7634 3230 7020 277b 7361 7665  t yuv420p '{save
-00029950: 5f70 6174 687d 2720 2d79 220a 2020 2020  _path}' -y".    
-00029960: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
-00029970: 636d 642c 2073 6865 6c6c 3d54 7275 652c  cmd, shell=True,
-00029980: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
-00029990: 7373 2e50 4950 4529 0a20 2020 2074 696d  ss.PIPE).    tim
-000299a0: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
-000299b0: 2020 2020 7374 646f 7574 5f73 7563 6365      stdout_succe
-000299c0: 7373 286d 7367 3d66 2756 6964 656f 207b  ss(msg=f'Video {
-000299d0: 7669 6465 6f5f 6e61 6d65 7d20 636f 6e76  video_name} conv
-000299e0: 6572 7465 642e 272c 2065 6c61 7073 6564  erted.', elapsed
-000299f0: 5f74 696d 653d 7469 6d65 722e 656c 6170  _time=timer.elap
-00029a00: 7365 645f 7469 6d65 5f73 7472 290a 0a0a  sed_time_str)...
-00029a10: 6465 6620 6372 6561 7465 5f61 7665 7261  def create_avera
-00029a20: 6765 5f66 726d 2876 6964 656f 5f70 6174  ge_frm(video_pat
-00029a30: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
-00029a40: 2e50 6174 684c 696b 655d 2c0a 2020 2020  .PathLike],.    
-00029a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a60: 2020 2073 7461 7274 5f66 726d 3a20 4f70     start_frm: Op
-00029a70: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00029a80: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00029a90: 2020 2020 2020 2020 2020 2065 6e64 5f66             end_f
-00029aa0: 726d 3a20 4f70 7469 6f6e 616c 5b69 6e74  rm: Optional[int
-00029ab0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00029ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ad0: 2073 7461 7274 5f74 696d 653a 204f 7074   start_time: Opt
-00029ae0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00029af0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00029b00: 2020 2020 2020 2020 2020 656e 645f 7469            end_ti
-00029b10: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-00029b20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00026210: 290a 0a64 6566 2073 7570 6572 696d 706f  )..def superimpo
+00026220: 7365 5f6f 7665 726c 6179 5f76 6964 656f  se_overlay_video
+00026230: 2876 6964 656f 5f70 6174 683a 2055 6e69  (video_path: Uni
+00026240: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+00026250: 696b 655d 2c0a 2020 2020 2020 2020 2020  ike],.          
+00026260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026270: 2020 2020 6f76 6572 6c61 795f 7669 6465      overlay_vide
+00026280: 6f5f 7061 7468 3a20 556e 696f 6e5b 7374  o_path: Union[st
+00026290: 722c 206f 732e 5061 7468 4c69 6b65 5d2c  r, os.PathLike],
+000262a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000262b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000262c0: 6f73 6974 696f 6e3a 204f 7074 696f 6e61  osition: Optiona
+000262d0: 6c5b 4c69 7465 7261 6c5b 2774 6f70 5f6c  l[Literal['top_l
+000262e0: 6566 7427 2c20 2762 6f74 746f 6d5f 7269  eft', 'bottom_ri
+000262f0: 6768 7427 2c20 2774 6f70 5f72 6967 6874  ght', 'top_right
+00026300: 272c 2027 626f 7474 6f6d 5f6c 6566 7427  ', 'bottom_left'
+00026310: 2c20 2763 656e 7465 7227 5d5d 203d 2027  , 'center']] = '
+00026320: 746f 705f 6c65 6674 272c 0a20 2020 2020  top_left',.     
+00026330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026340: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
+00026350: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+00026360: 5d20 3d20 302e 352c 0a20 2020 2020 2020  ] = 0.5,.       
+00026370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026380: 2020 2020 2020 2073 6361 6c65 3a20 4f70         scale: Op
+00026390: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+000263a0: 302e 3035 2c0a 2020 2020 2020 2020 2020  0.05,.          
+000263b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263c0: 2020 2020 7361 7665 5f64 6972 3a20 4f70      save_dir: Op
+000263d0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+000263e0: 2c20 6f73 2e50 6174 684c 696b 655d 5d20  , os.PathLike]] 
+000263f0: 3d20 4e6f 6e65 2920 2d3e 204e 6f6e 653a  = None) -> None:
+00026400: 0a20 2020 2022 2222 0a20 2020 2049 6e73  .    """.    Ins
+00026410: 6574 2061 2076 6964 656f 206f 7665 726c  et a video overl
+00026420: 6179 206f 6e20 6120 7365 636f 6e64 2076  ay on a second v
+00026430: 6964 656f 2077 6974 6820 7370 6563 6966  ideo with specif
+00026440: 6965 6420 7369 7a65 2c20 6f70 6163 6974  ied size, opacit
+00026450: 792c 2061 6e64 206c 6f63 6174 696f 6e2e  y, and location.
+00026460: 0a0a 2020 2020 2e2e 2076 6964 656f 3a3a  ..    .. video::
+00026470: 205f 7374 6174 6963 2f69 6d67 2f69 6e73   _static/img/ins
+00026480: 6574 5f6f 7665 726c 6179 5f76 6964 656f  et_overlay_video
+00026490: 2e77 6562 6d0a 2020 2020 2020 203a 7769  .webm.       :wi
+000264a0: 6474 683a 2037 3030 0a20 2020 2020 2020  dth: 700.       
+000264b0: 3a6c 6f6f 703a 0a0a 2020 2020 3a70 6172  :loop:..    :par
+000264c0: 616d 2055 6e69 6f6e 5b73 7472 2c20 6f73  am Union[str, os
+000264d0: 2e50 6174 684c 696b 655d 2076 6964 656f  .PathLike] video
+000264e0: 5f70 6174 683a 2054 6865 2070 6174 6820  _path: The path 
+000264f0: 746f 2074 6865 2076 6964 656f 2066 696c  to the video fil
+00026500: 652e 0a20 2020 203a 7061 7261 6d20 556e  e..    :param Un
+00026510: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+00026520: 4c69 6b65 5d20 6f76 6572 6c61 795f 7669  Like] overlay_vi
+00026530: 6465 6f5f 7061 7468 3a20 5468 6520 7061  deo_path: The pa
+00026540: 7468 2074 6f20 7669 6465 6f20 746f 2062  th to video to b
+00026550: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+00026560: 7468 6520 6060 7669 6465 6f5f 7061 7468  the ``video_path
+00026570: 6060 2076 6964 656f 2e0a 2020 2020 3a70  `` video..    :p
+00026580: 6172 616d 204f 7074 696f 6e61 6c5b 7374  aram Optional[st
+00026590: 725d 2070 6f73 6974 696f 6e3a 2054 6865  r] position: The
+000265a0: 2070 6f73 6974 696f 6e20 6f66 2074 6865   position of the
+000265b0: 2069 6e73 6574 206f 7665 726c 6179 2076   inset overlay v
+000265c0: 6964 656f 2e20 4f70 7469 6f6e 733a 2027  ideo. Options: '
+000265d0: 746f 705f 6c65 6674 272c 2027 626f 7474  top_left', 'bott
+000265e0: 6f6d 5f72 6967 6874 272c 2027 746f 705f  om_right', 'top_
+000265f0: 7269 6768 7427 2c20 2762 6f74 746f 6d5f  right', 'bottom_
+00026600: 6c65 6674 272c 2027 6365 6e74 6572 270a  left', 'center'.
+00026610: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00026620: 6e61 6c5b 666c 6f61 745d 206f 7061 6369  nal[float] opaci
+00026630: 7479 3a20 5468 6520 6f70 6163 6974 7920  ty: The opacity 
+00026640: 6f66 2074 6865 2069 6e73 6574 206f 7665  of the inset ove
+00026650: 726c 6179 2076 6964 656f 2061 7320 6120  rlay video as a 
+00026660: 7661 6c75 6520 6265 7477 6565 6e20 302d  value between 0-
+00026670: 312e 302e 2031 2e30 206d 6561 6e69 6e67  1.0. 1.0 meaning
+00026680: 2074 6865 2073 616d 6520 6173 2069 6e70   the same as inp
+00026690: 7574 2069 6d61 6765 2e20 4465 6661 756c  ut image. Defaul
+000266a0: 743a 2030 2e35 2e0a 2020 2020 3a70 6172  t: 0.5..    :par
+000266b0: 616d 204f 7074 696f 6e61 6c5b 666c 6f61  am Optional[floa
+000266c0: 745d 2073 6361 6c65 3a20 5468 6520 7363  t] scale: The sc
+000266d0: 616c 6520 6f66 2074 6865 2069 6e73 6574  ale of the inset
+000266e0: 206f 7665 726c 6179 2076 6964 656f 2061   overlay video a
+000266f0: 7320 6120 7261 7469 6f20 6f73 2074 6865  s a ratio os the
+00026700: 2069 6d61 6765 2073 697a 652e 2044 6566   image size. Def
+00026710: 6175 6c74 3a20 302e 3035 2e0a 2020 2020  ault: 0.05..    
+00026720: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+00026730: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00026740: 7468 4c69 6b65 5d5d 2073 6176 655f 6469  thLike]] save_di
+00026750: 723a 2054 6865 206c 6f63 6174 696f 6e20  r: The location 
+00026760: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
+00026770: 6520 6f75 7470 7574 2076 6964 656f 2e20  e output video. 
+00026780: 4966 204e 6f6e 652c 2074 6865 6e20 7361  If None, then sa
+00026790: 7665 7320 7468 6520 7669 6465 6f20 696e  ves the video in
+000267a0: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
+000267b0: 6f72 7920 6173 2074 6865 2066 6972 7374  ory as the first
+000267c0: 2076 6964 656f 2e0a 2020 2020 3a72 6574   video..    :ret
+000267d0: 7572 6e3a 204e 6f6e 650a 0a20 2020 203a  urn: None..    :
+000267e0: 6578 616d 706c 653a 0a20 2020 203e 3e3e  example:.    >>>
+000267f0: 2073 7570 6572 696d 706f 7365 5f6f 7665   superimpose_ove
+00026800: 726c 6179 5f76 6964 656f 2876 6964 656f  rlay_video(video
+00026810: 5f70 6174 683d 272f 5573 6572 732f 7369  _path='/Users/si
+00026820: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00026830: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00026840: 6f6f 7469 6e67 2f6d 756c 7469 5f61 6e69  ooting/multi_ani
+00026850: 6d61 6c5f 646c 635f 7477 6f5f 6335 372f  mal_dlc_two_c57/
+00026860: 7072 6f6a 6563 745f 666f 6c64 6572 2f76  project_folder/v
+00026870: 6964 656f 732f 7761 7465 726d 6172 6b2f  ideos/watermark/
+00026880: 546f 6765 7468 6572 5f31 5f70 6f77 6572  Together_1_power
+00026890: 706f 696e 7472 6561 6479 2e6d 7034 272c  pointready.mp4',
+000268a0: 206f 7665 726c 6179 5f76 6964 656f 5f70   overlay_video_p
+000268b0: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
+000268c0: 6e2f 4465 736b 746f 702f 7370 6c61 7368  n/Desktop/splash
+000268d0: 2e70 6e67 272c 2070 6f73 6974 696f 6e3d  .png', position=
+000268e0: 2774 6f70 5f6c 6566 7427 2c20 6f70 6163  'top_left', opac
+000268f0: 6974 793d 312e 302c 2073 6361 6c65 3d30  ity=1.0, scale=0
+00026900: 2e32 290a 2020 2020 2222 220a 0a20 2020  .2).    """..   
+00026910: 2074 696d 6572 203d 2053 696d 6261 5469   timer = SimbaTi
+00026920: 6d65 7228 7374 6172 743d 5472 7565 290a  mer(start=True).
+00026930: 2020 2020 504f 5349 5449 4f4e 5320 3d20      POSITIONS = 
+00026940: 5b27 746f 705f 6c65 6674 272c 2027 626f  ['top_left', 'bo
+00026950: 7474 6f6d 5f72 6967 6874 272c 2027 746f  ttom_right', 'to
+00026960: 705f 7269 6768 7427 2c20 2762 6f74 746f  p_right', 'botto
+00026970: 6d5f 6c65 6674 272c 2027 6365 6e74 6572  m_left', 'center
+00026980: 275d 0a20 2020 2063 6865 636b 5f66 6c6f  '].    check_flo
+00026990: 6174 286e 616d 653d 6627 7b73 7570 6572  at(name=f'{super
+000269a0: 696d 706f 7365 5f6f 7665 726c 6179 5f76  impose_overlay_v
+000269b0: 6964 656f 2e5f 5f6e 616d 655f 5f7d 206f  ideo.__name__} o
+000269c0: 7061 6369 7479 272c 2076 616c 7565 3d6f  pacity', value=o
+000269d0: 7061 6369 7479 2c20 6d69 6e5f 7661 6c75  pacity, min_valu
+000269e0: 653d 302e 3030 312c 206d 6178 5f76 616c  e=0.001, max_val
+000269f0: 7565 3d31 2e30 290a 2020 2020 6368 6563  ue=1.0).    chec
+00026a00: 6b5f 666c 6f61 7428 6e61 6d65 3d66 277b  k_float(name=f'{
+00026a10: 7375 7065 7269 6d70 6f73 655f 6f76 6572  superimpose_over
+00026a20: 6c61 795f 7669 6465 6f2e 5f5f 6e61 6d65  lay_video.__name
+00026a30: 5f5f 7d20 7363 616c 6527 2c20 7661 6c75  __} scale', valu
+00026a40: 653d 7363 616c 652c 206d 696e 5f76 616c  e=scale, min_val
+00026a50: 7565 3d30 2e30 3031 2c20 6d61 785f 7661  ue=0.001, max_va
+00026a60: 6c75 653d 302e 3939 3929 0a20 2020 2063  lue=0.999).    c
+00026a70: 6865 636b 5f73 7472 286e 616d 653d 6627  heck_str(name=f'
+00026a80: 7b73 7570 6572 696d 706f 7365 5f6f 7665  {superimpose_ove
+00026a90: 726c 6179 5f76 6964 656f 2e5f 5f6e 616d  rlay_video.__nam
+00026aa0: 655f 5f7d 2070 6f73 6974 696f 6e27 2c20  e__} position', 
+00026ab0: 7661 6c75 653d 706f 7369 7469 6f6e 2c20  value=position, 
+00026ac0: 6f70 7469 6f6e 733d 504f 5349 5449 4f4e  options=POSITION
+00026ad0: 5329 0a20 2020 2063 6865 636b 5f66 696c  S).    check_fil
+00026ae0: 655f 6578 6973 745f 616e 645f 7265 6164  e_exist_and_read
+00026af0: 6162 6c65 2866 696c 655f 7061 7468 3d76  able(file_path=v
+00026b00: 6964 656f 5f70 6174 6829 0a20 2020 2063  ideo_path).    c
+00026b10: 6865 636b 5f66 696c 655f 6578 6973 745f  heck_file_exist_
+00026b20: 616e 645f 7265 6164 6162 6c65 2866 696c  and_readable(fil
+00026b30: 655f 7061 7468 3d6f 7665 726c 6179 5f76  e_path=overlay_v
+00026b40: 6964 656f 5f70 6174 6829 0a0a 2020 2020  ideo_path)..    
+00026b50: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+00026b60: 6528 7669 6465 6f5f 7061 7468 293a 0a20  e(video_path):. 
+00026b70: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
+00026b80: 6873 203d 205b 7669 6465 6f5f 7061 7468  hs = [video_path
+00026b90: 5d0a 2020 2020 656c 6966 206f 732e 7061  ].    elif os.pa
+00026ba0: 7468 2e69 7364 6972 2876 6964 656f 5f70  th.isdir(video_p
+00026bb0: 6174 6829 3a0a 2020 2020 2020 2020 7669  ath):.        vi
+00026bc0: 6465 6f5f 7061 7468 7320 3d20 6c69 7374  deo_paths = list
+00026bd0: 2866 696e 645f 616c 6c5f 7669 6465 6f73  (find_all_videos
+00026be0: 5f69 6e5f 6469 7265 6374 6f72 7928 6469  _in_directory(di
+00026bf0: 7265 6374 6f72 793d 7669 6465 6f5f 7061  rectory=video_pa
+00026c00: 7468 2c20 6173 5f64 6963 743d 5472 7565  th, as_dict=True
+00026c10: 2c20 7261 6973 655f 6572 726f 723d 5472  , raise_error=Tr
+00026c20: 7565 292e 7661 6c75 6573 2829 290a 2020  ue).values()).  
+00026c30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00026c40: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
+00026c50: 7574 4572 726f 7228 6d73 673d 6627 7b76  utError(msg=f'{v
+00026c60: 6964 656f 5f70 6174 687d 2069 7320 6e6f  ideo_path} is no
+00026c70: 7420 6120 7661 6c69 6420 6669 6c65 2070  t a valid file p
+00026c80: 6174 6820 6f72 2061 2076 616c 6964 2064  ath or a valid d
+00026c90: 6972 6563 746f 7279 2070 6174 6827 2c0a  irectory path',.
+00026ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026cc0: 736f 7572 6365 3d73 7570 6572 696d 706f  source=superimpo
+00026cd0: 7365 5f6f 7665 726c 6179 5f76 6964 656f  se_overlay_video
+00026ce0: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2069  .__name__).    i
+00026cf0: 6620 7361 7665 5f64 6972 2069 7320 6e6f  f save_dir is no
+00026d00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00026d10: 6368 6563 6b5f 6966 5f64 6972 5f65 7869  check_if_dir_exi
+00026d20: 7374 7328 696e 5f64 6972 3d73 6176 655f  sts(in_dir=save_
+00026d30: 6469 7229 0a20 2020 2065 6c73 653a 0a20  dir).    else:. 
+00026d40: 2020 2020 2020 2073 6176 655f 6469 7220         save_dir 
+00026d50: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+00026d60: 6528 7669 6465 6f5f 7061 7468 735b 305d  e(video_paths[0]
+00026d70: 290a 2020 2020 666f 7220 6669 6c65 5f63  ).    for file_c
+00026d80: 6e74 2c20 7669 6465 6f5f 7061 7468 2069  nt, video_path i
+00026d90: 6e20 656e 756d 6572 6174 6528 7669 6465  n enumerate(vide
+00026da0: 6f5f 7061 7468 7329 3a0a 2020 2020 2020  o_paths):.      
+00026db0: 2020 5f2c 2076 6964 656f 5f6e 616d 652c    _, video_name,
+00026dc0: 2076 6964 656f 5f65 7874 203d 2067 6574   video_ext = get
+00026dd0: 5f66 6e5f 6578 7428 7669 6465 6f5f 7061  _fn_ext(video_pa
+00026de0: 7468 290a 2020 2020 2020 2020 5f20 3d20  th).        _ = 
+00026df0: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
+00026e00: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
+00026e10: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
+00026e20: 2020 2070 7269 6e74 2866 2749 6e73 6572     print(f'Inser
+00026e30: 7469 6e67 206f 7665 726c 6179 206f 6e74  ting overlay ont
+00026e40: 6f20 7b76 6964 656f 5f6e 616d 657d 2028  o {video_name} (
+00026e50: 5669 6465 6f20 7b66 696c 655f 636e 7420  Video {file_cnt 
+00026e60: 2b20 317d 2f7b 6c65 6e28 7669 6465 6f5f  + 1}/{len(video_
+00026e70: 7061 7468 7329 7d29 2e2e 2e27 290a 2020  paths)})...').  
+00026e80: 2020 2020 2020 6f75 745f 7061 7468 203d        out_path =
+00026e90: 206f 732e 7061 7468 2e6a 6f69 6e28 7361   os.path.join(sa
+00026ea0: 7665 5f64 6972 2c20 6627 7b76 6964 656f  ve_dir, f'{video
+00026eb0: 5f6e 616d 657d 5f69 6e73 6574 5f6f 7665  _name}_inset_ove
+00026ec0: 726c 6179 7b76 6964 656f 5f65 7874 7d27  rlay{video_ext}'
+00026ed0: 290a 2020 2020 2020 2020 6966 2070 6f73  ).        if pos
+00026ee0: 6974 696f 6e20 3d3d 2050 4f53 4954 494f  ition == POSITIO
+00026ef0: 4e53 5b30 5d3a 0a20 2020 2020 2020 2020  NS[0]:.         
+00026f00: 2020 2063 6d64 203d 2066 2766 666d 7065     cmd = f'ffmpe
+00026f10: 6720 2d69 2022 7b76 6964 656f 5f70 6174  g -i "{video_pat
+00026f20: 687d 2220 2d69 2022 7b6f 7665 726c 6179  h}" -i "{overlay
+00026f30: 5f76 6964 656f 5f70 6174 687d 2220 2d66  _video_path}" -f
+00026f40: 696c 7465 725f 636f 6d70 6c65 7820 225b  ilter_complex "[
+00026f50: 313a 765d 7363 616c 653d 6977 2a7b 7363  1:v]scale=iw*{sc
+00026f60: 616c 657d 3a2d 312c 666f 726d 6174 3d72  ale}:-1,format=r
+00026f70: 6762 612c 636f 6c6f 7263 6861 6e6e 656c  gba,colorchannel
+00026f80: 6d69 7865 723d 6161 3d7b 6f70 6163 6974  mixer=aa={opacit
+00026f90: 797d 5b69 6e73 6574 5d3b 5b30 3a76 5d5b  y}[inset];[0:v][
+00026fa0: 696e 7365 745d 6f76 6572 6c61 793d 303a  inset]overlay=0:
+00026fb0: 3022 2022 7b6f 7574 5f70 6174 687d 2220  0" "{out_path}" 
+00026fc0: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
+00026fd0: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
+00026fe0: 6e65 7220 2d79 270a 2020 2020 2020 2020  ner -y'.        
+00026ff0: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
+00027000: 2050 4f53 4954 494f 4e53 5b31 5d3a 0a20   POSITIONS[1]:. 
+00027010: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00027020: 2066 2766 666d 7065 6720 2d69 2022 7b76   f'ffmpeg -i "{v
+00027030: 6964 656f 5f70 6174 687d 2220 2d69 2022  ideo_path}" -i "
+00027040: 7b6f 7665 726c 6179 5f76 6964 656f 5f70  {overlay_video_p
+00027050: 6174 687d 2220 2d66 696c 7465 725f 636f  ath}" -filter_co
+00027060: 6d70 6c65 7820 225b 313a 765d 7363 616c  mplex "[1:v]scal
+00027070: 653d 6977 2a7b 7363 616c 657d 3a2d 312c  e=iw*{scale}:-1,
+00027080: 666f 726d 6174 3d72 6762 612c 636f 6c6f  format=rgba,colo
+00027090: 7263 6861 6e6e 656c 6d69 7865 723d 6161  rchannelmixer=aa
+000270a0: 3d7b 6f70 6163 6974 797d 5b69 6e73 6574  ={opacity}[inset
+000270b0: 5d3b 5b30 3a76 5d5b 696e 7365 745d 6f76  ];[0:v][inset]ov
+000270c0: 6572 6c61 793d 572d 773a 482d 6822 2022  erlay=W-w:H-h" "
+000270d0: 7b6f 7574 5f70 6174 687d 2220 2d6c 6f67  {out_path}" -log
+000270e0: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
+000270f0: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
+00027100: 2d79 270a 2020 2020 2020 2020 656c 6966  -y'.        elif
+00027110: 2070 6f73 6974 696f 6e20 3d3d 2050 4f53   position == POS
+00027120: 4954 494f 4e53 5b32 5d3a 0a20 2020 2020  ITIONS[2]:.     
+00027130: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
+00027140: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
+00027150: 5f70 6174 687d 2220 2d69 2022 7b6f 7665  _path}" -i "{ove
+00027160: 726c 6179 5f76 6964 656f 5f70 6174 687d  rlay_video_path}
+00027170: 2220 2d66 696c 7465 725f 636f 6d70 6c65  " -filter_comple
+00027180: 7820 225b 313a 765d 7363 616c 653d 6977  x "[1:v]scale=iw
+00027190: 2a7b 7363 616c 657d 3a2d 312c 666f 726d  *{scale}:-1,form
+000271a0: 6174 3d72 6762 612c 636f 6c6f 7263 6861  at=rgba,colorcha
+000271b0: 6e6e 656c 6d69 7865 723d 6161 3d7b 6f70  nnelmixer=aa={op
+000271c0: 6163 6974 797d 5b69 6e73 6574 5d3b 5b30  acity}[inset];[0
+000271d0: 3a76 5d5b 696e 7365 745d 6f76 6572 6c61  :v][inset]overla
+000271e0: 793d 572d 773a 3022 2022 7b6f 7574 5f70  y=W-w:0" "{out_p
+000271f0: 6174 687d 2220 2d6c 6f67 6c65 7665 6c20  ath}" -loglevel 
+00027200: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
+00027210: 6465 5f62 616e 6e65 7220 2d79 270a 2020  de_banner -y'.  
+00027220: 2020 2020 2020 656c 6966 2070 6f73 6974        elif posit
+00027230: 696f 6e20 3d3d 2050 4f53 4954 494f 4e53  ion == POSITIONS
+00027240: 5b33 5d3a 0a20 2020 2020 2020 2020 2020  [3]:.           
+00027250: 2063 6d64 203d 2066 2766 666d 7065 6720   cmd = f'ffmpeg 
+00027260: 2d69 2022 7b76 6964 656f 5f70 6174 687d  -i "{video_path}
+00027270: 2220 2d69 2022 7b6f 7665 726c 6179 5f76  " -i "{overlay_v
+00027280: 6964 656f 5f70 6174 687d 2220 2d66 696c  ideo_path}" -fil
+00027290: 7465 725f 636f 6d70 6c65 7820 225b 313a  ter_complex "[1:
+000272a0: 765d 7363 616c 653d 6977 2a7b 7363 616c  v]scale=iw*{scal
+000272b0: 657d 3a2d 312c 666f 726d 6174 3d72 6762  e}:-1,format=rgb
+000272c0: 612c 636f 6c6f 7263 6861 6e6e 656c 6d69  a,colorchannelmi
+000272d0: 7865 723d 6161 3d7b 6f70 6163 6974 797d  xer=aa={opacity}
+000272e0: 5b69 6e73 6574 5d3b 5b30 3a76 5d5b 696e  [inset];[0:v][in
+000272f0: 7365 745d 6f76 6572 6c61 793d 303a 482d  set]overlay=0:H-
+00027300: 6822 2022 7b6f 7574 5f70 6174 687d 2220  h" "{out_path}" 
+00027310: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
+00027320: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
+00027330: 6e65 7220 2d79 270a 2020 2020 2020 2020  ner -y'.        
+00027340: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00027350: 2020 636d 6420 3d20 6627 6666 6d70 6567    cmd = f'ffmpeg
+00027360: 202d 6920 227b 7669 6465 6f5f 7061 7468   -i "{video_path
+00027370: 7d22 202d 6920 227b 6f76 6572 6c61 795f  }" -i "{overlay_
+00027380: 7669 6465 6f5f 7061 7468 7d22 202d 6669  video_path}" -fi
+00027390: 6c74 6572 5f63 6f6d 706c 6578 2022 5b31  lter_complex "[1
+000273a0: 3a76 5d73 6361 6c65 3d69 772a 7b73 6361  :v]scale=iw*{sca
+000273b0: 6c65 7d3a 2d31 2c66 6f72 6d61 743d 7267  le}:-1,format=rg
+000273c0: 6261 2c63 6f6c 6f72 6368 616e 6e65 6c6d  ba,colorchannelm
+000273d0: 6978 6572 3d61 613d 7b6f 7061 6369 7479  ixer=aa={opacity
+000273e0: 7d5b 696e 7365 745d 3b5b 303a 765d 5b69  }[inset];[0:v][i
+000273f0: 6e73 6574 5d6f 7665 726c 6179 3d28 572d  nset]overlay=(W-
+00027400: 7729 2f32 3a28 482d 6829 2f32 2220 227b  w)/2:(H-h)/2" "{
+00027410: 6f75 745f 7061 7468 7d22 202d 6c6f 676c  out_path}" -logl
+00027420: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
+00027430: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
+00027440: 7927 0a20 2020 2020 2020 2073 7562 7072  y'.        subpr
+00027450: 6f63 6573 732e 6361 6c6c 2863 6d64 2c20  ocess.call(cmd, 
+00027460: 7368 656c 6c3d 5472 7565 2c20 7374 646f  shell=True, stdo
+00027470: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
+00027480: 5045 290a 2020 2020 7469 6d65 722e 7374  PE).    timer.st
+00027490: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
+000274a0: 7464 6f75 745f 7375 6363 6573 7328 6d73  tdout_success(ms
+000274b0: 673d 6627 7b6c 656e 2876 6964 656f 5f70  g=f'{len(video_p
+000274c0: 6174 6873 297d 206f 7665 726c 6179 2076  aths)} overlay v
+000274d0: 6964 656f 2873 2920 7361 7665 6420 696e  ideo(s) saved in
+000274e0: 207b 7361 7665 5f64 6972 7d27 2c20 656c   {save_dir}', el
+000274f0: 6170 7365 645f 7469 6d65 3d74 696d 6572  apsed_time=timer
+00027500: 2e65 6c61 7073 6564 5f74 696d 655f 7374  .elapsed_time_st
+00027510: 7229 0a0a 6465 6620 726f 695f 626c 7572  r)..def roi_blur
+00027520: 626f 7828 7669 6465 6f5f 7061 7468 3a20  box(video_path: 
+00027530: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00027540: 7468 4c69 6b65 5d2c 0a20 2020 2020 2020  thLike],.       
+00027550: 2020 2020 2020 2020 2062 6c75 725f 6c65           blur_le
+00027560: 7665 6c3a 204f 7074 696f 6e61 6c5b 666c  vel: Optional[fl
+00027570: 6f61 745d 203d 2030 2e30 322c 0a20 2020  oat] = 0.02,.   
+00027580: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
+00027590: 6572 743a 204f 7074 696f 6e61 6c5b 626f  ert: Optional[bo
+000275a0: 6f6c 5d20 3d20 4661 6c73 652c 0a20 2020  ol] = False,.   
+000275b0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+000275c0: 655f 7061 7468 3a20 4f70 7469 6f6e 616c  e_path: Optional
+000275d0: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
+000275e0: 6174 684c 696b 655d 5d20 3d20 4e6f 6e65  athLike]] = None
+000275f0: 2920 2d3e 204e 6f6e 653a 0a0a 2020 2020  ) -> None:..    
+00027600: 2222 220a 2020 2020 426c 7572 7320 6569  """.    Blurs ei
+00027610: 7468 6572 2074 6865 2073 656c 6563 7465  ther the selecte
+00027620: 6420 6f72 2075 6e73 656c 6563 7465 6420  d or unselected 
+00027630: 706f 7274 696f 6e20 6f66 2061 2075 7365  portion of a use
+00027640: 722d 7370 6563 6966 6965 6420 7265 6769  r-specified regi
+00027650: 6f6e 2d6f 662d 696e 7465 7265 7374 2061  on-of-interest a
+00027660: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+00027670: 7061 7373 6564 2062 6c75 7220 6c65 7665  passed blur leve
+00027680: 6c2e 0a20 2020 2048 6967 6865 7220 626c  l..    Higher bl
+00027690: 7572 206c 6576 656c 7320 7072 6f64 7563  ur levels produc
+000276a0: 6573 206d 6f72 6520 6f70 6171 7565 2072  es more opaque r
+000276b0: 6567 696f 6e73 2e0a 0a20 2020 202e 2e20  egions...    .. 
+000276c0: 7669 6465 6f3a 3a20 5f73 7461 7469 632f  video:: _static/
+000276d0: 696d 672f 726f 695f 626c 7572 626f 782e  img/roi_blurbox.
+000276e0: 7765 626d 0a20 2020 2020 2020 3a6c 6f6f  webm.       :loo
+000276f0: 703a 0a0a 2020 2020 3a70 6172 616d 2055  p:..    :param U
+00027700: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+00027710: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
+00027720: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
+00027730: 6865 2076 6964 656f 206f 6e20 6469 736b  he video on disk
+00027740: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00027750: 6f6e 616c 5b66 6c6f 6174 5d20 626c 7572  onal[float] blur
+00027760: 5f6c 6576 656c 3a20 5468 6520 6c65 7665  _level: The leve
+00027770: 6c20 6f66 2074 6865 2062 6c75 7220 6173  l of the blur as
+00027780: 2061 2072 6174 696f 2030 2d31 2e30 2e0a   a ratio 0-1.0..
+00027790: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+000277a0: 6e61 6c5b 626f 6f6c 5d20 696e 7665 7274  nal[bool] invert
+000277b0: 3a20 4966 2054 7275 652c 2062 6c75 7273  : If True, blurs
+000277c0: 2074 6865 2075 6e73 656c 6563 7465 6420   the unselected 
+000277d0: 7265 6769 6f6e 2e20 4966 2046 616c 7365  region. If False
+000277e0: 2c20 626c 7572 7320 7468 6520 7365 6c65  , blurs the sele
+000277f0: 6374 6564 2072 6567 696f 6e2e 0a20 2020  cted region..   
+00027800: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00027810: 5b55 6e69 6f6e 5b73 7472 2c20 6f73 2e50  [Union[str, os.P
+00027820: 6174 684c 696b 655d 5d20 7361 7665 5f70  athLike]] save_p
+00027830: 6174 683a 2054 6865 206c 6f63 6174 696f  ath: The locatio
+00027840: 6e20 7768 6572 6520 746f 2073 6176 6520  n where to save 
+00027850: 7468 6520 626c 7572 7265 6420 7669 6465  the blurred vide
+00027860: 6f2e 2049 6620 4e6f 6e65 2c20 7468 656e  o. If None, then
+00027870: 2073 6176 6573 2074 6865 2062 6c75 7272   saves the blurr
+00027880: 6564 2076 6964 656f 2069 6e20 7468 6520  ed video in the 
+00027890: 7361 6d65 2064 6972 6563 746f 7279 2061  same directory a
+000278a0: 7320 7468 6520 696e 7075 7420 7669 6465  s the input vide
+000278b0: 6f20 7769 7468 2074 6865 2060 605f 626c  o with the ``_bl
+000278c0: 7572 7265 6460 6020 7375 6666 6978 2e0a  urred`` suffix..
+000278d0: 2020 2020 3a72 6574 7572 6e3a 204e 6f6e      :return: Non
+000278e0: 650a 0a20 2020 203a 6578 616d 706c 653a  e..    :example:
+000278f0: 0a20 2020 203e 3e3e 2072 6f69 5f62 6c75  .    >>> roi_blu
+00027900: 7262 6f78 2876 6964 656f 5f70 6174 683d  rbox(video_path=
+00027910: 272f 5573 6572 732f 7369 6d6f 6e2f 446f  '/Users/simon/Do
+00027920: 776e 6c6f 6164 732f 315f 4c48 5f63 6c69  wnloads/1_LH_cli
+00027930: 7070 6564 5f64 6f77 6e73 616d 706c 6564  pped_downsampled
+00027940: 2e6d 7034 272c 2062 6c75 725f 6c65 7665  .mp4', blur_leve
+00027950: 6c3d 302e 322c 2069 6e76 6572 743d 5472  l=0.2, invert=Tr
+00027960: 7565 290a 2020 2020 2222 220a 0a20 2020  ue).    """..   
+00027970: 2063 6865 636b 5f66 666d 7065 675f 6176   check_ffmpeg_av
+00027980: 6169 6c61 626c 6528 7261 6973 655f 6572  ailable(raise_er
+00027990: 726f 723d 5472 7565 290a 2020 2020 7469  ror=True).    ti
+000279a0: 6d65 7220 3d20 5369 6d62 6154 696d 6572  mer = SimbaTimer
+000279b0: 2873 7461 7274 3d54 7275 6529 0a20 2020  (start=True).   
+000279c0: 2063 6865 636b 5f66 6c6f 6174 286e 616d   check_float(nam
+000279d0: 653d 6627 7b72 6f69 5f62 6c75 7262 6f78  e=f'{roi_blurbox
+000279e0: 2e5f 5f6e 616d 655f 5f7d 2062 6c75 725f  .__name__} blur_
+000279f0: 6c65 7665 6c27 2c20 7661 6c75 653d 626c  level', value=bl
+00027a00: 7572 5f6c 6576 656c 2c20 6d69 6e5f 7661  ur_level, min_va
+00027a10: 6c75 653d 302e 3030 312c 206d 6178 5f76  lue=0.001, max_v
+00027a20: 616c 7565 3d31 2e30 290a 2020 2020 6368  alue=1.0).    ch
+00027a30: 6563 6b5f 6669 6c65 5f65 7869 7374 5f61  eck_file_exist_a
+00027a40: 6e64 5f72 6561 6461 626c 6528 6669 6c65  nd_readable(file
+00027a50: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
+00027a60: 290a 2020 2020 6469 722c 2076 6964 656f  ).    dir, video
+00027a70: 5f6e 616d 652c 2065 7874 203d 2067 6574  _name, ext = get
+00027a80: 5f66 6e5f 6578 7428 7669 6465 6f5f 7061  _fn_ext(video_pa
+00027a90: 7468 290a 2020 2020 5f20 3d20 6765 745f  th).    _ = get_
+00027aa0: 7669 6465 6f5f 6d65 7461 5f64 6174 6128  video_meta_data(
+00027ab0: 7669 6465 6f5f 7061 7468 3d76 6964 656f  video_path=video
+00027ac0: 5f70 6174 6829 0a20 2020 2069 6620 7361  _path).    if sa
+00027ad0: 7665 5f70 6174 6820 6973 206e 6f74 204e  ve_path is not N
+00027ae0: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
+00027af0: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
+00027b00: 2869 6e5f 6469 723d 6f73 2e70 6174 682e  (in_dir=os.path.
+00027b10: 6469 726e 616d 6528 7361 7665 5f70 6174  dirname(save_pat
+00027b20: 6829 2c20 736f 7572 6365 3d72 6f69 5f62  h), source=roi_b
+00027b30: 6c75 7262 6f78 2e5f 5f6e 616d 655f 5f29  lurbox.__name__)
+00027b40: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00027b50: 2020 2073 6176 655f 7061 7468 203d 206f     save_path = o
+00027b60: 732e 7061 7468 2e6a 6f69 6e28 6469 722c  s.path.join(dir,
+00027b70: 2066 277b 7669 6465 6f5f 6e61 6d65 7d5f   f'{video_name}_
+00027b80: 626c 7572 7265 647b 6578 747d 2729 0a20  blurred{ext}'). 
+00027b90: 2020 2072 6f69 5f73 656c 6563 746f 7220     roi_selector 
+00027ba0: 3d20 524f 4953 656c 6563 746f 7228 7061  = ROISelector(pa
+00027bb0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+00027bc0: 2020 2072 6f69 5f73 656c 6563 746f 722e     roi_selector.
+00027bd0: 7275 6e28 290a 2020 2020 772c 2068 203d  run().    w, h =
+00027be0: 2072 6f69 5f73 656c 6563 746f 722e 7769   roi_selector.wi
+00027bf0: 6474 682c 2072 6f69 5f73 656c 6563 746f  dth, roi_selecto
+00027c00: 722e 6865 6967 6874 0a20 2020 2074 6f70  r.height.    top
+00027c10: 5f6c 6566 745f 782c 2074 6f70 5f6c 6566  _left_x, top_lef
+00027c20: 745f 7920 3d20 726f 695f 7365 6c65 6374  t_y = roi_select
+00027c30: 6f72 2e74 6f70 5f6c 6566 740a 2020 2020  or.top_left.    
+00027c40: 6d61 785f 626c 7572 5f76 616c 7565 203d  max_blur_value =
+00027c50: 2069 6e74 286d 696e 2877 2c20 6829 202f   int(min(w, h) /
+00027c60: 2032 2920 2f20 320a 2020 2020 626c 7572   2) / 2.    blur
+00027c70: 5f6c 6576 656c 203d 2069 6e74 286d 6178  _level = int(max
+00027c80: 5f62 6c75 725f 7661 6c75 6520 2a20 626c  _blur_value * bl
+00027c90: 7572 5f6c 6576 656c 290a 2020 2020 6966  ur_level).    if
+00027ca0: 206e 6f74 2069 6e76 6572 743a 0a20 2020   not invert:.   
+00027cb0: 2020 2020 2063 6d64 203d 2066 2766 666d       cmd = f'ffm
+00027cc0: 7065 6720 2d69 2022 7b76 6964 656f 5f70  peg -i "{video_p
+00027cd0: 6174 687d 2220 2d66 696c 7465 725f 636f  ath}" -filter_co
+00027ce0: 6d70 6c65 7820 225b 303a 765d 6372 6f70  mplex "[0:v]crop
+00027cf0: 3d7b 777d 3a7b 687d 3a7b 746f 705f 6c65  ={w}:{h}:{top_le
+00027d00: 6674 5f78 7d3a 7b74 6f70 5f6c 6566 745f  ft_x}:{top_left_
+00027d10: 797d 2c62 6f78 626c 7572 3d7b 696e 7428  y},boxblur={int(
+00027d20: 626c 7572 5f6c 6576 656c 297d 3a31 305b  blur_level)}:10[
+00027d30: 6667 5d3b 205b 303a 765d 5b66 675d 6f76  fg]; [0:v][fg]ov
+00027d40: 6572 6c61 793d 7b74 6f70 5f6c 6566 745f  erlay={top_left_
+00027d50: 787d 3a7b 746f 705f 6c65 6674 5f79 7d5b  x}:{top_left_y}[
+00027d60: 765d 2220 2d6d 6170 2022 5b76 5d22 2022  v]" -map "[v]" "
+00027d70: 7b73 6176 655f 7061 7468 7d22 202d 6c6f  {save_path}" -lo
+00027d80: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
+00027d90: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
+00027da0: 202d 7927 0a20 2020 2065 6c73 653a 0a20   -y'.    else:. 
+00027db0: 2020 2020 2020 2063 6d64 203d 2066 2766         cmd = f'f
+00027dc0: 666d 7065 6720 2d69 2022 7b76 6964 656f  fmpeg -i "{video
+00027dd0: 5f70 6174 687d 2220 2d66 696c 7465 725f  _path}" -filter_
+00027de0: 636f 6d70 6c65 7820 225b 303a 765d 626f  complex "[0:v]bo
+00027df0: 7862 6c75 723d 7b62 6c75 725f 6c65 7665  xblur={blur_leve
+00027e00: 6c7d 5b62 675d 3b5b 303a 765d 6372 6f70  l}[bg];[0:v]crop
+00027e10: 3d7b 777d 3a7b 687d 3a7b 746f 705f 6c65  ={w}:{h}:{top_le
+00027e20: 6674 5f78 7d3a 7b74 6f70 5f6c 6566 745f  ft_x}:{top_left_
+00027e30: 797d 5b66 675d 3b5b 6267 5d5b 6667 5d6f  y}[fg];[bg][fg]o
+00027e40: 7665 726c 6179 3d7b 746f 705f 6c65 6674  verlay={top_left
+00027e50: 5f78 7d3a 7b74 6f70 5f6c 6566 745f 797d  _x}:{top_left_y}
+00027e60: 2220 2d63 3a61 2063 6f70 7920 227b 7361  " -c:a copy "{sa
+00027e70: 7665 5f70 6174 687d 2220 2d6c 6f67 6c65  ve_path}" -logle
+00027e80: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
+00027e90: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
+00027ea0: 270a 2020 2020 7375 6270 726f 6365 7373  '.    subprocess
+00027eb0: 2e63 616c 6c28 636d 642c 2073 6865 6c6c  .call(cmd, shell
+00027ec0: 3d54 7275 652c 2073 7464 6f75 743d 7375  =True, stdout=su
+00027ed0: 6270 726f 6365 7373 2e50 4950 4529 0a20  bprocess.PIPE). 
+00027ee0: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
+00027ef0: 6d65 7228 290a 2020 2020 7374 646f 7574  mer().    stdout
+00027f00: 5f73 7563 6365 7373 286d 7367 3d66 2742  _success(msg=f'B
+00027f10: 6c75 7272 6564 207b 7669 6465 6f5f 6e61  lurred {video_na
+00027f20: 6d65 7d20 7669 6465 6f20 7361 7665 6420  me} video saved 
+00027f30: 696e 207b 7361 7665 5f70 6174 687d 272c  in {save_path}',
+00027f40: 2065 6c61 7073 6564 5f74 696d 653d 7469   elapsed_time=ti
+00027f50: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
+00027f60: 5f73 7472 290a 0a0a 6465 6620 7375 7065  _str)...def supe
+00027f70: 7269 6d70 6f73 655f 656c 6170 7365 645f  rimpose_elapsed_
+00027f80: 7469 6d65 2876 6964 656f 5f70 6174 683a  time(video_path:
+00027f90: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00027fa0: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
+00027fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fc0: 2020 2020 2020 2066 6f6e 745f 7369 7a65         font_size
+00027fd0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00027fe0: 3d20 3330 2c0a 2020 2020 2020 2020 2020  = 30,.          
+00027ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028000: 2020 2066 6f6e 745f 636f 6c6f 723a 204f     font_color: O
+00028010: 7074 696f 6e61 6c5b 7374 725d 203d 2027  ptional[str] = '
+00028020: 7768 6974 6527 2c0a 2020 2020 2020 2020  white',.        
+00028030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028040: 2020 2020 2066 6f6e 745f 626f 7264 6572       font_border
+00028050: 5f63 6f6c 6f72 3a20 4f70 7469 6f6e 616c  _color: Optional
+00028060: 5b73 7472 5d20 3d20 2762 6c61 636b 272c  [str] = 'black',
+00028070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028080: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00028090: 6e74 5f62 6f72 6465 725f 7769 6474 683a  nt_border_width:
+000280a0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000280b0: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+000280c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000280d0: 2070 6f73 6974 696f 6e3a 204f 7074 696f   position: Optio
+000280e0: 6e61 6c5b 4c69 7465 7261 6c5b 2774 6f70  nal[Literal['top
+000280f0: 5f6c 6566 7427 2c20 2774 6f70 5f72 6967  _left', 'top_rig
+00028100: 6874 272c 2027 626f 7474 6f6d 5f6c 6566  ht', 'bottom_lef
+00028110: 7427 2c20 2762 6f74 746f 6d5f 7269 6768  t', 'bottom_righ
+00028120: 7427 2c20 276d 6964 646c 655f 746f 7027  t', 'middle_top'
+00028130: 2c20 276d 6964 646c 655f 626f 7474 6f6d  , 'middle_bottom
+00028140: 275d 5d20 3d20 2774 6f70 5f6c 6566 7427  ']] = 'top_left'
+00028150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00028160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00028170: 6176 655f 6469 723a 204f 7074 696f 6e61  ave_dir: Optiona
+00028180: 6c5b 556e 696f 6e5b 7374 722c 206f 732e  l[Union[str, os.
+00028190: 5061 7468 4c69 6b65 5d5d 203d 204e 6f6e  PathLike]] = Non
+000281a0: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+000281b0: 2222 220a 2020 2020 5375 7065 7269 6d70  """.    Superimp
+000281c0: 6f73 6573 2065 6c61 7073 6564 2074 696d  oses elapsed tim
+000281d0: 6520 6f6e 2074 6865 2067 6976 656e 2076  e on the given v
+000281e0: 6964 656f 2066 696c 6528 7329 2061 6e64  ideo file(s) and
+000281f0: 2073 6176 6573 2074 6865 206d 6f64 6966   saves the modif
+00028200: 6965 6420 7669 6465 6f28 7329 2e0a 0a20  ied video(s)... 
+00028210: 2020 202e 2e20 7669 6465 6f3a 3a20 5f73     .. video:: _s
+00028220: 7461 7469 632f 696d 672f 7375 7065 7269  tatic/img/superi
+00028230: 6d70 6f73 655f 656c 6170 7365 645f 7469  mpose_elapsed_ti
+00028240: 6d65 2e77 6562 6d0a 2020 2020 2020 203a  me.webm.       :
+00028250: 7769 6474 683a 2039 3030 0a20 2020 2020  width: 900.     
+00028260: 2020 3a6c 6f6f 703a 0a0a 2020 2020 3a70    :loop:..    :p
+00028270: 6172 616d 2055 6e69 6f6e 5b73 7472 2c20  aram Union[str, 
+00028280: 6f73 2e50 6174 684c 696b 655d 2076 6964  os.PathLike] vid
+00028290: 656f 5f70 6174 683a 2050 6174 6820 746f  eo_path: Path to
+000282a0: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
+000282b0: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
+000282c0: 7279 2063 6f6e 7461 696e 696e 6720 7669  ry containing vi
+000282d0: 6465 6f20 6669 6c65 732e 0a20 2020 203a  deo files..    :
+000282e0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
+000282f0: 6e74 5d20 666f 6e74 5f73 697a 653a 2046  nt] font_size: F
+00028300: 6f6e 7420 7369 7a65 2066 6f72 2074 6865  ont size for the
+00028310: 2065 6c61 7073 6564 2074 696d 6520 7465   elapsed time te
+00028320: 7874 2e20 4465 6661 756c 7420 3330 2e0a  xt. Default 30..
+00028330: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00028340: 6e61 6c5b 7374 725d 2066 6f6e 745f 636f  nal[str] font_co
+00028350: 6c6f 723a 2020 466f 6e74 2063 6f6c 6f72  lor:  Font color
+00028360: 2066 6f72 2074 6865 2065 6c61 7073 6564   for the elapsed
+00028370: 2074 696d 6520 7465 7874 2e20 4465 6661   time text. Defa
+00028380: 756c 7420 7768 6974 650a 2020 2020 3a70  ult white.    :p
+00028390: 6172 616d 204f 7074 696f 6e61 6c5b 7374  aram Optional[st
+000283a0: 725d 2066 6f6e 745f 626f 7264 6572 5f63  r] font_border_c
+000283b0: 6f6c 6f72 3a20 466f 6e74 2062 6f72 6465  olor: Font borde
+000283c0: 7220 636f 6c6f 7220 666f 7220 7468 6520  r color for the 
+000283d0: 656c 6170 7365 6420 7469 6d65 2074 6578  elapsed time tex
+000283e0: 742e 2044 6566 6175 6c74 2062 6c61 636b  t. Default black
+000283f0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00028400: 696f 6e61 6c5b 696e 745d 2066 6f6e 745f  ional[int] font_
+00028410: 626f 7264 6572 5f77 6964 7468 3a20 466f  border_width: Fo
+00028420: 6e74 2062 6f72 6465 7220 7769 6474 6820  nt border width 
+00028430: 666f 7220 7468 6520 656c 6170 7365 6420  for the elapsed 
+00028440: 7469 6d65 2074 6578 7420 696e 2070 6978  time text in pix
+00028450: 656c 732e 2044 6566 6175 6c74 2032 2e0a  els. Default 2..
+00028460: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+00028470: 6e61 6c5b 4c69 7465 7261 6c5b 2774 6f70  nal[Literal['top
+00028480: 5f6c 6566 7427 2c20 2774 6f70 5f72 6967  _left', 'top_rig
+00028490: 6874 272c 2027 626f 7474 6f6d 5f6c 6566  ht', 'bottom_lef
+000284a0: 7427 2c20 2762 6f74 746f 6d5f 7269 6768  t', 'bottom_righ
+000284b0: 7427 2c20 276d 6964 646c 655f 746f 7027  t', 'middle_top'
+000284c0: 2c20 276d 6964 646c 655f 626f 7474 6f6d  , 'middle_bottom
+000284d0: 275d 5d20 706f 7369 7469 6f6e 3a20 506f  ']] position: Po
+000284e0: 7369 7469 6f6e 2077 6865 7265 2074 6865  sition where the
+000284f0: 2065 6c61 7073 6564 2074 696d 6520 7465   elapsed time te
+00028500: 7874 2077 696c 6c20 6265 2073 7570 6572  xt will be super
+00028510: 696d 706f 7365 642e 2044 6566 6175 6c74  imposed. Default
+00028520: 2060 6074 6f70 5f6c 6566 7460 602e 0a20   ``top_left``.. 
+00028530: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+00028540: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+00028550: 2e50 6174 684c 696b 655d 5d20 7361 7665  .PathLike]] save
+00028560: 5f64 6972 3a20 4469 7265 6374 6f72 7920  _dir: Directory 
+00028570: 7768 6572 6520 7468 6520 6d6f 6469 6669  where the modifi
+00028580: 6564 2076 6964 656f 2873 2920 7769 6c6c  ed video(s) will
+00028590: 2062 6520 7361 7665 642e 2049 6620 6e6f   be saved. If no
+000285a0: 7420 7072 6f76 6964 6564 2c20 7468 6520  t provided, the 
+000285b0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+000285c0: 2069 6e70 7574 2076 6964 656f 2873 2920   input video(s) 
+000285d0: 7769 6c6c 2062 6520 7573 6564 2e0a 2020  will be used..  
+000285e0: 2020 3a72 6574 7572 6e3a 204e 6f6e 650a    :return: None.
+000285f0: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+00028600: 2020 203e 3e3e 2073 7570 6572 696d 706f     >>> superimpo
+00028610: 7365 5f65 6c61 7073 6564 5f74 696d 6528  se_elapsed_time(
+00028620: 7669 6465 6f5f 7061 7468 3d27 2f55 7365  video_path='/Use
+00028630: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+00028640: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+00028650: 626c 6573 686f 6f74 696e 672f 6d6f 7573  bleshooting/mous
+00028660: 655f 6f70 656e 5f66 6965 6c64 2f70 726f  e_open_field/pro
+00028670: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+00028680: 6f73 2f74 6573 745f 342f 312e 6d70 3427  os/test_4/1.mp4'
+00028690: 2c20 706f 7369 7469 6f6e 3d27 6d69 6464  , position='midd
+000286a0: 6c65 5f74 6f70 272c 2066 6f6e 745f 636f  le_top', font_co
+000286b0: 6c6f 723d 2762 6c61 636b 272c 2066 6f6e  lor='black', fon
+000286c0: 745f 626f 7264 6572 5f63 6f6c 6f72 3d27  t_border_color='
+000286d0: 7069 6e6b 272c 2066 6f6e 745f 626f 7264  pink', font_bord
+000286e0: 6572 5f77 6964 7468 3d35 2c20 666f 6e74  er_width=5, font
+000286f0: 5f73 697a 653d 3330 290a 2020 2020 2222  _size=30).    ""
+00028700: 220a 0a20 2020 2063 6865 636b 5f66 666d  "..    check_ffm
+00028710: 7065 675f 6176 6169 6c61 626c 6528 7261  peg_available(ra
+00028720: 6973 655f 6572 726f 723d 5472 7565 290a  ise_error=True).
+00028730: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
+00028740: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
+00028750: 6529 0a20 2020 2050 4f53 4954 494f 4e53  e).    POSITIONS
+00028760: 203d 205b 2774 6f70 5f6c 6566 7427 2c20   = ['top_left', 
+00028770: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
+00028780: 7474 6f6d 5f6c 6566 7427 2c20 2762 6f74  ttom_left', 'bot
+00028790: 746f 6d5f 7269 6768 7427 2c20 2774 6f70  tom_right', 'top
+000287a0: 5f6d 6964 646c 6527 2c20 2762 6f74 746f  _middle', 'botto
+000287b0: 6d5f 6d69 6464 6c65 275d 0a20 2020 2063  m_middle'].    c
+000287c0: 6865 636b 5f73 7472 286e 616d 653d 6627  heck_str(name=f'
+000287d0: 7b73 7570 6572 696d 706f 7365 5f65 6c61  {superimpose_ela
+000287e0: 7073 6564 5f74 696d 652e 5f5f 6e61 6d65  psed_time.__name
+000287f0: 5f5f 7d20 706f 7369 7469 6f6e 272c 2076  __} position', v
+00028800: 616c 7565 3d70 6f73 6974 696f 6e2c 206f  alue=position, o
+00028810: 7074 696f 6e73 3d50 4f53 4954 494f 4e53  ptions=POSITIONS
+00028820: 290a 2020 2020 6368 6563 6b5f 696e 7428  ).    check_int(
+00028830: 6e61 6d65 3d66 277b 7375 7065 7269 6d70  name=f'{superimp
+00028840: 6f73 655f 656c 6170 7365 645f 7469 6d65  ose_elapsed_time
+00028850: 2e5f 5f6e 616d 655f 5f7d 2066 6f6e 745f  .__name__} font_
+00028860: 7369 7a65 272c 2076 616c 7565 3d66 6f6e  size', value=fon
+00028870: 745f 7369 7a65 2c20 6d69 6e5f 7661 6c75  t_size, min_valu
+00028880: 653d 3129 0a20 2020 2063 6865 636b 5f69  e=1).    check_i
+00028890: 6e74 286e 616d 653d 6627 7b73 7570 6572  nt(name=f'{super
+000288a0: 696d 706f 7365 5f65 6c61 7073 6564 5f74  impose_elapsed_t
+000288b0: 696d 652e 5f5f 6e61 6d65 5f5f 7d20 666f  ime.__name__} fo
+000288c0: 6e74 5f62 6f72 6465 725f 7769 6474 6827  nt_border_width'
+000288d0: 2c20 7661 6c75 653d 666f 6e74 5f62 6f72  , value=font_bor
+000288e0: 6465 725f 7769 6474 682c 206d 696e 5f76  der_width, min_v
+000288f0: 616c 7565 3d31 290a 2020 2020 666f 6e74  alue=1).    font
+00028900: 5f63 6f6c 6f72 203d 2027 272e 6a6f 696e  _color = ''.join
+00028910: 2866 696c 7465 7228 7374 722e 6973 616c  (filter(str.isal
+00028920: 6e75 6d2c 2066 6f6e 745f 636f 6c6f 7229  num, font_color)
+00028930: 292e 6c6f 7765 7228 290a 2020 2020 666f  ).lower().    fo
+00028940: 6e74 5f62 6f72 6465 725f 636f 6c6f 7220  nt_border_color 
+00028950: 3d20 2727 2e6a 6f69 6e28 6669 6c74 6572  = ''.join(filter
+00028960: 2873 7472 2e69 7361 6c6e 756d 2c20 666f  (str.isalnum, fo
+00028970: 6e74 5f62 6f72 6465 725f 636f 6c6f 7229  nt_border_color)
+00028980: 292e 6c6f 7765 7228 290a 2020 2020 6966  ).lower().    if
+00028990: 206f 732e 7061 7468 2e69 7366 696c 6528   os.path.isfile(
+000289a0: 7669 6465 6f5f 7061 7468 293a 0a20 2020  video_path):.   
+000289b0: 2020 2020 2076 6964 656f 5f70 6174 6873       video_paths
+000289c0: 203d 205b 7669 6465 6f5f 7061 7468 5d0a   = [video_path].
+000289d0: 2020 2020 656c 6966 206f 732e 7061 7468      elif os.path
+000289e0: 2e69 7364 6972 2876 6964 656f 5f70 6174  .isdir(video_pat
+000289f0: 6829 3a0a 2020 2020 2020 2020 7669 6465  h):.        vide
+00028a00: 6f5f 7061 7468 7320 3d20 6c69 7374 2866  o_paths = list(f
+00028a10: 696e 645f 616c 6c5f 7669 6465 6f73 5f69  ind_all_videos_i
+00028a20: 6e5f 6469 7265 6374 6f72 7928 6469 7265  n_directory(dire
+00028a30: 6374 6f72 793d 7669 6465 6f5f 7061 7468  ctory=video_path
+00028a40: 2c20 6173 5f64 6963 743d 5472 7565 2c20  , as_dict=True, 
+00028a50: 7261 6973 655f 6572 726f 723d 5472 7565  raise_error=True
+00028a60: 292e 7661 6c75 6573 2829 290a 2020 2020  ).values()).    
+00028a70: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
+00028a80: 6973 6520 496e 7661 6c69 6449 6e70 7574  ise InvalidInput
+00028a90: 4572 726f 7228 6d73 673d 6627 7b76 6964  Error(msg=f'{vid
+00028aa0: 656f 5f70 6174 687d 2069 7320 6e6f 7420  eo_path} is not 
+00028ab0: 6120 7661 6c69 6420 6669 6c65 2070 6174  a valid file pat
+00028ac0: 6820 6f72 2061 2076 616c 6964 2064 6972  h or a valid dir
+00028ad0: 6563 746f 7279 2070 6174 6827 2c0a 2020  ectory path',.  
+00028ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028af0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00028b00: 7572 6365 3d73 7570 6572 696d 706f 7365  urce=superimpose
+00028b10: 5f65 6c61 7073 6564 5f74 696d 652e 5f5f  _elapsed_time.__
+00028b20: 6e61 6d65 5f5f 290a 2020 2020 6966 2073  name__).    if s
+00028b30: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
+00028b40: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
+00028b50: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
+00028b60: 2869 6e5f 6469 723d 7361 7665 5f64 6972  (in_dir=save_dir
+00028b70: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00028b80: 2020 2020 7361 7665 5f64 6972 203d 206f      save_dir = o
+00028b90: 732e 7061 7468 2e64 6972 6e61 6d65 2876  s.path.dirname(v
+00028ba0: 6964 656f 5f70 6174 6873 5b30 5d29 0a20  ideo_paths[0]). 
+00028bb0: 2020 2066 6f72 2066 696c 655f 636e 742c     for file_cnt,
+00028bc0: 2076 6964 656f 5f70 6174 6820 696e 2065   video_path in e
+00028bd0: 6e75 6d65 7261 7465 2876 6964 656f 5f70  numerate(video_p
+00028be0: 6174 6873 293a 0a20 2020 2020 2020 205f  aths):.        _
+00028bf0: 2c20 7669 6465 6f5f 6e61 6d65 2c20 6578  , video_name, ex
+00028c00: 7420 3d20 6765 745f 666e 5f65 7874 2876  t = get_fn_ext(v
+00028c10: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
+00028c20: 2020 2070 7269 6e74 2866 2753 7570 6572     print(f'Super
+00028c30: 696d 706f 7369 6e67 2074 696d 6520 7b76  imposing time {v
+00028c40: 6964 656f 5f6e 616d 657d 2028 5669 6465  ideo_name} (Vide
+00028c50: 6f20 7b66 696c 655f 636e 7420 2b20 317d  o {file_cnt + 1}
+00028c60: 2f7b 6c65 6e28 7669 6465 6f5f 7061 7468  /{len(video_path
+00028c70: 7329 7d29 2e2e 2e27 290a 2020 2020 2020  s)})...').      
+00028c80: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
+00028c90: 2e70 6174 682e 6a6f 696e 2873 6176 655f  .path.join(save_
+00028ca0: 6469 722c 2066 277b 7669 6465 6f5f 6e61  dir, f'{video_na
+00028cb0: 6d65 7d5f 7469 6d65 5f73 7570 6572 696d  me}_time_superim
+00028cc0: 706f 7365 647b 6578 747d 2729 0a20 2020  posed{ext}').   
+00028cd0: 2020 2020 2069 6620 706f 7369 7469 6f6e       if position
+00028ce0: 203d 3d20 504f 5349 5449 4f4e 535b 305d   == POSITIONS[0]
+00028cf0: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00028d00: 6420 3d20 6622 6666 6d70 6567 202d 6920  d = f"ffmpeg -i 
+00028d10: 277b 7669 6465 6f5f 7061 7468 7d27 202d  '{video_path}' -
+00028d20: 7666 205c 2264 7261 7774 6578 743d 666f  vf \"drawtext=fo
+00028d30: 6e74 6669 6c65 3d41 7269 616c 2e74 7466  ntfile=Arial.ttf
+00028d40: 3a74 6578 743d 2725 7b7b 7074 735c 3a68  :text='%{{pts\:h
+00028d50: 6d73 7d7d 2e25 7b7b 6569 665c 3a6d 6f64  ms}}.%{{eif\:mod
+00028d60: 286e 5c5c 2c31 3030 3029 5c5c 3a64 5c5c  (n\\,1000)\\:d\\
+00028d70: 3a33 7d7d 273a 783d 353a 793d 353a 666f  :3}}':x=5:y=5:fo
+00028d80: 6e74 7369 7a65 3d7b 666f 6e74 5f73 697a  ntsize={font_siz
+00028d90: 657d 3a66 6f6e 7463 6f6c 6f72 3d7b 666f  e}:fontcolor={fo
+00028da0: 6e74 5f63 6f6c 6f72 7d3a 626f 7264 6572  nt_color}:border
+00028db0: 773d 7b66 6f6e 745f 626f 7264 6572 5f77  w={font_border_w
+00028dc0: 6964 7468 7d3a 626f 7264 6572 636f 6c6f  idth}:bordercolo
+00028dd0: 723d 7b66 6f6e 745f 626f 7264 6572 5f63  r={font_border_c
+00028de0: 6f6c 6f72 7d5c 2220 2d63 3a61 2063 6f70  olor}\" -c:a cop
+00028df0: 7920 277b 7361 7665 5f70 6174 687d 2720  y '{save_path}' 
+00028e00: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
+00028e10: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
+00028e20: 6e65 7220 2d79 220a 2020 2020 2020 2020  ner -y".        
+00028e30: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
+00028e40: 2050 4f53 4954 494f 4e53 5b31 5d3a 0a20   POSITIONS[1]:. 
+00028e50: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00028e60: 2066 2266 666d 7065 6720 2d69 2027 7b76   f"ffmpeg -i '{v
+00028e70: 6964 656f 5f70 6174 687d 2720 2d76 6620  ideo_path}' -vf 
+00028e80: 5c22 6472 6177 7465 7874 3d66 6f6e 7466  \"drawtext=fontf
+00028e90: 696c 653d 4172 6961 6c2e 7474 663a 7465  ile=Arial.ttf:te
+00028ea0: 7874 3d27 257b 7b70 7473 5c3a 686d 737d  xt='%{{pts\:hms}
+00028eb0: 7d2e 257b 7b65 6966 5c3a 6d6f 6428 6e5c  }.%{{eif\:mod(n\
+00028ec0: 5c2c 3130 3030 295c 5c3a 645c 5c3a 337d  \,1000)\\:d\\:3}
+00028ed0: 7d27 3a78 3d28 772d 7477 2d35 293a 793d  }':x=(w-tw-5):y=
+00028ee0: 353a 666f 6e74 7369 7a65 3d7b 666f 6e74  5:fontsize={font
+00028ef0: 5f73 697a 657d 3a66 6f6e 7463 6f6c 6f72  _size}:fontcolor
+00028f00: 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a 626f  ={font_color}:bo
+00028f10: 7264 6572 773d 7b66 6f6e 745f 626f 7264  rderw={font_bord
+00028f20: 6572 5f77 6964 7468 7d3a 626f 7264 6572  er_width}:border
+00028f30: 636f 6c6f 723d 7b66 6f6e 745f 626f 7264  color={font_bord
+00028f40: 6572 5f63 6f6c 6f72 7d5c 2220 2d63 3a61  er_color}\" -c:a
+00028f50: 2063 6f70 7920 277b 7361 7665 5f70 6174   copy '{save_pat
+00028f60: 687d 2720 2d6c 6f67 6c65 7665 6c20 6572  h}' -loglevel er
+00028f70: 726f 7220 2d73 7461 7473 202d 6869 6465  ror -stats -hide
+00028f80: 5f62 616e 6e65 7220 2d79 220a 2020 2020  _banner -y".    
+00028f90: 2020 2020 656c 6966 2070 6f73 6974 696f      elif positio
+00028fa0: 6e20 3d3d 2050 4f53 4954 494f 4e53 5b32  n == POSITIONS[2
+00028fb0: 5d3a 0a20 2020 2020 2020 2020 2020 2063  ]:.            c
+00028fc0: 6d64 203d 2066 2266 666d 7065 6720 2d69  md = f"ffmpeg -i
+00028fd0: 2027 7b76 6964 656f 5f70 6174 687d 2720   '{video_path}' 
+00028fe0: 2d76 6620 5c22 6472 6177 7465 7874 3d66  -vf \"drawtext=f
+00028ff0: 6f6e 7466 696c 653d 4172 6961 6c2e 7474  ontfile=Arial.tt
+00029000: 663a 7465 7874 3d27 257b 7b70 7473 5c3a  f:text='%{{pts\:
+00029010: 686d 737d 7d2e 257b 7b65 6966 5c3a 6d6f  hms}}.%{{eif\:mo
+00029020: 6428 6e5c 5c2c 3130 3030 295c 5c3a 645c  d(n\\,1000)\\:d\
+00029030: 5c3a 337d 7d27 3a78 3d35 3a79 3d28 682d  \:3}}':x=5:y=(h-
+00029040: 7468 2d35 293a 666f 6e74 7369 7a65 3d7b  th-5):fontsize={
+00029050: 666f 6e74 5f73 697a 657d 3a66 6f6e 7463  font_size}:fontc
+00029060: 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c 6f72  olor={font_color
+00029070: 7d3a 626f 7264 6572 773d 7b66 6f6e 745f  }:borderw={font_
+00029080: 626f 7264 6572 5f77 6964 7468 7d3a 626f  border_width}:bo
+00029090: 7264 6572 636f 6c6f 723d 7b66 6f6e 745f  rdercolor={font_
+000290a0: 626f 7264 6572 5f63 6f6c 6f72 7d5c 2220  border_color}\" 
+000290b0: 2d63 3a61 2063 6f70 7920 277b 7361 7665  -c:a copy '{save
+000290c0: 5f70 6174 687d 2720 2d6c 6f67 6c65 7665  _path}' -logleve
+000290d0: 6c20 6572 726f 7220 2d73 7461 7473 202d  l error -stats -
+000290e0: 6869 6465 5f62 616e 6e65 7220 2d79 220a  hide_banner -y".
+000290f0: 2020 2020 2020 2020 656c 6966 2070 6f73          elif pos
+00029100: 6974 696f 6e20 3d3d 2050 4f53 4954 494f  ition == POSITIO
+00029110: 4e53 5b33 5d3a 0a20 2020 2020 2020 2020  NS[3]:.         
+00029120: 2020 2063 6d64 203d 2066 2266 666d 7065     cmd = f"ffmpe
+00029130: 6720 2d69 2027 7b76 6964 656f 5f70 6174  g -i '{video_pat
+00029140: 687d 2720 2d76 6620 5c22 6472 6177 7465  h}' -vf \"drawte
+00029150: 7874 3d66 6f6e 7466 696c 653d 4172 6961  xt=fontfile=Aria
+00029160: 6c2e 7474 663a 7465 7874 3d27 257b 7b70  l.ttf:text='%{{p
+00029170: 7473 5c3a 686d 737d 7d2e 257b 7b65 6966  ts\:hms}}.%{{eif
+00029180: 5c3a 6d6f 6428 6e5c 5c2c 3130 3030 295c  \:mod(n\\,1000)\
+00029190: 5c3a 645c 5c3a 337d 7d27 3a78 3d28 772d  \:d\\:3}}':x=(w-
+000291a0: 7477 2d35 293a 793d 2868 2d74 682d 3529  tw-5):y=(h-th-5)
+000291b0: 3a66 6f6e 7473 697a 653d 7b66 6f6e 745f  :fontsize={font_
+000291c0: 7369 7a65 7d3a 666f 6e74 636f 6c6f 723d  size}:fontcolor=
+000291d0: 7b66 6f6e 745f 636f 6c6f 727d 3a62 6f72  {font_color}:bor
+000291e0: 6465 7277 3d7b 666f 6e74 5f62 6f72 6465  derw={font_borde
+000291f0: 725f 7769 6474 687d 3a62 6f72 6465 7263  r_width}:borderc
+00029200: 6f6c 6f72 3d7b 666f 6e74 5f62 6f72 6465  olor={font_borde
+00029210: 725f 636f 6c6f 727d 5c22 202d 633a 6120  r_color}\" -c:a 
+00029220: 636f 7079 2027 7b73 6176 655f 7061 7468  copy '{save_path
+00029230: 7d27 202d 6c6f 676c 6576 656c 2065 7272  }' -loglevel err
+00029240: 6f72 202d 7374 6174 7320 2d68 6964 655f  or -stats -hide_
+00029250: 6261 6e6e 6572 202d 7922 0a20 2020 2020  banner -y".     
+00029260: 2020 2065 6c69 6620 706f 7369 7469 6f6e     elif position
+00029270: 203d 3d20 504f 5349 5449 4f4e 535b 345d   == POSITIONS[4]
+00029280: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00029290: 6420 3d20 6622 6666 6d70 6567 202d 6920  d = f"ffmpeg -i 
+000292a0: 277b 7669 6465 6f5f 7061 7468 7d27 202d  '{video_path}' -
+000292b0: 7666 205c 2264 7261 7774 6578 743d 666f  vf \"drawtext=fo
+000292c0: 6e74 6669 6c65 3d41 7269 616c 2e74 7466  ntfile=Arial.ttf
+000292d0: 3a74 6578 743d 2725 7b7b 7074 735c 3a68  :text='%{{pts\:h
+000292e0: 6d73 7d7d 2e25 7b7b 6569 665c 3a6d 6f64  ms}}.%{{eif\:mod
+000292f0: 286e 5c5c 2c31 3030 3029 5c5c 3a64 5c5c  (n\\,1000)\\:d\\
+00029300: 3a33 7d7d 273a 783d 2877 2d74 7729 2f32  :3}}':x=(w-tw)/2
+00029310: 3a79 3d31 303a 666f 6e74 7369 7a65 3d7b  :y=10:fontsize={
+00029320: 666f 6e74 5f73 697a 657d 3a66 6f6e 7463  font_size}:fontc
+00029330: 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c 6f72  olor={font_color
+00029340: 7d3a 626f 7264 6572 773d 7b66 6f6e 745f  }:borderw={font_
+00029350: 626f 7264 6572 5f77 6964 7468 7d3a 626f  border_width}:bo
+00029360: 7264 6572 636f 6c6f 723d 7b66 6f6e 745f  rdercolor={font_
+00029370: 626f 7264 6572 5f63 6f6c 6f72 7d5c 2220  border_color}\" 
+00029380: 2d63 3a61 2063 6f70 7920 277b 7361 7665  -c:a copy '{save
+00029390: 5f70 6174 687d 2720 2d6c 6f67 6c65 7665  _path}' -logleve
+000293a0: 6c20 6572 726f 7220 2d73 7461 7473 202d  l error -stats -
+000293b0: 6869 6465 5f62 616e 6e65 7220 2d79 220a  hide_banner -y".
+000293c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000293d0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+000293e0: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
+000293f0: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
+00029400: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
+00029410: 6c65 3d41 7269 616c 2e74 7466 3a74 6578  le=Arial.ttf:tex
+00029420: 743d 2725 7b7b 7074 735c 3a68 6d73 7d7d  t='%{{pts\:hms}}
+00029430: 2e25 7b7b 6569 665c 3a6d 6f64 286e 5c5c  .%{{eif\:mod(n\\
+00029440: 2c31 3030 3029 5c5c 3a64 5c5c 3a33 7d7d  ,1000)\\:d\\:3}}
+00029450: 273a 783d 2877 2d74 7729 2f32 3a79 3d28  ':x=(w-tw)/2:y=(
+00029460: 682d 7468 2d31 3029 3a66 6f6e 7473 697a  h-th-10):fontsiz
+00029470: 653d 7b66 6f6e 745f 7369 7a65 7d3a 666f  e={font_size}:fo
+00029480: 6e74 636f 6c6f 723d 7b66 6f6e 745f 636f  ntcolor={font_co
+00029490: 6c6f 727d 3a62 6f72 6465 7277 3d7b 666f  lor}:borderw={fo
+000294a0: 6e74 5f62 6f72 6465 725f 7769 6474 687d  nt_border_width}
+000294b0: 3a62 6f72 6465 7263 6f6c 6f72 3d7b 666f  :bordercolor={fo
+000294c0: 6e74 5f62 6f72 6465 725f 636f 6c6f 727d  nt_border_color}
+000294d0: 5c22 202d 633a 6120 636f 7079 2027 7b73  \" -c:a copy '{s
+000294e0: 6176 655f 7061 7468 7d27 202d 6c6f 676c  ave_path}' -logl
+000294f0: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
+00029500: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
+00029510: 7922 0a20 2020 2020 2020 2073 7562 7072  y".        subpr
+00029520: 6f63 6573 732e 6361 6c6c 2863 6d64 2c20  ocess.call(cmd, 
+00029530: 7368 656c 6c3d 5472 7565 2c20 7374 646f  shell=True, stdo
+00029540: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
+00029550: 5045 290a 2020 2020 7469 6d65 722e 7374  PE).    timer.st
+00029560: 6f70 5f74 696d 6572 2829 0a20 2020 2073  op_timer().    s
+00029570: 7464 6f75 745f 7375 6363 6573 7328 6d73  tdout_success(ms
+00029580: 673d 6627 5375 7065 722d 696d 706f 7365  g=f'Super-impose
+00029590: 6420 7469 6d65 206f 6e20 7b6c 656e 2876  d time on {len(v
+000295a0: 6964 656f 5f70 6174 6873 297d 2076 6964  ideo_paths)} vid
+000295b0: 656f 2873 292c 2073 6176 6564 2069 6e20  eo(s), saved in 
+000295c0: 7b73 6176 655f 6469 727d 272c 2065 6c61  {save_dir}', ela
+000295d0: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
+000295e0: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
+000295f0: 290a 0a0a 6465 6620 7669 6465 6f5f 746f  )...def video_to
+00029600: 5f62 7728 7669 6465 6f5f 7061 7468 3a20  _bw(video_path: 
+00029610: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00029620: 7468 4c69 6b65 5d2c 0a20 2020 2020 2020  thLike],.       
+00029630: 2020 2020 2020 2020 2074 6872 6573 686f           thresho
+00029640: 6c64 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ld: Optional[flo
+00029650: 6174 5d20 3d20 302e 3529 202d 3e20 4e6f  at] = 0.5) -> No
+00029660: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
+00029670: 436f 6e76 6572 7420 7669 6465 6f20 746f  Convert video to
+00029680: 2062 6c61 636b 2061 6e64 2077 6869 7465   black and white
+00029690: 2075 7369 6e67 2070 6173 7365 6420 7468   using passed th
+000296a0: 7265 7368 6f6c 642e 0a0a 2020 2020 2e2e  reshold...    ..
+000296b0: 2076 6964 656f 3a3a 205f 7374 6174 6963   video:: _static
+000296c0: 2f69 6d67 2f76 6964 656f 5f74 6f5f 6277  /img/video_to_bw
+000296d0: 2e77 6562 6d0a 2020 2020 2020 203a 6c6f  .webm.       :lo
+000296e0: 6f70 3a0a 0a20 2020 203a 7061 7261 6d20  op:..    :param 
+000296f0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
+00029700: 7468 4c69 6b65 5d20 7669 6465 6f5f 7061  thLike] video_pa
+00029710: 7468 3a20 5061 7468 2074 6f20 7468 6520  th: Path to the 
+00029720: 7669 6465 6f0a 2020 2020 3a70 6172 616d  video.    :param
+00029730: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00029740: 2074 6872 6573 686f 6c64 3a20 5661 6c75   threshold: Valu
+00029750: 6520 6265 7477 6565 6e20 3020 616e 6420  e between 0 and 
+00029760: 312e 204c 6f77 6572 2076 616c 7565 7320  1. Lower values 
+00029770: 6769 7665 7320 6d6f 7265 2077 6869 7465  gives more white
+00029780: 2061 6e64 2076 6963 6520 7665 7273 612e   and vice versa.
+00029790: 0a20 2020 203a 7265 7475 726e 3a20 4e6f  .    :return: No
+000297a0: 6e65 2e0a 0a20 2020 203a 6578 616d 706c  ne...    :exampl
+000297b0: 653a 0a20 2020 203e 3e3e 2076 6964 656f  e:.    >>> video
+000297c0: 5f74 6f5f 6277 2876 6964 656f 5f70 6174  _to_bw(video_pat
+000297d0: 683d 272f 5573 6572 732f 7369 6d6f 6e2f  h='/Users/simon/
+000297e0: 446f 776e 6c6f 6164 732f 315f 4c48 5f63  Downloads/1_LH_c
+000297f0: 6c69 7070 6564 5f63 726f 7070 6564 5f65  lipped_cropped_e
+00029800: 715f 3230 3234 3035 3135 3133 3539 3236  q_20240515135926
+00029810: 2e6d 7034 272c 2074 6872 6573 686f 6c64  .mp4', threshold
+00029820: 3d30 2e30 3229 0a20 2020 2022 2222 0a0a  =0.02).    """..
+00029830: 2020 2020 6368 6563 6b5f 666c 6f61 7428      check_float(
+00029840: 6e61 6d65 3d66 277b 7669 6465 6f5f 746f  name=f'{video_to
+00029850: 5f62 772e 5f5f 6e61 6d65 5f5f 7d20 7468  _bw.__name__} th
+00029860: 7265 7368 6f6c 6427 2c20 7661 6c75 653d  reshold', value=
+00029870: 7468 7265 7368 6f6c 642c 206d 696e 5f76  threshold, min_v
+00029880: 616c 7565 3d30 2c20 6d61 785f 7661 6c75  alue=0, max_valu
+00029890: 653d 312e 3029 0a20 2020 2074 6872 6573  e=1.0).    thres
+000298a0: 686f 6c64 203d 2069 6e74 2832 3535 202a  hold = int(255 *
+000298b0: 2074 6872 6573 686f 6c64 290a 2020 2020   threshold).    
+000298c0: 6368 6563 6b5f 6666 6d70 6567 5f61 7661  check_ffmpeg_ava
+000298d0: 696c 6162 6c65 2872 6169 7365 5f65 7272  ilable(raise_err
+000298e0: 6f72 3d54 7275 6529 0a20 2020 2074 696d  or=True).    tim
+000298f0: 6572 203d 2053 696d 6261 5469 6d65 7228  er = SimbaTimer(
+00029900: 7374 6172 743d 5472 7565 290a 2020 2020  start=True).    
+00029910: 5f20 3d20 6765 745f 7669 6465 6f5f 6d65  _ = get_video_me
+00029920: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
+00029930: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
+00029940: 2020 2064 6972 2c20 7669 6465 6f5f 6e61     dir, video_na
+00029950: 6d65 2c20 6578 7420 3d20 6765 745f 666e  me, ext = get_fn
+00029960: 5f65 7874 2876 6964 656f 5f70 6174 6829  _ext(video_path)
+00029970: 0a20 2020 2073 6176 655f 7061 7468 203d  .    save_path =
+00029980: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
+00029990: 722c 2066 277b 7669 6465 6f5f 6e61 6d65  r, f'{video_name
+000299a0: 7d5f 6277 7b65 7874 7d27 290a 2020 2020  }_bw{ext}').    
+000299b0: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
+000299c0: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
+000299d0: 202d 7666 205c 2266 6f72 6d61 743d 6772   -vf \"format=gr
+000299e0: 6179 2c67 6571 3d6c 756d 5f65 7870 723d  ay,geq=lum_expr=
+000299f0: 2769 6628 6c74 286c 756d 2858 2c59 292c  'if(lt(lum(X,Y),
+00029a00: 7b74 6872 6573 686f 6c64 7d29 2c30 2c32  {threshold}),0,2
+00029a10: 3535 2927 5c22 202d 7069 785f 666d 7420  55)'\" -pix_fmt 
+00029a20: 7975 7634 3230 7020 277b 7361 7665 5f70  yuv420p '{save_p
+00029a30: 6174 687d 2720 2d79 220a 2020 2020 7375  ath}' -y".    su
+00029a40: 6270 726f 6365 7373 2e63 616c 6c28 636d  bprocess.call(cm
+00029a50: 642c 2073 6865 6c6c 3d54 7275 652c 2073  d, shell=True, s
+00029a60: 7464 6f75 743d 7375 6270 726f 6365 7373  tdout=subprocess
+00029a70: 2e50 4950 4529 0a20 2020 2074 696d 6572  .PIPE).    timer
+00029a80: 2e73 746f 705f 7469 6d65 7228 290a 2020  .stop_timer().  
+00029a90: 2020 7374 646f 7574 5f73 7563 6365 7373    stdout_success
+00029aa0: 286d 7367 3d66 2756 6964 656f 207b 7669  (msg=f'Video {vi
+00029ab0: 6465 6f5f 6e61 6d65 7d20 636f 6e76 6572  deo_name} conver
+00029ac0: 7465 642e 272c 2065 6c61 7073 6564 5f74  ted.', elapsed_t
+00029ad0: 696d 653d 7469 6d65 722e 656c 6170 7365  ime=timer.elapse
+00029ae0: 645f 7469 6d65 5f73 7472 290a 0a0a 6465  d_time_str)...de
+00029af0: 6620 6372 6561 7465 5f61 7665 7261 6765  f create_average
+00029b00: 5f66 726d 2876 6964 656f 5f70 6174 683a  _frm(video_path:
+00029b10: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
+00029b20: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
 00029b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b40: 2073 6176 655f 7061 7468 3a20 4f70 7469   save_path: Opti
-00029b50: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-00029b60: 6f73 2e50 6174 684c 696b 655d 5d20 3d20  os.PathLike]] = 
-00029b70: 4e6f 6e65 2920 2d3e 2055 6e69 6f6e 5b4e  None) -> Union[N
-00029b80: 6f6e 652c 206e 702e 6e64 6172 7261 795d  one, np.ndarray]
-00029b90: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
-00029ba0: 6561 7465 2061 6e20 696d 6167 6520 7265  eate an image re
-00029bb0: 7072 6573 656e 7469 6e67 2074 6865 2061  presenting the a
-00029bc0: 7665 7261 6765 2066 7261 6d65 206f 6620  verage frame of 
-00029bd0: 6120 7365 676d 656e 7420 696e 2061 2076  a segment in a v
-00029be0: 6964 656f 206f 7220 616e 2065 6e74 6972  ideo or an entir
-00029bf0: 6520 7669 6465 6f2e 0a0a 2020 2020 2e2e  e video...    ..
-00029c00: 206e 6f74 653a 3a0a 2020 2020 2020 2055   note::.       U
-00029c10: 7365 6675 6c20 6865 6c70 6572 2066 6f72  seful helper for
-00029c20: 2065 2e67 2e2c 2076 6964 656f 2062 6163   e.g., video bac
-00029c30: 6b67 726f 756e 6420 7375 6274 7261 6374  kground subtract
-00029c40: 696f 6e20 6060 7369 6d62 612e 7669 6465  ion ``simba.vide
-00029c50: 6f5f 7072 6f63 6573 736f 7273 2e76 6964  o_processors.vid
-00029c60: 656f 5f70 726f 6365 7373 696e 672e 7669  eo_processing.vi
-00029c70: 6465 6f5f 6267 5f73 7562 7374 7261 6374  deo_bg_substract
-00029c80: 696f 6e28 2960 600a 2020 2020 2020 2045  ion()``.       E
-00029c90: 6974 6865 7220 7061 7373 2060 6073 7461  ither pass ``sta
-00029ca0: 7274 5f66 726d 6060 2061 6e64 2060 6065  rt_frm`` and ``e
-00029cb0: 6e64 5f66 726d 6060 204f 5220 6060 7374  nd_frm`` OR ``st
-00029cc0: 6172 745f 7469 6d65 6060 2061 6e64 2060  art_time`` and `
-00029cd0: 6065 6e64 5f74 696d 6560 6020 4f52 2070  `end_time`` OR p
-00029ce0: 6173 7320 616c 6c20 666f 7572 2061 7267  ass all four arg
-00029cf0: 756d 656e 7473 2061 7320 4e6f 6e65 2e0a  uments as None..
-00029d00: 2020 2020 2020 2049 6620 616c 6c20 6172         If all ar
-00029d10: 6520 4e6f 6e65 2c20 7468 656e 2074 6865  e None, then the
-00029d20: 2065 6e74 6972 6520 7669 6465 6f20 7769   entire video wi
-00029d30: 6c6c 2062 6520 7573 6564 2074 6f20 6372  ll be used to cr
-00029d40: 6561 7465 2074 6865 2061 7665 7261 6765  eate the average
-00029d50: 2066 7261 6d65 2e0a 0a20 2020 203a 7061   frame...    :pa
-00029d60: 7261 6d20 556e 696f 6e5b 7374 722c 206f  ram Union[str, o
-00029d70: 732e 5061 7468 4c69 6b65 5d20 7669 6465  s.PathLike] vide
-00029d80: 6f5f 7061 7468 3a20 5468 6520 7061 7468  o_path: The path
-00029d90: 2074 6f20 7468 6520 7669 6465 6f20 746f   to the video to
-00029da0: 2063 7265 6174 6520 7468 6520 6176 6572   create the aver
-00029db0: 6167 6520 6672 616d 6520 6672 6f6d 2e20  age frame from. 
-00029dc0: 4465 6661 756c 743a 204e 6f6e 652e 0a20  Default: None.. 
-00029dd0: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
-00029de0: 616c 5b69 6e74 5d20 7374 6172 745f 6672  al[int] start_fr
-00029df0: 6d3a 2054 6865 2066 6972 7374 2066 7261  m: The first fra
-00029e00: 6d65 2069 6e20 7468 6520 7365 676d 656e  me in the segmen
-00029e10: 7420 746f 2063 7265 6174 6520 7468 6520  t to create the 
-00029e20: 6176 6572 6167 6520 6672 616d 6520 6672  average frame fr
-00029e30: 6f6d 2e20 4465 6661 756c 743a 204e 6f6e  om. Default: Non
-00029e40: 652e 0a20 2020 203a 7061 7261 6d20 4f70  e..    :param Op
-00029e50: 7469 6f6e 616c 5b69 6e74 5d20 656e 645f  tional[int] end_
-00029e60: 6672 6d3a 2054 6865 206c 6173 7420 6672  frm: The last fr
-00029e70: 616d 6520 696e 2074 6865 2073 6567 6d65  ame in the segme
-00029e80: 6e74 2074 6f20 6372 6561 7465 2074 6865  nt to create the
-00029e90: 2061 7665 7261 6765 2066 7261 6d65 2066   average frame f
-00029ea0: 726f 6d2e 2044 6566 6175 6c74 3a20 4e6f  rom. Default: No
-00029eb0: 6e65 2e0a 2020 2020 3a70 6172 616d 204f  ne..    :param O
-00029ec0: 7074 696f 6e61 6c5b 7374 725d 2073 7461  ptional[str] sta
-00029ed0: 7274 5f74 696d 653a 2054 6865 2073 7461  rt_time: The sta
-00029ee0: 7274 2074 696d 6573 7461 6d70 2069 6e20  rt timestamp in 
-00029ef0: 6048 483a 4d4d 3a53 5360 2066 6f72 6d61  `HH:MM:SS` forma
-00029f00: 7420 696e 2074 6865 2073 6567 6d65 6e74  t in the segment
-00029f10: 2074 6f20 6372 6561 7465 2074 6865 2061   to create the a
-00029f20: 7665 7261 6765 2066 7261 6d65 2066 726f  verage frame fro
-00029f30: 6d2e 2044 6566 6175 6c74 3a20 4e6f 6e65  m. Default: None
-00029f40: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-00029f50: 696f 6e61 6c5b 7374 725d 2065 6e64 5f74  ional[str] end_t
-00029f60: 696d 653a 2054 6865 2065 6e64 2074 696d  ime: The end tim
-00029f70: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
-00029f80: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
-00029f90: 6865 2073 6567 6d65 6e74 2074 6f20 6372  he segment to cr
-00029fa0: 6561 7465 2074 6865 2061 7665 7261 6765  eate the average
-00029fb0: 2066 7261 6d65 2066 726f 6d2e 2044 6566   frame from. Def
-00029fc0: 6175 6c74 3a20 4e6f 6e65 2e0a 2020 2020  ault: None..    
-00029fd0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-00029fe0: 556e 696f 6e5b 7374 722c 206f 732e 5061  Union[str, os.Pa
-00029ff0: 7468 4c69 6b65 5d5d 2073 6176 655f 7061  thLike]] save_pa
-0002a000: 7468 3a20 5468 6520 7061 7468 2074 6f20  th: The path to 
-0002a010: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
-0002a020: 6520 6176 6572 6167 6520 696d 6167 652e  e average image.
-0002a030: 2049 6620 4e6f 6e65 2c20 7468 656e 2072   If None, then r
-0002a040: 6561 7475 7265 6e73 2074 6865 2061 7665  eaturens the ave
-0002a050: 7261 6765 2069 6d61 6765 2069 6e20 6e70  rage image in np
-0002a060: 2c6e 6461 7272 6179 2066 6f72 6d61 742e  ,ndarray format.
-0002a070: 2044 6566 6175 6c74 3a20 4e6f 6e65 2e0a   Default: None..
-0002a080: 2020 2020 3a72 6574 7572 6e20 556e 696f      :return Unio
-0002a090: 6e5b 4e6f 6e65 2c20 6e70 2e6e 6461 7272  n[None, np.ndarr
-0002a0a0: 6179 5d3a 2054 6865 2061 7665 7261 6765  ay]: The average
-0002a0b0: 2069 6d61 6765 2028 6966 2060 6073 6176   image (if ``sav
-0002a0c0: 655f 7061 7468 6060 2069 7320 6e6f 7420  e_path`` is not 
-0002a0d0: 4e6f 6e65 2920 6f72 204e 6f6e 6520 6966  None) or None if
-0002a0e0: 2020 6060 7361 7665 5f70 6174 6860 6020    ``save_path`` 
-0002a0f0: 6973 2070 6173 7365 642e 0a20 2020 2022  is passed..    "
-0002a100: 2222 0a0a 2020 2020 6966 2028 2873 7461  ""..    if ((sta
-0002a110: 7274 5f66 726d 2069 7320 6e6f 7420 4e6f  rt_frm is not No
-0002a120: 6e65 2920 6f72 2028 656e 645f 6672 6d20  ne) or (end_frm 
-0002a130: 6973 206e 6f74 204e 6f6e 6529 2920 616e  is not None)) an
-0002a140: 6420 2828 7374 6172 745f 7469 6d65 2069  d ((start_time i
-0002a150: 7320 6e6f 7420 4e6f 6e65 2920 6f72 2028  s not None) or (
-0002a160: 656e 645f 7469 6d65 2069 7320 6e6f 7420  end_time is not 
-0002a170: 4e6f 6e65 2929 3a0a 2020 2020 2020 2020  None)):.        
-0002a180: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
-0002a190: 7574 4572 726f 7228 6d73 673d 6627 5061  utError(msg=f'Pa
-0002a1a0: 7373 2073 7461 7274 5f66 726d 2061 6e64  ss start_frm and
-0002a1b0: 2065 6e64 5f66 726d 204f 5220 7374 6172   end_frm OR star
-0002a1c0: 745f 7469 6d65 2061 6e64 2065 6e64 5f74  t_time and end_t
-0002a1d0: 696d 6527 2c0a 2020 2020 2020 2020 2020  ime',.          
-0002a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a1f0: 2020 2020 2020 736f 7572 6365 3d63 7265        source=cre
-0002a200: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
-0002a210: 5f5f 6e61 6d65 5f5f 290a 2020 2020 656c  __name__).    el
-0002a220: 6966 2074 7970 6528 7374 6172 745f 6672  if type(start_fr
-0002a230: 6d29 2021 3d20 7479 7065 2865 6e64 5f66  m) != type(end_f
-0002a240: 726d 293a 0a20 2020 2020 2020 2072 6169  rm):.        rai
-0002a250: 7365 2049 6e76 616c 6964 496e 7075 7445  se InvalidInputE
-0002a260: 7272 6f72 286d 7367 3d66 2750 6173 7320  rror(msg=f'Pass 
-0002a270: 7374 6172 7420 6672 616d 6520 616e 6420  start frame and 
-0002a280: 656e 6420 6672 616d 6527 2c20 736f 7572  end frame', sour
-0002a290: 6365 3d63 7265 6174 655f 6176 6572 6167  ce=create_averag
-0002a2a0: 655f 6672 6d2e 5f5f 6e61 6d65 5f5f 290a  e_frm.__name__).
-0002a2b0: 2020 2020 656c 6966 2074 7970 6528 7374      elif type(st
-0002a2c0: 6172 745f 7469 6d65 2920 213d 2074 7970  art_time) != typ
-0002a2d0: 6528 656e 645f 7469 6d65 293a 0a20 2020  e(end_time):.   
-0002a2e0: 2020 2020 2072 6169 7365 2049 6e76 616c       raise Inval
-0002a2f0: 6964 496e 7075 7445 7272 6f72 286d 7367  idInputError(msg
-0002a300: 3d66 2750 6173 7320 7374 6172 7420 7469  =f'Pass start ti
-0002a310: 6d65 2061 6e64 2065 6e64 2074 696d 6527  me and end time'
-0002a320: 2c20 736f 7572 6365 3d63 7265 6174 655f  , source=create_
-0002a330: 6176 6572 6167 655f 6672 6d2e 5f5f 6e61  average_frm.__na
-0002a340: 6d65 5f5f 290a 2020 2020 6368 6563 6b5f  me__).    check_
-0002a350: 6669 6c65 5f65 7869 7374 5f61 6e64 5f72  file_exist_and_r
-0002a360: 6561 6461 626c 6528 6669 6c65 5f70 6174  eadable(file_pat
-0002a370: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-0002a380: 2020 7669 6465 6f5f 6d65 7461 5f64 6174    video_meta_dat
-0002a390: 6120 3d20 6765 745f 7669 6465 6f5f 6d65  a = get_video_me
-0002a3a0: 7461 5f64 6174 6128 7669 6465 6f5f 7061  ta_data(video_pa
-0002a3b0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
-0002a3c0: 2020 2063 6170 203d 2063 7632 2e56 6964     cap = cv2.Vid
-0002a3d0: 656f 4361 7074 7572 6528 7669 6465 6f5f  eoCapture(video_
-0002a3e0: 7061 7468 290a 2020 2020 6966 2028 7374  path).    if (st
-0002a3f0: 6172 745f 6672 6d20 6973 206e 6f74 204e  art_frm is not N
-0002a400: 6f6e 6529 2061 6e64 2028 656e 645f 6672  one) and (end_fr
-0002a410: 6d20 6973 206e 6f74 204e 6f6e 6529 3a0a  m is not None):.
-0002a420: 2020 2020 2020 2020 6368 6563 6b5f 696e          check_in
-0002a430: 7428 6e61 6d65 3d27 7374 6172 745f 6672  t(name='start_fr
-0002a440: 6d27 2c20 7661 6c75 653d 7374 6172 745f  m', value=start_
-0002a450: 6672 6d2c 206d 696e 5f76 616c 7565 3d30  frm, min_value=0
-0002a460: 2c20 6d61 785f 7661 6c75 653d 7669 6465  , max_value=vide
-0002a470: 6f5f 6d65 7461 5f64 6174 615b 2766 7261  o_meta_data['fra
-0002a480: 6d65 5f63 6f75 6e74 275d 290a 2020 2020  me_count']).    
-0002a490: 2020 2020 6368 6563 6b5f 696e 7428 6e61      check_int(na
-0002a4a0: 6d65 3d27 656e 645f 6672 6d27 2c20 7661  me='end_frm', va
-0002a4b0: 6c75 653d 656e 645f 6672 6d2c 206d 696e  lue=end_frm, min
-0002a4c0: 5f76 616c 7565 3d30 2c20 6d61 785f 7661  _value=0, max_va
-0002a4d0: 6c75 653d 7669 6465 6f5f 6d65 7461 5f64  lue=video_meta_d
-0002a4e0: 6174 615b 2766 7261 6d65 5f63 6f75 6e74  ata['frame_count
-0002a4f0: 275d 290a 2020 2020 2020 2020 6966 2073  ']).        if s
-0002a500: 7461 7274 5f66 726d 203e 2065 6e64 5f66  tart_frm > end_f
-0002a510: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
-0002a520: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
-0002a530: 7574 4572 726f 7228 6d73 673d 6627 5374  utError(msg=f'St
-0002a540: 6172 7420 6672 616d 6520 287b 7374 6172  art frame ({star
-0002a550: 745f 6672 6d7d 2920 6861 7320 746f 2062  t_frm}) has to b
-0002a560: 6520 6265 666f 7265 2065 6e64 2066 7261  e before end fra
-0002a570: 6d65 2028 7b65 6e64 5f66 726d 7d29 2e27  me ({end_frm}).'
-0002a580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a5a0: 2020 2020 2020 736f 7572 6365 3d63 7265        source=cre
-0002a5b0: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
-0002a5c0: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
-0002a5d0: 2020 6672 616d 655f 6964 7320 3d20 6c69    frame_ids = li
-0002a5e0: 7374 2872 616e 6765 2873 7461 7274 5f66  st(range(start_f
-0002a5f0: 726d 2c20 656e 645f 6672 6d20 2b20 3129  rm, end_frm + 1)
-0002a600: 290a 2020 2020 656c 6966 2028 7374 6172  ).    elif (star
-0002a610: 745f 7469 6d65 2069 7320 6e6f 7420 4e6f  t_time is not No
-0002a620: 6e65 2920 616e 6420 2865 6e64 5f74 696d  ne) and (end_tim
-0002a630: 6520 6973 206e 6f74 204e 6f6e 6529 3a0a  e is not None):.
-0002a640: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
-0002a650: 5f73 7472 696e 675f 7661 6c75 655f 6973  _string_value_is
-0002a660: 5f76 616c 6964 5f76 6964 656f 5f74 696d  _valid_video_tim
-0002a670: 6573 7461 6d70 2876 616c 7565 3d73 7461  estamp(value=sta
-0002a680: 7274 5f74 696d 652c 206e 616d 653d 6372  rt_time, name=cr
-0002a690: 6561 7465 5f61 7665 7261 6765 5f66 726d  eate_average_frm
-0002a6a0: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2020  .__name__).     
-0002a6b0: 2020 2063 6865 636b 5f69 665f 7374 7269     check_if_stri
-0002a6c0: 6e67 5f76 616c 7565 5f69 735f 7661 6c69  ng_value_is_vali
-0002a6d0: 645f 7669 6465 6f5f 7469 6d65 7374 616d  d_video_timestam
-0002a6e0: 7028 7661 6c75 653d 656e 645f 7469 6d65  p(value=end_time
-0002a6f0: 2c20 6e61 6d65 3d63 7265 6174 655f 6176  , name=create_av
-0002a700: 6572 6167 655f 6672 6d2e 5f5f 6e61 6d65  erage_frm.__name
-0002a710: 5f5f 290a 2020 2020 2020 2020 6368 6563  __).        chec
-0002a720: 6b5f 7468 6174 5f68 686d 6d73 735f 7374  k_that_hhmmss_st
-0002a730: 6172 745f 6973 5f62 6566 6f72 655f 656e  art_is_before_en
-0002a740: 6428 7374 6172 745f 7469 6d65 3d73 7461  d(start_time=sta
-0002a750: 7274 5f74 696d 652c 2065 6e64 5f74 696d  rt_time, end_tim
-0002a760: 653d 656e 645f 7469 6d65 2c0a 2020 2020  e=end_time,.    
-0002a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a790: 2020 2020 2020 2020 2020 6e61 6d65 3d63            name=c
-0002a7a0: 7265 6174 655f 6176 6572 6167 655f 6672  reate_average_fr
-0002a7b0: 6d2e 5f5f 6e61 6d65 5f5f 290a 2020 2020  m.__name__).    
-0002a7c0: 2020 2020 6368 6563 6b5f 6966 5f68 686d      check_if_hhm
-0002a7d0: 6d73 735f 7469 6d65 7374 616d 705f 6973  mss_timestamp_is
-0002a7e0: 5f76 616c 6964 5f70 6172 745f 6f66 5f76  _valid_part_of_v
-0002a7f0: 6964 656f 2874 696d 6573 7461 6d70 3d73  ideo(timestamp=s
-0002a800: 7461 7274 5f74 696d 652c 2076 6964 656f  tart_time, video
-0002a810: 5f70 6174 683d 7669 6465 6f5f 7061 7468  _path=video_path
-0002a820: 290a 2020 2020 2020 2020 6672 616d 655f  ).        frame_
-0002a830: 6964 7320 3d20 6669 6e64 5f66 7261 6d65  ids = find_frame
-0002a840: 5f6e 756d 6265 7273 5f66 726f 6d5f 7469  _numbers_from_ti
-0002a850: 6d65 5f73 7461 6d70 2873 7461 7274 5f74  me_stamp(start_t
-0002a860: 696d 653d 7374 6172 745f 7469 6d65 2c20  ime=start_time, 
-0002a870: 656e 645f 7469 6d65 3d65 6e64 5f74 696d  end_time=end_tim
-0002a880: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0002a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a8b0: 2020 2020 2020 2020 2020 6670 733d 7669            fps=vi
-0002a8c0: 6465 6f5f 6d65 7461 5f64 6174 615b 2766  deo_meta_data['f
-0002a8d0: 7073 275d 290a 2020 2020 656c 7365 3a0a  ps']).    else:.
-0002a8e0: 2020 2020 2020 2020 6672 616d 655f 6964          frame_id
-0002a8f0: 7320 3d20 6c69 7374 2872 616e 6765 2830  s = list(range(0
-0002a900: 2c20 7669 6465 6f5f 6d65 7461 5f64 6174  , video_meta_dat
-0002a910: 615b 2766 7261 6d65 5f63 6f75 6e74 275d  a['frame_count']
-0002a920: 2929 0a20 2020 2063 6170 2e73 6574 2830  )).    cap.set(0
-0002a930: 2c20 6672 616d 655f 6964 735b 305d 290a  , frame_ids[0]).
-0002a940: 2020 2020 6267 5f73 756d 2c20 6672 6d5f      bg_sum, frm_
-0002a950: 636e 742c 2066 726d 5f6c 656e 203d 204e  cnt, frm_len = N
-0002a960: 6f6e 652c 2030 2c20 6c65 6e28 6672 616d  one, 0, len(fram
-0002a970: 655f 6964 7329 0a20 2020 2077 6869 6c65  e_ids).    while
-0002a980: 2066 726d 5f63 6e74 203c 3d20 6672 6d5f   frm_cnt <= frm_
-0002a990: 6c65 6e3a 0a20 2020 2020 2020 2072 6574  len:.        ret
-0002a9a0: 2c20 6672 6d20 3d20 6361 702e 7265 6164  , frm = cap.read
-0002a9b0: 2829 0a20 2020 2020 2020 2069 6620 6267  ().        if bg
-0002a9c0: 5f73 756d 2069 7320 4e6f 6e65 3a20 6267  _sum is None: bg
-0002a9d0: 5f73 756d 203d 206e 702e 666c 6f61 7433  _sum = np.float3
-0002a9e0: 3228 6672 6d29 0a20 2020 2020 2020 2065  2(frm).        e
-0002a9f0: 6c73 653a 2063 7632 2e61 6363 756d 756c  lse: cv2.accumul
-0002aa00: 6174 6528 6672 6d2c 2062 675f 7375 6d29  ate(frm, bg_sum)
-0002aa10: 0a20 2020 2020 2020 2066 726d 5f63 6e74  .        frm_cnt
-0002aa20: 202b 3d20 310a 2020 2020 696d 6720 3d20   += 1.    img = 
-0002aa30: 6376 322e 636f 6e76 6572 7453 6361 6c65  cv2.convertScale
-0002aa40: 4162 7328 6267 5f73 756d 202f 2066 726d  Abs(bg_sum / frm
-0002aa50: 5f6c 656e 290a 2020 2020 6361 702e 7265  _len).    cap.re
-0002aa60: 6c65 6173 6528 290a 2020 2020 6966 2073  lease().    if s
-0002aa70: 6176 655f 7061 7468 2069 7320 6e6f 7420  ave_path is not 
-0002aa80: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
-0002aa90: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
-0002aaa0: 7328 696e 5f64 6972 3d6f 732e 7061 7468  s(in_dir=os.path
-0002aab0: 2e64 6972 6e61 6d65 2873 6176 655f 7061  .dirname(save_pa
-0002aac0: 7468 292c 2073 6f75 7263 653d 6372 6561  th), source=crea
-0002aad0: 7465 5f61 7665 7261 6765 5f66 726d 2e5f  te_average_frm._
-0002aae0: 5f6e 616d 655f 5f29 0a20 2020 2020 2020  _name__).       
-0002aaf0: 2063 7632 2e69 6d77 7269 7465 2873 6176   cv2.imwrite(sav
-0002ab00: 655f 7061 7468 2c20 696d 6729 0a20 2020  e_path, img).   
-0002ab10: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-0002ab20: 6574 7572 6e20 696d 670a 0a0a 6465 6620  eturn img...def 
-0002ab30: 7669 6465 6f5f 6267 5f73 7562 7472 6163  video_bg_subtrac
-0002ab40: 7469 6f6e 2876 6964 656f 5f70 6174 683a  tion(video_path:
-0002ab50: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-0002ab60: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
-0002ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ab80: 2020 2020 6267 5f76 6964 656f 5f70 6174      bg_video_pat
-0002ab90: 683a 204f 7074 696f 6e61 6c5b 556e 696f  h: Optional[Unio
-0002aba0: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-0002abb0: 6b65 5d5d 203d 204e 6f6e 652c 0a20 2020  ke]] = None,.   
-0002abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002abd0: 2020 2020 2020 2062 675f 7374 6172 745f         bg_start_
-0002abe0: 6672 6d3a 204f 7074 696f 6e61 6c5b 696e  frm: Optional[in
-0002abf0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-0002ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac10: 2020 2020 2062 675f 656e 645f 6672 6d3a       bg_end_frm:
-0002ac20: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0002ac30: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0002ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac50: 2062 675f 7374 6172 745f 7469 6d65 3a20   bg_start_time: 
-0002ac60: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0002ac70: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0002ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac90: 6267 5f65 6e64 5f74 696d 653a 204f 7074  bg_end_time: Opt
-0002aca0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0002acb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0002acc0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
-0002acd0: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
-0002ace0: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
-0002acf0: 696e 745d 5d20 3d20 2830 2c20 302c 2030  int]] = (0, 0, 0
-0002ad00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0002ad10: 2020 2020 2020 2020 2020 2020 2066 675f               fg_
-0002ad20: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
-0002ad30: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
-0002ad40: 696e 745d 5d20 3d20 4e6f 6e65 2c0a 2020  int]] = None,.  
-0002ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ad60: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
-0002ad70: 683a 204f 7074 696f 6e61 6c5b 556e 696f  h: Optional[Unio
-0002ad80: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-0002ad90: 6b65 5d5d 203d 204e 6f6e 6529 202d 3e20  ke]] = None) -> 
-0002ada0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-0002adb0: 2020 5375 6274 7261 6374 2074 6865 2062    Subtract the b
-0002adc0: 6163 6b67 726f 756e 6420 6672 6f6d 2061  ackground from a
-0002add0: 2076 6964 656f 2e0a 0a20 2020 202e 2e20   video...    .. 
-0002ade0: 7669 6465 6f3a 3a20 5f73 7461 7469 632f  video:: _static/
-0002adf0: 696d 672f 7669 6465 6f5f 6267 5f73 7562  img/video_bg_sub
-0002ae00: 7472 6163 7469 6f6e 2e77 6562 6d0a 2020  traction.webm.  
-0002ae10: 2020 2020 203a 6c6f 6f70 3a0a 0a20 2020       :loop:..   
-0002ae20: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
-0002ae30: 2020 4966 2020 6060 6267 5f76 6964 656f    If  ``bg_video
-0002ae40: 5f70 6174 6860 6020 6973 2070 6173 7365  _path`` is passe
-0002ae50: 642c 2074 6861 7420 7669 6465 6f20 7769  d, that video wi
-0002ae60: 6c6c 2062 6520 7573 6564 2074 6f20 7061  ll be used to pa
-0002ae70: 7273 6520 7468 6520 6261 636b 6772 6f75  rse the backgrou
-0002ae80: 6e64 2e20 4966 204e 6f6e 652c 2060 6076  nd. If None, ``v
-0002ae90: 6964 656f 5f70 6174 6860 6020 7769 6c6c  ideo_path`` will
-0002aea0: 2062 6520 7573 6520 6474 6f20 7061 7273   be use dto pars
-0002aeb0: 6520 6261 636b 6772 6f75 6e64 2e0a 2020  e background..  
-0002aec0: 2020 2020 2045 6974 6865 7220 7061 7373       Either pass
-0002aed0: 2060 6073 7461 7274 5f66 726d 6060 2061   ``start_frm`` a
-0002aee0: 6e64 2060 6065 6e64 5f66 726d 6060 204f  nd ``end_frm`` O
-0002aef0: 5220 6060 7374 6172 745f 7469 6d65 6060  R ``start_time``
-0002af00: 2061 6e64 2060 6065 6e64 5f74 696d 6560   and ``end_time`
-0002af10: 6020 4f52 2070 6173 7320 616c 6c20 666f  ` OR pass all fo
-0002af20: 7572 2061 7267 756d 656e 7473 2061 7320  ur arguments as 
-0002af30: 4e6f 6e65 2e0a 2020 2020 2020 2054 686f  None..       Tho
-0002af40: 7365 2074 776f 2061 7267 756d 656e 7473  se two arguments
-0002af50: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
-0002af60: 2073 6c69 6365 2074 6865 2062 6163 6b67   slice the backg
-0002af70: 726f 756e 6420 7669 6465 6f2c 2061 6e64  round video, and
-0002af80: 2074 6865 2073 6c69 6365 6420 7061 7274   the sliced part
-0002af90: 2069 7320 7573 6564 2074 6f20 7061 7273   is used to pars
-0002afa0: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
-0002afb0: 2e0a 0a20 2020 2020 2020 466f 7220 6578  ...       For ex
-0002afc0: 616d 706c 652c 2069 6e20 7468 6520 7363  ample, in the sc
-0002afd0: 656e 6172 696f 2077 6865 7265 2074 6865  enario where the
-0002afe0: 7265 2069 7320 2a2a 6e6f 2a2a 2061 6e69  re is **no** ani
-0002aff0: 6d61 6c20 696e 2074 6865 2060 6076 6964  mal in the ``vid
-0002b000: 656f 5f70 6174 6860 6020 7669 6465 6f20  eo_path`` video 
-0002b010: 666f 7220 7468 6520 6669 7273 7420 3230  for the first 20
-0002b020: 732c 2074 6865 6e20 7468 6520 6669 7273  s, then the firs
-0002b030: 7420 3230 7320 6361 6e20 6265 2075 7365  t 20s can be use
-0002b040: 6420 746f 2070 6172 7365 2074 6865 2062  d to parse the b
-0002b050: 6163 6b67 726f 756e 642e 0a20 2020 2020  ackground..     
-0002b060: 2020 496e 2074 6869 7320 7363 656e 6172    In this scenar
-0002b070: 696f 2c20 6060 6267 5f76 6964 656f 5f70  io, ``bg_video_p
-0002b080: 6174 6860 6020 6361 6e20 6265 2070 6173  ath`` can be pas
-0002b090: 7365 6420 6173 2060 604e 6f6e 6560 6020  sed as ``None`` 
-0002b0a0: 616e 6420 6267 5f73 7461 7274 5f74 696d  and bg_start_tim
-0002b0b0: 6520 616e 6420 6267 5f65 6e64 5f74 696d  e and bg_end_tim
-0002b0c0: 6520 6361 6e20 6265 2060 6030 303a 3030  e can be ``00:00
-0002b0d0: 3a30 3060 6020 616e 6420 6060 3030 3a30  :00`` and ``00:0
-0002b0e0: 303a 3230 6060 2c20 7265 7065 6374 6976  0:20``, repectiv
-0002b0f0: 656c 792e 0a0a 2020 2020 2020 2049 6e20  ely...       In 
-0002b100: 7468 6520 7363 656e 6172 696f 2077 6865  the scenario whe
-0002b110: 7265 2074 6865 7265 202a 2a69 732a 2a20  re there **is** 
-0002b120: 616e 696d 616c 2873 2920 696e 2074 6865  animal(s) in the
-0002b130: 2065 6e74 6972 6520 6060 7669 6465 6f5f   entire ``video_
-0002b140: 7061 7468 6060 2076 6964 656f 2c20 7061  path`` video, pa
-0002b150: 7373 2060 6062 675f 7669 6465 6f5f 7061  ss ``bg_video_pa
-0002b160: 7468 6060 2061 7320 6120 7061 7468 2074  th`` as a path t
-0002b170: 6f20 6120 7669 6465 6f20 7265 636f 7264  o a video record
-0002b180: 696e 6720 7468 6520 6172 656e 6120 7769  ing the arena wi
-0002b190: 7468 6f75 7420 7468 6520 616e 696d 616c  thout the animal
-0002b1a0: 732e 0a0a 2020 2020 3a70 6172 616d 2055  s...    :param U
-0002b1b0: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-0002b1c0: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
-0002b1d0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
-0002b1e0: 6865 2076 6964 656f 2074 6f20 7265 6d6f  he video to remo
-0002b1f0: 7665 2074 6865 2062 6163 6b67 726f 756e  ve the backgroun
-0002b200: 6420 6672 6f6d 2e0a 2020 2020 3a70 6172  d from..    :par
-0002b210: 616d 204f 7074 696f 6e61 6c5b 556e 696f  am Optional[Unio
-0002b220: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-0002b230: 6b65 5d5d 2062 675f 7669 6465 6f5f 7061  ke]] bg_video_pa
-0002b240: 7468 3a20 5061 7468 2074 6f20 7468 6520  th: Path to the 
-0002b250: 7669 6465 6f20 7768 6963 6820 636f 6e74  video which cont
-0002b260: 6169 6e73 2061 2073 6567 6d65 6e74 2077  ains a segment w
-0002b270: 6974 6820 7468 6520 6261 636b 6772 6f75  ith the backgrou
-0002b280: 6e64 206f 6e6c 792e 2049 6620 4e6f 6e65  nd only. If None
-0002b290: 2c20 7468 656e 2060 6076 6964 656f 5f70  , then ``video_p
-0002b2a0: 6174 6860 6020 7769 6c6c 2062 6520 7573  ath`` will be us
-0002b2b0: 6564 2e0a 2020 2020 3a70 6172 616d 204f  ed..    :param O
-0002b2c0: 7074 696f 6e61 6c5b 696e 745d 2062 675f  ptional[int] bg_
-0002b2d0: 7374 6172 745f 6672 6d3a 2054 6865 2066  start_frm: The f
-0002b2e0: 6972 7374 2066 7261 6d65 2069 6e20 7468  irst frame in th
-0002b2f0: 6520 6261 636b 6772 6f75 6e64 2076 6964  e background vid
-0002b300: 656f 2074 6f20 7573 6520 7768 656e 2063  eo to use when c
-0002b310: 7265 6174 696e 6720 6120 7265 7072 6573  reating a repres
-0002b320: 656e 7461 7469 7665 2062 6163 6b67 726f  entative backgro
-0002b330: 756e 6420 696d 6167 652e 2044 6566 6175  und image. Defau
-0002b340: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a70  lt: None..    :p
-0002b350: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
-0002b360: 745d 2062 675f 656e 645f 6672 6d3a 2054  t] bg_end_frm: T
-0002b370: 6865 206c 6173 7420 6672 616d 6520 696e  he last frame in
-0002b380: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002b390: 7669 6465 6f20 746f 2075 7365 2077 6865  video to use whe
-0002b3a0: 6e20 6372 6561 7469 6e67 2061 2072 6570  n creating a rep
-0002b3b0: 7265 7365 6e74 6174 6976 6520 6261 636b  resentative back
-0002b3c0: 6772 6f75 6e64 2069 6d61 6765 2e20 4465  ground image. De
-0002b3d0: 6661 756c 743a 204e 6f6e 652e 0a20 2020  fault: None..   
-0002b3e0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-0002b3f0: 5b73 7472 5d20 6267 5f73 7461 7274 5f74  [str] bg_start_t
-0002b400: 696d 653a 2054 6865 2073 7461 7274 2074  ime: The start t
-0002b410: 696d 6573 7461 6d70 2069 6e20 6048 483a  imestamp in `HH:
-0002b420: 4d4d 3a53 5360 2066 6f72 6d61 7420 696e  MM:SS` format in
-0002b430: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002b440: 7669 6465 6f20 746f 2075 7365 2074 6f20  video to use to 
-0002b450: 6372 6561 7465 2061 2072 6570 7265 7365  create a represe
-0002b460: 6e74 6174 6976 6520 6261 636b 6772 6f75  ntative backgrou
-0002b470: 6e64 2069 6d61 6765 2e20 4465 6661 756c  nd image. Defaul
-0002b480: 743a 204e 6f6e 652e 0a20 2020 203a 7061  t: None..    :pa
-0002b490: 7261 6d20 4f70 7469 6f6e 616c 5b73 7472  ram Optional[str
-0002b4a0: 5d20 6267 5f65 6e64 5f74 696d 653a 2054  ] bg_end_time: T
-0002b4b0: 6865 2065 6e64 2074 696d 6573 7461 6d70  he end timestamp
-0002b4c0: 2069 6e20 6048 483a 4d4d 3a53 5360 2066   in `HH:MM:SS` f
-0002b4d0: 6f72 6d61 7420 696e 2074 6865 2062 6163  ormat in the bac
-0002b4e0: 6b67 726f 756e 6420 7669 6465 6f20 746f  kground video to
-0002b4f0: 2075 7365 2074 6f20 6372 6561 7465 2061   use to create a
-0002b500: 2072 6570 7265 7365 6e74 6174 6976 6520   representative 
-0002b510: 6261 636b 6772 6f75 6e64 2069 6d61 6765  background image
-0002b520: 2e20 4465 6661 756c 743a 204e 6f6e 652e  . Default: None.
-0002b530: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-0002b540: 6f6e 616c 5b54 7570 6c65 5b69 6e74 2c20  onal[Tuple[int, 
-0002b550: 696e 742c 2069 6e74 5d5d 2062 675f 636f  int, int]] bg_co
-0002b560: 6c6f 723a 2054 6865 2052 4742 2063 6f6c  lor: The RGB col
-0002b570: 6f72 206f 6620 7468 6520 6d6f 7669 6e67  or of the moving
-0002b580: 206f 626a 6563 7473 2069 6e20 7468 6520   objects in the 
-0002b590: 6f75 7470 7574 2076 6964 656f 2e20 4465  output video. De
-0002b5a0: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
-0002b5b0: 7768 6963 6820 7265 7072 6573 656e 7473  which represents
-0002b5c0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
-0002b5d0: 6c6f 7273 206f 6620 7468 6520 6d6f 7669  lors of the movi
-0002b5e0: 6e67 206f 626a 6563 7473 2e0a 2020 2020  ng objects..    
-0002b5f0: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-0002b600: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
-0002b610: 696e 745d 5d20 6667 5f63 6f6c 6f72 3a20  int]] fg_color: 
-0002b620: 5468 6520 5247 4220 636f 6c6f 7220 6f66  The RGB color of
-0002b630: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002b640: 6f75 7470 7574 2076 6964 656f 2e20 4465  output video. De
-0002b650: 6661 756c 7473 2074 6f20 626c 6163 6b20  faults to black 
-0002b660: 2830 2c20 302c 2030 292e 0a20 2020 203a  (0, 0, 0)..    :
-0002b670: 7061 7261 6d20 4f70 7469 6f6e 616c 5b55  param Optional[U
-0002b680: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-0002b690: 684c 696b 655d 5d20 7361 7665 5f70 6174  hLike]] save_pat
-0002b6a0: 683a 2054 6865 2070 6174 6368 2074 6f20  h: The patch to 
-0002b6b0: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
-0002b6c0: 6520 6f75 7470 7574 2076 6964 656f 2077  e output video w
-0002b6d0: 6865 7265 2074 6865 2062 6163 6b67 726f  here the backgro
-0002b6e0: 756e 6420 6973 2072 656d 6f76 6564 2e20  und is removed. 
-0002b6f0: 4966 204e 6f6e 652c 2073 6176 6573 2074  If None, saves t
-0002b700: 6865 206f 7574 7075 7420 7669 6465 6f20  he output video 
-0002b710: 696e 2074 6865 2073 616d 6520 6469 7265  in the same dire
-0002b720: 6374 6f72 7920 6173 2074 6865 2069 6e70  ctory as the inp
-0002b730: 7574 2076 6964 656f 2077 6974 6820 7468  ut video with th
-0002b740: 6520 6060 5f62 675f 7375 6274 7261 6374  e ``_bg_subtract
-0002b750: 6564 6060 2073 7566 6669 782e 2044 6566  ed`` suffix. Def
-0002b760: 6175 6c74 3a20 4e6f 6e65 2e0a 2020 2020  ault: None..    
-0002b770: 3a72 6574 7572 6e3a 204e 6f6e 652e 0a0a  :return: None...
-0002b780: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
-0002b790: 2020 3e3e 3e20 7669 6465 6f5f 6267 5f73    >>> video_bg_s
-0002b7a0: 7562 7472 6163 7469 6f6e 2876 6964 656f  ubtraction(video
-0002b7b0: 5f70 6174 683d 272f 5573 6572 732f 7369  _path='/Users/si
-0002b7c0: 6d6f 6e2f 446f 776e 6c6f 6164 732f 315f  mon/Downloads/1_
-0002b7d0: 4c48 5f63 726f 7070 6564 2e6d 7034 272c  LH_cropped.mp4',
-0002b7e0: 2062 675f 7374 6172 745f 7469 6d65 3d27   bg_start_time='
-0002b7f0: 3030 3a30 303a 3030 272c 2062 675f 656e  00:00:00', bg_en
-0002b800: 645f 7469 6d65 3d27 3030 3a30 303a 3130  d_time='00:00:10
-0002b810: 272c 2062 675f 636f 6c6f 723d 2830 2c20  ', bg_color=(0, 
-0002b820: 3130 362c 2031 3637 292c 2066 675f 636f  106, 167), fg_co
-0002b830: 6c6f 723d 2832 3534 2c20 3230 342c 2032  lor=(254, 204, 2
-0002b840: 2929 0a20 2020 2022 2222 0a0a 2020 2020  )).    """..    
-0002b850: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
-0002b860: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
-0002b870: 2020 2063 6865 636b 5f66 696c 655f 6578     check_file_ex
-0002b880: 6973 745f 616e 645f 7265 6164 6162 6c65  ist_and_readable
-0002b890: 2866 696c 655f 7061 7468 3d76 6964 656f  (file_path=video
-0002b8a0: 5f70 6174 6829 0a20 2020 2069 6620 6267  _path).    if bg
-0002b8b0: 5f76 6964 656f 5f70 6174 6820 6973 204e  _video_path is N
-0002b8c0: 6f6e 653a 0a20 2020 2020 2020 2062 675f  one:.        bg_
-0002b8d0: 7669 6465 6f5f 7061 7468 203d 2064 6565  video_path = dee
-0002b8e0: 7063 6f70 7928 7669 6465 6f5f 7061 7468  pcopy(video_path
-0002b8f0: 290a 2020 2020 7669 6465 6f5f 6d65 7461  ).    video_meta
-0002b900: 5f64 6174 6120 3d20 6765 745f 7669 6465  _data = get_vide
-0002b910: 6f5f 6d65 7461 5f64 6174 6128 7669 6465  o_meta_data(vide
-0002b920: 6f5f 7061 7468 3d76 6964 656f 5f70 6174  o_path=video_pat
-0002b930: 6829 0a20 2020 2064 6972 2c20 7669 6465  h).    dir, vide
-0002b940: 6f5f 6e61 6d65 2c20 6578 7420 3d20 6765  o_name, ext = ge
-0002b950: 745f 666e 5f65 7874 2866 696c 6570 6174  t_fn_ext(filepat
-0002b960: 683d 7669 6465 6f5f 7061 7468 290a 2020  h=video_path).  
-0002b970: 2020 6966 2073 6176 655f 7061 7468 2069    if save_path i
-0002b980: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002b990: 7361 7665 5f70 6174 6820 3d20 6f73 2e70  save_path = os.p
-0002b9a0: 6174 682e 6a6f 696e 2864 6972 2c20 6627  ath.join(dir, f'
-0002b9b0: 7b76 6964 656f 5f6e 616d 657d 5f62 675f  {video_name}_bg_
-0002b9c0: 7375 6274 7261 6374 6564 7b65 7874 7d27  subtracted{ext}'
-0002b9d0: 290a 2020 2020 666f 7572 6363 203d 2063  ).    fourcc = c
-0002b9e0: 7632 2e56 6964 656f 5772 6974 6572 5f66  v2.VideoWriter_f
-0002b9f0: 6f75 7263 6328 2a46 6f72 6d61 7473 2e4d  ourcc(*Formats.M
-0002ba00: 5034 5f43 4f44 4543 2e76 616c 7565 290a  P4_CODEC.value).
-0002ba10: 2020 2020 7772 6974 6572 203d 2063 7632      writer = cv2
-0002ba20: 2e56 6964 656f 5772 6974 6572 2873 6176  .VideoWriter(sav
-0002ba30: 655f 7061 7468 2c20 666f 7572 6363 2c20  e_path, fourcc, 
-0002ba40: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
-0002ba50: 2766 7073 275d 2c0a 2020 2020 2020 2020  'fps'],.        
-0002ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ba70: 2020 2020 2028 7669 6465 6f5f 6d65 7461       (video_meta
-0002ba80: 5f64 6174 615b 2777 6964 7468 275d 2c20  _data['width'], 
-0002ba90: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
-0002baa0: 2768 6569 6768 7427 5d29 290a 2020 2020  'height'])).    
-0002bab0: 6267 5f66 726d 203d 2063 7265 6174 655f  bg_frm = create_
-0002bac0: 6176 6572 6167 655f 6672 6d28 7669 6465  average_frm(vide
-0002bad0: 6f5f 7061 7468 3d62 675f 7669 6465 6f5f  o_path=bg_video_
-0002bae0: 7061 7468 2c20 7374 6172 745f 6672 6d3d  path, start_frm=
-0002baf0: 6267 5f73 7461 7274 5f66 726d 2c20 656e  bg_start_frm, en
-0002bb00: 645f 6672 6d3d 6267 5f65 6e64 5f66 726d  d_frm=bg_end_frm
-0002bb10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bb30: 2020 7374 6172 745f 7469 6d65 3d62 675f    start_time=bg_
-0002bb40: 7374 6172 745f 7469 6d65 2c20 656e 645f  start_time, end_
-0002bb50: 7469 6d65 3d62 675f 656e 645f 7469 6d65  time=bg_end_time
-0002bb60: 290a 2020 2020 6267 5f66 726d 203d 2063  ).    bg_frm = c
-0002bb70: 7632 2e72 6573 697a 6528 6267 5f66 726d  v2.resize(bg_frm
-0002bb80: 2c20 2876 6964 656f 5f6d 6574 615f 6461  , (video_meta_da
-0002bb90: 7461 5b27 7769 6474 6827 5d2c 2076 6964  ta['width'], vid
-0002bba0: 656f 5f6d 6574 615f 6461 7461 5b27 6865  eo_meta_data['he
-0002bbb0: 6967 6874 275d 2929 0a20 2020 2062 6720  ight'])).    bg 
-0002bbc0: 3d20 6376 322e 6376 7443 6f6c 6f72 286e  = cv2.cvtColor(n
-0002bbd0: 702e 6675 6c6c 5f6c 696b 6528 6267 5f66  p.full_like(bg_f
-0002bbe0: 726d 2c20 6267 5f63 6f6c 6f72 292c 2063  rm, bg_color), c
-0002bbf0: 7632 2e43 4f4c 4f52 5f42 4752 3252 4742  v2.COLOR_BGR2RGB
-0002bc00: 290a 2020 2020 6361 7020 3d20 6376 322e  ).    cap = cv2.
-0002bc10: 5669 6465 6f43 6170 7475 7265 2876 6964  VideoCapture(vid
-0002bc20: 656f 5f70 6174 6829 0a20 2020 2066 726d  eo_path).    frm
-0002bc30: 5f63 6e74 203d 2030 0a20 2020 2077 6869  _cnt = 0.    whi
-0002bc40: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
-0002bc50: 2072 6574 2c20 6672 6d20 3d20 6361 702e   ret, frm = cap.
-0002bc60: 7265 6164 2829 0a20 2020 2020 2020 2069  read().        i
-0002bc70: 6620 6e6f 7420 7265 743a 0a20 2020 2020  f not ret:.     
-0002bc80: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-0002bc90: 2020 2020 2064 6966 6620 3d20 6376 322e       diff = cv2.
-0002bca0: 6162 7364 6966 6628 6672 6d2c 2062 675f  absdiff(frm, bg_
-0002bcb0: 6672 6d29 0a20 2020 2020 2020 2067 7261  frm).        gra
-0002bcc0: 795f 6469 6666 203d 2063 7632 2e63 7674  y_diff = cv2.cvt
-0002bcd0: 436f 6c6f 7228 6469 6666 2c20 6376 322e  Color(diff, cv2.
-0002bce0: 434f 4c4f 525f 4247 5232 4752 4159 290a  COLOR_BGR2GRAY).
-0002bcf0: 2020 2020 2020 2020 5f2c 206d 6173 6b20          _, mask 
-0002bd00: 3d20 6376 322e 7468 7265 7368 6f6c 6428  = cv2.threshold(
-0002bd10: 6772 6179 5f64 6966 662c 2035 302c 2032  gray_diff, 50, 2
-0002bd20: 3535 2c20 6376 322e 5448 5245 5348 5f42  55, cv2.THRESH_B
-0002bd30: 494e 4152 5929 0a20 2020 2020 2020 2069  INARY).        i
-0002bd40: 6620 6667 5f63 6f6c 6f72 2069 7320 4e6f  f fg_color is No
-0002bd50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002bd60: 6667 203d 2063 7632 2e62 6974 7769 7365  fg = cv2.bitwise
-0002bd70: 5f61 6e64 2866 726d 2c20 6672 6d2c 206d  _and(frm, frm, m
-0002bd80: 6173 6b3d 6d61 736b 290a 2020 2020 2020  ask=mask).      
-0002bd90: 2020 2020 2020 7265 7375 6c74 203d 2063        result = c
-0002bda0: 7632 2e61 6464 2862 672c 2066 6729 0a20  v2.add(bg, fg). 
-0002bdb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0002bdc0: 2020 2020 2020 2020 206d 6173 6b5f 696e           mask_in
-0002bdd0: 7620 3d20 6376 322e 6269 7477 6973 655f  v = cv2.bitwise_
-0002bde0: 6e6f 7428 6d61 736b 290a 2020 2020 2020  not(mask).      
-0002bdf0: 2020 2020 2020 6667 5f63 6c72 203d 2063        fg_clr = c
-0002be00: 7632 2e63 7674 436f 6c6f 7228 6e70 2e66  v2.cvtColor(np.f
-0002be10: 756c 6c5f 6c69 6b65 2866 726d 2c20 6667  ull_like(frm, fg
-0002be20: 5f63 6f6c 6f72 292c 2063 7632 2e43 4f4c  _color), cv2.COL
-0002be30: 4f52 5f42 4752 3252 4742 290a 2020 2020  OR_BGR2RGB).    
-0002be40: 2020 2020 2020 2020 6667 5f63 6c72 203d          fg_clr =
-0002be50: 2063 7632 2e62 6974 7769 7365 5f61 6e64   cv2.bitwise_and
-0002be60: 2866 675f 636c 722c 2066 675f 636c 722c  (fg_clr, fg_clr,
-0002be70: 206d 6173 6b3d 6d61 736b 290a 2020 2020   mask=mask).    
-0002be80: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002be90: 2063 7632 2e62 6974 7769 7365 5f61 6e64   cv2.bitwise_and
-0002bea0: 2862 672c 2062 672c 206d 6173 6b3d 6d61  (bg, bg, mask=ma
-0002beb0: 736b 5f69 6e76 290a 2020 2020 2020 2020  sk_inv).        
-0002bec0: 2020 2020 7265 7375 6c74 203d 2063 7632      result = cv2
-0002bed0: 2e61 6464 2872 6573 756c 742c 2066 675f  .add(result, fg_
-0002bee0: 636c 7229 0a20 2020 2020 2020 2077 7269  clr).        wri
-0002bef0: 7465 722e 7772 6974 6528 7265 7375 6c74  ter.write(result
-0002bf00: 290a 2020 2020 2020 2020 6672 6d5f 636e  ).        frm_cn
-0002bf10: 7420 2b3d 2031 0a20 2020 2020 2020 2070  t += 1.        p
-0002bf20: 7269 6e74 2866 2742 6163 6b67 726f 756e  rint(f'Backgroun
-0002bf30: 6420 7375 6274 7261 6374 696f 6e20 6672  d subtraction fr
-0002bf40: 616d 6520 7b66 726d 5f63 6e74 7d2f 7b76  ame {frm_cnt}/{v
-0002bf50: 6964 656f 5f6d 6574 615f 6461 7461 5b22  ideo_meta_data["
-0002bf60: 6672 616d 655f 636f 756e 7422 5d7d 2028  frame_count"]} (
-0002bf70: 5669 6465 6f3a 207b 7669 6465 6f5f 6e61  Video: {video_na
-0002bf80: 6d65 7d29 2729 0a0a 2020 2020 7772 6974  me})')..    writ
-0002bf90: 6572 2e72 656c 6561 7365 2829 0a20 2020  er.release().   
-0002bfa0: 2063 6170 2e72 656c 6561 7365 2829 0a20   cap.release(). 
-0002bfb0: 2020 2074 696d 6572 2e73 746f 705f 7469     timer.stop_ti
-0002bfc0: 6d65 7228 290a 2020 2020 7374 646f 7574  mer().    stdout
-0002bfd0: 5f73 7563 6365 7373 286d 7367 3d66 2742  _success(msg=f'B
-0002bfe0: 6163 6b67 726f 756e 6420 7375 6274 7261  ackground subtra
-0002bff0: 6374 6564 2066 726f 6d20 7b76 6964 656f  cted from {video
-0002c000: 5f6e 616d 657d 2061 6e64 2073 6176 6564  _name} and saved
-0002c010: 2061 7420 7b73 6176 655f 7061 7468 7d27   at {save_path}'
-0002c020: 2c20 656c 6170 7365 645f 7469 6d65 3d74  , elapsed_time=t
-0002c030: 696d 6572 2e65 6c61 7073 6564 5f74 696d  imer.elapsed_tim
-0002c040: 6529 0a0a 6465 6620 5f62 675f 7265 6d6f  e)..def _bg_remo
-0002c050: 7665 725f 6d70 2866 726d 5f72 616e 6765  ver_mp(frm_range
-0002c060: 3a20 5475 706c 655b 696e 742c 206e 702e  : Tuple[int, np.
-0002c070: 6e64 6172 7261 795d 2c0a 2020 2020 2020  ndarray],.      
-0002c080: 2020 2020 2020 2020 2020 2020 2076 6964               vid
-0002c090: 656f 5f70 6174 683a 2055 6e69 6f6e 5b73  eo_path: Union[s
-0002c0a0: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
-0002c0b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c0c0: 2020 2020 2062 675f 6672 6d3a 206e 702e       bg_frm: np.
-0002c0d0: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
-0002c0e0: 2020 2020 2020 2020 2020 2020 6267 5f63              bg_c
-0002c0f0: 6c72 3a20 5475 706c 655b 696e 742c 2069  lr: Tuple[int, i
-0002c100: 6e74 2c20 696e 745d 2c0a 2020 2020 2020  nt, int],.      
-0002c110: 2020 2020 2020 2020 2020 2020 2066 675f               fg_
-0002c120: 636c 723a 2054 7570 6c65 5b69 6e74 2c20  clr: Tuple[int, 
-0002c130: 696e 742c 2069 6e74 5d2c 0a20 2020 2020  int, int],.     
-0002c140: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0002c150: 6465 6f5f 6d65 7461 5f64 6174 613a 2044  deo_meta_data: D
-0002c160: 6963 745b 7374 722c 2041 6e79 5d2c 0a20  ict[str, Any],. 
-0002c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c180: 2020 7465 6d70 5f64 6972 3a20 556e 696f    temp_dir: Unio
-0002c190: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
-0002c1a0: 6b65 5d29 3a0a 0a20 2020 2062 6174 6368  ke]):..    batch
-0002c1b0: 2c20 6672 6d5f 7261 6e67 6520 3d20 6672  , frm_range = fr
-0002c1c0: 6d5f 7261 6e67 655b 305d 2c20 6672 6d5f  m_range[0], frm_
-0002c1d0: 7261 6e67 655b 315d 0a20 2020 2073 7461  range[1].    sta
-0002c1e0: 7274 5f66 726d 2c20 6375 7272 656e 745f  rt_frm, current_
-0002c1f0: 6672 6d2c 2065 6e64 5f66 726d 203d 2066  frm, end_frm = f
-0002c200: 726d 5f72 616e 6765 5b30 5d2c 2066 726d  rm_range[0], frm
-0002c210: 5f72 616e 6765 5b30 5d2c 2066 726d 5f72  _range[0], frm_r
-0002c220: 616e 6765 5b2d 315d 0a20 2020 2063 6170  ange[-1].    cap
-0002c230: 203d 2063 7632 2e56 6964 656f 4361 7074   = cv2.VideoCapt
-0002c240: 7572 6528 7669 6465 6f5f 7061 7468 290a  ure(video_path).
-0002c250: 2020 2020 666f 7572 6363 203d 2063 7632      fourcc = cv2
-0002c260: 2e56 6964 656f 5772 6974 6572 5f66 6f75  .VideoWriter_fou
-0002c270: 7263 6328 2a46 6f72 6d61 7473 2e4d 5034  rcc(*Formats.MP4
-0002c280: 5f43 4f44 4543 2e76 616c 7565 290a 2020  _CODEC.value).  
-0002c290: 2020 7361 7665 5f70 6174 6820 3d20 6f73    save_path = os
-0002c2a0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
-0002c2b0: 6469 722c 2066 227b 6261 7463 687d 2e6d  dir, f"{batch}.m
-0002c2c0: 7034 2229 0a20 2020 2063 6170 2e73 6574  p4").    cap.set
-0002c2d0: 2831 2c20 7374 6172 745f 6672 6d29 0a20  (1, start_frm). 
-0002c2e0: 2020 2077 7269 7465 7220 3d20 6376 322e     writer = cv2.
-0002c2f0: 5669 6465 6f57 7269 7465 7228 7361 7665  VideoWriter(save
-0002c300: 5f70 6174 682c 2066 6f75 7263 632c 2076  _path, fourcc, v
-0002c310: 6964 656f 5f6d 6574 615f 6461 7461 5b27  ideo_meta_data['
-0002c320: 6670 7327 5d2c 2028 7669 6465 6f5f 6d65  fps'], (video_me
-0002c330: 7461 5f64 6174 615b 2777 6964 7468 275d  ta_data['width']
-0002c340: 2c20 7669 6465 6f5f 6d65 7461 5f64 6174  , video_meta_dat
-0002c350: 615b 2768 6569 6768 7427 5d29 290a 2020  a['height'])).  
-0002c360: 2020 6267 203d 206e 702e 6675 6c6c 5f6c    bg = np.full_l
-0002c370: 696b 6528 6267 5f66 726d 2c20 6267 5f63  ike(bg_frm, bg_c
-0002c380: 6c72 290a 2020 2020 6267 203d 2062 675b  lr).    bg = bg[
-0002c390: 3a2c 203a 2c20 3a3a 2d31 5d0a 2020 2020  :, :, ::-1].    
-0002c3a0: 6469 722c 2076 6964 656f 5f6e 616d 652c  dir, video_name,
-0002c3b0: 2065 7874 203d 2067 6574 5f66 6e5f 6578   ext = get_fn_ex
-0002c3c0: 7428 6669 6c65 7061 7468 3d76 6964 656f  t(filepath=video
-0002c3d0: 5f70 6174 6829 0a20 2020 2077 6869 6c65  _path).    while
-0002c3e0: 2063 7572 7265 6e74 5f66 726d 203c 3d20   current_frm <= 
-0002c3f0: 656e 645f 6672 6d3a 0a20 2020 2020 2020  end_frm:.       
-0002c400: 2072 6574 2c20 6672 6d20 3d20 6361 702e   ret, frm = cap.
-0002c410: 7265 6164 2829 0a20 2020 2020 2020 2069  read().        i
-0002c420: 6620 6e6f 7420 7265 743a 0a20 2020 2020  f not ret:.     
-0002c430: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-0002c440: 2020 2020 2064 6966 6620 3d20 6376 322e       diff = cv2.
-0002c450: 6162 7364 6966 6628 6672 6d2c 2062 675f  absdiff(frm, bg_
-0002c460: 6672 6d29 0a20 2020 2020 2020 2062 2c20  frm).        b, 
-0002c470: 672c 2072 203d 2064 6966 665b 3a2c 203a  g, r = diff[:, :
-0002c480: 2c20 305d 2c20 6469 6666 5b3a 2c20 3a2c  , 0], diff[:, :,
-0002c490: 2031 5d2c 2064 6966 665b 3a2c 203a 2c20   1], diff[:, :, 
-0002c4a0: 325d 0a20 2020 2020 2020 2067 7261 795f  2].        gray_
-0002c4b0: 6469 6666 203d 2030 2e32 3938 3920 2a20  diff = 0.2989 * 
-0002c4c0: 7220 2b20 302e 3538 3730 202a 2067 202b  r + 0.5870 * g +
-0002c4d0: 2030 2e31 3134 3020 2a20 620a 2020 2020   0.1140 * b.    
-0002c4e0: 2020 2020 6772 6179 5f64 6966 6620 3d20      gray_diff = 
-0002c4f0: 6772 6179 5f64 6966 662e 6173 7479 7065  gray_diff.astype
-0002c500: 286e 702e 7569 6e74 3829 2020 2320 456e  (np.uint8)  # En
-0002c510: 7375 7265 2074 6865 2074 7970 6520 6973  sure the type is
-0002c520: 2075 696e 7438 0a20 2020 2020 2020 206d   uint8.        m
-0002c530: 6173 6b20 3d20 6e70 2e77 6865 7265 2867  ask = np.where(g
-0002c540: 7261 795f 6469 6666 203e 2035 302c 2032  ray_diff > 50, 2
-0002c550: 3535 2c20 3029 2e61 7374 7970 6528 6e70  55, 0).astype(np
-0002c560: 2e75 696e 7438 290a 2020 2020 2020 2020  .uint8).        
-0002c570: 6966 2066 675f 636c 7220 6973 204e 6f6e  if fg_clr is Non
-0002c580: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0002c590: 6720 3d20 6376 322e 6269 7477 6973 655f  g = cv2.bitwise_
-0002c5a0: 616e 6428 6672 6d2c 2066 726d 2c20 6d61  and(frm, frm, ma
-0002c5b0: 736b 3d6d 6173 6b29 0a20 2020 2020 2020  sk=mask).       
-0002c5c0: 2020 2020 2072 6573 756c 7420 3d20 6376       result = cv
-0002c5d0: 322e 6164 6428 6267 2c20 6667 290a 2020  2.add(bg, fg).  
-0002c5e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002c5f0: 2020 2020 2020 2020 6d61 736b 5f69 6e76          mask_inv
-0002c600: 203d 2063 7632 2e62 6974 7769 7365 5f6e   = cv2.bitwise_n
-0002c610: 6f74 286d 6173 6b29 0a20 2020 2020 2020  ot(mask).       
-0002c620: 2020 2020 2066 675f 636c 725f 696d 6720       fg_clr_img 
-0002c630: 3d20 6e70 2e66 756c 6c5f 6c69 6b65 2866  = np.full_like(f
-0002c640: 726d 2c20 6667 5f63 6c72 290a 2020 2020  rm, fg_clr).    
-0002c650: 2020 2020 2020 2020 6667 5f63 6c72 5f69          fg_clr_i
-0002c660: 6d67 203d 2066 675f 636c 725f 696d 675b  mg = fg_clr_img[
-0002c670: 3a2c 203a 2c20 3a3a 2d31 5d0a 2020 2020  :, :, ::-1].    
-0002c680: 2020 2020 2020 2020 6667 5f63 6c72 5f69          fg_clr_i
-0002c690: 6d67 203d 2063 7632 2e62 6974 7769 7365  mg = cv2.bitwise
-0002c6a0: 5f61 6e64 2866 675f 636c 725f 696d 672c  _and(fg_clr_img,
-0002c6b0: 2066 675f 636c 725f 696d 672c 206d 6173   fg_clr_img, mas
-0002c6c0: 6b3d 6d61 736b 290a 2020 2020 2020 2020  k=mask).        
-0002c6d0: 2020 2020 7265 7375 6c74 203d 2063 7632      result = cv2
-0002c6e0: 2e62 6974 7769 7365 5f61 6e64 2862 672c  .bitwise_and(bg,
-0002c6f0: 2062 672c 206d 6173 6b3d 6d61 736b 5f69   bg, mask=mask_i
-0002c700: 6e76 290a 2020 2020 2020 2020 2020 2020  nv).            
-0002c710: 7265 7375 6c74 203d 2063 7632 2e61 6464  result = cv2.add
-0002c720: 2872 6573 756c 742c 2066 675f 636c 725f  (result, fg_clr_
-0002c730: 696d 6729 0a20 2020 2020 2020 2077 7269  img).        wri
-0002c740: 7465 722e 7772 6974 6528 7265 7375 6c74  ter.write(result
-0002c750: 290a 2020 2020 2020 2020 6375 7272 656e  ).        curren
-0002c760: 745f 6672 6d20 2b3d 2031 0a20 2020 2020  t_frm += 1.     
-0002c770: 2020 2070 7269 6e74 2866 2742 6163 6b67     print(f'Backg
-0002c780: 726f 756e 6420 7375 6274 7261 6374 696f  round subtractio
-0002c790: 6e20 6672 616d 6520 7b63 7572 7265 6e74  n frame {current
-0002c7a0: 5f66 726d 7d2f 7b76 6964 656f 5f6d 6574  _frm}/{video_met
-0002c7b0: 615f 6461 7461 5b22 6672 616d 655f 636f  a_data["frame_co
-0002c7c0: 756e 7422 5d7d 2028 5669 6465 6f3a 207b  unt"]} (Video: {
-0002c7d0: 7669 6465 6f5f 6e61 6d65 7d29 2729 0a20  video_name})'). 
-0002c7e0: 2020 2077 7269 7465 722e 7265 6c65 6173     writer.releas
-0002c7f0: 6528 290a 2020 2020 6361 702e 7265 6c65  e().    cap.rele
-0002c800: 6173 6528 290a 2020 2020 7265 7475 726e  ase().    return
-0002c810: 2062 6174 6368 0a0a 6465 6620 7669 6465   batch..def vide
-0002c820: 6f5f 6267 5f73 7562 7374 7261 6374 696f  o_bg_substractio
-0002c830: 6e5f 6d70 2876 6964 656f 5f70 6174 683a  n_mp(video_path:
-0002c840: 2055 6e69 6f6e 5b73 7472 2c20 6f73 2e50   Union[str, os.P
-0002c850: 6174 684c 696b 655d 2c0a 2020 2020 2020  athLike],.      
-0002c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c870: 2020 2020 2020 2062 675f 7669 6465 6f5f         bg_video_
-0002c880: 7061 7468 3a20 4f70 7469 6f6e 616c 5b55  path: Optional[U
-0002c890: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-0002c8a0: 684c 696b 655d 5d20 3d20 4e6f 6e65 2c0a  hLike]] = None,.
-0002c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c8c0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
-0002c8d0: 7374 6172 745f 6672 6d3a 204f 7074 696f  start_frm: Optio
-0002c8e0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0002c8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c900: 2020 2020 2020 2020 2020 2020 2020 6267                bg
-0002c910: 5f65 6e64 5f66 726d 3a20 4f70 7469 6f6e  _end_frm: Option
-0002c920: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-0002c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c940: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
-0002c950: 7374 6172 745f 7469 6d65 3a20 4f70 7469  start_time: Opti
-0002c960: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0002c970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c980: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002c990: 675f 656e 645f 7469 6d65 3a20 4f70 7469  g_end_time: Opti
-0002c9a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0002c9b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002c9c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002c9d0: 675f 636f 6c6f 723a 204f 7074 696f 6e61  g_color: Optiona
-0002c9e0: 6c5b 5475 706c 655b 696e 742c 2069 6e74  l[Tuple[int, int
-0002c9f0: 2c20 696e 745d 5d20 3d20 2830 2c20 302c  , int]] = (0, 0,
-0002ca00: 2030 292c 0a20 2020 2020 2020 2020 2020   0),.           
+00029b40: 2073 7461 7274 5f66 726d 3a20 4f70 7469   start_frm: Opti
+00029b50: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00029b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029b70: 2020 2020 2020 2020 2065 6e64 5f66 726d           end_frm
+00029b80: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00029b90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00029ba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00029bb0: 7461 7274 5f74 696d 653a 204f 7074 696f  tart_time: Optio
+00029bc0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00029bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029be0: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
+00029bf0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00029c00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00029c10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00029c20: 6176 655f 7061 7468 3a20 4f70 7469 6f6e  ave_path: Option
+00029c30: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+00029c40: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
+00029c50: 6e65 2920 2d3e 2055 6e69 6f6e 5b4e 6f6e  ne) -> Union[Non
+00029c60: 652c 206e 702e 6e64 6172 7261 795d 3a0a  e, np.ndarray]:.
+00029c70: 2020 2020 2222 220a 2020 2020 4372 6561      """.    Crea
+00029c80: 7465 2061 6e20 696d 6167 6520 7265 7072  te an image repr
+00029c90: 6573 656e 7469 6e67 2074 6865 2061 7665  esenting the ave
+00029ca0: 7261 6765 2066 7261 6d65 206f 6620 6120  rage frame of a 
+00029cb0: 7365 676d 656e 7420 696e 2061 2076 6964  segment in a vid
+00029cc0: 656f 206f 7220 616e 2065 6e74 6972 6520  eo or an entire 
+00029cd0: 7669 6465 6f2e 0a0a 2020 2020 2e2e 206e  video...    .. n
+00029ce0: 6f74 653a 3a0a 2020 2020 2020 2055 7365  ote::.       Use
+00029cf0: 6675 6c20 6865 6c70 6572 2066 6f72 2065  ful helper for e
+00029d00: 2e67 2e2c 2076 6964 656f 2062 6163 6b67  .g., video backg
+00029d10: 726f 756e 6420 7375 6274 7261 6374 696f  round subtractio
+00029d20: 6e20 6060 7369 6d62 612e 7669 6465 6f5f  n ``simba.video_
+00029d30: 7072 6f63 6573 736f 7273 2e76 6964 656f  processors.video
+00029d40: 5f70 726f 6365 7373 696e 672e 7669 6465  _processing.vide
+00029d50: 6f5f 6267 5f73 7562 7374 7261 6374 696f  o_bg_substractio
+00029d60: 6e28 2960 600a 2020 2020 2020 2045 6974  n()``.       Eit
+00029d70: 6865 7220 7061 7373 2060 6073 7461 7274  her pass ``start
+00029d80: 5f66 726d 6060 2061 6e64 2060 6065 6e64  _frm`` and ``end
+00029d90: 5f66 726d 6060 204f 5220 6060 7374 6172  _frm`` OR ``star
+00029da0: 745f 7469 6d65 6060 2061 6e64 2060 6065  t_time`` and ``e
+00029db0: 6e64 5f74 696d 6560 6020 4f52 2070 6173  nd_time`` OR pas
+00029dc0: 7320 616c 6c20 666f 7572 2061 7267 756d  s all four argum
+00029dd0: 656e 7473 2061 7320 4e6f 6e65 2e0a 2020  ents as None..  
+00029de0: 2020 2020 2049 6620 616c 6c20 6172 6520       If all are 
+00029df0: 4e6f 6e65 2c20 7468 656e 2074 6865 2065  None, then the e
+00029e00: 6e74 6972 6520 7669 6465 6f20 7769 6c6c  ntire video will
+00029e10: 2062 6520 7573 6564 2074 6f20 6372 6561   be used to crea
+00029e20: 7465 2074 6865 2061 7665 7261 6765 2066  te the average f
+00029e30: 7261 6d65 2e0a 0a20 2020 203a 7061 7261  rame...    :para
+00029e40: 6d20 556e 696f 6e5b 7374 722c 206f 732e  m Union[str, os.
+00029e50: 5061 7468 4c69 6b65 5d20 7669 6465 6f5f  PathLike] video_
+00029e60: 7061 7468 3a20 5468 6520 7061 7468 2074  path: The path t
+00029e70: 6f20 7468 6520 7669 6465 6f20 746f 2063  o the video to c
+00029e80: 7265 6174 6520 7468 6520 6176 6572 6167  reate the averag
+00029e90: 6520 6672 616d 6520 6672 6f6d 2e20 4465  e frame from. De
+00029ea0: 6661 756c 743a 204e 6f6e 652e 0a20 2020  fault: None..   
+00029eb0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+00029ec0: 5b69 6e74 5d20 7374 6172 745f 6672 6d3a  [int] start_frm:
+00029ed0: 2054 6865 2066 6972 7374 2066 7261 6d65   The first frame
+00029ee0: 2069 6e20 7468 6520 7365 676d 656e 7420   in the segment 
+00029ef0: 746f 2063 7265 6174 6520 7468 6520 6176  to create the av
+00029f00: 6572 6167 6520 6672 616d 6520 6672 6f6d  erage frame from
+00029f10: 2e20 4465 6661 756c 743a 204e 6f6e 652e  . Default: None.
+00029f20: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+00029f30: 6f6e 616c 5b69 6e74 5d20 656e 645f 6672  onal[int] end_fr
+00029f40: 6d3a 2054 6865 206c 6173 7420 6672 616d  m: The last fram
+00029f50: 6520 696e 2074 6865 2073 6567 6d65 6e74  e in the segment
+00029f60: 2074 6f20 6372 6561 7465 2074 6865 2061   to create the a
+00029f70: 7665 7261 6765 2066 7261 6d65 2066 726f  verage frame fro
+00029f80: 6d2e 2044 6566 6175 6c74 3a20 4e6f 6e65  m. Default: None
+00029f90: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+00029fa0: 696f 6e61 6c5b 7374 725d 2073 7461 7274  ional[str] start
+00029fb0: 5f74 696d 653a 2054 6865 2073 7461 7274  _time: The start
+00029fc0: 2074 696d 6573 7461 6d70 2069 6e20 6048   timestamp in `H
+00029fd0: 483a 4d4d 3a53 5360 2066 6f72 6d61 7420  H:MM:SS` format 
+00029fe0: 696e 2074 6865 2073 6567 6d65 6e74 2074  in the segment t
+00029ff0: 6f20 6372 6561 7465 2074 6865 2061 7665  o create the ave
+0002a000: 7261 6765 2066 7261 6d65 2066 726f 6d2e  rage frame from.
+0002a010: 2044 6566 6175 6c74 3a20 4e6f 6e65 2e0a   Default: None..
+0002a020: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+0002a030: 6e61 6c5b 7374 725d 2065 6e64 5f74 696d  nal[str] end_tim
+0002a040: 653a 2054 6865 2065 6e64 2074 696d 6573  e: The end times
+0002a050: 7461 6d70 2069 6e20 6048 483a 4d4d 3a53  tamp in `HH:MM:S
+0002a060: 5360 2066 6f72 6d61 7420 696e 2074 6865  S` format in the
+0002a070: 2073 6567 6d65 6e74 2074 6f20 6372 6561   segment to crea
+0002a080: 7465 2074 6865 2061 7665 7261 6765 2066  te the average f
+0002a090: 7261 6d65 2066 726f 6d2e 2044 6566 6175  rame from. Defau
+0002a0a0: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a70  lt: None..    :p
+0002a0b0: 6172 616d 204f 7074 696f 6e61 6c5b 556e  aram Optional[Un
+0002a0c0: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
+0002a0d0: 4c69 6b65 5d5d 2073 6176 655f 7061 7468  Like]] save_path
+0002a0e0: 3a20 5468 6520 7061 7468 2074 6f20 7768  : The path to wh
+0002a0f0: 6572 6520 746f 2073 6176 6520 7468 6520  ere to save the 
+0002a100: 6176 6572 6167 6520 696d 6167 652e 2049  average image. I
+0002a110: 6620 4e6f 6e65 2c20 7468 656e 2072 6561  f None, then rea
+0002a120: 7475 7265 6e73 2074 6865 2061 7665 7261  turens the avera
+0002a130: 6765 2069 6d61 6765 2069 6e20 6e70 2c6e  ge image in np,n
+0002a140: 6461 7272 6179 2066 6f72 6d61 742e 2044  darray format. D
+0002a150: 6566 6175 6c74 3a20 4e6f 6e65 2e0a 2020  efault: None..  
+0002a160: 2020 3a72 6574 7572 6e20 556e 696f 6e5b    :return Union[
+0002a170: 4e6f 6e65 2c20 6e70 2e6e 6461 7272 6179  None, np.ndarray
+0002a180: 5d3a 2054 6865 2061 7665 7261 6765 2069  ]: The average i
+0002a190: 6d61 6765 2028 6966 2060 6073 6176 655f  mage (if ``save_
+0002a1a0: 7061 7468 6060 2069 7320 6e6f 7420 4e6f  path`` is not No
+0002a1b0: 6e65 2920 6f72 204e 6f6e 6520 6966 2020  ne) or None if  
+0002a1c0: 6060 7361 7665 5f70 6174 6860 6020 6973  ``save_path`` is
+0002a1d0: 2070 6173 7365 642e 0a20 2020 2022 2222   passed..    """
+0002a1e0: 0a0a 2020 2020 6966 2028 2873 7461 7274  ..    if ((start
+0002a1f0: 5f66 726d 2069 7320 6e6f 7420 4e6f 6e65  _frm is not None
+0002a200: 2920 6f72 2028 656e 645f 6672 6d20 6973  ) or (end_frm is
+0002a210: 206e 6f74 204e 6f6e 6529 2920 616e 6420   not None)) and 
+0002a220: 2828 7374 6172 745f 7469 6d65 2069 7320  ((start_time is 
+0002a230: 6e6f 7420 4e6f 6e65 2920 6f72 2028 656e  not None) or (en
+0002a240: 645f 7469 6d65 2069 7320 6e6f 7420 4e6f  d_time is not No
+0002a250: 6e65 2929 3a0a 2020 2020 2020 2020 7261  ne)):.        ra
+0002a260: 6973 6520 496e 7661 6c69 6449 6e70 7574  ise InvalidInput
+0002a270: 4572 726f 7228 6d73 673d 6627 5061 7373  Error(msg=f'Pass
+0002a280: 2073 7461 7274 5f66 726d 2061 6e64 2065   start_frm and e
+0002a290: 6e64 5f66 726d 204f 5220 7374 6172 745f  nd_frm OR start_
+0002a2a0: 7469 6d65 2061 6e64 2065 6e64 5f74 696d  time and end_tim
+0002a2b0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+0002a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2d0: 2020 2020 736f 7572 6365 3d63 7265 6174      source=creat
+0002a2e0: 655f 6176 6572 6167 655f 6672 6d2e 5f5f  e_average_frm.__
+0002a2f0: 6e61 6d65 5f5f 290a 2020 2020 656c 6966  name__).    elif
+0002a300: 2074 7970 6528 7374 6172 745f 6672 6d29   type(start_frm)
+0002a310: 2021 3d20 7479 7065 2865 6e64 5f66 726d   != type(end_frm
+0002a320: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+0002a330: 2049 6e76 616c 6964 496e 7075 7445 7272   InvalidInputErr
+0002a340: 6f72 286d 7367 3d66 2750 6173 7320 7374  or(msg=f'Pass st
+0002a350: 6172 7420 6672 616d 6520 616e 6420 656e  art frame and en
+0002a360: 6420 6672 616d 6527 2c20 736f 7572 6365  d frame', source
+0002a370: 3d63 7265 6174 655f 6176 6572 6167 655f  =create_average_
+0002a380: 6672 6d2e 5f5f 6e61 6d65 5f5f 290a 2020  frm.__name__).  
+0002a390: 2020 656c 6966 2074 7970 6528 7374 6172    elif type(star
+0002a3a0: 745f 7469 6d65 2920 213d 2074 7970 6528  t_time) != type(
+0002a3b0: 656e 645f 7469 6d65 293a 0a20 2020 2020  end_time):.     
+0002a3c0: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+0002a3d0: 496e 7075 7445 7272 6f72 286d 7367 3d66  InputError(msg=f
+0002a3e0: 2750 6173 7320 7374 6172 7420 7469 6d65  'Pass start time
+0002a3f0: 2061 6e64 2065 6e64 2074 696d 6527 2c20   and end time', 
+0002a400: 736f 7572 6365 3d63 7265 6174 655f 6176  source=create_av
+0002a410: 6572 6167 655f 6672 6d2e 5f5f 6e61 6d65  erage_frm.__name
+0002a420: 5f5f 290a 2020 2020 6368 6563 6b5f 6669  __).    check_fi
+0002a430: 6c65 5f65 7869 7374 5f61 6e64 5f72 6561  le_exist_and_rea
+0002a440: 6461 626c 6528 6669 6c65 5f70 6174 683d  dable(file_path=
+0002a450: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
+0002a460: 7669 6465 6f5f 6d65 7461 5f64 6174 6120  video_meta_data 
+0002a470: 3d20 6765 745f 7669 6465 6f5f 6d65 7461  = get_video_meta
+0002a480: 5f64 6174 6128 7669 6465 6f5f 7061 7468  _data(video_path
+0002a490: 3d76 6964 656f 5f70 6174 6829 0a20 2020  =video_path).   
+0002a4a0: 2063 6170 203d 2063 7632 2e56 6964 656f   cap = cv2.Video
+0002a4b0: 4361 7074 7572 6528 7669 6465 6f5f 7061  Capture(video_pa
+0002a4c0: 7468 290a 2020 2020 6966 2028 7374 6172  th).    if (star
+0002a4d0: 745f 6672 6d20 6973 206e 6f74 204e 6f6e  t_frm is not Non
+0002a4e0: 6529 2061 6e64 2028 656e 645f 6672 6d20  e) and (end_frm 
+0002a4f0: 6973 206e 6f74 204e 6f6e 6529 3a0a 2020  is not None):.  
+0002a500: 2020 2020 2020 6368 6563 6b5f 696e 7428        check_int(
+0002a510: 6e61 6d65 3d27 7374 6172 745f 6672 6d27  name='start_frm'
+0002a520: 2c20 7661 6c75 653d 7374 6172 745f 6672  , value=start_fr
+0002a530: 6d2c 206d 696e 5f76 616c 7565 3d30 2c20  m, min_value=0, 
+0002a540: 6d61 785f 7661 6c75 653d 7669 6465 6f5f  max_value=video_
+0002a550: 6d65 7461 5f64 6174 615b 2766 7261 6d65  meta_data['frame
+0002a560: 5f63 6f75 6e74 275d 290a 2020 2020 2020  _count']).      
+0002a570: 2020 6368 6563 6b5f 696e 7428 6e61 6d65    check_int(name
+0002a580: 3d27 656e 645f 6672 6d27 2c20 7661 6c75  ='end_frm', valu
+0002a590: 653d 656e 645f 6672 6d2c 206d 696e 5f76  e=end_frm, min_v
+0002a5a0: 616c 7565 3d30 2c20 6d61 785f 7661 6c75  alue=0, max_valu
+0002a5b0: 653d 7669 6465 6f5f 6d65 7461 5f64 6174  e=video_meta_dat
+0002a5c0: 615b 2766 7261 6d65 5f63 6f75 6e74 275d  a['frame_count']
+0002a5d0: 290a 2020 2020 2020 2020 6966 2073 7461  ).        if sta
+0002a5e0: 7274 5f66 726d 203e 2065 6e64 5f66 726d  rt_frm > end_frm
+0002a5f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0002a600: 6973 6520 496e 7661 6c69 6449 6e70 7574  ise InvalidInput
+0002a610: 4572 726f 7228 6d73 673d 6627 5374 6172  Error(msg=f'Star
+0002a620: 7420 6672 616d 6520 287b 7374 6172 745f  t frame ({start_
+0002a630: 6672 6d7d 2920 6861 7320 746f 2062 6520  frm}) has to be 
+0002a640: 6265 666f 7265 2065 6e64 2066 7261 6d65  before end frame
+0002a650: 2028 7b65 6e64 5f66 726d 7d29 2e27 2c0a   ({end_frm}).',.
+0002a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a680: 2020 2020 736f 7572 6365 3d63 7265 6174      source=creat
+0002a690: 655f 6176 6572 6167 655f 6672 6d2e 5f5f  e_average_frm.__
+0002a6a0: 6e61 6d65 5f5f 290a 2020 2020 2020 2020  name__).        
+0002a6b0: 6672 616d 655f 6964 7320 3d20 6c69 7374  frame_ids = list
+0002a6c0: 2872 616e 6765 2873 7461 7274 5f66 726d  (range(start_frm
+0002a6d0: 2c20 656e 645f 6672 6d20 2b20 3129 290a  , end_frm + 1)).
+0002a6e0: 2020 2020 656c 6966 2028 7374 6172 745f      elif (start_
+0002a6f0: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
+0002a700: 2920 616e 6420 2865 6e64 5f74 696d 6520  ) and (end_time 
+0002a710: 6973 206e 6f74 204e 6f6e 6529 3a0a 2020  is not None):.  
+0002a720: 2020 2020 2020 6368 6563 6b5f 6966 5f73        check_if_s
+0002a730: 7472 696e 675f 7661 6c75 655f 6973 5f76  tring_value_is_v
+0002a740: 616c 6964 5f76 6964 656f 5f74 696d 6573  alid_video_times
+0002a750: 7461 6d70 2876 616c 7565 3d73 7461 7274  tamp(value=start
+0002a760: 5f74 696d 652c 206e 616d 653d 6372 6561  _time, name=crea
+0002a770: 7465 5f61 7665 7261 6765 5f66 726d 2e5f  te_average_frm._
+0002a780: 5f6e 616d 655f 5f29 0a20 2020 2020 2020  _name__).       
+0002a790: 2063 6865 636b 5f69 665f 7374 7269 6e67   check_if_string
+0002a7a0: 5f76 616c 7565 5f69 735f 7661 6c69 645f  _value_is_valid_
+0002a7b0: 7669 6465 6f5f 7469 6d65 7374 616d 7028  video_timestamp(
+0002a7c0: 7661 6c75 653d 656e 645f 7469 6d65 2c20  value=end_time, 
+0002a7d0: 6e61 6d65 3d63 7265 6174 655f 6176 6572  name=create_aver
+0002a7e0: 6167 655f 6672 6d2e 5f5f 6e61 6d65 5f5f  age_frm.__name__
+0002a7f0: 290a 2020 2020 2020 2020 6368 6563 6b5f  ).        check_
+0002a800: 7468 6174 5f68 686d 6d73 735f 7374 6172  that_hhmmss_star
+0002a810: 745f 6973 5f62 6566 6f72 655f 656e 6428  t_is_before_end(
+0002a820: 7374 6172 745f 7469 6d65 3d73 7461 7274  start_time=start
+0002a830: 5f74 696d 652c 2065 6e64 5f74 696d 653d  _time, end_time=
+0002a840: 656e 645f 7469 6d65 2c0a 2020 2020 2020  end_time,.      
+0002a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a870: 2020 2020 2020 2020 6e61 6d65 3d63 7265          name=cre
+0002a880: 6174 655f 6176 6572 6167 655f 6672 6d2e  ate_average_frm.
+0002a890: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
+0002a8a0: 2020 6368 6563 6b5f 6966 5f68 686d 6d73    check_if_hhmms
+0002a8b0: 735f 7469 6d65 7374 616d 705f 6973 5f76  s_timestamp_is_v
+0002a8c0: 616c 6964 5f70 6172 745f 6f66 5f76 6964  alid_part_of_vid
+0002a8d0: 656f 2874 696d 6573 7461 6d70 3d73 7461  eo(timestamp=sta
+0002a8e0: 7274 5f74 696d 652c 2076 6964 656f 5f70  rt_time, video_p
+0002a8f0: 6174 683d 7669 6465 6f5f 7061 7468 290a  ath=video_path).
+0002a900: 2020 2020 2020 2020 6672 616d 655f 6964          frame_id
+0002a910: 7320 3d20 6669 6e64 5f66 7261 6d65 5f6e  s = find_frame_n
+0002a920: 756d 6265 7273 5f66 726f 6d5f 7469 6d65  umbers_from_time
+0002a930: 5f73 7461 6d70 2873 7461 7274 5f74 696d  _stamp(start_tim
+0002a940: 653d 7374 6172 745f 7469 6d65 2c20 656e  e=start_time, en
+0002a950: 645f 7469 6d65 3d65 6e64 5f74 696d 652c  d_time=end_time,
+0002a960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a990: 2020 2020 2020 2020 6670 733d 7669 6465          fps=vide
+0002a9a0: 6f5f 6d65 7461 5f64 6174 615b 2766 7073  o_meta_data['fps
+0002a9b0: 275d 290a 2020 2020 656c 7365 3a0a 2020  ']).    else:.  
+0002a9c0: 2020 2020 2020 6672 616d 655f 6964 7320        frame_ids 
+0002a9d0: 3d20 6c69 7374 2872 616e 6765 2830 2c20  = list(range(0, 
+0002a9e0: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+0002a9f0: 2766 7261 6d65 5f63 6f75 6e74 275d 2929  'frame_count']))
+0002aa00: 0a20 2020 2063 6170 2e73 6574 2830 2c20  .    cap.set(0, 
+0002aa10: 6672 616d 655f 6964 735b 305d 290a 2020  frame_ids[0]).  
+0002aa20: 2020 6267 5f73 756d 2c20 6672 6d5f 636e    bg_sum, frm_cn
+0002aa30: 742c 2066 726d 5f6c 656e 203d 204e 6f6e  t, frm_len = Non
+0002aa40: 652c 2030 2c20 6c65 6e28 6672 616d 655f  e, 0, len(frame_
+0002aa50: 6964 7329 0a20 2020 2077 6869 6c65 2066  ids).    while f
+0002aa60: 726d 5f63 6e74 203c 3d20 6672 6d5f 6c65  rm_cnt <= frm_le
+0002aa70: 6e3a 0a20 2020 2020 2020 2072 6574 2c20  n:.        ret, 
+0002aa80: 6672 6d20 3d20 6361 702e 7265 6164 2829  frm = cap.read()
+0002aa90: 0a20 2020 2020 2020 2069 6620 6267 5f73  .        if bg_s
+0002aaa0: 756d 2069 7320 4e6f 6e65 3a20 6267 5f73  um is None: bg_s
+0002aab0: 756d 203d 206e 702e 666c 6f61 7433 3228  um = np.float32(
+0002aac0: 6672 6d29 0a20 2020 2020 2020 2065 6c73  frm).        els
+0002aad0: 653a 2063 7632 2e61 6363 756d 756c 6174  e: cv2.accumulat
+0002aae0: 6528 6672 6d2c 2062 675f 7375 6d29 0a20  e(frm, bg_sum). 
+0002aaf0: 2020 2020 2020 2066 726d 5f63 6e74 202b         frm_cnt +
+0002ab00: 3d20 310a 2020 2020 696d 6720 3d20 6376  = 1.    img = cv
+0002ab10: 322e 636f 6e76 6572 7453 6361 6c65 4162  2.convertScaleAb
+0002ab20: 7328 6267 5f73 756d 202f 2066 726d 5f6c  s(bg_sum / frm_l
+0002ab30: 656e 290a 2020 2020 6361 702e 7265 6c65  en).    cap.rele
+0002ab40: 6173 6528 290a 2020 2020 6966 2073 6176  ase().    if sav
+0002ab50: 655f 7061 7468 2069 7320 6e6f 7420 4e6f  e_path is not No
+0002ab60: 6e65 3a0a 2020 2020 2020 2020 6368 6563  ne:.        chec
+0002ab70: 6b5f 6966 5f64 6972 5f65 7869 7374 7328  k_if_dir_exists(
+0002ab80: 696e 5f64 6972 3d6f 732e 7061 7468 2e64  in_dir=os.path.d
+0002ab90: 6972 6e61 6d65 2873 6176 655f 7061 7468  irname(save_path
+0002aba0: 292c 2073 6f75 7263 653d 6372 6561 7465  ), source=create
+0002abb0: 5f61 7665 7261 6765 5f66 726d 2e5f 5f6e  _average_frm.__n
+0002abc0: 616d 655f 5f29 0a20 2020 2020 2020 2063  ame__).        c
+0002abd0: 7632 2e69 6d77 7269 7465 2873 6176 655f  v2.imwrite(save_
+0002abe0: 7061 7468 2c20 696d 6729 0a20 2020 2065  path, img).    e
+0002abf0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+0002ac00: 7572 6e20 696d 670a 0a0a 6465 6620 7669  urn img...def vi
+0002ac10: 6465 6f5f 6267 5f73 7562 7472 6163 7469  deo_bg_subtracti
+0002ac20: 6f6e 2876 6964 656f 5f70 6174 683a 2055  on(video_path: U
+0002ac30: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002ac40: 684c 696b 655d 2c0a 2020 2020 2020 2020  hLike],.        
+0002ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ac60: 2020 6267 5f76 6964 656f 5f70 6174 683a    bg_video_path:
+0002ac70: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0002ac80: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002ac90: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0002aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002acb0: 2020 2020 2062 675f 7374 6172 745f 6672       bg_start_fr
+0002acc0: 6d3a 204f 7074 696f 6e61 6c5b 696e 745d  m: Optional[int]
+0002acd0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002acf0: 2020 2062 675f 656e 645f 6672 6d3a 204f     bg_end_frm: O
+0002ad00: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0002ad10: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0002ad20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0002ad30: 675f 7374 6172 745f 7469 6d65 3a20 4f70  g_start_time: Op
+0002ad40: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0002ad50: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0002ad60: 2020 2020 2020 2020 2020 2020 2020 6267                bg
+0002ad70: 5f65 6e64 5f74 696d 653a 204f 7074 696f  _end_time: Optio
+0002ad80: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0002ad90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ada0: 2020 2020 2020 2020 2020 2062 675f 636f             bg_co
+0002adb0: 6c6f 723a 204f 7074 696f 6e61 6c5b 5475  lor: Optional[Tu
+0002adc0: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
+0002add0: 745d 5d20 3d20 2830 2c20 302c 2030 292c  t]] = (0, 0, 0),
+0002ade0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002adf0: 2020 2020 2020 2020 2020 2066 675f 636f             fg_co
+0002ae00: 6c6f 723a 204f 7074 696f 6e61 6c5b 5475  lor: Optional[Tu
+0002ae10: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
+0002ae20: 745d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  t]] = None,.    
+0002ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ae40: 2020 2020 2020 7361 7665 5f70 6174 683a        save_path:
+0002ae50: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0002ae60: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002ae70: 5d5d 203d 204e 6f6e 6529 202d 3e20 4e6f  ]] = None) -> No
+0002ae80: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
+0002ae90: 5375 6274 7261 6374 2074 6865 2062 6163  Subtract the bac
+0002aea0: 6b67 726f 756e 6420 6672 6f6d 2061 2076  kground from a v
+0002aeb0: 6964 656f 2e0a 0a20 2020 202e 2e20 7669  ideo...    .. vi
+0002aec0: 6465 6f3a 3a20 5f73 7461 7469 632f 696d  deo:: _static/im
+0002aed0: 672f 7669 6465 6f5f 6267 5f73 7562 7472  g/video_bg_subtr
+0002aee0: 6163 7469 6f6e 2e77 6562 6d0a 2020 2020  action.webm.    
+0002aef0: 2020 203a 6c6f 6f70 3a0a 0a20 2020 202e     :loop:..    .
+0002af00: 2e20 6e6f 7465 3a3a 0a20 2020 2020 2020  . note::.       
+0002af10: 4966 2020 6060 6267 5f76 6964 656f 5f70  If  ``bg_video_p
+0002af20: 6174 6860 6020 6973 2070 6173 7365 642c  ath`` is passed,
+0002af30: 2074 6861 7420 7669 6465 6f20 7769 6c6c   that video will
+0002af40: 2062 6520 7573 6564 2074 6f20 7061 7273   be used to pars
+0002af50: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
+0002af60: 2e20 4966 204e 6f6e 652c 2060 6076 6964  . If None, ``vid
+0002af70: 656f 5f70 6174 6860 6020 7769 6c6c 2062  eo_path`` will b
+0002af80: 6520 7573 6520 6474 6f20 7061 7273 6520  e use dto parse 
+0002af90: 6261 636b 6772 6f75 6e64 2e0a 2020 2020  background..    
+0002afa0: 2020 2045 6974 6865 7220 7061 7373 2060     Either pass `
+0002afb0: 6073 7461 7274 5f66 726d 6060 2061 6e64  `start_frm`` and
+0002afc0: 2060 6065 6e64 5f66 726d 6060 204f 5220   ``end_frm`` OR 
+0002afd0: 6060 7374 6172 745f 7469 6d65 6060 2061  ``start_time`` a
+0002afe0: 6e64 2060 6065 6e64 5f74 696d 6560 6020  nd ``end_time`` 
+0002aff0: 4f52 2070 6173 7320 616c 6c20 666f 7572  OR pass all four
+0002b000: 2061 7267 756d 656e 7473 2061 7320 4e6f   arguments as No
+0002b010: 6e65 2e0a 2020 2020 2020 2054 686f 7365  ne..       Those
+0002b020: 2074 776f 2061 7267 756d 656e 7473 2077   two arguments w
+0002b030: 696c 6c20 6265 2075 7365 6420 746f 2073  ill be used to s
+0002b040: 6c69 6365 2074 6865 2062 6163 6b67 726f  lice the backgro
+0002b050: 756e 6420 7669 6465 6f2c 2061 6e64 2074  und video, and t
+0002b060: 6865 2073 6c69 6365 6420 7061 7274 2069  he sliced part i
+0002b070: 7320 7573 6564 2074 6f20 7061 7273 6520  s used to parse 
+0002b080: 7468 6520 6261 636b 6772 6f75 6e64 2e0a  the background..
+0002b090: 0a20 2020 2020 2020 466f 7220 6578 616d  .       For exam
+0002b0a0: 706c 652c 2069 6e20 7468 6520 7363 656e  ple, in the scen
+0002b0b0: 6172 696f 2077 6865 7265 2074 6865 7265  ario where there
+0002b0c0: 2069 7320 2a2a 6e6f 2a2a 2061 6e69 6d61   is **no** anima
+0002b0d0: 6c20 696e 2074 6865 2060 6076 6964 656f  l in the ``video
+0002b0e0: 5f70 6174 6860 6020 7669 6465 6f20 666f  _path`` video fo
+0002b0f0: 7220 7468 6520 6669 7273 7420 3230 732c  r the first 20s,
+0002b100: 2074 6865 6e20 7468 6520 6669 7273 7420   then the first 
+0002b110: 3230 7320 6361 6e20 6265 2075 7365 6420  20s can be used 
+0002b120: 746f 2070 6172 7365 2074 6865 2062 6163  to parse the bac
+0002b130: 6b67 726f 756e 642e 0a20 2020 2020 2020  kground..       
+0002b140: 496e 2074 6869 7320 7363 656e 6172 696f  In this scenario
+0002b150: 2c20 6060 6267 5f76 6964 656f 5f70 6174  , ``bg_video_pat
+0002b160: 6860 6020 6361 6e20 6265 2070 6173 7365  h`` can be passe
+0002b170: 6420 6173 2060 604e 6f6e 6560 6020 616e  d as ``None`` an
+0002b180: 6420 6267 5f73 7461 7274 5f74 696d 6520  d bg_start_time 
+0002b190: 616e 6420 6267 5f65 6e64 5f74 696d 6520  and bg_end_time 
+0002b1a0: 6361 6e20 6265 2060 6030 303a 3030 3a30  can be ``00:00:0
+0002b1b0: 3060 6020 616e 6420 6060 3030 3a30 303a  0`` and ``00:00:
+0002b1c0: 3230 6060 2c20 7265 7065 6374 6976 656c  20``, repectivel
+0002b1d0: 792e 0a0a 2020 2020 2020 2049 6e20 7468  y...       In th
+0002b1e0: 6520 7363 656e 6172 696f 2077 6865 7265  e scenario where
+0002b1f0: 2074 6865 7265 202a 2a69 732a 2a20 616e   there **is** an
+0002b200: 696d 616c 2873 2920 696e 2074 6865 2065  imal(s) in the e
+0002b210: 6e74 6972 6520 6060 7669 6465 6f5f 7061  ntire ``video_pa
+0002b220: 7468 6060 2076 6964 656f 2c20 7061 7373  th`` video, pass
+0002b230: 2060 6062 675f 7669 6465 6f5f 7061 7468   ``bg_video_path
+0002b240: 6060 2061 7320 6120 7061 7468 2074 6f20  `` as a path to 
+0002b250: 6120 7669 6465 6f20 7265 636f 7264 696e  a video recordin
+0002b260: 6720 7468 6520 6172 656e 6120 7769 7468  g the arena with
+0002b270: 6f75 7420 7468 6520 616e 696d 616c 732e  out the animals.
+0002b280: 0a0a 2020 2020 3a70 6172 616d 2055 6e69  ..    :param Uni
+0002b290: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0002b2a0: 696b 655d 2076 6964 656f 5f70 6174 683a  ike] video_path:
+0002b2b0: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
+0002b2c0: 2076 6964 656f 2074 6f20 7265 6d6f 7665   video to remove
+0002b2d0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002b2e0: 6672 6f6d 2e0a 2020 2020 3a70 6172 616d  from..    :param
+0002b2f0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0002b300: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002b310: 5d5d 2062 675f 7669 6465 6f5f 7061 7468  ]] bg_video_path
+0002b320: 3a20 5061 7468 2074 6f20 7468 6520 7669  : Path to the vi
+0002b330: 6465 6f20 7768 6963 6820 636f 6e74 6169  deo which contai
+0002b340: 6e73 2061 2073 6567 6d65 6e74 2077 6974  ns a segment wit
+0002b350: 6820 7468 6520 6261 636b 6772 6f75 6e64  h the background
+0002b360: 206f 6e6c 792e 2049 6620 4e6f 6e65 2c20   only. If None, 
+0002b370: 7468 656e 2060 6076 6964 656f 5f70 6174  then ``video_pat
+0002b380: 6860 6020 7769 6c6c 2062 6520 7573 6564  h`` will be used
+0002b390: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+0002b3a0: 696f 6e61 6c5b 696e 745d 2062 675f 7374  ional[int] bg_st
+0002b3b0: 6172 745f 6672 6d3a 2054 6865 2066 6972  art_frm: The fir
+0002b3c0: 7374 2066 7261 6d65 2069 6e20 7468 6520  st frame in the 
+0002b3d0: 6261 636b 6772 6f75 6e64 2076 6964 656f  background video
+0002b3e0: 2074 6f20 7573 6520 7768 656e 2063 7265   to use when cre
+0002b3f0: 6174 696e 6720 6120 7265 7072 6573 656e  ating a represen
+0002b400: 7461 7469 7665 2062 6163 6b67 726f 756e  tative backgroun
+0002b410: 6420 696d 6167 652e 2044 6566 6175 6c74  d image. Default
+0002b420: 3a20 4e6f 6e65 2e0a 2020 2020 3a70 6172  : None..    :par
+0002b430: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
+0002b440: 2062 675f 656e 645f 6672 6d3a 2054 6865   bg_end_frm: The
+0002b450: 206c 6173 7420 6672 616d 6520 696e 2074   last frame in t
+0002b460: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
+0002b470: 6465 6f20 746f 2075 7365 2077 6865 6e20  deo to use when 
+0002b480: 6372 6561 7469 6e67 2061 2072 6570 7265  creating a repre
+0002b490: 7365 6e74 6174 6976 6520 6261 636b 6772  sentative backgr
+0002b4a0: 6f75 6e64 2069 6d61 6765 2e20 4465 6661  ound image. Defa
+0002b4b0: 756c 743a 204e 6f6e 652e 0a20 2020 203a  ult: None..    :
+0002b4c0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b73  param Optional[s
+0002b4d0: 7472 5d20 6267 5f73 7461 7274 5f74 696d  tr] bg_start_tim
+0002b4e0: 653a 2054 6865 2073 7461 7274 2074 696d  e: The start tim
+0002b4f0: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
+0002b500: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
+0002b510: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
+0002b520: 6465 6f20 746f 2075 7365 2074 6f20 6372  deo to use to cr
+0002b530: 6561 7465 2061 2072 6570 7265 7365 6e74  eate a represent
+0002b540: 6174 6976 6520 6261 636b 6772 6f75 6e64  ative background
+0002b550: 2069 6d61 6765 2e20 4465 6661 756c 743a   image. Default:
+0002b560: 204e 6f6e 652e 0a20 2020 203a 7061 7261   None..    :para
+0002b570: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
+0002b580: 6267 5f65 6e64 5f74 696d 653a 2054 6865  bg_end_time: The
+0002b590: 2065 6e64 2074 696d 6573 7461 6d70 2069   end timestamp i
+0002b5a0: 6e20 6048 483a 4d4d 3a53 5360 2066 6f72  n `HH:MM:SS` for
+0002b5b0: 6d61 7420 696e 2074 6865 2062 6163 6b67  mat in the backg
+0002b5c0: 726f 756e 6420 7669 6465 6f20 746f 2075  round video to u
+0002b5d0: 7365 2074 6f20 6372 6561 7465 2061 2072  se to create a r
+0002b5e0: 6570 7265 7365 6e74 6174 6976 6520 6261  epresentative ba
+0002b5f0: 636b 6772 6f75 6e64 2069 6d61 6765 2e20  ckground image. 
+0002b600: 4465 6661 756c 743a 204e 6f6e 652e 0a20  Default: None.. 
+0002b610: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+0002b620: 616c 5b54 7570 6c65 5b69 6e74 2c20 696e  al[Tuple[int, in
+0002b630: 742c 2069 6e74 5d5d 2062 675f 636f 6c6f  t, int]] bg_colo
+0002b640: 723a 2054 6865 2052 4742 2063 6f6c 6f72  r: The RGB color
+0002b650: 206f 6620 7468 6520 6d6f 7669 6e67 206f   of the moving o
+0002b660: 626a 6563 7473 2069 6e20 7468 6520 6f75  bjects in the ou
+0002b670: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
+0002b680: 756c 7473 2074 6f20 4e6f 6e65 2c20 7768  ults to None, wh
+0002b690: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
+0002b6a0: 6865 206f 7269 6769 6e61 6c20 636f 6c6f  he original colo
+0002b6b0: 7273 206f 6620 7468 6520 6d6f 7669 6e67  rs of the moving
+0002b6c0: 206f 626a 6563 7473 2e0a 2020 2020 3a70   objects..    :p
+0002b6d0: 6172 616d 204f 7074 696f 6e61 6c5b 5475  aram Optional[Tu
+0002b6e0: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
+0002b6f0: 745d 5d20 6667 5f63 6f6c 6f72 3a20 5468  t]] fg_color: Th
+0002b700: 6520 5247 4220 636f 6c6f 7220 6f66 2074  e RGB color of t
+0002b710: 6865 2062 6163 6b67 726f 756e 6420 6f75  he background ou
+0002b720: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
+0002b730: 756c 7473 2074 6f20 626c 6163 6b20 2830  ults to black (0
+0002b740: 2c20 302c 2030 292e 0a20 2020 203a 7061  , 0, 0)..    :pa
+0002b750: 7261 6d20 4f70 7469 6f6e 616c 5b55 6e69  ram Optional[Uni
+0002b760: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0002b770: 696b 655d 5d20 7361 7665 5f70 6174 683a  ike]] save_path:
+0002b780: 2054 6865 2070 6174 6368 2074 6f20 7768   The patch to wh
+0002b790: 6572 6520 746f 2073 6176 6520 7468 6520  ere to save the 
+0002b7a0: 6f75 7470 7574 2076 6964 656f 2077 6865  output video whe
+0002b7b0: 7265 2074 6865 2062 6163 6b67 726f 756e  re the backgroun
+0002b7c0: 6420 6973 2072 656d 6f76 6564 2e20 4966  d is removed. If
+0002b7d0: 204e 6f6e 652c 2073 6176 6573 2074 6865   None, saves the
+0002b7e0: 206f 7574 7075 7420 7669 6465 6f20 696e   output video in
+0002b7f0: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
+0002b800: 6f72 7920 6173 2074 6865 2069 6e70 7574  ory as the input
+0002b810: 2076 6964 656f 2077 6974 6820 7468 6520   video with the 
+0002b820: 6060 5f62 675f 7375 6274 7261 6374 6564  ``_bg_subtracted
+0002b830: 6060 2073 7566 6669 782e 2044 6566 6175  `` suffix. Defau
+0002b840: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a72  lt: None..    :r
+0002b850: 6574 7572 6e3a 204e 6f6e 652e 0a0a 2020  eturn: None...  
+0002b860: 2020 3a65 7861 6d70 6c65 3a0a 2020 2020    :example:.    
+0002b870: 3e3e 3e20 7669 6465 6f5f 6267 5f73 7562  >>> video_bg_sub
+0002b880: 7472 6163 7469 6f6e 2876 6964 656f 5f70  traction(video_p
+0002b890: 6174 683d 272f 5573 6572 732f 7369 6d6f  ath='/Users/simo
+0002b8a0: 6e2f 446f 776e 6c6f 6164 732f 315f 4c48  n/Downloads/1_LH
+0002b8b0: 5f63 726f 7070 6564 2e6d 7034 272c 2062  _cropped.mp4', b
+0002b8c0: 675f 7374 6172 745f 7469 6d65 3d27 3030  g_start_time='00
+0002b8d0: 3a30 303a 3030 272c 2062 675f 656e 645f  :00:00', bg_end_
+0002b8e0: 7469 6d65 3d27 3030 3a30 303a 3130 272c  time='00:00:10',
+0002b8f0: 2062 675f 636f 6c6f 723d 2830 2c20 3130   bg_color=(0, 10
+0002b900: 362c 2031 3637 292c 2066 675f 636f 6c6f  6, 167), fg_colo
+0002b910: 723d 2832 3534 2c20 3230 342c 2032 2929  r=(254, 204, 2))
+0002b920: 0a20 2020 2022 2222 0a0a 2020 2020 7469  .    """..    ti
+0002b930: 6d65 7220 3d20 5369 6d62 6154 696d 6572  mer = SimbaTimer
+0002b940: 2873 7461 7274 3d54 7275 6529 0a20 2020  (start=True).   
+0002b950: 2063 6865 636b 5f66 696c 655f 6578 6973   check_file_exis
+0002b960: 745f 616e 645f 7265 6164 6162 6c65 2866  t_and_readable(f
+0002b970: 696c 655f 7061 7468 3d76 6964 656f 5f70  ile_path=video_p
+0002b980: 6174 6829 0a20 2020 2069 6620 6267 5f76  ath).    if bg_v
+0002b990: 6964 656f 5f70 6174 6820 6973 204e 6f6e  ideo_path is Non
+0002b9a0: 653a 0a20 2020 2020 2020 2062 675f 7669  e:.        bg_vi
+0002b9b0: 6465 6f5f 7061 7468 203d 2064 6565 7063  deo_path = deepc
+0002b9c0: 6f70 7928 7669 6465 6f5f 7061 7468 290a  opy(video_path).
+0002b9d0: 2020 2020 7669 6465 6f5f 6d65 7461 5f64      video_meta_d
+0002b9e0: 6174 6120 3d20 6765 745f 7669 6465 6f5f  ata = get_video_
+0002b9f0: 6d65 7461 5f64 6174 6128 7669 6465 6f5f  meta_data(video_
+0002ba00: 7061 7468 3d76 6964 656f 5f70 6174 6829  path=video_path)
+0002ba10: 0a20 2020 2064 6972 2c20 7669 6465 6f5f  .    dir, video_
+0002ba20: 6e61 6d65 2c20 6578 7420 3d20 6765 745f  name, ext = get_
+0002ba30: 666e 5f65 7874 2866 696c 6570 6174 683d  fn_ext(filepath=
+0002ba40: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
+0002ba50: 6966 2073 6176 655f 7061 7468 2069 7320  if save_path is 
+0002ba60: 4e6f 6e65 3a0a 2020 2020 2020 2020 7361  None:.        sa
+0002ba70: 7665 5f70 6174 6820 3d20 6f73 2e70 6174  ve_path = os.pat
+0002ba80: 682e 6a6f 696e 2864 6972 2c20 6627 7b76  h.join(dir, f'{v
+0002ba90: 6964 656f 5f6e 616d 657d 5f62 675f 7375  ideo_name}_bg_su
+0002baa0: 6274 7261 6374 6564 7b65 7874 7d27 290a  btracted{ext}').
+0002bab0: 2020 2020 666f 7572 6363 203d 2063 7632      fourcc = cv2
+0002bac0: 2e56 6964 656f 5772 6974 6572 5f66 6f75  .VideoWriter_fou
+0002bad0: 7263 6328 2a46 6f72 6d61 7473 2e4d 5034  rcc(*Formats.MP4
+0002bae0: 5f43 4f44 4543 2e76 616c 7565 290a 2020  _CODEC.value).  
+0002baf0: 2020 7772 6974 6572 203d 2063 7632 2e56    writer = cv2.V
+0002bb00: 6964 656f 5772 6974 6572 2873 6176 655f  ideoWriter(save_
+0002bb10: 7061 7468 2c20 666f 7572 6363 2c20 7669  path, fourcc, vi
+0002bb20: 6465 6f5f 6d65 7461 5f64 6174 615b 2766  deo_meta_data['f
+0002bb30: 7073 275d 2c0a 2020 2020 2020 2020 2020  ps'],.          
+0002bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bb50: 2020 2028 7669 6465 6f5f 6d65 7461 5f64     (video_meta_d
+0002bb60: 6174 615b 2777 6964 7468 275d 2c20 7669  ata['width'], vi
+0002bb70: 6465 6f5f 6d65 7461 5f64 6174 615b 2768  deo_meta_data['h
+0002bb80: 6569 6768 7427 5d29 290a 2020 2020 6267  eight'])).    bg
+0002bb90: 5f66 726d 203d 2063 7265 6174 655f 6176  _frm = create_av
+0002bba0: 6572 6167 655f 6672 6d28 7669 6465 6f5f  erage_frm(video_
+0002bbb0: 7061 7468 3d62 675f 7669 6465 6f5f 7061  path=bg_video_pa
+0002bbc0: 7468 2c20 7374 6172 745f 6672 6d3d 6267  th, start_frm=bg
+0002bbd0: 5f73 7461 7274 5f66 726d 2c20 656e 645f  _start_frm, end_
+0002bbe0: 6672 6d3d 6267 5f65 6e64 5f66 726d 2c0a  frm=bg_end_frm,.
+0002bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bc10: 7374 6172 745f 7469 6d65 3d62 675f 7374  start_time=bg_st
+0002bc20: 6172 745f 7469 6d65 2c20 656e 645f 7469  art_time, end_ti
+0002bc30: 6d65 3d62 675f 656e 645f 7469 6d65 290a  me=bg_end_time).
+0002bc40: 2020 2020 6267 5f66 726d 203d 2063 7632      bg_frm = cv2
+0002bc50: 2e72 6573 697a 6528 6267 5f66 726d 2c20  .resize(bg_frm, 
+0002bc60: 2876 6964 656f 5f6d 6574 615f 6461 7461  (video_meta_data
+0002bc70: 5b27 7769 6474 6827 5d2c 2076 6964 656f  ['width'], video
+0002bc80: 5f6d 6574 615f 6461 7461 5b27 6865 6967  _meta_data['heig
+0002bc90: 6874 275d 2929 0a20 2020 2062 6720 3d20  ht'])).    bg = 
+0002bca0: 6376 322e 6376 7443 6f6c 6f72 286e 702e  cv2.cvtColor(np.
+0002bcb0: 6675 6c6c 5f6c 696b 6528 6267 5f66 726d  full_like(bg_frm
+0002bcc0: 2c20 6267 5f63 6f6c 6f72 292c 2063 7632  , bg_color), cv2
+0002bcd0: 2e43 4f4c 4f52 5f42 4752 3252 4742 290a  .COLOR_BGR2RGB).
+0002bce0: 2020 2020 6361 7020 3d20 6376 322e 5669      cap = cv2.Vi
+0002bcf0: 6465 6f43 6170 7475 7265 2876 6964 656f  deoCapture(video
+0002bd00: 5f70 6174 6829 0a20 2020 2066 726d 5f63  _path).    frm_c
+0002bd10: 6e74 203d 2030 0a20 2020 2077 6869 6c65  nt = 0.    while
+0002bd20: 2054 7275 653a 0a20 2020 2020 2020 2072   True:.        r
+0002bd30: 6574 2c20 6672 6d20 3d20 6361 702e 7265  et, frm = cap.re
+0002bd40: 6164 2829 0a20 2020 2020 2020 2069 6620  ad().        if 
+0002bd50: 6e6f 7420 7265 743a 0a20 2020 2020 2020  not ret:.       
+0002bd60: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+0002bd70: 2020 2064 6966 6620 3d20 6376 322e 6162     diff = cv2.ab
+0002bd80: 7364 6966 6628 6672 6d2c 2062 675f 6672  sdiff(frm, bg_fr
+0002bd90: 6d29 0a20 2020 2020 2020 2067 7261 795f  m).        gray_
+0002bda0: 6469 6666 203d 2063 7632 2e63 7674 436f  diff = cv2.cvtCo
+0002bdb0: 6c6f 7228 6469 6666 2c20 6376 322e 434f  lor(diff, cv2.CO
+0002bdc0: 4c4f 525f 4247 5232 4752 4159 290a 2020  LOR_BGR2GRAY).  
+0002bdd0: 2020 2020 2020 5f2c 206d 6173 6b20 3d20        _, mask = 
+0002bde0: 6376 322e 7468 7265 7368 6f6c 6428 6772  cv2.threshold(gr
+0002bdf0: 6179 5f64 6966 662c 2035 302c 2032 3535  ay_diff, 50, 255
+0002be00: 2c20 6376 322e 5448 5245 5348 5f42 494e  , cv2.THRESH_BIN
+0002be10: 4152 5929 0a20 2020 2020 2020 2069 6620  ARY).        if 
+0002be20: 6667 5f63 6f6c 6f72 2069 7320 4e6f 6e65  fg_color is None
+0002be30: 3a0a 2020 2020 2020 2020 2020 2020 6667  :.            fg
+0002be40: 203d 2063 7632 2e62 6974 7769 7365 5f61   = cv2.bitwise_a
+0002be50: 6e64 2866 726d 2c20 6672 6d2c 206d 6173  nd(frm, frm, mas
+0002be60: 6b3d 6d61 736b 290a 2020 2020 2020 2020  k=mask).        
+0002be70: 2020 2020 7265 7375 6c74 203d 2063 7632      result = cv2
+0002be80: 2e61 6464 2862 672c 2066 6729 0a20 2020  .add(bg, fg).   
+0002be90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0002bea0: 2020 2020 2020 206d 6173 6b5f 696e 7620         mask_inv 
+0002beb0: 3d20 6376 322e 6269 7477 6973 655f 6e6f  = cv2.bitwise_no
+0002bec0: 7428 6d61 736b 290a 2020 2020 2020 2020  t(mask).        
+0002bed0: 2020 2020 6667 5f63 6c72 203d 2063 7632      fg_clr = cv2
+0002bee0: 2e63 7674 436f 6c6f 7228 6e70 2e66 756c  .cvtColor(np.ful
+0002bef0: 6c5f 6c69 6b65 2866 726d 2c20 6667 5f63  l_like(frm, fg_c
+0002bf00: 6f6c 6f72 292c 2063 7632 2e43 4f4c 4f52  olor), cv2.COLOR
+0002bf10: 5f42 4752 3252 4742 290a 2020 2020 2020  _BGR2RGB).      
+0002bf20: 2020 2020 2020 6667 5f63 6c72 203d 2063        fg_clr = c
+0002bf30: 7632 2e62 6974 7769 7365 5f61 6e64 2866  v2.bitwise_and(f
+0002bf40: 675f 636c 722c 2066 675f 636c 722c 206d  g_clr, fg_clr, m
+0002bf50: 6173 6b3d 6d61 736b 290a 2020 2020 2020  ask=mask).      
+0002bf60: 2020 2020 2020 7265 7375 6c74 203d 2063        result = c
+0002bf70: 7632 2e62 6974 7769 7365 5f61 6e64 2862  v2.bitwise_and(b
+0002bf80: 672c 2062 672c 206d 6173 6b3d 6d61 736b  g, bg, mask=mask
+0002bf90: 5f69 6e76 290a 2020 2020 2020 2020 2020  _inv).          
+0002bfa0: 2020 7265 7375 6c74 203d 2063 7632 2e61    result = cv2.a
+0002bfb0: 6464 2872 6573 756c 742c 2066 675f 636c  dd(result, fg_cl
+0002bfc0: 7229 0a20 2020 2020 2020 2077 7269 7465  r).        write
+0002bfd0: 722e 7772 6974 6528 7265 7375 6c74 290a  r.write(result).
+0002bfe0: 2020 2020 2020 2020 6672 6d5f 636e 7420          frm_cnt 
+0002bff0: 2b3d 2031 0a20 2020 2020 2020 2070 7269  += 1.        pri
+0002c000: 6e74 2866 2742 6163 6b67 726f 756e 6420  nt(f'Background 
+0002c010: 7375 6274 7261 6374 696f 6e20 6672 616d  subtraction fram
+0002c020: 6520 7b66 726d 5f63 6e74 7d2f 7b76 6964  e {frm_cnt}/{vid
+0002c030: 656f 5f6d 6574 615f 6461 7461 5b22 6672  eo_meta_data["fr
+0002c040: 616d 655f 636f 756e 7422 5d7d 2028 5669  ame_count"]} (Vi
+0002c050: 6465 6f3a 207b 7669 6465 6f5f 6e61 6d65  deo: {video_name
+0002c060: 7d29 2729 0a0a 2020 2020 7772 6974 6572  })')..    writer
+0002c070: 2e72 656c 6561 7365 2829 0a20 2020 2063  .release().    c
+0002c080: 6170 2e72 656c 6561 7365 2829 0a20 2020  ap.release().   
+0002c090: 2074 696d 6572 2e73 746f 705f 7469 6d65   timer.stop_time
+0002c0a0: 7228 290a 2020 2020 7374 646f 7574 5f73  r().    stdout_s
+0002c0b0: 7563 6365 7373 286d 7367 3d66 2742 6163  uccess(msg=f'Bac
+0002c0c0: 6b67 726f 756e 6420 7375 6274 7261 6374  kground subtract
+0002c0d0: 6564 2066 726f 6d20 7b76 6964 656f 5f6e  ed from {video_n
+0002c0e0: 616d 657d 2061 6e64 2073 6176 6564 2061  ame} and saved a
+0002c0f0: 7420 7b73 6176 655f 7061 7468 7d27 2c20  t {save_path}', 
+0002c100: 656c 6170 7365 645f 7469 6d65 3d74 696d  elapsed_time=tim
+0002c110: 6572 2e65 6c61 7073 6564 5f74 696d 6529  er.elapsed_time)
+0002c120: 0a0a 6465 6620 5f62 675f 7265 6d6f 7665  ..def _bg_remove
+0002c130: 725f 6d70 2866 726d 5f72 616e 6765 3a20  r_mp(frm_range: 
+0002c140: 5475 706c 655b 696e 742c 206e 702e 6e64  Tuple[int, np.nd
+0002c150: 6172 7261 795d 2c0a 2020 2020 2020 2020  array],.        
+0002c160: 2020 2020 2020 2020 2020 2076 6964 656f             video
+0002c170: 5f70 6174 683a 2055 6e69 6f6e 5b73 7472  _path: Union[str
+0002c180: 2c20 6f73 2e50 6174 684c 696b 655d 2c0a  , os.PathLike],.
+0002c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c1a0: 2020 2062 675f 6672 6d3a 206e 702e 6e64     bg_frm: np.nd
+0002c1b0: 6172 7261 792c 0a20 2020 2020 2020 2020  array,.         
+0002c1c0: 2020 2020 2020 2020 2020 6267 5f63 6c72            bg_clr
+0002c1d0: 3a20 5475 706c 655b 696e 742c 2069 6e74  : Tuple[int, int
+0002c1e0: 2c20 696e 745d 2c0a 2020 2020 2020 2020  , int],.        
+0002c1f0: 2020 2020 2020 2020 2020 2066 675f 636c             fg_cl
+0002c200: 723a 2054 7570 6c65 5b69 6e74 2c20 696e  r: Tuple[int, in
+0002c210: 742c 2069 6e74 5d2c 0a20 2020 2020 2020  t, int],.       
+0002c220: 2020 2020 2020 2020 2020 2020 7669 6465              vide
+0002c230: 6f5f 6d65 7461 5f64 6174 613a 2044 6963  o_meta_data: Dic
+0002c240: 745b 7374 722c 2041 6e79 5d2c 0a20 2020  t[str, Any],.   
+0002c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c260: 7465 6d70 5f64 6972 3a20 556e 696f 6e5b  temp_dir: Union[
+0002c270: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002c280: 5d29 3a0a 0a20 2020 2062 6174 6368 2c20  ]):..    batch, 
+0002c290: 6672 6d5f 7261 6e67 6520 3d20 6672 6d5f  frm_range = frm_
+0002c2a0: 7261 6e67 655b 305d 2c20 6672 6d5f 7261  range[0], frm_ra
+0002c2b0: 6e67 655b 315d 0a20 2020 2073 7461 7274  nge[1].    start
+0002c2c0: 5f66 726d 2c20 6375 7272 656e 745f 6672  _frm, current_fr
+0002c2d0: 6d2c 2065 6e64 5f66 726d 203d 2066 726d  m, end_frm = frm
+0002c2e0: 5f72 616e 6765 5b30 5d2c 2066 726d 5f72  _range[0], frm_r
+0002c2f0: 616e 6765 5b30 5d2c 2066 726d 5f72 616e  ange[0], frm_ran
+0002c300: 6765 5b2d 315d 0a20 2020 2063 6170 203d  ge[-1].    cap =
+0002c310: 2063 7632 2e56 6964 656f 4361 7074 7572   cv2.VideoCaptur
+0002c320: 6528 7669 6465 6f5f 7061 7468 290a 2020  e(video_path).  
+0002c330: 2020 666f 7572 6363 203d 2063 7632 2e56    fourcc = cv2.V
+0002c340: 6964 656f 5772 6974 6572 5f66 6f75 7263  ideoWriter_fourc
+0002c350: 6328 2a46 6f72 6d61 7473 2e4d 5034 5f43  c(*Formats.MP4_C
+0002c360: 4f44 4543 2e76 616c 7565 290a 2020 2020  ODEC.value).    
+0002c370: 7361 7665 5f70 6174 6820 3d20 6f73 2e70  save_path = os.p
+0002c380: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
+0002c390: 722c 2066 227b 6261 7463 687d 2e6d 7034  r, f"{batch}.mp4
+0002c3a0: 2229 0a20 2020 2063 6170 2e73 6574 2831  ").    cap.set(1
+0002c3b0: 2c20 7374 6172 745f 6672 6d29 0a20 2020  , start_frm).   
+0002c3c0: 2077 7269 7465 7220 3d20 6376 322e 5669   writer = cv2.Vi
+0002c3d0: 6465 6f57 7269 7465 7228 7361 7665 5f70  deoWriter(save_p
+0002c3e0: 6174 682c 2066 6f75 7263 632c 2076 6964  ath, fourcc, vid
+0002c3f0: 656f 5f6d 6574 615f 6461 7461 5b27 6670  eo_meta_data['fp
+0002c400: 7327 5d2c 2028 7669 6465 6f5f 6d65 7461  s'], (video_meta
+0002c410: 5f64 6174 615b 2777 6964 7468 275d 2c20  _data['width'], 
+0002c420: 7669 6465 6f5f 6d65 7461 5f64 6174 615b  video_meta_data[
+0002c430: 2768 6569 6768 7427 5d29 290a 2020 2020  'height'])).    
+0002c440: 6267 203d 206e 702e 6675 6c6c 5f6c 696b  bg = np.full_lik
+0002c450: 6528 6267 5f66 726d 2c20 6267 5f63 6c72  e(bg_frm, bg_clr
+0002c460: 290a 2020 2020 6267 203d 2062 675b 3a2c  ).    bg = bg[:,
+0002c470: 203a 2c20 3a3a 2d31 5d0a 2020 2020 6469   :, ::-1].    di
+0002c480: 722c 2076 6964 656f 5f6e 616d 652c 2065  r, video_name, e
+0002c490: 7874 203d 2067 6574 5f66 6e5f 6578 7428  xt = get_fn_ext(
+0002c4a0: 6669 6c65 7061 7468 3d76 6964 656f 5f70  filepath=video_p
+0002c4b0: 6174 6829 0a20 2020 2077 6869 6c65 2063  ath).    while c
+0002c4c0: 7572 7265 6e74 5f66 726d 203c 3d20 656e  urrent_frm <= en
+0002c4d0: 645f 6672 6d3a 0a20 2020 2020 2020 2072  d_frm:.        r
+0002c4e0: 6574 2c20 6672 6d20 3d20 6361 702e 7265  et, frm = cap.re
+0002c4f0: 6164 2829 0a20 2020 2020 2020 2069 6620  ad().        if 
+0002c500: 6e6f 7420 7265 743a 0a20 2020 2020 2020  not ret:.       
+0002c510: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+0002c520: 2020 2064 6966 6620 3d20 6376 322e 6162     diff = cv2.ab
+0002c530: 7364 6966 6628 6672 6d2c 2062 675f 6672  sdiff(frm, bg_fr
+0002c540: 6d29 0a20 2020 2020 2020 2062 2c20 672c  m).        b, g,
+0002c550: 2072 203d 2064 6966 665b 3a2c 203a 2c20   r = diff[:, :, 
+0002c560: 305d 2c20 6469 6666 5b3a 2c20 3a2c 2031  0], diff[:, :, 1
+0002c570: 5d2c 2064 6966 665b 3a2c 203a 2c20 325d  ], diff[:, :, 2]
+0002c580: 0a20 2020 2020 2020 2067 7261 795f 6469  .        gray_di
+0002c590: 6666 203d 2030 2e32 3938 3920 2a20 7220  ff = 0.2989 * r 
+0002c5a0: 2b20 302e 3538 3730 202a 2067 202b 2030  + 0.5870 * g + 0
+0002c5b0: 2e31 3134 3020 2a20 620a 2020 2020 2020  .1140 * b.      
+0002c5c0: 2020 6772 6179 5f64 6966 6620 3d20 6772    gray_diff = gr
+0002c5d0: 6179 5f64 6966 662e 6173 7479 7065 286e  ay_diff.astype(n
+0002c5e0: 702e 7569 6e74 3829 2020 2320 456e 7375  p.uint8)  # Ensu
+0002c5f0: 7265 2074 6865 2074 7970 6520 6973 2075  re the type is u
+0002c600: 696e 7438 0a20 2020 2020 2020 206d 6173  int8.        mas
+0002c610: 6b20 3d20 6e70 2e77 6865 7265 2867 7261  k = np.where(gra
+0002c620: 795f 6469 6666 203e 2035 302c 2032 3535  y_diff > 50, 255
+0002c630: 2c20 3029 2e61 7374 7970 6528 6e70 2e75  , 0).astype(np.u
+0002c640: 696e 7438 290a 2020 2020 2020 2020 6966  int8).        if
+0002c650: 2066 675f 636c 7220 6973 204e 6f6e 653a   fg_clr is None:
+0002c660: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+0002c670: 3d20 6376 322e 6269 7477 6973 655f 616e  = cv2.bitwise_an
+0002c680: 6428 6672 6d2c 2066 726d 2c20 6d61 736b  d(frm, frm, mask
+0002c690: 3d6d 6173 6b29 0a20 2020 2020 2020 2020  =mask).         
+0002c6a0: 2020 2072 6573 756c 7420 3d20 6376 322e     result = cv2.
+0002c6b0: 6164 6428 6267 2c20 6667 290a 2020 2020  add(bg, fg).    
+0002c6c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002c6d0: 2020 2020 2020 6d61 736b 5f69 6e76 203d        mask_inv =
+0002c6e0: 2063 7632 2e62 6974 7769 7365 5f6e 6f74   cv2.bitwise_not
+0002c6f0: 286d 6173 6b29 0a20 2020 2020 2020 2020  (mask).         
+0002c700: 2020 2066 675f 636c 725f 696d 6720 3d20     fg_clr_img = 
+0002c710: 6e70 2e66 756c 6c5f 6c69 6b65 2866 726d  np.full_like(frm
+0002c720: 2c20 6667 5f63 6c72 290a 2020 2020 2020  , fg_clr).      
+0002c730: 2020 2020 2020 6667 5f63 6c72 5f69 6d67        fg_clr_img
+0002c740: 203d 2066 675f 636c 725f 696d 675b 3a2c   = fg_clr_img[:,
+0002c750: 203a 2c20 3a3a 2d31 5d0a 2020 2020 2020   :, ::-1].      
+0002c760: 2020 2020 2020 6667 5f63 6c72 5f69 6d67        fg_clr_img
+0002c770: 203d 2063 7632 2e62 6974 7769 7365 5f61   = cv2.bitwise_a
+0002c780: 6e64 2866 675f 636c 725f 696d 672c 2066  nd(fg_clr_img, f
+0002c790: 675f 636c 725f 696d 672c 206d 6173 6b3d  g_clr_img, mask=
+0002c7a0: 6d61 736b 290a 2020 2020 2020 2020 2020  mask).          
+0002c7b0: 2020 7265 7375 6c74 203d 2063 7632 2e62    result = cv2.b
+0002c7c0: 6974 7769 7365 5f61 6e64 2862 672c 2062  itwise_and(bg, b
+0002c7d0: 672c 206d 6173 6b3d 6d61 736b 5f69 6e76  g, mask=mask_inv
+0002c7e0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0002c7f0: 7375 6c74 203d 2063 7632 2e61 6464 2872  sult = cv2.add(r
+0002c800: 6573 756c 742c 2066 675f 636c 725f 696d  esult, fg_clr_im
+0002c810: 6729 0a20 2020 2020 2020 2077 7269 7465  g).        write
+0002c820: 722e 7772 6974 6528 7265 7375 6c74 290a  r.write(result).
+0002c830: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0002c840: 6672 6d20 2b3d 2031 0a20 2020 2020 2020  frm += 1.       
+0002c850: 2070 7269 6e74 2866 2742 6163 6b67 726f   print(f'Backgro
+0002c860: 756e 6420 7375 6274 7261 6374 696f 6e20  und subtraction 
+0002c870: 6672 616d 6520 7b63 7572 7265 6e74 5f66  frame {current_f
+0002c880: 726d 7d2f 7b76 6964 656f 5f6d 6574 615f  rm}/{video_meta_
+0002c890: 6461 7461 5b22 6672 616d 655f 636f 756e  data["frame_coun
+0002c8a0: 7422 5d7d 2028 5669 6465 6f3a 207b 7669  t"]} (Video: {vi
+0002c8b0: 6465 6f5f 6e61 6d65 7d29 2729 0a20 2020  deo_name})').   
+0002c8c0: 2077 7269 7465 722e 7265 6c65 6173 6528   writer.release(
+0002c8d0: 290a 2020 2020 6361 702e 7265 6c65 6173  ).    cap.releas
+0002c8e0: 6528 290a 2020 2020 7265 7475 726e 2062  e().    return b
+0002c8f0: 6174 6368 0a0a 6465 6620 7669 6465 6f5f  atch..def video_
+0002c900: 6267 5f73 7562 7374 7261 6374 696f 6e5f  bg_substraction_
+0002c910: 6d70 2876 6964 656f 5f70 6174 683a 2055  mp(video_path: U
+0002c920: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002c930: 684c 696b 655d 2c0a 2020 2020 2020 2020  hLike],.        
+0002c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c950: 2020 2020 2062 675f 7669 6465 6f5f 7061       bg_video_pa
+0002c960: 7468 3a20 4f70 7469 6f6e 616c 5b55 6e69  th: Optional[Uni
+0002c970: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
+0002c980: 696b 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ike]] = None,.  
+0002c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c9a0: 2020 2020 2020 2020 2020 2062 675f 7374             bg_st
+0002c9b0: 6172 745f 6672 6d3a 204f 7074 696f 6e61  art_frm: Optiona
+0002c9c0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+0002c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c9e0: 2020 2020 2020 2020 2020 2020 6267 5f65              bg_e
+0002c9f0: 6e64 5f66 726d 3a20 4f70 7469 6f6e 616c  nd_frm: Optional
+0002ca00: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
 0002ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca20: 2020 6667 5f63 6f6c 6f72 3a20 4f70 7469    fg_color: Opti
-0002ca30: 6f6e 616c 5b54 7570 6c65 5b69 6e74 2c20  onal[Tuple[int, 
-0002ca40: 696e 742c 2069 6e74 5d5d 203d 204e 6f6e  int, int]] = Non
-0002ca50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0002ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca70: 7361 7665 5f70 6174 683a 204f 7074 696f  save_path: Optio
-0002ca80: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
-0002ca90: 732e 5061 7468 4c69 6b65 5d5d 203d 204e  s.PathLike]] = N
-0002caa0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0002cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cac0: 2020 636f 7265 5f63 6e74 3a20 4f70 7469    core_cnt: Opti
-0002cad0: 6f6e 616c 5b69 6e74 5d20 3d20 2d31 2920  onal[int] = -1) 
-0002cae0: 2d3e 204e 6f6e 653a 0a0a 2020 2020 2222  -> None:..    ""
-0002caf0: 220a 2020 2020 5375 6274 7261 6374 2074  ".    Subtract t
-0002cb00: 6865 2062 6163 6b67 726f 756e 6420 6672  he background fr
-0002cb10: 6f6d 2061 2076 6964 656f 2075 7369 6e67  om a video using
-0002cb20: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
-0002cb30: 2e0a 0a20 2020 202e 2e20 7669 6465 6f3a  ...    .. video:
-0002cb40: 3a20 5f73 7461 7469 632f 696d 672f 7669  : _static/img/vi
-0002cb50: 6465 6f5f 6267 5f73 7562 7374 7261 6374  deo_bg_substract
-0002cb60: 696f 6e5f 6d70 2e77 6562 6d0a 2020 2020  ion_mp.webm.    
-0002cb70: 2020 203a 7769 6474 683a 2039 3030 0a20     :width: 900. 
-0002cb80: 2020 2020 2020 3a61 7574 6f70 6c61 793a        :autoplay:
-0002cb90: 0a20 2020 2020 2020 3a6c 6f6f 703a 0a0a  .       :loop:..
-0002cba0: 2020 2020 2e2e 206e 6f74 653a 3a0a 2020      .. note::.  
-0002cbb0: 2020 2020 2020 466f 7220 7369 6e67 6c65        For single
-0002cbc0: 2063 6f72 6520 616c 7465 726e 6174 6976   core alternativ
-0002cbd0: 652c 2073 6565 2060 6073 696d 6261 2e76  e, see ``simba.v
-0002cbe0: 6964 656f 5f70 726f 6365 7373 6f72 732e  ideo_processors.
-0002cbf0: 7669 6465 6f5f 7072 6f63 6573 7369 6e67  video_processing
-0002cc00: 2e76 6964 656f 5f62 675f 7375 6274 7261  .video_bg_subtra
-0002cc10: 6374 696f 6e60 600a 0a20 2020 2020 2020  ction``..       
-0002cc20: 4966 2020 6060 6267 5f76 6964 656f 5f70  If  ``bg_video_p
-0002cc30: 6174 6860 6020 6973 2070 6173 7365 642c  ath`` is passed,
-0002cc40: 2074 6861 7420 7669 6465 6f20 7769 6c6c   that video will
-0002cc50: 2062 6520 7573 6564 2074 6f20 7061 7273   be used to pars
-0002cc60: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
-0002cc70: 2e20 4966 204e 6f6e 652c 2060 6076 6964  . If None, ``vid
-0002cc80: 656f 5f70 6174 6860 6020 7769 6c6c 2062  eo_path`` will b
-0002cc90: 6520 7573 6520 6474 6f20 7061 7273 6520  e use dto parse 
-0002cca0: 6261 636b 6772 6f75 6e64 2e0a 2020 2020  background..    
-0002ccb0: 2020 2045 6974 6865 7220 7061 7373 2060     Either pass `
-0002ccc0: 6073 7461 7274 5f66 726d 6060 2061 6e64  `start_frm`` and
-0002ccd0: 2060 6065 6e64 5f66 726d 6060 204f 5220   ``end_frm`` OR 
-0002cce0: 6060 7374 6172 745f 7469 6d65 6060 2061  ``start_time`` a
-0002ccf0: 6e64 2060 6065 6e64 5f74 696d 6560 6020  nd ``end_time`` 
-0002cd00: 4f52 2070 6173 7320 616c 6c20 666f 7572  OR pass all four
-0002cd10: 2061 7267 756d 656e 7473 2061 7320 4e6f   arguments as No
-0002cd20: 6e65 2e0a 2020 2020 2020 2054 686f 7365  ne..       Those
-0002cd30: 2074 776f 2061 7267 756d 656e 7473 2077   two arguments w
-0002cd40: 696c 6c20 6265 2075 7365 6420 746f 2073  ill be used to s
-0002cd50: 6c69 6365 2074 6865 2062 6163 6b67 726f  lice the backgro
-0002cd60: 756e 6420 7669 6465 6f2c 2061 6e64 2074  und video, and t
-0002cd70: 6865 2073 6c69 6365 6420 7061 7274 2069  he sliced part i
-0002cd80: 7320 7573 6564 2074 6f20 7061 7273 6520  s used to parse 
-0002cd90: 7468 6520 6261 636b 6772 6f75 6e64 2e0a  the background..
-0002cda0: 0a20 2020 2020 2020 466f 7220 6578 616d  .       For exam
-0002cdb0: 706c 652c 2069 6e20 7468 6520 7363 656e  ple, in the scen
-0002cdc0: 6172 696f 2077 6865 7265 2074 6865 7265  ario where there
-0002cdd0: 2069 7320 2a2a 6e6f 2a2a 2061 6e69 6d61   is **no** anima
-0002cde0: 6c20 696e 2074 6865 2060 6076 6964 656f  l in the ``video
-0002cdf0: 5f70 6174 6860 6020 7669 6465 6f20 666f  _path`` video fo
-0002ce00: 7220 7468 6520 6669 7273 7420 3230 732c  r the first 20s,
-0002ce10: 2074 6865 6e20 7468 6520 6669 7273 7420   then the first 
-0002ce20: 3230 7320 6361 6e20 6265 2075 7365 6420  20s can be used 
-0002ce30: 746f 2070 6172 7365 2074 6865 2062 6163  to parse the bac
-0002ce40: 6b67 726f 756e 642e 0a20 2020 2020 2020  kground..       
-0002ce50: 496e 2074 6869 7320 7363 656e 6172 696f  In this scenario
-0002ce60: 2c20 6060 6267 5f76 6964 656f 5f70 6174  , ``bg_video_pat
-0002ce70: 6860 6020 6361 6e20 6265 2070 6173 7365  h`` can be passe
-0002ce80: 6420 6173 2060 604e 6f6e 6560 6020 616e  d as ``None`` an
-0002ce90: 6420 6267 5f73 7461 7274 5f74 696d 6520  d bg_start_time 
-0002cea0: 616e 6420 6267 5f65 6e64 5f74 696d 6520  and bg_end_time 
-0002ceb0: 6361 6e20 6265 2060 6030 303a 3030 3a30  can be ``00:00:0
-0002cec0: 3060 6020 616e 6420 6060 3030 3a30 303a  0`` and ``00:00:
-0002ced0: 3230 6060 2c20 7265 7065 6374 6976 656c  20``, repectivel
-0002cee0: 792e 0a0a 2020 2020 2020 2049 6e20 7468  y...       In th
-0002cef0: 6520 7363 656e 6172 696f 2077 6865 7265  e scenario where
-0002cf00: 2074 6865 7265 202a 2a69 732a 2a20 616e   there **is** an
-0002cf10: 696d 616c 2873 2920 696e 2074 6865 2065  imal(s) in the e
-0002cf20: 6e74 6972 6520 6060 7669 6465 6f5f 7061  ntire ``video_pa
-0002cf30: 7468 6060 2076 6964 656f 2c20 7061 7373  th`` video, pass
-0002cf40: 2060 6062 675f 7669 6465 6f5f 7061 7468   ``bg_video_path
-0002cf50: 6060 2061 7320 6120 7061 7468 2074 6f20  `` as a path to 
-0002cf60: 6120 7669 6465 6f20 7265 636f 7264 696e  a video recordin
-0002cf70: 6720 7468 6520 6172 656e 6120 7769 7468  g the arena with
-0002cf80: 6f75 7420 7468 6520 616e 696d 616c 732e  out the animals.
-0002cf90: 0a0a 2020 2020 3a70 6172 616d 2055 6e69  ..    :param Uni
-0002cfa0: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-0002cfb0: 696b 655d 2076 6964 656f 5f70 6174 683a  ike] video_path:
-0002cfc0: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
-0002cfd0: 2076 6964 656f 2074 6f20 7265 6d6f 7665   video to remove
-0002cfe0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
-0002cff0: 6672 6f6d 2e0a 2020 2020 3a70 6172 616d  from..    :param
-0002d000: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-0002d010: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
-0002d020: 5d5d 2062 675f 7669 6465 6f5f 7061 7468  ]] bg_video_path
-0002d030: 3a20 5061 7468 2074 6f20 7468 6520 7669  : Path to the vi
-0002d040: 6465 6f20 7768 6963 6820 636f 6e74 6169  deo which contai
-0002d050: 6e73 2061 2073 6567 6d65 6e74 2077 6974  ns a segment wit
-0002d060: 6820 7468 6520 6261 636b 6772 6f75 6e64  h the background
-0002d070: 206f 6e6c 792e 2049 6620 4e6f 6e65 2c20   only. If None, 
-0002d080: 7468 656e 2060 6076 6964 656f 5f70 6174  then ``video_pat
-0002d090: 6860 6020 7769 6c6c 2062 6520 7573 6564  h`` will be used
-0002d0a0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
-0002d0b0: 696f 6e61 6c5b 696e 745d 2062 675f 7374  ional[int] bg_st
-0002d0c0: 6172 745f 6672 6d3a 2054 6865 2066 6972  art_frm: The fir
-0002d0d0: 7374 2066 7261 6d65 2069 6e20 7468 6520  st frame in the 
-0002d0e0: 6261 636b 6772 6f75 6e64 2076 6964 656f  background video
-0002d0f0: 2074 6f20 7573 6520 7768 656e 2063 7265   to use when cre
-0002d100: 6174 696e 6720 6120 7265 7072 6573 656e  ating a represen
-0002d110: 7461 7469 7665 2062 6163 6b67 726f 756e  tative backgroun
-0002d120: 6420 696d 6167 652e 2044 6566 6175 6c74  d image. Default
-0002d130: 3a20 4e6f 6e65 2e0a 2020 2020 3a70 6172  : None..    :par
-0002d140: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
-0002d150: 2062 675f 656e 645f 6672 6d3a 2054 6865   bg_end_frm: The
-0002d160: 206c 6173 7420 6672 616d 6520 696e 2074   last frame in t
-0002d170: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
-0002d180: 6465 6f20 746f 2075 7365 2077 6865 6e20  deo to use when 
-0002d190: 6372 6561 7469 6e67 2061 2072 6570 7265  creating a repre
-0002d1a0: 7365 6e74 6174 6976 6520 6261 636b 6772  sentative backgr
-0002d1b0: 6f75 6e64 2069 6d61 6765 2e20 4465 6661  ound image. Defa
-0002d1c0: 756c 743a 204e 6f6e 652e 0a20 2020 203a  ult: None..    :
-0002d1d0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b73  param Optional[s
-0002d1e0: 7472 5d20 6267 5f73 7461 7274 5f74 696d  tr] bg_start_tim
-0002d1f0: 653a 2054 6865 2073 7461 7274 2074 696d  e: The start tim
-0002d200: 6573 7461 6d70 2069 6e20 6048 483a 4d4d  estamp in `HH:MM
-0002d210: 3a53 5360 2066 6f72 6d61 7420 696e 2074  :SS` format in t
-0002d220: 6865 2062 6163 6b67 726f 756e 6420 7669  he background vi
-0002d230: 6465 6f20 746f 2075 7365 2074 6f20 6372  deo to use to cr
-0002d240: 6561 7465 2061 2072 6570 7265 7365 6e74  eate a represent
-0002d250: 6174 6976 6520 6261 636b 6772 6f75 6e64  ative background
-0002d260: 2069 6d61 6765 2e20 4465 6661 756c 743a   image. Default:
-0002d270: 204e 6f6e 652e 0a20 2020 203a 7061 7261   None..    :para
-0002d280: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
-0002d290: 6267 5f65 6e64 5f74 696d 653a 2054 6865  bg_end_time: The
-0002d2a0: 2065 6e64 2074 696d 6573 7461 6d70 2069   end timestamp i
-0002d2b0: 6e20 6048 483a 4d4d 3a53 5360 2066 6f72  n `HH:MM:SS` for
-0002d2c0: 6d61 7420 696e 2074 6865 2062 6163 6b67  mat in the backg
-0002d2d0: 726f 756e 6420 7669 6465 6f20 746f 2075  round video to u
-0002d2e0: 7365 2074 6f20 6372 6561 7465 2061 2072  se to create a r
-0002d2f0: 6570 7265 7365 6e74 6174 6976 6520 6261  epresentative ba
-0002d300: 636b 6772 6f75 6e64 2069 6d61 6765 2e20  ckground image. 
-0002d310: 4465 6661 756c 743a 204e 6f6e 652e 0a20  Default: None.. 
-0002d320: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
-0002d330: 616c 5b54 7570 6c65 5b69 6e74 2c20 696e  al[Tuple[int, in
-0002d340: 742c 2069 6e74 5d5d 2062 675f 636f 6c6f  t, int]] bg_colo
-0002d350: 723a 2054 6865 2052 4742 2063 6f6c 6f72  r: The RGB color
-0002d360: 206f 6620 7468 6520 6d6f 7669 6e67 206f   of the moving o
-0002d370: 626a 6563 7473 2069 6e20 7468 6520 6f75  bjects in the ou
-0002d380: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
-0002d390: 756c 7473 2074 6f20 4e6f 6e65 2c20 7768  ults to None, wh
-0002d3a0: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
-0002d3b0: 6865 206f 7269 6769 6e61 6c20 636f 6c6f  he original colo
-0002d3c0: 7273 206f 6620 7468 6520 6d6f 7669 6e67  rs of the moving
-0002d3d0: 206f 626a 6563 7473 2e0a 2020 2020 3a70   objects..    :p
-0002d3e0: 6172 616d 204f 7074 696f 6e61 6c5b 5475  aram Optional[Tu
-0002d3f0: 706c 655b 696e 742c 2069 6e74 2c20 696e  ple[int, int, in
-0002d400: 745d 5d20 6667 5f63 6f6c 6f72 3a20 5468  t]] fg_color: Th
-0002d410: 6520 5247 4220 636f 6c6f 7220 6f66 2074  e RGB color of t
-0002d420: 6865 2062 6163 6b67 726f 756e 6420 6f75  he background ou
-0002d430: 7470 7574 2076 6964 656f 2e20 4465 6661  tput video. Defa
-0002d440: 756c 7473 2074 6f20 626c 6163 6b20 2830  ults to black (0
-0002d450: 2c20 302c 2030 292e 0a20 2020 203a 7061  , 0, 0)..    :pa
-0002d460: 7261 6d20 4f70 7469 6f6e 616c 5b55 6e69  ram Optional[Uni
-0002d470: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-0002d480: 696b 655d 5d20 7361 7665 5f70 6174 683a  ike]] save_path:
-0002d490: 2054 6865 2070 6174 6368 2074 6f20 7768   The patch to wh
-0002d4a0: 6572 6520 746f 2073 6176 6520 7468 6520  ere to save the 
-0002d4b0: 6f75 7470 7574 2076 6964 656f 2077 6865  output video whe
-0002d4c0: 7265 2074 6865 2062 6163 6b67 726f 756e  re the backgroun
-0002d4d0: 6420 6973 2072 656d 6f76 6564 2e20 4966  d is removed. If
-0002d4e0: 204e 6f6e 652c 2073 6176 6573 2074 6865   None, saves the
-0002d4f0: 206f 7574 7075 7420 7669 6465 6f20 696e   output video in
-0002d500: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
-0002d510: 6f72 7920 6173 2074 6865 2069 6e70 7574  ory as the input
-0002d520: 2076 6964 656f 2077 6974 6820 7468 6520   video with the 
-0002d530: 6060 5f62 675f 7375 6274 7261 6374 6564  ``_bg_subtracted
-0002d540: 6060 2073 7566 6669 782e 2044 6566 6175  `` suffix. Defau
-0002d550: 6c74 3a20 4e6f 6e65 2e0a 2020 2020 3a70  lt: None..    :p
-0002d560: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
-0002d570: 745d 2063 6f72 655f 636e 743a 2054 6865  t] core_cnt: The
-0002d580: 206e 756d 6265 7220 6f66 2063 6f72 6573   number of cores
-0002d590: 2074 6f20 7573 652e 2044 6566 6175 6c74   to use. Default
-0002d5a0: 7320 746f 202d 3120 7265 7072 6573 656e  s to -1 represen
-0002d5b0: 7469 6e67 2061 6c6c 2061 7661 696c 6162  ting all availab
-0002d5c0: 6c65 2063 6f72 6573 2e0a 2020 2020 3a72  le cores..    :r
-0002d5d0: 6574 7572 6e3a 204e 6f6e 652e 0a0a 2020  eturn: None...  
-0002d5e0: 2020 3a65 7861 6d70 6c65 3a0a 2020 2020    :example:.    
-0002d5f0: 3e3e 3e20 7669 6465 6f5f 6267 5f73 7562  >>> video_bg_sub
-0002d600: 7374 7261 6374 696f 6e5f 6d70 2876 6964  straction_mp(vid
-0002d610: 656f 5f70 6174 683d 272f 5573 6572 732f  eo_path='/Users/
-0002d620: 7369 6d6f 6e2f 446f 776e 6c6f 6164 732f  simon/Downloads/
-0002d630: 315f 4c48 2e6d 7034 272c 2062 675f 7374  1_LH.mp4', bg_st
-0002d640: 6172 745f 7469 6d65 3d27 3030 3a30 303a  art_time='00:00:
-0002d650: 3030 272c 2062 675f 656e 645f 7469 6d65  00', bg_end_time
-0002d660: 3d27 3030 3a30 303a 3130 272c 2062 675f  ='00:00:10', bg_
-0002d670: 636f 6c6f 723d 2830 2c20 302c 2030 292c  color=(0, 0, 0),
-0002d680: 2066 675f 636f 6c6f 723d 2832 3535 2c20   fg_color=(255, 
-0002d690: 3235 352c 2032 3535 2929 0a20 2020 2022  255, 255)).    "
-0002d6a0: 2222 0a0a 2020 2020 7469 6d65 7220 3d20  ""..    timer = 
-0002d6b0: 5369 6d62 6154 696d 6572 2873 7461 7274  SimbaTimer(start
-0002d6c0: 3d54 7275 6529 0a20 2020 2063 6865 636b  =True).    check
-0002d6d0: 5f66 696c 655f 6578 6973 745f 616e 645f  _file_exist_and_
-0002d6e0: 7265 6164 6162 6c65 2866 696c 655f 7061  readable(file_pa
-0002d6f0: 7468 3d76 6964 656f 5f70 6174 6829 0a20  th=video_path). 
-0002d700: 2020 2069 6620 6267 5f76 6964 656f 5f70     if bg_video_p
-0002d710: 6174 6820 6973 204e 6f6e 653a 0a20 2020  ath is None:.   
-0002d720: 2020 2020 2062 675f 7669 6465 6f5f 7061       bg_video_pa
-0002d730: 7468 203d 2064 6565 7063 6f70 7928 7669  th = deepcopy(vi
-0002d740: 6465 6f5f 7061 7468 290a 2020 2020 7669  deo_path).    vi
-0002d750: 6465 6f5f 6d65 7461 5f64 6174 6120 3d20  deo_meta_data = 
-0002d760: 6765 745f 7669 6465 6f5f 6d65 7461 5f64  get_video_meta_d
-0002d770: 6174 6128 7669 6465 6f5f 7061 7468 3d76  ata(video_path=v
-0002d780: 6964 656f 5f70 6174 6829 0a20 2020 2064  ideo_path).    d
-0002d790: 6972 2c20 7669 6465 6f5f 6e61 6d65 2c20  ir, video_name, 
-0002d7a0: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
-0002d7b0: 2866 696c 6570 6174 683d 7669 6465 6f5f  (filepath=video_
-0002d7c0: 7061 7468 290a 2020 2020 6966 2073 6176  path).    if sav
-0002d7d0: 655f 7061 7468 2069 7320 4e6f 6e65 3a0a  e_path is None:.
-0002d7e0: 2020 2020 2020 2020 7361 7665 5f70 6174          save_pat
-0002d7f0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-0002d800: 2864 6972 2c20 6627 7b76 6964 656f 5f6e  (dir, f'{video_n
-0002d810: 616d 657d 5f62 675f 7375 6274 7261 6374  ame}_bg_subtract
-0002d820: 6564 7b65 7874 7d27 290a 2020 2020 6474  ed{ext}').    dt
-0002d830: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
-0002d840: 292e 7374 7266 7469 6d65 2822 2559 256d  ).strftime("%Y%m
-0002d850: 2564 2548 254d 2553 2229 0a20 2020 2074  %d%H%M%S").    t
-0002d860: 656d 705f 6469 7220 3d20 6f73 2e70 6174  emp_dir = os.pat
-0002d870: 682e 6a6f 696e 2864 6972 2c20 6627 7465  h.join(dir, f'te
-0002d880: 6d70 5f7b 7669 6465 6f5f 6e61 6d65 7d5f  mp_{video_name}_
-0002d890: 7b64 747d 2729 0a20 2020 206f 732e 6d61  {dt}').    os.ma
-0002d8a0: 6b65 6469 7273 2874 656d 705f 6469 7229  kedirs(temp_dir)
-0002d8b0: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
-0002d8c0: 616d 653d 6627 7b76 6964 656f 5f62 675f  ame=f'{video_bg_
-0002d8d0: 7375 6273 7472 6163 7469 6f6e 5f6d 702e  substraction_mp.
-0002d8e0: 5f5f 6e61 6d65 5f5f 7d20 636f 7265 5f63  __name__} core_c
-0002d8f0: 6e74 272c 2076 616c 7565 3d63 6f72 655f  nt', value=core_
-0002d900: 636e 742c 206d 696e 5f76 616c 7565 3d2d  cnt, min_value=-
-0002d910: 312c 206d 6178 5f76 616c 7565 3d66 696e  1, max_value=fin
-0002d920: 645f 636f 7265 5f63 6e74 2829 5b30 5d29  d_core_cnt()[0])
-0002d930: 0a20 2020 2069 6620 636f 7265 5f63 6e74  .    if core_cnt
-0002d940: 203d 3d20 2d31 3a20 636f 7265 5f63 6e74   == -1: core_cnt
-0002d950: 203d 2066 696e 645f 636f 7265 5f63 6e74   = find_core_cnt
-0002d960: 2829 5b30 5d0a 2020 2020 6267 5f66 726d  ()[0].    bg_frm
-0002d970: 203d 2063 7265 6174 655f 6176 6572 6167   = create_averag
-0002d980: 655f 6672 6d28 7669 6465 6f5f 7061 7468  e_frm(video_path
-0002d990: 3d62 675f 7669 6465 6f5f 7061 7468 2c20  =bg_video_path, 
-0002d9a0: 7374 6172 745f 6672 6d3d 6267 5f73 7461  start_frm=bg_sta
-0002d9b0: 7274 5f66 726d 2c20 656e 645f 6672 6d3d  rt_frm, end_frm=
-0002d9c0: 6267 5f65 6e64 5f66 726d 2c20 7374 6172  bg_end_frm, star
-0002d9d0: 745f 7469 6d65 3d62 675f 7374 6172 745f  t_time=bg_start_
-0002d9e0: 7469 6d65 2c20 656e 645f 7469 6d65 3d62  time, end_time=b
-0002d9f0: 675f 656e 645f 7469 6d65 290a 2020 2020  g_end_time).    
-0002da00: 6267 5f66 726d 203d 2063 7632 2e72 6573  bg_frm = cv2.res
-0002da10: 697a 6528 6267 5f66 726d 2c20 2876 6964  ize(bg_frm, (vid
-0002da20: 656f 5f6d 6574 615f 6461 7461 5b27 7769  eo_meta_data['wi
-0002da30: 6474 6827 5d2c 2076 6964 656f 5f6d 6574  dth'], video_met
-0002da40: 615f 6461 7461 5b27 6865 6967 6874 275d  a_data['height']
-0002da50: 2929 0a20 2020 2062 675f 6672 6d20 3d20  )).    bg_frm = 
-0002da60: 6267 5f66 726d 5b3a 2c20 3a2c 203a 3a2d  bg_frm[:, :, ::-
-0002da70: 315d 0a20 2020 2066 726d 5f6c 6973 7420  1].    frm_list 
-0002da80: 3d20 6e70 2e61 7272 6179 5f73 706c 6974  = np.array_split
-0002da90: 286c 6973 7428 7261 6e67 6528 302c 2076  (list(range(0, v
-0002daa0: 6964 656f 5f6d 6574 615f 6461 7461 5b27  ideo_meta_data['
-0002dab0: 6672 616d 655f 636f 756e 7427 5d29 292c  frame_count'])),
-0002dac0: 2063 6f72 655f 636e 7429 0a20 2020 2066   core_cnt).    f
-0002dad0: 726d 5f64 6174 6120 3d20 5b5d 0a20 2020  rm_data = [].   
-0002dae0: 2066 6f72 2063 2c20 6920 696e 2065 6e75   for c, i in enu
-0002daf0: 6d65 7261 7465 2866 726d 5f6c 6973 7429  merate(frm_list)
-0002db00: 3a0a 2020 2020 2020 2020 6672 6d5f 6461  :.        frm_da
-0002db10: 7461 2e61 7070 656e 6428 2863 2c20 6929  ta.append((c, i)
-0002db20: 290a 2020 2020 7769 7468 206d 756c 7469  ).    with multi
-0002db30: 7072 6f63 6573 7369 6e67 2e50 6f6f 6c28  processing.Pool(
-0002db40: 636f 7265 5f63 6e74 2c20 6d61 7874 6173  core_cnt, maxtas
-0002db50: 6b73 7065 7263 6869 6c64 3d39 3030 3029  ksperchild=9000)
-0002db60: 2061 7320 706f 6f6c 3a0a 2020 2020 2020   as pool:.      
-0002db70: 2020 636f 6e73 7461 6e74 7320 3d20 6675    constants = fu
-0002db80: 6e63 746f 6f6c 732e 7061 7274 6961 6c28  nctools.partial(
-0002db90: 5f62 675f 7265 6d6f 7665 725f 6d70 2c0a  _bg_remover_mp,.
-0002dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dbc0: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
-0002dbd0: 3d76 6964 656f 5f70 6174 682c 0a20 2020  =video_path,.   
-0002dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc00: 2020 2062 675f 6672 6d3d 6267 5f66 726d     bg_frm=bg_frm
-0002dc10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc30: 2020 2020 2020 2020 6267 5f63 6c72 3d62          bg_clr=b
-0002dc40: 675f 636f 6c6f 722c 0a20 2020 2020 2020  g_color,.       
-0002dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dc60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0002dc70: 675f 636c 723d 6667 5f63 6f6c 6f72 2c0a  g_clr=fg_color,.
+0002ca20: 2020 2020 2020 2020 2020 2062 675f 7374             bg_st
+0002ca30: 6172 745f 7469 6d65 3a20 4f70 7469 6f6e  art_time: Option
+0002ca40: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0002ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ca60: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
+0002ca70: 656e 645f 7469 6d65 3a20 4f70 7469 6f6e  end_time: Option
+0002ca80: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0002ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002caa0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
+0002cab0: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
+0002cac0: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
+0002cad0: 696e 745d 5d20 3d20 2830 2c20 302c 2030  int]] = (0, 0, 0
+0002cae0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0002caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cb00: 6667 5f63 6f6c 6f72 3a20 4f70 7469 6f6e  fg_color: Option
+0002cb10: 616c 5b54 7570 6c65 5b69 6e74 2c20 696e  al[Tuple[int, in
+0002cb20: 742c 2069 6e74 5d5d 203d 204e 6f6e 652c  t, int]] = None,
+0002cb30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cb40: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0002cb50: 7665 5f70 6174 683a 204f 7074 696f 6e61  ve_path: Optiona
+0002cb60: 6c5b 556e 696f 6e5b 7374 722c 206f 732e  l[Union[str, os.
+0002cb70: 5061 7468 4c69 6b65 5d5d 203d 204e 6f6e  PathLike]] = Non
+0002cb80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cba0: 636f 7265 5f63 6e74 3a20 4f70 7469 6f6e  core_cnt: Option
+0002cbb0: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
+0002cbc0: 204e 6f6e 653a 0a0a 2020 2020 2222 220a   None:..    """.
+0002cbd0: 2020 2020 5375 6274 7261 6374 2074 6865      Subtract the
+0002cbe0: 2062 6163 6b67 726f 756e 6420 6672 6f6d   background from
+0002cbf0: 2061 2076 6964 656f 2075 7369 6e67 206d   a video using m
+0002cc00: 756c 7469 7072 6f63 6573 7369 6e67 2e0a  ultiprocessing..
+0002cc10: 0a20 2020 202e 2e20 7669 6465 6f3a 3a20  .    .. video:: 
+0002cc20: 5f73 7461 7469 632f 696d 672f 7669 6465  _static/img/vide
+0002cc30: 6f5f 6267 5f73 7562 7374 7261 6374 696f  o_bg_substractio
+0002cc40: 6e5f 6d70 2e77 6562 6d0a 2020 2020 2020  n_mp.webm.      
+0002cc50: 203a 7769 6474 683a 2039 3030 0a20 2020   :width: 900.   
+0002cc60: 2020 2020 3a61 7574 6f70 6c61 793a 0a20      :autoplay:. 
+0002cc70: 2020 2020 2020 3a6c 6f6f 703a 0a0a 2020        :loop:..  
+0002cc80: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+0002cc90: 2020 2020 466f 7220 7369 6e67 6c65 2063      For single c
+0002cca0: 6f72 6520 616c 7465 726e 6174 6976 652c  ore alternative,
+0002ccb0: 2073 6565 2060 6073 696d 6261 2e76 6964   see ``simba.vid
+0002ccc0: 656f 5f70 726f 6365 7373 6f72 732e 7669  eo_processors.vi
+0002ccd0: 6465 6f5f 7072 6f63 6573 7369 6e67 2e76  deo_processing.v
+0002cce0: 6964 656f 5f62 675f 7375 6274 7261 6374  ideo_bg_subtract
+0002ccf0: 696f 6e60 600a 0a20 2020 2020 2020 4966  ion``..       If
+0002cd00: 2020 6060 6267 5f76 6964 656f 5f70 6174    ``bg_video_pat
+0002cd10: 6860 6020 6973 2070 6173 7365 642c 2074  h`` is passed, t
+0002cd20: 6861 7420 7669 6465 6f20 7769 6c6c 2062  hat video will b
+0002cd30: 6520 7573 6564 2074 6f20 7061 7273 6520  e used to parse 
+0002cd40: 7468 6520 6261 636b 6772 6f75 6e64 2e20  the background. 
+0002cd50: 4966 204e 6f6e 652c 2060 6076 6964 656f  If None, ``video
+0002cd60: 5f70 6174 6860 6020 7769 6c6c 2062 6520  _path`` will be 
+0002cd70: 7573 6520 6474 6f20 7061 7273 6520 6261  use dto parse ba
+0002cd80: 636b 6772 6f75 6e64 2e0a 2020 2020 2020  ckground..      
+0002cd90: 2045 6974 6865 7220 7061 7373 2060 6073   Either pass ``s
+0002cda0: 7461 7274 5f66 726d 6060 2061 6e64 2060  tart_frm`` and `
+0002cdb0: 6065 6e64 5f66 726d 6060 204f 5220 6060  `end_frm`` OR ``
+0002cdc0: 7374 6172 745f 7469 6d65 6060 2061 6e64  start_time`` and
+0002cdd0: 2060 6065 6e64 5f74 696d 6560 6020 4f52   ``end_time`` OR
+0002cde0: 2070 6173 7320 616c 6c20 666f 7572 2061   pass all four a
+0002cdf0: 7267 756d 656e 7473 2061 7320 4e6f 6e65  rguments as None
+0002ce00: 2e0a 2020 2020 2020 2054 686f 7365 2074  ..       Those t
+0002ce10: 776f 2061 7267 756d 656e 7473 2077 696c  wo arguments wil
+0002ce20: 6c20 6265 2075 7365 6420 746f 2073 6c69  l be used to sli
+0002ce30: 6365 2074 6865 2062 6163 6b67 726f 756e  ce the backgroun
+0002ce40: 6420 7669 6465 6f2c 2061 6e64 2074 6865  d video, and the
+0002ce50: 2073 6c69 6365 6420 7061 7274 2069 7320   sliced part is 
+0002ce60: 7573 6564 2074 6f20 7061 7273 6520 7468  used to parse th
+0002ce70: 6520 6261 636b 6772 6f75 6e64 2e0a 0a20  e background... 
+0002ce80: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
+0002ce90: 652c 2069 6e20 7468 6520 7363 656e 6172  e, in the scenar
+0002cea0: 696f 2077 6865 7265 2074 6865 7265 2069  io where there i
+0002ceb0: 7320 2a2a 6e6f 2a2a 2061 6e69 6d61 6c20  s **no** animal 
+0002cec0: 696e 2074 6865 2060 6076 6964 656f 5f70  in the ``video_p
+0002ced0: 6174 6860 6020 7669 6465 6f20 666f 7220  ath`` video for 
+0002cee0: 7468 6520 6669 7273 7420 3230 732c 2074  the first 20s, t
+0002cef0: 6865 6e20 7468 6520 6669 7273 7420 3230  hen the first 20
+0002cf00: 7320 6361 6e20 6265 2075 7365 6420 746f  s can be used to
+0002cf10: 2070 6172 7365 2074 6865 2062 6163 6b67   parse the backg
+0002cf20: 726f 756e 642e 0a20 2020 2020 2020 496e  round..       In
+0002cf30: 2074 6869 7320 7363 656e 6172 696f 2c20   this scenario, 
+0002cf40: 6060 6267 5f76 6964 656f 5f70 6174 6860  ``bg_video_path`
+0002cf50: 6020 6361 6e20 6265 2070 6173 7365 6420  ` can be passed 
+0002cf60: 6173 2060 604e 6f6e 6560 6020 616e 6420  as ``None`` and 
+0002cf70: 6267 5f73 7461 7274 5f74 696d 6520 616e  bg_start_time an
+0002cf80: 6420 6267 5f65 6e64 5f74 696d 6520 6361  d bg_end_time ca
+0002cf90: 6e20 6265 2060 6030 303a 3030 3a30 3060  n be ``00:00:00`
+0002cfa0: 6020 616e 6420 6060 3030 3a30 303a 3230  ` and ``00:00:20
+0002cfb0: 6060 2c20 7265 7065 6374 6976 656c 792e  ``, repectively.
+0002cfc0: 0a0a 2020 2020 2020 2049 6e20 7468 6520  ..       In the 
+0002cfd0: 7363 656e 6172 696f 2077 6865 7265 2074  scenario where t
+0002cfe0: 6865 7265 202a 2a69 732a 2a20 616e 696d  here **is** anim
+0002cff0: 616c 2873 2920 696e 2074 6865 2065 6e74  al(s) in the ent
+0002d000: 6972 6520 6060 7669 6465 6f5f 7061 7468  ire ``video_path
+0002d010: 6060 2076 6964 656f 2c20 7061 7373 2060  `` video, pass `
+0002d020: 6062 675f 7669 6465 6f5f 7061 7468 6060  `bg_video_path``
+0002d030: 2061 7320 6120 7061 7468 2074 6f20 6120   as a path to a 
+0002d040: 7669 6465 6f20 7265 636f 7264 696e 6720  video recording 
+0002d050: 7468 6520 6172 656e 6120 7769 7468 6f75  the arena withou
+0002d060: 7420 7468 6520 616e 696d 616c 732e 0a0a  t the animals...
+0002d070: 2020 2020 3a70 6172 616d 2055 6e69 6f6e      :param Union
+0002d080: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+0002d090: 655d 2076 6964 656f 5f70 6174 683a 2054  e] video_path: T
+0002d0a0: 6865 2070 6174 6820 746f 2074 6865 2076  he path to the v
+0002d0b0: 6964 656f 2074 6f20 7265 6d6f 7665 2074  ideo to remove t
+0002d0c0: 6865 2062 6163 6b67 726f 756e 6420 6672  he background fr
+0002d0d0: 6f6d 2e0a 2020 2020 3a70 6172 616d 204f  om..    :param O
+0002d0e0: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+0002d0f0: 722c 206f 732e 5061 7468 4c69 6b65 5d5d  r, os.PathLike]]
+0002d100: 2062 675f 7669 6465 6f5f 7061 7468 3a20   bg_video_path: 
+0002d110: 5061 7468 2074 6f20 7468 6520 7669 6465  Path to the vide
+0002d120: 6f20 7768 6963 6820 636f 6e74 6169 6e73  o which contains
+0002d130: 2061 2073 6567 6d65 6e74 2077 6974 6820   a segment with 
+0002d140: 7468 6520 6261 636b 6772 6f75 6e64 206f  the background o
+0002d150: 6e6c 792e 2049 6620 4e6f 6e65 2c20 7468  nly. If None, th
+0002d160: 656e 2060 6076 6964 656f 5f70 6174 6860  en ``video_path`
+0002d170: 6020 7769 6c6c 2062 6520 7573 6564 2e0a  ` will be used..
+0002d180: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+0002d190: 6e61 6c5b 696e 745d 2062 675f 7374 6172  nal[int] bg_star
+0002d1a0: 745f 6672 6d3a 2054 6865 2066 6972 7374  t_frm: The first
+0002d1b0: 2066 7261 6d65 2069 6e20 7468 6520 6261   frame in the ba
+0002d1c0: 636b 6772 6f75 6e64 2076 6964 656f 2074  ckground video t
+0002d1d0: 6f20 7573 6520 7768 656e 2063 7265 6174  o use when creat
+0002d1e0: 696e 6720 6120 7265 7072 6573 656e 7461  ing a representa
+0002d1f0: 7469 7665 2062 6163 6b67 726f 756e 6420  tive background 
+0002d200: 696d 6167 652e 2044 6566 6175 6c74 3a20  image. Default: 
+0002d210: 4e6f 6e65 2e0a 2020 2020 3a70 6172 616d  None..    :param
+0002d220: 204f 7074 696f 6e61 6c5b 696e 745d 2062   Optional[int] b
+0002d230: 675f 656e 645f 6672 6d3a 2054 6865 206c  g_end_frm: The l
+0002d240: 6173 7420 6672 616d 6520 696e 2074 6865  ast frame in the
+0002d250: 2062 6163 6b67 726f 756e 6420 7669 6465   background vide
+0002d260: 6f20 746f 2075 7365 2077 6865 6e20 6372  o to use when cr
+0002d270: 6561 7469 6e67 2061 2072 6570 7265 7365  eating a represe
+0002d280: 6e74 6174 6976 6520 6261 636b 6772 6f75  ntative backgrou
+0002d290: 6e64 2069 6d61 6765 2e20 4465 6661 756c  nd image. Defaul
+0002d2a0: 743a 204e 6f6e 652e 0a20 2020 203a 7061  t: None..    :pa
+0002d2b0: 7261 6d20 4f70 7469 6f6e 616c 5b73 7472  ram Optional[str
+0002d2c0: 5d20 6267 5f73 7461 7274 5f74 696d 653a  ] bg_start_time:
+0002d2d0: 2054 6865 2073 7461 7274 2074 696d 6573   The start times
+0002d2e0: 7461 6d70 2069 6e20 6048 483a 4d4d 3a53  tamp in `HH:MM:S
+0002d2f0: 5360 2066 6f72 6d61 7420 696e 2074 6865  S` format in the
+0002d300: 2062 6163 6b67 726f 756e 6420 7669 6465   background vide
+0002d310: 6f20 746f 2075 7365 2074 6f20 6372 6561  o to use to crea
+0002d320: 7465 2061 2072 6570 7265 7365 6e74 6174  te a representat
+0002d330: 6976 6520 6261 636b 6772 6f75 6e64 2069  ive background i
+0002d340: 6d61 6765 2e20 4465 6661 756c 743a 204e  mage. Default: N
+0002d350: 6f6e 652e 0a20 2020 203a 7061 7261 6d20  one..    :param 
+0002d360: 4f70 7469 6f6e 616c 5b73 7472 5d20 6267  Optional[str] bg
+0002d370: 5f65 6e64 5f74 696d 653a 2054 6865 2065  _end_time: The e
+0002d380: 6e64 2074 696d 6573 7461 6d70 2069 6e20  nd timestamp in 
+0002d390: 6048 483a 4d4d 3a53 5360 2066 6f72 6d61  `HH:MM:SS` forma
+0002d3a0: 7420 696e 2074 6865 2062 6163 6b67 726f  t in the backgro
+0002d3b0: 756e 6420 7669 6465 6f20 746f 2075 7365  und video to use
+0002d3c0: 2074 6f20 6372 6561 7465 2061 2072 6570   to create a rep
+0002d3d0: 7265 7365 6e74 6174 6976 6520 6261 636b  resentative back
+0002d3e0: 6772 6f75 6e64 2069 6d61 6765 2e20 4465  ground image. De
+0002d3f0: 6661 756c 743a 204e 6f6e 652e 0a20 2020  fault: None..   
+0002d400: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+0002d410: 5b54 7570 6c65 5b69 6e74 2c20 696e 742c  [Tuple[int, int,
+0002d420: 2069 6e74 5d5d 2062 675f 636f 6c6f 723a   int]] bg_color:
+0002d430: 2054 6865 2052 4742 2063 6f6c 6f72 206f   The RGB color o
+0002d440: 6620 7468 6520 6d6f 7669 6e67 206f 626a  f the moving obj
+0002d450: 6563 7473 2069 6e20 7468 6520 6f75 7470  ects in the outp
+0002d460: 7574 2076 6964 656f 2e20 4465 6661 756c  ut video. Defaul
+0002d470: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
+0002d480: 6820 7265 7072 6573 656e 7473 2074 6865  h represents the
+0002d490: 206f 7269 6769 6e61 6c20 636f 6c6f 7273   original colors
+0002d4a0: 206f 6620 7468 6520 6d6f 7669 6e67 206f   of the moving o
+0002d4b0: 626a 6563 7473 2e0a 2020 2020 3a70 6172  bjects..    :par
+0002d4c0: 616d 204f 7074 696f 6e61 6c5b 5475 706c  am Optional[Tupl
+0002d4d0: 655b 696e 742c 2069 6e74 2c20 696e 745d  e[int, int, int]
+0002d4e0: 5d20 6667 5f63 6f6c 6f72 3a20 5468 6520  ] fg_color: The 
+0002d4f0: 5247 4220 636f 6c6f 7220 6f66 2074 6865  RGB color of the
+0002d500: 2062 6163 6b67 726f 756e 6420 6f75 7470   background outp
+0002d510: 7574 2076 6964 656f 2e20 4465 6661 756c  ut video. Defaul
+0002d520: 7473 2074 6f20 626c 6163 6b20 2830 2c20  ts to black (0, 
+0002d530: 302c 2030 292e 0a20 2020 203a 7061 7261  0, 0)..    :para
+0002d540: 6d20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  m Optional[Union
+0002d550: 5b73 7472 2c20 6f73 2e50 6174 684c 696b  [str, os.PathLik
+0002d560: 655d 5d20 7361 7665 5f70 6174 683a 2054  e]] save_path: T
+0002d570: 6865 2070 6174 6368 2074 6f20 7768 6572  he patch to wher
+0002d580: 6520 746f 2073 6176 6520 7468 6520 6f75  e to save the ou
+0002d590: 7470 7574 2076 6964 656f 2077 6865 7265  tput video where
+0002d5a0: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+0002d5b0: 6973 2072 656d 6f76 6564 2e20 4966 204e  is removed. If N
+0002d5c0: 6f6e 652c 2073 6176 6573 2074 6865 206f  one, saves the o
+0002d5d0: 7574 7075 7420 7669 6465 6f20 696e 2074  utput video in t
+0002d5e0: 6865 2073 616d 6520 6469 7265 6374 6f72  he same director
+0002d5f0: 7920 6173 2074 6865 2069 6e70 7574 2076  y as the input v
+0002d600: 6964 656f 2077 6974 6820 7468 6520 6060  ideo with the ``
+0002d610: 5f62 675f 7375 6274 7261 6374 6564 6060  _bg_subtracted``
+0002d620: 2073 7566 6669 782e 2044 6566 6175 6c74   suffix. Default
+0002d630: 3a20 4e6f 6e65 2e0a 2020 2020 3a70 6172  : None..    :par
+0002d640: 616d 204f 7074 696f 6e61 6c5b 696e 745d  am Optional[int]
+0002d650: 2063 6f72 655f 636e 743a 2054 6865 206e   core_cnt: The n
+0002d660: 756d 6265 7220 6f66 2063 6f72 6573 2074  umber of cores t
+0002d670: 6f20 7573 652e 2044 6566 6175 6c74 7320  o use. Defaults 
+0002d680: 746f 202d 3120 7265 7072 6573 656e 7469  to -1 representi
+0002d690: 6e67 2061 6c6c 2061 7661 696c 6162 6c65  ng all available
+0002d6a0: 2063 6f72 6573 2e0a 2020 2020 3a72 6574   cores..    :ret
+0002d6b0: 7572 6e3a 204e 6f6e 652e 0a0a 2020 2020  urn: None...    
+0002d6c0: 3a65 7861 6d70 6c65 3a0a 2020 2020 3e3e  :example:.    >>
+0002d6d0: 3e20 7669 6465 6f5f 6267 5f73 7562 7374  > video_bg_subst
+0002d6e0: 7261 6374 696f 6e5f 6d70 2876 6964 656f  raction_mp(video
+0002d6f0: 5f70 6174 683d 272f 5573 6572 732f 7369  _path='/Users/si
+0002d700: 6d6f 6e2f 446f 776e 6c6f 6164 732f 315f  mon/Downloads/1_
+0002d710: 4c48 2e6d 7034 272c 2062 675f 7374 6172  LH.mp4', bg_star
+0002d720: 745f 7469 6d65 3d27 3030 3a30 303a 3030  t_time='00:00:00
+0002d730: 272c 2062 675f 656e 645f 7469 6d65 3d27  ', bg_end_time='
+0002d740: 3030 3a30 303a 3130 272c 2062 675f 636f  00:00:10', bg_co
+0002d750: 6c6f 723d 2830 2c20 302c 2030 292c 2066  lor=(0, 0, 0), f
+0002d760: 675f 636f 6c6f 723d 2832 3535 2c20 3235  g_color=(255, 25
+0002d770: 352c 2032 3535 2929 0a20 2020 2022 2222  5, 255)).    """
+0002d780: 0a0a 2020 2020 7469 6d65 7220 3d20 5369  ..    timer = Si
+0002d790: 6d62 6154 696d 6572 2873 7461 7274 3d54  mbaTimer(start=T
+0002d7a0: 7275 6529 0a20 2020 2063 6865 636b 5f66  rue).    check_f
+0002d7b0: 696c 655f 6578 6973 745f 616e 645f 7265  ile_exist_and_re
+0002d7c0: 6164 6162 6c65 2866 696c 655f 7061 7468  adable(file_path
+0002d7d0: 3d76 6964 656f 5f70 6174 6829 0a20 2020  =video_path).   
+0002d7e0: 2069 6620 6267 5f76 6964 656f 5f70 6174   if bg_video_pat
+0002d7f0: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+0002d800: 2020 2062 675f 7669 6465 6f5f 7061 7468     bg_video_path
+0002d810: 203d 2064 6565 7063 6f70 7928 7669 6465   = deepcopy(vide
+0002d820: 6f5f 7061 7468 290a 2020 2020 7669 6465  o_path).    vide
+0002d830: 6f5f 6d65 7461 5f64 6174 6120 3d20 6765  o_meta_data = ge
+0002d840: 745f 7669 6465 6f5f 6d65 7461 5f64 6174  t_video_meta_dat
+0002d850: 6128 7669 6465 6f5f 7061 7468 3d76 6964  a(video_path=vid
+0002d860: 656f 5f70 6174 6829 0a20 2020 2064 6972  eo_path).    dir
+0002d870: 2c20 7669 6465 6f5f 6e61 6d65 2c20 6578  , video_name, ex
+0002d880: 7420 3d20 6765 745f 666e 5f65 7874 2866  t = get_fn_ext(f
+0002d890: 696c 6570 6174 683d 7669 6465 6f5f 7061  ilepath=video_pa
+0002d8a0: 7468 290a 2020 2020 6966 2073 6176 655f  th).    if save_
+0002d8b0: 7061 7468 2069 7320 4e6f 6e65 3a0a 2020  path is None:.  
+0002d8c0: 2020 2020 2020 7361 7665 5f70 6174 6820        save_path 
+0002d8d0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2864  = os.path.join(d
+0002d8e0: 6972 2c20 6627 7b76 6964 656f 5f6e 616d  ir, f'{video_nam
+0002d8f0: 657d 5f62 675f 7375 6274 7261 6374 6564  e}_bg_subtracted
+0002d900: 7b65 7874 7d27 290a 2020 2020 6474 203d  {ext}').    dt =
+0002d910: 2064 6174 6574 696d 652e 6e6f 7728 292e   datetime.now().
+0002d920: 7374 7266 7469 6d65 2822 2559 256d 2564  strftime("%Y%m%d
+0002d930: 2548 254d 2553 2229 0a20 2020 2074 656d  %H%M%S").    tem
+0002d940: 705f 6469 7220 3d20 6f73 2e70 6174 682e  p_dir = os.path.
+0002d950: 6a6f 696e 2864 6972 2c20 6627 7465 6d70  join(dir, f'temp
+0002d960: 5f7b 7669 6465 6f5f 6e61 6d65 7d5f 7b64  _{video_name}_{d
+0002d970: 747d 2729 0a20 2020 206f 732e 6d61 6b65  t}').    os.make
+0002d980: 6469 7273 2874 656d 705f 6469 7229 0a20  dirs(temp_dir). 
+0002d990: 2020 2063 6865 636b 5f69 6e74 286e 616d     check_int(nam
+0002d9a0: 653d 6627 7b76 6964 656f 5f62 675f 7375  e=f'{video_bg_su
+0002d9b0: 6273 7472 6163 7469 6f6e 5f6d 702e 5f5f  bstraction_mp.__
+0002d9c0: 6e61 6d65 5f5f 7d20 636f 7265 5f63 6e74  name__} core_cnt
+0002d9d0: 272c 2076 616c 7565 3d63 6f72 655f 636e  ', value=core_cn
+0002d9e0: 742c 206d 696e 5f76 616c 7565 3d2d 312c  t, min_value=-1,
+0002d9f0: 206d 6178 5f76 616c 7565 3d66 696e 645f   max_value=find_
+0002da00: 636f 7265 5f63 6e74 2829 5b30 5d29 0a20  core_cnt()[0]). 
+0002da10: 2020 2069 6620 636f 7265 5f63 6e74 203d     if core_cnt =
+0002da20: 3d20 2d31 3a20 636f 7265 5f63 6e74 203d  = -1: core_cnt =
+0002da30: 2066 696e 645f 636f 7265 5f63 6e74 2829   find_core_cnt()
+0002da40: 5b30 5d0a 2020 2020 6267 5f66 726d 203d  [0].    bg_frm =
+0002da50: 2063 7265 6174 655f 6176 6572 6167 655f   create_average_
+0002da60: 6672 6d28 7669 6465 6f5f 7061 7468 3d62  frm(video_path=b
+0002da70: 675f 7669 6465 6f5f 7061 7468 2c20 7374  g_video_path, st
+0002da80: 6172 745f 6672 6d3d 6267 5f73 7461 7274  art_frm=bg_start
+0002da90: 5f66 726d 2c20 656e 645f 6672 6d3d 6267  _frm, end_frm=bg
+0002daa0: 5f65 6e64 5f66 726d 2c20 7374 6172 745f  _end_frm, start_
+0002dab0: 7469 6d65 3d62 675f 7374 6172 745f 7469  time=bg_start_ti
+0002dac0: 6d65 2c20 656e 645f 7469 6d65 3d62 675f  me, end_time=bg_
+0002dad0: 656e 645f 7469 6d65 290a 2020 2020 6267  end_time).    bg
+0002dae0: 5f66 726d 203d 2063 7632 2e72 6573 697a  _frm = cv2.resiz
+0002daf0: 6528 6267 5f66 726d 2c20 2876 6964 656f  e(bg_frm, (video
+0002db00: 5f6d 6574 615f 6461 7461 5b27 7769 6474  _meta_data['widt
+0002db10: 6827 5d2c 2076 6964 656f 5f6d 6574 615f  h'], video_meta_
+0002db20: 6461 7461 5b27 6865 6967 6874 275d 2929  data['height']))
+0002db30: 0a20 2020 2062 675f 6672 6d20 3d20 6267  .    bg_frm = bg
+0002db40: 5f66 726d 5b3a 2c20 3a2c 203a 3a2d 315d  _frm[:, :, ::-1]
+0002db50: 0a20 2020 2066 726d 5f6c 6973 7420 3d20  .    frm_list = 
+0002db60: 6e70 2e61 7272 6179 5f73 706c 6974 286c  np.array_split(l
+0002db70: 6973 7428 7261 6e67 6528 302c 2076 6964  ist(range(0, vid
+0002db80: 656f 5f6d 6574 615f 6461 7461 5b27 6672  eo_meta_data['fr
+0002db90: 616d 655f 636f 756e 7427 5d29 292c 2063  ame_count'])), c
+0002dba0: 6f72 655f 636e 7429 0a20 2020 2066 726d  ore_cnt).    frm
+0002dbb0: 5f64 6174 6120 3d20 5b5d 0a20 2020 2066  _data = [].    f
+0002dbc0: 6f72 2063 2c20 6920 696e 2065 6e75 6d65  or c, i in enume
+0002dbd0: 7261 7465 2866 726d 5f6c 6973 7429 3a0a  rate(frm_list):.
+0002dbe0: 2020 2020 2020 2020 6672 6d5f 6461 7461          frm_data
+0002dbf0: 2e61 7070 656e 6428 2863 2c20 6929 290a  .append((c, i)).
+0002dc00: 2020 2020 7769 7468 206d 756c 7469 7072      with multipr
+0002dc10: 6f63 6573 7369 6e67 2e50 6f6f 6c28 636f  ocessing.Pool(co
+0002dc20: 7265 5f63 6e74 2c20 6d61 7874 6173 6b73  re_cnt, maxtasks
+0002dc30: 7065 7263 6869 6c64 3d39 3030 3029 2061  perchild=9000) a
+0002dc40: 7320 706f 6f6c 3a0a 2020 2020 2020 2020  s pool:.        
+0002dc50: 636f 6e73 7461 6e74 7320 3d20 6675 6e63  constants = func
+0002dc60: 746f 6f6c 732e 7061 7274 6961 6c28 5f62  tools.partial(_b
+0002dc70: 675f 7265 6d6f 7665 725f 6d70 2c0a 2020  g_remover_mp,.  
 0002dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dca0: 2020 2020 2020 7669 6465 6f5f 6d65 7461        video_meta
-0002dcb0: 5f64 6174 613d 7669 6465 6f5f 6d65 7461  _data=video_meta
-0002dcc0: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+0002dca0: 2020 2020 7669 6465 6f5f 7061 7468 3d76      video_path=v
+0002dcb0: 6964 656f 5f70 6174 682c 0a20 2020 2020  ideo_path,.     
+0002dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dce0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0002dcf0: 705f 6469 723d 7465 6d70 5f64 6972 290a  p_dir=temp_dir).
-0002dd00: 2020 2020 2020 2020 666f 7220 636e 742c          for cnt,
-0002dd10: 2072 6573 756c 7420 696e 2065 6e75 6d65   result in enume
-0002dd20: 7261 7465 2870 6f6f 6c2e 696d 6170 2863  rate(pool.imap(c
-0002dd30: 6f6e 7374 616e 7473 2c20 6672 6d5f 6461  onstants, frm_da
-0002dd40: 7461 2c20 6368 756e 6b73 697a 653d 3129  ta, chunksize=1)
-0002dd50: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-0002dd60: 7269 6e74 2866 2746 7261 6d65 2062 6174  rint(f'Frame bat
-0002dd70: 6368 207b 7265 7375 6c74 2b31 7d20 636f  ch {result+1} co
-0002dd80: 6d70 6c65 7465 642e 2e2e 2729 0a20 2020  mpleted...').   
-0002dd90: 2020 2020 2070 6f6f 6c2e 7465 726d 696e       pool.termin
-0002dda0: 6174 6528 290a 2020 2020 2020 2020 706f  ate().        po
-0002ddb0: 6f6c 2e6a 6f69 6e28 290a 0a20 2020 2070  ol.join()..    p
-0002ddc0: 7269 6e74 2866 224a 6f69 6e69 6e67 207b  rint(f"Joining {
-0002ddd0: 7669 6465 6f5f 6e61 6d65 7d20 6d75 6c74  video_name} mult
-0002dde0: 6970 726f 6365 7373 6564 2076 6964 656f  iprocessed video
-0002ddf0: 2e2e 2e22 290a 2020 2020 636f 6e63 6174  ...").    concat
-0002de00: 656e 6174 655f 7669 6465 6f73 5f69 6e5f  enate_videos_in_
-0002de10: 666f 6c64 6572 2869 6e5f 666f 6c64 6572  folder(in_folder
-0002de20: 3d74 656d 705f 6469 722c 2073 6176 655f  =temp_dir, save_
-0002de30: 7061 7468 3d73 6176 655f 7061 7468 2c20  path=save_path, 
-0002de40: 7669 6465 6f5f 666f 726d 6174 3d65 7874  video_format=ext
-0002de50: 5b31 3a5d 2c20 7265 6d6f 7665 5f73 706c  [1:], remove_spl
-0002de60: 6974 733d 5472 7565 290a 2020 2020 7469  its=True).    ti
-0002de70: 6d65 722e 7374 6f70 5f74 696d 6572 2829  mer.stop_timer()
-0002de80: 0a20 2020 2073 7464 6f75 745f 7375 6363  .    stdout_succ
-0002de90: 6573 7328 6d73 673d 6627 5669 6465 6f20  ess(msg=f'Video 
-0002dea0: 7361 7665 6420 6174 207b 7361 7665 5f70  saved at {save_p
-0002deb0: 6174 687d 272c 2065 6c61 7073 6564 5f74  ath}', elapsed_t
-0002dec0: 696d 653d 7469 6d65 722e 656c 6170 7365  ime=timer.elapse
-0002ded0: 645f 7469 6d65 5f73 7472 290a 0a0a 0a0a  d_time_str).....
-0002dee0: 2320 7669 6465 6f5f 7061 7468 7320 3d20  # video_paths = 
-0002def0: 5b27 2f55 7365 7273 2f73 696d 6f6e 2f44  ['/Users/simon/D
-0002df00: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0002df10: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0002df20: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0002df30: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
-0002df40: 6765 2f54 7269 616c 2020 2020 3130 5f63  ge/Trial    10_c
-0002df50: 6c69 7070 6564 5f67 616e 7474 2e6d 7034  lipped_gantt.mp4
-0002df60: 272c 0a23 2020 2020 2020 2020 2020 2020  ',.#            
-0002df70: 2020 2020 272f 5573 6572 732f 7369 6d6f      '/Users/simo
-0002df80: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
-0002df90: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
-0002dfa0: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
-0002dfb0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
-0002dfc0: 6d65 7267 652f 5472 6961 6c20 2020 2031  merge/Trial    1
-0002dfd0: 305f 636c 6970 7065 642e 6d70 3427 2c0a  0_clipped.mp4',.
-0002dfe0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002dff0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
-0002e000: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0002e010: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0002e020: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0002e030: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
-0002e040: 6765 2f54 7269 616c 2020 2020 3130 5f63  ge/Trial    10_c
-0002e050: 6c69 7070 6564 5f6c 696e 652e 6d70 3427  lipped_line.mp4'
-0002e060: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
-0002e070: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
-0002e080: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-0002e090: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-0002e0a0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
-0002e0b0: 7072 6f6a 6563 745f 666f 6c64 6572 2f6d  project_folder/m
-0002e0c0: 6572 6765 2f54 7269 616c 2020 2020 2033  erge/Trial     3
-0002e0d0: 5f63 6c69 7070 6564 2e6d 7034 275d 0a23  _clipped.mp4'].#
-0002e0e0: 0a23 2076 6964 656f 5f70 6174 6873 203d  .# video_paths =
-0002e0f0: 205b 272f 5573 6572 732f 7369 6d6f 6e2f   ['/Users/simon/
-0002e100: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0002e110: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0002e120: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
-0002e130: 726f 6a65 6374 5f66 6f6c 6465 722f 7669  roject_folder/vi
-0002e140: 6465 6f73 2f54 7269 616c 2020 2020 3130  deos/Trial    10
-0002e150: 2e6d 7034 272c 0a23 2020 2020 2020 2020  .mp4',.#        
-0002e160: 2020 2020 2020 2020 272f 5573 6572 732f          '/Users/
-0002e170: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-0002e180: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-0002e190: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
-0002e1a0: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
-0002e1b0: 6465 722f 6d65 7267 652f 5472 6961 6c20  der/merge/Trial 
-0002e1c0: 2020 2031 305f 636c 6970 7065 645f 6761     10_clipped_ga
-0002e1d0: 6e74 742e 6d70 3427 2c0a 2320 2020 2020  ntt.mp4',.#     
-0002e1e0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
-0002e1f0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-0002e200: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-0002e210: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
-0002e220: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
-0002e230: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
-0002e240: 616c 2020 2020 3130 5f63 6c69 7070 6564  al    10_clipped
-0002e250: 5f6c 696e 652e 6d70 3427 2c0a 2320 2020  _line.mp4',.#   
-0002e260: 2020 2020 2020 2020 2020 2020 2027 2f55               '/U
-0002e270: 7365 7273 2f73 696d 6f6e 2f44 6573 6b74  sers/simon/Deskt
-0002e280: 6f70 2f65 6e76 732f 7369 6d62 612f 7472  op/envs/simba/tr
-0002e290: 6f75 626c 6573 686f 6f74 696e 672f 6265  oubleshooting/be
-0002e2a0: 6570 626f 6f70 3137 342f 7072 6f6a 6563  epboop174/projec
-0002e2b0: 745f 666f 6c64 6572 2f6d 6572 6765 2f54  t_folder/merge/T
-0002e2c0: 7269 616c 2020 2020 2033 5f63 6c69 7070  rial     3_clipp
-0002e2d0: 6564 2e6d 7034 275d 0a23 0a23 2073 6176  ed.mp4'].#.# sav
-0002e2e0: 655f 7061 7468 203d 2027 2f55 7365 7273  e_path = '/Users
-0002e2f0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-0002e300: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-0002e310: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-0002e320: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-0002e330: 6c64 6572 2f6d 6572 6765 2f6f 7574 2e6d  lder/merge/out.m
-0002e340: 7034 270a 0a23 0a23 2076 6964 656f 5f70  p4'..#.# video_p
-0002e350: 6174 6873 203d 205b 272f 5573 6572 732f  aths = ['/Users/
-0002e360: 7369 6d6f 6e2f 4465 736b 746f 702f 656e  simon/Desktop/en
-0002e370: 7673 2f73 696d 6261 2f74 726f 7562 6c65  vs/simba/trouble
-0002e380: 7368 6f6f 7469 6e67 2f62 6565 7062 6f6f  shooting/beepboo
-0002e390: 7031 3734 2f70 726f 6a65 6374 5f66 6f6c  p174/project_fol
-0002e3a0: 6465 722f 6672 616d 6573 2f6f 7574 7075  der/frames/outpu
-0002e3b0: 742f 6761 6e74 745f 706c 6f74 732f 5472  t/gantt_plots/Tr
-0002e3c0: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
-0002e3d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002e3e0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
-0002e3f0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-0002e400: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-0002e410: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-0002e420: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-0002e430: 656f 732f 5472 6961 6c20 2020 2031 302e  eos/Trial    10.
-0002e440: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
-0002e450: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
-0002e460: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
-0002e470: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
-0002e480: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
-0002e490: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
-0002e4a0: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
-0002e4b0: 2f6c 696e 655f 706c 6f74 2f54 7269 616c  /line_plot/Trial
-0002e4c0: 2020 2020 3130 2e6d 7034 272c 0a23 2020      10.mp4',.#  
-0002e4d0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-0002e4e0: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
-0002e4f0: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
-0002e500: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
-0002e510: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
-0002e520: 6374 5f66 6f6c 6465 722f 6672 616d 6573  ct_folder/frames
-0002e530: 2f6f 7574 7075 742f 6c69 6e65 5f70 6c6f  /output/line_plo
-0002e540: 742f 5472 6961 6c20 2020 2020 332e 6d70  t/Trial     3.mp
-0002e550: 3427 5d0a 2320 7361 7665 5f70 6174 6820  4'].# save_path 
-0002e560: 3d20 272f 5573 6572 732f 7369 6d6f 6e2f  = '/Users/simon/
-0002e570: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0002e580: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0002e590: 6e67 2f52 4154 5f4e 4f52 2f70 726f 6a65  ng/RAT_NOR/proje
-0002e5a0: 6374 5f66 6f6c 6465 722f 7669 6465 6f73  ct_folder/videos
-0002e5b0: 2f74 6573 742f 6e65 772f 626c 616e 6b5f  /test/new/blank_
-0002e5c0: 7465 7374 2e6d 7034 270a 0a23 2076 6964  test.mp4'..# vid
-0002e5d0: 656f 5f70 6174 6873 203d 205b 272f 5573  eo_paths = ['/Us
-0002e5e0: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0002e5f0: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0002e600: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
-0002e610: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
-0002e620: 5f66 6f6c 6465 722f 7669 6465 6f73 2f54  _folder/videos/T
-0002e630: 7269 616c 2020 2020 3130 2e6d 7034 272c  rial    10.mp4',
-0002e640: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-0002e650: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
-0002e660: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0002e670: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
-0002e680: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
-0002e690: 726f 6a65 6374 5f66 6f6c 6465 722f 6672  roject_folder/fr
-0002e6a0: 616d 6573 2f6f 7574 7075 742f 6c69 6e65  ames/output/line
-0002e6b0: 5f70 6c6f 742f 5472 6961 6c20 2020 2031  _plot/Trial    1
-0002e6c0: 302e 6d70 3427 2c0a 2320 2020 2020 2020  0.mp4',.#       
-0002e6d0: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
-0002e6e0: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-0002e6f0: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-0002e700: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-0002e710: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-0002e720: 6c64 6572 2f66 7261 6d65 732f 6f75 7470  lder/frames/outp
-0002e730: 7574 2f6c 696e 655f 706c 6f74 2f54 7269  ut/line_plot/Tri
-0002e740: 616c 2020 2020 2033 2e6d 7034 275d 0a0a  al     3.mp4']..
-0002e750: 2320 6d69 7865 645f 6d6f 7361 6963 5f63  # mixed_mosaic_c
-0002e760: 6f6e 6361 7465 6e61 746f 7228 7669 6465  oncatenator(vide
-0002e770: 6f5f 7061 7468 733d 7669 6465 6f5f 7061  o_paths=video_pa
-0002e780: 7468 732c 2073 6176 655f 7061 7468 3d73  ths, save_path=s
-0002e790: 6176 655f 7061 7468 2c20 6770 753d 4661  ave_path, gpu=Fa
-0002e7a0: 6c73 652c 2076 6572 626f 7365 3d54 7275  lse, verbose=Tru
-0002e7b0: 6529 0a                                  e).
+0002dce0: 2062 675f 6672 6d3d 6267 5f66 726d 2c0a   bg_frm=bg_frm,.
+0002dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dd10: 2020 2020 2020 6267 5f63 6c72 3d62 675f        bg_clr=bg_
+0002dd20: 636f 6c6f 722c 0a20 2020 2020 2020 2020  color,.         
+0002dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dd40: 2020 2020 2020 2020 2020 2020 2066 675f               fg_
+0002dd50: 636c 723d 6667 5f63 6f6c 6f72 2c0a 2020  clr=fg_color,.  
+0002dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dd80: 2020 2020 7669 6465 6f5f 6d65 7461 5f64      video_meta_d
+0002dd90: 6174 613d 7669 6465 6f5f 6d65 7461 5f64  ata=video_meta_d
+0002dda0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+0002ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ddc0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0002ddd0: 6469 723d 7465 6d70 5f64 6972 290a 2020  dir=temp_dir).  
+0002dde0: 2020 2020 2020 666f 7220 636e 742c 2072        for cnt, r
+0002ddf0: 6573 756c 7420 696e 2065 6e75 6d65 7261  esult in enumera
+0002de00: 7465 2870 6f6f 6c2e 696d 6170 2863 6f6e  te(pool.imap(con
+0002de10: 7374 616e 7473 2c20 6672 6d5f 6461 7461  stants, frm_data
+0002de20: 2c20 6368 756e 6b73 697a 653d 3129 293a  , chunksize=1)):
+0002de30: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0002de40: 6e74 2866 2746 7261 6d65 2062 6174 6368  nt(f'Frame batch
+0002de50: 207b 7265 7375 6c74 2b31 7d20 636f 6d70   {result+1} comp
+0002de60: 6c65 7465 642e 2e2e 2729 0a20 2020 2020  leted...').     
+0002de70: 2020 2070 6f6f 6c2e 7465 726d 696e 6174     pool.terminat
+0002de80: 6528 290a 2020 2020 2020 2020 706f 6f6c  e().        pool
+0002de90: 2e6a 6f69 6e28 290a 0a20 2020 2070 7269  .join()..    pri
+0002dea0: 6e74 2866 224a 6f69 6e69 6e67 207b 7669  nt(f"Joining {vi
+0002deb0: 6465 6f5f 6e61 6d65 7d20 6d75 6c74 6970  deo_name} multip
+0002dec0: 726f 6365 7373 6564 2076 6964 656f 2e2e  rocessed video..
+0002ded0: 2e22 290a 2020 2020 636f 6e63 6174 656e  .").    concaten
+0002dee0: 6174 655f 7669 6465 6f73 5f69 6e5f 666f  ate_videos_in_fo
+0002def0: 6c64 6572 2869 6e5f 666f 6c64 6572 3d74  lder(in_folder=t
+0002df00: 656d 705f 6469 722c 2073 6176 655f 7061  emp_dir, save_pa
+0002df10: 7468 3d73 6176 655f 7061 7468 2c20 7669  th=save_path, vi
+0002df20: 6465 6f5f 666f 726d 6174 3d65 7874 5b31  deo_format=ext[1
+0002df30: 3a5d 2c20 7265 6d6f 7665 5f73 706c 6974  :], remove_split
+0002df40: 733d 5472 7565 290a 2020 2020 7469 6d65  s=True).    time
+0002df50: 722e 7374 6f70 5f74 696d 6572 2829 0a20  r.stop_timer(). 
+0002df60: 2020 2073 7464 6f75 745f 7375 6363 6573     stdout_succes
+0002df70: 7328 6d73 673d 6627 5669 6465 6f20 7361  s(msg=f'Video sa
+0002df80: 7665 6420 6174 207b 7361 7665 5f70 6174  ved at {save_pat
+0002df90: 687d 272c 2065 6c61 7073 6564 5f74 696d  h}', elapsed_tim
+0002dfa0: 653d 7469 6d65 722e 656c 6170 7365 645f  e=timer.elapsed_
+0002dfb0: 7469 6d65 5f73 7472 290a 0a0a 6465 6620  time_str)...def 
+0002dfc0: 7375 7065 7269 6d70 6f73 655f 7669 6465  superimpose_vide
+0002dfd0: 6f5f 6e61 6d65 7328 7669 6465 6f5f 7061  o_names(video_pa
+0002dfe0: 7468 3a20 556e 696f 6e5b 7374 722c 206f  th: Union[str, o
+0002dff0: 732e 5061 7468 4c69 6b65 5d2c 0a20 2020  s.PathLike],.   
+0002e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e010: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
+0002e020: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
+0002e030: 5d20 3d20 3330 2c0a 2020 2020 2020 2020  ] = 30,.        
+0002e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e050: 2020 2020 666f 6e74 5f63 6f6c 6f72 3a20      font_color: 
+0002e060: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0002e070: 2777 6869 7465 272c 0a20 2020 2020 2020  'white',.       
+0002e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e090: 2020 2020 2066 6f6e 745f 626f 7264 6572       font_border
+0002e0a0: 5f63 6f6c 6f72 3a20 4f70 7469 6f6e 616c  _color: Optional
+0002e0b0: 5b73 7472 5d20 3d20 2762 6c61 636b 272c  [str] = 'black',
+0002e0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002e0d0: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+0002e0e0: 745f 626f 7264 6572 5f77 6964 7468 3a20  t_border_width: 
+0002e0f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0002e100: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+0002e110: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002e120: 6f73 6974 696f 6e3a 204f 7074 696f 6e61  osition: Optiona
+0002e130: 6c5b 4c69 7465 7261 6c5b 2774 6f70 5f6c  l[Literal['top_l
+0002e140: 6566 7427 2c20 2774 6f70 5f72 6967 6874  eft', 'top_right
+0002e150: 272c 2027 626f 7474 6f6d 5f6c 6566 7427  ', 'bottom_left'
+0002e160: 2c20 2762 6f74 746f 6d5f 7269 6768 7427  , 'bottom_right'
+0002e170: 2c20 276d 6964 646c 655f 746f 7027 2c20  , 'middle_top', 
+0002e180: 276d 6964 646c 655f 626f 7474 6f6d 275d  'middle_bottom']
+0002e190: 5d20 3d20 2774 6f70 5f6c 6566 7427 2c0a  ] = 'top_left',.
+0002e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e1b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0002e1c0: 5f64 6972 3a20 4f70 7469 6f6e 616c 5b55  _dir: Optional[U
+0002e1d0: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
+0002e1e0: 684c 696b 655d 5d20 3d20 4e6f 6e65 2920  hLike]] = None) 
+0002e1f0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+0002e200: 0a20 2020 2053 7570 6572 696d 706f 7365  .    Superimpose
+0002e210: 7320 7468 6520 7669 6465 6f20 6e61 6d65  s the video name
+0002e220: 206f 6e20 7468 6520 6769 7665 6e20 7669   on the given vi
+0002e230: 6465 6f20 6669 6c65 2873 2920 616e 6420  deo file(s) and 
+0002e240: 7361 7665 7320 7468 6520 6d6f 6469 6669  saves the modifi
+0002e250: 6564 2076 6964 656f 2873 292e 0a0a 2020  ed video(s)...  
+0002e260: 2020 2e2e 2076 6964 656f 3a3a 205f 7374    .. video:: _st
+0002e270: 6174 6963 2f69 6d67 2f73 7570 6572 696d  atic/img/superim
+0002e280: 706f 7365 5f65 6c61 7073 6564 5f74 696d  pose_elapsed_tim
+0002e290: 652e 7765 626d 0a20 2020 2020 2020 3a77  e.webm.       :w
+0002e2a0: 6964 7468 3a20 3930 300a 2020 2020 2020  idth: 900.      
+0002e2b0: 203a 6c6f 6f70 3a0a 0a20 2020 203a 7061   :loop:..    :pa
+0002e2c0: 7261 6d20 556e 696f 6e5b 7374 722c 206f  ram Union[str, o
+0002e2d0: 732e 5061 7468 4c69 6b65 5d20 7669 6465  s.PathLike] vide
+0002e2e0: 6f5f 7061 7468 3a20 5061 7468 2074 6f20  o_path: Path to 
+0002e2f0: 7468 6520 696e 7075 7420 7669 6465 6f20  the input video 
+0002e300: 6669 6c65 206f 7220 6469 7265 6374 6f72  file or director
+0002e310: 7920 636f 6e74 6169 6e69 6e67 2076 6964  y containing vid
+0002e320: 656f 2066 696c 6573 2e0a 2020 2020 3a70  eo files..    :p
+0002e330: 6172 616d 204f 7074 696f 6e61 6c5b 696e  aram Optional[in
+0002e340: 745d 2066 6f6e 745f 7369 7a65 3a20 466f  t] font_size: Fo
+0002e350: 6e74 2073 697a 6520 666f 7220 7468 6520  nt size for the 
+0002e360: 7669 6465 6f20 6e61 6d65 2074 6578 742e  video name text.
+0002e370: 2044 6566 6175 6c74 2033 302e 0a20 2020   Default 30..   
+0002e380: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+0002e390: 5b73 7472 5d20 666f 6e74 5f63 6f6c 6f72  [str] font_color
+0002e3a0: 3a20 2046 6f6e 7420 636f 6c6f 7220 666f  :  Font color fo
+0002e3b0: 7220 7468 6520 7669 6465 6f20 6e61 6d65  r the video name
+0002e3c0: 2074 6578 742e 2044 6566 6175 6c74 2077   text. Default w
+0002e3d0: 6869 7465 0a20 2020 203a 7061 7261 6d20  hite.    :param 
+0002e3e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 666f  Optional[str] fo
+0002e3f0: 6e74 5f62 6f72 6465 725f 636f 6c6f 723a  nt_border_color:
+0002e400: 2046 6f6e 7420 626f 7264 6572 2063 6f6c   Font border col
+0002e410: 6f72 2066 6f72 2074 6865 2076 6964 656f  or for the video
+0002e420: 206e 616d 6520 7465 7874 2e20 4465 6661   name text. Defa
+0002e430: 756c 7420 626c 6163 6b2e 0a20 2020 203a  ult black..    :
+0002e440: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
+0002e450: 6e74 5d20 666f 6e74 5f62 6f72 6465 725f  nt] font_border_
+0002e460: 7769 6474 683a 2046 6f6e 7420 626f 7264  width: Font bord
+0002e470: 6572 2077 6964 7468 2066 6f72 2074 6865  er width for the
+0002e480: 2076 6964 656f 206e 616d 6520 7465 7874   video name text
+0002e490: 2069 6e20 7069 7865 6c73 2e20 4465 6661   in pixels. Defa
+0002e4a0: 756c 7420 322e 0a20 2020 203a 7061 7261  ult 2..    :para
+0002e4b0: 6d20 4f70 7469 6f6e 616c 5b4c 6974 6572  m Optional[Liter
+0002e4c0: 616c 5b27 746f 705f 6c65 6674 272c 2027  al['top_left', '
+0002e4d0: 746f 705f 7269 6768 7427 2c20 2762 6f74  top_right', 'bot
+0002e4e0: 746f 6d5f 6c65 6674 272c 2027 626f 7474  tom_left', 'bott
+0002e4f0: 6f6d 5f72 6967 6874 272c 2027 746f 705f  om_right', 'top_
+0002e500: 6d69 6464 6c65 272c 2027 626f 7474 6f6d  middle', 'bottom
+0002e510: 5f6d 6964 646c 6527 5d5d 2070 6f73 6974  _middle']] posit
+0002e520: 696f 6e3a 2050 6f73 6974 696f 6e20 7768  ion: Position wh
+0002e530: 6572 6520 7468 6520 7669 6465 6f20 6e61  ere the video na
+0002e540: 6d65 2077 696c 6c20 6265 2073 7570 6572  me will be super
+0002e550: 696d 706f 7365 642e 2044 6566 6175 6c74  imposed. Default
+0002e560: 2060 6074 6f70 5f6c 6566 7460 602e 0a20   ``top_left``.. 
+0002e570: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
+0002e580: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+0002e590: 2e50 6174 684c 696b 655d 5d20 7361 7665  .PathLike]] save
+0002e5a0: 5f64 6972 3a20 4469 7265 6374 6f72 7920  _dir: Directory 
+0002e5b0: 7768 6572 6520 7468 6520 6d6f 6469 6669  where the modifi
+0002e5c0: 6564 2076 6964 656f 2873 2920 7769 6c6c  ed video(s) will
+0002e5d0: 2062 6520 7361 7665 642e 2049 6620 6e6f   be saved. If no
+0002e5e0: 7420 7072 6f76 6964 6564 2c20 7468 6520  t provided, the 
+0002e5f0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+0002e600: 2069 6e70 7574 2076 6964 656f 2873 2920   input video(s) 
+0002e610: 7769 6c6c 2062 6520 7573 6564 2e0a 2020  will be used..  
+0002e620: 2020 3a72 6574 7572 6e3a 204e 6f6e 650a    :return: None.
+0002e630: 0a20 2020 203a 6578 616d 706c 653a 0a20  .    :example:. 
+0002e640: 2020 203e 3e3e 2073 7570 6572 696d 706f     >>> superimpo
+0002e650: 7365 5f76 6964 656f 5f6e 616d 6573 2876  se_video_names(v
+0002e660: 6964 656f 5f70 6174 683d 272f 5573 6572  ideo_path='/User
+0002e670: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+0002e680: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+0002e690: 6c65 7368 6f6f 7469 6e67 2f6d 6f75 7365  leshooting/mouse
+0002e6a0: 5f6f 7065 6e5f 6669 656c 642f 7072 6f6a  _open_field/proj
+0002e6b0: 6563 745f 666f 6c64 6572 2f76 6964 656f  ect_folder/video
+0002e6c0: 732f 7465 7374 5f34 2f31 2e6d 7034 272c  s/test_4/1.mp4',
+0002e6d0: 2070 6f73 6974 696f 6e3d 276d 6964 646c   position='middl
+0002e6e0: 655f 746f 7027 2c20 666f 6e74 5f63 6f6c  e_top', font_col
+0002e6f0: 6f72 3d27 626c 6163 6b27 2c20 666f 6e74  or='black', font
+0002e700: 5f62 6f72 6465 725f 636f 6c6f 723d 2770  _border_color='p
+0002e710: 696e 6b27 2c20 666f 6e74 5f62 6f72 6465  ink', font_borde
+0002e720: 725f 7769 6474 683d 352c 2066 6f6e 745f  r_width=5, font_
+0002e730: 7369 7a65 3d33 3029 0a20 2020 2022 2222  size=30).    """
+0002e740: 0a0a 2020 2020 6368 6563 6b5f 6666 6d70  ..    check_ffmp
+0002e750: 6567 5f61 7661 696c 6162 6c65 2872 6169  eg_available(rai
+0002e760: 7365 5f65 7272 6f72 3d54 7275 6529 0a20  se_error=True). 
+0002e770: 2020 2074 696d 6572 203d 2053 696d 6261     timer = Simba
+0002e780: 5469 6d65 7228 7374 6172 743d 5472 7565  Timer(start=True
+0002e790: 290a 2020 2020 504f 5349 5449 4f4e 5320  ).    POSITIONS 
+0002e7a0: 3d20 5b27 746f 705f 6c65 6674 272c 2027  = ['top_left', '
+0002e7b0: 746f 705f 7269 6768 7427 2c20 2762 6f74  top_right', 'bot
+0002e7c0: 746f 6d5f 6c65 6674 272c 2027 626f 7474  tom_left', 'bott
+0002e7d0: 6f6d 5f72 6967 6874 272c 2027 746f 705f  om_right', 'top_
+0002e7e0: 6d69 6464 6c65 272c 2027 626f 7474 6f6d  middle', 'bottom
+0002e7f0: 5f6d 6964 646c 6527 5d0a 2020 2020 6368  _middle'].    ch
+0002e800: 6563 6b5f 7374 7228 6e61 6d65 3d66 277b  eck_str(name=f'{
+0002e810: 7375 7065 7269 6d70 6f73 655f 7669 6465  superimpose_vide
+0002e820: 6f5f 6e61 6d65 732e 5f5f 6e61 6d65 5f5f  o_names.__name__
+0002e830: 7d20 706f 7369 7469 6f6e 272c 2076 616c  } position', val
+0002e840: 7565 3d70 6f73 6974 696f 6e2c 206f 7074  ue=position, opt
+0002e850: 696f 6e73 3d50 4f53 4954 494f 4e53 290a  ions=POSITIONS).
+0002e860: 2020 2020 6368 6563 6b5f 696e 7428 6e61      check_int(na
+0002e870: 6d65 3d66 277b 7375 7065 7269 6d70 6f73  me=f'{superimpos
+0002e880: 655f 7669 6465 6f5f 6e61 6d65 732e 5f5f  e_video_names.__
+0002e890: 6e61 6d65 5f5f 7d20 666f 6e74 5f73 697a  name__} font_siz
+0002e8a0: 6527 2c20 7661 6c75 653d 666f 6e74 5f73  e', value=font_s
+0002e8b0: 697a 652c 206d 696e 5f76 616c 7565 3d31  ize, min_value=1
+0002e8c0: 290a 2020 2020 6368 6563 6b5f 696e 7428  ).    check_int(
+0002e8d0: 6e61 6d65 3d66 277b 7375 7065 7269 6d70  name=f'{superimp
+0002e8e0: 6f73 655f 7669 6465 6f5f 6e61 6d65 732e  ose_video_names.
+0002e8f0: 5f5f 6e61 6d65 5f5f 7d20 666f 6e74 5f62  __name__} font_b
+0002e900: 6f72 6465 725f 7769 6474 6827 2c20 7661  order_width', va
+0002e910: 6c75 653d 666f 6e74 5f62 6f72 6465 725f  lue=font_border_
+0002e920: 7769 6474 682c 206d 696e 5f76 616c 7565  width, min_value
+0002e930: 3d31 290a 2020 2020 666f 6e74 5f63 6f6c  =1).    font_col
+0002e940: 6f72 203d 2027 272e 6a6f 696e 2866 696c  or = ''.join(fil
+0002e950: 7465 7228 7374 722e 6973 616c 6e75 6d2c  ter(str.isalnum,
+0002e960: 2066 6f6e 745f 636f 6c6f 7229 292e 6c6f   font_color)).lo
+0002e970: 7765 7228 290a 2020 2020 666f 6e74 5f62  wer().    font_b
+0002e980: 6f72 6465 725f 636f 6c6f 7220 3d20 2727  order_color = ''
+0002e990: 2e6a 6f69 6e28 6669 6c74 6572 2873 7472  .join(filter(str
+0002e9a0: 2e69 7361 6c6e 756d 2c20 666f 6e74 5f62  .isalnum, font_b
+0002e9b0: 6f72 6465 725f 636f 6c6f 7229 292e 6c6f  order_color)).lo
+0002e9c0: 7765 7228 290a 2020 2020 6966 206f 732e  wer().    if os.
+0002e9d0: 7061 7468 2e69 7366 696c 6528 7669 6465  path.isfile(vide
+0002e9e0: 6f5f 7061 7468 293a 0a20 2020 2020 2020  o_path):.       
+0002e9f0: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
+0002ea00: 7669 6465 6f5f 7061 7468 5d0a 2020 2020  video_path].    
+0002ea10: 656c 6966 206f 732e 7061 7468 2e69 7364  elif os.path.isd
+0002ea20: 6972 2876 6964 656f 5f70 6174 6829 3a0a  ir(video_path):.
+0002ea30: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
+0002ea40: 7468 7320 3d20 6c69 7374 2866 696e 645f  ths = list(find_
+0002ea50: 616c 6c5f 7669 6465 6f73 5f69 6e5f 6469  all_videos_in_di
+0002ea60: 7265 6374 6f72 7928 6469 7265 6374 6f72  rectory(director
+0002ea70: 793d 7669 6465 6f5f 7061 7468 2c20 6173  y=video_path, as
+0002ea80: 5f64 6963 743d 5472 7565 2c20 7261 6973  _dict=True, rais
+0002ea90: 655f 6572 726f 723d 5472 7565 292e 7661  e_error=True).va
+0002eaa0: 6c75 6573 2829 290a 2020 2020 656c 7365  lues()).    else
+0002eab0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+0002eac0: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
+0002ead0: 7228 6d73 673d 6627 7b76 6964 656f 5f70  r(msg=f'{video_p
+0002eae0: 6174 687d 2069 7320 6e6f 7420 6120 7661  ath} is not a va
+0002eaf0: 6c69 6420 6669 6c65 2070 6174 6820 6f72  lid file path or
+0002eb00: 2061 2076 616c 6964 2064 6972 6563 746f   a valid directo
+0002eb10: 7279 2070 6174 6827 2c20 736f 7572 6365  ry path', source
+0002eb20: 3d73 7570 6572 696d 706f 7365 5f76 6964  =superimpose_vid
+0002eb30: 656f 5f6e 616d 6573 2e5f 5f6e 616d 655f  eo_names.__name_
+0002eb40: 5f29 0a20 2020 2069 6620 7361 7665 5f64  _).    if save_d
+0002eb50: 6972 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ir is not None:.
+0002eb60: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
+0002eb70: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
+0002eb80: 6972 3d73 6176 655f 6469 7229 0a20 2020  ir=save_dir).   
+0002eb90: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+0002eba0: 6176 655f 6469 7220 3d20 6f73 2e70 6174  ave_dir = os.pat
+0002ebb0: 682e 6469 726e 616d 6528 7669 6465 6f5f  h.dirname(video_
+0002ebc0: 7061 7468 735b 305d 290a 2020 2020 666f  paths[0]).    fo
+0002ebd0: 7220 6669 6c65 5f63 6e74 2c20 7669 6465  r file_cnt, vide
+0002ebe0: 6f5f 7061 7468 2069 6e20 656e 756d 6572  o_path in enumer
+0002ebf0: 6174 6528 7669 6465 6f5f 7061 7468 7329  ate(video_paths)
+0002ec00: 3a0a 2020 2020 2020 2020 5f2c 2076 6964  :.        _, vid
+0002ec10: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
+0002ec20: 6574 5f66 6e5f 6578 7428 7669 6465 6f5f  et_fn_ext(video_
+0002ec30: 7061 7468 290a 2020 2020 2020 2020 7072  path).        pr
+0002ec40: 696e 7428 6627 5375 7065 7269 6d70 6f73  int(f'Superimpos
+0002ec50: 696e 6720 7669 6465 6f20 6e61 6d65 206f  ing video name o
+0002ec60: 6e20 7b76 6964 656f 5f6e 616d 657d 2028  n {video_name} (
+0002ec70: 5669 6465 6f20 7b66 696c 655f 636e 7420  Video {file_cnt 
+0002ec80: 2b20 317d 2f7b 6c65 6e28 7669 6465 6f5f  + 1}/{len(video_
+0002ec90: 7061 7468 7329 7d29 2e2e 2e27 290a 2020  paths)})...').  
+0002eca0: 2020 2020 2020 7361 7665 5f70 6174 6820        save_path 
+0002ecb0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+0002ecc0: 6176 655f 6469 722c 2066 277b 7669 6465  ave_dir, f'{vide
+0002ecd0: 6f5f 6e61 6d65 7d5f 7669 6465 6f5f 6e61  o_name}_video_na
+0002ece0: 6d65 5f73 7570 6572 696d 706f 7365 647b  me_superimposed{
+0002ecf0: 6578 747d 2729 0a20 2020 2020 2020 2069  ext}').        i
+0002ed00: 6620 706f 7369 7469 6f6e 203d 3d20 504f  f position == PO
+0002ed10: 5349 5449 4f4e 535b 305d 3a0a 2020 2020  SITIONS[0]:.    
+0002ed20: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
+0002ed30: 6666 6d70 6567 202d 6920 277b 7669 6465  ffmpeg -i '{vide
+0002ed40: 6f5f 7061 7468 7d27 202d 7666 205c 2264  o_path}' -vf \"d
+0002ed50: 7261 7774 6578 743d 666f 6e74 6669 6c65  rawtext=fontfile
+0002ed60: 3d41 7269 616c 2e74 7466 3a74 6578 743d  =Arial.ttf:text=
+0002ed70: 7b76 6964 656f 5f6e 616d 657d 3a78 3d35  {video_name}:x=5
+0002ed80: 3a79 3d35 3a66 6f6e 7473 697a 653d 7b66  :y=5:fontsize={f
+0002ed90: 6f6e 745f 7369 7a65 7d3a 666f 6e74 636f  ont_size}:fontco
+0002eda0: 6c6f 723d 7b66 6f6e 745f 636f 6c6f 727d  lor={font_color}
+0002edb0: 3a62 6f72 6465 7277 3d7b 666f 6e74 5f62  :borderw={font_b
+0002edc0: 6f72 6465 725f 7769 6474 687d 3a62 6f72  order_width}:bor
+0002edd0: 6465 7263 6f6c 6f72 3d7b 666f 6e74 5f62  dercolor={font_b
+0002ede0: 6f72 6465 725f 636f 6c6f 727d 5c22 202d  order_color}\" -
+0002edf0: 633a 6120 636f 7079 2027 7b73 6176 655f  c:a copy '{save_
+0002ee00: 7061 7468 7d27 202d 6c6f 676c 6576 656c  path}' -loglevel
+0002ee10: 2065 7272 6f72 202d 7374 6174 7320 2d68   error -stats -h
+0002ee20: 6964 655f 6261 6e6e 6572 202d 7922 0a20  ide_banner -y". 
+0002ee30: 2020 2020 2020 2065 6c69 6620 706f 7369         elif posi
+0002ee40: 7469 6f6e 203d 3d20 504f 5349 5449 4f4e  tion == POSITION
+0002ee50: 535b 315d 3a0a 2020 2020 2020 2020 2020  S[1]:.          
+0002ee60: 2020 636d 6420 3d20 6622 6666 6d70 6567    cmd = f"ffmpeg
+0002ee70: 202d 6920 277b 7669 6465 6f5f 7061 7468   -i '{video_path
+0002ee80: 7d27 202d 7666 205c 2264 7261 7774 6578  }' -vf \"drawtex
+0002ee90: 743d 666f 6e74 6669 6c65 3d41 7269 616c  t=fontfile=Arial
+0002eea0: 2e74 7466 3a74 6578 743d 7b76 6964 656f  .ttf:text={video
+0002eeb0: 5f6e 616d 657d 3a78 3d28 772d 7477 2d35  _name}:x=(w-tw-5
+0002eec0: 293a 793d 353a 666f 6e74 7369 7a65 3d7b  ):y=5:fontsize={
+0002eed0: 666f 6e74 5f73 697a 657d 3a66 6f6e 7463  font_size}:fontc
+0002eee0: 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c 6f72  olor={font_color
+0002eef0: 7d3a 626f 7264 6572 773d 7b66 6f6e 745f  }:borderw={font_
+0002ef00: 626f 7264 6572 5f77 6964 7468 7d3a 626f  border_width}:bo
+0002ef10: 7264 6572 636f 6c6f 723d 7b66 6f6e 745f  rdercolor={font_
+0002ef20: 626f 7264 6572 5f63 6f6c 6f72 7d5c 2220  border_color}\" 
+0002ef30: 2d63 3a61 2063 6f70 7920 277b 7361 7665  -c:a copy '{save
+0002ef40: 5f70 6174 687d 2720 2d6c 6f67 6c65 7665  _path}' -logleve
+0002ef50: 6c20 6572 726f 7220 2d73 7461 7473 202d  l error -stats -
+0002ef60: 6869 6465 5f62 616e 6e65 7220 2d79 220a  hide_banner -y".
+0002ef70: 2020 2020 2020 2020 656c 6966 2070 6f73          elif pos
+0002ef80: 6974 696f 6e20 3d3d 2050 4f53 4954 494f  ition == POSITIO
+0002ef90: 4e53 5b32 5d3a 0a20 2020 2020 2020 2020  NS[2]:.         
+0002efa0: 2020 2063 6d64 203d 2066 2266 666d 7065     cmd = f"ffmpe
+0002efb0: 6720 2d69 2027 7b76 6964 656f 5f70 6174  g -i '{video_pat
+0002efc0: 687d 2720 2d76 6620 5c22 6472 6177 7465  h}' -vf \"drawte
+0002efd0: 7874 3d66 6f6e 7466 696c 653d 4172 6961  xt=fontfile=Aria
+0002efe0: 6c2e 7474 663a 7465 7874 3d7b 7669 6465  l.ttf:text={vide
+0002eff0: 6f5f 6e61 6d65 7d3a 783d 353a 793d 2868  o_name}:x=5:y=(h
+0002f000: 2d74 682d 3529 3a66 6f6e 7473 697a 653d  -th-5):fontsize=
+0002f010: 7b66 6f6e 745f 7369 7a65 7d3a 666f 6e74  {font_size}:font
+0002f020: 636f 6c6f 723d 7b66 6f6e 745f 636f 6c6f  color={font_colo
+0002f030: 727d 3a62 6f72 6465 7277 3d7b 666f 6e74  r}:borderw={font
+0002f040: 5f62 6f72 6465 725f 7769 6474 687d 3a62  _border_width}:b
+0002f050: 6f72 6465 7263 6f6c 6f72 3d7b 666f 6e74  ordercolor={font
+0002f060: 5f62 6f72 6465 725f 636f 6c6f 727d 5c22  _border_color}\"
+0002f070: 202d 633a 6120 636f 7079 2027 7b73 6176   -c:a copy '{sav
+0002f080: 655f 7061 7468 7d27 202d 6c6f 676c 6576  e_path}' -loglev
+0002f090: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
+0002f0a0: 2d68 6964 655f 6261 6e6e 6572 202d 7922  -hide_banner -y"
+0002f0b0: 0a20 2020 2020 2020 2065 6c69 6620 706f  .        elif po
+0002f0c0: 7369 7469 6f6e 203d 3d20 504f 5349 5449  sition == POSITI
+0002f0d0: 4f4e 535b 335d 3a0a 2020 2020 2020 2020  ONS[3]:.        
+0002f0e0: 2020 2020 636d 6420 3d20 6622 6666 6d70      cmd = f"ffmp
+0002f0f0: 6567 202d 6920 277b 7669 6465 6f5f 7061  eg -i '{video_pa
+0002f100: 7468 7d27 202d 7666 205c 2264 7261 7774  th}' -vf \"drawt
+0002f110: 6578 743d 666f 6e74 6669 6c65 3d41 7269  ext=fontfile=Ari
+0002f120: 616c 2e74 7466 3a74 6578 743d 7b76 6964  al.ttf:text={vid
+0002f130: 656f 5f6e 616d 657d 3a78 3d28 772d 7477  eo_name}:x=(w-tw
+0002f140: 2d35 293a 793d 2868 2d74 682d 3529 3a66  -5):y=(h-th-5):f
+0002f150: 6f6e 7473 697a 653d 7b66 6f6e 745f 7369  ontsize={font_si
+0002f160: 7a65 7d3a 666f 6e74 636f 6c6f 723d 7b66  ze}:fontcolor={f
+0002f170: 6f6e 745f 636f 6c6f 727d 3a62 6f72 6465  ont_color}:borde
+0002f180: 7277 3d7b 666f 6e74 5f62 6f72 6465 725f  rw={font_border_
+0002f190: 7769 6474 687d 3a62 6f72 6465 7263 6f6c  width}:bordercol
+0002f1a0: 6f72 3d7b 666f 6e74 5f62 6f72 6465 725f  or={font_border_
+0002f1b0: 636f 6c6f 727d 5c22 202d 633a 6120 636f  color}\" -c:a co
+0002f1c0: 7079 2027 7b73 6176 655f 7061 7468 7d27  py '{save_path}'
+0002f1d0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
+0002f1e0: 202d 7374 6174 7320 2d68 6964 655f 6261   -stats -hide_ba
+0002f1f0: 6e6e 6572 202d 7922 0a20 2020 2020 2020  nner -y".       
+0002f200: 2065 6c69 6620 706f 7369 7469 6f6e 203d   elif position =
+0002f210: 3d20 504f 5349 5449 4f4e 535b 345d 3a0a  = POSITIONS[4]:.
+0002f220: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+0002f230: 3d20 6622 6666 6d70 6567 202d 6920 277b  = f"ffmpeg -i '{
+0002f240: 7669 6465 6f5f 7061 7468 7d27 202d 7666  video_path}' -vf
+0002f250: 205c 2264 7261 7774 6578 743d 666f 6e74   \"drawtext=font
+0002f260: 6669 6c65 3d41 7269 616c 2e74 7466 3a74  file=Arial.ttf:t
+0002f270: 6578 743d 7b76 6964 656f 5f6e 616d 657d  ext={video_name}
+0002f280: 3a78 3d28 772d 7477 292f 323a 793d 3130  :x=(w-tw)/2:y=10
+0002f290: 3a66 6f6e 7473 697a 653d 7b66 6f6e 745f  :fontsize={font_
+0002f2a0: 7369 7a65 7d3a 666f 6e74 636f 6c6f 723d  size}:fontcolor=
+0002f2b0: 7b66 6f6e 745f 636f 6c6f 727d 3a62 6f72  {font_color}:bor
+0002f2c0: 6465 7277 3d7b 666f 6e74 5f62 6f72 6465  derw={font_borde
+0002f2d0: 725f 7769 6474 687d 3a62 6f72 6465 7263  r_width}:borderc
+0002f2e0: 6f6c 6f72 3d7b 666f 6e74 5f62 6f72 6465  olor={font_borde
+0002f2f0: 725f 636f 6c6f 727d 5c22 202d 633a 6120  r_color}\" -c:a 
+0002f300: 636f 7079 2027 7b73 6176 655f 7061 7468  copy '{save_path
+0002f310: 7d27 202d 6c6f 676c 6576 656c 2065 7272  }' -loglevel err
+0002f320: 6f72 202d 7374 6174 7320 2d68 6964 655f  or -stats -hide_
+0002f330: 6261 6e6e 6572 202d 7922 0a20 2020 2020  banner -y".     
+0002f340: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002f350: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
+0002f360: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
+0002f370: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
+0002f380: 7465 7874 3d66 6f6e 7466 696c 653d 4172  text=fontfile=Ar
+0002f390: 6961 6c2e 7474 663a 7465 7874 3d7b 7669  ial.ttf:text={vi
+0002f3a0: 6465 6f5f 6e61 6d65 7d3a 783d 2877 2d74  deo_name}:x=(w-t
+0002f3b0: 7729 2f32 3a79 3d28 682d 7468 2d31 3029  w)/2:y=(h-th-10)
+0002f3c0: 3a66 6f6e 7473 697a 653d 7b66 6f6e 745f  :fontsize={font_
+0002f3d0: 7369 7a65 7d3a 666f 6e74 636f 6c6f 723d  size}:fontcolor=
+0002f3e0: 7b66 6f6e 745f 636f 6c6f 727d 3a62 6f72  {font_color}:bor
+0002f3f0: 6465 7277 3d7b 666f 6e74 5f62 6f72 6465  derw={font_borde
+0002f400: 725f 7769 6474 687d 3a62 6f72 6465 7263  r_width}:borderc
+0002f410: 6f6c 6f72 3d7b 666f 6e74 5f62 6f72 6465  olor={font_borde
+0002f420: 725f 636f 6c6f 727d 5c22 202d 633a 6120  r_color}\" -c:a 
+0002f430: 636f 7079 2027 7b73 6176 655f 7061 7468  copy '{save_path
+0002f440: 7d27 202d 6c6f 676c 6576 656c 2065 7272  }' -loglevel err
+0002f450: 6f72 202d 7374 6174 7320 2d68 6964 655f  or -stats -hide_
+0002f460: 6261 6e6e 6572 202d 7922 0a20 2020 2020  banner -y".     
+0002f470: 2020 2073 7562 7072 6f63 6573 732e 6361     subprocess.ca
+0002f480: 6c6c 2863 6d64 2c20 7368 656c 6c3d 5472  ll(cmd, shell=Tr
+0002f490: 7565 2c20 7374 646f 7574 3d73 7562 7072  ue, stdout=subpr
+0002f4a0: 6f63 6573 732e 5049 5045 290a 2020 2020  ocess.PIPE).    
+0002f4b0: 7469 6d65 722e 7374 6f70 5f74 696d 6572  timer.stop_timer
+0002f4c0: 2829 0a20 2020 2073 7464 6f75 745f 7375  ().    stdout_su
+0002f4d0: 6363 6573 7328 6d73 673d 6627 5375 7065  ccess(msg=f'Supe
+0002f4e0: 722d 696d 706f 7365 6420 7669 6465 6f20  r-imposed video 
+0002f4f0: 6e61 6d65 206f 6e20 7b6c 656e 2876 6964  name on {len(vid
+0002f500: 656f 5f70 6174 6873 297d 2076 6964 656f  eo_paths)} video
+0002f510: 2873 292c 2073 6176 6564 2069 6e20 7b73  (s), saved in {s
+0002f520: 6176 655f 6469 727d 272c 2065 6c61 7073  ave_dir}', elaps
+0002f530: 6564 5f74 696d 653d 7469 6d65 722e 656c  ed_time=timer.el
+0002f540: 6170 7365 645f 7469 6d65 5f73 7472 290a  apsed_time_str).
+0002f550: 0a64 6566 2073 7570 6572 696d 706f 7365  .def superimpose
+0002f560: 5f66 7265 6574 6578 7428 7669 6465 6f5f  _freetext(video_
+0002f570: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+0002f580: 206f 732e 5061 7468 4c69 6b65 5d2c 0a20   os.PathLike],. 
+0002f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f5a0: 2020 2020 2020 2020 7465 7874 3a20 7374          text: st
+0002f5b0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0002f5c0: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+0002f5d0: 5f73 697a 653a 204f 7074 696f 6e61 6c5b  _size: Optional[
+0002f5e0: 696e 745d 203d 2033 302c 0a20 2020 2020  int] = 30,.     
+0002f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f600: 2020 2020 666f 6e74 5f63 6f6c 6f72 3a20      font_color: 
+0002f610: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0002f620: 2777 6869 7465 272c 0a20 2020 2020 2020  'white',.       
+0002f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f640: 2020 666f 6e74 5f62 6f72 6465 725f 636f    font_border_co
+0002f650: 6c6f 723a 204f 7074 696f 6e61 6c5b 7374  lor: Optional[st
+0002f660: 725d 203d 2027 626c 6163 6b27 2c0a 2020  r] = 'black',.  
+0002f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f680: 2020 2020 2020 2066 6f6e 745f 626f 7264         font_bord
+0002f690: 6572 5f77 6964 7468 3a20 4f70 7469 6f6e  er_width: Option
+0002f6a0: 616c 5b69 6e74 5d20 3d20 322c 0a20 2020  al[int] = 2,.   
+0002f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f6c0: 2020 2020 2020 706f 7369 7469 6f6e 3a20        position: 
+0002f6d0: 4f70 7469 6f6e 616c 5b4c 6974 6572 616c  Optional[Literal
+0002f6e0: 5b27 746f 705f 6c65 6674 272c 2027 746f  ['top_left', 'to
+0002f6f0: 705f 7269 6768 7427 2c20 2762 6f74 746f  p_right', 'botto
+0002f700: 6d5f 6c65 6674 272c 2027 626f 7474 6f6d  m_left', 'bottom
+0002f710: 5f72 6967 6874 272c 2027 6d69 6464 6c65  _right', 'middle
+0002f720: 5f74 6f70 272c 2027 6d69 6464 6c65 5f62  _top', 'middle_b
+0002f730: 6f74 746f 6d27 5d5d 203d 2027 746f 705f  ottom']] = 'top_
+0002f740: 6c65 6674 272c 0a20 2020 2020 2020 2020  left',.         
+0002f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f760: 7361 7665 5f64 6972 3a20 4f70 7469 6f6e  save_dir: Option
+0002f770: 616c 5b55 6e69 6f6e 5b73 7472 2c20 6f73  al[Union[str, os
+0002f780: 2e50 6174 684c 696b 655d 5d20 3d20 4e6f  .PathLike]] = No
+0002f790: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
+0002f7a0: 2022 2222 0a20 2020 2053 7570 6572 696d   """.    Superim
+0002f7b0: 706f 7365 7320 7061 7373 6564 2074 6578  poses passed tex
+0002f7c0: 7420 6f6e 2074 6865 2067 6976 656e 2076  t on the given v
+0002f7d0: 6964 656f 2066 696c 6528 7329 2061 6e64  ideo file(s) and
+0002f7e0: 2073 6176 6573 2074 6865 206d 6f64 6966   saves the modif
+0002f7f0: 6965 6420 7669 6465 6f28 7329 2e0a 0a20  ied video(s)... 
+0002f800: 2020 202e 2e20 7669 6465 6f3a 3a20 5f73     .. video:: _s
+0002f810: 7461 7469 632f 696d 672f 7375 7065 7269  tatic/img/superi
+0002f820: 6d70 6f73 655f 656c 6170 7365 645f 7469  mpose_elapsed_ti
+0002f830: 6d65 2e77 6562 6d0a 2020 2020 2020 203a  me.webm.       :
+0002f840: 7769 6474 683a 2039 3030 0a20 2020 2020  width: 900.     
+0002f850: 2020 3a6c 6f6f 703a 0a0a 2020 2020 3a70    :loop:..    :p
+0002f860: 6172 616d 2055 6e69 6f6e 5b73 7472 2c20  aram Union[str, 
+0002f870: 6f73 2e50 6174 684c 696b 655d 2076 6964  os.PathLike] vid
+0002f880: 656f 5f70 6174 683a 2050 6174 6820 746f  eo_path: Path to
+0002f890: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
+0002f8a0: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
+0002f8b0: 7279 2063 6f6e 7461 696e 696e 6720 7669  ry containing vi
+0002f8c0: 6465 6f20 6669 6c65 732e 0a20 2020 203a  deo files..    :
+0002f8d0: 7061 7261 6d20 7374 7220 7465 7874 3a20  param str text: 
+0002f8e0: 5468 6520 7465 7874 2074 6f20 6f76 6572  The text to over
+0002f8f0: 6c61 7920 6f6e 2074 6865 2076 6964 656f  lay on the video
+0002f900: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
+0002f910: 6f6e 616c 5b69 6e74 5d20 666f 6e74 5f73  onal[int] font_s
+0002f920: 697a 653a 2046 6f6e 7420 7369 7a65 2066  ize: Font size f
+0002f930: 6f72 2074 6865 2074 6578 742e 2044 6566  or the text. Def
+0002f940: 6175 6c74 2033 302e 0a20 2020 203a 7061  ault 30..    :pa
+0002f950: 7261 6d20 4f70 7469 6f6e 616c 5b73 7472  ram Optional[str
+0002f960: 5d20 666f 6e74 5f63 6f6c 6f72 3a20 2046  ] font_color:  F
+0002f970: 6f6e 7420 636f 6c6f 7220 666f 7220 7465  ont color for te
+0002f980: 7874 2e20 4465 6661 756c 7420 7768 6974  xt. Default whit
+0002f990: 650a 2020 2020 3a70 6172 616d 204f 7074  e.    :param Opt
+0002f9a0: 696f 6e61 6c5b 7374 725d 2066 6f6e 745f  ional[str] font_
+0002f9b0: 626f 7264 6572 5f63 6f6c 6f72 3a20 466f  border_color: Fo
+0002f9c0: 6e74 2062 6f72 6465 7220 636f 6c6f 7220  nt border color 
+0002f9d0: 666f 7220 7468 6520 7465 7874 2e20 4465  for the text. De
+0002f9e0: 6661 756c 7420 626c 6163 6b2e 0a20 2020  fault black..   
+0002f9f0: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
+0002fa00: 5b69 6e74 5d20 666f 6e74 5f62 6f72 6465  [int] font_borde
+0002fa10: 725f 7769 6474 683a 2046 6f6e 7420 626f  r_width: Font bo
+0002fa20: 7264 6572 2077 6964 7468 2066 6f72 2074  rder width for t
+0002fa30: 6865 2074 6578 7420 696e 2070 6978 656c  he text in pixel
+0002fa40: 732e 2044 6566 6175 6c74 2032 2e0a 2020  s. Default 2..  
+0002fa50: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+0002fa60: 6c5b 4c69 7465 7261 6c5b 2774 6f70 5f6c  l[Literal['top_l
+0002fa70: 6566 7427 2c20 2774 6f70 5f72 6967 6874  eft', 'top_right
+0002fa80: 272c 2027 626f 7474 6f6d 5f6c 6566 7427  ', 'bottom_left'
+0002fa90: 2c20 2762 6f74 746f 6d5f 7269 6768 7427  , 'bottom_right'
+0002faa0: 2c20 2774 6f70 5f6d 6964 646c 6527 2c20  , 'top_middle', 
+0002fab0: 2762 6f74 746f 6d5f 6d69 6464 6c65 275d  'bottom_middle']
+0002fac0: 5d20 706f 7369 7469 6f6e 3a20 506f 7369  ] position: Posi
+0002fad0: 7469 6f6e 2077 6865 7265 2074 6865 2074  tion where the t
+0002fae0: 6578 7420 7769 6c6c 2062 6520 7375 7065  ext will be supe
+0002faf0: 7269 6d70 6f73 6564 2e20 4465 6661 756c  rimposed. Defaul
+0002fb00: 7420 6060 746f 705f 6c65 6674 6060 2e0a  t ``top_left``..
+0002fb10: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+0002fb20: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+0002fb30: 732e 5061 7468 4c69 6b65 5d5d 2073 6176  s.PathLike]] sav
+0002fb40: 655f 6469 723a 2044 6972 6563 746f 7279  e_dir: Directory
+0002fb50: 2077 6865 7265 2074 6865 206d 6f64 6966   where the modif
+0002fb60: 6965 6420 7669 6465 6f28 7329 2077 696c  ied video(s) wil
+0002fb70: 6c20 6265 2073 6176 6564 2e20 4966 206e  l be saved. If n
+0002fb80: 6f74 2070 726f 7669 6465 642c 2074 6865  ot provided, the
+0002fb90: 2064 6972 6563 746f 7279 206f 6620 7468   directory of th
+0002fba0: 6520 696e 7075 7420 7669 6465 6f28 7329  e input video(s)
+0002fbb0: 2077 696c 6c20 6265 2075 7365 642e 0a20   will be used.. 
+0002fbc0: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
+0002fbd0: 0a20 2020 2022 2222 0a0a 2020 2020 6368  .    """..    ch
+0002fbe0: 6563 6b5f 6666 6d70 6567 5f61 7661 696c  eck_ffmpeg_avail
+0002fbf0: 6162 6c65 2872 6169 7365 5f65 7272 6f72  able(raise_error
+0002fc00: 3d54 7275 6529 0a20 2020 2074 696d 6572  =True).    timer
+0002fc10: 203d 2053 696d 6261 5469 6d65 7228 7374   = SimbaTimer(st
+0002fc20: 6172 743d 5472 7565 290a 2020 2020 504f  art=True).    PO
+0002fc30: 5349 5449 4f4e 5320 3d20 5b27 746f 705f  SITIONS = ['top_
+0002fc40: 6c65 6674 272c 2027 746f 705f 7269 6768  left', 'top_righ
+0002fc50: 7427 2c20 2762 6f74 746f 6d5f 6c65 6674  t', 'bottom_left
+0002fc60: 272c 2027 626f 7474 6f6d 5f72 6967 6874  ', 'bottom_right
+0002fc70: 272c 2027 746f 705f 6d69 6464 6c65 272c  ', 'top_middle',
+0002fc80: 2027 626f 7474 6f6d 5f6d 6964 646c 6527   'bottom_middle'
+0002fc90: 5d0a 2020 2020 6368 6563 6b5f 7374 7228  ].    check_str(
+0002fca0: 6e61 6d65 3d66 277b 7375 7065 7269 6d70  name=f'{superimp
+0002fcb0: 6f73 655f 6672 6565 7465 7874 2e5f 5f6e  ose_freetext.__n
+0002fcc0: 616d 655f 5f7d 2070 6f73 6974 696f 6e27  ame__} position'
+0002fcd0: 2c20 7661 6c75 653d 706f 7369 7469 6f6e  , value=position
+0002fce0: 2c20 6f70 7469 6f6e 733d 504f 5349 5449  , options=POSITI
+0002fcf0: 4f4e 5329 0a20 2020 2063 6865 636b 5f69  ONS).    check_i
+0002fd00: 6e74 286e 616d 653d 6627 7b73 7570 6572  nt(name=f'{super
+0002fd10: 696d 706f 7365 5f66 7265 6574 6578 742e  impose_freetext.
+0002fd20: 5f5f 6e61 6d65 5f5f 7d20 666f 6e74 5f73  __name__} font_s
+0002fd30: 697a 6527 2c20 7661 6c75 653d 666f 6e74  ize', value=font
+0002fd40: 5f73 697a 652c 206d 696e 5f76 616c 7565  _size, min_value
+0002fd50: 3d31 290a 2020 2020 6368 6563 6b5f 696e  =1).    check_in
+0002fd60: 7428 6e61 6d65 3d66 277b 7375 7065 7269  t(name=f'{superi
+0002fd70: 6d70 6f73 655f 6672 6565 7465 7874 2e5f  mpose_freetext._
+0002fd80: 5f6e 616d 655f 5f7d 2066 6f6e 745f 626f  _name__} font_bo
+0002fd90: 7264 6572 5f77 6964 7468 272c 2076 616c  rder_width', val
+0002fda0: 7565 3d66 6f6e 745f 626f 7264 6572 5f77  ue=font_border_w
+0002fdb0: 6964 7468 2c20 6d69 6e5f 7661 6c75 653d  idth, min_value=
+0002fdc0: 3129 0a20 2020 2063 6865 636b 5f73 7472  1).    check_str
+0002fdd0: 286e 616d 653d 6627 7b73 7570 6572 696d  (name=f'{superim
+0002fde0: 706f 7365 5f66 7265 6574 6578 742e 5f5f  pose_freetext.__
+0002fdf0: 6e61 6d65 5f5f 7d20 7465 7874 272c 2076  name__} text', v
+0002fe00: 616c 7565 3d74 6578 7429 0a20 2020 2066  alue=text).    f
+0002fe10: 6f6e 745f 636f 6c6f 7220 3d20 2727 2e6a  ont_color = ''.j
+0002fe20: 6f69 6e28 6669 6c74 6572 2873 7472 2e69  oin(filter(str.i
+0002fe30: 7361 6c6e 756d 2c20 666f 6e74 5f63 6f6c  salnum, font_col
+0002fe40: 6f72 2929 2e6c 6f77 6572 2829 0a20 2020  or)).lower().   
+0002fe50: 2066 6f6e 745f 626f 7264 6572 5f63 6f6c   font_border_col
+0002fe60: 6f72 203d 2027 272e 6a6f 696e 2866 696c  or = ''.join(fil
+0002fe70: 7465 7228 7374 722e 6973 616c 6e75 6d2c  ter(str.isalnum,
+0002fe80: 2066 6f6e 745f 626f 7264 6572 5f63 6f6c   font_border_col
+0002fe90: 6f72 2929 2e6c 6f77 6572 2829 0a20 2020  or)).lower().   
+0002fea0: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+0002feb0: 6c65 2876 6964 656f 5f70 6174 6829 3a0a  le(video_path):.
+0002fec0: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
+0002fed0: 7468 7320 3d20 5b76 6964 656f 5f70 6174  ths = [video_pat
+0002fee0: 685d 0a20 2020 2065 6c69 6620 6f73 2e70  h].    elif os.p
+0002fef0: 6174 682e 6973 6469 7228 7669 6465 6f5f  ath.isdir(video_
+0002ff00: 7061 7468 293a 0a20 2020 2020 2020 2076  path):.        v
+0002ff10: 6964 656f 5f70 6174 6873 203d 206c 6973  ideo_paths = lis
+0002ff20: 7428 6669 6e64 5f61 6c6c 5f76 6964 656f  t(find_all_video
+0002ff30: 735f 696e 5f64 6972 6563 746f 7279 2864  s_in_directory(d
+0002ff40: 6972 6563 746f 7279 3d76 6964 656f 5f70  irectory=video_p
+0002ff50: 6174 682c 2061 735f 6469 6374 3d54 7275  ath, as_dict=Tru
+0002ff60: 652c 2072 6169 7365 5f65 7272 6f72 3d54  e, raise_error=T
+0002ff70: 7275 6529 2e76 616c 7565 7328 2929 0a20  rue).values()). 
+0002ff80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002ff90: 2072 6169 7365 2049 6e76 616c 6964 496e   raise InvalidIn
+0002ffa0: 7075 7445 7272 6f72 286d 7367 3d66 277b  putError(msg=f'{
+0002ffb0: 7669 6465 6f5f 7061 7468 7d20 6973 206e  video_path} is n
+0002ffc0: 6f74 2061 2076 616c 6964 2066 696c 6520  ot a valid file 
+0002ffd0: 7061 7468 206f 7220 6120 7661 6c69 6420  path or a valid 
+0002ffe0: 6469 7265 6374 6f72 7920 7061 7468 272c  directory path',
+0002fff0: 2073 6f75 7263 653d 7375 7065 7269 6d70   source=superimp
+00030000: 6f73 655f 7669 6465 6f5f 6e61 6d65 732e  ose_video_names.
+00030010: 5f5f 6e61 6d65 5f5f 290a 2020 2020 6966  __name__).    if
+00030020: 2073 6176 655f 6469 7220 6973 206e 6f74   save_dir is not
+00030030: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
+00030040: 6865 636b 5f69 665f 6469 725f 6578 6973  heck_if_dir_exis
+00030050: 7473 2869 6e5f 6469 723d 7361 7665 5f64  ts(in_dir=save_d
+00030060: 6972 290a 2020 2020 656c 7365 3a0a 2020  ir).    else:.  
+00030070: 2020 2020 2020 7361 7665 5f64 6972 203d        save_dir =
+00030080: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+00030090: 2876 6964 656f 5f70 6174 6873 5b30 5d29  (video_paths[0])
+000300a0: 0a20 2020 2066 6f72 2066 696c 655f 636e  .    for file_cn
+000300b0: 742c 2076 6964 656f 5f70 6174 6820 696e  t, video_path in
+000300c0: 2065 6e75 6d65 7261 7465 2876 6964 656f   enumerate(video
+000300d0: 5f70 6174 6873 293a 0a20 2020 2020 2020  _paths):.       
+000300e0: 205f 2c20 7669 6465 6f5f 6e61 6d65 2c20   _, video_name, 
+000300f0: 6578 7420 3d20 6765 745f 666e 5f65 7874  ext = get_fn_ext
+00030100: 2876 6964 656f 5f70 6174 6829 0a20 2020  (video_path).   
+00030110: 2020 2020 2070 7269 6e74 2866 2753 7570       print(f'Sup
+00030120: 6572 696d 706f 7369 6e67 2076 6964 656f  erimposing video
+00030130: 206e 616d 6520 6f6e 207b 7669 6465 6f5f   name on {video_
+00030140: 6e61 6d65 7d20 2856 6964 656f 207b 6669  name} (Video {fi
+00030150: 6c65 5f63 6e74 202b 2031 7d2f 7b6c 656e  le_cnt + 1}/{len
+00030160: 2876 6964 656f 5f70 6174 6873 297d 292e  (video_paths)}).
+00030170: 2e2e 2729 0a20 2020 2020 2020 2073 6176  ..').        sav
+00030180: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
+00030190: 2e6a 6f69 6e28 7361 7665 5f64 6972 2c20  .join(save_dir, 
+000301a0: 6627 7b76 6964 656f 5f6e 616d 657d 5f74  f'{video_name}_t
+000301b0: 6578 745f 7375 7065 7269 6d70 6f73 6564  ext_superimposed
+000301c0: 7b65 7874 7d27 290a 2020 2020 2020 2020  {ext}').        
+000301d0: 6966 2070 6f73 6974 696f 6e20 3d3d 2050  if position == P
+000301e0: 4f53 4954 494f 4e53 5b30 5d3a 0a20 2020  OSITIONS[0]:.   
+000301f0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+00030200: 2266 666d 7065 6720 2d69 2027 7b76 6964  "ffmpeg -i '{vid
+00030210: 656f 5f70 6174 687d 2720 2d76 6620 5c22  eo_path}' -vf \"
+00030220: 6472 6177 7465 7874 3d66 6f6e 7466 696c  drawtext=fontfil
+00030230: 653d 4172 6961 6c2e 7474 663a 7465 7874  e=Arial.ttf:text
+00030240: 3d7b 7465 7874 7d3a 783d 353a 793d 353a  ={text}:x=5:y=5:
+00030250: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
+00030260: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
+00030270: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
+00030280: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
+00030290: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
+000302a0: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
+000302b0: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
+000302c0: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
+000302d0: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
+000302e0: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
+000302f0: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
+00030300: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
+00030310: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
+00030320: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00030330: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
+00030340: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
+00030350: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
+00030360: 7466 696c 653d 4172 6961 6c2e 7474 663a  tfile=Arial.ttf:
+00030370: 7465 7874 3d7b 7465 7874 7d3a 783d 2877  text={text}:x=(w
+00030380: 2d74 772d 3529 3a79 3d35 3a66 6f6e 7473  -tw-5):y=5:fonts
+00030390: 697a 653d 7b66 6f6e 745f 7369 7a65 7d3a  ize={font_size}:
+000303a0: 666f 6e74 636f 6c6f 723d 7b66 6f6e 745f  fontcolor={font_
+000303b0: 636f 6c6f 727d 3a62 6f72 6465 7277 3d7b  color}:borderw={
+000303c0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+000303d0: 687d 3a62 6f72 6465 7263 6f6c 6f72 3d7b  h}:bordercolor={
+000303e0: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+000303f0: 727d 5c22 202d 633a 6120 636f 7079 2027  r}\" -c:a copy '
+00030400: 7b73 6176 655f 7061 7468 7d27 202d 6c6f  {save_path}' -lo
+00030410: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
+00030420: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
+00030430: 202d 7922 0a20 2020 2020 2020 2065 6c69   -y".        eli
+00030440: 6620 706f 7369 7469 6f6e 203d 3d20 504f  f position == PO
+00030450: 5349 5449 4f4e 535b 325d 3a0a 2020 2020  SITIONS[2]:.    
+00030460: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
+00030470: 6666 6d70 6567 202d 6920 277b 7669 6465  ffmpeg -i '{vide
+00030480: 6f5f 7061 7468 7d27 202d 7666 205c 2264  o_path}' -vf \"d
+00030490: 7261 7774 6578 743d 666f 6e74 6669 6c65  rawtext=fontfile
+000304a0: 3d41 7269 616c 2e74 7466 3a74 6578 743d  =Arial.ttf:text=
+000304b0: 7b74 6578 747d 3a78 3d35 3a79 3d28 682d  {text}:x=5:y=(h-
+000304c0: 7468 2d35 293a 666f 6e74 7369 7a65 3d7b  th-5):fontsize={
+000304d0: 666f 6e74 5f73 697a 657d 3a66 6f6e 7463  font_size}:fontc
+000304e0: 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c 6f72  olor={font_color
+000304f0: 7d3a 626f 7264 6572 773d 7b66 6f6e 745f  }:borderw={font_
+00030500: 626f 7264 6572 5f77 6964 7468 7d3a 626f  border_width}:bo
+00030510: 7264 6572 636f 6c6f 723d 7b66 6f6e 745f  rdercolor={font_
+00030520: 626f 7264 6572 5f63 6f6c 6f72 7d5c 2220  border_color}\" 
+00030530: 2d63 3a61 2063 6f70 7920 277b 7361 7665  -c:a copy '{save
+00030540: 5f70 6174 687d 2720 2d6c 6f67 6c65 7665  _path}' -logleve
+00030550: 6c20 6572 726f 7220 2d73 7461 7473 202d  l error -stats -
+00030560: 6869 6465 5f62 616e 6e65 7220 2d79 220a  hide_banner -y".
+00030570: 2020 2020 2020 2020 656c 6966 2070 6f73          elif pos
+00030580: 6974 696f 6e20 3d3d 2050 4f53 4954 494f  ition == POSITIO
+00030590: 4e53 5b33 5d3a 0a20 2020 2020 2020 2020  NS[3]:.         
+000305a0: 2020 2063 6d64 203d 2066 2266 666d 7065     cmd = f"ffmpe
+000305b0: 6720 2d69 2027 7b76 6964 656f 5f70 6174  g -i '{video_pat
+000305c0: 687d 2720 2d76 6620 5c22 6472 6177 7465  h}' -vf \"drawte
+000305d0: 7874 3d66 6f6e 7466 696c 653d 4172 6961  xt=fontfile=Aria
+000305e0: 6c2e 7474 663a 7465 7874 3d7b 7465 7874  l.ttf:text={text
+000305f0: 7d3a 783d 2877 2d74 772d 3529 3a79 3d28  }:x=(w-tw-5):y=(
+00030600: 682d 7468 2d35 293a 666f 6e74 7369 7a65  h-th-5):fontsize
+00030610: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
+00030620: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
+00030630: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
+00030640: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
+00030650: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
+00030660: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
+00030670: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
+00030680: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
+00030690: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
+000306a0: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
+000306b0: 220a 2020 2020 2020 2020 656c 6966 2070  ".        elif p
+000306c0: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
+000306d0: 494f 4e53 5b34 5d3a 0a20 2020 2020 2020  IONS[4]:.       
+000306e0: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
+000306f0: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
+00030700: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
+00030710: 7465 7874 3d66 6f6e 7466 696c 653d 4172  text=fontfile=Ar
+00030720: 6961 6c2e 7474 663a 7465 7874 3d7b 7465  ial.ttf:text={te
+00030730: 7874 7d3a 783d 2877 2d74 7729 2f32 3a79  xt}:x=(w-tw)/2:y
+00030740: 3d31 303a 666f 6e74 7369 7a65 3d7b 666f  =10:fontsize={fo
+00030750: 6e74 5f73 697a 657d 3a66 6f6e 7463 6f6c  nt_size}:fontcol
+00030760: 6f72 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a  or={font_color}:
+00030770: 626f 7264 6572 773d 7b66 6f6e 745f 626f  borderw={font_bo
+00030780: 7264 6572 5f77 6964 7468 7d3a 626f 7264  rder_width}:bord
+00030790: 6572 636f 6c6f 723d 7b66 6f6e 745f 626f  ercolor={font_bo
+000307a0: 7264 6572 5f63 6f6c 6f72 7d5c 2220 2d63  rder_color}\" -c
+000307b0: 3a61 2063 6f70 7920 277b 7361 7665 5f70  :a copy '{save_p
+000307c0: 6174 687d 2720 2d6c 6f67 6c65 7665 6c20  ath}' -loglevel 
+000307d0: 6572 726f 7220 2d73 7461 7473 202d 6869  error -stats -hi
+000307e0: 6465 5f62 616e 6e65 7220 2d79 220a 2020  de_banner -y".  
+000307f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00030800: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
+00030810: 6666 6d70 6567 202d 6920 277b 7669 6465  ffmpeg -i '{vide
+00030820: 6f5f 7061 7468 7d27 202d 7666 205c 2264  o_path}' -vf \"d
+00030830: 7261 7774 6578 743d 666f 6e74 6669 6c65  rawtext=fontfile
+00030840: 3d41 7269 616c 2e74 7466 3a74 6578 743d  =Arial.ttf:text=
+00030850: 7b74 6578 747d 3a78 3d28 772d 7477 292f  {text}:x=(w-tw)/
+00030860: 323a 793d 2868 2d74 682d 3130 293a 666f  2:y=(h-th-10):fo
+00030870: 6e74 7369 7a65 3d7b 666f 6e74 5f73 697a  ntsize={font_siz
+00030880: 657d 3a66 6f6e 7463 6f6c 6f72 3d7b 666f  e}:fontcolor={fo
+00030890: 6e74 5f63 6f6c 6f72 7d3a 626f 7264 6572  nt_color}:border
+000308a0: 773d 7b66 6f6e 745f 626f 7264 6572 5f77  w={font_border_w
+000308b0: 6964 7468 7d3a 626f 7264 6572 636f 6c6f  idth}:bordercolo
+000308c0: 723d 7b66 6f6e 745f 626f 7264 6572 5f63  r={font_border_c
+000308d0: 6f6c 6f72 7d5c 2220 2d63 3a61 2063 6f70  olor}\" -c:a cop
+000308e0: 7920 277b 7361 7665 5f70 6174 687d 2720  y '{save_path}' 
+000308f0: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
+00030900: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
+00030910: 6e65 7220 2d79 220a 2020 2020 2020 2020  ner -y".        
+00030920: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
+00030930: 636d 642c 2073 6865 6c6c 3d54 7275 652c  cmd, shell=True,
+00030940: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
+00030950: 7373 2e50 4950 4529 0a20 2020 2074 696d  ss.PIPE).    tim
+00030960: 6572 2e73 746f 705f 7469 6d65 7228 290a  er.stop_timer().
+00030970: 2020 2020 7374 646f 7574 5f73 7563 6365      stdout_succe
+00030980: 7373 286d 7367 3d66 2753 7570 6572 2d69  ss(msg=f'Super-i
+00030990: 6d70 6f73 6564 2066 7265 652d 7465 7874  mposed free-text
+000309a0: 206f 6e20 7b6c 656e 2876 6964 656f 5f70   on {len(video_p
+000309b0: 6174 6873 297d 2076 6964 656f 2873 292c  aths)} video(s),
+000309c0: 2073 6176 6564 2069 6e20 7b73 6176 655f   saved in {save_
+000309d0: 6469 727d 272c 2065 6c61 7073 6564 5f74  dir}', elapsed_t
+000309e0: 696d 653d 7469 6d65 722e 656c 6170 7365  ime=timer.elapse
+000309f0: 645f 7469 6d65 5f73 7472 290a 0a0a 2320  d_time_str)...# 
+00030a00: 7669 6465 6f5f 7061 7468 7320 3d20 5b27  video_paths = ['
+00030a10: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00030a20: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00030a30: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00030a40: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+00030a50: 6563 745f 666f 6c64 6572 2f6d 6572 6765  ect_folder/merge
+00030a60: 2f54 7269 616c 2020 2020 3130 5f63 6c69  /Trial    10_cli
+00030a70: 7070 6564 5f67 616e 7474 2e6d 7034 272c  pped_gantt.mp4',
+00030a80: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
+00030a90: 2020 272f 5573 6572 732f 7369 6d6f 6e2f    '/Users/simon/
+00030aa0: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
+00030ab0: 6261 2f74 726f 7562 6c65 7368 6f6f 7469  ba/troubleshooti
+00030ac0: 6e67 2f62 6565 7062 6f6f 7031 3734 2f70  ng/beepboop174/p
+00030ad0: 726f 6a65 6374 5f66 6f6c 6465 722f 6d65  roject_folder/me
+00030ae0: 7267 652f 5472 6961 6c20 2020 2031 305f  rge/Trial    10_
+00030af0: 636c 6970 7065 642e 6d70 3427 2c0a 2320  clipped.mp4',.# 
+00030b00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00030b10: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00030b20: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00030b30: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00030b40: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+00030b50: 6563 745f 666f 6c64 6572 2f6d 6572 6765  ect_folder/merge
+00030b60: 2f54 7269 616c 2020 2020 3130 5f63 6c69  /Trial    10_cli
+00030b70: 7070 6564 5f6c 696e 652e 6d70 3427 2c0a  pped_line.mp4',.
+00030b80: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00030b90: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+00030ba0: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+00030bb0: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+00030bc0: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+00030bd0: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
+00030be0: 6765 2f54 7269 616c 2020 2020 2033 5f63  ge/Trial     3_c
+00030bf0: 6c69 7070 6564 2e6d 7034 275d 0a23 0a23  lipped.mp4'].#.#
+00030c00: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
+00030c10: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+00030c20: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+00030c30: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+00030c40: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+00030c50: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+00030c60: 6f73 2f54 7269 616c 2020 2020 3130 2e6d  os/Trial    10.m
+00030c70: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
+00030c80: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
+00030c90: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00030ca0: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00030cb0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+00030cc0: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+00030cd0: 722f 6d65 7267 652f 5472 6961 6c20 2020  r/merge/Trial   
+00030ce0: 2031 305f 636c 6970 7065 645f 6761 6e74   10_clipped_gant
+00030cf0: 742e 6d70 3427 2c0a 2320 2020 2020 2020  t.mp4',.#       
+00030d00: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
+00030d10: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
+00030d20: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
+00030d30: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
+00030d40: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
+00030d50: 6c64 6572 2f6d 6572 6765 2f54 7269 616c  lder/merge/Trial
+00030d60: 2020 2020 3130 5f63 6c69 7070 6564 5f6c      10_clipped_l
+00030d70: 696e 652e 6d70 3427 2c0a 2320 2020 2020  ine.mp4',.#     
+00030d80: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
+00030d90: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+00030da0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+00030db0: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+00030dc0: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+00030dd0: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
+00030de0: 616c 2020 2020 2033 5f63 6c69 7070 6564  al     3_clipped
+00030df0: 2e6d 7034 275d 0a23 0a23 2073 6176 655f  .mp4'].#.# save_
+00030e00: 7061 7468 203d 2027 2f55 7365 7273 2f73  path = '/Users/s
+00030e10: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00030e20: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00030e30: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+00030e40: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+00030e50: 6572 2f6d 6572 6765 2f6f 7574 2e6d 7034  er/merge/out.mp4
+00030e60: 270a 0a23 0a23 2076 6964 656f 5f70 6174  '..#.# video_pat
+00030e70: 6873 203d 205b 272f 5573 6572 732f 7369  hs = ['/Users/si
+00030e80: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00030e90: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00030ea0: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+00030eb0: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+00030ec0: 722f 6672 616d 6573 2f6f 7574 7075 742f  r/frames/output/
+00030ed0: 6761 6e74 745f 706c 6f74 732f 5472 6961  gantt_plots/Tria
+00030ee0: 6c20 2020 2031 302e 6d70 3427 2c0a 2320  l    10.mp4',.# 
+00030ef0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00030f00: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00030f10: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00030f20: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00030f30: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+00030f40: 6563 745f 666f 6c64 6572 2f76 6964 656f  ect_folder/video
+00030f50: 732f 5472 6961 6c20 2020 2031 302e 6d70  s/Trial    10.mp
+00030f60: 3427 2c0a 2320 2020 2020 2020 2020 2020  4',.#           
+00030f70: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
+00030f80: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+00030f90: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00030fa0: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
+00030fb0: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
+00030fc0: 2f66 7261 6d65 732f 6f75 7470 7574 2f6c  /frames/output/l
+00030fd0: 696e 655f 706c 6f74 2f54 7269 616c 2020  ine_plot/Trial  
+00030fe0: 2020 3130 2e6d 7034 272c 0a23 2020 2020    10.mp4',.#    
+00030ff0: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
+00031000: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+00031010: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+00031020: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+00031030: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+00031040: 5f66 6f6c 6465 722f 6672 616d 6573 2f6f  _folder/frames/o
+00031050: 7574 7075 742f 6c69 6e65 5f70 6c6f 742f  utput/line_plot/
+00031060: 5472 6961 6c20 2020 2020 332e 6d70 3427  Trial     3.mp4'
+00031070: 5d0a 2320 7361 7665 5f70 6174 6820 3d20  ].# save_path = 
+00031080: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+00031090: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+000310a0: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+000310b0: 2f52 4154 5f4e 4f52 2f70 726f 6a65 6374  /RAT_NOR/project
+000310c0: 5f66 6f6c 6465 722f 7669 6465 6f73 2f74  _folder/videos/t
+000310d0: 6573 742f 6e65 772f 626c 616e 6b5f 7465  est/new/blank_te
+000310e0: 7374 2e6d 7034 270a 0a23 2076 6964 656f  st.mp4'..# video
+000310f0: 5f70 6174 6873 203d 205b 272f 5573 6572  _paths = ['/User
+00031100: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+00031110: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+00031120: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
+00031130: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
+00031140: 6f6c 6465 722f 7669 6465 6f73 2f54 7269  older/videos/Tri
+00031150: 616c 2020 2020 3130 2e6d 7034 272c 0a23  al    10.mp4',.#
+00031160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031170: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+00031180: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+00031190: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+000311a0: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+000311b0: 6a65 6374 5f66 6f6c 6465 722f 6672 616d  ject_folder/fram
+000311c0: 6573 2f6f 7574 7075 742f 6c69 6e65 5f70  es/output/line_p
+000311d0: 6c6f 742f 5472 6961 6c20 2020 2031 302e  lot/Trial    10.
+000311e0: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
+000311f0: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
+00031200: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00031210: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00031220: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+00031230: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+00031240: 6572 2f66 7261 6d65 732f 6f75 7470 7574  er/frames/output
+00031250: 2f6c 696e 655f 706c 6f74 2f54 7269 616c  /line_plot/Trial
+00031260: 2020 2020 2033 2e6d 7034 275d 0a0a 2320       3.mp4']..# 
+00031270: 6d69 7865 645f 6d6f 7361 6963 5f63 6f6e  mixed_mosaic_con
+00031280: 6361 7465 6e61 746f 7228 7669 6465 6f5f  catenator(video_
+00031290: 7061 7468 733d 7669 6465 6f5f 7061 7468  paths=video_path
+000312a0: 732c 2073 6176 655f 7061 7468 3d73 6176  s, save_path=sav
+000312b0: 655f 7061 7468 2c20 6770 753d 4661 6c73  e_path, gpu=Fals
+000312c0: 652c 2076 6572 626f 7365 3d54 7275 6529  e, verbose=True)
+000312d0: 0a                                       .
```

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/brightness_contrast_ui.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/brightness_contrast_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/video_processors/clahe_ui.py` & `Simba-UW-tf-dev-1.93.4/simba/video_processors/clahe_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.93.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.93.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.93.4/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,16 @@
     DownsampleVideoPopUp, ExtractAllFramesPopUp, ExtractAnnotationFramesPopUp,
     ExtractSEQFramesPopUp, ExtractSpecificFramesPopUp,
     GreyscaleSingleVideoPopUp, ImportFrameDirectoryPopUp,
     InitiateClipMultipleVideosByFrameNumbersPopUp,
     InitiateClipMultipleVideosByTimestampsPopUp, InteractiveClahePopUp,
     MergeFrames2VideoPopUp, MultiCropPopUp, MultiShortenPopUp,
     SuperImposeFrameCountPopUp, VideoRotatorPopUp, VideoTemporalJoinPopUp,
-    SuperimposeTimerPopUp, SuperimposeWatermarkPopUp, SuperimposeProgressBarPopUp)
+    SuperimposeTimerPopUp, SuperimposeWatermarkPopUp, SuperimposeProgressBarPopUp, SuperimposeVideoPopUp, SuperimposeVideoNamesPopUp,
+    SuperimposeTextPopUp, BoxBlurPopUp)
 from simba.ui.pop_ups.visualize_pose_in_dir_pop_up import \
     VisualizePoseInFolderPopUp
 from simba.ui.tkinter_functions import DropDownMenu, Entry_Box, FileSelect
 from simba.ui.video_info_ui import VideoInfoTable
 from simba.utils.checks import (check_ffmpeg_available,
                                 check_file_exist_and_readable, check_int)
 from simba.utils.custom_feature_extractor import CustomFeatureExtractor
@@ -1779,25 +1780,22 @@
         )
 
         superimpose_menu = Menu(menu)
         superimpose_menu.add_command(label="Superimpose frame numbers on videos", command=SuperImposeFrameCountPopUp)
         superimpose_menu.add_command(label="Superimpose watermark on videos", command=SuperimposeWatermarkPopUp)
         superimpose_menu.add_command(label="Superimpose timer on videos", command=SuperimposeTimerPopUp)
         superimpose_menu.add_command(label="Superimpose progress-bar on videos", command=SuperimposeProgressBarPopUp)
+        superimpose_menu.add_command(label="Superimpose video on video", command=SuperimposeVideoPopUp)
+        superimpose_menu.add_command(label="Superimpose video names on video", command=SuperimposeVideoNamesPopUp)
+        superimpose_menu.add_command(label="Superimpose free-text on video", command=SuperimposeTextPopUp)
         video_process_menu.add_cascade(label="Superimpose on videos...", compound="left", image=self.menu_icons["superimpose"]["img"], menu=superimpose_menu)
 
         video_process_menu.add_command(label="Temporal join videos", compound="left", image=self.menu_icons["stopwatch"]["img"], command=VideoTemporalJoinPopUp)
-
-        video_process_menu.add_cascade(
-            label="Visualize pose-estimation in folder...",
-            compound="left",
-            image=self.menu_icons["visualize"]["img"],
-            command=VisualizePoseInFolderPopUp,
-        )
-
+        video_process_menu.add_cascade(label="Box blur videos...", compound="left", image=self.menu_icons["blur"]["img"], command=BoxBlurPopUp)
+        video_process_menu.add_cascade(label="Visualize pose-estimation in folder...", compound="left", image=self.menu_icons["visualize"]["img"], command=VisualizePoseInFolderPopUp)
         help_menu = Menu(menu)
         menu.add_cascade(label="Help", menu=help_menu)
 
         links_menu = Menu(help_menu)
         links_menu.add_command(
             label="Download weights",
             command=lambda: webbrowser.open_new(str(r"https://osf.io/sr3ck/")),
```

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.93.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.93.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.93.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.93.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.93.4/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.93.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.93.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.93.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.93.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.93.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/brightness.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/brightness.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.93.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.93.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.93.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.93.3
+Version: 1.93.4
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 simba/assets/icons/.DS_Store
 simba/assets/icons/SimBA_logo.icns
 simba/assets/icons/SimBA_logo.ico
 simba/assets/icons/SimBA_logo.png
 simba/assets/icons/__init__.py
 simba/assets/icons/about.png
 simba/assets/icons/add_on.png
+simba/assets/icons/blur.png
 simba/assets/icons/boris.png
 simba/assets/icons/brightness.png
 simba/assets/icons/browse.png
 simba/assets/icons/calipher.png
 simba/assets/icons/change.png
 simba/assets/icons/circle.png
 simba/assets/icons/clahe.png
@@ -469,14 +470,15 @@
 simba/sandbox/spontaneous_alternation_calculator.py
 simba/sandbox/spontaneuous_alternation_plotter.py
 simba/sandbox/spontanous_alternations.py
 simba/sandbox/statistics_ex.py
 simba/sandbox/superimpose_elapsed_time.py
 simba/sandbox/superimpose_frame_count.py
 simba/sandbox/superimpose_popups.py
+simba/sandbox/superimpose_text.py
 simba/sandbox/superpixels.py
 simba/sandbox/termite_rois.csv
 simba/sandbox/time_stamp_calculator.py
 simba/sandbox/total_variation_distance.py
 simba/sandbox/train_model.py
 simba/sandbox/two_fish_feature_extractor_040924.py
 simba/sandbox/two_fish_feature_extractor_040924.py.zip
```

### Comparing `Simba-UW-tf-dev-1.93.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.93.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/LICENSE` & `Simba-UW-tf-dev-1.93.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.93.4/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.93.4/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_stats.py` & `Simba-UW-tf-dev-1.93.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.93.4/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.93.4/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.93.4/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.93.4/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.93.4/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.93.4/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.93.4/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.93.4/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.93.4/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.93.4/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/README.md` & `Simba-UW-tf-dev-1.93.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.3/setup.py` & `Simba-UW-tf-dev-1.93.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.93.3",
+    version="1.93.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

