# Comparing `tmp/Simba-UW-tf-dev-1.60.2.tar.gz` & `tmp/Simba-UW-tf-dev-1.60.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.2.tar", last modified: Sat May 20 12:38:25 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.3.tar", last modified: Sun May 21 18:08:49 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.60.2.tar` & `Simba-UW-tf-dev-1.60.3.tar`

### file list

```diff
@@ -1,504 +1,503 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.60.2/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.60.2/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.2/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.60.2/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-19 21:21:01.000000 Simba-UW-tf-dev-1.60.2/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.60.2/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.2/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.2/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.60.2/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.2/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.2/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.2/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.2/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.2/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.2/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.2/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.2/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.2/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.2/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.2/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19618 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.2/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.2/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.2/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-20 12:38:16.000000 Simba-UW-tf-dev-1.60.2/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.60.3/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.60.3/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.3/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.3/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.3/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.3/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.3/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.3/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.3/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-21 17:57:48.000000 Simba-UW-tf-dev-1.60.3/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.60.3/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.3/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10627 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.3/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.3/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.3/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.3/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.3/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    41782 2023-05-21 17:06:37.000000 Simba-UW-tf-dev-1.60.3/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.3/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.3/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.3/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.3/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.3/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.3/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.3/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.3/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.60.3/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.3/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.3/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.3/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.3/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.60.3/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.3/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.3/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.3/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.3/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18395 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       11 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-21 18:08:48.000000 Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.3/LICENSE.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.60.3/test/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.60.3/test/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.60.3/test/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.60.3/pyproject.toml
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.3/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.3/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-21 18:08:33.000000 Simba-UW-tf-dev-1.60.3/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-21 18:08:49.000000 Simba-UW-tf-dev-1.60.3/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.60.2/PKG-INFO` & `Simba-UW-tf-dev-1.60.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.2
+Version: 1.60.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.60.3/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.60.3/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.60.3/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.60.3/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.60.3/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.60.3/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.60.3/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -99,38 +99,38 @@
 00000620: 0128 012a 012b 012d 0136 0137 0139 013a  .(.*.+.-.6.7.9.:
 00000630: 0143 0144 0145 0147 0150 0151 0153 0154  .C.D.E.G.P.Q.S.T
 00000640: 0156 015f 0160 0162 0163 0165 016e 016f  .V._.`.b.c.e.n.o
 00000650: 0171 0172 0174 017d 017e 0180 0181 0183  .q.r.t.}.~......
 00000660: 018c 018d 0190 0191 0193 0194 019d 01aa  ................
 00000670: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
 00000680: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00000690: 01b4 2425 180a 5473 697a 6510 6108 09d4  ..$%..Tsize.a...
-000006a0: 0d0e 0f10 292a 0a0a 546b 696e 6410 7309  ....)*..Tkind.s.
-000006b0: 09d4 0d0e 0f10 2e2f 0a18 556c 6162 656c  ......./..Ulabel
-000006c0: 1064 0908 d40d 0e0f 1033 340a 1857 7665  .d.......34..Wve
-000006d0: 7273 696f 6e10 4b09 08d4 0d0e 0f10 3839  rsion.K.......89
-000006e0: 0a18 5863 6f6d 6d65 6e74 7311 012c 0908  ..Xcomments..,..
-000006f0: d40d 0e0f 103d 3e18 185e 6461 7465 4c61  .....=>..^dateLa
-00000700: 7374 4f70 656e 6564 10c8 0808 d40d 0e0f  stOpened........
-00000710: 1042 1c18 1859 6461 7465 4164 6465 6408  .B...YdateAdded.
-00000720: 0808 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
-00000730: 4d6f 6469 6669 6564 2340 3000 0000 0000  Modified#@0.....
-00000740: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00000750: 0070 0079 008c 008e 008f 009b 00a4 00af  .p.y............
-00000760: 00b5 00bf 00c7 00cc 00cf 00d0 00d1 00da  ................
-00000770: 00e3 00e5 00e6 00e7 00f0 00fd 00ff 0100  ................
-00000780: 0101 010a 0116 0117 0118 0121 0126 0128  ...........!.&.(
-00000790: 0129 012a 0133 0138 013a 013b 013c 0145  .).*.3.8.:.;.<.E
-000007a0: 014b 014d 014e 014f 0158 0160 0162 0163  .K.M.N.O.X.`.b.c
-000007b0: 0164 016d 0176 0179 017a 017b 0184 0193  .d.m.v.y.z.{....
-000007c0: 0195 0196 0197 01a0 01aa 01ab 01ac 01ad  ................
-000007d0: 01b6 01c3 01cc 0000 0000 0000 0201 0000  ................
-000007e0: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-000007f0: 0000 0000 01cd 0000 000c 0075 006e 0073  ...........u.n.s
-00000800: 0075 0070 0000 0001 0000 0000 0000 080b  .u.p............
+00000690: 01b4 1024 2518 0a54 7369 7a65 1061 0809  ...$%..Tsize.a..
+000006a0: d40d 0e0f 1029 2a0a 0a54 6b69 6e64 1073  .....)*..Tkind.s
+000006b0: 0909 d40d 0e0f 102e 2f0a 1855 6c61 6265  ......../..Ulabe
+000006c0: 6c10 6409 08d4 0d0e 0f10 3334 0a18 5776  l.d.......34..Wv
+000006d0: 6572 7369 6f6e 104b 0908 d40d 0e0f 1038  ersion.K.......8
+000006e0: 390a 1858 636f 6d6d 656e 7473 1101 2c09  9..Xcomments..,.
+000006f0: 08d4 0d0e 0f10 3d3e 1818 5e64 6174 654c  ......=>..^dateL
+00000700: 6173 744f 7065 6e65 6410 c808 08d4 0d0e  astOpened.......
+00000710: 0f10 421c 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
+00000720: 0808 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
+00000730: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
+00000740: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+00000750: 6500 7000 7900 8c00 8e00 8f00 9b00 a400  e.p.y...........
+00000760: af00 b500 bf00 c700 cc00 cf00 d000 d100  ................
+00000770: da00 e300 e500 e600 e700 f000 fd00 ff01  ................
+00000780: 0001 0101 0a01 1601 1701 1801 2101 2601  ............!.&.
+00000790: 2801 2901 2a01 3301 3801 3a01 3b01 3c01  (.).*.3.8.:.;.<.
+000007a0: 4501 4b01 4d01 4e01 4f01 5801 6001 6201  E.K.M.N.O.X.`.b.
+000007b0: 6301 6401 6d01 7601 7901 7a01 7b01 8401  c.d.m.v.y.z.{...
+000007c0: 9301 9501 9601 9701 a001 aa01 ab01 ac01  ................
+000007d0: ad01 b601 c301 cc00 0000 0000 0002 0100  ................
+000007e0: 0000 0000 0000 4a00 0000 0000 0000 0000  ......J.........
+000007f0: 0000 0000 0001 cd00 0000 0c00 7500 6e00  ............u.n.
+00000800: 7300 7500 0000 0001 0000 0000 0000 080b  s.u.............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -713,66 +713,66 @@
 00002c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 00002c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 00002ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 00002cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 00002cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 00002cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 00002ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002cf0: 0054 7369 7a65 556c 6162 656c 546b 696e  .TsizeUlabelTkin
-00002d00: 6457 7665 7273 696f 6e54 6e61 6d65 d416  dWversionTname..
-00002d10: 1718 191a 1b0a 1d57 7669 7369 626c 6555  .......WvisibleU
-00002d20: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
-00002d30: 696e 6465 7808 1101 2c09 1007 d416 1718  index...,.......
-00002d40: 191a 201a 2208 10c8 0810 08d4 1617 1819  .. ."...........
-00002d50: 0a25 1a09 0910 b508 d416 1718 191a 251a  .%............%.
-00002d60: 2a08 0810 02d4 1617 1819 0a2d 1a2f 0910  *..........-./..
-00002d70: 6108 1003 d416 1718 191a 320a 3408 1064  a.........2.4..d
-00002d80: 0910 05d4 1617 1819 0a37 0a39 0910 7309  .........7.9..s.
-00002d90: 1004 d416 1718 191a 3c0a 3e08 104b 0910  ........<.>..K..
-00002da0: 06d4 1617 1819 0a41 0a43 0911 01c7 0910  .......A.C......
-00002db0: 0008 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
-00002dc0: 4d6f 6469 6669 6564 2340 3000 0000 0000  Modified#@0.....
-00002dd0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00002de0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
-00002df0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
-00002e00: 0101 0107 0111 0117 0118 011b 011c 011e  ................
-00002e10: 0127 0128 012a 012b 012d 0136 0137 0139  .'.(.*.+.-.6.7.9
-00002e20: 013a 0143 0144 0145 0147 0150 0151 0153  .:.C.D.E.G.P.Q.S
-00002e30: 0154 0156 015f 0160 0162 0163 0165 016e  .T.V._.`.b.c.e.n
-00002e40: 016f 0171 0172 0174 017d 017e 0180 0181  .o.q.r.t.}.~....
-00002e50: 0183 018c 018d 0190 0191 0193 0194 019d  ................
-00002e60: 01aa 01b3 0000 0000 0000 0201 0000 0000  ................
-00002e70: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-00002e80: 0000 01b4 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-00002e90: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00002ea0: 6d6f 4444 626c 6f62 0000 0008 04d0 54a0  moDDblob......T.
-00002eb0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-00002ec0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00002ed0: 6d6f 6444 626c 6f62 0000 0008 04d0 54a0  modDblob......T.
-00002ee0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-00002ef0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00002f00: 7068 3153 636f 6d70 0000 0000 0009 b000  ph1Scomp........
-00002f10: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
-00002f20: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
-00002f30: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
-00002f40: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
-00002f50: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00002f60: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00002f70: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00002f80: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00002f90: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00002fa0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00002fb0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00002fc0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00002fd0: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
-00002fe0: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-00002ff0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+00002cf0: 0064 5473 697a 6555 6c61 6265 6c54 6b69  .dTsizeUlabelTki
+00002d00: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+00002d10: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
+00002d20: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002d30: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
+00002d40: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
+00002d50: 190a 251a 0909 10b5 08d4 1617 1819 1a25  ..%............%
+00002d60: 1a2a 0808 1002 d416 1718 190a 2d1a 2f09  .*..........-./.
+00002d70: 1061 0810 03d4 1617 1819 1a32 0a34 0810  .a.........2.4..
+00002d80: 6409 1005 d416 1718 190a 370a 3909 1073  d.........7.9..s
+00002d90: 0910 04d4 1617 1819 1a3c 0a3e 0810 4b09  .........<.>..K.
+00002da0: 1006 d416 1718 190a 410a 4309 1101 c709  ........A.C.....
+00002db0: 1000 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
+00002dc0: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
+00002dd0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+00002de0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
+00002df0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
+00002e00: f901 0101 0701 1101 1701 1801 1b01 1c01  ................
+00002e10: 1e01 2701 2801 2a01 2b01 2d01 3601 3701  ..'.(.*.+.-.6.7.
+00002e20: 3901 3a01 4301 4401 4501 4701 5001 5101  9.:.C.D.E.G.P.Q.
+00002e30: 5301 5401 5601 5f01 6001 6201 6301 6501  S.T.V._.`.b.c.e.
+00002e40: 6e01 6f01 7101 7201 7401 7d01 7e01 8001  n.o.q.r.t.}.~...
+00002e50: 8101 8301 8c01 8d01 9001 9101 9301 9401  ................
+00002e60: 9d01 aa01 b300 0000 0000 0002 0100 0000  ................
+00002e70: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
+00002e80: 0000 0001 b400 0000 0c00 7500 6e00 7300  ..........u.n.s.
+00002e90: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+00002ea0: 646d 6f44 4462 6c6f 6200 0000 08e7 da8e  dmoDDblob.......
+00002eb0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
+00002ec0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+00002ed0: 646d 6f64 4462 6c6f 6200 0000 08e7 da8e  dmodDblob.......
+00002ee0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
+00002ef0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+00002f00: 6470 6831 5363 6f6d 7000 0000 0000 02b0  dph1Scomp.......
+00002f10: 0000 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
+00002f20: 6500 7200 7600 6900 7300 6500 6476 5372  e.r.v.i.s.e.dvSr
+00002f30: 6e6c 6f6e 6700 0000 0100 0000 0500 7500  nlong.........u.
+00002f40: 7400 6900 6c00 7362 7773 7062 6c6f 6200  t.i.l.sbwspblob.
+00002f50: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00002f60: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00002f70: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00002f80: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+00002f90: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00002fa0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00002fb0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00002fc0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+00002fd0: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
+00002fe0: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
+00002ff0: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
 00003000: 0000 0101 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0005 fd4d 0000 0005 0075  mp.......M.....u
+00003020: 6d70 0000 0000 0004 22e0 0000 0005 0075  mp......"......u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,142 +848,142 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 08e0 a68e  smoDDblob.......
-00003570: 2eda 09c5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08e0  l.smodDblob.....
-00003590: a27b 4b44 09c5 4100 0000 0500 7500 7400  .{KD..A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 084d 44b7  smoDDblob....MD.
+00003570: 8e43 0dc5 4100 0000 0500 7500 7400 6900  .C..A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 084b  l.smodDblob....K
+00003590: 8540 afbf 0cc5 4100 0000 0500 7500 7400  .@....A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0720 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
+000035b0: 0000 04d0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000035f0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
+000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00003630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00003640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00003650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00003660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00003670: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00003680: 7b7b 3233 322c 2031 3931 7d2c 207b 3133  {{232, 191}, {13
-00003690: 3032 2c20 3731 347d 7d09 0817 2531 3d49  02, 714}}...%1=I
-000036a0: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-000036b0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-000036c0: 0000 0000 0000 0000 9b00 0000 1000 7600  ..............v.
-000036d0: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
-000036e0: 6300 6500 7300 7300 6f00 7200 7364 7363  c.e.s.s.o.r.sdsc
-000036f0: 6c62 6f6f 6c00 0000 0010 0076 0069 0064  lbool......v.i.d
-00003700: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
-00003710: 0073 0073 006f 0072 0073 6c67 3153 636f  .s.s.o.r.slg1Sco
-00003720: 6d70 0000 0000 0004 ee86 0000 0010 0076  mp.............v
-00003730: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
-00003740: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
-00003750: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
-00003760: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
-00003770: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
-00003780: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00003790: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000037a0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-000037b0: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
-000037c0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-000037d0: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
-000037e0: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
-000037f0: ab0c 151d 2226 2b30 353a 3f44 d40d 0e0f  ...."&+05:?D....
-00003800: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
-00003810: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00003820: 5776 6973 6962 6c65 546e 616d 6511 01c7  WvisibleTname...
-00003830: 0909 d416 1718 0d19 1a19 1c57 7669 7369  ...........Wvisi
-00003840: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00003850: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
-00003860: d40d 0e0f 101e 1f19 0a5c 6461 7465 4d6f  .........\dateMo
-00003870: 6469 6669 6564 10b5 0809 d40d 0e0f 1023  dified.........#
-00003880: 1f19 195b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
-00003890: 08d4 0d0e 0f10 2728 190a 5473 697a 6510  ......'(..Tsize.
-000038a0: 6108 09d4 0d0e 0f10 2c2d 0a0a 546b 696e  a.......,-..Tkin
-000038b0: 6410 7309 09d4 0d0e 0f10 3132 0a19 556c  d.s.......12..Ul
-000038c0: 6162 656c 1064 0908 d40d 0e0f 1036 370a  abel.d.......67.
-000038d0: 1957 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
-000038e0: 0f10 3b3c 0a19 5863 6f6d 6d65 6e74 7311  ..;<..Xcomments.
-000038f0: 012c 0908 d40d 0e0f 1040 4119 195e 6461  .,.......@A..^da
-00003900: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
-00003910: d416 1718 0d19 1f19 4708 0859 6461 7465  ........G..Ydate
-00003920: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00003930: 6e61 6d65 0910 0100 0800 1900 2200 3400  name........".4.
-00003940: 3c00 5000 5900 6400 7700 8c00 9500 9600  <.P.Y.d.w.......
-00003950: a200 ab00 b600 bc00 c600 ce00 d300 d600  ................
-00003960: d700 d800 e100 e900 ef00 f900 fa00 fc00  ................
-00003970: fd01 0601 0f01 1c01 1e01 1f01 2001 2901  ............ .).
-00003980: 3501 3601 3701 4001 4501 4701 4801 4901  5.6.7.@.E.G.H.I.
-00003990: 5201 5701 5901 5a01 5b01 6401 6a01 6c01  R.W.Y.Z.[.d.j.l.
-000039a0: 6d01 6e01 7701 7f01 8101 8201 8301 8c01  m.n.w...........
-000039b0: 9501 9801 9901 9a01 a301 b201 b401 b501  ................
-000039c0: b601 bf01 c001 c101 cb01 cc01 d501 da01  ................
-000039d0: db00 0000 0000 0002 0100 0000 0000 0000  ................
-000039e0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
-000039f0: dd00 0000 1000 7600 6900 6400 6500 6f00  ......v.i.d.e.o.
-00003a00: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00003a10: 6f00 7200 736c 7376 7062 6c6f 6200 0002  o.r.slsvpblob...
-00003a20: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
-00003a30: 0708 090a 0b1a 4647 0a44 5869 636f 6e53  ......FG.DXiconS
-00003a40: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-00003a50: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00003a60: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00003a70: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00003a80: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00003a90: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-00003aa0: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-00003ab0: 0000 0000 0000 09d9 0c0d 0e0f 1011 1213  ................
-00003ac0: 1415 1e23 282d 3237 3c41 5863 6f6d 6d65  ...#(-27<AXcomme
-00003ad0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-00003ae0: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00003af0: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00003b00: 6572 7369 6f6e 546e 616d 655c 6461 7465  ersionTname\date
-00003b10: 4d6f 6469 6669 6564 d416 1718 191a 1b0a  Modified........
-00003b20: 1d57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00003b30: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
-00003b40: 1101 2c09 1007 d416 1718 191a 201a 2208  ..,......... .".
-00003b50: 10c8 0810 08d4 1617 1819 1a25 1a27 0810  ...........%.'..
-00003b60: b508 1002 d416 1718 190a 2a1a 2c09 1061  ..........*.,..a
-00003b70: 0810 03d4 1617 1819 1a2f 0a31 0810 6409  ........./.1..d.
-00003b80: 1005 d416 1718 190a 340a 3609 1073 0910  ........4.6..s..
-00003b90: 04d4 1617 1819 1a39 0a3b 0810 4b09 1006  .......9.;..K...
-00003ba0: d416 1718 190a 3e0a 4009 1101 c709 1000  ......>.@.......
-00003bb0: d416 1718 190a 251a 4409 0810 0108 2340  ......%.D.....#@
-00003bc0: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00003bd0: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00003be0: 8c00 9500 9600 a900 b200 c100 cd00 d200  ................
-00003bf0: d800 dd00 e500 ea00 f701 0001 0801 0e01  ................
-00003c00: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-00003c10: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-00003c20: 4c01 4d01 4f01 5001 5201 5b01 5c01 5e01  L.M.O.P.R.[.\.^.
-00003c30: 5f01 6101 6a01 6b01 6d01 6e01 7001 7901  _.a.j.k.m.n.p.y.
-00003c40: 7a01 7c01 7d01 7f01 8801 8901 8c01 8d01  z.|.}...........
-00003c50: 8f01 9801 9901 9a01 9c01 9d01 a601 ab00  ................
-00003c60: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00003c70: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
-00003c80: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00003c90: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00003ca0: 7200 736d 6f44 4462 6c6f 6200 0000 0862  r.smoDDblob....b
-00003cb0: 4b01 eef4 09c5 4100 0000 1000 7600 6900  K.....A.....v.i.
-00003cc0: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
-00003cd0: 6500 7300 7300 6f00 7200 736d 6f64 4462  e.s.s.o.r.smodDb
-00003ce0: 6c6f 6200 0000 08e7 4238 5ea7 08c5 4100  lob.....B8^...A.
-00003cf0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00003d00: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00003d10: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-00003d20: 0620 0000 0000 1000 7600 6900 6400 6500  . ......v.i.d.e.
-00003d30: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
-00003d40: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
-00003d50: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00003670: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
+00003680: 7b7b 3333 352c 2031 3938 7d2c 207b 3932  {{335, 198}, {92
+00003690: 372c 2035 3638 7d7d 0908 1725 313d 4960  7, 568}}...%1=I`
+000036a0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
+000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
+000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
+000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
+000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
+00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
+00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
+00003720: 7000 0000 0000 0315 b900 0000 1000 7600  p.............v.
+00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
+00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
+00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
+00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
+00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
+00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+000037a0: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+000037b0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+000037c0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000037d0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000037e0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
+000037f0: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
+00003800: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+00003810: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+00003820: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
+00003830: 09d4 1617 180d 191a 191c 5776 6973 6962  ..........Wvisib
+00003840: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00003850: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
+00003860: 0d0e 0f10 1e1f 190a 5c64 6174 654d 6f64  ........\dateMod
+00003870: 6966 6965 6410 b508 09d4 0d0e 0f10 231f  ified.........#.
+00003880: 1919 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00003890: d40d 0e0f 1027 2819 0a54 7369 7a65 1061  .....'(..Tsize.a
+000038a0: 0809 d40d 0e0f 102c 2d0a 0a54 6b69 6e64  .......,-..Tkind
+000038b0: 1073 0909 d40d 0e0f 1031 320a 1955 6c61  .s.......12..Ula
+000038c0: 6265 6c10 6409 08d4 0d0e 0f10 3637 0a19  bel.d.......67..
+000038d0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
+000038e0: 103b 3c0a 1958 636f 6d6d 656e 7473 1101  .;<..Xcomments..
+000038f0: 2c09 08d4 0d0e 0f10 4041 1919 5e64 6174  ,.......@A..^dat
+00003900: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+00003910: 1617 180d 191f 1947 0808 5964 6174 6541  .......G..YdateA
+00003920: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
+00003930: 616d 6509 1001 0008 0019 0022 0034 003c  ame........".4.<
+00003940: 0050 0059 0064 0077 008c 0095 0096 00a2  .P.Y.d.w........
+00003950: 00ab 00b6 00bc 00c6 00ce 00d3 00d6 00d7  ................
+00003960: 00d8 00e1 00e9 00ef 00f9 00fa 00fc 00fd  ................
+00003970: 0106 010f 011c 011e 011f 0120 0129 0135  ........... .).5
+00003980: 0136 0137 0140 0145 0147 0148 0149 0152  .6.7.@.E.G.H.I.R
+00003990: 0157 0159 015a 015b 0164 016a 016c 016d  .W.Y.Z.[.d.j.l.m
+000039a0: 016e 0177 017f 0181 0182 0183 018c 0195  .n.w............
+000039b0: 0198 0199 019a 01a3 01b2 01b4 01b5 01b6  ................
+000039c0: 01bf 01c0 01c1 01cb 01cc 01d5 01da 01db  ................
+000039d0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+000039e0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
+000039f0: 0000 0010 0076 0069 0064 0065 006f 005f  .....v.i.d.e.o._
+00003a00: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
+00003a10: 0072 0073 6c73 7670 626c 6f62 0000 025e  .r.slsvpblob...^
+00003a20: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00003a30: 0809 0a0b 1a46 470a 4458 6963 6f6e 5369  .....FG.DXiconSi
+00003a40: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00003a50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00003a60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00003a70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+00003a80: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+00003a90: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+00003aa0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+00003ab0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
+00003ac0: 151e 2328 2d32 373c 4158 636f 6d6d 656e  ..#(-27<AXcommen
+00003ad0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+00003ae0: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
+00003af0: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
+00003b00: 7273 696f 6e54 6e61 6d65 5c64 6174 654d  rsionTname\dateM
+00003b10: 6f64 6966 6965 64d4 1617 1819 1a1b 0a1d  odified.........
+00003b20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00003b30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00003b40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
+00003b50: c808 1008 d416 1718 191a 251a 2708 10b5  ..........%.'...
+00003b60: 0810 02d4 1617 1819 0a2a 1a2c 0910 6108  .........*.,..a.
+00003b70: 1003 d416 1718 191a 2f0a 3108 1064 0910  ......../.1..d..
+00003b80: 05d4 1617 1819 0a34 0a36 0910 7309 1004  .......4.6..s...
+00003b90: d416 1718 191a 390a 3b08 104b 0910 06d4  ......9.;..K....
+00003ba0: 1617 1819 0a3e 0a40 0911 01c7 0910 00d4  .....>.@........
+00003bb0: 1617 1819 0a25 1a44 0908 1001 0823 4028  .....%.D.....#@(
+00003bc0: 0000 0000 0000 546e 616d 6509 0008 0019  ......Tname.....
+00003bd0: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00003be0: 0095 0096 00a9 00b2 00c1 00cd 00d2 00d8  ................
+00003bf0: 00dd 00e5 00ea 00f7 0100 0108 010e 0118  ................
+00003c00: 011e 011f 0122 0123 0125 012e 012f 0131  .....".#.%.../.1
+00003c10: 0132 0134 013d 013e 0140 0141 0143 014c  .2.4.=.>.@.A.C.L
+00003c20: 014d 014f 0150 0152 015b 015c 015e 015f  .M.O.P.R.[.\.^._
+00003c30: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
+00003c40: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
+00003c50: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
+00003c60: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
+00003c70: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
+00003c80: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
+00003c90: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
+00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 85b8  .smoDDblob......
+00003cb0: 5eee cc0c c541 0000 0010 0076 0069 0064  ^....A.....v.i.d
+00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
+00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
+00003ce0: 6f62 0000 0008 85b8 5eee cc0c c541 0000  ob......^....A..
+00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
+00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
+00003d10: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
+00003d20: d000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
+00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
+00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1034,40 +1034,40 @@
 00004090: 006d 0062 0061 005f 0064 0065 0076 002f  .m.b.a._.d.e.v./
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-00004100: 005f 6c67 3153 636f 6d70 0000 0000 003f  ._lg1Scomp.....?
-00004110: e687 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
+00004100: 005f 6c67 3153 636f 6d70 0000 0000 0000  ._lg1Scomp......
+00004110: c6eb 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 b90a 572b b90a c541  blob......W+...A
+00004130: 626c 6f62 0000 0008 a913 1348 cc0c c541  blob.......H...A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 ff8d e56c 4e07 c541 0000  ob.......lN..A..
+00004160: 6f62 0000 0008 a913 1348 cc0c c541 0000  ob.......H...A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
-00004190: 0000 0000 004d c000 0000 0006 0061 0073  .....M.......a.s
+00004190: 0000 0000 0000 e000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
 000041b0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
 000041c0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 000041d0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 000041e0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 000041f0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00004200: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00004210: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00004220: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00004230: 0809 5f10 187b 7b31 3132 2c20 3535 7d2c  .._..{{112, 55},
-00004240: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
+00004230: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
+00004240: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
 00004250: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 00004260: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 00004270: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 00004280: 0600 6100 7300 7300 6500 7400 736c 6731  ..a.s.s.e.t.slg1
-00004290: 5363 6f6d 7000 0000 0000 7ddc 3800 0000  Scomp.....}.8...
+00004290: 5363 6f6d 7000 0000 0000 7ddb 9300 0000  Scomp.....}.....
 000042a0: 0600 6100 7300 7300 6500 7400 736c 7376  ..a.s.s.e.t.slsv
 000042b0: 4362 6c6f 6200 0002 b062 706c 6973 7430  Cblob....bplist0
 000042c0: 30da 0102 0304 0506 0708 090a 0b0c 0d1a  0...............
 000042d0: 4849 484a 0c4c 5869 636f 6e53 697a 655f  HIHJ.LXiconSize_
 000042e0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
 000042f0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
 00004300: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
@@ -1154,28 +1154,28 @@
 00004810: 0000 0000 0000 0000 01dd 0000 0006 0061  ...............a
 00004820: 0073 0073 0065 0074 0073 6d6f 4444 626c  .s.s.e.t.smoDDbl
 00004830: 6f62 0000 0008 cf95 8ce8 d0e1 c441 0000  ob...........A..
 00004840: 0006 0061 0073 0073 0065 0074 0073 6d6f  ...a.s.s.e.t.smo
 00004850: 6444 626c 6f62 0000 0008 cf95 8ce8 d0e1  dDblob..........
 00004860: c441 0000 0006 0061 0073 0073 0065 0074  .A.....a.s.s.e.t
 00004870: 0073 7068 3153 636f 6d70 0000 0000 0081  .sph1Scomp......
-00004880: b000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
+00004880: a000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
 00004890: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 000048a0: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
 000048b0: 006f 0072 0061 0067 0065 6277 7370 626c  .o.r.a.g.ebwspbl
 000048c0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
 000048d0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 000048e0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 000048f0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00004900: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00004910: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00004920: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00004930: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00004940: 0809 0809 5f10 187b 7b35 3139 2c20 3333  ...._..{{519, 33
-00004950: 347d 2c20 7b37 3730 2c20 3433 367d 7d09  4}, {770, 436}}.
+00004940: 0809 0809 5f10 187b 7b33 3335 2c20 3139  ...._..{{335, 19
+00004950: 387d 2c20 7b39 3237 2c20 3536 387d 7d09  8}, {927, 568}}.
 00004960: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 00004970: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 00004980: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 00004990: 0000 0c00 6200 6c00 6f00 6200 5f00 7300  ....b.l.o.b._.s.
 000049a0: 7400 6f00 7200 6100 6700 656c 6731 5363  t.o.r.a.g.elg1Sc
 000049b0: 6f6d 7000 0000 0000 0018 0400 0000 0c00  omp.............
 000049c0: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
@@ -1188,77 +1188,77 @@
 00004a30: 7200 6100 6700 6570 6831 5363 6f6d 7000  r.a.g.eph1Scomp.
 00004a40: 0000 0000 0020 0000 0000 0c00 6200 6c00  ..... ......b.l.
 00004a50: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
 00004a60: 6700 6576 5372 6e6c 6f6e 6700 0000 0100  g.evSrnlong.....
 00004a70: 0000 1200 6200 6f00 7500 6e00 6400 6900  ....b.o.u.n.d.i.
 00004a80: 6e00 6700 5f00 6200 6f00 7800 5f00 7400  n.g._.b.o.x._.t.
 00004a90: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
-00004aa0: 0000 c862 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00004aa0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 00004ab0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00004ac0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
 00004ad0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
 00004ae0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00004af0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00004b00: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00004b10: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00004b20: 095f 1017 7b7b 3932 2c20 3735 7d2c 207b  ._..{{92, 75}, {
-00004b30: 3131 3939 2c20 3736 397d 7d09 0817 2531  1199, 769}}...%1
-00004b40: 3d49 606d 797a 7b7c 7d7e 9800 0000 0000  =I`myz{|}~......
-00004b50: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
-00004b60: 0000 0000 0000 0000 0000 9900 0000 1200  ................
-00004b70: 6200 6f00 7500 6e00 6400 6900 6e00 6700  b.o.u.n.d.i.n.g.
-00004b80: 5f00 6200 6f00 7800 5f00 7400 6f00 6f00  _.b.o.x._.t.o.o.
-00004b90: 6c00 7364 7363 6c62 6f6f 6c00 0000 0012  l.sdsclbool.....
-00004ba0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-00004bb0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-00004bc0: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00004bd0: 0003 1734 0000 0012 0062 006f 0075 006e  ...4.....b.o.u.n
-00004be0: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
-00004bf0: 005f 0074 006f 006f 006c 0073 6c73 7643  ._.t.o.o.l.slsvC
-00004c00: 626c 6f62 0000 0279 6270 6c69 7374 3030  blob...ybplist00
-00004c10: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
-00004c20: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-00004c30: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00004c40: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00004c50: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00004c60: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00004c70: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-00004c80: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-00004c90: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
-00004ca0: 373c 41d4 0d0e 0f10 0a12 0a14 5776 6973  7<A.........Wvis
-00004cb0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-00004cc0: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
-00004cd0: 1101 c709 546e 616d 65d4 0d0e 0f10 1617  ....Tname.......
-00004ce0: 1619 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
-00004cf0: 0d0e 0f10 0a1c 161e 0910 b508 5c64 6174  ............\dat
-00004d00: 654d 6f64 6966 6965 64d4 0d0e 0f10 161c  eModified.......
-00004d10: 1622 0808 5b64 6174 6543 7265 6174 6564  ."..[dateCreated
-00004d20: d40d 0e0f 100a 2516 2709 1061 0854 7369  ......%.'..a.Tsi
-00004d30: 7a65 d40d 0e0f 100a 2a0a 2c09 1073 0954  ze......*.,..s.T
-00004d40: 6b69 6e64 d40d 0e0f 1016 2f0a 3108 1064  kind....../.1..d
-00004d50: 0955 6c61 6265 6cd4 0d0e 0f10 1634 0a36  .Ulabel......4.6
-00004d60: 0810 4b09 5776 6572 7369 6f6e d40d 0e0f  ..K.Wversion....
-00004d70: 1016 390a 3b08 1101 2c09 5863 6f6d 6d65  ..9.;...,.Xcomme
-00004d80: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
-00004d90: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
-00004da0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
-00004db0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
-00004dc0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-00004dd0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-00004de0: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
-00004df0: c700 c800 cb00 cc00 d100 da00 db00 dd00  ................
-00004e00: de00 e700 f000 f100 f300 f401 0101 0a01  ................
-00004e10: 0b01 0c01 1801 2101 2201 2401 2501 2a01  ......!.".$.%.*.
-00004e20: 3301 3401 3601 3701 3c01 4501 4601 4801  3.4.6.7.<.E.F.H.
-00004e30: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
-00004e40: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
-00004e50: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
-00004e60: c400 0000 0000 0002 0100 0000 0000 0000  ................
-00004e70: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-00004e80: c500 0000 0000 0000 0000 0000 0000 0000  ................
+00004b20: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
+00004b30: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
+00004b40: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
+00004b50: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00004b60: 0000 0000 0000 0000 0000 009a 0000 0012  ................
+00004b70: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
+00004b80: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
+00004b90: 006c 0073 6473 636c 626f 6f6c 0000 0000  .l.sdsclbool....
+00004ba0: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
+00004bb0: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
+00004bc0: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
+00004bd0: 0000 019d 6000 0000 1200 6200 6f00 7500  ....`.....b.o.u.
+00004be0: 6e00 6400 6900 6e00 6700 5f00 6200 6f00  n.d.i.n.g._.b.o.
+00004bf0: 7800 5f00 7400 6f00 6f00 6c00 736c 7376  x._.t.o.o.l.slsv
+00004c00: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
+00004c10: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
+00004c20: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
+00004c30: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00004c40: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00004c50: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00004c60: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+00004c70: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00004c80: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+00004c90: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
+00004ca0: 3237 3c41 d40d 0e0f 100a 120a 1457 7669  27<A.........Wvi
+00004cb0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00004cc0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
+00004cd0: 0911 01c7 0954 6e61 6d65 d40d 0e0f 1016  .....Tname......
+00004ce0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+00004cf0: d40d 0e0f 100a 1c16 1e09 10b5 085c 6461  .............\da
+00004d00: 7465 4d6f 6469 6669 6564 d40d 0e0f 1016  teModified......
+00004d10: 1c16 2208 085b 6461 7465 4372 6561 7465  .."..[dateCreate
+00004d20: 64d4 0d0e 0f10 0a25 1627 0910 6108 5473  d......%.'..a.Ts
+00004d30: 697a 65d4 0d0e 0f10 0a2a 0a2c 0910 7309  ize......*.,..s.
+00004d40: 546b 696e 64d4 0d0e 0f10 162f 0a31 0810  Tkind....../.1..
+00004d50: 6409 556c 6162 656c d40d 0e0f 1016 340a  d.Ulabel......4.
+00004d60: 3608 104b 0957 7665 7273 696f 6ed4 0d0e  6..K.Wversion...
+00004d70: 0f10 1639 0a3b 0811 012c 0958 636f 6d6d  ...9.;...,.Xcomm
+00004d80: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
+00004d90: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+00004da0: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
+00004db0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00004dc0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00004dd0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
+00004de0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
+00004df0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
+00004e00: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
+00004e10: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
+00004e20: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
+00004e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
+00004e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00004e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00004e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00004e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00004e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
 00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1278,71 +1278,71 @@
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 001d 0000 0012  ................
 00005010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 00005020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 00005030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-00005040: 1fe8 e082 4c09 c541 0000 0012 0062 006f  ....L..A.....b.o
+00005040: 1799 b1f1 cc0c c541 0000 0012 0062 006f  .......A.....b.o
 00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-00005070: 6d6f 6444 626c 6f62 0000 0008 1fe8 e082  modDblob........
-00005080: 4c09 c541 0000 0012 0062 006f 0075 006e  L..A.....b.o.u.n
+00005070: 6d6f 6444 626c 6f62 0000 0008 1799 b1f1  modDblob........
+00005080: cc0c c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
 00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
 000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000050b0: 636f 6d70 0000 0000 0003 c000 0000 0012  comp............
+000050b0: 636f 6d70 0000 0000 0001 f000 0000 0012  comp............
 000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 00005100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
 00005110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
 00005120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
 00005130: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00005140: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
 00005150: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 00005160: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 00005170: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 00005180: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 00005190: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-000051a0: 7b33 3934 2c20 3138 317d 2c20 7b37 3730  {394, 181}, {770
-000051b0: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
+000051a0: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+000051b0: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 000051c0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 000051d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 000051e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
 000051f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
 00005200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
 00005210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
 00005220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00005240: 0002 996a 0000 000f 0063 0075 0065 005f  ...j.....c.u.e._
+00005240: 0001 da29 0000 000f 0063 0075 0065 005f  ...).....c.u.e._
 00005250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
 00005260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
-00005270: 0008 40f3 04c6 030a c541 0000 000f 0063  ..@......A.....c
+00005270: 0008 00ae d77f cc0c c541 0000 000f 0063  .........A.....c
 00005280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
 00005290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-000052a0: 626c 6f62 0000 0008 d824 2d67 9605 c541  blob.....$-g...A
+000052a0: 626c 6f62 0000 0008 00ae d77f cc0c c541  blob...........A
 000052b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 000052c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-000052d0: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
-000052e0: 7000 0000 000f 0063 0075 0065 005f 006c  p......c.u.e._.l
+000052d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
+000052e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
 000052f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00005310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
 00005320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
 00005330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00005340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00005350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
 00005360: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00005370: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00005380: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00005390: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 000053a0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-000053b0: 187b 7b36 3537 2c20 3237 307d 2c20 7b39  .{{657, 270}, {9
-000053c0: 3839 2c20 3433 367d 7d09 0817 2531 3d49  89, 436}}...%1=I
+000053b0: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
+000053c0: 3237 2c20 3536 387d 7d09 0817 2531 3d49  27, 568}}...%1=I
 000053d0: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
 000053e0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000053f0: 0000 0000 0000 0000 9a00 0000 0800 6400  ..............d.
 00005400: 6100 7300 6800 5f00 6100 7000 706c 6731  a.s.h._.a.p.plg1
 00005410: 5363 6f6d 7000 0000 0000 0135 6200 0000  Scomp......5b...
 00005420: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
 00005430: 706d 6f44 4462 6c6f 6200 0000 087e 81a5  pmoDDblob....~..
@@ -1370,15 +1370,15 @@
 00005590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000055a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
 000055b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 000055c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
 000055d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
 000055e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000055f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-00005600: 0000 0459 f000 0000 0f00 6400 6100 7400  ...Y......d.a.t.
+00005600: 0000 032d 2c00 0000 0f00 6400 6100 7400  ...-,.....d.a.t.
 00005610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005620: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
 00005630: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
 00005640: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
 00005650: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
 00005660: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
 00005670: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
@@ -1457,22 +1457,22 @@
 00005b00: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
 00005b10: 0180 0181 0183 018c 018d 0190 0191 0193  ................
 00005b20: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
 00005b30: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
 00005b40: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
 00005b50: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 00005b60: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00005b70: 6f62 0000 0008 10ae 0e75 fb0b c541 0000  ob.......u...A..
+00005b70: 6f62 0000 0008 abe0 caed cc0c c541 0000  ob...........A..
 00005b80: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
 00005b90: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
-00005ba0: 6d6f 6444 626c 6f62 0000 0008 10ae 0e75  modDblob.......u
-00005bb0: fb0b c541 0000 000f 0064 0061 0074 0061  ...A.....d.a.t.a
+00005ba0: 6d6f 6444 626c 6f62 0000 0008 abe0 caed  modDblob........
+00005bb0: cc0c c541 0000 000f 0064 0061 0074 0061  ...A.....d.a.t.a
 00005bc0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00005bd0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
-00005be0: 0000 0005 b000 0000 000f 0064 0061 0074  ...........d.a.t
+00005be0: 0000 0004 1000 0000 000f 0064 0061 0074  ...........d.a.t
 00005bf0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005c00: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
 00005c10: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
 00005c20: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 00005c30: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
 00005c40: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
 00005c50: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
@@ -1489,32 +1489,32 @@
 00005d00: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 9a00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00005d20: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00005d30: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00005d40: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00005d50: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d60: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d70: 6d70 0000 0000 0016 34fb 5863 6f6d 6d65  mp......4.Xcomme
-00005d80: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
-00005d90: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
-00005da0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
-00005db0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
-00005dc0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-00005dd0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-00005de0: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
-00005df0: c700 c800 cb00 cc00 d100 da00 db00 dd00  ................
-00005e00: de00 e700 f000 f100 f300 f401 0101 0a01  ................
-00005e10: 0b01 0c01 1801 2101 2201 2401 2501 2a01  ......!.".$.%.*.
-00005e20: 3301 3401 3601 3701 3c01 4501 4601 4801  3.4.6.7.<.E.F.H.
-00005e30: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
-00005e40: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
-00005e50: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
-00005e60: c400 0000 0000 0002 0100 0000 0000 0000  ................
-00005e70: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-00005e80: c500 0000 0000 0000 0000 0000 0000 0000  ................
+00005d70: 6d70 0000 0000 0008 ae3a 0958 636f 6d6d  mp.......:.Xcomm
+00005d80: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
+00005d90: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+00005da0: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
+00005db0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00005dc0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00005dd0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
+00005de0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
+00005df0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
+00005e00: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
+00005e10: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
+00005e20: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
+00005e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
+00005e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00005e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00005e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00005e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00005e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
 00005e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1579,22 +1579,22 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 086f ba2a 3a04 0cc5 4100 0000 1200 6600  .o.*:...A.....f.
+00006310: 0869 3ef0 203f 0dc5 4100 0000 1200 6600  .i>. ?..A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 086f ba2a  smodDblob....o.*
-00006350: 3a04 0cc5 4100 0000 1200 6600 6500 6100  :...A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 08cc d9f8  smodDblob.......
+00006350: 15cc 0cc5 4100 0000 1200 6600 6500 6100  ....A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 1900 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0a90 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -1606,16 +1606,16 @@
 00006450: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
 00006460: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
 00006470: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
 00006480: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
 00006490: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 000064a0: 0000 0000 0000 0000 0000 009a 0000 0009  ................
 000064b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0002  .glg1Scomp......
-000064d0: 416b 0000 0009 006c 0061 0062 0065 006c  Ak.....l.a.b.e.l
+000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0001  .glg1Scomp......
+000064d0: 8eb7 0000 0009 006c 0061 0062 0065 006c  .......l.a.b.e.l
 000064e0: 006c 0069 006e 0067 6c73 7643 626c 6f62  .l.i.n.glsvCblob
 000064f0: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
 00006500: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00006510: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00006520: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00006530: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00006540: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -1690,21 +1690,21 @@
 00006990: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
 000069a0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
 000069b0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
 000069c0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
 000069d0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 000069e0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000069f0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 0855  n.gmoDDblob....U
-00006a10: a5c5 4cc9 0bc5 4100 0000 0900 6c00 6100  ..L...A.....l.a.
+00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 08ed  n.gmoDDblob.....
+00006a10: 41b1 f1cc 0cc5 4100 0000 0900 6c00 6100  A.....A.....l.a.
 00006a20: 6200 6500 6c00 6c00 6900 6e00 676d 6f64  b.e.l.l.i.n.gmod
-00006a30: 4462 6c6f 6200 0000 0855 a5c5 4cc9 0bc5  Dblob....U..L...
+00006a30: 4462 6c6f 6200 0000 08ed 41b1 f1cc 0cc5  Dblob.....A.....
 00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
 00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
-00006a60: 0000 0000 02a0 0000 0000 0900 6c00 6100  ............l.a.
+00006a60: 0000 0000 01d0 0000 0000 0900 6c00 6100  ............l.a.
 00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
 00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
 00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
 00006aa0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
 00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
@@ -1714,15 +1714,15 @@
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
 00006b20: 0908 095f 1018 7b7b 3333 352c 2031 3938  ..._..{{335, 198
 00006b30: 7d2c 207b 3932 372c 2035 3638 7d7d 0908  }, {927, 568}}..
 00006b40: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
 00006b50: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 00006b60: 0000 0000 0000 0000 0000 0000 009a 0000  ................
 00006b70: 0006 006d 0069 0078 0069 006e 0073 6c67  ...m.i.x.i.n.slg
-00006b80: 3153 636f 6d70 0000 0000 0010 6f38 0000  1Scomp......o8..
+00006b80: 3153 636f 6d70 0000 0000 0007 e2f9 0000  1Scomp..........
 00006b90: 0006 006d 0069 0078 0069 006e 0073 6c73  ...m.i.x.i.n.sls
 00006ba0: 7643 626c 6f62 0000 0281 6270 6c69 7374  vCblob....bplist
 00006bb0: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
 00006bc0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
 00006bd0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 00006be0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 00006bf0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -1756,21 +1756,21 @@
 00006db0: fd00 ff01 0001 0101 0a01 1601 1701 1801  ................
 00006dc0: 2101 2601 2801 2901 2a01 3301 3801 3a01  !.&.(.).*.3.8.:.
 00006dd0: 3b01 3c01 4501 4b01 4d01 4e01 4f01 5801  ;.<.E.K.M.N.O.X.
 00006de0: 6001 6201 6301 6401 6d01 7601 7901 7a01  `.b.c.d.m.v.y.z.
 00006df0: 7b01 8401 9301 9501 9601 9701 a001 a101  {...............
 00006e00: a201 ac01 ad01 b601 c301 cc00 0000 0000  ................
 00006e10: 0002 0100 0000 0000 0000 4a00 0000 0000  ..........J.....
-00006e20: 0000 0000 0000 0000 0001 cd01 4601 4801  ............F.H.
-00006e30: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
-00006e40: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
-00006e50: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
-00006e60: c400 0000 0000 0002 0100 0000 0000 0000  ................
-00006e70: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-00006e80: c500 0000 0000 0000 0000 0000 0000 0000  ................
+00006e20: 0000 0000 0000 0000 0001 cd45 0146 0148  ...........E.F.H
+00006e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
+00006e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00006e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00006e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00006e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00006e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 30ce 1923 0f0c c541  blob....0..#...A
+00007020: 626c 6f62 0000 0008 5404 fa15 cc0c c541  blob....T......A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 30ce 1923  modDblob....0..#
-00007050: 0f0c c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 5404 fa15  modDblob....T...
+00007050: cc0c c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0011 e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0008 9000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3335  bar....._..{{335
 00007130: 2c20 3139 387d 2c20 7b39 3237 2c20 3536  , 198}, {927, 56
 00007140: 387d 7d09 0817 2531 3d49 606d 797a 7b7c  8}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 017c  llg1Scomp......|
-00007190: 0100 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 012c  llg1Scomp......,
+00007190: b200 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1893,19 +1893,19 @@
 00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
 00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
 00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
 00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
-000076b0: 6f62 0000 0008 7e87 fcf0 c80b c541 0000  ob....~......A..
+000076b0: 6f62 0000 0008 32f5 d3ed cc0c c541 0000  ob....2......A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
-000076d0: 626c 6f62 0000 0008 7e87 fcf0 c80b c541  blob....~......A
+000076d0: 626c 6f62 0000 0008 32f5 d3ed cc0c c541  blob....2......A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
-000076f0: 3153 636f 6d70 0000 0000 0001 c000 0000  1Scomp..........
+000076f0: 3153 636f 6d70 0000 0000 0001 6000 0000  1Scomp......`...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
 00007740: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
@@ -1917,15 +1917,15 @@
 000077c0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000077d0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000077e0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000077f0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 00007800: 0000 0000 0000 0000 0000 9a00 0000 0d00  ................
 00007810: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
 00007820: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
-00007830: 7000 0000 0000 0159 9a00 0000 0d00 6f00  p......Y......o.
+00007830: 7000 0000 0000 00bd b900 0000 0d00 6f00  p.............o.
 00007840: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00007850: 6f00 6f00 6c00 736c 7376 4362 6c6f 6200  o.o.l.slsvCblob.
 00007860: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
 00007870: 0506 0708 090a 0b0c 0d18 4849 484a 0c4c  ..........HIHJ.L
 00007880: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 00007890: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
 000078a0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
@@ -2009,22 +2009,22 @@
 00007d80: 0187 0189 018b 018c 018d 0196 0198 019a  ................
 00007d90: 019b 019c 01a5 01a7 01a9 01aa 01ab 01b4  ................
 00007da0: 01b5 01b8 01b9 01bb 01bc 01c5 01ce 01d3  ................
 00007db0: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
 00007dc0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
 00007dd0: 01dd 0000 000d 006f 0075 0074 006c 0069  .......o.u.t.l.i
 00007de0: 0065 0072 005f 0074 006f 006f 006c 0073  .e.r._.t.o.o.l.s
-00007df0: 6d6f 4444 626c 6f62 0000 0008 e309 3e65  moDDblob......>e
-00007e00: fc0b c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
+00007df0: 6d6f 4444 626c 6f62 0000 0008 bea6 cfed  moDDblob........
+00007e00: cc0c c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
 00007e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00007e20: 0073 6d6f 6444 626c 6f62 0000 0008 e309  .smodDblob......
-00007e30: 3e65 fc0b c541 0000 000d 006f 0075 0074  >e...A.....o.u.t
+00007e20: 0073 6d6f 6444 626c 6f62 0000 0008 bea6  .smodDblob......
+00007e30: cfed cc0c c541 0000 000d 006f 0075 0074  .....A.....o.u.t
 00007e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00007e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
-00007e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00007e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
 00007e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
 00007e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 00007e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
 00007ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
 00007eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
 00007ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00007ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
@@ -2035,15 +2035,15 @@
 00007f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
 00007f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
 00007f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 00007f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 00007f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00007f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
 00007f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00007f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
+00007f90: 6f6d 7000 0000 0000 08bf a500 0000 0000  omp.............
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,20 +2088,20 @@
 00008270: 7901 7b01 7d01 7e01 7f01 8801 8a01 8c01  y.{.}.~.........
 00008280: 8d01 8e01 9701 9901 9b01 9c01 9d01 a601  ................
 00008290: a801 aa01 ab01 ac01 b501 b701 ba01 bb01  ................
 000082a0: bc01 bd01 c601 cf01 dc00 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 08d6 95ef 57e4 0bc5  Dblob.......W...
+000082e0: 4462 6c6f 6200 0000 08dc f782 48cc 0cc5  Dblob.......H...
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 08d6 95ef 57e4 0bc5 4100 0000 0800 7000  ....W...A.....p.
+00008310: 08dc f782 48cc 0cc5 4100 0000 0800 7000  ....H...A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
-00008330: 5363 6f6d 7000 0000 0000 0fb0 0000 0000  Scomp...........
+00008330: 5363 6f6d 7000 0000 0000 0ae0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
 00008390: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000083a0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -2264,23 +2264,23 @@
 00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
 00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 03f6 c75f 0074 006f 006f 006c 0073  ....._.t.o.o.l.s
-00008df0: 6d6f 4444 626c 6f62 0000 0008 e309 3e65  moDDblob......>e
-00008e00: fc0b c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
+00008de0: 0000 020c 7a5f 0074 006f 006f 006c 0073  ....z_.t.o.o.l.s
+00008df0: 6d6f 4444 626c 6f62 0000 0008 bea6 cfed  moDDblob........
+00008e00: cc0c c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
 00008e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00008e20: 0073 6d6f 6444 626c 6f62 0000 0008 e309  .smodDblob......
-00008e30: 3e65 fc0b c541 0000 000d 006f 0075 0074  >e...A.....o.u.t
+00008e20: 0073 6d6f 6444 626c 6f62 0000 0008 bea6  .smodDblob......
+00008e30: cfed cc0c c541 0000 000d 006f 0075 0074  .....A.....o.u.t
 00008e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00008e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
-00008e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00008e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
 00008e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
 00008e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 00008e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
 00008ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
 00008eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
 00008ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00008ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
@@ -2291,15 +2291,15 @@
 00008f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
 00008f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
 00008f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 00008f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 00008f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00008f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
 00008f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00008f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
+00008f90: 6f6d 7000 0000 0000 08bf a500 0000 0000  omp.............
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2342,22 +2342,22 @@
 00009250: 0160 0162 0163 0165 016e 016f 0171 0172  .`.b.c.e.n.o.q.r
 00009260: 0174 017d 017e 0180 0181 0183 018c 018d  .t.}.~..........
 00009270: 0190 0191 0193 0194 019d 01aa 01b3 0000  ................
 00009280: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00009290: 0000 0000 0000 0000 0000 0000 01b4 0000  ................
 000092a0: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
 000092b0: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-000092c0: 4444 626c 6f62 0000 0008 487a 6cbc b80a  DDblob....Hzl...
+000092c0: 4444 626c 6f62 0000 0008 23bd 51ed cc0c  DDblob....#.Q...
 000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
-000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 eacd  .smodDblob......
-00009300: db43 ad08 c541 0000 000e 0070 006f 0073  .C...A.....p.o.s
+000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 23bd  .smodDblob....#.
+00009300: 51ed cc0c c541 0000 000e 0070 006f 0073  Q....A.....p.o.s
 00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00009330: 0000 0004 f000 0000 000e 0070 006f 0073  ...........p.o.s
+00009330: 0000 0002 8000 0000 000e 0070 006f 0073  ...........p.o.s
 00009340: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009350: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
 00009360: 0001 0000 000f 0070 006f 0073 0065 005f  .......p.o.s.e._
 00009370: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
 00009380: 0072 0073 6277 7370 626c 6f62 0000 00ca  .r.sbwspblob....
 00009390: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 000093a0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
@@ -2370,15 +2370,15 @@
 00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
 00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
 00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00009480: 636f 6d70 0000 0000 0000 d9d3 0000 000f  comp............
+00009480: 636f 6d70 0000 0000 0000 84af 0000 000f  comp............
 00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
 000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -2458,22 +2458,22 @@
 00009990: 6101 6a01 6b01 6d01 6e01 7001 7901 7a01  a.j.k.m.n.p.y.z.
 000099a0: 7c01 7d01 7f01 8801 8901 8c01 8d01 8f01  |.}.............
 000099b0: 9801 9901 9a01 9c01 9d01 a601 ab00 0000  ................
 000099c0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 000099d0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000099e0: 0f00 7000 6f00 7300 6500 5f00 7000 7200  ..p.o.s.e._.p.r.
 000099f0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
-00009a00: 6f44 4462 6c6f 6200 0000 08f1 8082 0e4e  oDDblob........N
-00009a10: 09c5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
+00009a00: 6f44 4462 6c6f 6200 0000 08e3 bf98 f1cc  oDDblob.........
+00009a10: 0cc5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
 00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
-00009a40: 0892 deca 6739 05c5 4100 0000 0f00 7000  ....g9..A.....p.
+00009a40: 08e3 bf98 f1cc 0cc5 4100 0000 0f00 7000  ........A.....p.
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
-00009a70: 6f6d 7000 0000 0000 0180 0000 0000 0f00  omp.............
+00009a70: 6f6d 7000 0000 0000 00e0 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
 00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 05e0 ab00 0000 0900  omp.............
+00009bb0: 6f6d 7000 0000 0000 042b 2400 0000 0900  omp......+$.....
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2528,15 +2528,15 @@
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
 00009e50: 0000 0000 01c5 3153 636f 6d70 0000 0000  ......1Scomp....
-00009e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00009e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
 00009e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
 00009e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
 00009e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
 00009ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
 00009eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
 00009ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00009ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
@@ -2547,527 +2547,527 @@
 00009f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
 00009f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
 00009f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 00009f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 00009f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00009f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
 00009f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00009f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
+00009f90: 6f6d 7000 0000 0000 08bf a500 0000 0000  omp.............
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
-0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 ed0d  .smoDDblob......
-0000a030: fc73 dd09 c541 0000 0009 0072 006f 0069  .s...A.....r.o.i
+0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 d6ea  .smoDDblob......
+0000a030: 0380 cc0c c541 0000 0009 0072 006f 0069  .....A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-0000a050: 626c 6f62 0000 0008 6cfb e0c5 4905 c541  blob....l...I..A
+0000a050: 626c 6f62 0000 0008 d6ea 0380 cc0c c541  blob...........A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-0000a080: 0000 0007 6000 0000 0009 0072 006f 0069  ....`......r.o.i
+0000a080: 0000 0005 1000 0000 0009 0072 006f 0069  ...........r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
 0000a0b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
 0000a0c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
 0000a0d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-0000a0e0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+0000a0e0: 0073 6277 7370 626c 6f62 0000 00ca 6270  .sbwspblob....bp
 0000a0f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
 0000a100: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
 0000a110: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
 0000a120: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 0000a130: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 0000a140: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 0000a150: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-0000a160: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-0000a170: 7b33 322c 2031 3233 7d2c 207b 3132 3033  {32, 123}, {1203
-0000a180: 2c20 3735 347d 7d09 0817 2531 3d49 606d  , 754}}...%1=I`m
-0000a190: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-0000a1a0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-0000a1b0: 0000 0000 0000 9a00 0000 1b00 7400 6800  ............t.h.
-0000a1c0: 6900 7200 6400 5f00 7000 6100 7200 7400  i.r.d._.p.a.r.t.
-0000a1d0: 7900 5f00 6c00 6100 6200 6500 6c00 5f00  y._.l.a.b.e.l._.
-0000a1e0: 6100 7000 7000 6500 6e00 6400 6500 7200  a.p.p.e.n.d.e.r.
-0000a1f0: 736c 6731 5363 6f6d 7000 0000 0000 02fc  slg1Scomp.......
-0000a200: 1500 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
-0000a210: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
-0000a220: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
-0000a230: 6500 6e00 6400 6500 7200 736c 7376 4362  e.n.d.e.r.slsvCb
-0000a240: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
-0000a250: 0102 0304 0506 0708 090a 0b16 4647 480a  ............FGH.
-0000a260: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-0000a270: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-0000a280: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-0000a290: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-0000a2a0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-0000a2b0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
-0000a2c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-0000a2d0: 7465 7310 0109 ab0c 151a 1f23 282d 3237  tes........#(-27
-0000a2e0: 3c41 d40d 0e0f 100a 120a 1457 7669 7369  <A.........Wvisi
-0000a2f0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-0000a300: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
-0000a310: 01a6 0954 6e61 6d65 d40d 0e0f 1016 1716  ...Tname........
-0000a320: 1908 1023 0858 7562 6971 7569 7479 d40d  ...#.Xubiquity..
-0000a330: 0e0f 100a 1c16 1e09 10b5 085c 6461 7465  ...........\date
-0000a340: 4d6f 6469 6669 6564 d40d 0e0f 1016 1c16  Modified........
-0000a350: 2208 085b 6461 7465 4372 6561 7465 64d4  "..[dateCreated.
-0000a360: 0d0e 0f10 0a25 1627 0910 6108 5473 697a  .....%.'..a.Tsiz
-0000a370: 65d4 0d0e 0f10 0a2a 0a2c 0910 7309 546b  e......*.,..s.Tk
-0000a380: 696e 64d4 0d0e 0f10 162f 0a31 0810 6409  ind....../.1..d.
-0000a390: 556c 6162 656c d40d 0e0f 1016 340a 3608  Ulabel......4.6.
-0000a3a0: 104b 0957 7665 7273 696f 6ed4 0d0e 0f10  .K.Wversion.....
-0000a3b0: 1639 0a3b 0811 012c 0958 636f 6d6d 656e  .9.;...,.Xcommen
-0000a3c0: 7473 d40d 0e0f 1016 3e16 4008 10c8 085e  ts......>.@....^
-0000a3d0: 6461 7465 4c61 7374 4f70 656e 6564 d40d  dateLastOpened..
-0000a3e0: 0e0f 1016 1c16 4408 0859 6461 7465 4164  ......D..YdateAd
-0000a3f0: 6465 6408 2340 2800 0000 0000 0054 6e61  ded.#@(......Tna
-0000a400: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
-0000a410: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
-0000a420: 008e 008f 009b 00a4 00ac 00b2 00bc 00c7  ................
-0000a430: 00c8 00cb 00cc 00d1 00da 00db 00dd 00de  ................
-0000a440: 00e7 00f0 00f1 00f3 00f4 0101 010a 010b  ................
-0000a450: 010c 0118 0121 0122 0124 0125 012a 0133  .....!.".$.%.*.3
-0000a460: 0134 0136 0137 013c 0145 0146 0148 0149  .4.6.7.<.E.F.H.I
-0000a470: 014f 0158 0159 015b 015c 0164 016d 016e  .O.X.Y.[.\.d.m.n
-0000a480: 0171 0172 017b 0184 0185 0187 0188 0197  .q.r.{..........
-0000a490: 01a0 01a1 01a2 01ac 01ad 01b6 01bb 01c4  ................
-0000a4a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-0000a4b0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-0000a4c0: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
-0000a4d0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
-0000a4e0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-0000a4f0: 006e 0064 0065 0072 0073 6c73 7670 626c  .n.d.e.r.slsvpbl
-0000a500: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
-0000a510: 0203 0405 0607 0809 0a0b 1d45 4647 0a5f  ...........EFG._
-0000a520: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-0000a530: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-0000a540: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-0000a550: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-0000a560: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-0000a570: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-0000a580: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-0000a590: 6573 1001 09d9 0c0d 0e0f 1011 1213 1415  es..............
-0000a5a0: 1e23 272b 3035 3a3f 5863 6f6d 6d65 6e74  .#'+05:?Xcomment
-0000a5b0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-0000a5c0: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-0000a5d0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-0000a5e0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-0000a5f0: 6e54 6e61 6d65 d416 1718 191a 1b0a 1d55  nTname.........U
-0000a600: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
-0000a610: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
-0000a620: 012c 0908 d416 1718 191f 201d 1d10 0810  .,........ .....
-0000a630: c808 08d4 1617 1819 0924 1d0a 10b5 0809  .........$......
-0000a640: d416 1718 1928 241d 1d10 0208 08d4 1617  .....($.........
-0000a650: 1819 2c2d 1d0a 1003 1061 0809 d416 1718  ..,-.....a......
-0000a660: 1931 320a 1d10 0510 6409 08d4 1617 1819  .12.....d.......
-0000a670: 3637 0a0a 1004 1073 0909 d416 1718 193b  67.....s.......;
-0000a680: 3c0a 1d10 0610 4b09 08d4 1617 1819 4041  <.....K.......@A
-0000a690: 0a0a 1000 1101 a609 0908 2340 2800 0000  ..........#@(...
-0000a6a0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-0000a6b0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-0000a6c0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
-0000a6d0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
-0000a6e0: 00ff 0105 010f 0117 0119 011c 011d 011e  ................
-0000a6f0: 0127 0129 012b 012c 012d 0136 0138 0139  .'.).+.,.-.6.8.9
-0000a700: 013a 0143 0145 0146 0147 0150 0152 0154  .:.C.E.F.G.P.R.T
-0000a710: 0155 0156 015f 0161 0163 0164 0165 016e  .U.V._.a.c.d.e.n
-0000a720: 0170 0172 0173 0174 017d 017f 0181 0182  .p.r.s.t.}......
-0000a730: 0183 018c 018e 0191 0192 0193 0194 019d  ................
-0000a740: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
-0000a750: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-0000a760: 0000 01ac 0000 001b 0074 0068 0069 0072  .........t.h.i.r
-0000a770: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
-0000a780: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
-0000a790: 0070 0065 006e 0064 0065 0072 0073 6d6f  .p.e.n.d.e.r.smo
-0000a7a0: 4444 626c 6f62 0000 0008 b6c2 e7a3 5009  DDblob........P.
-0000a7b0: c541 0000 001b 0074 0068 0069 0072 0064  .A.....t.h.i.r.d
-0000a7c0: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
-0000a7d0: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
-0000a7e0: 0065 006e 0064 0065 0072 0073 6d6f 6444  .e.n.d.e.r.smodD
-0000a7f0: 626c 6f62 0000 0008 b989 9f32 1302 c541  blob.......2...A
-0000a800: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
-0000a810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
-0000a820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-0000a830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-0000a840: 6d70 0000 0000 0003 e000 0000 001b 0074  mp.............t
-0000a850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-0000a860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-0000a870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-0000a880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
-0000a890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
-0000a8a0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-0000a8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-0000a8c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-0000a8d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-0000a8e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-0000a8f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-0000a900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-0000a910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000a920: 0809 5f10 187b 7b31 3132 2c20 3535 7d2c  .._..{{112, 55},
-0000a930: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
-0000a940: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-0000a950: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-0000a960: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-0000a970: 0200 7500 6964 7363 6c62 6f6f 6c00 0000  ..u.idsclbool...
-0000a980: 0002 0075 0069 6c67 3153 636f 6d70 0000  ...u.ilg1Scomp..
-0000a990: 0000 0009 419c 0000 0002 0075 0069 6c73  ....A......u.ils
-0000a9a0: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-0000a9b0: 3030 d801 0203 0405 0607 0809 0a0b 1846  00.............F
-0000a9c0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-0000a9d0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-0000a9e0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-0000a9f0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-0000aa00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-0000aa10: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-0000aa20: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-0000aa30: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-0000aa40: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-0000aa50: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-0000aa60: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-0000aa70: 7209 1101 c709 546e 616d 65d4 100e 0f0d  r.....Tname.....
-0000aa80: 1617 1818 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
-0000aa90: 08d4 100f 0e0d 1b18 1d0a 5c64 6174 654d  ..........\dateM
-0000aaa0: 6f64 6966 6965 6408 10b5 09d4 100f 0e0d  odified.........
-0000aab0: 2018 1d18 5b64 6174 6543 7265 6174 6564   ...[dateCreated
-0000aac0: 0808 d410 0f0e 0d24 1826 0a54 7369 7a65  .......$.&.Tsize
-0000aad0: 0810 6109 d410 0f0e 0d29 0a2b 0a54 6b69  ..a......).+.Tki
-0000aae0: 6e64 0910 7309 d410 0f0e 0d2e 0a30 1855  nd..s........0.U
-0000aaf0: 6c61 6265 6c09 1064 08d4 100f 0e0d 330a  label..d......3.
-0000ab00: 3518 5776 6572 7369 6f6e 0910 4b08 d410  5.Wversion..K...
-0000ab10: 0f0e 0d38 0a3a 1858 636f 6d6d 656e 7473  ...8.:.Xcomments
-0000ab20: 0911 012c 08d4 100f 0e0d 3d18 3f18 5e64  ...,......=.?.^d
-0000ab30: 6174 654c 6173 744f 7065 6e65 6408 10c8  ateLastOpened...
-0000ab40: 08d4 100e 0f0d 421d 1818 5964 6174 6541  ......B...YdateA
-0000ab50: 6464 6564 0808 0823 4028 0000 0000 0000  dded...#@(......
-0000ab60: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-0000ab70: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-0000ab80: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-0000ab90: bc00 c700 c800 cb00 cc00 d100 da00 e300  ................
-0000aba0: e500 e600 e700 f000 fd00 fe01 0001 0101  ................
-0000abb0: 0a01 1601 1701 1801 2101 2601 2701 2901  ........!.&.'.).
-0000abc0: 2a01 3301 3801 3901 3b01 3c01 4501 4b01  *.3.8.9.;.<.E.K.
-0000abd0: 4c01 4e01 4f01 5801 6001 6101 6301 6401  L.N.O.X.`.a.c.d.
-0000abe0: 6d01 7601 7701 7a01 7b01 8401 9301 9401  m.v.w.z.{.......
-0000abf0: 9601 9701 a001 aa01 ab01 ac01 ad01 b601  ................
-0000ac00: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-0000ac10: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-0000ac20: 0001 c500 0000 0200 7500 696c 7376 7062  ........u.ilsvpb
-0000ac30: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
-0000ac40: 0102 0304 0506 0708 090a 0b1a 4546 470a  ............EFG.
-0000ac50: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-0000ac60: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-0000ac70: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-0000ac80: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-0000ac90: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-0000aca0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
-0000acb0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-0000acc0: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
-0000acd0: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
-0000ace0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-0000acf0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-0000ad00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-0000ad10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-0000ad20: 6f6e 546e 616d 65d4 1617 1819 1a0a 1c1d  onTname.........
-0000ad30: 5776 6973 6962 6c65 5961 7363 656e 6469  WvisibleYascendi
-0000ad40: 6e67 5577 6964 7468 5569 6e64 6578 0809  ngUwidthUindex..
-0000ad50: 1101 2c10 07d4 1617 1819 1a1a 2122 0808  ..,.........!"..
-0000ad60: 10c8 1008 d416 1718 190a 1a26 0909 0810  ...........&....
-0000ad70: b5d4 1617 1819 1a1a 262a 0808 1002 d416  ........&*......
-0000ad80: 1718 190a 1a2e 2f09 0810 6110 03d4 1617  ....../...a.....
-0000ad90: 1819 1a0a 3334 0809 1064 1005 d416 1718  ....34...d......
-0000ada0: 190a 0a38 3909 0910 7310 04d4 1617 1819  ...89...s.......
-0000adb0: 1a0a 3d3e 0809 104b 1006 d419 1817 1640  ..=>...K.......@
-0000adc0: 410a 0a10 0011 01c7 0909 0823 4028 0000  A..........#@(..
-0000add0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-0000ade0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-0000adf0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
-0000ae00: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
-0000ae10: f901 0101 0b01 1101 1701 1801 1901 1c01  ................
-0000ae20: 1e01 2701 2801 2901 2b01 2d01 3601 3701  ..'.(.).+.-.6.7.
-0000ae30: 3801 3a01 4301 4401 4501 4701 5001 5101  8.:.C.D.E.G.P.Q.
-0000ae40: 5201 5401 5601 5f01 6001 6101 6301 6501  R.T.V._.`.a.c.e.
-0000ae50: 6e01 6f01 7001 7201 7401 7d01 7e01 7f01  n.o.p.r.t.}.~...
-0000ae60: 8101 8301 8c01 8e01 9101 9201 9301 9401  ................
-0000ae70: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
-0000ae80: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
-0000ae90: 0000 0001 ac00 0000 0200 7500 696d 6f44  ..........u.imoD
-0000aea0: 4462 6c6f 6200 0000 086c 6d0e 79f5 09c5  Dblob....lm.y...
-0000aeb0: 4100 0000 0200 7500 696d 6f64 4462 6c6f  A.....u.imodDblo
-0000aec0: 6200 0000 0862 2d63 9153 09c5 4100 0000  b....b-c.S..A...
-0000aed0: 0200 7500 6970 6831 5363 6f6d 7000 0000  ..u.iph1Scomp...
-0000aee0: 0000 0c50 006f 6f6c 6261 725b 5368 6f77  ...P.oolbar[Show
+0000a160: 5369 6465 6261 7208 0809 0809 5f10 197b  Sidebar....._..{
+0000a170: 7b33 3535 2c20 3132 357d 2c20 7b31 3037  {355, 125}, {107
+0000a180: 362c 2036 3231 7d7d 0908 1725 313d 4960  6, 621}}...%1=I`
+0000a190: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
+0000a1a0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+0000a1b0: 0000 0000 0000 009b 0000 001b 0074 0068  .............t.h
+0000a1c0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
+0000a1d0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
+0000a1e0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
+0000a1f0: 0073 6c67 3153 636f 6d70 0000 0000 0002  .slg1Scomp......
+0000a200: 25f3 0000 001b 0074 0068 0069 0072 0064  %......t.h.i.r.d
+0000a210: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
+0000a220: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
+0000a230: 0065 006e 0064 0065 0072 0073 6c73 7643  .e.n.d.e.r.slsvC
+0000a240: 626c 6f62 0000 0279 6270 6c69 7374 3030  blob...ybplist00
+0000a250: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
+0000a260: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+0000a270: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+0000a280: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000a290: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000a2a0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000a2b0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+0000a2c0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+0000a2d0: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
+0000a2e0: 373c 41d4 0d0e 0f10 0a12 0a14 5776 6973  7<A.........Wvis
+0000a2f0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+0000a300: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+0000a310: 1101 a609 546e 616d 65d4 0d0e 0f10 1617  ....Tname.......
+0000a320: 1619 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
+0000a330: 0d0e 0f10 0a1c 161e 0910 b508 5c64 6174  ............\dat
+0000a340: 654d 6f64 6966 6965 64d4 0d0e 0f10 161c  eModified.......
+0000a350: 1622 0808 5b64 6174 6543 7265 6174 6564  ."..[dateCreated
+0000a360: d40d 0e0f 100a 2516 2709 1061 0854 7369  ......%.'..a.Tsi
+0000a370: 7a65 d40d 0e0f 100a 2a0a 2c09 1073 0954  ze......*.,..s.T
+0000a380: 6b69 6e64 d40d 0e0f 1016 2f0a 3108 1064  kind....../.1..d
+0000a390: 0955 6c61 6265 6cd4 0d0e 0f10 1634 0a36  .Ulabel......4.6
+0000a3a0: 0810 4b09 5776 6572 7369 6f6e d40d 0e0f  ..K.Wversion....
+0000a3b0: 1016 390a 3b08 1101 2c09 5863 6f6d 6d65  ..9.;...,.Xcomme
+0000a3c0: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
+0000a3d0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+0000a3e0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
+0000a3f0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
+0000a400: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+0000a410: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+0000a420: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
+0000a430: c700 c800 cb00 cc00 d100 da00 db00 dd00  ................
+0000a440: de00 e700 f000 f100 f300 f401 0101 0a01  ................
+0000a450: 0b01 0c01 1801 2101 2201 2401 2501 2a01  ......!.".$.%.*.
+0000a460: 3301 3401 3601 3701 3c01 4501 4601 4801  3.4.6.7.<.E.F.H.
+0000a470: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
+0000a480: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
+0000a490: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
+0000a4a0: c400 0000 0000 0002 0100 0000 0000 0000  ................
+0000a4b0: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
+0000a4c0: c500 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
+0000a4d0: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
+0000a4e0: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
+0000a4f0: 6500 6e00 6400 6500 7200 736c 7376 7062  e.n.d.e.r.slsvpb
+0000a500: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
+0000a510: 0102 0304 0506 0708 090a 0b1d 4546 470a  ............EFG.
+0000a520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+0000a530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+0000a540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+0000a550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+0000a560: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+0000a570: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+0000a580: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+0000a590: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
+0000a5a0: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
+0000a5b0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+0000a5c0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+0000a5d0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+0000a5e0: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+0000a5f0: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+0000a600: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+0000a610: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+0000a620: 1101 2c09 08d4 1617 1819 1f20 1d1d 1008  ..,........ ....
+0000a630: 10c8 0808 d416 1718 1909 241d 0a10 b508  ..........$.....
+0000a640: 09d4 1617 1819 2824 1d1d 1002 0808 d416  ......($........
+0000a650: 1718 192c 2d1d 0a10 0310 6108 09d4 1617  ...,-.....a.....
+0000a660: 1819 3132 0a1d 1005 1064 0908 d416 1718  ..12.....d......
+0000a670: 1936 370a 0a10 0410 7309 09d4 1617 1819  .67.....s.......
+0000a680: 3b3c 0a1d 1006 104b 0908 d416 1718 1940  ;<.....K.......@
+0000a690: 410a 0a10 0011 01a6 0909 0823 4028 0000  A..........#@(..
+0000a6a0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
+0000a6b0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+0000a6c0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
+0000a6d0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
+0000a6e0: f900 ff01 0501 0f01 1701 1901 1c01 1d01  ................
+0000a6f0: 1e01 2701 2901 2b01 2c01 2d01 3601 3801  ..'.).+.,.-.6.8.
+0000a700: 3901 3a01 4301 4501 4601 4701 5001 5201  9.:.C.E.F.G.P.R.
+0000a710: 5401 5501 5601 5f01 6101 6301 6401 6501  T.U.V._.a.c.d.e.
+0000a720: 6e01 7001 7201 7301 7401 7d01 7f01 8101  n.p.r.s.t.}.....
+0000a730: 8201 8301 8c01 8e01 9101 9201 9301 9401  ................
+0000a740: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
+0000a750: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
+0000a760: 0000 0001 ac00 0000 1b00 7400 6800 6900  ..........t.h.i.
+0000a770: 7200 6400 5f00 7000 6100 7200 7400 7900  r.d._.p.a.r.t.y.
+0000a780: 5f00 6c00 6100 6200 6500 6c00 5f00 6100  _.l.a.b.e.l._.a.
+0000a790: 7000 7000 6500 6e00 6400 6500 7200 736d  p.p.e.n.d.e.r.sm
+0000a7a0: 6f44 4462 6c6f 6200 0000 0896 55ea 6347  oDDblob.....U.cG
+0000a7b0: 0dc5 4100 0000 1b00 7400 6800 6900 7200  ..A.....t.h.i.r.
+0000a7c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+0000a7d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
+0000a7e0: 7000 6500 6e00 6400 6500 7200 736d 6f64  p.e.n.d.e.r.smod
+0000a7f0: 4462 6c6f 6200 0000 08cb c8d0 edcc 0cc5  Dblob...........
+0000a800: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
+0000a810: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
+0000a820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
+0000a830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
+0000a840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
+0000a850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
+0000a860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
+0000a870: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
+0000a880: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
+0000a890: 0100 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
+0000a8a0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+0000a8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+0000a8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+0000a8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+0000a8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+0000a8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+0000a900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+0000a910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+0000a920: 0908 095f 1018 7b7b 3131 322c 2035 357d  ..._..{{112, 55}
+0000a930: 2c20 7b31 3139 392c 2037 3639 7d7d 0908  , {1199, 769}}..
+0000a940: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
+0000a950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000a960: 0000 0000 0000 0000 0000 0000 009a 0000  ................
+0000a970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
+0000a980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
+0000a990: 0000 0000 0947 3a00 0000 0200 7500 696c  .....G:.....u.il
+0000a9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
+0000a9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+0000a9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+0000a9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+0000a9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+0000a9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+0000aa00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+0000aa10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+0000aa20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+0000aa30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+0000aa40: 282d 3237 3c41 d40d 0e0f 100a 120a 1457  (-27<A.........W
+0000aa50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+0000aa60: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+0000aa70: 6572 0911 01c7 0954 6e61 6d65 d410 0e0f  er.....Tname....
+0000aa80: 0d16 1718 1858 7562 6971 7569 7479 1023  .....Xubiquity.#
+0000aa90: 0808 d410 0f0e 0d1b 181d 0a5c 6461 7465  ...........\date
+0000aaa0: 4d6f 6469 6669 6564 0810 b509 d410 0f0e  Modified........
+0000aab0: 0d20 181d 185b 6461 7465 4372 6561 7465  . ...[dateCreate
+0000aac0: 6408 08d4 100f 0e0d 2418 260a 5473 697a  d.......$.&.Tsiz
+0000aad0: 6508 1061 09d4 100f 0e0d 290a 2b0a 546b  e..a......).+.Tk
+0000aae0: 696e 6409 1073 09d4 100f 0e0d 2e0a 3018  ind..s........0.
+0000aaf0: 556c 6162 656c 0910 6408 d410 0f0e 0d33  Ulabel..d......3
+0000ab00: 0a35 1857 7665 7273 696f 6e09 104b 08d4  .5.Wversion..K..
+0000ab10: 100f 0e0d 380a 3a18 5863 6f6d 6d65 6e74  ....8.:.Xcomment
+0000ab20: 7309 1101 2c08 d410 0f0e 0d3d 183f 185e  s...,......=.?.^
+0000ab30: 6461 7465 4c61 7374 4f70 656e 6564 0810  dateLastOpened..
+0000ab40: c808 d410 0e0f 0d42 1d18 1859 6461 7465  .......B...Ydate
+0000ab50: 4164 6465 6408 0808 2340 2800 0000 0000  Added...#@(.....
+0000ab60: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
+0000ab70: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+0000ab80: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
+0000ab90: 00bc 00c7 00c8 00cb 00cc 00d1 00da 00e3  ................
+0000aba0: 00e5 00e6 00e7 00f0 00fd 00fe 0100 0101  ................
+0000abb0: 010a 0116 0117 0118 0121 0126 0127 0129  .........!.&.'.)
+0000abc0: 012a 0133 0138 0139 013b 013c 0145 014b  .*.3.8.9.;.<.E.K
+0000abd0: 014c 014e 014f 0158 0160 0161 0163 0164  .L.N.O.X.`.a.c.d
+0000abe0: 016d 0176 0177 017a 017b 0184 0193 0194  .m.v.w.z.{......
+0000abf0: 0196 0197 01a0 01aa 01ab 01ac 01ad 01b6  ................
+0000ac00: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
+0000ac10: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+0000ac20: 0000 01c5 0000 0002 0075 0069 6c73 7670  .........u.ilsvp
+0000ac30: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+0000ac40: d801 0203 0405 0607 0809 0a0b 1a45 4647  .............EFG
+0000ac50: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+0000ac60: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+0000ac70: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000ac80: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000ac90: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000aca0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+0000acb0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+0000acc0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
+0000acd0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
+0000ace0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+0000acf0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+0000ad00: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+0000ad10: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+0000ad20: 696f 6e54 6e61 6d65 d416 1718 191a 0a1c  ionTname........
+0000ad30: 1d57 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
+0000ad40: 696e 6755 7769 6474 6855 696e 6465 7808  ingUwidthUindex.
+0000ad50: 0911 012c 1007 d416 1718 191a 1a21 2208  ...,.........!".
+0000ad60: 0810 c810 08d4 1617 1819 0a1a 2609 0908  ............&...
+0000ad70: 10b5 d416 1718 191a 1a26 2a08 0810 02d4  .........&*.....
+0000ad80: 1617 1819 0a1a 2e2f 0908 1061 1003 d416  ......./...a....
+0000ad90: 1718 191a 0a33 3408 0910 6410 05d4 1617  .....34...d.....
+0000ada0: 1819 0a0a 3839 0909 1073 1004 d416 1718  ....89...s......
+0000adb0: 191a 0a3d 3e08 0910 4b10 06d4 1918 1716  ...=>...K.......
+0000adc0: 4041 0a0a 1000 1101 c709 0908 2340 2800  @A..........#@(.
+0000add0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+0000ade0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+0000adf0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+0000ae00: 00ba 00c7 00d3 00d8 00de 00e3 00eb 00f0  ................
+0000ae10: 00f9 0101 010b 0111 0117 0118 0119 011c  ................
+0000ae20: 011e 0127 0128 0129 012b 012d 0136 0137  ...'.(.).+.-.6.7
+0000ae30: 0138 013a 0143 0144 0145 0147 0150 0151  .8.:.C.D.E.G.P.Q
+0000ae40: 0152 0154 0156 015f 0160 0161 0163 0165  .R.T.V._.`.a.c.e
+0000ae50: 016e 016f 0170 0172 0174 017d 017e 017f  .n.o.p.r.t.}.~..
+0000ae60: 0181 0183 018c 018e 0191 0192 0193 0194  ................
+0000ae70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
+0000ae80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000ae90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
+0000aea0: 4444 626c 6f62 0000 0008 f6bf 1d48 cc0c  DDblob.......H..
+0000aeb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
+0000aec0: 6f62 0000 0008 f6bf 1d48 cc0c c541 0000  ob.......H...A..
+0000aed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
+0000aee0: 0000 000c 5000 6f6c 6261 725b 5368 6f77  ....P.olbar[Show
 0000aef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 0000af00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 0000af10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 0000af20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
 0000af30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
 0000af40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 0000af50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 0000af60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 0000af70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
 0000af80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000af90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
+0000af90: 6f6d 7000 0000 0000 08bf a500 0000 0000  omp.............
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
 0000b010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
 0000b020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
-0000b030: 0000 00c8 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b030: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
 0000b040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 0000b050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 0000b060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 0000b070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 0000b080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 0000b090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 0000b0a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b0b0: 0809 5f10 177b 7b39 322c 2037 357d 2c20  .._..{{92, 75}, 
-0000b0c0: 7b31 3139 392c 2037 3639 7d7d 0908 1725  {1199, 769}}...%
-0000b0d0: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
-0000b0e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-0000b0f0: 0000 0000 0000 0000 0000 0099 0000 000c  ................
-0000b100: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-0000b110: 0069 0073 0065 0064 6473 636c 626f 6f6c  .i.s.e.ddsclbool
-0000b120: 0000 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
-0000b130: 6500 7200 7600 6900 7300 6500 646c 6731  e.r.v.i.s.e.dlg1
-0000b140: 5363 6f6d 7000 0000 0000 07ac 4200 0000  Scomp.......B...
-0000b150: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
-0000b160: 7600 6900 7300 6500 646c 7376 4362 6c6f  v.i.s.e.dlsvCblo
-0000b170: 6200 0002 8162 706c 6973 7430 30d8 0102  b....bplist00...
-0000b180: 0304 0506 0708 090a 0b18 4647 480a 5f10  ..........FGH._.
-0000b190: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-0000b1a0: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-0000b1b0: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-0000b1c0: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-0000b1d0: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-0000b1e0: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
-0000b1f0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-0000b200: 7310 0109 ab0c 151a 1f23 282d 3237 3c41  s........#(-27<A
-0000b210: d40d 0e0f 1011 120a 0a5a 6964 656e 7469  .........Zidenti
-0000b220: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
-0000b230: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
-0000b240: 6511 01c7 0909 d40d 0e0f 1016 1718 1858  e..............X
-0000b250: 7562 6971 7569 7479 1023 0808 d40d 0e0f  ubiquity.#......
-0000b260: 101b 1c18 0a5c 6461 7465 4d6f 6469 6669  .....\dateModifi
-0000b270: 6564 10b5 0809 d40d 0e0f 1020 1c18 185b  ed......... ...[
-0000b280: 6461 7465 4372 6561 7465 6408 08d4 0d0e  dateCreated.....
-0000b290: 0f10 2425 180a 5473 697a 6510 6108 09d4  ..$%..Tsize.a...
-0000b2a0: 0d0e 0f10 292a 0a0a 546b 696e 6410 7309  ....)*..Tkind.s.
-0000b2b0: 09d4 0d0e 0f10 2e2f 0a18 556c 6162 656c  ......./..Ulabel
-0000b2c0: 1064 0908 d40d 0e0f 1033 340a 1857 7665  .d.......34..Wve
-0000b2d0: 7273 696f 6e10 4b09 08d4 0d0e 0f10 3839  rsion.K.......89
-0000b2e0: 0a18 5863 6f6d 6d65 6e74 7311 012c 0908  ..Xcomments..,..
-0000b2f0: d40d 0e0f 103d 3e18 185e 6461 7465 4c61  .....=>..^dateLa
-0000b300: 7374 4f70 656e 6564 10c8 0808 d40d 0e0f  stOpened........
-0000b310: 1042 1c18 1859 6461 7465 4164 6465 6408  .B...YdateAdded.
-0000b320: 0808 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
-0000b330: 4d6f 6469 6669 6564 2340 3000 0000 0000  Modified#@0.....
-0000b340: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-0000b350: 0070 0079 008c 008e 008f 009b 00a4 00af  .p.y............
-0000b360: 00b5 00bf 00c7 00cc 00cf 00d0 00d1 00da  ................
-0000b370: 00e3 00e5 00e6 00e7 00f0 00fd 00ff 0100  ................
-0000b380: 0101 010a 0116 0117 0118 0121 0126 0128  ...........!.&.(
-0000b390: 0129 012a 0133 0138 013a 013b 013c 0145  .).*.3.8.:.;.<.E
-0000b3a0: 014b 014d 014e 014f 0158 0160 0162 0163  .K.M.N.O.X.`.b.c
-0000b3b0: 0164 016d 0176 0179 017a 017b 0184 0193  .d.m.v.y.z.{....
-0000b3c0: 0195 0196 0197 01a0 01aa 01ab 01ac 01ad  ................
-0000b3d0: 01b6 01c3 01cc 0000 0000 0000 0201 0000  ................
-0000b3e0: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-0000b3f0: 0000 0000 01cd 0000 000c 0075 006e 0073  ...........u.n.s
-0000b400: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b410: 0064 6c73 7670 626c 6f62 0000 0266 6270  .dlsvpblob...fbp
-0000b420: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
-0000b430: 0a0b 1a45 4647 0a5f 1012 7669 6577 4f70  ...EFG._..viewOp
-0000b440: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
-0000b450: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-0000b460: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-0000b470: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-0000b480: 697a 655a 736f 7274 436f 6c75 6d6e 5869  izeZsortColumnXi
-0000b490: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
-0000b4a0: 6174 6976 6544 6174 6573 1001 09d9 0c0d  ativeDates......
-0000b4b0: 0e0f 1011 1213 1415 1e23 272b 3035 3a3f  .........#'+05:?
-0000b4c0: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
-0000b4d0: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
-0000b4e0: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
-0000b4f0: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
-0000b500: 6457 7665 7273 696f 6e54 6e61 6d65 d416  dWversionTname..
-0000b510: 1718 191a 1b0a 1d57 7669 7369 626c 6555  .......WvisibleU
-0000b520: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
-0000b530: 696e 6465 7808 1101 2c09 1007 d416 1718  index...,.......
-0000b540: 191a 201a 2208 10c8 0810 08d4 1617 1819  .. ."...........
-0000b550: 0a25 1a09 0910 b508 d416 1718 191a 251a  .%............%.
-0000b560: 2a08 0810 02d4 1617 1819 0a2d 1a2f 0910  *..........-./..
-0000b570: 6108 1003 d416 1718 191a 320a 3408 1064  a.........2.4..d
-0000b580: 0910 05d4 1617 1819 0a37 0a39 0910 7309  .........7.9..s.
-0000b590: 1004 d416 1718 191a 3c0a 3e08 104b 0910  ........<.>..K..
-0000b5a0: 06d4 1617 1819 0a41 0a43 0911 01c7 0910  .......A.C......
-0000b5b0: 0008 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
-0000b5c0: 4d6f 6469 6669 6564 2340 3000 0000 0000  Modified#@0.....
-0000b5d0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-0000b5e0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
-0000b5f0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
-0000b600: 0101 0107 0111 0117 0118 011b 011c 011e  ................
-0000b610: 0127 0128 012a 012b 012d 0136 0137 0139  .'.(.*.+.-.6.7.9
-0000b620: 013a 0143 0144 0145 0147 0150 0151 0153  .:.C.D.E.G.P.Q.S
-0000b630: 0154 0156 015f 0160 0162 0163 0165 016e  .T.V._.`.b.c.e.n
-0000b640: 016f 0171 0172 0174 017d 017e 0180 0181  .o.q.r.t.}.~....
-0000b650: 0183 018c 018d 0190 0191 0193 0194 019d  ................
-0000b660: 01aa 01b3 0000 0000 0000 0201 0000 0000  ................
-0000b670: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-0000b680: 0000 01b4 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-0000b690: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-0000b6a0: 6d6f 4444 626c 6f62 0000 0008 04d0 54a0  moDDblob......T.
-0000b6b0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-0000b6c0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-0000b6d0: 6d6f 6444 626c 6f62 0000 0008 04d0 54a0  modDblob......T.
-0000b6e0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-0000b6f0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-0000b700: 7068 3153 636f 6d70 0000 0000 0009 b000  ph1Scomp........
-0000b710: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
-0000b720: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
-0000b730: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
-0000b740: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
-0000b750: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-0000b760: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-0000b770: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-0000b780: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-0000b790: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-0000b7a0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-0000b7b0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-0000b7c0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-0000b7d0: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
-0000b7e0: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-0000b7f0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+0000b0b0: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
+0000b0c0: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
+0000b0d0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+0000b0e0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+0000b0f0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
+0000b100: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
+0000b110: 7600 6900 7300 6500 6464 7363 6c62 6f6f  v.i.s.e.ddsclboo
+0000b120: 6c00 0000 000c 0075 006e 0073 0075 0070  l......u.n.s.u.p
+0000b130: 0065 0072 0076 0069 0073 0065 0064 6c67  .e.r.v.i.s.e.dlg
+0000b140: 3153 636f 6d70 0000 0000 0002 4b53 0000  1Scomp......KS..
+0000b150: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+0000b160: 0076 0069 0073 0065 0064 6c73 7643 626c  .v.i.s.e.dlsvCbl
+0000b170: 6f62 0000 0281 6270 6c69 7374 3030 d801  ob....bplist00..
+0000b180: 0203 0405 0607 0809 0a0b 1846 4748 0a5f  ...........FGH._
+0000b190: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+0000b1a0: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+0000b1b0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+0000b1c0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+0000b1d0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+0000b1e0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+0000b1f0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+0000b200: 6573 1001 09ab 0c15 1a1f 2328 2d32 373c  es........#(-27<
+0000b210: 41d4 0d0e 0f10 1112 0a0a 5a69 6465 6e74  A.........Zident
+0000b220: 6966 6965 7255 7769 6474 6859 6173 6365  ifierUwidthYasce
+0000b230: 6e64 696e 6757 7669 7369 626c 6554 6e61  ndingWvisibleTna
+0000b240: 6d65 1101 c709 09d4 0d0e 0f10 1617 1818  me..............
+0000b250: 5875 6269 7175 6974 7910 2308 08d4 0d0e  Xubiquity.#.....
+0000b260: 0f10 1b1c 180a 5c64 6174 654d 6f64 6966  ......\dateModif
+0000b270: 6965 6410 b508 09d4 0d0e 0f10 201c 1818  ied......... ...
+0000b280: 5b64 6174 6543 7265 6174 6564 0808 d40d  [dateCreated....
+0000b290: 0e0f 1024 2518 0a54 7369 7a65 1061 0809  ...$%..Tsize.a..
+0000b2a0: d40d 0e0f 1029 2a0a 0a54 6b69 6e64 1073  .....)*..Tkind.s
+0000b2b0: 0909 d40d 0e0f 102e 2f0a 1855 6c61 6265  ......../..Ulabe
+0000b2c0: 6c10 6409 08d4 0d0e 0f10 3334 0a18 5776  l.d.......34..Wv
+0000b2d0: 6572 7369 6f6e 104b 0908 d40d 0e0f 1038  ersion.K.......8
+0000b2e0: 390a 1858 636f 6d6d 656e 7473 1101 2c09  9..Xcomments..,.
+0000b2f0: 08d4 0d0e 0f10 3d3e 1818 5e64 6174 654c  ......=>..^dateL
+0000b300: 6173 744f 7065 6e65 6410 c808 08d4 0d0e  astOpened.......
+0000b310: 0f10 421c 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
+0000b320: 0808 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
+0000b330: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
+0000b340: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+0000b350: 6500 7000 7900 8c00 8e00 8f00 9b00 a400  e.p.y...........
+0000b360: af00 b500 bf00 c700 cc00 cf00 d000 d100  ................
+0000b370: da00 e300 e500 e600 e700 f000 fd00 ff01  ................
+0000b380: 0001 0101 0a01 1601 1701 1801 2101 2601  ............!.&.
+0000b390: 2801 2901 2a01 3301 3801 3a01 3b01 3c01  (.).*.3.8.:.;.<.
+0000b3a0: 4501 4b01 4d01 4e01 4f01 5801 6001 6201  E.K.M.N.O.X.`.b.
+0000b3b0: 6301 6401 6d01 7601 7901 7a01 7b01 8401  c.d.m.v.y.z.{...
+0000b3c0: 9301 9501 9601 9701 a001 aa01 ab01 ac01  ................
+0000b3d0: ad01 b601 c301 cc00 0000 0000 0002 0100  ................
+0000b3e0: 0000 0000 0000 4a00 0000 0000 0000 0000  ......J.........
+0000b3f0: 0000 0000 0001 cd00 0000 0c00 7500 6e00  ............u.n.
+0000b400: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
+0000b410: 6500 646c 7376 7062 6c6f 6200 0002 6662  e.dlsvpblob...fb
+0000b420: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+0000b430: 090a 0b1a 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
+0000b440: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+0000b450: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+0000b460: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+0000b470: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+0000b480: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
+0000b490: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
+0000b4a0: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
+0000b4b0: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
+0000b4c0: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
+0000b4d0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+0000b4e0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+0000b4f0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+0000b500: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+0000b510: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
+0000b520: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+0000b530: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
+0000b540: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
+0000b550: 190a 251a 0909 10b5 08d4 1617 1819 1a25  ..%............%
+0000b560: 1a2a 0808 1002 d416 1718 190a 2d1a 2f09  .*..........-./.
+0000b570: 1061 0810 03d4 1617 1819 1a32 0a34 0810  .a.........2.4..
+0000b580: 6409 1005 d416 1718 190a 370a 3909 1073  d.........7.9..s
+0000b590: 0910 04d4 1617 1819 1a3c 0a3e 0810 4b09  .........<.>..K.
+0000b5a0: 1006 d416 1718 190a 410a 4309 1101 c709  ........A.C.....
+0000b5b0: 1000 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
+0000b5c0: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
+0000b5d0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+0000b5e0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
+0000b5f0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
+0000b600: f901 0101 0701 1101 1701 1801 1b01 1c01  ................
+0000b610: 1e01 2701 2801 2a01 2b01 2d01 3601 3701  ..'.(.*.+.-.6.7.
+0000b620: 3901 3a01 4301 4401 4501 4701 5001 5101  9.:.C.D.E.G.P.Q.
+0000b630: 5301 5401 5601 5f01 6001 6201 6301 6501  S.T.V._.`.b.c.e.
+0000b640: 6e01 6f01 7101 7201 7401 7d01 7e01 8001  n.o.q.r.t.}.~...
+0000b650: 8101 8301 8c01 8d01 9001 9101 9301 9401  ................
+0000b660: 9d01 aa01 b300 0000 0000 0002 0100 0000  ................
+0000b670: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
+0000b680: 0000 0001 b400 0000 0c00 7500 6e00 7300  ..........u.n.s.
+0000b690: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+0000b6a0: 646d 6f44 4462 6c6f 6200 0000 08e7 da8e  dmoDDblob.......
+0000b6b0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
+0000b6c0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+0000b6d0: 646d 6f64 4462 6c6f 6200 0000 08e7 da8e  dmodDblob.......
+0000b6e0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
+0000b6f0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
+0000b700: 6470 6831 5363 6f6d 7000 0000 0000 02b0  dph1Scomp.......
+0000b710: 0000 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
+0000b720: 6500 7200 7600 6900 7300 6500 6476 5372  e.r.v.i.s.e.dvSr
+0000b730: 6e6c 6f6e 6700 0000 0100 0000 0500 7500  nlong.........u.
+0000b740: 7400 6900 6c00 7362 7773 7062 6c6f 6200  t.i.l.sbwspblob.
+0000b750: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+0000b760: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+0000b770: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+0000b780: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+0000b790: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+0000b7a0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+0000b7b0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+0000b7c0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+0000b7d0: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
+0000b7e0: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
+0000b7f0: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
 0000b800: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-0000b810: 0000 0000 0000 0000 0000 009b 006c 0061  .............l.a
-0000b820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-0000b830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-0000b840: 6d70 0000 0000 0003 e000 0000 001b 0074  mp.............t
-0000b850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-0000b860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-0000b870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-0000b880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
-0000b890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
-0000b8a0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-0000b8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-0000b8c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-0000b8d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-0000b8e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-0000b8f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-0000b900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-0000b910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b920: 0809 5f10 187b 7b31 3132 2c20 3535 7d2c  .._..{{112, 55},
-0000b930: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
-0000b940: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-0000b950: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-0000b960: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-0000b970: 0200 7500 6964 7363 6c62 6f6f 6c00 0000  ..u.idsclbool...
-0000b980: 0002 0075 0069 6c67 3153 636f 6d70 0000  ...u.ilg1Scomp..
-0000b990: 0000 0009 419c 0000 0002 0075 0069 6c73  ....A......u.ils
-0000b9a0: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-0000b9b0: 3030 d801 0203 0405 0607 0809 0a0b 1846  00.............F
-0000b9c0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-0000b9d0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-0000b9e0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-0000b9f0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-0000ba00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-0000ba10: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-0000ba20: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-0000ba30: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-0000ba40: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-0000ba50: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-0000ba60: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-0000ba70: 7209 1101 c709 546e 616d 65d4 100e 0f0d  r.....Tname.....
-0000ba80: 1617 1818 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
-0000ba90: 08d4 100f 0e0d 1b18 1d0a 5c64 6174 654d  ..........\dateM
-0000baa0: 6f64 6966 6965 6408 10b5 09d4 100f 0e0d  odified.........
-0000bab0: 2018 1d18 5b64 6174 6543 7265 6174 6564   ...[dateCreated
-0000bac0: 0808 d410 0f0e 0d24 1826 0a54 7369 7a65  .......$.&.Tsize
-0000bad0: 0810 6109 d410 0f0e 0d29 0a2b 0a54 6b69  ..a......).+.Tki
-0000bae0: 6e64 0910 7309 d410 0f0e 0d2e 0a30 1855  nd..s........0.U
-0000baf0: 6c61 6265 6c09 1064 08d4 100f 0e0d 330a  label..d......3.
-0000bb00: 3518 5776 6572 7369 6f6e 0910 4b08 d410  5.Wversion..K...
-0000bb10: 0f0e 0d38 0a3a 1858 636f 6d6d 656e 7473  ...8.:.Xcomments
-0000bb20: 0911 012c 08d4 100f 0e0d 3d18 3f18 5e64  ...,......=.?.^d
-0000bb30: 6174 654c 6173 744f 7065 6e65 6408 10c8  ateLastOpened...
-0000bb40: 08d4 100e 0f0d 421d 1818 5964 6174 6541  ......B...YdateA
-0000bb50: 6464 6564 0808 0823 4028 0000 0000 0000  dded...#@(......
-0000bb60: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-0000bb70: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-0000bb80: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-0000bb90: bc00 c700 c800 cb00 cc00 d100 da00 e300  ................
-0000bba0: e500 e600 e700 f000 fd00 fe01 0001 0101  ................
-0000bbb0: 0a01 1601 1701 1801 2101 2601 2701 2901  ........!.&.'.).
-0000bbc0: 2a01 3301 3801 3901 3b01 3c01 4501 4b01  *.3.8.9.;.<.E.K.
-0000bbd0: 4c01 4e01 4f01 5801 6001 6101 6301 6401  L.N.O.X.`.a.c.d.
-0000bbe0: 6d01 7601 7701 7a01 7b01 8401 9301 9401  m.v.w.z.{.......
-0000bbf0: 9601 9701 a001 aa01 ab01 ac01 ad01 b601  ................
-0000bc00: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-0000bc10: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-0000bc20: 0001 c500 0000 0200 7500 696c 7376 7062  ........u.ilsvpb
-0000bc30: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
-0000bc40: 0102 0304 0506 0708 090a 0b1a 4546 470a  ............EFG.
-0000bc50: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-0000bc60: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-0000bc70: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-0000bc80: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-0000bc90: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-0000bca0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
-0000bcb0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-0000bcc0: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
-0000bcd0: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
-0000bce0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-0000bcf0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-0000bd00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-0000bd10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-0000bd20: 6f6e 546e 616d 65d4 1617 1819 1a0a 1c1d  onTname.........
-0000bd30: 5776 6973 6962 6c65 5961 7363 656e 6469  WvisibleYascendi
-0000bd40: 6e67 5577 6964 7468 5569 6e64 6578 0809  ngUwidthUindex..
-0000bd50: 1101 2c10 07d4 1617 1819 1a1a 2122 0808  ..,.........!"..
-0000bd60: 10c8 1008 d416 1718 190a 1a26 0909 0810  ...........&....
-0000bd70: b5d4 1617 1819 1a1a 262a 0808 1002 d416  ........&*......
-0000bd80: 1718 190a 1a2e 2f09 0810 6110 03d4 1617  ....../...a.....
-0000bd90: 1819 1a0a 3334 0809 1064 1005 d416 1718  ....34...d......
-0000bda0: 190a 0a38 3909 0910 7310 04d4 1617 1819  ...89...s.......
-0000bdb0: 1a0a 3d3e 0809 104b 1006 d419 1817 1640  ..=>...K.......@
-0000bdc0: 410a 0a10 0011 01c7 0909 0823 4028 0000  A..........#@(..
-0000bdd0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-0000bde0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-0000bdf0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
-0000be00: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
-0000be10: f901 0101 0b01 1101 1701 1801 1901 1c01  ................
-0000be20: 1e01 2701 2801 2901 2b01 2d01 3601 3701  ..'.(.).+.-.6.7.
-0000be30: 3801 3a01 4301 4401 4501 4701 5001 5101  8.:.C.D.E.G.P.Q.
-0000be40: 5201 5401 5601 5f01 6001 6101 6301 6501  R.T.V._.`.a.c.e.
-0000be50: 6e01 6f01 7001 7201 7401 7d01 7e01 7f01  n.o.p.r.t.}.~...
-0000be60: 8101 8301 8c01 8e01 9101 9201 9301 9401  ................
-0000be70: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
-0000be80: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
-0000be90: 0000 0001 ac00 0000 0200 7500 696d 6f44  ..........u.imoD
-0000bea0: 4462 6c6f 6200 0000 086c 6d0e 79f5 09c5  Dblob....lm.y...
-0000beb0: 4100 0000 0200 7500 696d 6f64 4462 6c6f  A.....u.imodDblo
-0000bec0: 6200 0000 0862 2d63 9153 09c5 4100 0000  b....b-c.S..A...
-0000bed0: 0200 7500 6970 6831 5363 6f6d 7000 0000  ..u.iph1Scomp...
-0000bee0: 0000 0c50 006f 6f6c 6261 725b 5368 6f77  ...P.oolbar[Show
+0000b810: 0000 0000 0000 0000 0000 009a 5f00 6c00  ............_.l.
+0000b820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
+0000b830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
+0000b840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
+0000b850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
+0000b860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
+0000b870: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
+0000b880: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
+0000b890: 0100 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
+0000b8a0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+0000b8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+0000b8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+0000b8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+0000b8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+0000b8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+0000b900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+0000b910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+0000b920: 0908 095f 1018 7b7b 3131 322c 2035 357d  ..._..{{112, 55}
+0000b930: 2c20 7b31 3139 392c 2037 3639 7d7d 0908  , {1199, 769}}..
+0000b940: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
+0000b950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000b960: 0000 0000 0000 0000 0000 0000 009a 0000  ................
+0000b970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
+0000b980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
+0000b990: 0000 0000 0947 3a00 0000 0200 7500 696c  .....G:.....u.il
+0000b9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
+0000b9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+0000b9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+0000b9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+0000b9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+0000b9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+0000ba00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+0000ba10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+0000ba20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+0000ba30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+0000ba40: 282d 3237 3c41 d40d 0e0f 100a 120a 1457  (-27<A.........W
+0000ba50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+0000ba60: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+0000ba70: 6572 0911 01c7 0954 6e61 6d65 d410 0e0f  er.....Tname....
+0000ba80: 0d16 1718 1858 7562 6971 7569 7479 1023  .....Xubiquity.#
+0000ba90: 0808 d410 0f0e 0d1b 181d 0a5c 6461 7465  ...........\date
+0000baa0: 4d6f 6469 6669 6564 0810 b509 d410 0f0e  Modified........
+0000bab0: 0d20 181d 185b 6461 7465 4372 6561 7465  . ...[dateCreate
+0000bac0: 6408 08d4 100f 0e0d 2418 260a 5473 697a  d.......$.&.Tsiz
+0000bad0: 6508 1061 09d4 100f 0e0d 290a 2b0a 546b  e..a......).+.Tk
+0000bae0: 696e 6409 1073 09d4 100f 0e0d 2e0a 3018  ind..s........0.
+0000baf0: 556c 6162 656c 0910 6408 d410 0f0e 0d33  Ulabel..d......3
+0000bb00: 0a35 1857 7665 7273 696f 6e09 104b 08d4  .5.Wversion..K..
+0000bb10: 100f 0e0d 380a 3a18 5863 6f6d 6d65 6e74  ....8.:.Xcomment
+0000bb20: 7309 1101 2c08 d410 0f0e 0d3d 183f 185e  s...,......=.?.^
+0000bb30: 6461 7465 4c61 7374 4f70 656e 6564 0810  dateLastOpened..
+0000bb40: c808 d410 0e0f 0d42 1d18 1859 6461 7465  .......B...Ydate
+0000bb50: 4164 6465 6408 0808 2340 2800 0000 0000  Added...#@(.....
+0000bb60: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
+0000bb70: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+0000bb80: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
+0000bb90: 00bc 00c7 00c8 00cb 00cc 00d1 00da 00e3  ................
+0000bba0: 00e5 00e6 00e7 00f0 00fd 00fe 0100 0101  ................
+0000bbb0: 010a 0116 0117 0118 0121 0126 0127 0129  .........!.&.'.)
+0000bbc0: 012a 0133 0138 0139 013b 013c 0145 014b  .*.3.8.9.;.<.E.K
+0000bbd0: 014c 014e 014f 0158 0160 0161 0163 0164  .L.N.O.X.`.a.c.d
+0000bbe0: 016d 0176 0177 017a 017b 0184 0193 0194  .m.v.w.z.{......
+0000bbf0: 0196 0197 01a0 01aa 01ab 01ac 01ad 01b6  ................
+0000bc00: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
+0000bc10: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+0000bc20: 0000 01c5 0000 0002 0075 0069 6c73 7670  .........u.ilsvp
+0000bc30: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+0000bc40: d801 0203 0405 0607 0809 0a0b 1a45 4647  .............EFG
+0000bc50: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+0000bc60: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+0000bc70: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000bc80: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000bc90: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000bca0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+0000bcb0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+0000bcc0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
+0000bcd0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
+0000bce0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+0000bcf0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+0000bd00: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+0000bd10: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+0000bd20: 696f 6e54 6e61 6d65 d416 1718 191a 0a1c  ionTname........
+0000bd30: 1d57 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
+0000bd40: 696e 6755 7769 6474 6855 696e 6465 7808  ingUwidthUindex.
+0000bd50: 0911 012c 1007 d416 1718 191a 1a21 2208  ...,.........!".
+0000bd60: 0810 c810 08d4 1617 1819 0a1a 2609 0908  ............&...
+0000bd70: 10b5 d416 1718 191a 1a26 2a08 0810 02d4  .........&*.....
+0000bd80: 1617 1819 0a1a 2e2f 0908 1061 1003 d416  ......./...a....
+0000bd90: 1718 191a 0a33 3408 0910 6410 05d4 1617  .....34...d.....
+0000bda0: 1819 0a0a 3839 0909 1073 1004 d416 1718  ....89...s......
+0000bdb0: 191a 0a3d 3e08 0910 4b10 06d4 1918 1716  ...=>...K.......
+0000bdc0: 4041 0a0a 1000 1101 c709 0908 2340 2800  @A..........#@(.
+0000bdd0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+0000bde0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+0000bdf0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+0000be00: 00ba 00c7 00d3 00d8 00de 00e3 00eb 00f0  ................
+0000be10: 00f9 0101 010b 0111 0117 0118 0119 011c  ................
+0000be20: 011e 0127 0128 0129 012b 012d 0136 0137  ...'.(.).+.-.6.7
+0000be30: 0138 013a 0143 0144 0145 0147 0150 0151  .8.:.C.D.E.G.P.Q
+0000be40: 0152 0154 0156 015f 0160 0161 0163 0165  .R.T.V._.`.a.c.e
+0000be50: 016e 016f 0170 0172 0174 017d 017e 017f  .n.o.p.r.t.}.~..
+0000be60: 0181 0183 018c 018e 0191 0192 0193 0194  ................
+0000be70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
+0000be80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000be90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
+0000bea0: 4444 626c 6f62 0000 0008 f6bf 1d48 cc0c  DDblob.......H..
+0000beb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
+0000bec0: 6f62 0000 0008 f6bf 1d48 cc0c c541 0000  ob.......H...A..
+0000bed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
+0000bee0: 0000 000c 5000 6f6c 6261 725b 5368 6f77  ....P.olbar[Show
 0000bef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 0000bf00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 0000bf10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 0000bf20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
 0000bf30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
 0000bf40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
 0000bf50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
 0000bf60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
 0000bf80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000bf90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
+0000bf90: 6f6d 7000 0000 0000 08bf a500 0000 0000  omp.............
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 00000000: 8004 950a 0000 0000 0000 008c 0630 2e35  .............0.5
-00000010: 322e 3094 2e80 0495 6903 0000 0000 0000  2.0.....i.......
-00000020: 4741 d90a e505 5138 344d 3e07 8694 7d94  GA....Q84M>...}.
-00000030: 8c12 2866 6c6f 6174 3634 5b3a 2c20 3a2c  ..(float64[:, :,
-00000040: 3a5d 2c29 948c 1978 3836 5f36 342d 6170  :],)...x86_64-ap
-00000050: 706c 652d 6461 7277 696e 3139 2e36 2e30  ple-darwin19.6.0
-00000060: 948c 0e69 6365 6c61 6b65 2d63 6c69 656e  ...icelake-clien
-00000070: 7494 5855 0200 002b 3634 6269 742c 2b61  t.XU...+64bit,+a
-00000080: 6478 2c2b 6165 732c 2b61 7678 2c2b 6176  dx,+aes,+avx,+av
-00000090: 7832 2c2d 6176 7835 3132 6266 3136 2c2b  x2,-avx512bf16,+
-000000a0: 6176 7835 3132 6269 7461 6c67 2c2b 6176  avx512bitalg,+av
-000000b0: 7835 3132 6277 2c2b 6176 7835 3132 6364  x512bw,+avx512cd
-000000c0: 2c2b 6176 7835 3132 6471 2c2d 6176 7835  ,+avx512dq,-avx5
-000000d0: 3132 6572 2c2b 6176 7835 3132 662c 2b61  12er,+avx512f,+a
-000000e0: 7678 3531 3269 666d 612c 2d61 7678 3531  vx512ifma,-avx51
-000000f0: 3270 662c 2b61 7678 3531 3276 626d 692c  2pf,+avx512vbmi,
-00000100: 2b61 7678 3531 3276 626d 6932 2c2b 6176  +avx512vbmi2,+av
-00000110: 7835 3132 766c 2c2b 6176 7835 3132 766e  x512vl,+avx512vn
-00000120: 6e69 2c2b 6176 7835 3132 7670 6f70 636e  ni,+avx512vpopcn
-00000130: 7464 712c 2b62 6d69 2c2b 626d 6932 2c2d  tdq,+bmi,+bmi2,-
-00000140: 636c 6465 6d6f 7465 2c2b 636c 666c 7573  cldemote,+clflus
-00000150: 686f 7074 2c2d 636c 7762 2c2d 636c 7a65  hopt,-clwb,-clze
-00000160: 726f 2c2b 636d 6f76 2c2b 6378 3136 2c2b  ro,+cmov,+cx16,+
-00000170: 6378 382c 2d65 6e71 636d 642c 2b66 3136  cx8,-enqcmd,+f16
-00000180: 632c 2b66 6d61 2c2d 666d 6134 2c2b 6673  c,+fma,-fma4,+fs
-00000190: 6773 6261 7365 2c2b 6678 7372 2c2b 6766  gsbase,+fxsr,+gf
-000001a0: 6e69 2c2b 696e 7670 6369 642c 2d6c 7770  ni,+invpcid,-lwp
-000001b0: 2c2b 6c7a 636e 742c 2b6d 6d78 2c2b 6d6f  ,+lzcnt,+mmx,+mo
-000001c0: 7662 652c 2d6d 6f76 6469 7236 3462 2c2d  vbe,-movdir64b,-
-000001d0: 6d6f 7664 6972 692c 2d6d 7761 6974 782c  movdiri,-mwaitx,
-000001e0: 2b70 636c 6d75 6c2c 2d70 636f 6e66 6967  +pclmul,-pconfig
-000001f0: 2c2d 706b 752c 2b70 6f70 636e 742c 2d70  ,-pku,+popcnt,-p
-00000200: 7265 6665 7463 6877 7431 2c2b 7072 6663  refetchwt1,+prfc
-00000210: 6877 2c2d 7074 7772 6974 652c 2b72 6470  hw,-ptwrite,+rdp
-00000220: 6964 2c2b 7264 726e 642c 2b72 6473 6565  id,+rdrnd,+rdsee
-00000230: 642c 2d72 746d 2c2b 7361 6866 2c2b 7367  d,-rtm,+sahf,+sg
-00000240: 782c 2b73 6861 2c2d 7368 7374 6b2c 2b73  x,+sha,-shstk,+s
-00000250: 7365 2c2b 7373 6532 2c2b 7373 6533 2c2b  se,+sse2,+sse3,+
-00000260: 7373 6534 2e31 2c2b 7373 6534 2e32 2c2d  sse4.1,+sse4.2,-
-00000270: 7373 6534 612c 2b73 7373 6533 2c2d 7462  sse4a,+ssse3,-tb
-00000280: 6d2c 2b76 6165 732c 2b76 7063 6c6d 756c  m,+vaes,+vpclmul
-00000290: 7164 712c 2d77 6169 7470 6b67 2c2d 7762  qdq,-waitpkg,-wb
-000002a0: 6e6f 696e 7664 2c2d 786f 702c 2b78 7361  noinvd,-xop,+xsa
-000002b0: 7665 2c2b 7873 6176 6563 2c2b 7873 6176  ve,+xsavec,+xsav
-000002c0: 656f 7074 2c2b 7873 6176 6573 9487 948c  eopt,+xsaves....
-000002d0: 4034 3637 3539 3865 3831 3732 3235 3763  @467598e8172257c
-000002e0: 6633 3730 6130 6536 3461 3535 3639 6330  f370a0e64a5569c0
-000002f0: 3935 6365 3466 6434 3162 3231 3361 3064  95ce4fd41b213a0d
-00000300: 6563 3761 6266 3430 3431 3563 6131 3834  ec7abf40415ca184
-00000310: 6294 8c40 6533 6230 6334 3432 3938 6663  b..@e3b0c44298fc
-00000320: 3163 3134 3961 6662 6634 6338 3939 3666  1c149afbf4c8996f
-00000330: 6239 3234 3237 6165 3431 6534 3634 3962  b92427ae41e4649b
-00000340: 3933 3463 6134 3935 3939 3162 3738 3532  934ca495991b7852
-00000350: 6238 3535 9486 9487 948c 2970 6572 696d  b855......)perim
-00000360: 6574 6572 5f6a 6974 2e71 7569 636b 6875  eter_jit.quickhu
-00000370: 6c6c 5f32 642d 3136 2e70 7933 366d 2e31  ll_2d-16.py36m.1
-00000380: 2e6e 6263 9473 8694 2e                   .nbc.s...
+00000010: 322e 3094 2e80 0495 3e04 0000 0000 0000  2.0.....>.......
+00000020: 4741 d919 e59a f585 9e4d ec90 8694 7d94  GA.......M....}.
+00000030: 288c 196e 756d 6261 2e63 6f72 652e 7479  (..numba.core.ty
+00000040: 7065 732e 6162 7374 7261 6374 948c 135f  pes.abstract..._
+00000050: 7479 7065 5f72 6563 6f6e 7374 7275 6374  type_reconstruct
+00000060: 6f72 9493 948c 0763 6f70 7972 6567 948c  or.....copyreg..
+00000070: 0e5f 7265 636f 6e73 7472 7563 746f 7294  ._reconstructor.
+00000080: 9394 8c18 6e75 6d62 612e 636f 7265 2e74  ....numba.core.t
+00000090: 7970 6573 2e73 6361 6c61 7273 948c 0546  ypes.scalars...F
+000000a0: 6c6f 6174 9493 948c 0862 7569 6c74 696e  loat.....builtin
+000000b0: 7394 8c06 6f62 6a65 6374 9493 944e 8794  s...object...N..
+000000c0: 7d94 288c 046e 616d 6594 8c07 666c 6f61  }.(..name...floa
+000000d0: 7433 3294 8c08 6269 7477 6964 7468 944b  t32...bitwidth.K
+000000e0: 208c 055f 636f 6465 944b 1675 8794 5294   .._code.K.u..R.
+000000f0: 6815 6815 6815 6815 6815 7494 8c19 7838  h.h.h.h.h.t...x8
+00000100: 365f 3634 2d61 7070 6c65 2d64 6172 7769  6_64-apple-darwi
+00000110: 6e31 392e 362e 3094 8c0e 6963 656c 616b  n19.6.0...icelak
+00000120: 652d 636c 6965 6e74 9458 5502 0000 2b36  e-client.XU...+6
+00000130: 3462 6974 2c2b 6164 782c 2b61 6573 2c2b  4bit,+adx,+aes,+
+00000140: 6176 782c 2b61 7678 322c 2d61 7678 3531  avx,+avx2,-avx51
+00000150: 3262 6631 362c 2b61 7678 3531 3262 6974  2bf16,+avx512bit
+00000160: 616c 672c 2b61 7678 3531 3262 772c 2b61  alg,+avx512bw,+a
+00000170: 7678 3531 3263 642c 2b61 7678 3531 3264  vx512cd,+avx512d
+00000180: 712c 2d61 7678 3531 3265 722c 2b61 7678  q,-avx512er,+avx
+00000190: 3531 3266 2c2b 6176 7835 3132 6966 6d61  512f,+avx512ifma
+000001a0: 2c2d 6176 7835 3132 7066 2c2b 6176 7835  ,-avx512pf,+avx5
+000001b0: 3132 7662 6d69 2c2b 6176 7835 3132 7662  12vbmi,+avx512vb
+000001c0: 6d69 322c 2b61 7678 3531 3276 6c2c 2b61  mi2,+avx512vl,+a
+000001d0: 7678 3531 3276 6e6e 692c 2b61 7678 3531  vx512vnni,+avx51
+000001e0: 3276 706f 7063 6e74 6471 2c2b 626d 692c  2vpopcntdq,+bmi,
+000001f0: 2b62 6d69 322c 2d63 6c64 656d 6f74 652c  +bmi2,-cldemote,
+00000200: 2b63 6c66 6c75 7368 6f70 742c 2d63 6c77  +clflushopt,-clw
+00000210: 622c 2d63 6c7a 6572 6f2c 2b63 6d6f 762c  b,-clzero,+cmov,
+00000220: 2b63 7831 362c 2b63 7838 2c2d 656e 7163  +cx16,+cx8,-enqc
+00000230: 6d64 2c2b 6631 3663 2c2b 666d 612c 2d66  md,+f16c,+fma,-f
+00000240: 6d61 342c 2b66 7367 7362 6173 652c 2b66  ma4,+fsgsbase,+f
+00000250: 7873 722c 2b67 666e 692c 2b69 6e76 7063  xsr,+gfni,+invpc
+00000260: 6964 2c2d 6c77 702c 2b6c 7a63 6e74 2c2b  id,-lwp,+lzcnt,+
+00000270: 6d6d 782c 2b6d 6f76 6265 2c2d 6d6f 7664  mmx,+movbe,-movd
+00000280: 6972 3634 622c 2d6d 6f76 6469 7269 2c2d  ir64b,-movdiri,-
+00000290: 6d77 6169 7478 2c2b 7063 6c6d 756c 2c2d  mwaitx,+pclmul,-
+000002a0: 7063 6f6e 6669 672c 2d70 6b75 2c2b 706f  pconfig,-pku,+po
+000002b0: 7063 6e74 2c2d 7072 6566 6574 6368 7774  pcnt,-prefetchwt
+000002c0: 312c 2b70 7266 6368 772c 2d70 7477 7269  1,+prfchw,-ptwri
+000002d0: 7465 2c2b 7264 7069 642c 2b72 6472 6e64  te,+rdpid,+rdrnd
+000002e0: 2c2b 7264 7365 6564 2c2d 7274 6d2c 2b73  ,+rdseed,-rtm,+s
+000002f0: 6168 662c 2b73 6778 2c2b 7368 612c 2d73  ahf,+sgx,+sha,-s
+00000300: 6873 746b 2c2b 7373 652c 2b73 7365 322c  hstk,+sse,+sse2,
+00000310: 2b73 7365 332c 2b73 7365 342e 312c 2b73  +sse3,+sse4.1,+s
+00000320: 7365 342e 322c 2d73 7365 3461 2c2b 7373  se4.2,-sse4a,+ss
+00000330: 7365 332c 2d74 626d 2c2b 7661 6573 2c2b  se3,-tbm,+vaes,+
+00000340: 7670 636c 6d75 6c71 6471 2c2d 7761 6974  vpclmulqdq,-wait
+00000350: 706b 672c 2d77 626e 6f69 6e76 642c 2d78  pkg,-wbnoinvd,-x
+00000360: 6f70 2c2b 7873 6176 652c 2b78 7361 7665  op,+xsave,+xsave
+00000370: 632c 2b78 7361 7665 6f70 742c 2b78 7361  c,+xsaveopt,+xsa
+00000380: 7665 7394 8794 8c40 3661 6466 3839 6465  ves....@6adf89de
+00000390: 6430 3263 6237 6463 3163 3937 3263 6239  d02cb7dc1c972cb9
+000003a0: 3030 3735 3934 6566 3166 3634 6362 6430  007594ef1f64cbd0
+000003b0: 6634 3664 3961 3437 6261 3035 3237 3762  f46d9a47ba05277b
+000003c0: 6662 3732 3234 6336 948c 4065 3362 3063  fb7224c6..@e3b0c
+000003d0: 3434 3239 3866 6331 6331 3439 6166 6266  44298fc1c149afbf
+000003e0: 3463 3839 3936 6662 3932 3432 3761 6534  4c8996fb92427ae4
+000003f0: 3165 3436 3439 6239 3334 6361 3439 3539  1e4649b934ca4959
+00000400: 3931 6237 3835 3262 3835 3594 8694 8794  91b7852b855.....
+00000410: 8c47 6665 6174 7572 655f 6578 7472 6163  .Gfeature_extrac
+00000420: 7469 6f6e 5f6d 6978 696e 2e46 6561 7475  tion_mixin.Featu
+00000430: 7265 4578 7472 6163 7469 6f6e 4d69 7869  reExtractionMixi
+00000440: 6e2e 616e 676c 6533 7074 2d38 342e 7079  n.angle3pt-84.py
+00000450: 3336 6d2e 312e 6e62 6394 7386 942e       36m.1.nbc.s...
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 00000000: 8004 950a 0000 0000 0000 008c 0630 2e35  .............0.5
-00000010: 322e 3094 2e80 0495 7503 0000 0000 0000  2.0.....u.......
-00000020: 4741 d90b 02ac ab25 dc4d 4a07 8694 7d94  GA.....%.MJ...}.
-00000030: 8c12 2866 6c6f 6174 3634 5b3a 2c20 3a2c  ..(float64[:, :,
-00000040: 3a5d 2c29 948c 1978 3836 5f36 342d 6170  :],)...x86_64-ap
-00000050: 706c 652d 6461 7277 696e 3139 2e36 2e30  ple-darwin19.6.0
-00000060: 948c 0e69 6365 6c61 6b65 2d63 6c69 656e  ...icelake-clien
-00000070: 7494 5855 0200 002b 3634 6269 742c 2b61  t.XU...+64bit,+a
-00000080: 6478 2c2b 6165 732c 2b61 7678 2c2b 6176  dx,+aes,+avx,+av
-00000090: 7832 2c2d 6176 7835 3132 6266 3136 2c2b  x2,-avx512bf16,+
-000000a0: 6176 7835 3132 6269 7461 6c67 2c2b 6176  avx512bitalg,+av
-000000b0: 7835 3132 6277 2c2b 6176 7835 3132 6364  x512bw,+avx512cd
-000000c0: 2c2b 6176 7835 3132 6471 2c2d 6176 7835  ,+avx512dq,-avx5
-000000d0: 3132 6572 2c2b 6176 7835 3132 662c 2b61  12er,+avx512f,+a
-000000e0: 7678 3531 3269 666d 612c 2d61 7678 3531  vx512ifma,-avx51
-000000f0: 3270 662c 2b61 7678 3531 3276 626d 692c  2pf,+avx512vbmi,
-00000100: 2b61 7678 3531 3276 626d 6932 2c2b 6176  +avx512vbmi2,+av
-00000110: 7835 3132 766c 2c2b 6176 7835 3132 766e  x512vl,+avx512vn
-00000120: 6e69 2c2b 6176 7835 3132 7670 6f70 636e  ni,+avx512vpopcn
-00000130: 7464 712c 2b62 6d69 2c2b 626d 6932 2c2d  tdq,+bmi,+bmi2,-
-00000140: 636c 6465 6d6f 7465 2c2b 636c 666c 7573  cldemote,+clflus
-00000150: 686f 7074 2c2d 636c 7762 2c2d 636c 7a65  hopt,-clwb,-clze
-00000160: 726f 2c2b 636d 6f76 2c2b 6378 3136 2c2b  ro,+cmov,+cx16,+
-00000170: 6378 382c 2d65 6e71 636d 642c 2b66 3136  cx8,-enqcmd,+f16
-00000180: 632c 2b66 6d61 2c2d 666d 6134 2c2b 6673  c,+fma,-fma4,+fs
-00000190: 6773 6261 7365 2c2b 6678 7372 2c2b 6766  gsbase,+fxsr,+gf
-000001a0: 6e69 2c2b 696e 7670 6369 642c 2d6c 7770  ni,+invpcid,-lwp
-000001b0: 2c2b 6c7a 636e 742c 2b6d 6d78 2c2b 6d6f  ,+lzcnt,+mmx,+mo
-000001c0: 7662 652c 2d6d 6f76 6469 7236 3462 2c2d  vbe,-movdir64b,-
-000001d0: 6d6f 7664 6972 692c 2d6d 7761 6974 782c  movdiri,-mwaitx,
-000001e0: 2b70 636c 6d75 6c2c 2d70 636f 6e66 6967  +pclmul,-pconfig
-000001f0: 2c2d 706b 752c 2b70 6f70 636e 742c 2d70  ,-pku,+popcnt,-p
-00000200: 7265 6665 7463 6877 7431 2c2b 7072 6663  refetchwt1,+prfc
-00000210: 6877 2c2d 7074 7772 6974 652c 2b72 6470  hw,-ptwrite,+rdp
-00000220: 6964 2c2b 7264 726e 642c 2b72 6473 6565  id,+rdrnd,+rdsee
-00000230: 642c 2d72 746d 2c2b 7361 6866 2c2b 7367  d,-rtm,+sahf,+sg
-00000240: 782c 2b73 6861 2c2d 7368 7374 6b2c 2b73  x,+sha,-shstk,+s
-00000250: 7365 2c2b 7373 6532 2c2b 7373 6533 2c2b  se,+sse2,+sse3,+
-00000260: 7373 6534 2e31 2c2b 7373 6534 2e32 2c2d  sse4.1,+sse4.2,-
-00000270: 7373 6534 612c 2b73 7373 6533 2c2d 7462  sse4a,+ssse3,-tb
-00000280: 6d2c 2b76 6165 732c 2b76 7063 6c6d 756c  m,+vaes,+vpclmul
-00000290: 7164 712c 2d77 6169 7470 6b67 2c2d 7762  qdq,-waitpkg,-wb
-000002a0: 6e6f 696e 7664 2c2d 786f 702c 2b78 7361  noinvd,-xop,+xsa
-000002b0: 7665 2c2b 7873 6176 6563 2c2b 7873 6176  ve,+xsavec,+xsav
-000002c0: 656f 7074 2c2b 7873 6176 6573 9487 948c  eopt,+xsaves....
-000002d0: 4034 3637 3539 3865 3831 3732 3235 3763  @467598e8172257c
-000002e0: 6633 3730 6130 6536 3461 3535 3639 6330  f370a0e64a5569c0
-000002f0: 3935 6365 3466 6434 3162 3231 3361 3064  95ce4fd41b213a0d
-00000300: 6563 3761 6266 3430 3431 3563 6131 3834  ec7abf40415ca184
-00000310: 6294 8c40 6533 6230 6334 3432 3938 6663  b..@e3b0c44298fc
-00000320: 3163 3134 3961 6662 6634 6338 3939 3666  1c149afbf4c8996f
-00000330: 6239 3234 3237 6165 3431 6534 3634 3962  b92427ae41e4649b
-00000340: 3933 3463 6134 3935 3939 3162 3738 3532  934ca495991b7852
-00000350: 6238 3535 9486 9487 948c 3570 6572 696d  b855......5perim
-00000360: 6574 6572 5f6a 6974 2e63 6f6e 7665 785f  eter_jit.convex_
-00000370: 6875 6c6c 5f70 6572 696d 6574 6572 5f32  hull_perimeter_2
-00000380: 642d 3136 2e70 7933 366d 2e31 2e6e 6263  d-16.py36m.1.nbc
-00000390: 9473 8694 2e                             .s...
+00000010: 322e 3094 2e80 0495 a704 0000 0000 0000  2.0.............
+00000020: 4741 d919 e59a f585 9e4d ec90 8694 7d94  GA.......M....}.
+00000030: 8c19 6e75 6d62 612e 636f 7265 2e74 7970  ..numba.core.typ
+00000040: 6573 2e61 6273 7472 6163 7494 8c13 5f74  es.abstract..._t
+00000050: 7970 655f 7265 636f 6e73 7472 7563 746f  ype_reconstructo
+00000060: 7294 9394 8c07 636f 7079 7265 6794 8c0e  r.....copyreg...
+00000070: 5f72 6563 6f6e 7374 7275 6374 6f72 9493  _reconstructor..
+00000080: 948c 196e 756d 6261 2e63 6f72 652e 7479  ...numba.core.ty
+00000090: 7065 732e 6e70 7974 7970 6573 948c 0541  pes.npytypes...A
+000000a0: 7272 6179 9493 948c 0862 7569 6c74 696e  rray.....builtin
+000000b0: 7394 8c06 6f62 6a65 6374 9493 944e 8794  s...object...N..
+000000c0: 7d94 288c 0564 7479 7065 9468 0468 078c  }.(..dtype.h.h..
+000000d0: 186e 756d 6261 2e63 6f72 652e 7479 7065  .numba.core.type
+000000e0: 732e 7363 616c 6172 7394 8c05 466c 6f61  s.scalars...Floa
+000000f0: 7494 9394 680d 4e87 947d 9428 8c04 6e61  t...h.N..}.(..na
+00000100: 6d65 948c 0766 6c6f 6174 3332 948c 0862  me...float32...b
+00000110: 6974 7769 6474 6894 4b20 8c05 5f63 6f64  itwidth.K .._cod
+00000120: 6594 4b16 7587 9452 948c 046e 6469 6d94  e.K.u..R...ndim.
+00000130: 4b02 8c06 6c61 796f 7574 948c 0141 9468  K...layout...A.h
+00000140: 168c 1561 7272 6179 2866 6c6f 6174 3332  ...array(float32
+00000150: 2c20 3264 2c20 4129 9468 194d f703 7587  , 2d, A).h.M..u.
+00000160: 9452 9468 2186 948c 1978 3836 5f36 342d  .R.h!....x86_64-
+00000170: 6170 706c 652d 6461 7277 696e 3139 2e36  apple-darwin19.6
+00000180: 2e30 948c 0e69 6365 6c61 6b65 2d63 6c69  .0...icelake-cli
+00000190: 656e 7494 5855 0200 002b 3634 6269 742c  ent.XU...+64bit,
+000001a0: 2b61 6478 2c2b 6165 732c 2b61 7678 2c2b  +adx,+aes,+avx,+
+000001b0: 6176 7832 2c2d 6176 7835 3132 6266 3136  avx2,-avx512bf16
+000001c0: 2c2b 6176 7835 3132 6269 7461 6c67 2c2b  ,+avx512bitalg,+
+000001d0: 6176 7835 3132 6277 2c2b 6176 7835 3132  avx512bw,+avx512
+000001e0: 6364 2c2b 6176 7835 3132 6471 2c2d 6176  cd,+avx512dq,-av
+000001f0: 7835 3132 6572 2c2b 6176 7835 3132 662c  x512er,+avx512f,
+00000200: 2b61 7678 3531 3269 666d 612c 2d61 7678  +avx512ifma,-avx
+00000210: 3531 3270 662c 2b61 7678 3531 3276 626d  512pf,+avx512vbm
+00000220: 692c 2b61 7678 3531 3276 626d 6932 2c2b  i,+avx512vbmi2,+
+00000230: 6176 7835 3132 766c 2c2b 6176 7835 3132  avx512vl,+avx512
+00000240: 766e 6e69 2c2b 6176 7835 3132 7670 6f70  vnni,+avx512vpop
+00000250: 636e 7464 712c 2b62 6d69 2c2b 626d 6932  cntdq,+bmi,+bmi2
+00000260: 2c2d 636c 6465 6d6f 7465 2c2b 636c 666c  ,-cldemote,+clfl
+00000270: 7573 686f 7074 2c2d 636c 7762 2c2d 636c  ushopt,-clwb,-cl
+00000280: 7a65 726f 2c2b 636d 6f76 2c2b 6378 3136  zero,+cmov,+cx16
+00000290: 2c2b 6378 382c 2d65 6e71 636d 642c 2b66  ,+cx8,-enqcmd,+f
+000002a0: 3136 632c 2b66 6d61 2c2d 666d 6134 2c2b  16c,+fma,-fma4,+
+000002b0: 6673 6773 6261 7365 2c2b 6678 7372 2c2b  fsgsbase,+fxsr,+
+000002c0: 6766 6e69 2c2b 696e 7670 6369 642c 2d6c  gfni,+invpcid,-l
+000002d0: 7770 2c2b 6c7a 636e 742c 2b6d 6d78 2c2b  wp,+lzcnt,+mmx,+
+000002e0: 6d6f 7662 652c 2d6d 6f76 6469 7236 3462  movbe,-movdir64b
+000002f0: 2c2d 6d6f 7664 6972 692c 2d6d 7761 6974  ,-movdiri,-mwait
+00000300: 782c 2b70 636c 6d75 6c2c 2d70 636f 6e66  x,+pclmul,-pconf
+00000310: 6967 2c2d 706b 752c 2b70 6f70 636e 742c  ig,-pku,+popcnt,
+00000320: 2d70 7265 6665 7463 6877 7431 2c2b 7072  -prefetchwt1,+pr
+00000330: 6663 6877 2c2d 7074 7772 6974 652c 2b72  fchw,-ptwrite,+r
+00000340: 6470 6964 2c2b 7264 726e 642c 2b72 6473  dpid,+rdrnd,+rds
+00000350: 6565 642c 2d72 746d 2c2b 7361 6866 2c2b  eed,-rtm,+sahf,+
+00000360: 7367 782c 2b73 6861 2c2d 7368 7374 6b2c  sgx,+sha,-shstk,
+00000370: 2b73 7365 2c2b 7373 6532 2c2b 7373 6533  +sse,+sse2,+sse3
+00000380: 2c2b 7373 6534 2e31 2c2b 7373 6534 2e32  ,+sse4.1,+sse4.2
+00000390: 2c2d 7373 6534 612c 2b73 7373 6533 2c2d  ,-sse4a,+ssse3,-
+000003a0: 7462 6d2c 2b76 6165 732c 2b76 7063 6c6d  tbm,+vaes,+vpclm
+000003b0: 756c 7164 712c 2d77 6169 7470 6b67 2c2d  ulqdq,-waitpkg,-
+000003c0: 7762 6e6f 696e 7664 2c2d 786f 702c 2b78  wbnoinvd,-xop,+x
+000003d0: 7361 7665 2c2b 7873 6176 6563 2c2b 7873  save,+xsavec,+xs
+000003e0: 6176 656f 7074 2c2b 7873 6176 6573 9487  aveopt,+xsaves..
+000003f0: 948c 4033 6330 3233 3230 6562 3131 6239  ..@3c02320eb11b9
+00000400: 6338 3363 6563 6538 3630 6363 3934 3663  c83cece860cc946c
+00000410: 3835 3834 6463 3138 6638 3838 6632 3965  8584dc18f888f29e
+00000420: 6239 3939 3133 3930 3734 6130 6561 6630  b999139074a0eaf0
+00000430: 3139 3294 8c40 6533 6230 6334 3432 3938  192..@e3b0c44298
+00000440: 6663 3163 3134 3961 6662 6634 6338 3939  fc1c149afbf4c899
+00000450: 3666 6239 3234 3237 6165 3431 6534 3634  6fb92427ae41e464
+00000460: 3962 3933 3463 6134 3935 3939 3162 3738  9b934ca495991b78
+00000470: 3532 6238 3535 9486 9487 948c 4566 6561  52b855......Efea
+00000480: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
+00000490: 6d69 7869 6e2e 4665 6174 7572 6545 7874  mixin.FeatureExt
+000004a0: 7261 6374 696f 6e4d 6978 696e 2e63 6469  ractionMixin.cdi
+000004b0: 7374 2d33 3333 2e70 7933 366d 2e31 2e6e  st-333.py36m.1.n
+000004c0: 6263 9473 8694 2e                        bc.s...
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,16 @@
             self.data_df_comb = pd.concat([self.data_df, self.data_df_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
             self.__euclid_dist_between_bps_of_other_animals()
             self.__movement_of_all_bps()
             self.__rolling_windows_bp_distances()
             self.__rolling_windows_movement()
             self.__pose_probability_filters()
             save_path = os.path.join(self.save_dir, file_name + '.' + self.file_type)
-            self.data_df = self.data_df.reset_index(drop=True).fillna(0)
-            write_df(df=self.data_df, file_type=self.file_type, save_path=save_path)
+            self.out_data = self.data_df.reset_index(drop=True).fillna(0)
+            write_df(df=self.out_data, file_type=self.file_type, save_path=save_path)
             video_timer.stop_timer()
             print(f'Feature extraction complete for video {file_name} (elapsed time: {video_timer.elapsed_time_str}s)')
 
         self.timer.stop_timer()
         stdout_success(f'Feature extraction complete for {str(len(self.files_found))} video(s). Results are saved inside the project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = UserDefinedFeatureExtractor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.3/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/requirements.txt` & `Simba-UW-tf-dev-1.60.3/simba/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 # tkinter_functions.py: 2
 # train_model\train_model_user_defined.py: 21
 # train_model_2.py: 21
 # train_model_3_scramble.py: 20
 # train_multiple_models_from_meta.py: 21
 # train_multiple_models_from_meta_scramble.py: 21
 # validate_model_on_single_video.py: 14
-numpy == 1.18.1
+
 
 # ROI_draw_defined.py: 3
 # ROI_freehand_draw_3.py: 3
 # ROI_plot.py: 4
 # ROI_plot_multi_process.py: 4
 # ROI_visualize_features.py: 7
 # SimBA.py: 24
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files 11% similar despite different names*

```diff
@@ -1,3119 +1,3239 @@
-00000000: 8004 95db c200 0000 0000 0028 8c1c 4665  ...........(..Fe
+00000000: 8004 9556 ca00 0000 0000 0028 8c1c 4665  ...V.......(..Fe
 00000010: 6174 7572 6545 7874 7261 6374 696f 6e4d  atureExtractionM
 00000020: 6978 696e 2e63 6469 7374 948c 066f 626a  ixin.cdist...obj
-00000030: 6563 7494 4228 3200 00cf faed fe07 0000  ect.B(2.........
+00000030: 6563 7494 4238 3200 00cf faed fe07 0000  ect.B82.........
 00000040: 0103 0000 0001 0000 0004 0000 0050 0200  .............P..
 00000050: 0000 2000 0000 0000 0019 0000 00d8 0100  .. .............
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000070: 0000 0000 0000 0000 0018 1c00 0000 0000  ................
-00000080: 0070 0200 0000 0000 0018 1c00 0000 0000  .p..............
+00000070: 0000 0000 0000 0000 0028 1c00 0000 0000  .........(......
+00000080: 0070 0200 0000 0000 0028 1c00 0000 0000  .p.......(......
 00000090: 0007 0000 0007 0000 0005 0000 0000 0000  ................
 000000a0: 005f 5f74 6578 7400 0000 0000 0000 0000  .__text.........
 000000b0: 005f 5f54 4558 5400 0000 0000 0000 0000  .__TEXT.........
-000000c0: 0000 0000 0000 0000 00eb 1200 0000 0000  ................
-000000d0: 0070 0200 0004 0000 0088 1e00 0044 0000  .p...........D..
+000000c0: 0000 0000 0000 0000 00fb 1200 0000 0000  ................
+000000d0: 0070 0200 0004 0000 0098 1e00 0044 0000  .p...........D..
 000000e0: 0000 0400 8000 0000 0000 0000 0000 0000  ................
 000000f0: 005f 5f63 6f6e 7374 0000 0000 0000 0000  .__const........
 00000100: 005f 5f44 4154 4100 0000 0000 0000 0000  .__DATA.........
-00000110: 00f0 1200 0000 0000 00f8 0000 0000 0000  ................
-00000120: 0060 1500 0004 0000 00a8 2000 0010 0000  .`........ .....
+00000110: 0000 1300 0000 0000 00f8 0000 0000 0000  ................
+00000120: 0070 1500 0004 0000 00b8 2000 0010 0000  .p........ .....
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 005f 5f63 6f6e 7374 0000 0000 0000 0000  .__const........
 00000150: 005f 5f54 4558 5400 0000 0000 0000 0000  .__TEXT.........
-00000160: 00f0 1300 0000 0000 0074 0600 0000 0000  .........t......
-00000170: 0060 1600 0004 0000 0000 0000 0000 0000  .`..............
+00000160: 0000 1400 0000 0000 0074 0600 0000 0000  .........t......
+00000170: 0070 1600 0004 0000 0000 0000 0000 0000  .p..............
 00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000190: 005f 5f63 6f6d 7061 6374 5f75 6e77 696e  .__compact_unwin
 000001a0: 645f 5f4c 4400 0000 0000 0000 0000 0000  d__LD...........
-000001b0: 0068 1a00 0000 0000 0080 0000 0000 0000  .h..............
-000001c0: 00d8 1c00 0003 0000 0028 2100 0004 0000  .........(!.....
+000001b0: 0078 1a00 0000 0000 0080 0000 0000 0000  .x..............
+000001c0: 00e8 1c00 0003 0000 0038 2100 0004 0000  .........8!.....
 000001d0: 0000 0000 0200 0000 0000 0000 0000 0000  ................
 000001e0: 005f 5f65 685f 6672 616d 6500 0000 0000  .__eh_frame.....
 000001f0: 005f 5f54 4558 5400 0000 0000 0000 0000  .__TEXT.........
-00000200: 00e8 1a00 0000 0000 0030 0100 0000 0000  .........0......
-00000210: 0058 1d00 0003 0000 0000 0000 0000 0000  .X..............
+00000200: 00f8 1a00 0000 0000 0030 0100 0000 0000  .........0......
+00000210: 0068 1d00 0003 0000 0000 0000 0000 0000  .h..............
 00000220: 000b 0000 6800 0000 0000 0000 0000 0000  ....h...........
 00000230: 0024 0000 0010 0000 0000 0f0a 0000 0000  .$..............
-00000240: 0002 0000 0018 0000 0048 2100 0046 0000  .........H!..F..
-00000250: 00a8 2500 0080 0c00 000b 0000 0050 0000  ..%..........P..
+00000240: 0002 0000 0018 0000 0058 2100 0046 0000  .........X!..F..
+00000250: 00b8 2500 0080 0c00 000b 0000 0050 0000  ..%..........P..
 00000260: 0000 0000 001f 0000 001f 0000 0007 0000  ................
 00000270: 0026 0000 0020 0000 0000 0000 0000 0000  .&... ..........
 00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002a0: 0000 0000 0000 0000 0055 4157 4156 4155  .........UAWAVAU
 000002b0: 4154 5348 81ec 1801 0000 4989 f549 89fe  ATSH......I..I..
 000002c0: 4c8b bc24 a001 0000 488b ac24 7801 0000  L..$....H..$x...
 000002d0: 4c8b a424 5801 0000 48bb 0000 0000 0000  L..$X...H.......
-000002e0: 0000 4889 5424 4048 89d7 ffd3 4889 efff  ..H.T$@H....H...
-000002f0: d3b8 0100 0000 4c89 f94c 09e1 0f88 8d09  ......L..L......
+000002e0: 0000 4889 5424 4848 89d7 ffd3 4889 efff  ..H.T$HH....H...
+000002f0: d3b8 0100 0000 4c89 f94c 09e1 0f88 9d09  ......L..L......
 00000300: 0000 4c89 e64c 89e1 490f afcf 486b f908  ..L..L..I...Hk..
 00000310: 0f90 c249 0faf f748 b900 0000 0000 0000  ...I...H........
-00000320: 000f 8072 0900 0084 d20f 856a 0900 0048  ...r.......j...H
+00000320: 000f 8082 0900 0084 d20f 857a 0900 0048  ...........z...H
 00000330: 89b4 24a8 0000 004c 89b4 24b0 0000 004c  ..$....L..$....L
-00000340: 896c 2430 48b8 0000 0000 0000 0000 be20  .l$0H.......... 
+00000340: 896c 2438 48b8 0000 0000 0000 0000 be20  .l$8H.......... 
 00000350: 0000 00ff d04c 8b84 2458 0100 0048 8984  .....L..$X...H..
 00000360: 24a0 0000 0048 8b40 184d 85c0 745a 4d85  $....H.@.M..tZM.
 00000370: ff74 5531 ed49 b900 0000 0000 00f8 7f31  .tU1.I.........1
 00000380: f60f 1f84 0000 0000 0048 89f7 4889 e948  .........H..H..H
 00000390: 8d56 0148 8d5d 014c 39c3 bd00 0000 0048  .V.H.].L9......H
 000003a0: 0f4c eb4c 39fa be00 0000 0048 0f4c f248  .L.L9......H.L.H
 000003b0: 0f4c e949 0faf cf48 01f9 4c89 0cc8 4c39  .L.I...H..L...L9
-000003c0: c37c c64c 39fa 7cc1 4889 4424 604d 85c0  .|.L9.|.H.D$`M..
-000003d0: 0f8e 0508 0000 488b 9424 b801 0000 488b  ......H..$....H.
+000003c0: c37c c64c 39fa 7cc1 4889 4424 684d 85c0  .|.L9.|.H.D$hM..
+000003d0: 0f8e 1508 0000 488b 9424 b801 0000 488b  ......H..$....H.
 000003e0: b424 a801 0000 488b bc24 6001 0000 31c0  .$....H..$`...1.
 000003f0: 4d85 ff0f 9fc0 4c89 f948 c1f9 3fc4 c2f0  M.....L..H..?...
 00000400: f2cf 4829 c148 898c 24b8 0000 0048 39fe  ..H).H..$....H9.
 00000410: 0f94 c048 83ff 010f 94c1 480f 44fe 08c1  ...H......H.D...
 00000420: 4883 fe01 0f94 c048 0f45 fe08 c888 4424  H......H.E....D$
-00000430: 1e48 6bc7 0848 8984 24f8 0000 000f 9044  .Hk..H..$......D
-00000440: 241f 488d 47f0 48c1 e804 4889 8424 9800  $.H.G.H...H..$..
-00000450: 0000 48ff c048 89f9 4883 e1f0 4889 8c24  ..H..H..H...H..$
+00000430: 1e48 6bc7 0448 8984 24f8 0000 000f 9044  .Hk..H..$......D
+00000440: 241f 488d 47e0 48c1 e805 4889 8424 9800  $.H.G.H...H..$..
+00000450: 0000 48ff c048 89f9 4883 e1e0 4889 8c24  ..H..H..H...H..$
 00000460: 9000 0000 89c1 83e1 0148 898c 2488 0000  .........H..$...
 00000470: 0048 83e0 fe48 8984 2480 0000 0089 f883  .H...H..$.......
 00000480: e007 4889 8424 c800 0000 89f8 83e0 0348  ..H..$.........H
 00000490: 8984 24f0 0000 0048 89f8 4883 e0fc 4889  ..$....H..H...H.
-000004a0: 4424 3848 8b84 2470 0100 0049 8d70 ff48  D$8H..$p...I.p.H
-000004b0: 89f9 4889 7c24 2048 8d4f ff48 894c 2428  ..H.|$ H.O.H.L$(
-000004c0: 488d 0c40 4889 4c24 5848 8d04 8500 0000  H..@H.L$XH......
-000004d0: 0048 8944 2450 488d 0452 4889 8424 e800  .H.D$PH..RH..$..
-000004e0: 0000 488d 0495 0000 0000 4889 4424 4845  ..H.......H.D$HE
+000004a0: 4424 4048 8b84 2470 0100 0049 8d70 ff48  D$@H..$p...I.p.H
+000004b0: 89f9 4889 7c24 2048 8d4f ff48 894c 2430  ..H.|$ H.O.H.L$0
+000004c0: 488d 0c40 4889 4c24 6048 8d04 8500 0000  H..@H.L$`H......
+000004d0: 0048 8944 2458 488d 0452 4889 8424 e800  .H.D$XH..RH..$..
+000004e0: 0000 488d 0495 0000 0000 4889 4424 5045  ..H.......H.D$PE
 000004f0: 31e4 eb32 0f1f 4400 0031 c048 8b94 24d0  1..2..D..1.H..$.
 00000500: 0000 0048 85d2 0f9f c048 89d1 4829 c149  ...H.....H..H).I
 00000510: ffc4 4885 d248 89ce 4c8b 8424 5801 0000  ..H..H..L..$X...
-00000520: 0f8e b506 0000 4889 b424 d000 0000 4d85  ......H..$....M.
+00000520: 0f8e c506 0000 4889 b424 d000 0000 4d85  ......H..$....M.
 00000530: ff7e c64c 89e0 48c1 f83f 4823 8424 5801  .~.L..H..?H#.$X.
 00000540: 0000 4c01 e049 89c5 4c0f afac 2468 0100  ..L..I..L...$h..
-00000550: 0049 0faf c748 8b4c 2460 488d 04c1 4889  .I...H.L$`H...H.
+00000550: 0049 0faf c748 8b4c 2468 488d 04c1 4889  .I...H.L$hH...H.
 00000560: 8424 e000 0000 488b 8424 5001 0000 4a8d  .$....H..$P...J.
 00000570: 0c28 48ff c148 898c 24c0 0000 0049 01c5  .(H..H..$....I..
 00000580: 31ed 8a5c 241e 488b 8c24 b800 0000 4c89  1..\$.H..$....L.
-00000590: a424 d800 0000 eb52 9048 8b44 2478 488b  .$.....R.H.D$xH.
-000005a0: 8c24 e000 0000 488b 5424 6848 8904 d148  .$....H.T$hH...H
-000005b0: 89df 48b8 0000 0000 0000 0000 ffd0 31c0  ..H...........1.
-000005c0: 488b 9424 1001 0000 4885 d20f 9fc0 4889  H..$....H.....H.
-000005d0: d148 29c1 488b ac24 0001 0000 48ff c5b3  .H).H..$....H...
-000005e0: 0148 85d2 0f8e 0fff ffff 4889 8c24 1001  .H........H..$..
-000005f0: 0000 488b 7c24 4049 be00 0000 0000 0000  ..H.|$@I........
-00000600: 0041 ffd6 488b bc24 7801 0000 41ff d6f6  .A..H..$x...A...
-00000610: c301 0f84 3206 0000 807c 241f 000f 8543  ....2....|$....C
-00000620: 0600 0048 89e8 48c1 f83f 4c21 f848 89ac  ...H..H..?L!.H..
-00000630: 2400 0100 0048 01e8 4889 4424 6848 8bbc  $....H..H.D$hH..
-00000640: 24f8 0000 00be 2000 0000 48b8 0000 0000  $..... ...H.....
-00000650: 0000 0000 ffd0 4889 8424 0801 0000 488b  ......H..$....H.
-00000660: 6818 4883 7c24 2000 4c8b 9c24 b801 0000  h.H.|$ .L..$....
-00000670: 4c8b 8c24 f000 0000 4c8b b424 7001 0000  L..$....L..$p...
-00000680: 488b 9c24 e800 0000 0f8e ab03 0000 4c8b  H..$..........L.
-00000690: 4424 684c 0faf 8424 b001 0000 488b 8424  D$hL...$....H..$
-000006a0: 9801 0000 4c01 c048 83bc 24a8 0100 0002  ....L..H..$.....
-000006b0: 7227 4883 bc24 6001 0000 0176 3a48 837c  r'H..$`....v:H.|
-000006c0: 2428 034c 8b54 2438 0f83 2f01 0000 31c0  $(.L.T$8../...1.
-000006d0: e9a5 0100 000f 1f40 0048 83bc 2460 0100  .......@.H..$`..
-000006e0: 0002 722b 4883 7c24 2803 0f83 e901 0000  ..r+H.|$(.......
-000006f0: 31c9 e94b 0200 0048 837c 2428 0348 8b4c  1..K...H.|$(.H.L
-00000700: 2438 0f83 7e02 0000 31d2 e9db 0200 0048  $8..~...1......H
-00000710: 837c 2420 0f0f 87a6 0300 0031 c948 8b54  .|$ .......1.H.T
-00000720: 2428 4829 ca48 8bb4 24c8 0000 0048 85f6  $(H).H..$....H..
-00000730: 741f 0f1f 8000 0000 00c4 c17b 1045 00c5  t..........{.E..
-00000740: fb5c 00c5 fb11 44cd 0048 ffc1 48ff ce75  .\....D..H..H..u
-00000750: e848 83fa 070f 82de 0200 0066 2e0f 1f84  .H.........f....
-00000760: 0000 0000 000f 1f40 00c4 c17b 1045 00c5  .......@...{.E..
-00000770: fb5c 00c5 fb11 44cd 00c4 c17b 1045 00c5  .\....D....{.E..
-00000780: fb5c 00c5 fb11 44cd 08c4 c17b 1045 00c5  .\....D....{.E..
-00000790: fb5c 00c5 fb11 44cd 10c4 c17b 1045 00c5  .\....D....{.E..
-000007a0: fb5c 00c5 fb11 44cd 18c4 c17b 1045 00c5  .\....D....{.E..
-000007b0: fb5c 00c5 fb11 44cd 20c4 c17b 1045 00c5  .\....D. ..{.E..
-000007c0: fb5c 00c5 fb11 44cd 28c4 c17b 1045 00c5  .\....D.(..{.E..
-000007d0: fb5c 00c5 fb11 44cd 30c4 c17b 1045 00c5  .\....D.0..{.E..
-000007e0: fb5c 00c5 fb11 44cd 3848 83c1 0848 394c  .\....D.8H...H9L
-000007f0: 2420 0f85 71ff ffff e93c 0200 0048 8b84  $ ..q....<...H..
-00000800: 2498 0100 0049 8d14 004c 89ee 31c0 488b  $....I...L..1.H.
-00000810: 4c24 5848 8b7c 2450 4c8b 6424 4866 2e0f  L$XH.|$PL.d$Hf..
-00000820: 1f84 0000 0000 0066 90c5 fb10 06c5 fb5c  .......f.......\
-00000830: 02c5 fb11 44c5 00c4 c17b 1004 36c4 c17b  ....D....{..6..{
-00000840: 5c04 13c5 fb11 44c5 08c4 a17b 1004 76c4  \.....D....{..v.
-00000850: a17b 5c04 5ac5 fb11 44c5 10c5 fb10 0431  .{\.Z...D......1
-00000860: c5fb 5c04 13c5 fb11 44c5 1848 83c0 044c  ..\.....D..H...L
-00000870: 01e2 4801 fe49 39c2 75af f644 2420 034c  ..H..I9.u..D$ .L
-00000880: 8ba4 24d8 0000 000f 84ac 0100 0048 8d14  ..$..........H..
-00000890: c500 0000 0048 01ea 4c89 f648 0faf f04c  .....H..L..H...L
-000008a0: 01ee 490f afc3 4803 8424 9801 0000 4c01  ..I...H..$....L.
-000008b0: c031 c966 0f1f 4400 00c5 fb10 06c5 fb5c  .1.f..D........\
-000008c0: 00c5 fb11 04ca 48ff c14c 01f6 4c01 d849  ......H..L..L..I
-000008d0: 39c9 75e5 e960 0100 004c 89ea 31c9 488b  9.u..`...L..1.H.
-000008e0: 7424 3848 8b7c 2458 488b 5c24 5066 2e0f  t$8H.|$XH.\$Pf..
-000008f0: 1f84 0000 0000 0066 90c5 fb10 02c5 fb5c  .......f.......\
-00000900: 00c5 fb11 44cd 00c4 c17b 1004 16c5 fb5c  ....D....{.....\
-00000910: 00c5 fb11 44cd 08c4 a17b 1004 72c5 fb5c  ....D....{..r..\
-00000920: 00c5 fb11 44cd 10c5 fb10 0417 c5fb 5c00  ....D.........\.
-00000930: c5fb 1144 cd18 4883 c104 4801 da48 39ce  ...D..H...H..H9.
-00000940: 75b7 4d85 c90f 84ee 0000 0048 8d14 cd00  u.M........H....
-00000950: 0000 0048 01ea 490f afce 4c01 e931 f666  ...H..I...L..1.f
-00000960: 2e0f 1f84 0000 0000 00c5 fb10 01c5 fb5c  ...............\
-00000970: 00c5 fb11 04f2 48ff c64c 01f1 4939 f175  ......H..L..I9.u
-00000980: e8e9 b300 0000 31d2 488b 7424 4866 2e0f  ......1.H.t$Hf..
-00000990: 1f84 0000 0000 0066 90c4 c17b 1045 00c5  .......f...{.E..
-000009a0: fb5c 00c5 fb11 44d5 00c4 c17b 1045 00c4  .\....D....{.E..
-000009b0: c17b 5c04 03c5 fb11 44d5 08c4 c17b 1045  .{\.....D....{.E
-000009c0: 00c4 a17b 5c04 58c5 fb11 44d5 10c4 c17b  ...{\.X...D....{
-000009d0: 1045 00c5 fb5c 0403 c5fb 1144 d518 4883  .E...\.....D..H.
-000009e0: c204 4801 f048 39d1 75af f644 2420 0374  ..H..H9.u..D$ .t
-000009f0: 4848 8d04 d500 0000 0048 01e8 490f afd3  HH.......H..I...
-00000a00: 4803 9424 9801 0000 4c01 c231 c966 2e0f  H..$....L..1.f..
-00000a10: 1f84 0000 0000 0066 90c4 c17b 1045 00c5  .......f...{.E..
-00000a20: fb5c 02c5 fb11 04c8 48ff c14c 01da 4939  .\......H..L..I9
-00000a30: c975 e666 0f1f 4400 0048 8b7c 2440 49be  .u.f..D..H.|$@I.
-00000a40: 0000 0000 0000 0000 c5f8 7741 ffd6 488b  ..........wA..H.
-00000a50: bc24 7801 0000 41ff d64c 8b44 2420 48c7  .$x...A..L.D$ H.
-00000a60: 4424 7000 0000 0048 c744 2478 0000 0000  D$p....H.D$x....
-00000a70: 4c89 4424 0848 892c 2448 c744 2410 0800  L.D$.H.,$H.D$...
-00000a80: 0000 41b9 0800 0000 488d 7c24 7848 8d74  ..A.....H.|$xH.t
-00000a90: 2470 488b 9c24 0801 0000 4889 da31 c948  $pH..$....H..1.H
-00000aa0: b800 0000 0000 0000 00ff d085 c00f 84e6  ................
-00000ab0: faff ff83 f8fe 0f84 ddfa ffff e995 0100  ................
-00000ac0: 0048 8b4c 2420 488d 0ccd 0000 0000 4801  .H.L$ H.......H.
-00000ad0: e948 8d50 0148 39ea 400f 97c7 4839 c841  .H.P.H9.@...H9.A
-00000ae0: 0f92 c048 39ac 24c0 0000 000f 97c2 4939  ...H9.$.......I9
-00000af0: cd40 0f92 c644 84c7 0f85 1dfc ffff b900  .@...D..........
-00000b00: 0000 0040 20f2 0f85 11fc ffff 4883 bc24  ...@ .......H..$
-00000b10: 9800 0000 000f 84b1 0000 00c4 c17b 1045  .............{.E
-00000b20: 00c5 fb5c 00c4 e27d 19c0 31c9 488b 9424  ...\...}..1.H..$
-00000b30: 8000 0000 0f1f 4400 00c5 fd11 44cd 00c5  ......D.....D...
-00000b40: fd11 44cd 20c5 fd11 44cd 40c5 fd11 44cd  ..D. ...D.@...D.
-00000b50: 60c5 fd11 84cd 8000 0000 c5fd 1184 cda0  `...............
-00000b60: 0000 00c5 fd11 84cd c000 0000 c5fd 1184  ................
-00000b70: cde0 0000 0048 83c1 2048 83c2 fe75 ba48  .....H.. H...u.H
-00000b80: 83bc 2488 0000 0000 7427 c4c1 7b10 4500  ..$.....t'..{.E.
-00000b90: c5fb 5c00 c4e2 7d19 c0c5 fd11 44cd 00c5  ..\...}.....D...
-00000ba0: fd11 44cd 20c5 fd11 44cd 40c5 fd11 44cd  ..D. ...D.@...D.
-00000bb0: 6048 8b94 2490 0000 0048 89d1 4839 5424  `H..$....H..H9T$
-00000bc0: 200f 8556 fbff ffe9 6dfe ffff 31c9 4883   ..V....m...1.H.
-00000bd0: bc24 8800 0000 0075 b1eb d648 8b84 24b0  .$.....u...H..$.
-00000be0: 0000 0048 8b8c 24a0 0000 0048 8908 48c7  ...H..$....H..H.
-00000bf0: 4008 0000 0000 488b 8c24 a800 0000 4889  @.....H..$....H.
-00000c00: 4810 48c7 4018 0800 0000 488b 4c24 6048  H.H.@.....H.L$`H
-00000c10: 8948 204c 8940 284c 8978 3049 c1e7 034c  .H L.@(L.x0I...L
-00000c20: 8978 3848 c740 4008 0000 0048 8bbc 2478  .x8H.@@....H..$x
-00000c30: 0100 0048 bb00 0000 0000 0000 00ff d348  ...H...........H
-00000c40: 8b7c 2440 ffd3 31c0 eb33 48b8 0000 0000  .|$@..1..3H.....
-00000c50: 0000 0000 eb1a 488b 4c24 704c 8b6c 2430  ......H.L$pL.l$0
-00000c60: 4989 4d00 eb17 48b8 0000 0000 0000 0000  I.M...H.........
-00000c70: 488b 4c24 3048 8901 b801 0000 0048 81c4  H.L$0H.......H..
-00000c80: 1801 0000 5b41 5c41 5d41 5e41 5f5d c348  ....[A\A]A^A_].H
-00000c90: b900 0000 0000 0000 0049 894d 00eb de66  .........I.M...f
-00000ca0: 2e0f 1f84 0000 0000 0055 4889 e541 5741  .........UH..AWA
-00000cb0: 5641 5541 5453 4883 e4e0 4881 ec80 0200  VAUATSH...H.....
-00000cc0: 0048 89f7 48be 0000 0000 0000 0000 48bb  .H..H.........H.
-00000cd0: 0000 0000 0000 0000 4c8d 8424 9800 0000  ........L..$....
-00000ce0: 4c8d 8c24 9000 0000 ba02 0000 00b9 0200  L..$............
-00000cf0: 0000 31c0 ffd3 c5f8 57c0 c5fc 2984 24a0  ..1.....W...).$.
-00000d00: 0000 00c5 fc29 8424 c000 0000 48c7 8424  .....).$....H..$
-00000d10: e000 0000 0000 0000 c5fc 2984 2400 0100  ..........).$...
-00000d20: 00c5 fc29 8424 2001 0000 48c7 8424 4001  ...).$ ...H..$@.
-00000d30: 0000 0000 0000 c5fc 2984 2460 0100 00c5  ........).$`....
-00000d40: fc29 8424 8001 0000 48c7 8424 a001 0000  .).$....H..$....
-00000d50: 0000 0000 48c7 8424 8000 0000 0000 0000  ....H..$........
-00000d60: c5fc 2984 24e0 0100 00c5 fc29 8424 0002  ..).$......).$..
-00000d70: 0000 48c7 8424 2002 0000 0000 0000 85c0  ..H..$ .........
-00000d80: 0f84 7403 0000 48b8 0000 0000 0000 0000  ..t...H.........
-00000d90: 488b 1848 85db 0f84 2503 0000 488b bc24  H..H....%...H..$
-00000da0: 9800 0000 c5f8 57c0 c5fc 2984 24a0 0000  ......W...).$...
-00000db0: 00c5 fc29 8424 c000 0000 48c7 8424 e000  ...).$....H..$..
-00000dc0: 0000 0000 0000 49bc 0000 0000 0000 0000  ......I.........
-00000dd0: 488d b424 a000 0000 c5f8 7741 ffd4 85c0  H..$......wA....
-00000de0: 0f85 f102 0000 4883 bc24 b800 0000 080f  ......H..$......
-00000df0: 85e2 0200 0048 899c 2488 0000 004c 8bbc  .....H..$....L..
-00000e00: 24a0 0000 0048 8b84 24c0 0000 0048 8944  $....H..$....H.D
-00000e10: 2478 488b 8424 c800 0000 4889 8424 c001  $xH..$....H..$..
-00000e20: 0000 4c8b ac24 d000 0000 4c8b b424 d800  ..L..$....L..$..
-00000e30: 0000 488b 9c24 e000 0000 488b bc24 9000  ..H..$....H..$..
-00000e40: 0000 c5f8 57c0 c5fc 2984 2400 0100 00c5  ....W...).$.....
-00000e50: fc29 8424 2001 0000 48c7 8424 4001 0000  .).$ ...H..$@...
-00000e60: 0000 0000 488d b424 0001 0000 c5f8 7741  ....H..$......wA
-00000e70: ffd4 85c0 0f85 9402 0000 4883 bc24 1801  ..........H..$..
-00000e80: 0000 080f 8585 0200 004c 8ba4 2400 0100  .........L..$...
-00000e90: 00c5 fc28 8424 2001 0000 488b 8424 4001  ...(.$ ...H..$@.
-00000ea0: 0000 c5f0 57c9 c5fc 298c 2460 0100 00c5  ....W...).$`....
-00000eb0: fc29 8c24 8001 0000 48c7 8424 a001 0000  .).$....H..$....
-00000ec0: 0000 0000 4889 4424 68c5 fc11 4424 484c  ....H.D$h...D$HL
-00000ed0: 8964 2428 4889 5c24 204c 8974 2418 4c89  .d$(H.\$ L.t$.L.
-00000ee0: 6c24 1048 8b84 24c0 0100 0048 8944 2408  l$.H..$....H.D$.
-00000ef0: 488b 4424 7848 8904 2448 b800 0000 0000  H.D$xH..$H......
-00000f00: 0000 0048 8dbc 2460 0100 0048 8db4 2480  ...H..$`...H..$.
-00000f10: 0000 004c 89fa c5f8 77ff d089 c34c 8bac  ...L....w....L..
-00000f20: 2480 0000 0048 8b84 2460 0100 0048 8944  $....H..$`...H.D
-00000f30: 2478 c5fc 1084 2468 0100 00c5 fc29 8424  $x....$h.....).$
-00000f40: c001 0000 c5fc 1084 2488 0100 00c5 fc29  ........$......)
-00000f50: 8424 4002 0000 49be 0000 0000 0000 0000  .$@...I.........
-00000f60: 4c89 ffc5 f877 41ff d64c 89e7 41ff d683  L....wA..L..A...
-00000f70: fbfe 742b 85db 7548 488b 8424 8800 0000  ..t+..uHH..$....
-00000f80: 488b 7818 4885 ff74 7e48 b800 0000 0000  H.x.H..t~H......
-00000f90: 0000 0031 f6ff d048 89c1 e98a 0000 0048  ...1...H.......H
-00000fa0: bb00 0000 0000 0000 0048 b800 0000 0000  .........H......
-00000fb0: 0000 0048 89df ffd0 4889 d8e9 3c01 0000  ...H....H...<...
-00000fc0: 0f8e c300 0000 48b8 0000 0000 0000 0000  ......H.........
-00000fd0: ffd0 498b 5510 418b 7508 498b 7d00 48b8  ..I.U.A.u.I.}.H.
-00000fe0: 0000 0000 0000 0000 ffd0 4885 c00f 8407  ..........H.....
-00000ff0: 0100 0048 b900 0000 0000 0000 0048 89c7  ...H.........H..
-00001000: ffd1 e9f3 0000 0048 bf00 0000 0000 0000  .......H........
-00001010: 0048 be00 0000 0000 0000 0048 b800 0000  .H.........H....
-00001020: 0000 0000 00ff d031 c948 8b5c 2478 4889  .......1.H.\$xH.
-00001030: 9c24 e001 0000 c5fc 2884 24c0 0100 00c5  .$......(.$.....
-00001040: fc11 8424 e801 0000 c5fc 2884 2440 0200  ...$......(.$@..
-00001050: 00c5 fc11 8424 0802 0000 48b8 0000 0000  .....$....H.....
-00001060: 0000 0000 488d bc24 e001 0000 be02 0000  ....H..$........
-00001070: 00ba 0100 0000 c5f8 77ff d049 89c7 4889  ........w..I..H.
-00001080: df41 ffd6 4c89 f8eb 7383 fbfd 741b 83fb  .A..L...s...t...
-00001090: ff74 6748 bf00 0000 0000 0000 0048 be00  .tgH.........H..
-000010a0: 0000 0000 0000 00eb 4248 bf00 0000 0000  ........BH......
-000010b0: 0000 0048 b800 0000 0000 0000 00ff d0eb  ...H............
-000010c0: 3948 bf00 0000 0000 0000 0048 be00 0000  9H.........H....
-000010d0: 0000 0000 00eb 1448 bf00 0000 0000 0000  .......H........
-000010e0: 0048 be00 0000 0000 0000 0048 b800 0000  .H.........H....
-000010f0: 0000 0000 00c5 f877 ffd0 31c0 488d 65d8  .......w..1.H.e.
-00001100: 5b41 5c41 5d41 5e41 5f5d c5f8 77c3 48bf  [A\A]A^A_]..w.H.
-00001110: 0000 0000 0000 0000 48be 0000 0000 0000  ........H.......
-00001120: 0000 48b8 0000 0000 0000 0000 ffd0 48b8  ..H...........H.
-00001130: 0000 0000 0000 0000 4c89 ffff d0eb bb66  ........L......f
-00001140: 2e0f 1f84 0000 0000 0055 4889 e541 5741  .........UH..AWA
-00001150: 5641 5541 5453 4883 e4e0 4881 ec20 0100  VAUATSH...H.. ..
-00001160: 00c5 fc10 4510 4889 f248 89fb 488b 4530  ....E.H..H..H.E0
-00001170: c5fc 104d 5048 8b4d 70c5 e857 d2c5 fc29  ...MPH.Mp..W...)
-00001180: 9424 e000 0000 c5fc 2994 24c0 0000 0048  .$......).$....H
-00001190: c784 2400 0100 0000 0000 0048 c784 2480  ..$........H..$.
-000011a0: 0000 0000 0000 0048 894c 2468 c5fc 114c  .......H.L$h...L
-000011b0: 2448 4889 4424 28c5 fc11 4424 084c 890c  $HH.D$(...D$.L..
-000011c0: 2448 b800 0000 0000 0000 0048 8dbc 24c0  $H.........H..$.
-000011d0: 0000 0048 8db4 2480 0000 00c5 f877 ffd0  ...H..$......w..
-000011e0: 4189 c64c 8bbc 2480 0000 004c 8b84 24c0  A..L..$....L..$.
-000011f0: 0000 004c 8ba4 24c8 0000 004c 8bac 24d0  ...L..$....L..$.
-00001200: 0000 0048 8b8c 24d8 0000 0048 8b94 24e0  ...H..$....H..$.
-00001210: 0000 0048 8bb4 24e8 0000 0048 8bbc 24f0  ...H..$....H..$.
-00001220: 0000 0048 8b84 24f8 0000 004c 8b8c 2400  ...H..$....L..$.
-00001230: 0100 00c7 4424 7c00 0000 0041 83fe fe0f  ....D$|....A....
-00001240: 8412 0100 0045 85f6 0f84 0901 0000 4c89  .....E........L.
-00001250: 8c24 8800 0000 4889 8424 9000 0000 4889  .$....H..$....H.
-00001260: bc24 9800 0000 4889 b424 a000 0000 4889  .$....H..$....H.
-00001270: 9424 a800 0000 4889 8c24 b000 0000 4c89  .$....H..$....L.
-00001280: 8424 b800 0000 48b8 0000 0000 0000 0000  .$....H.........
-00001290: 488d 7c24 7cff d045 85f6 0f8e ec00 0000  H.|$|..E........
-000012a0: 48b8 0000 0000 0000 0000 ffd0 498b 5710  H...........I.W.
-000012b0: 418b 7708 498b 3f48 b800 0000 0000 0000  A.w.I.?H........
-000012c0: 00ff d048 85c0 740f 48b9 0000 0000 0000  ...H..t.H.......
-000012d0: 0000 4889 c7ff d148 bf00 0000 0000 0000  ..H....H........
-000012e0: 0048 b800 0000 0000 0000 00ff d049 89c6  .H...........I..
-000012f0: 48b8 0000 0000 0000 0000 4c89 f7ff d048  H.........L....H
-00001300: b800 0000 0000 0000 004c 89f7 ffd0 48b8  .........L....H.
-00001310: 0000 0000 0000 0000 488d 7c24 7cff d04c  ........H.|$|..L
-00001320: 8b84 24b8 0000 0048 8b8c 24b0 0000 0048  ..$....H..$....H
-00001330: 8b94 24a8 0000 0048 8bb4 24a0 0000 0048  ..$....H..$....H
-00001340: 8bbc 2498 0000 0048 8b84 2490 0000 004c  ..$....H..$....L
-00001350: 8b8c 2488 0000 004c 8903 4c89 6308 4c89  ..$....L..L.c.L.
-00001360: 6b10 4889 4b18 4889 5320 4889 7328 4889  k.H.K.H.S H.s(H.
-00001370: 7b30 4889 4338 4c89 4b40 4889 d848 8d65  {0H.C8L.K@H..H.e
-00001380: d85b 415c 415d 415e 415f 5dc3 4183 fefd  .[A\A]A^A_].A...
-00001390: 742f 4183 feff 0f84 3bff ffff 48bf 0000  t/A.....;...H...
-000013a0: 0000 0000 0000 48be 0000 0000 0000 0000  ......H.........
-000013b0: 48b8 0000 0000 0000 0000 ffd0 e916 ffff  H...............
-000013c0: ff48 bf00 0000 0000 0000 0048 b800 0000  .H.........H....
-000013d0: 0000 0000 00ff d0e9 fbfe ffff 662e 0f1f  ............f...
-000013e0: 8400 0000 0000 0f1f 0041 5741 5641 5541  .........AWAVAUA
-000013f0: 5453 4c89 cb4d 89c4 4989 f649 89ff 48b8  TSL..M..I..I..H.
-00001400: 0000 0000 0000 0000 bf08 0000 00be 2000  .............. .
-00001410: 0000 ffd0 4885 db0f 8412 0100 0049 89c5  ....H........I..
-00001420: 488b 7424 3848 8b54 2430 c4e1 fb2a c348  H.t$8H.T$0...*.H
-00001430: 8b58 18c4 e1f3 2a4c 2440 c5f3 5ec0 c4e1  .X....*L$@..^...
-00001440: fb2c c848 b800 0000 0000 0000 00bf 6400  .,.H..........d.
-00001450: 0000 4989 d8ff d085 c00f 8899 0000 0048  ..I............H
-00001460: be00 0000 0000 0000 0048 b800 0000 0000  .........H......
-00001470: 0000 00bf 2800 0000 ffd0 4885 c00f 84b8  ....(.....H.....
-00001480: 0000 0048 8b48 1848 c741 0802 0000 0048  ...H.H.H.A.....H
-00001490: 8b48 1848 c701 0000 0000 488b 4818 c641  .H.H......H.H..A
-000014a0: 1000 488b 4818 c5f9 57c0 c5f9 1141 1848  ..H.H...W....A.H
-000014b0: 8b48 1848 c701 0200 0000 488b 4818 48c7  .H.H......H.H.H.
-000014c0: 4118 0100 0000 488b 4818 4c89 6120 488b  A.....H.H.L.a H.
-000014d0: 4818 4883 3900 7e6f 49be 0000 0000 0000  H.H.9.~oI.......
-000014e0: 0000 4889 c741 ffd6 488b 1b4c 89ef 41ff  ..H..A..H..L..A.
-000014f0: d649 891f 31c0 eb2d 48b8 0000 0000 0000  .I..1..-H.......
-00001500: 0000 4c89 efff d048 b800 0000 0000 0000  ..L....H........
-00001510: 00ff d048 b800 0000 0000 0000 0049 8906  ...H.........I..
-00001520: b801 0000 005b 415c 415d 415e 415f c348  .....[A\A]A^A_.H
-00001530: b800 0000 0000 0000 00eb e248 b800 0000  ...........H....
-00001540: 0000 0000 00eb d648 b800 0000 0000 0000  .......H........
-00001550: 00eb ca66 0f1f 4400 0048 85ff 7406 f048  ...f..D..H..t..H
-00001560: ff0f 7401 c348 b800 0000 0000 0000 00ff  ..t..H..........
-00001570: e00f 1f84 0000 0000 00c3 662e 0f1f 8400  ..........f.....
-00001580: 0000 0000 0f1f 4400 0048 85ff 7405 f048  ......D..H..t..H
-00001590: ff07 c3c3 0000 0000 0000 0000 0000 0000  ................
-000015a0: 00b6 0000 0000 0000 0000 0000 0000 0000  ................
-000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015c0: 0083 0000 0000 0000 0000 0000 0000 0000  ................
-000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015e0: 0047 0000 0000 0000 0000 0000 0000 0000  .G..............
-000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001600: 0083 0000 0000 0000 0000 0000 0000 0000  ................
-00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001620: 008b 0000 0000 0000 0000 0000 0000 0000  ................
-00001630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001640: 003f 0000 0000 0000 0000 0000 0000 0000  .?..............
-00001650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001660: 003d 0000 0000 0000 0000 0000 0000 0000  .=..............
-00001670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001680: 003c 0000 0000 0000 0000 0000 0000 0000  .<..............
-00001690: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-000016a0: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
-000016b0: 7100 585b 0000 0061 7272 6179 2069 7320  q.X[...array is 
-000016c0: 746f 6f20 6269 673b 2060 6172 722e 7369  too big; `arr.si
-000016d0: 7a65 202a 2061 7272 2e64 7479 7065 2e69  ze * arr.dtype.i
-000016e0: 7465 6d73 697a 6560 2069 7320 6c61 7267  temsize` is larg
-000016f0: 6572 2074 6861 6e20 7468 6520 6d61 7869  er than the maxi
-00001700: 6d75 6d20 706f 7373 6962 6c65 2073 697a  mum possible siz
-00001710: 652e 7101 8571 024e 8771 032e 0000 0000  e.q..q.N.q......
-00001720: 0000 0000 0000 0000 0036 3738 f0a8 d2e2  .........678....
-00001730: 6071 fb50 e9d2 1b4b 80a9 532f 0600 0000  `q.P...K..S/....
-00001740: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001750: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
-00001760: 7100 588e 0000 0075 6e61 626c 6520 746f  q.X....unable to
-00001770: 2062 726f 6164 6361 7374 2061 7267 756d   broadcast argum
-00001780: 656e 7420 3120 746f 206f 7574 7075 7420  ent 1 to output 
-00001790: 6172 7261 790a 4669 6c65 2022 2f55 7365  array.File "/Use
-000017a0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-000017b0: 2f65 6e76 732f 7369 6d62 615f 6465 762f  /envs/simba_dev/
-000017c0: 7369 6d62 612f 6d69 7869 6e73 2f66 6561  simba/mixins/fea
-000017d0: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
-000017e0: 6d69 7869 6e2e 7079 222c 206c 696e 6520  mixin.py", line 
-000017f0: 3138 392c 2071 0185 7102 4e87 7103 2e00  189, q..q.N.q...
-00001800: 0000 0000 0000 0000 0006 f009 ba62 c366  .............b.f
-00001810: 22c2 2f52 cb5f 4bc0 5c8d d65d 5900 0000  "./R._K.\..]Y...
-00001820: 0000 0000 0000 0000 0046 6561 7475 7265  .........Feature
-00001830: 4578 7472 6163 7469 6f6e 4d69 7869 6e2e  ExtractionMixin.
-00001840: 6364 6973 7400 0000 006d 6973 7369 6e67  cdist....missing
-00001850: 2045 6e76 6972 6f6e 6d65 6e74 3a20 5f5a   Environment: _Z
-00001860: 4e30 384e 756d 6261 456e 7635 7369 6d62  N08NumbaEnv5simb
-00001870: 6136 6d69 7869 6e73 3234 6665 6174 7572  a6mixins24featur
-00001880: 655f 6578 7472 6163 7469 6f6e 5f6d 6978  e_extraction_mix
-00001890: 696e 3232 4665 6174 7572 6545 7874 7261  in22FeatureExtra
-000018a0: 6374 696f 6e4d 6978 696e 3130 6364 6973  ctionMixin10cdis
-000018b0: 7424 3234 3535 4535 4172 7261 7949 644c  t$2455E5ArrayIdL
-000018c0: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
-000018d0: 6967 6e65 6445 3541 7272 6179 4964 4c69  ignedE5ArrayIdLi
-000018e0: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
-000018f0: 676e 6564 4500 0000 0063 616e 2774 2075  gnedE....can't u
-00001900: 6e62 6f78 2061 7272 6179 2066 726f 6d20  nbox array from 
-00001910: 5079 4f62 6a65 6374 2069 6e74 6f20 6e61  PyObject into na
-00001920: 7469 7665 2076 616c 7565 2e20 2054 6865  tive value.  The
-00001930: 206f 626a 6563 7420 6d61 7962 6520 6f66   object maybe of
-00001940: 2061 2064 6966 6665 7265 6e74 2074 7970   a different typ
-00001950: 6500 0000 0000 0000 0060 656e 762e 636f  e........`env.co
-00001960: 6e73 7473 6020 6973 204e 554c 4c20 696e  nsts` is NULL in
-00001970: 2060 7265 6164 5f63 6f6e 7374 6000 0000   `read_const`...
-00001980: 0000 0000 0000 0000 0075 6e6b 6e6f 776e  .........unknown
-00001990: 2065 7272 6f72 2077 6865 6e20 6361 6c6c   error when call
-000019a0: 696e 6720 6e61 7469 7665 2066 756e 6374  ing native funct
-000019b0: 696f 6e00 0000 0000 003c 6e75 6d62 612e  ion......<numba.
-000019c0: 636f 7265 2e63 7075 2e43 5055 436f 6e74  core.cpu.CPUCont
-000019d0: 6578 7420 6f62 6a65 6374 2061 7420 3078  ext object at 0x
-000019e0: 3766 6362 6635 3561 6432 3038 3e00 0000  7fcbf55ad208>...
-000019f0: 0000 0000 0000 0000 0075 6e6b 6e6f 776e  .........unknown
-00001a00: 2065 7272 6f72 2077 6865 6e20 6361 6c6c   error when call
-00001a10: 696e 6720 6e61 7469 7665 2066 756e 6374  ing native funct
-00001a20: 696f 6e00 0000 0000 0080 0363 6275 696c  ion........cbuil
-00001a30: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
-00001a40: 7100 585b 0000 0061 7272 6179 2069 7320  q.X[...array is 
-00001a50: 746f 6f20 6269 673b 2060 6172 722e 7369  too big; `arr.si
-00001a60: 7a65 202a 2061 7272 2e64 7479 7065 2e69  ze * arr.dtype.i
-00001a70: 7465 6d73 697a 6560 2069 7320 6c61 7267  temsize` is larg
-00001a80: 6572 2074 6861 6e20 7468 6520 6d61 7869  er than the maxi
-00001a90: 6d75 6d20 706f 7373 6962 6c65 2073 697a  mum possible siz
-00001aa0: 652e 7101 8571 024e 8771 032e 0000 0000  e.q..q.N.q......
-00001ab0: 0000 0000 0000 0000 0036 3738 f0a8 d2e2  .........678....
-00001ac0: 6071 fb50 e9d2 1b4b 80a9 532f 0600 0000  `q.P...K..S/....
-00001ad0: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001ae0: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
-00001af0: 7100 581f 0000 006e 6567 6174 6976 6520  q.X....negative 
-00001b00: 6469 6d65 6e73 696f 6e73 206e 6f74 2061  dimensions not a
-00001b10: 6c6c 6f77 6564 7101 8571 024e 8771 032e  llowedq..q.N.q..
-00001b20: 0000 0000 0000 0000 00ae da98 e06c 49b7  .............lI.
-00001b30: ad8d 31d8 f7bf e26d 725c eeb4 fd00 0000  ..1....mr\......
-00001b40: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001b50: 7469 6e73 0a49 6e64 6578 4572 726f 720a  tins.IndexError.
-00001b60: 7100 5814 0000 0067 6574 6974 656d 206f  q.X....getitem o
-00001b70: 7574 206f 6620 7261 6e67 6571 0185 7102  ut of rangeq..q.
-00001b80: 4e87 7103 2e00 0000 0020 07e5 5362 341d  N.q...... ..Sb4.
-00001b90: 8cb1 31a7 6c9a ffe8 647a bda8 6d00 0000  ..1.l...dz..m...
-00001ba0: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001bb0: 7469 6e73 0a4d 656d 6f72 7945 7272 6f72  tins.MemoryError
-00001bc0: 0a71 0058 1400 0000 6361 6e6e 6f74 2061  .q.X....cannot a
-00001bd0: 6c6c 6f63 6174 6520 6c69 7374 7101 8571  llocate listq..q
-00001be0: 024e 8771 032e 0000 00ee a280 57b5 a3e7  .N.q........W...
-00001bf0: aa1c aed9 439a e21e e2dc 0c7a 9b00 0000  ....C......z....
-00001c00: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001c10: 7469 6e73 0a5a 6572 6f44 6976 6973 696f  tins.ZeroDivisio
-00001c20: 6e45 7272 6f72 0a71 0058 1000 0000 6469  nError.q.X....di
-00001c30: 7669 7369 6f6e 2062 7920 7a65 726f 7101  vision by zeroq.
-00001c40: 8571 024e 8771 032e 007e 37a9 709c 0a80  .q.N.q...~7.p...
-00001c50: 79dd 9427 5983 7d90 f293 2bae 3600 0000  y..'Y.}...+.6...
-00001c60: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
-00001c70: 7469 6e73 0a41 7373 6572 7469 6f6e 4572  tins.AssertionEr
-00001c80: 726f 720a 7100 2958 0400 0000 696d 706c  ror.q.)X....impl
-00001c90: 7101 5851 0000 002f 5573 6572 732f 7369  q.XQ.../Users/si
-00001ca0: 6d6f 6e2f 2e63 6f6e 6461 2f65 6e76 732f  mon/.conda/envs/
-00001cb0: 7369 6d62 615f 6465 762f 6c69 622f 7079  simba_dev/lib/py
-00001cc0: 7468 6f6e 332e 362f 7369 7465 2d70 6163  thon3.6/site-pac
-00001cd0: 6b61 6765 732f 6e75 6d62 612f 6e70 2f6c  kages/numba/np/l
-00001ce0: 696e 616c 672e 7079 7102 4d5e 0887 7103  inalg.pyq.M^..q.
-00001cf0: 8771 042e 0000 0000 0049 1f9a 1741 ace0  .q.......I...A..
-00001d00: 7701 f821 d0e5 1919 89e8 abf9 9d00 0000  w..!............
-00001d10: 0000 0000 0000 0000 00f6 0900 0000 182a  ...............*
-00001d20: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0000 0a00 0000 0000 0096 0400 00d1 5805  ..............X.
-00001d40: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-00001d50: 00a0 0e00 0000 0000 0093 0200 00d1 5805  ..............X.
-00001d60: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-00001d70: 0040 1100 0000 0000 006a 0100 0000 1406  .@.......j......
-00001d80: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0014 0000 0000 0000 0001 7a52 0001 7810  ..........zR..x.
-00001da0: 0110 0c07 0890 0100 003c 0000 001c 0000  .........<......
-00001db0: 00f8 e4ff ffff ffff fff6 0900 0000 0000  ................
-00001dc0: 0000 410e 1042 0e18 420e 2042 0e28 420e  ..A..B..B. B.(B.
-00001dd0: 3041 0e38 470e d002 8307 8c06 8d05 8e04  0A.8G...........
-00001de0: 8f03 8602 0000 0000 002c 0000 005c 0000  .........,...\..
-00001df0: 00b8 eeff ffff ffff ff96 0400 0000 0000  ................
-00001e00: 0000 410e 1086 0243 0d06 5483 078c 068d  ..A....C..T.....
-00001e10: 058e 048f 0300 0000 002c 0000 008c 0000  .........,......
-00001e20: 0028 f3ff ffff ffff ff93 0200 0000 0000  .(..............
-00001e30: 0000 410e 1086 0243 0d06 5483 078c 068d  ..A....C..T.....
-00001e40: 058e 048f 0300 0000 0034 0000 00bc 0000  .........4......
-00001e50: 0098 f5ff ffff ffff ff6a 0100 0000 0000  .........j......
-00001e60: 0000 420e 1042 0e18 420e 2042 0e28 410e  ..B..B..B. B.(A.
-00001e70: 3083 068c 058d 048e 038f 0200 0000 0000  0...............
-00001e80: 001c 0000 00f4 0000 00d0 f6ff ffff ffff  ................
-00001e90: ff18 0000 0000 0000 0000 0000 0000 0000  ................
-00001ea0: 001c 0000 0014 0100 00d0 f6ff ffff ffff  ................
-00001eb0: ff01 0000 0000 0000 0000 0000 0000 0000  ................
-00001ec0: 00be 1200 0027 0000 0ea0 1200 000e 0000  .....'..........
-00001ed0: 0e94 1200 000d 0000 0e88 1200 000c 0000  ................
-00001ee0: 0e6c 1200 000b 0000 0e60 1200 0041 0000  .l.......`...A..
-00001ef0: 0e51 1200 0020 0000 0e31 1200 0020 0000  .Q... ...1... ..
-00001f00: 0ec2 1100 0028 0000 0eb8 1100 001f 0000  .....(..........
-00001f10: 0e9c 1100 0045 0000 0e57 1100 0026 0000  .....E...W...&..
-00001f20: 0e24 1100 002d 0000 0e1a 1100 0031 0000  .$...-.......1..
-00001f30: 0e09 1100 002e 0000 0eff 1000 000a 0000  ................
-00001f40: 0ef5 1000 0032 0000 0e67 1000 0043 0000  .....2...g...C..
-00001f50: 0e58 1000 0036 0000 0e49 1000 002f 0000  .X...6...I.../..
-00001f60: 0e3a 1000 0035 0000 0e30 1000 0009 0000  .:...5...0......
-00001f70: 0e21 1000 0040 0000 0e10 1000 0044 0000  .!...@.......D..
-00001f80: 0ef9 0f00 002c 0000 0edf 0f00 0042 0000  .....,.......B..
-00001f90: 0e1a 0f00 0023 0000 0e87 0e00 0020 0000  .....#....... ..
-00001fa0: 0e7b 0e00 002e 0000 0e71 0e00 0008 0000  .{.......q......
-00001fb0: 0e67 0e00 0033 0000 0e44 0e00 002e 0000  .g...3...D......
-00001fc0: 0e3a 0e00 0008 0000 0e30 0e00 0033 0000  .:.......0...3..
-00001fd0: 0e24 0e00 0007 0000 0e1a 0e00 0030 0000  .$...........0..
-00001fe0: 0e0c 0e00 002d 0000 0e02 0e00 0031 0000  .....-.......1..
-00001ff0: 0ef6 0d00 0006 0000 0eec 0d00 0032 0000  .............2..
-00002000: 0eb3 0d00 002a 0000 0e74 0d00 002e 0000  .....*...t......
-00002010: 0e6a 0d00 0005 0000 0e60 0d00 0030 0000  .j.......`...0..
-00002020: 0e4c 0d00 0040 0000 0e37 0d00 0044 0000  .L...@...7...D..
-00002030: 0e1f 0d00 002c 0000 0e02 0d00 0037 0000  .....,.......7..
-00002040: 0ef8 0c00 0038 0000 0ee2 0c00 0034 0000  .....8.......4..
-00002050: 0eaf 0c00 0020 0000 0e52 0c00 0023 0000  ..... ...R...#..
-00002060: 0e1f 0b00 0029 0000 0edf 0a00 003f 0000  .....).......?..
-00002070: 0e27 0a00 002b 0000 0e1d 0a00 0004 0000  .'...+..........
-00002080: 0ee8 0900 0003 0000 0ebf 0900 0002 0000  ................
-00002090: 0ea3 0900 0001 0000 0e8c 0900 0020 0000  ............. ..
-000020a0: 0ef8 0700 0022 0000 0e97 0700 0020 0000  ....."....... ..
-000020b0: 0ea3 0300 0026 0000 0e50 0300 0021 0000  .....&...P...!..
-000020c0: 0e0b 0300 0020 0000 0e9d 0000 0026 0000  ..... .......&..
-000020d0: 0e70 0000 0000 0000 0e31 0000 0021 0000  .p.......1...!..
-000020e0: 0ef0 0000 001e 0000 0ee0 0000 001d 0000  ................
-000020f0: 0ed0 0000 001c 0000 0ec0 0000 001b 0000  ................
-00002100: 0eb0 0000 001a 0000 0ea0 0000 0019 0000  ................
-00002110: 0e90 0000 0018 0000 0e80 0000 0017 0000  ................
-00002120: 0e70 0000 0016 0000 0e60 0000 0015 0000  .p.......`......
-00002130: 0e50 0000 0014 0000 0e40 0000 0013 0000  .P.......@......
-00002140: 0e30 0000 0012 0000 0e20 0000 0011 0000  .0....... ......
-00002150: 0e10 0000 0010 0000 0e00 0000 000f 0000  ................
-00002160: 0e60 0000 0001 0000 0640 0000 0001 0000  .`.......@......
-00002170: 0620 0000 0001 0000 0600 0000 0001 0000  . ..............
-00002180: 0691 0900 000e 0200 0050 1300 0000 0000  .........P......
-00002190: 0007 0900 000e 0200 00f0 1200 0000 0000  ................
-000021a0: 00c5 0a00 000e 0200 0010 1300 0000 0000  ................
-000021b0: 00d6 0900 000e 0200 0030 1300 0000 0000  .........0......
-000021c0: 0001 0000 000e 0300 0080 1500 0000 0000  ................
-000021d0: 00fb 0300 000e 0300 00b0 1600 0000 0000  ................
-000021e0: 00c3 0000 000e 0300 00e0 1600 0000 0000  ................
-000021f0: 008b 0500 000e 0300 00a0 1500 0000 0000  ................
-00002200: 00e8 0100 000e 0300 0050 1600 0000 0000  .........P......
-00002210: 00fb 0700 000e 0300 0010 1700 0000 0000  ................
-00002220: 004a 0c00 000e 0300 0050 1700 0000 0000  .J.......P......
-00002230: 001b 0a00 000e 0200 0070 1300 0000 0000  .........p......
-00002240: 0072 0a00 000e 0200 0090 1300 0000 0000  .r..............
-00002250: 00c2 0800 000e 0200 00b0 1300 0000 0000  ................
-00002260: 004c 0900 000e 0200 00d0 1300 0000 0000  .L..............
-00002270: 0029 0900 000e 0300 00a0 1400 0000 0000  .)..............
-00002280: 0032 0b00 000e 0300 0060 1500 0000 0000  .2.......`......
-00002290: 00e7 0a00 000e 0300 00f0 1300 0000 0000  ................
-000022a0: 0022 0c00 000e 0300 0080 1400 0000 0000  ."..............
-000022b0: 00f8 0900 000e 0300 0030 1800 0000 0000  .........0......
-000022c0: 00aa 0b00 000e 0300 0080 1800 0000 0000  ................
-000022d0: 00b3 0900 000e 0300 0080 1700 0000 0000  ................
-000022e0: 0082 0b00 000e 0300 0010 1800 0000 0000  ................
-000022f0: 003d 0a00 000e 0300 00c0 1900 0000 0000  .=..............
-00002300: 00d2 0b00 000e 0300 0050 1a00 0000 0000  .........P......
-00002310: 0094 0a00 000e 0300 0060 1900 0000 0000  .........`......
-00002320: 00fa 0b00 000e 0300 00a0 1900 0000 0000  ................
-00002330: 00e4 0800 000e 0300 0000 1900 0000 0000  ................
-00002340: 000a 0b00 000e 0300 0040 1900 0000 0000  .........@......
-00002350: 006e 0900 000e 0300 00a0 1800 0000 0000  .n..............
-00002360: 005a 0b00 000e 0300 00e0 1800 0000 0000  .Z..............
-00002370: 0060 0a00 000f 0180 00d0 1200 0000 0000  .`..............
-00002380: 0091 0100 000f 01c0 00b0 1200 0000 0000  ................
-00002390: 0085 0100 000f 01c0 00e0 1200 0000 0000  ................
-000023a0: 0092 0400 000f 01c0 0040 1100 0000 0000  .........@......
-000023b0: 00d7 0600 000f 0100 0000 0000 0000 0000  ................
-000023c0: 0040 0600 000f 0100 0000 0a00 0000 0000  .@..............
-000023d0: 0066 0700 000f 0100 00a0 0e00 0000 0000  .f..............
-000023e0: 00ed 0200 0001 0000 0000 0000 0000 0000  ................
-000023f0: 0036 0000 0001 0000 0000 0000 0000 0000  .6..............
-00002400: 004d 0000 0001 0000 0000 0000 0000 0000  .M..............
-00002410: 000b 0100 0001 0000 0000 0000 0000 0000  ................
-00002420: 0061 0100 0001 0000 0000 0000 0000 0000  .a..............
-00002430: 0058 0200 0001 0000 0000 0000 0000 0000  .X..............
-00002440: 00b6 0000 0001 0000 0000 0000 0000 0000  ................
-00002450: 0049 0200 0001 0000 0000 0000 0000 0000  .I..............
-00002460: 003a 0100 0001 0000 0000 0000 0000 0000  .:..............
-00002470: 007b 0200 0001 0000 0000 0000 0000 0000  .{..............
-00002480: 00a2 0000 0001 0000 0000 0000 0000 0000  ................
-00002490: 00f6 0000 0001 0000 0000 0000 0000 0000  ................
-000024a0: 007e 0000 0001 0000 0000 0000 0000 0000  .~..............
-000024b0: 0091 0000 0001 0000 0000 0000 0000 0000  ................
-000024c0: 002a 0100 0001 0000 0000 0000 0000 0000  .*..............
-000024d0: 004b 0100 0001 0000 0000 0000 0000 0000  .K..............
-000024e0: 00a8 0100 0001 0000 0000 0000 0000 0000  ................
-000024f0: 009d 0100 0001 0000 0000 0000 0000 0000  ................
-00002500: 0026 0000 0001 0000 0000 0000 0000 0000  .&..............
-00002510: 000d 0300 0001 0000 0308 0000 0000 0000  ................
-00002520: 0038 0800 0001 0000 0308 0000 0000 0000  .8..............
-00002530: 0028 0400 0001 0000 0308 0000 0000 0000  .(..............
-00002540: 0092 0200 0001 0000 0308 0000 0000 0000  ................
-00002550: 00b0 0300 0001 0000 0308 0000 0000 0000  ................
-00002560: 0056 0300 0001 0000 0308 0000 0000 0000  .V..............
-00002570: 00f2 0400 0001 0000 0308 0000 0000 0000  ................
-00002580: 00b3 0100 0001 0000 0000 0000 0000 0000  ................
-00002590: 006b 0000 0001 0000 0000 0000 0000 0000  .k..............
-000025a0: 00d6 0100 0001 0000 0000 0000 0000 0000  ................
-000025b0: 00c3 0100 0001 0000 0000 0000 0000 0000  ................
-000025c0: 006b 0200 0001 0000 0000 0000 0000 0000  .k..............
-000025d0: 00b7 0a00 0001 0000 0000 0000 0000 0000  ................
-000025e0: 0000 5f2e 636f 6e73 742e 4665 6174 7572  .._.const.Featur
-000025f0: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
-00002600: 2e63 6469 7374 005f 5f50 795f 4e6f 6e65  .cdist.__Py_None
-00002610: 5374 7275 6374 005f 4e52 545f 4d65 6d49  Struct._NRT_MemI
-00002620: 6e66 6f5f 6361 6c6c 5f64 746f 7200 5f4e  nfo_call_dtor._N
-00002630: 5254 5f4d 656d 496e 666f 5f6e 6577 5f76  RT_MemInfo_new_v
-00002640: 6172 7369 7a65 5f64 746f 7200 5f6e 756d  arsize_dtor._num
-00002650: 6261 5f66 6174 616c 5f65 7272 6f72 005f  ba_fatal_error._
-00002660: 5079 4578 635f 5379 7374 656d 4572 726f  PyExc_SystemErro
-00002670: 7200 5f50 7945 7863 5f54 7970 6545 7272  r._PyExc_TypeErr
-00002680: 6f72 005f 5079 4578 635f 5275 6e74 696d  or._PyExc_Runtim
-00002690: 6545 7272 6f72 005f 5079 4572 725f 436c  eError._PyErr_Cl
-000026a0: 6561 7200 5f2e 636f 6e73 742e 756e 6b6e  ear._.const.unkn
-000026b0: 6f77 6e20 6572 726f 7220 7768 656e 2063  own error when c
-000026c0: 616c 6c69 6e67 206e 6174 6976 6520 6675  alling native fu
-000026d0: 6e63 7469 6f6e 005f 5079 4578 635f 5374  nction._PyExc_St
-000026e0: 6f70 4974 6572 6174 696f 6e00 5f4e 5254  opIteration._NRT
-000026f0: 5f61 6461 7074 5f6e 6461 7272 6179 5f66  _adapt_ndarray_f
-00002700: 726f 6d5f 7079 7468 6f6e 005f 5079 4c69  rom_python._PyLi
-00002710: 7374 5f47 6574 4974 656d 005f 5079 4572  st_GetItem._PyEr
-00002720: 725f 5365 7453 7472 696e 6700 5f50 7955  r_SetString._PyU
-00002730: 6e69 636f 6465 5f46 726f 6d53 7472 696e  nicode_FromStrin
-00002740: 6700 5f4e 5254 5f61 6461 7074 5f6e 6461  g._NRT_adapt_nda
-00002750: 7272 6179 5f74 6f5f 7079 7468 6f6e 5f61  rray_to_python_a
-00002760: 6371 7265 6600 5f4e 5254 5f69 6e63 7265  cqref._NRT_incre
-00002770: 6600 5f4e 5254 5f64 6563 7265 6600 5f50  f._NRT_decref._P
-00002780: 795f 496e 6352 6566 005f 5079 5f44 6563  y_IncRef._Py_Dec
-00002790: 5265 6600 5f6e 756d 6261 5f64 6f5f 7261  Ref._numba_do_ra
-000027a0: 6973 6500 5f6e 756d 6261 5f67 696c 5f72  ise._numba_gil_r
-000027b0: 656c 6561 7365 005f 6e75 6d62 615f 6769  elease._numba_gi
-000027c0: 6c5f 656e 7375 7265 005f 2e63 6f6e 7374  l_ensure._.const
-000027d0: 2e63 616e 2774 2075 6e62 6f78 2061 7272  .can't unbox arr
-000027e0: 6179 2066 726f 6d20 5079 4f62 6a65 6374  ay from PyObject
-000027f0: 2069 6e74 6f20 6e61 7469 7665 2076 616c   into native val
-00002800: 7565 2e20 2054 6865 206f 626a 6563 7420  ue.  The object 
-00002810: 6d61 7962 6520 6f66 2061 2064 6966 6665  maybe of a diffe
-00002820: 7265 6e74 2074 7970 6500 5f50 7945 7272  rent type._PyErr
-00002830: 5f53 6574 4e6f 6e65 005f 5079 4172 675f  _SetNone._PyArg_
-00002840: 556e 7061 636b 5475 706c 6500 5f6e 756d  UnpackTuple._num
-00002850: 6261 5f75 6e70 6963 6b6c 6500 5f50 7945  ba_unpickle._PyE
-00002860: 7272 5f57 7269 7465 556e 7261 6973 6162  rr_WriteUnraisab
-00002870: 6c65 005f 5f5a 4e30 384e 756d 6261 456e  le.__ZN08NumbaEn
-00002880: 7635 6e75 6d62 6132 6e70 366c 696e 616c  v5numba2np6linal
-00002890: 6732 355f 6475 6d6d 795f 6c69 7665 6e65  g25_dummy_livene
-000028a0: 7373 5f66 756e 6324 3234 3239 4533 306c  ss_func$2429E30l
-000028b0: 6973 7424 3238 696e 7436 3424 3239 2433  ist$28int64$29$3
-000028c0: 6369 7624 3364 4e6f 6e65 2433 6500 5f4e  civ$3dNone$3e._N
-000028d0: 5254 5f4d 656d 496e 666f 5f61 6c6c 6f63  RT_MemInfo_alloc
-000028e0: 5f73 6166 655f 616c 6967 6e65 6400 5f5f  _safe_aligned.__
-000028f0: 5a4e 3038 4e75 6d62 6145 6e76 3133 2433  ZN08NumbaEnv13$3
-00002900: 6364 796e 616d 6963 2433 6533 385f 5f6e  cdynamic$3e38__n
-00002910: 756d 6261 5f61 7272 6179 5f65 7870 725f  umba_array_expr_
-00002920: 3078 3766 6362 6635 3562 3265 3438 2432  0x7fcbf55b2e48$2
-00002930: 3435 3745 6464 005f 5f5a 4e30 384e 756d  457Edd.__ZN08Num
-00002940: 6261 456e 7635 6e75 6d62 6132 6e70 3861  baEnv5numba2np8a
-00002950: 7272 6179 6f62 6a31 336e 756d 7079 5f66  rrayobj13numpy_f
-00002960: 756c 6c5f 6e64 3132 2433 636c 6f63 616c  ull_nd12$3clocal
-00002970: 7324 3365 3966 756c 6c24 3234 3536 4538  s$3e9full$2456E8
-00002980: 556e 6954 7570 6c65 4978 4c69 3245 4564  UniTupleIxLi2EEd
-00002990: 005f 5f5a 4e30 384e 756d 6261 456e 7635  .__ZN08NumbaEnv5
-000029a0: 6e75 6d62 6132 6e70 376e 7079 696d 706c  numba2np7npyimpl
-000029b0: 3230 5f62 726f 6164 6361 7374 5f6f 6e74  20_broadcast_ont
-000029c0: 6f24 3234 3130 4578 3869 6e74 3634 2432  o$2410Ex8int64$2
-000029d0: 6178 3869 6e74 3634 2432 6100 5f2e 636f  ax8int64$2a._.co
-000029e0: 6e73 742e 6065 6e76 2e63 6f6e 7374 7360  nst.`env.consts`
-000029f0: 2069 7320 4e55 4c4c 2069 6e20 6072 6561   is NULL in `rea
-00002a00: 645f 636f 6e73 7460 005f 5f5a 4e30 384e  d_const`.__ZN08N
-00002a10: 756d 6261 456e 7635 6e75 6d62 6132 6e70  umbaEnv5numba2np
-00002a20: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
-00002a30: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
-00002a40: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
-00002a50: 3238 4535 4172 7261 7949 644c 6931 4531  28E5ArrayIdLi1E1
-00002a60: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
-00002a70: 6445 005f 5f5a 4e35 6e75 6d62 6132 6e70  dE.__ZN5numba2np
-00002a80: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
-00002a90: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
-00002aa0: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
-00002ab0: 3238 4535 4172 7261 7949 644c 6931 4531  28E5ArrayIdLi1E1
-00002ac0: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
-00002ad0: 6445 005f 5f5a 4e30 384e 756d 6261 456e  dE.__ZN08NumbaEn
-00002ae0: 7635 7369 6d62 6136 6d69 7869 6e73 3234  v5simba6mixins24
-00002af0: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
-00002b00: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
-00002b10: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
-00002b20: 3130 6364 6973 7424 3234 3535 4535 4172  10cdist$2455E5Ar
-00002b30: 7261 7949 644c 6932 4531 4137 6d75 7461  rayIdLi2E1A7muta
-00002b40: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
-00002b50: 6179 4964 4c69 3245 3141 376d 7574 6162  ayIdLi2E1A7mutab
-00002b60: 6c65 3761 6c69 676e 6564 4500 5f2e 636f  le7alignedE._.co
-00002b70: 6e73 742e 6d69 7373 696e 6720 456e 7669  nst.missing Envi
-00002b80: 726f 6e6d 656e 743a 205f 5a4e 3038 4e75  ronment: _ZN08Nu
-00002b90: 6d62 6145 6e76 3573 696d 6261 366d 6978  mbaEnv5simba6mix
-00002ba0: 696e 7332 3466 6561 7475 7265 5f65 7874  ins24feature_ext
-00002bb0: 7261 6374 696f 6e5f 6d69 7869 6e32 3246  raction_mixin22F
-00002bc0: 6561 7475 7265 4578 7472 6163 7469 6f6e  eatureExtraction
-00002bd0: 4d69 7869 6e31 3063 6469 7374 2432 3435  Mixin10cdist$245
-00002be0: 3545 3541 7272 6179 4964 4c69 3245 3141  5E5ArrayIdLi2E1A
-00002bf0: 376d 7574 6162 6c65 3761 6c69 676e 6564  7mutable7aligned
-00002c00: 4535 4172 7261 7949 644c 6932 4531 4137  E5ArrayIdLi2E1A7
-00002c10: 6d75 7461 626c 6537 616c 6967 6e65 6445  mutable7alignedE
-00002c20: 005f 5f5a 4e37 6370 7974 686f 6e35 7369  .__ZN7cpython5si
-00002c30: 6d62 6136 6d69 7869 6e73 3234 6665 6174  mba6mixins24feat
-00002c40: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
-00002c50: 6978 696e 3232 4665 6174 7572 6545 7874  ixin22FeatureExt
-00002c60: 7261 6374 696f 6e4d 6978 696e 3130 6364  ractionMixin10cd
-00002c70: 6973 7424 3234 3535 4535 4172 7261 7949  ist$2455E5ArrayI
-00002c80: 644c 6932 4531 4137 6d75 7461 626c 6537  dLi2E1A7mutable7
-00002c90: 616c 6967 6e65 6445 3541 7272 6179 4964  alignedE5ArrayId
-00002ca0: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
-00002cb0: 6c69 676e 6564 4500 5f5f 5a4e 3573 696d  lignedE.__ZN5sim
-00002cc0: 6261 366d 6978 696e 7332 3466 6561 7475  ba6mixins24featu
-00002cd0: 7265 5f65 7874 7261 6374 696f 6e5f 6d69  re_extraction_mi
-00002ce0: 7869 6e32 3246 6561 7475 7265 4578 7472  xin22FeatureExtr
-00002cf0: 6163 7469 6f6e 4d69 7869 6e31 3063 6469  actionMixin10cdi
-00002d00: 7374 2432 3435 3545 3541 7272 6179 4964  st$2455E5ArrayId
-00002d10: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
-00002d20: 6c69 676e 6564 4535 4172 7261 7949 644c  lignedE5ArrayIdL
-00002d30: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
-00002d40: 6967 6e65 6445 005f 6366 756e 632e 5f5a  ignedE._cfunc._Z
-00002d50: 4e35 7369 6d62 6136 6d69 7869 6e73 3234  N5simba6mixins24
-00002d60: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
-00002d70: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
-00002d80: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
-00002d90: 3130 6364 6973 7424 3234 3535 4535 4172  10cdist$2455E5Ar
-00002da0: 7261 7949 644c 6932 4531 4137 6d75 7461  rayIdLi2E1A7muta
-00002db0: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
-00002dc0: 6179 4964 4c69 3245 3141 376d 7574 6162  ayIdLi2E1A7mutab
-00002dd0: 6c65 3761 6c69 676e 6564 4500 5f2e 636f  le7alignedE._.co
-00002de0: 6e73 742e 3c6e 756d 6261 2e63 6f72 652e  nst.<numba.core.
-00002df0: 6370 752e 4350 5543 6f6e 7465 7874 206f  cpu.CPUContext o
-00002e00: 626a 6563 7420 6174 2030 7837 6663 6266  bject at 0x7fcbf
-00002e10: 3535 6164 3230 383e 005f 5f5a 4e30 384e  55ad208>.__ZN08N
-00002e20: 756d 6261 456e 7635 6e75 6d62 6132 6e70  umbaEnv5numba2np
-00002e30: 366c 696e 616c 6731 345f 6765 745f 6e6f  6linalg14_get_no
-00002e40: 726d 5f69 6d70 6c31 3224 3363 6c6f 6361  rm_impl12$3cloca
-00002e50: 6c73 2433 6531 346f 6e65 445f 696d 706c  ls$3e14oneD_impl
-00002e60: 2432 3432 3745 3541 7272 6179 4964 4c69  $2427E5ArrayIdLi
-00002e70: 3145 3143 376d 7574 6162 6c65 3761 6c69  1E1C7mutable7ali
-00002e80: 676e 6564 4532 376f 6d69 7474 6564 2432  gnedE27omitted$2
-00002e90: 3864 6566 6175 6c74 2433 644e 6f6e 6524  8default$3dNone$
-00002ea0: 3239 005f 2e63 6f6e 7374 2e70 6963 6b6c  29._.const.pickl
-00002eb0: 6562 7566 2e31 3430 3531 3339 3638 3839  ebuf.14051396889
-00002ec0: 3230 3838 005f 2e63 6f6e 7374 2e70 6963  2088._.const.pic
-00002ed0: 6b6c 6564 6174 612e 3134 3035 3133 3936  kledata.14051396
-00002ee0: 3838 3932 3038 3800 5f2e 636f 6e73 742e  8892088._.const.
-00002ef0: 7069 636b 6c65 6275 662e 3134 3035 3133  picklebuf.140513
-00002f00: 3937 3932 3633 3434 3800 5f2e 636f 6e73  979263448._.cons
-00002f10: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
-00002f20: 3531 3339 3739 3236 3334 3438 005f 2e63  513979263448._.c
-00002f30: 6f6e 7374 2e70 6963 6b6c 6562 7566 2e31  onst.picklebuf.1
-00002f40: 3430 3531 3339 3732 3735 3534 3038 005f  40513972755408._
-00002f50: 2e63 6f6e 7374 2e70 6963 6b6c 6564 6174  .const.pickledat
-00002f60: 612e 3134 3035 3133 3937 3237 3535 3430  a.14051397275540
-00002f70: 3800 5f2e 636f 6e73 742e 7069 636b 6c65  8._.const.pickle
-00002f80: 6275 662e 3134 3035 3133 3937 3938 3032  buf.140513979802
-00002f90: 3533 3600 5f2e 636f 6e73 742e 7069 636b  536._.const.pick
-00002fa0: 6c65 6461 7461 2e31 3430 3531 3339 3739  ledata.140513979
-00002fb0: 3830 3235 3336 005f 2e63 6f6e 7374 2e70  802536._.const.p
-00002fc0: 6963 6b6c 6562 7566 2e31 3430 3531 3339  icklebuf.1405139
-00002fd0: 3633 3036 3631 3336 005f 2e63 6f6e 7374  63066136._.const
-00002fe0: 2e70 6963 6b6c 6564 6174 612e 3134 3035  .pickledata.1405
-00002ff0: 3133 3936 3330 3636 3133 3600 5f2e 636f  13963066136._.co
-00003000: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
-00003010: 3035 3133 3937 3338 3130 3031 3600 5f2e  0513973810016._.
-00003020: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
-00003030: 2e31 3430 3531 3339 3733 3831 3030 3136  .140513973810016
-00003040: 005f 2e64 746f 722e 6c69 7374 2e69 6e74  ._.dtor.list.int
-00003050: 3634 005f 2e63 6f6e 7374 2e70 6963 6b6c  64._.const.pickl
-00003060: 6562 7566 2e31 3430 3531 3339 3634 3135  ebuf.14051396415
-00003070: 3031 3434 005f 2e63 6f6e 7374 2e70 6963  0144._.const.pic
-00003080: 6b6c 6564 6174 612e 3134 3035 3133 3936  kledata.14051396
-00003090: 3431 3530 3134 3400 5f6e 756d 6261 5f78  4150144._numba_x
-000030a0: 786e 726d 3200 5f2e 636f 6e73 742e 7069  xnrm2._.const.pi
-000030b0: 636b 6c65 6275 662e 3134 3035 3133 3936  cklebuf.14051396
-000030c0: 3833 3237 3939 3200 5f2e 636f 6e73 742e  8327992._.const.
-000030d0: 7069 636b 6c65 6461 7461 2e31 3430 3531  pickledata.14051
-000030e0: 3339 3638 3332 3739 3932 005f 2e63 6f6e  3968327992._.con
-000030f0: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-00003100: 3035 3133 3936 3838 3932 3038 382e 7368  0513968892088.sh
-00003110: 6131 005f 2e63 6f6e 7374 2e70 6963 6b6c  a1._.const.pickl
-00003120: 6564 6174 612e 3134 3035 3133 3937 3932  edata.1405139792
-00003130: 3633 3434 382e 7368 6131 005f 2e63 6f6e  63448.sha1._.con
-00003140: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-00003150: 3035 3133 3937 3237 3535 3430 382e 7368  0513972755408.sh
-00003160: 6131 005f 2e63 6f6e 7374 2e70 6963 6b6c  a1._.const.pickl
-00003170: 6564 6174 612e 3134 3035 3133 3937 3938  edata.1405139798
-00003180: 3032 3533 362e 7368 6131 005f 2e63 6f6e  02536.sha1._.con
-00003190: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-000031a0: 3035 3133 3936 3330 3636 3133 362e 7368  0513963066136.sh
-000031b0: 6131 005f 2e63 6f6e 7374 2e70 6963 6b6c  a1._.const.pickl
-000031c0: 6564 6174 612e 3134 3035 3133 3937 3338  edata.1405139738
-000031d0: 3130 3031 362e 7368 6131 005f 2e63 6f6e  10016.sha1._.con
-000031e0: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-000031f0: 3035 3133 3936 3431 3530 3134 342e 7368  0513964150144.sh
-00003200: 6131 005f 2e63 6f6e 7374 2e70 6963 6b6c  a1._.const.pickl
-00003210: 6564 6174 612e 3134 3035 3133 3936 3833  edata.1405139683
-00003220: 3237 3939 322e 7368 6131 005f 2e63 6f6e  27992.sha1._.con
-00003230: 7374 2e75 6e6b 6e6f 776e 2065 7272 6f72  st.unknown error
-00003240: 2077 6865 6e20 6361 6c6c 696e 6720 6e61   when calling na
-00003250: 7469 7665 2066 756e 6374 696f 6e2e 3100  tive function.1.
-00003260: 0094 4210 6d00 00de c017 0b00 0000 0014  ..B.m...........
-00003270: 0000 00f8 6c00 0007 0000 0142 43c0 de35  ....l......BC..5
-00003280: 1400 0005 0000 0062 0c30 244a 59be 664d  .......b.0$JY.fM
-00003290: fbb4 5f0b 5180 4c01 0000 0021 0c00 00da  .._.Q.L....!....
-000032a0: 1200 000b 0221 0002 0000 0016 0000 0007  .....!..........
-000032b0: 8123 9141 c804 4906 1032 3992 0184 0c25  .#.A..I..29....%
-000032c0: 0508 191e 048b 6280 1c45 0242 920b 42e4  ......b..E.B..B.
-000032d0: 1032 1438 0818 4b0a 3272 8848 70c4 2123  .2.8..K.2r.Hp.!#
-000032e0: 4412 878c 1041 9202 64c8 08b1 1420 4346  D....A..d.... CF
-000032f0: 8820 c901 3272 8418 2a28 2a90 317c b05c  . ..2r..*(*.1|.\
-00003300: 9120 c7c8 0000 0089 2000 004d 0000 0032  . ...... ..M...2
-00003310: 22c8 0920 6485 0493 23a4 8404 9323 e384  ".. d...#....#..
-00003320: a190 1412 4c8e 8c0b 84e4 4c10 98c3 1c01  ....L.....L.....
-00003330: 4200 0acc 1180 8119 0283 0011 7230 0040  B...........r0.@
-00003340: 86a4 0010 226d 0300 a4c8 0e00 31b2 3500  ...."m......1.5.
-00003350: 408e cc02 1024 4b00 24c9 1500 51b2 0640  @....$K.$...Q..@
-00003360: 963c 0210 2679 00a4 c91e 0071 f207 409e  .<..&y.....q..@.
-00003370: 5c0c 0010 688e 0014 8600 6894 0222 7304  \...h.....h.."s.
-00003380: 0222 11a9 5422 1315 4a35 38a1 0201 9188  ."..T"..J58.....
-00003390: 2412 8944 8180 4844 1289 4422 4acd 1104  $..D..HD..D"J...
-000033a0: 4610 adca c012 89a8 5586 8068 40af 4204  F.......U..h@.B.
-000033b0: 0281 00c5 6a31 0804 4422 9a8d 0094 a116  ....j1..D"......
-000033c0: 0890 ad0c 8340 8070 45a8 0548 5786 4040  .....@.pE..HW.@@
-000033d0: 44bc 5204 0283 4180 7c25 a811 b010 81c0  D.R...A.|%......
-000033e0: 2040 c232 984c 2622 d2a0 0835 231d 8b10   @.2.L&"...5#...
-000033f0: 0850 b228 0312 2a10 1089 4822 112d 4b30  .P.(..*...H".-K0
-00003400: a066 3106 0011 4944 a267 1902 a200 454b  .f1...ID.g....EK
-00003410: 510b 0044 2b9a 96a1 260a 50b5 0cb5 8080  Q..D+...&.P.....
-00003420: ae03 0153 0044 22d1 3002 3106 c308 c440  ...S.D".0.1....@
-00003430: dd61 0442 0c08 6c08 9108 2022 318d 890b  .a.B..l... "1...
-00003440: 0000 0051 1800 002d 0000 001b 8c20 0012  ...Q...-..... ..
-00003450: 60d9 6008 0290 00cb 0663 2080 05a0 3618  `.`......c ...6.
-00003460: 4403 2c00 b541 29fe ffff ff7f 0024 8002  D.,..A)......$..
-00003470: ea00 e883 0d84 0100 c906 e308 8005 a036  ...............6
-00003480: 18c8 002c 00b5 8148 0260 d940 2802 b06c  ...,...H.`.@(..l
-00003490: 2096 ffff ffff 1f00 6703 c2fc ffff ffff   .......g.......
-000034a0: 00b4 0120 017d b0c1 6802 6001 e860 03e1  ... .}..h.`..`..
-000034b0: 1000 1f6c 509e ffff ffff 1f00 3f00 1c00  ...lP.......?...
-000034c0: 0e00 6903 0105 001f 6c20 a2ff ffff ff1f  ..i.....l ......
-000034d0: 0069 0321 09c0 196c 20a6 0038 830d 0455  .i.!...l ..8...U
-000034e0: 0067 b081 a80c e00c 3628 5600 9c41 1020  .g......6(V..A. 
-000034f0: 411a a0c2 06e5 0a80 3308 8220 4803 0849  A.......3.. H..I
-00003500: 1800 0010 0000 0013 8840 1888 0941 3121  .........@...A1!
-00003510: 3026 0807 3241 4894 0941 3281 0804 6498  0&..2AH..A2...d.
-00003520: 102c 1306 a671 2604 cf84 8181 9409 4134  .,...q&.......A4
-00003530: 2190 2608 9334 41a0 aa09 8135 2198 260c  !.&..4A....5!.&.
-00003540: cb24 4d08 2e00 0013 327c c003 3bf8 053b  .$M.....2|..;..;
-00003550: a083 3608 0778 8007 7628 8736 2087 7090  ..6..x..v(.6 .p.
-00003560: 877b 4807 7788 833c 7003 3b70 0338 d860  .{H.w..<p.;p.8.`
-00003570: 0ae5 d006 eda0 07ef d006 f020 0777 0007  ........... .w..
-00003580: 7a30 0772 a007 7320 076d 000f 7270 0771  z0.r..s .m..rp.q
-00003590: a007 7320 077a 3007 72d0 06f0 2007 7720  ..s .z0.r... .w 
-000035a0: 077a 6007 74a0 0776 4007 6d90 0e76 4007  .z`.t..v@.m..v@.
-000035b0: 7a60 0774 d006 e680 0770 a007 7120 0778  z`.t.....p..q .x
-000035c0: d006 ee80 077a 1007 76a0 0773 2007 7a60  .....z..v..s .z`
-000035d0: 0774 d006 b310 0772 8007 4a0f 0811 1243  .t.....r..J....C
-000035e0: 868c 9400 0134 4298 9c22 bc39 5d9e 769f  .....4B..".9].v.
-000035f0: 7d3b 24e0 2602 2117 1000 0000 0100 0000  };$.&.!.........
-00003600: b809 6087 7413 6040 0cea 3000 0000 0000  ..`.t.`@..0.....
-00003610: 0000 c14d 003b a4bb 0003 6258 8701 0000  ...M.;....bX....
-00003620: 0000 0000 086e 02d8 21dd 4618 1883 3c0c  .....n..!.F...<.
-00003630: 0000 0000 0000 4070 13c0 0e09 3fcc 0019  ......@p....?...
-00003640: e661 0000 0000 0000 0082 9b00 7648 3e12  .a..........vH>.
-00003650: 06ca a00f 0300 0000 0000 0010 dc04 b043  ...............C
-00003660: fa13 3340 067a 1800 0000 0000 0080 e026  ..3@.z.........&
-00003670: 801d 52b9 8c01 33ec c300 0000 0000 0000  ..R...3.........
-00003680: 0437 0110 7140 0210 00b0 43d2 99b9 7006  .7..q@....C...p.
-00003690: 7e18 0000 0000 0000 80e0 2600 3613 3c00  ~.........&.6.<.
-000036a0: 0200 7648 bcf4 0bd0 d00f 0300 0000 0000  ..vH............
-000036b0: 0010 dc04 c0dd 0207 4000 c00e 29b5 d640  ........@...)..@
-000036c0: 1afc 6100 0000 0000 0000 829b 0048 5f30  ..a..........H_0
-000036d0: 0108 00e0 a141 0420 0060 8784 6371 400d  .....A. .`..cq@.
-000036e0: ff30 0000 0000 0000 00c1 4d00 3ba4 54db  .0........M.;.T.
-000036f0: 036b 0089 0100 0000 0000 0008 6e02 d821  .k..........n..!
-00003700: 91dc 1c50 c33f 0c00 0000 0000 0040 7013  ...P.?.......@p.
-00003710: c00e e9ee 7021 1072 0101 0000 1000 0000  ....p!.r........
-00003720: 809b 0076 482f 1880 0131 b0c3 0000 0000  ...vH/...1......
-00003730: 0000 0004 3701 ec90 de30 0003 6268 8701  ....7....0..bh..
-00003740: 0000 0000 0000 086e 02d8 21bd 6210 06c6  .......n..!.b...
-00003750: 200f 0300 0000 0000 0010 dc04 b043 82c7   ............C..
-00003760: c00c 9061 1e06 0000 0000 0000 20b8 0960  ...a........ ..`
-00003770: 8764 9341 1860 4348 0c00 0000 0000 0040  .d.A.`CH.......@
-00003780: 7013 c00e e92e 0333 4086 7a18 0000 0000  p......3@.z.....
-00003790: 0000 80e0 2680 1d52 6f06 a710 08b9 8000  ....&..Ro.......
-000037a0: 0000 0800 0000 c04d 003b 2432 0d52 2110  .......M.;$2.R!.
-000037b0: 7201 0100 0010 0000 0080 9b00 7648 ed1a  r...........vH..
-000037c0: a044 20e4 0202 0000 2000 0000 0037 01ec  .D ..... ....7..
-000037d0: 90ea 3740 8740 c805 0400 0040 0000 0000  ..7@.@.....@....
-000037e0: 6e02 d821 f572 900b 8190 0b08 0000 8000  n..!.r..........
-000037f0: 0000 00dc 04b0 43b2 eb00 0c88 c11d 0600  ......C.........
-00003800: 0000 0000 0020 b809 6087 64db 0118 10c3  ..... ..`.d.....
-00003810: 3b0c 0000 0000 0000 4070 13c0 0ec9 be03  ;.......@p......
-00003820: 3020 0678 1800 0000 0000 0080 e026 801d  0 .x.........&..
-00003830: 928d 0760 400c f130 0000 0000 0000 00c1  ...`@..0........
-00003840: 4d00 3b24 3b0f c240 1b44 6200 0000 0000  M.;$;..@.Db.....
-00003850: 0000 829b 0076 48b7 1e98 0132 d8c3 0000  .....vH....2....
-00003860: 0000 0000 0004 3701 ec90 fa3d 0803 6e18  ......7....=..n.
-00003870: 8901 0000 0000 0000 086e 02d8 21f9 7c60  .........n..!.|`
-00003880: 06c8 700f 0300 0000 0000 0010 dc04 b043  ..p............C
-00003890: 22fd 200c bc81 2406 0000 0000 0000 20b8  ". ...$....... .
-000038a0: 0960 8754 fe81 1920 033e 0c00 0000 0000  .`.T... .>......
-000038b0: 0040 7013 c00e 6905 8530 0083 a124 0600  .@p...i..0...$..
-000038c0: 0000 0000 0020 b809 6087 c486 8219 2043  ..... ..`..... C
-000038d0: 3e0c 0000 0000 0000 4070 13c0 904a 1685  >.......@p...J..
-000038e0: 9648 0300 9802 0000 0001 0000 0000 809b  .H..............
-000038f0: 0086 54bf 296c 6d00 0480 0000 0000 0000  ..T.)lm.........
-00003900: 0000 0070 13c0 904a 3f05 ef0d 8000 1800  ...p...J?.......
-00003910: 0000 0400 0000 0000 6e02 1852 e1a8 5013  ........n..R..P.
-00003920: 7100 0013 0100 0020 0000 0000 0070 13c0  q...... .....p..
-00003930: 90aa 6d85 680e 8000 0000 0000 0400 0000  ..m.h...........
-00003940: 0000 6e02 1852 f9ad f0d8 0110 0000 0000  ..n..R..........
-00003950: 8000 0000 0000 c04d 0043 aad6 153a 3c00  .......M.C...:<.
-00003960: 02a0 0000 0010 0000 0000 00b8 0960 48a5  .............`H.
-00003970: be42 a207 4000 0000 0000 0200 0000 0000  .B..@...........
-00003980: 3701 0ca9 e657 70f8 0008 0000 0000 4000  7....Wp.......@.
-00003990: 0000 0000 e026 8021 5508 0b62 e007 4000  .....&.!U..b..@.
-000039a0: 1800 0000 0200 0000 0000 3701 0ca9 c658  ..........7....X
-000039b0: 5840 0108 0000 0000 4000 0000 0000 e026  X@......@......&
-000039c0: 8021 951b 0b8e 2800 0100 0000 0008 0000  .!....(.........
-000039d0: 0000 00dc 0430 a4e2 63c1 d103 2000 0000  .....0..c... ...
-000039e0: 0000 0100 0000 0080 9b00 8654 aa2c 347a  ...........T.,4z
-000039f0: 0004 0000 0000 2000 0000 0000 7013 c090  ...... .....p...
-00003a00: ea96 8599 2005 0098 0000 0000 0100 0000  .... ...........
-00003a10: 0080 9b00 8654 ea2d 40a7 0004 0000 0000  .....T.-@.......
-00003a20: 2000 0000 0000 7013 c090 4abf 052a 1580   .....p...J..*..
-00003a30: 0000 0000 0004 0000 0000 006e 0218 52b9  ...........n..R.
-00003a40: b850 e901 1000 0000 0080 0000 0000 00c0  .P..............
-00003a50: 4d00 43aa 3117 123d 0002 0000 0000 1000  M.C.1..=........
-00003a60: 0000 0000 b809 6048 c5e6 4274 0a40 0000  ......`H..Bt.@..
-00003a70: 0000 0002 0000 0000 0037 010c a9fa 5cf0  .........7....\.
-00003a80: 8555 0080 e900 0000 1000 0000 0000 b809  .U..............
-00003a90: 6048 b5f3 82a2 0700 3021 0000 0002 0000  `H......0!......
-00003aa0: 0000 0037 010c a9ca 5e88 5a01 0800 0000  ...7....^.Z.....
-00003ab0: 0040 0000 0000 00e0 2680 2195 dd0b cc2b  .@......&.!....+
-00003ac0: 0001 0000 0000 0800 0000 0000 dc04 30a4  ..............0.
-00003ad0: 127d 01d2 0300 9800 0000 0000 0000 0000  .}..............
-00003ae0: 809b 0086 54b2 2f70 b100 0400 0000 0020  ....T./p....... 
-00003af0: 0000 0000 0070 13c0 90ca fd05 6a16 8000  .....p......j...
-00003b00: 4800 0000 0000 0000 0000 6e02 1852 89e0  H.........n..R..
-00003b10: 50e9 0110 0000 0000 8000 0000 0000 c04d  P..............M
-00003b20: 0043 aa1b 1c14 3d00 8049 0100 0010 0000  .C....=..I......
-00003b30: 0000 00b8 0960 4815 8603 560b 4000 2c00  .....`H...V.@.,.
-00003b40: 0000 0000 0000 0000 3701 0ca9 f270 b06a  ........7....p.j
-00003b50: 0108 8005 0000 0000 0000 0000 e026 8021  .............&.!
-00003b60: d52b 0ed3 2d00 01c0 0000 0000 0000 0000  .+..-...........
-00003b70: 00dc 0420 b141 a070 b604 0040 1608 0076  ... .A.p...@...v
-00003b80: 0100 0032 1e98 2019 114c 908c 0926 47c6  ...2.. ..L...&G.
-00003b90: 0443 1a8c 0094 a140 b10b 9463 4059 0a94  .C.....@...c@Y..
-00003ba0: 5fe9 155e 390e 9464 6640 0994 7100 ad6a  _..^9..df@..q..j
-00003bb0: 8002 2300 431d ca52 0cab 30ac c250 0792  ..#.C..R..0..P..
-00003bc0: 18c3 2a0c ab30 d461 1cc3 b00a c32a 0c75  ..*..0.a.....*.u
-00003bd0: 2009 31ac c2b0 0a43 1d58 860d ab30 acc2   .1....C.X...0..
-00003be0: 5007 9264 c32a 0cab 30d4 611c d6b0 0ac3  P..d.*..0.a.....
-00003bf0: 2a0c 7520 c935 acc2 b00a 431d 6010 0669  *.u .5....C.`..i
-00003c00: 30ac c2b0 0a43 1d48 a206 c32a 0cab 30d4  0....C.H...*..0.
-00003c10: e17d 6730 acc2 b00a 431d 4882 06c3 2a0c  .}g0....C.H...*.
-00003c20: ab30 d4c1 7565 30ac c2b0 0a43 1d48 6206  .0..ue0....C.Hb.
-00003c30: c32a 0cab 30d4 a16d 6330 acc2 b00a 431d  .*..0..mc0....C.
-00003c40: 4842 06c3 2a0c ab40 041c b29a b470 d862  HB..*..@.....p.b
-00003c50: e2c2 a1cb c90b 872f 2630 1cc2 9ec4 7018  ......./&0....p.
-00003c60: 8322 c3a1 2cca 0c87 3329 3432 e448 000e  ."..,...3)42.H..
-00003c70: 8c89 d5a5 b1d1 a5b9 cd29 5885 b1d5 9515  .........)X.....
-00003c80: c9c9 bdc9 29c4 0160 6d01 0000 84c9 c985  ....)..`m.......
-00003c90: e581 a4cd 81d0 bdbd 8188 a59d ed80 8085  ................
-00003ca0: c9c9 b9cc a5e9 9581 a880 84c9 c9b9 90d1  ................
-00003cb0: e5c1 95b9 a4d1 95b5 cda5 e995 8181 a4cd  ................
-00003cc0: 81b0 85c9 9d95 c981 d0a1 85b9 81d0 a195  ................
-00003cd0: 81b4 85e1 a5b5 d5b5 81c0 bdcd cda5 89b1  ................
-00003ce0: 9581 cca5 e995 b9c4 0514 c609 381d c60d  ............8...
-00003cf0: b810 2229 9b1b 1c78 5469 71b0 b87d a874  ..")...xTiq..}.t
-00003d00: e98d 25c0 d4a9 1783 a40c e013 74c5 86cd  ..%.........t...
-00003d10: 4484 5fa4 96bf 9680 b91a adbb b292 72d5  D._...........r.
-00003d20: c604 674b ba6d 6d8c c1be ff15 6f93 e372  ..gK.mm.....o..r
-00003d30: a7ed 4f0a e4a0 7c4a 8ca6 8331 36e6 944d  ..O...|J...16..M
-00003d40: f31f 9d4c af17 b52d 2977 51c0 abda d173  ...L...-)wQ....s
-00003d50: 550e d7ec 214d 710f 716e 06bd cda4 fc6e  U...!Mq.qn.....n
-00003d60: 52e1 3815 00f3 ba29 4fb2 06fb 20e5 2757  R.8....)O... .'W
-00003d70: 5c6d 924a fad0 bc08 6205 bf0b c00f 812e  \m.J....b.......
-00003d80: cfc8 4844 5fcd ef24 45da 05e0 c098 585d  ..HD_..$E.....X]
-00003d90: 1a1b 5d9a db9c 8255 185b 5d59 919c dc9b  ..]....U.[]Y....
-00003da0: 9c42 1c00 9623 0000 409d 5b98 185b 1908  .B...#..@.[..[..
-00003db0: dd1b 8898 dc5b 18d9 58d8 1c1d 4898 dc59  .....[..X...H..Y
-00003dc0: 5d5b 991b 1d48 0c08 dd1b c85b 1d1d 5c1d  ][...H.....[..\.
-00003dd0: 1d48 989c 5c58 9e82 511a 5b19 88c8 4bd5  .H..\X..Q.[...K.
-00003de0: 5c99 dcdc cb5c 5adb 9bdb 0b51 d9dc 1add  \....\Z....Q....
-00003df0: 1bdc 4b99 9bdd dccb 5c5a 9b58 d817 5999  ..K.....\Z.X..Y.
-00003e00: ddcb 5c5a 9b58 d84b 5b1a 5e9a dbdc 8b59  ..\Z.X.K[.^....Y
-00003e10: 5918 5d9d 5cd9 5719 1e9d 5cd8 185d da9b  Y.].\.W...\..]..
-00003e20: db57 5b1a 5e9a 9b0b 5c9e 080b 085b 9a5b  .W[.^...\....[.[
-00003e30: 1948 0c4e 0e0b 485c 4061 9c80 d361 dc80  .H.N..H\@a...a..
-00003e40: 0b31 96fb 0860 a222 c2bb a608 1026 c469  .1...`.".....&.i
-00003e50: 4ce4 421a 5f18 1069 2287 b245 3b3d 9fa7  L.B._..i"..E;=..
-00003e60: dd67 50d1 6d4f cbdf ee76 d94d d781 be5a  .gP.mO...v.M...Z
-00003e70: 270c e7ac b7c5 e1a2 db5e 9ba7 dbe2 b0ad  '........^......
-00003e80: 9dc6 a7dd 7319 cd5c 0ed3 ebf2 f2b7 8ca7  ....s..\........
-00003e90: cbc3 637a faed feb6 d3f8 b45b 2633 96c3  ..cz.......[&3..
-00003ea0: f4ba bc5c c4d3 e5e1 313d fd76 37d3 f8b4  ...\....1=.v7...
-00003eb0: 3b06 1b93 d373 3a49 46ab d58a b5a0 5c1e  ;....s:IF.....\.
-00003ec0: ce27 c9cc b4ac 180b deda 757a 58cc 2edf  .'........uzX...
-00003ed0: c2ec f4d9 5d26 176b 41b9 3c9c 4f92 9969  ....]&.kA.<.O..i
-00003ee0: 5931 16bc b5eb f4b0 985d be85 d9e9 b3bb  Y1.......]......
-00003ef0: 4c2e 1244 7161 1c76 9fe8 a0ba 5bfc c683  L..Dqa.v....[...
-00003f00: c272 7938 0f32 cbdf 6d10 34ff 14ab cb63  .ry8.2..m.4....c
-00003f10: 3a28 eda6 bf41 ee30 3d6d 2f83 ec61 76bd  :(...A.0=m/..av.
-00003f20: ec02 81a8 e832 e82d 5697 c774 503b 9c17  .....2.-V..tP;..
-00003f30: 9741 6f33 280c 22a7 cde6 b2bc eca6 83e8  .Ao3(.".........
-00003f40: 7978 9924 4a06 e0b2 dbee 1abf dd73 fa1c  yx.$J........s..
-00003f50: 0c4a cf41 ce2a 9309 4abb 4160 7939 4cfe  .J.A.*..J.A`y9L.
-00003f60: 8edf ee39 1d4c 1455 83ba 7bed 7edf dda0  ...9.L.U..{.~...
-00003f70: b25c fe96 83ee e8b2 1b34 0eb3 d969 f719  .\.......4...i..
-00003f80: e40e d3d3 f632 c85c 778f e9e9 b79b 2c4a  .....2.\w.....,J
-00003f90: 073c 77bd 2d0e bbc6 6f79 d935 86d7 5d43  .<w.-...oy.5..]C
-00003fa0: 6875 f876 d3cb 783a e82d 5697 c774 5098  hu.v..x:.-V..tP.
-00003fb0: 0e82 e16f e6b1 d85c ab85 c932 18ce 4798  ...o...\...2..G.
-00003fc0: 3c05 c081 31b1 ba34 36ba 34b7 3905 ab30  <...1..46.4.9..0
-00003fd0: b6ba b222 39b9 3739 8538 00ac 0f00 0000  ..."9.79.8......
-00003fe0: b7b2 b330 ba34 bb32 10b2 b4b6 32b7 b9b4  ...0.4.2....2...
-00003ff0: 37b7 3910 b737 3a90 3036 b6b7 bb32 b2b8  7.9..7:.06...2..
-00004000: 80c2 3801 a7c3 b801 17d2 241f 000e 8c89  ..8.......$.....
-00004010: d5a5 b1d1 a5b9 cd29 24b9 9195 e115 c9c9  .......)$.......
-00004020: bdc9 29c4 0160 5100 0000 9c95 d1a5 d195  ..)..`Q.........
-00004030: b581 bcd5 d181 bc99 81c8 85b9 9d95 c505  ................
-00004040: 14c6 0938 1dc6 0db8 1027 fb00 7060 4cac  ...8.....'..p`L.
-00004050: 2e8d 8d2e cd6d 4ea1 a9ac ed4d 2eaf 484e  .....mN....M..HN
-00004060: ee4d 4e21 0e00 8b02 0000 602c cccd ed8d  .MN!......`,....
-00004070: 0e24 8c8d ed6d 2c8c ae0c 842d 6d8e 2e2e  .$...m,....-m...
-00004080: a030 4ec0 e930 6ec0 853c f907 8003 6362  .0N..0n..<....cb
-00004090: 7569 6c74 696e 730a 5a65 726f 4469 7669  uiltins.ZeroDivi
-000040a0: 7369 6f6e 4572 726f 720a 7100 5810 0000  sionError.q.X...
-000040b0: 0064 6976 6973 696f 6e20 6279 207a 6572  .division by zer
-000040c0: 6f71 0185 7102 4e87 7103 2e04 ca95 001c  oq..q.N.q.......
-000040d0: 1813 ab4b 63a3 4b73 9b53 089a 9b2b 93a3  ...Kc.Ks.S...+..
-000040e0: 4b7b 732b 9293 7b93 5388 0348 c122 0000  K{s+..{.S..H."..
-000040f0: 0048 6b83 638b 0bc0 8a02 0000 78a9 9a2b  .Hk.c.......x..+
-00004100: 939b 7b99 4b6b 7b73 7b71 197b 7323 0b7b  ..{.Kk{s{q.{s#.{
-00004110: 2973 b39b 7b99 4b6b 130b fb22 2bb3 7b61  )s..{.Kk..."+.{a
-00004120: 4b13 7b81 cba3 437b 739b 71b1 7999 4ba3  K.{...C{s.q.y.K.
-00004130: 2b6b 810b 1b5b 0b3b 2b9b 7b71 ab6b 130b  +k...[.;+.{q.k..
-00004140: 7b71 837b 614b 730b 633b 7381 cb8b 1368  {q.{aKs.c;s....h
-00004150: f242 388c 1b38 8c23 7001 00b1 1800 009e  .B8..8.#p.......
-00004160: 0000 0033 0880 1cc4 e11c 6614 013d 8843  ...3......f..=.C
-00004170: 3884 c38c 4280 0779 7807 7398 710c e600  8...B..yx.s.q...
-00004180: 0fed 100e f480 0e33 0c42 1ec2 c11d cea1  .......3.B......
-00004190: 1c66 3005 3d88 4338 8483 1bcc 033d c843  .f0.=.C8.....=.C
-000041a0: 3d8c 033d cc78 8c74 7007 7b08 0779 4887  =..=.x.tp.{..yH.
-000041b0: 7070 077a 7003 7678 8770 2087 19cc 110e  pp.zp.vx.p .....
-000041c0: ec90 0ee1 300f 6e30 0fe3 f00e f050 0e33  ....0.n0.....P.3
-000041d0: 10c4 1dde 211c d821 1dc2 611e 6630 893b  ....!..!..a.f0.;
-000041e0: bc83 3bd0 4339 b403 3cbc 833c 8403 3bcc  ..;.C9..<..<..;.
-000041f0: f014 7660 077b 6807 3768 8772 6807 3780  ..v`.{h.7h.rh.7.
-00004200: 8770 9087 7060 0776 2807 76f8 0576 7887  .p..p`.v(.v..vx.
-00004210: 7780 875f 0887 7118 8772 9887 7998 812c  w.._..q..r..y..,
-00004220: eef0 0eee e00e f5c0 0eec 3003 62c8 a11c  ..........0.b...
-00004230: e4a1 1ccc a11c e4a1 1cdc 611c ca21 1cc4  ..........a..!..
-00004240: 811d ca61 06d6 9043 39c8 4339 9843 39c8  ...a...C9.C9.C9.
-00004250: 4339 b8c3 3894 4338 8803 3b94 c32f bc83  C9..8.C8..;../..
-00004260: 3cfc 823b d403 3bb0 c30c c769 8770 5887  <..;..;....i.pX.
-00004270: 7270 8374 6807 7860 8774 1887 74a0 8719  rp.th.x`.t..t...
-00004280: ce53 0fee 000f f250 0ee4 900e e340 0fe1  .S.....P.....@..
-00004290: 200e ec50 0e33 2028 1ddc c11e c241 1ed2   ..P.3 (.....A..
-000042a0: 211c dc81 1edc e01c e4e1 1dea 011e 6618  !.............f.
-000042b0: 5138 b043 3a9c 833b cc50 2476 6007 7b68  Q8.C:..;.P$v`.{h
-000042c0: 0737 6087 7778 0778 9851 4cf4 900f f050  .7`.wx.x.QL....P
-000042d0: 0e33 1e6a 1eca 611c e821 1dde c11d 7e01  .3.j..a..!....~.
-000042e0: 1ee4 a11c cc21 1df0 6106 5485 8338 ccc3  .....!..a.T..8..
-000042f0: 3bb0 433d d043 39fc c23c e443 3b88 c33b  ;.C=.C9..<.C;..;
-00004300: b0c3 8cc5 0a87 7998 8777 1887 7408 077a  ......y..w..t..z
-00004310: 2807 7298 815c e310 0eec c00e e550 0ef3  (.r..\.......P..
-00004320: 3023 c1d2 411e e4e1 17d8 e11d de01 1e66  0#..A..........f
-00004330: 4819 3bb0 833d b483 1b84 c338 8c43 39cc  H.;..=.....8.C9.
-00004340: c33c b8c1 39c8 c33b d403 3ccc 48b4 7108  .<..9..;..<.H.q.
-00004350: 0776 6007 7108 8771 5887 19db c60e ec60  .v`.q..qX......`
-00004360: 0fed e006 f020 0fe5 300f e520 0ff6 500e  ..... ..0.. ..P.
-00004370: 6e10 0ee3 300e e530 0ff3 e006 e9e0 0ee4  n...0..0........
-00004380: 500e f830 43e1 da21 1de6 a11c f001 1eca  P..0C..!........
-00004390: 611c e861 46d4 d9c3 3884 033b b0c3 2fd8  a..aF...8..;../.
-000043a0: 433a cc43 3a88 433a b043 3ad0 433e cc68  C:.C:.C:.C:.C>.h
-000043b0: 3c79 2807 7af8 8574 9887 5f90 8770 4887  <y(.z..t.._..pH.
-000043c0: 7928 8719 ce87 0ee5 100e f010 0eec c00e  y(..............
-000043d0: ef30 0ef3 900e f450 0e00 0079 2000 001e  .0.....P...y ...
-000043e0: 0000 0072 1e48 2043 880c 1909 7232 4820  ...r.H C....r2H 
-000043f0: 2381 8c91 91d1 44a0 1028 643c 3132 428e  #.....D..(d<12B.
-00004400: 9021 a318 1012 000e 0000 0062 7261 6e63  .!.........branc
-00004410: 685f 7765 6967 6874 7300 0023 0843 2d8c  h_weights..#.C-.
-00004420: 200c b630 82b0 06b7 3045 00cc 3004 c230   ..0....0E..0..0
-00004430: 4340 c848 6082 d273 ab6b 130b fb0a 933b  C@.H`..s.k.....;
-00004440: 9bfb 6a0b cbfb 0a63 bb0b cb9b fb72 2b2b  ..j....c.....r++
-00004450: 23fb 7293 a31b 4520 0800 00a9 1800 0011  #.r...E ........
-00004460: 0000 000b 0a72 2887 7780 077a 5870 9843  .....r(.w..zXp.C
-00004470: 3db8 c338 b043 39d0 c382 e61c c6a1 0de8  =..8.C9.........
-00004480: 411e c2c1 1de6 211d e821 1dde c11d 1634  A.....!..!.....4
-00004490: e360 0ee7 500f e120 0fe4 400f e120 0fe7  .`..P.. ..@.. ..
-000044a0: 500e f400 0000 00d1 1000 0006 0000 0007  P...............
-000044b0: cc3c a483 3b9c 033b 9403 3da0 833c 9443  .<..;..;..=..<.C
-000044c0: 3890 c301 0000 0061 2000 0066 0900 0013  8......a ..f....
-000044d0: 0477 100b 0400 0016 0000 0034 28a0 5228  .w.........4(.R(
-000044e0: 8622 2883 42a8 0212 8d00 1444 0994 41c1  ."(.B......D..A.
-000044f0: 1441 2114 480d 1450 8594 8365 a1c2 b240  .A!.H..P...e...@
-00004500: 5180 0105 1c50 8002 052c 5080 0305 3c50  Q....P...,P...<P
-00004510: 0585 5150 0556 70e4 1d01 a0c2 0800 8dc6  ..QP.Vp.........
-00004520: 0840 1004 4110 0441 d0ff 8f11 00ea ce00  .@..A..A........
-00004530: 0000 00f1 3000 00d2 0000 0022 47c8 9051  ....0......"G..Q
-00004540: 268c 6b01 0000 00ae 800b b780 2996 3fa0  &.k.........).?.
-00004550: c449 005f 5a4e 356e 756d 6261 326e 7038  .I._ZN5numba2np8
-00004560: 6172 7261 796f 626a 3133 6e75 6d70 795f  arrayobj13numpy_
-00004570: 6675 6c6c 5f6e 6431 3224 3363 6c6f 6361  full_nd12$3cloca
-00004580: 6c73 2433 6539 6675 6c6c 2432 3435 3645  ls$3e9full$2456E
-00004590: 3855 6e69 5475 706c 6549 784c 6932 4545  8UniTupleIxLi2EE
-000045a0: 645f 5a4e 356e 756d 6261 326e 7038 6172  d_ZN5numba2np8ar
-000045b0: 7261 796f 626a 3133 6e75 6d70 795f 6675  rayobj13numpy_fu
-000045c0: 6c6c 5f6e 6431 3224 3363 6c6f 6361 6c73  ll_nd12$3clocals
-000045d0: 2433 6539 6675 6c6c 2432 3435 3645 3855  $3e9full$2456E8U
-000045e0: 6e69 5475 706c 6549 784c 6932 4545 643a  niTupleIxLi2EEd:
-000045f0: 2025 6578 6369 6e66 6f5f 5a4e 356e 756d   %excinfo_ZN5num
-00004600: 6261 326e 7038 6172 7261 796f 626a 3133  ba2np8arrayobj13
-00004610: 6e75 6d70 795f 6675 6c6c 5f6e 6431 3224  numpy_full_nd12$
-00004620: 3363 6c6f 6361 6c73 2433 6539 6675 6c6c  3clocals$3e9full
-00004630: 2432 3435 3645 3855 6e69 5475 706c 6549  $2456E8UniTupleI
-00004640: 784c 6932 4545 643a 2025 7265 7470 7472  xLi2EEd: %retptr
-00004650: 6c6c 766d 2e6c 6f6f 702e 756e 726f 6c6c  llvm.loop.unroll
-00004660: 2e64 6973 6162 6c65 4c56 6572 446f 6d61  .disableLVerDoma
-00004670: 696e 6c6c 766d 2e6c 6f6f 702e 6973 7665  inllvm.loop.isve
-00004680: 6374 6f72 697a 6564 5f5a 4e35 6e75 6d62  ctorized_ZN5numb
-00004690: 6132 6e70 366c 696e 616c 6731 345f 6765  a2np6linalg14_ge
-000046a0: 745f 6e6f 726d 5f69 6d70 6c31 3224 3363  t_norm_impl12$3c
-000046b0: 6c6f 6361 6c73 2433 6531 346f 6e65 445f  locals$3e14oneD_
-000046c0: 696d 706c 2432 3432 3745 3541 7272 6179  impl$2427E5Array
-000046d0: 4964 4c69 3145 3143 376d 7574 6162 6c65  IdLi1E1C7mutable
-000046e0: 3761 6c69 676e 6564 4532 376f 6d69 7474  7alignedE27omitt
-000046f0: 6564 2432 3864 6566 6175 6c74 2433 644e  ed$28default$3dN
-00004700: 6f6e 6524 3239 5f5a 4e35 6e75 6d62 6132  one$29_ZN5numba2
-00004710: 6e70 366c 696e 616c 6731 345f 6765 745f  np6linalg14_get_
-00004720: 6e6f 726d 5f69 6d70 6c31 3224 3363 6c6f  norm_impl12$3clo
-00004730: 6361 6c73 2433 6531 346f 6e65 445f 696d  cals$3e14oneD_im
-00004740: 706c 2432 3432 3745 3541 7272 6179 4964  pl$2427E5ArrayId
-00004750: 4c69 3145 3143 376d 7574 6162 6c65 3761  Li1E1C7mutable7a
-00004760: 6c69 676e 6564 4532 376f 6d69 7474 6564  lignedE27omitted
-00004770: 2432 3864 6566 6175 6c74 2433 644e 6f6e  $28default$3dNon
-00004780: 6524 3239 3a20 2565 7863 696e 666f 5f5a  e$29: %excinfo_Z
-00004790: 4e35 6e75 6d62 6132 6e70 366c 696e 616c  N5numba2np6linal
-000047a0: 6731 345f 6765 745f 6e6f 726d 5f69 6d70  g14_get_norm_imp
-000047b0: 6c31 3224 3363 6c6f 6361 6c73 2433 6531  l12$3clocals$3e1
-000047c0: 346f 6e65 445f 696d 706c 2432 3432 3745  4oneD_impl$2427E
-000047d0: 3541 7272 6179 4964 4c69 3145 3143 376d  5ArrayIdLi1E1C7m
-000047e0: 7574 6162 6c65 3761 6c69 676e 6564 4532  utable7alignedE2
-000047f0: 376f 6d69 7474 6564 2432 3864 6566 6175  7omitted$28defau
-00004800: 6c74 2433 644e 6f6e 6524 3239 3a20 2572  lt$3dNone$29: %r
-00004810: 6574 7074 7200 0013 8461 1626 0803 2dac  etptr....a.&..-.
-00004820: 1026 64c5 404d c98a a19a 9415 8265 062b  .&d.@M.......e.+
-00004830: 848b 5921 60d7 0a21 bb56 08da b542 d8d6  ..Y!`..!.V...B..
-00004840: 6085 c0ad c10a a133 8315 8267 062b 84cf  `......3...g.+..
-00004850: 0c56 0860 e0ac 18c2 000c 9e15 8318 8001  .V.`............
-00004860: b461 0822 6983 5051 1b86 6010 3604 cb86  .a."i.PQ..`.6...
-00004870: 00db 1064 1b02 6d83 8065 1b84 46d8 2088  ...d..m..e..F. .
-00004880: 4118 0033 1163 30d4 0229 cc44 1443 2d90  A..3.c0..).D.C-.
-00004890: c288 4101 8420 18e8 413e e4c1 8841 0184  ..A.. ..A>...A..
-000048a0: 2018 e841 3ec0 c1ad 011d ec70 4310 0668   ..A>......pC..h
-000048b0: 30cb 7004 c188 8101 8420 18b4 814d d841  0.p...... ...M.A
-000048c0: 1b8c 2604 c068 8210 8c18 1840 0882 411b  ..&..h.....@..A.
-000048d0: e484 4006 a309 4170 43b0 b30c 8710 dc1c  ..@...ApC.......
-000048e0: 94c1 8d26 10c0 8881 0184 2018 bc41 4f04  ...&...... ..AO.
-000048f0: 71d0 0042 7006 196c 9702 1219 6e10 0537  q..Bp..l....n..7
-00004900: 0083 e106 3d78 0330 3821 d859 0664 0866  ....=x.08!.Y.d.f
-00004910: 0988 810a 3188 0871 1806 2ac4 a021 c861  ....1..q..*..!.a
-00004920: c020 0e60 60b8 21f8 0334 4062 0e40 60b8  . .``.!..4@b.@`.
-00004930: 2150 0534 986e 10ee 2098 6e28 f080 986e  !P.4.n.. .n(...n
-00004940: 4084 e208 634f 3105 b940 8136 12a0 60d8  @...cO1..@.6..`.
-00004950: 8008 c680 0066 1908 8418 8e70 fdff ffff  .....f.....p....
-00004960: 410c fcc0 0c32 10c9 0805 ecff ffff 0f62  A....2.........b
-00004970: 1000 c208 85ec ffff ff0f 62f0 0740 301c  ..........b..@0.
-00004980: 21fb ffff ff83 1888 8219 cc32 2846 9099  !..........2(F..
-00004990: 28f3 17b8 3b6c 4004 0201 74d3 000e a500  (...;l@...t.....
-000049a0: 1319 7077 d880 084e 8100 ba69 1087 5358  ..pw...N...i..SX
-000049b0: 8561 0322 2803 02e8 a661 1c50 6115 860d  .a."(....a.Pa...
-000049c0: 8800 1508 a09b 0672 4885 5518 3620 828e  .......rH.U.6 ..
-000049d0: 00ba 8928 0755 8005 5518 3620 825f 2080  ...(.U..U.6 ._ .
-000049e0: 6e22 cc61 1562 2115 860d 88e0 1608 a09b  n".a.b!.........
-000049f0: 8873 6085 5860 8561 0322 2803 02e8 2602  .s`.X`.a."(...&.
-00004a00: 1d5a 4116 5661 d880 085a 8100 460c 0a20  .ZA.Va...Z..F.. 
-00004a10: 04c1 400f dcc2 1746 0c0a 2004 c140 0fdc  ..@....F.. ..@..
-00004a20: e21c 762c 063a c4e0 0603 3b20 8940 2480  ..v,.:....; .@$.
-00004a30: 818e e1fe ec80 4e02 3a01 521d b83b 6c40  ......N.:.R..;l@
-00004a40: 0403 01ac 30dc 500e b160 06b3 0c89 11a0  ....0.P..`......
-00004a50: 39a8 0208 0c37 f8c2 2c98 c174 c32f d042  9....7..,..t./.B
-00004a60: 9082 4850 0840 60b8 211c 6a01 0c86 1bc4  ..HP.@`.!.j.....
-00004a70: 611d c060 b881 1d6e 010c 2e10 76ba a11c  a..`...n....v...
-00004a80: dc41 b842 d8e9 06e1 1c8c 1103 0308 4130  .A.B..........A0
-00004a90: 6803 d908 7a61 3421 0846 1304 e088 5b80  h...za4!.F....[.
-00004aa0: 0b78 0131 0807 18b8 8317 e090 5dd0 1bc8  .x.1........]...
-00004ab0: 4191 0862 e096 5ed0 63cc 41af 09e2 f801  A..b..^.c.A.....
-00004ac0: 1de4 fae1 1cee ea41 1de4 ec21 1d6e 9640  .......A...!.n.@
-00004ad0: 19a8 1003 df48 78a1 18a8 1003 3e48 c0a1  .....Hx.....>H..
-00004ae0: 186e e087 7830 8359 86a5 08f2 2444 39dc  .n..x0.Y....$D9.
-00004af0: 40cc 031a 4c37 a004 3d04 1718 7001 4ac8  @...L7..=...p.J.
-00004b00: 0505 dc30 12d2 4602 2b04 3904 b401 8420  ...0..F.+.9.... 
-00004b10: 1f0e 69e0 5e22 9063 02b8 4680 7306 9825  ..i.^".c..F.s..%
-00004b20: 6006 2ac4 4044 96b3 ab83 818a 3560 85c5  `.*.@D......5`..
-00004b30: 66ea 60a0 420c 7461 09bb 3a48 9810 e588  f.`.B.ta..:H....
-00004b40: 4101 8420 18e8 816f f8c4 7003 5112 6830  A.. ...o..p.Q.h0
-00004b50: dd10 1326 115c 60c0 0531 2117 1430 6250  ...&.\`..1!..0bP
-00004b60: 0021 0806 7a30 1e3a 31cb e034 c8b0 0141  .!..z0.:1..4...A
-00004b70: 1669 4200 5b1b b30c 0fb4 06c3 0604 59a0  .iB.[.........Y.
-00004b80: 0901 6c6d 0c37 b481 4a98 c188 8101 8420  ..lm.7..J...... 
-00004b90: 18bc 817f ac81 4c34 8010 a044 06db a580  ......L4...D....
-00004ba0: 4466 1922 3a28 861b 72a2 25c4 6096 41ca  Df.":(..r.%.`.A.
-00004bb0: 82e1 86b1 7009 3198 65a8 a660 b8a1 0d5c  ....p.1.e..`...\
-00004bc0: 820c 6619 dc80 0ad2 2744 798d 04d7 1381  ..f.....'Dy.....
-00004bd0: dc10 c02c 0136 dc20 0733 4106 b30c 6b60  ...,.6. .3A...k`
-00004be0: 0539 16a2 3ce9 8213 8b40 6e08 6096 e01a  .9..<....@n.`...
-00004bf0: a810 033c b0e2 e11a a810 03c2 6a87 6ba0  ...<........j.k.
-00004c00: 420c d2e1 d213 2b05 9252 3022 5990 9482  B.....+..R0"Y...
-00004c10: 11b9 6088 33c4 42d2 0a6c 0308 8190 0169  ..`.3.B..l.....i
-00004c20: 870d 88a0 2080 7b8b 0532 2029 0523 727b  .... .{..2 ).#r{
-00004c30: f140 0624 a560 442e 20e2 a2b6 900c 83c0  .@.$.`D. .......
-00004c40: 3680 1008 0d20 0470 9101 6987 0d88 c020  6.... .p..i.... 
-00004c50: 80bc 487a 7cf1 1692 4260 1b40 0884 0c48  ..Hz|...B`.@...H
-00004c60: 4bc1 88a4 47d2 5b8d ba90 1402 db00 4220  K...G.[.......B 
-00004c70: 6440 5a0a 46e4 8223 6e0c fe42 720e 02db  d@Z.F..#n..Br...
-00004c80: 0042 2034 8010 f045 06a4 1d36 2002 8300  .B 4...E...6 ...
-00004c90: 0e17 d200 3220 2905 2372 bdd0 0690 0149  ....2 ).#r.....I
-00004ca0: 2918 910b 88b8 3758 0dc9 3f08 6c03 0881  ).....7X..?.l...
-00004cb0: d000 42b0 1a19 9076 d880 080c 0240 3a58  ..B....v.....@:X
-00004cc0: 0d18 383b 2007 383c 3807 186e 5087 010c  ..8; .8<8..nP...
-00004cd0: 6619 d6e0 0a06 2ac4 0024 a85d c006 2ac4  f.....*..$.]..*.
-00004ce0: e016 30b6 a112 1c48 9a03 4929 1811 1a46  ..0....H..I)...F
-00004cf0: e402 21ce d80d c957 086c 0308 8190 0169  ..!....W.l.....i
-00004d00: 870d 88a0 2080 438f 0532 2029 0523 42cc  .... .C..2 ).#B.
-00004d10: 885c 20c4 3de4 2189 0b81 6d00 2110 1a40  .\ .=.!...m.!..@
-00004d20: 08ce 2303 d20e 1b10 8141 0059 91f4 e6c3  ..#......A.Y....
-00004d30: 3c24 85c0 3680 1008 1990 9682 11a1 6c44  <$..6.........lD
-00004d40: 2e10 e2b8 f890 2c87 c036 8010 080d 2004  ......,..6.... .
-00004d50: ee91 0169 870d 88c0 2080 5309 3180 0c48  ...i.... .S.1..H
-00004d60: 4ac1 88d0 188c c805 429c 19ec 87e4 3b04  J.......B.....;.
-00004d70: b601 8440 6800 21d8 8f0c 483b 6c40 0406  ...@h.!...H;l@..
-00004d80: 01e0 1aec 070c 5c1b d004 0c37 e484 0006  ......\....7....
-00004d90: b30c 6e80 05c3 0d37 2222 6230 cba0 71c1  ..n....7""b0..q.
-00004da0: 7043 5888 0819 cc32 c4c1 16cc 12a4 c170  pCX....2.......p
-00004db0: 435a fc07 19cc 3274 6210 0c74 8881 0b89  CZ....2tb..t....
-00004dc0: 810b 71a4 8206 c30d 6081 2260 7065 21c4  ..q.....`."`pe!.
-00004dd0: 2c03 1878 c22c c137 5021 06d1 6778 0315  ,..x.,.7P!..gx..
-00004de0: 6210 7da6 e2e5 4890 346d 82a4 248c 0809  b.}...H.4m..$...
-00004df0: 2372 8110 6d24 8cc4 316c 4004 0201 2002  #r..m$..1l@... .
-00004e00: 2330 70c8 8ac0 7043 4023 6030 cb00 065f  #0p...pC@#`0..._
-00004e10: 3050 2106 5c67 7cc3 0dcd 8a90 c12c 031d  0P!.\g|......,..
-00004e20: 8441 304b a006 e912 014d 9508 6c8a 4540  .A0K.....M..l.E@
-00004e30: db48 6089 bec8 20b0 0d20 143a 9234 11d0  .H`... .. .:.4..
-00004e40: e106 c110 83e1 0681 2083 1302 1d6e 308b  ........ ....n0.
-00004e50: 440c 861b 9283 0c4e 08f4 8860 6719 ba31  D......N...`g..1
-00004e60: 0886 1b46 a34c c060 96c1 0cc8 20c8 9e20  ...F.L.`.... .. 
-00004e70: 69c2 0549 4918 9139 0616 09fc 658e a145  i..II..9....e..E
-00004e80: 847f 9963 7091 0164 e618 5e84 0819 3246  ...cp..d..^...2F
-00004e90: 648e 2146 8291 9963 9011 8164 e618 6664  d.!F...c...d..fd
-00004ea0: 2899 3906 1a21 4ce6 8824 0619 021b d191  (.9..!L..$......
-00004eb0: 2b94 1864 0870 8447 ce58 6290 21d0 111f  +..d.p.G.Xb.!...
-00004ec0: b983 8941 8680 47c0 84a8 1199 63f0 9100  ...A..G.....c...
-00004ed0: 66e6 187e 4488 9939 0630 1964 668e 214c  f..~D..9.0.df.!L
-00004ee0: 8899 216c 44e6 18c6 24a8 9939 0632 116c  ..!lD...$..9.2.l
-00004ef0: 668e a14c 869b 9963 3013 0267 8e48 6290  f..L...c0..g.Hb.
-00004f00: 2140 1336 b942 8941 8640 4ddc e48c 2506  !@.6.B.A.@M...%.
-00004f10: 1902 3681 933b 9818 6408 dc44 4e66 09ca  ..6..;..d..DNf..
-00004f20: 60a0 420c 708a 0c66 a10c 062a c480 75c8  `.B.p..f...*..u.
-00004f30: 6016 cae0 8456 910c 8dc0 3680 1008 197c  `....V....6....|
-00004f40: 77d8 8008 3e02 3823 5624 4b23 b00d 2004  w...>.8#V$K#.. .
-00004f50: 4203 0801 ab64 f0dd 6103 2210 0302 b8c5  B....d..a.".....
-00004f60: 5624 5523 b00d 2004 4203 0801 ab64 f0dd  V$U#.. .B....d..
-00004f70: 6103 2228 0302 3868 5724 5f23 b00d 2004  a."(..8hW$_#.. .
-00004f80: 4203 0801 ac64 f0dd 6103 2240 0302 b80a  B....d..a."@....
-00004f90: 5c24 6923 b00d 2004 4203 0801 ad64 f0dd  \$i#.. .B....d..
-00004fa0: 6103 2208 0302 38ad 5c24 7323 b00d 2004  a."...8.\$s#.. .
-00004fb0: 4203 0801 ae64 f0dd 6103 2220 0302 b84f  B....d..a." ...O
-00004fc0: 5d24 7d23 b00d 2004 4203 0801 af64 f0dd  ]$}#.. .B....d..
-00004fd0: 6103 2238 0302 3832 7817 c9f1 086c 0308  a."8..82x....l..
-00004fe0: 81d0 0042 002e 197c 77d8 8008 d480 002e  ...B...|w.......
-00004ff0: 0dd8 052e 0dc4 0586 1b82 7b01 8359 0633  ..........{..Y.3
-00005000: 2883 60a0 420c e06b 0c8c 3218 6e98 917c  (.`.B..k..2.n..|
-00005010: 0183 5906 3438 8320 e383 a449 2224 2561  ..Y.48. ...I"$%a
-00005020: 44e6 18c0 2590 9d39 8670 1166 678e 415c  D...%..9.p.fg.A\
-00005030: 06da 9963 1817 a276 c818 9139 8672 096e  ...c...v...9.r.n
-00005040: 678e c15c 04dc 9963 3897 2177 e618 d085  g..\...c8.!w....
-00005050: d09d 2392 1864 08d4 c55d ae50 6290 2160  ..#..d...].Pb.!`
-00005060: 1778 3963 8941 86c0 5de4 e50e 2606 1902  .x9c.A..]...&...
-00005070: 78a1 9736 1240 c4ca e0bb c306 4490 1040  x..6.@......D..@
-00005080: 1b09 82ca 64f0 dd61 0322 4808 a08d 0422  ....d..a."H...."
-00005090: 6632 f8ee b001 1124 04d0 4682 f12f 197c  f2.....$..F../.|
-000050a0: 77d8 8008 1202 9825 4083 e186 3c89 1330  w......%@...<..0
-000050b0: 9865 a083 2e18 a810 0339 da76 210d 062a  .e.......9.v!..*
-000050c0: c4e0 16d2 00ce b684 1192 5230 2249 9094  ..........R0"I..
-000050d0: 8211 b960 8833 7a46 3246 02db 0042 2064  ...`.3zF2F...B d
-000050e0: 40da 6103 2228 0880 9211 39ba 6120 0392  @.a."(....9.a ..
-000050f0: 5230 2217 1071 8fd9 48ea 4860 1b40 0884  R0"..q..H.H`.@..
-00005100: 0610 82b4 c980 b4c3 0644 6010 004d 2392  .........D`..M#.
-00005110: 1649 ef6f d246 5208 6c03 0881 9001 6929  .I.o.FR.l.....i)
-00005120: 1891 0b8e 386e 6e24 cf24 b00d 2004 4203  ....8nn$.$.. .B.
-00005130: 0801 dc64 40da 6103 2230 0880 c060 44ee  ...d@.a."0...`D.
-00005140: 55c6 0032 2029 0523 7201 1167 067d 2319  U..2 ).#r..g.}#.
-00005150: 2781 6d00 2110 1a40 08fa 2603 d20e 1b10  '.m.!..@..&.....
-00005160: 8141 00b8 067d 0303 d706 b802 c30d bb22  .A...}........."
-00005170: 80c1 2c43 1ca4 4130 5021 0625 a106 e212  ..,C..A0P!.%....
-00005180: 06e9 2724 cd58 2129 0923 42c2 885c 20c4  ..'$.X!).#B..\ .
-00005190: 19ab 23f9 2781 6d00 2110 3220 edb0 0111  ..#.'.m.!.2 ....
-000051a0: 1404 40c9 8850 3222 1708 718d ec48 9a4a  ..@..P2"..q..H.J
-000051b0: 601b 4008 8406 1082 dac9 80b4 c306 4460  `.@...........D`
-000051c0: 1000 4523 42d1 885c 20c4 55ba 23e9 2a81  ..E#B..\ .U.#.*.
-000051d0: 6d00 2110 1a40 086e 2703 d20e 1b10 8141  m.!..@.n'......A
-000051e0: 0094 8d08 6523 7281 10d7 898f a4ad 04b6  ....e#r.........
-000051f0: 0184 4068 0021 109f 0c48 3b6c 4004 0601  ..@h.!...H;l@...
-00005200: 5018 8c08 85c1 885c 20c4 9581 fa48 fa4a  P......\ ....H.J
-00005210: 601b 4008 8406 1082 f2c9 80b4 c306 4460  `.@...........D`
-00005220: 1000 a5c1 8850 1a8c c805 425c 1bc8 8fa4  .....P....B\....
-00005230: b904 b601 8440 6800 2100 9f0c 483b 6c40  .....@h.!...H;l@
-00005240: 0406 0150 1c8c 08c5 c188 5c20 c4d5 81fe  ...P......\ ....
-00005250: 48ba 4b60 1b40 0884 0610 82f3 c980 b4c3  H.K`.@..........
-00005260: 0644 6010 00e5 c188 501e 8cc8 0542 5c1f  .D`.....P....B\.
-00005270: 8890 a4bd 04b6 0184 4068 0021 709f 0c48  ........@h.!p..H
-00005280: 3b6c 4004 0601 a028 9c10 0c0c 37b0 4d00  ;l@....(....7.M.
-00005290: 06b3 0c74 a006 c140 8518 d060 50c9 d375  ...t...@...`P..u
-000052a0: 6e83 423a dc10 b010 18cc 32d0 011b 0499  n.B:......2.....
-000052b0: 43a2 6c23 0164 8803 a342 0e66 02b8 1c3a  C.l#.d...B.f...:
-000052c0: e48a 00ae 6564 06ae 8702 b921 8059 8236  ....ed.....!.Y.6
-000052d0: 18a8 1003 810d ae36 18a8 1003 870d a636  .......6.......6
-000052e0: 18a8 1003 380c d8e0 6983 1c48 4ac1 8824  ....8...i..HJ..$
-000052f0: 4152 0a46 e482 21da 4880 8c61 0322 1008  AR.F..!.H..a."..
-00005300: 008f 1e82 814b e208 6e49 2318 6ec8 9b01  .....K..nI#.n...
-00005310: 0c66 19e8 a00d 8281 0a31 30c5 6022 25ec  .f.......10.`"%.
-00005320: 4e27 8c74 b821 2823 3098 65a0 8337 0852  N'.t.!(#0.e..7.R
-00005330: 8e44 d946 42ce 1007 4785 dc10 c091 4dda  .D.FB...G.....M.
-00005340: c0d1 5120 3704 304b 0007 0315 6220 bcc1  ..Q 7.0K....b ..
-00005350: 0407 0315 62c0 8bc1 1b3c 7090 7843 d21c  ....b....<p.xC..
-00005360: 484a c188 d030 2217 08d1 4642 630c 1b10  HJ...0"...FBc...
-00005370: 8140 0078 cc11 0c5c e247 30dc e03a 0218  .@.x...\.G0..:..
-00005380: cc32 d001 1c04 0315 6200 8f81 a61e 6930  .2......b.....i0
-00005390: dc00 3b79 0406 b30c 7420 0741 1b09 6c23  ..;y....t .A..l#
-000053a0: 1c2b 0d72 7d13 c02c c11c 0c54 8881 2007  .+.r}..,...T.. .
-000053b0: d31c 0c54 8801 3f06 72f0 cc41 da0d 4929  ...T..?.r..A..I)
-000053c0: 1891 2448 4ac1 885c 3044 1b09 8a31 6c40  ..$HJ..\0D...1l@
-000053d0: 0402 01e0 314a 3070 c92d c170 83ef 0860  ....1J0p.-.p...`
-000053e0: 30cb 4007 7310 641a 0536 d728 b023 0605  0.@.s.d..6.(.#..
-000053f0: 1082 60a0 076a 354e 2306 0510 8260 a007  ..`..j5N#....`..
-00005400: 6aa5 4b23 0646 0382 6050 0b62 954a c188  j.K#.F..`P.b.J..
-00005410: 81d1 8020 18d4 8258 a592 306c 40ac 111c  ... ...X..0l@...
-00005420: 11c0 b001 c146 6e44 0023 068d 0382 60b0  .....FnD.#....`.
-00005430: 0a6b c546 6bf4 3732 d53e a9c4 37ed 934a  .k.Fk.72.>..7..J
-00005440: c31c 4360 073f 5107 ab50 07d9 46dc cd36  ..C`.?Q..P..F..6
-00005450: 0a6c be51 6069 1091 1103 a301 4130 a805  .l.Q`i......A0..
-00005460: b372 2561 c4c0 6840 100c 6ac1 ac5c 6968  .r%a..h@..j..\ih
-00005470: 23c1 7650 2703 ee0e 1b10 c140 0023 0605  #.vP'......@.#..
-00005480: 1082 60a0 0771 653a c30d ae13 4b66 9081  ..`..qe:....Kf..
-00005490: 4810 7602 10c0 d991 2508 186e 909d 5a32  H.v.....%..n..Z2
-000054a0: 8359 06a6 08f2 8e02 9b79 14d8 cc23 ee52  .Y.......y...#.R
-000054b0: 2022 2306 4603 8260 500b 7195 4bc3 8881   "#.F..`P.q.K...
-000054c0: d180 2018 d442 5ce5 1231 4b70 8403 0123  .. ..B\..1Kp...#
-000054d0: 0500 0016 5ce0 2c52 e423 95df 10d7 84df  ....\.,R.#......
-000054e0: b501 0b28 7ecf f73e 25f9 9464 b503 d1e2  ...(~..>%..d....
-000054f0: 388f 8f34 0371 d5fd ee53 4d64 ca01 85df  8..4.q...SMd....
-00005500: df3e 62da 0153 0344 9163 ddb8 3f10 8c13  .>b..S.D.c..?...
-00005510: 1940 e323 27b1 154e e407 ce80 f94f 441c  .@.#'..N.....OD.
-00005520: 0430 1091 2f3d 0b32 f994 64d3 058d 5fe3  .0../=.2..d..._.
-00005530: 3ee2 5392 4f3c c862 d501 867f d3b7 8f18  >.S.O<.b........
-00005540: 7880 e1df 34ee d796 2f70 f83d 4ffb 9454  x...4.../p.=O..T
-00005550: a202 8f58 de2e cbcf 6517 5c5e 6ec1 d1e9  ...X....e.\^n...
-00005560: f3b8 0a27 f203 67c0 fc27 7216 ff89 8883  ...'..g..'r.....
-00005570: 0006 2232 dd81 4312 88ca 209e 93e9 0a27  .."2..C... ....'
-00005580: f203 67c0 7c4a b2f5 dc27 1e64 f19f 8838  ..g.|J...'.d...8
-00005590: 0860 2022 330e 287c 3ef7 1173 0fd0 884b  .` "3.(|>..s...K
-000055a0: 409a c2f1 6b5f 8a1c c0a7 7dda 7f0e 5f42  @...k_....}..._B
-000055b0: 1ac5 0c05 906b 8a00 6422 223b 0c68 80c8  .....k..d"";.h..
-000055c0: f081 2802 b0bf f669 430c 6880 c8f0 8128  ..(....iC.h....(
-000055d0: 02b0 bff6 6b4b 0c68 80c8 f081 2802 b0bf  ....kK.h....(...
-000055e0: f66d 530c 6880 c8f0 8128 02b0 bff6 6f5b  .mS.h....(....o[
-000055f0: 0c68 80c8 f081 2802 b0bf f671 2b14 281a  .h....(....q+.(.
-00005600: bf22 04eb 2558 fc1a f711 9f92 ec3d 37e9  ."..%X.......=7.
-00005610: 02c6 ef7b daa7 249f 7890 c5f6 0510 bfc6  ...{..$.x.......
-00005620: 7dc4 a724 1b1c 48fc bea7 7d4a f26b 831c  }..$..H...}J.k..
-00005630: 48fc bea7 7d4a f26d d31c 48fc bea7 7d4a  H...}J.m..H...}J
-00005640: f2ef 3b40 36da 470a 1f29 8c9c c059 a4c8  ..;@6.G..)...Y..
-00005650: 472a bf21 aee9 de7b cb0e 98fc baa7 6b5f  G*.!...{......k_
-00005660: 8a1c c0a7 fdda 7f0e 1f39 876d db69 9f68  .........9.m.i.h
-00005670: 06a4 f089 6640 0a9f 6806 a4f0 8966 400a  ....f@..h....f@.
-00005680: b30e 30fc 9bc6 7dc4 0207 12bf df7b 9f92  ..0...}......{..
-00005690: fcda 3007 12bf df7b 9f92 fcdb 8e03 0a9f  ..0....{........
-000056a0: d77d c420 031a 2032 7c20 8a00 ecb7 7dda  .}. .. 2| ....}.
-000056b0: 2203 1a20 327c 208a 00ec b7fd da24 031a  ".. 2| ......$..
-000056c0: 2032 7c20 8a00 ecb7 7ddb 2603 1a20 327c   2| ....}.&.. 2|
-000056d0: 208a 00ec b7fd db28 031a 2032 7c20 8a00   ......(.. 2| ..
-000056e0: ecb7 7dfc 4692 8a10 2627 f29f e352 9cc2  ..}.F...&'...R..
-000056f0: 89fc c019 309f 926c 3db7 f202 6791 221f  ....0..l=...g.".
-00005700: a9fc 86b8 a6bb a7cd bcc0 59a4 c847 2abf  ..........Y..G*.
-00005710: 21ae e9ee 6fa3 2f70 1629 f291 ca6f 886b  !...o./p.)...o.k
-00005720: bafb dc44 079c 458a 7ca4 f21b e29a ee7e  ...D..E.|......~
-00005730: bf92 a522 84c9 89fc c019 301b 2768 fc9a  ..."......0.'h..
-00005740: ae7b 9f92 ec7d f7ef 7bd1 0a27 f203 67c0  .{...}..{..'..g.
-00005750: 7c4a f289 0759 fc27 220e 0218 88c8 8403  |J...Y.'".......
-00005760: 0a7f e77d e434 b0c2 89fc c019 309f 926c  ...}.4......0..l
-00005770: 3df7 9f88 3808 6020 2213 2f78 fcbe a77d  =...8.` "./x...}
-00005780: 4ab2 77dc 271e 6431 4d81 c3ef f9de ee7b  J.w.'.d1M......{
-00005790: d317 38fc bea7 7d4a b2d3 0168 719c c747  ..8...}J...hq..G
-000057a0: 9a81 b8ea 7ef7 9fc3 8e0b 1449 202a 8378  ....~......I *.x
-000057b0: 705a 37ea 0245 1288 ca20 1e9c eead 3ee0  pZ7..E... ....>.
-000057c0: f0f3 9db7 73db 3005 0abf ae6b db32 050a  ....s.0....k.2..
-000057d0: bfae 6bdc f603 16e9 2104 5f22 1642 986c  ..k.....!._".B.l
-000057e0: 9740 f17b bef7 29c9 de6f 231e 6004 a729  .@.{..)..o#.`..)
-000057f0: 1644 98fc 68b8 6c38 a0f0 f7de 470c 7640  .D..h.l8....G.v@
-00005800: f16b dc47 fc27 7216 630c 7880 c8f0 8128  .k.G.'r.c.x....(
-00005810: 02b0 bff6 739f b6c6 8007 880c 1f88 2200  ....s.........".
-00005820: fb6b 3ff7 6bcb 2d78 fc7e ef7d 4af2 29c9  .k?.k.-x.~.}J.).
-00005830: 271e 6431 de81 8332 16cc 201e 432d 38fc  '.d1...2.. .C-8.
-00005840: 9aae 7b7f 3f85 64cb 719f 6806 a430 d702  ..{.?.d.q.h..0..
-00005850: 4512 88ca 201e dcc6 cdb7 4091 04a2 3288  E... .....@...2.
-00005860: 07b7 7713 2e80 8807 597c 6422 a2db ce7d  ..w.....Y|d"...}
-00005870: 8179 8c3f 80f0 9f88 b0df 8085 b804 a429  .y.?...........)
-00005880: 1cbf f611 eb1d 1002 c12c 0998 0699 88c8  .........,......
-00005890: 6f24 2af0 eb6b 990a 27f2 0367 c07c 4af2  o$*..k..'..g.|J.
-000058a0: 29c9 271e 64b1 de02 c8af 711f f129 c9a7  ).'.d.....q..)..
-000058b0: 249f 7890 c51c 031e 2032 7c20 8a00 ecaf  $.x..... 2| ....
-000058c0: 7ddd a7ed 31e0 0122 c307 a208 c0fe dad7  }...1.."........
-000058d0: fdfa 188c edd6 7da4 b7d8 0145 1288 ca20  ......}....E... 
-000058e0: 9e5b afad 5760 5a1c e7f1 9166 20ae badf  .[..W`Z....f ...
-000058f0: 7d4a f229 c9e0 090c bfe7 69bf 367c 02c3  }J.)......i.6|..
-00005900: ef79 dab7 af80 d970 de5f 1ce7 212e 64ba  .y.....p._..!.d.
-00005910: 8467 cb71 9f68 06a4 f097 c87f 8e03 2888  .g.q.h........(.
-00005920: 668a 3003 2c30 fc9e a7fd db10 0b0c bfe7  f.0.,0..........
-00005930: 691f 37d0 02c3 ef79 dadf 0db3 c0f0 7b9e  i.7....y......{.
-00005940: f675 832c 30fc 9ea7 fddc 5805 083f f711  .u.,0.....X..?..
-00005950: fb15 50fc 9ea7 7d4a f229 c982 0792 c0a1  ..P...}J.)......
-00005960: 9a81 be69 dbf0 0310 bfde 731f a969 8b17  ...i......s..i..
-00005970: 68fc 9aae 7b9f 927c 4af2 6ff3 0d28 fcbb  h...{..|J.o..(..
-00005980: f611 5b27 28fc 1af7 11db 1d50 2481 a80c  ..['(......P$...
-00005990: e2b1 fbdd 8607 a2c2 a19a c117 9ca6 5810  ..............X.
-000059a0: 61ba 69dc ec05 a0c5 711e 1f69 06e2 aafb  a.i.....q..i....
-000059b0: dda7 24ab 0c78 80c8 f081 2802 b0df f673  ..$..x....(....s
-000059c0: 9f36 cb80 0788 0c1f 8822 00fb 6d3f f76b  .6......."..m?.k
-000059d0: 931d 50fc 9aae 7bff 899c c588 0918 bfe7  ..P...{.........
-000059e0: 7b9f 92ec fdf6 6bdb 2660 fc9e ef7d 4ab2  {.....k.&`...}J.
-000059f0: f7db bf4d b5e0 5a1c e7f1 9166 20ae badf  ...M..Z....f ...
-00005a00: 7d4a f229 c9a7 9ac8 b40b 1449 202a 8378  }J.).......I *.x
-00005a10: 6e9e b7f5 002d 22a6 678a fc88 7800 41b1  n....-".g...x.A.
-00005a20: e9dd 8f88 0710 14bb be8d 7da0 409a 81b8  ..........}.@...
-00005a30: 4c3e 20f1 6f1a f76b 5ba7 ed92 8069 9089  L> .o..k[....i..
-00005a40: 88fc 4660 1ebf b6fb 00c3 b777 da47 0c52  ..F`.......w.G.R
-00005a50: 20f1 6f1a f76b 5bb7 0dbc e0f1 7b9e f629   .o..k[.....{..)
-00005a60: c9d6 7b9f 7890 c5d4 03ae 8898 9e29 f223  ..{.x........).#
-00005a70: e201 04c5 a677 3f22 1e40 504c 9880 f17b  .....w?".@PL...{
-00005a80: 9ef6 29c9 d67b bf36 6602 c6ef 79da a724  ..)..{.6f...y..$
-00005a90: 5bef 7ddb b209 18bf e769 9f92 6cbd f76f  [.}......i..l..o
-00005aa0: 232f 5024 81a8 0ce2 b9fb dabc 0308 ffd6  #/P$............
-00005ab0: 7392 89d5 9646 46c6 56e6 22c6 f636 b6e6  s....FF.V."..6..
-00005ac0: 52e7 26d7 c236 3637 1766 f104 86df f7b4  R.&..667.f......
-00005ad0: 5f1b 7400 d200 51e4 583e 6281 0586 dff7  _.t...Q.X>b.....
-00005ae0: b47f 5b62 81e1 f73d ede3 964f 60f8 7d4f  ..[b...=...O`.}O
-00005af0: fbb6 4516 187e dfd3 7e6e a105 86df f7b4  ..E..~..~n......
-00005b00: bf5b 6681 e1f7 3ded eb24 97ce ec4d cea5  .[f...=..$...M..
-00005b10: cc8d cc85 eded 0dae 0c2f 8d6e 0606 c7a5  ........./.n....
-00005b20: ce4d ae85 6d6c 6e2e cc2e 031e 2032 7c20  .M..mln..... 2| 
-00005b30: 8a00 ecb7 7ddd a70d 33e0 0122 c307 a208  ....}...3.."....
-00005b40: c07e dbd7 fdda b003 26bf eee9 da97 2207  .~......&.....".
-00005b50: f075 bff6 9fc3 47ec bda0 f0eb 9ab7 4d78  .u....G.......Mx
-00005b60: 2009 1caa 19ea 9bbe 2db5 4021 2e64 129c   .......-.@!.d..
-00005b70: 66f0 77b3 0f48 fc9c e6fd dace 6f1b 1548  f.w..H......o..H
-00005b80: fc9c e6fd dace 7573 2e48 1629 f291 0aa7  ......us.H.)....
-00005b90: 77fb 0e20 fc7b c7ad b920 59a4 c847 2abc  w.. .{... Y..G*.
-00005ba0: a68d 5720 59a4 c847 2abc b66d 5720 59a4  ..W Y..G*..mW Y.
-00005bb0: c847 2abc c62d 3a40 f2eb 9eae 7d29 7200  .G*..-:@....})r.
-00005bc0: 9ff6 e95b f711 3b0f 8022 627a a6c8 8f88  ...[..;.."bz....
-00005bd0: 0710 149b ae0d 3d00 8a88 e999 223f 221e  ......=....."?".
-00005be0: 4050 6cfa 36fa 0047 7a08 c197 8885 1026  @Pl.6..Gz......&
-00005bf0: 1bef 2d3d 008a 88e9 9922 3f22 1e40 506c  ..-=....."?".@Pl
-00005c00: 3a37 7382 6671 9cc7 479a 81b8 ea7e b762  :7s.fq..G....~.b
-00005c10: 02c6 ef7b daa7 247b c7fd daa4 0918 bfef  ...{..${........
-00005c20: 699f 92ec 1df7 6de3 2660 fcbe a77d 4ab2  i.....m.&`...}J.
-00005c30: 77dc bfef 04aa 0861 7222 3f70 06cc 271e  w......ar"?p..'.
-00005c40: 6439 9aa3 7022 9f68 861b a8b6 dbf6 8966  d9..p".h.......f
-00005c50: 400a 1ff1 9f88 3808 6020 22c3 2598 16c7  @.....8.` ".%...
-00005c60: 797c a419 88ab ee77 9f92 6c5d 37dc 8264  y|.....w..l]7..d
-00005c70: 9122 1fa9 703b b7db 8264 9122 1fa9 709b  ."..p;...d."..p.
-00005c80: 3763 82c6 af71 1ff1 29c9 de73 bfb6 6982  7c...q..)..s..i.
-00005c90: c6af 711f f129 c9de 73df b66e 82c6 af71  ..q..)..s..n...q
-00005ca0: 1ff1 29c9 de73 ffb6 fe80 477a 08c1 9788  ..)..s....Gz....
-00005cb0: 8510 269f a12e d325 50fc 9ea7 7d4a b2f5  ..&....%P...}J..
-00005cc0: dee4 090e bfc6 7dc4 af4d 9fe0 f06b dc47  ......}..M...k.G
-00005cd0: 7cdb 040b 0ebf c67d c4bf 4db1 e0f0 6bdc  |......}..M...k.
-00005ce0: 477c dc24 0b0e bfc6 7dc4 cf4d b3e0 f06b  G|.$....}..M...k
-00005cf0: dc47 7cdd 440b 0ebf c67d c4df 4db7 e0f1  .G|.D....}..M...
-00005d00: 7b9e f629 c9a7 249f 7890 c56c 0b92 458a  {..)..$.x..l..E.
-00005d10: 7ca4 c26f da5c 0712 bfe7 69ff 899c c5a4  |..o.\....i.....
-00005d20: 0324 bfee e9da 9722 07f0 759f be73 1f31  .$....."..u..s.1
-00005d30: 6401 c6ef f7de a724 9f92 fcda cc05 18bf  d......$........
-00005d40: df7b 9f92 7c4a f2ef fb68 0a27 f203 67c0  .{..|J...h.'..g.
-00005d50: fc27 7296 9b99 0a27 f203 67c0 7c4a b2f5  .'r....'..g.|J..
-00005d60: dc27 1e64 b1e5 00c3 cf7d c447 2cbe 80f0  .'.d.....}.G,...
-00005d70: 73bd 37ec 826b 719c c747 9a81 b8ea 7ef7  s.7..kq..G....~.
-00005d80: 29c9 d675 9f6a 224b 1660 fc9e a77d 4af2  )..u.j"K.`...}J.
-00005d90: 29c9 af0d 5b80 f17b 9ef6 29c9 a724 dfb6  )...[..{..)..$..
-00005da0: 6001 c5ef 7bda a724 9f92 ec5c 80f1 7b9e  `...{..$...\..{.
-00005db0: f629 c9a7 24ff b6d5 81e4 899c c547 2622  .)..$........G&"
-00005dc0: b2f6 81a2 4126 22b2 f902 c3cf 69de af4f  ....A&".....i..O
-00005dd0: 400c 36da 279a 0129 7ca2 1990 c227 9a01  @.6.'..)|....'..
-00005de0: 297c a219 90c2 279a 0129 7cc4 dc09 1689  )|....'..)|.....
-00005df0: 6a14 6018 a29c a66d 9e60 91a8 4601 8621  j.`....m.`..F..!
-00005e00: cae9 daea 0916 896a 1460 18a2 9cb6 cd9e  .......j.`......
-00005e10: 6091 a846 0186 21ca e9db f609 1689 6a14  `..F..!.......j.
-00005e20: 6018 a29c c6ad 9f60 91a8 4601 8621 cae9  `......`..F..!..
-00005e30: dcfc 0916 896a 1460 18a2 9cd6 6db0 6091  .....j.`....m.`.
-00005e40: a846 0186 21ca e9dd 0a0b 1689 6a14 6018  .F..!.......j.`.
-00005e50: a29c e6cd b060 91a8 4601 8621 cae9 deca  .....`..F..!....
-00005e60: 099e 0699 88e8 ae79 bf11 98c7 bf4d be80  .......y.....M..
-00005e70: f0f3 9db7 5b82 6491 221f a9ee 9db7 4a02  ....[.d.".....J.
-00005e80: 0669 06e2 f21b e29a fcda 160b 1689 6a14  .i............j.
-00005e90: 6018 a2bc a6ad b160 91a8 4601 8621 caeb  `......`..F..!..
-00005ea0: da1c 0b16 896a 1460 18a2 bcb6 ad58 6091  .....j.`.....X`.
-00005eb0: a846 0186 21c2 6fdb 9c05 1689 6a14 6018  .F..!.o.....j.`.
-00005ec0: 22fc be0d 5a60 91a8 4601 8621 c26f dca2  "...Z`..F..!.o..
-00005ed0: 0516 896a 1460 1822 fcce 6d5a 6091 a846  ...j.`."..mZ`..F
-00005ee0: 0186 21c2 6fdd a805 1689 6a14 6018 22fc  ..!.o.....j.`.".
-00005ef0: decd 5a60 91a8 4601 8621 c26f deb2 0516  ..Z`..F..!.o....
-00005f00: 896a 1460 1822 fcee cdb2 6091 a846 0186  .j.`."....`..F..
-00005f10: 21ca ebdc 360b 1689 6a14 6018 a2bc d68d  !...6...j.`.....
-00005f20: 7040 f16b dc47 7c4a f26b 8b1c 50fc 1af7  p@.k.G|J.k..P...
-00005f30: 119f 927c db0a 038c 8898 9e29 b2ed 00c3  ...|.......)....
-00005f40: c771 dc47 acb3 6091 a846 0186 21ca ebdd  .q.G..`..F..!...
-00005f50: 3607 14bf c67d c4a7 24ff b6ca 8245 a21a  6....}..$....E..
-00005f60: 0518 8628 af71 db2d 78fc 9eef 7d4a f229  ...(.q.-x...}J.)
-00005f70: c927 1e64 3996 ae70 223f 7006 cca7 249f  .'.d9..p"?p...$.
-00005f80: 927c e241 16ff 8988 8300 0622 32cf 8245  .|.A......."2..E
-00005f90: a21a 0518 8628 af79 9b2c 5824 aa51 8061  .....(.y.,X$.Q.a
-00005fa0: 88f2 fa36 ef82 6491 221f a96e bebf 0566  ...6..d."..n...f
-00005fb0: bb75 1fe9 fd25 f29f c34a 0508 7fcf 6f33  .u...%...J....o3
-00005fc0: 1520 fc3d c76d 5280 f0f5 3d37 4a01 c2d7  . .=.mR...=7J...
-00005fd0: 77dd 2a05 085f df77 2b2d 5824 aa51 8061  w.*.._.w+-X$.Q.a
-00005fe0: 8872 9b36 6d81 45a2 1a05 1886 08c7 693b  .r.6m.E.......i;
-00005ff0: 1520 fc3d cf8d 5b60 91a8 4601 8621 c2f1  . .=..[`..F..!..
-00006000: dac4 0516 896a 1460 1822 1cbf 6d5c 6091  .....j.`."..m\`.
-00006010: a846 0186 21c2 71dc d805 1689 6a14 6018  .F..!.q.....j.`.
-00006020: 221c cfcd 5d60 91a8 4601 8621 c271 ddde  "...]`..F..!.q..
-00006030: 0516 896a 1460 1822 1cdf 8d5f 6091 a846  ...j.`."..._`..F
-00006040: 0186 21c2 71de fc05 1689 6a14 6018 221c  ..!.q.....j.`.".
-00006050: ef2d 5420 59a4 c847 aabb c76d b460 91a8  .-T Y..G...m.`..
-00006060: 4601 8621 caeb dec0 0516 896a 1460 1822  F..!.......j.`."
-00006070: 1cb7 ad5e 2059 a4c8 47aa bbd7 adbb 2059  ...^ Y..G..... Y
-00006080: a4c8 47aa bbb7 cdb4 6091 a846 0186 21ca  ..G.....`..F..!.
-00006090: edda ae0b 20e2 4116 1f99 88e8 b669 5f60  .... .A......i_`
-000060a0: 1ef3 0f20 fcde a60d 5080 f07b bbb6 ff00  ... ....P..{....
-000060b0: c2ef 6ddb 0a07 1689 6a14 6018 223c a7ed  ..m.....j.`."<..
-000060c0: 7060 91a8 4601 8621 c2f3 da10 0716 896a  p`..F..!.......j
-000060d0: 1460 1822 3cb7 4d71 6091 a846 0186 21c2  .`."<.Mq`..F..!.
-000060e0: f3db 1607 1689 6a14 6018 223c c7ad 7160  ......j.`."<..q`
-000060f0: 91a8 4601 8621 c2f3 dc24 0716 896a 1460  ..F..!...$...j.`
-00006100: 1822 3cd7 8d72 6091 a846 0186 21c2 f3dd  ."<..r`..F..!...
-00006110: 2a07 1689 6a14 6018 223c e78d 7360 91a8  *...j.`."<..s`..
-00006120: 4601 8621 c2f3 de86 0ba8 c571 1e1f 6906  F..!.......q..i.
-00006130: e2aa fbdd a724 9f6a 22cb 2f30 fc9b af7d  .....$.j"./0...}
-00006140: c49a 030e 5ff7 11db 47ac bee0 d96e dd47  ...._...G....n.G
-00006150: 7a7f 2222 4670 9ac1 ca03 a088 989e 29f2  z.""Fp........).
-00006160: 23e2 0104 a5ee 7b9b 0f40 fcbc ee7d a4a9  #.....{..@...}..
-00006170: 6c55 80f0 fb9b 3654 01c2 dff7 da68 079a  lU....6T.....h..
-00006180: 2772 161f 9988 c817 98c7 5205 087f df6f  'r........R....o
-00006190: b314 207c bdbf 0f06 2a9c c80f 9c01 f329  .. |....*......)
-000061a0: c927 1e64 3982 65bb 6d9f 6806 a4f0 11bb  .'.d9.e.m.h.....
-000061b0: 1420 7cbd cfcd 7360 91a8 4601 8621 c275  . |...s`..F..!.u
-000061c0: da3e 0716 896a 1460 1822 5caf cd7d 6091  .>...j.`."\..}`.
-000061d0: a846 0186 21c2 75db e007 1689 6a14 6018  .F..!.u.....j.`.
-000061e0: 225c bf4d 7e60 91a8 4601 8621 c275 fc32  "\.M~`..F..!.u.2
-000061f0: b0c2 89fc c019 30ff 8988 8300 0622 f2a5  ......0......"..
-00006200: 6741 267b 1d48 fcbe a7fd 2772 16ab 1f58  gA&{.H....'r...X
-00006210: 24aa 5180 6188 705d b747 0163 9122 1fa9  $.Q.a.p].G.c."..
-00006220: 4c7f 6091 a846 0186 21c2 f5de ee07 1689  L.`..F..!.......
-00006230: 6a14 6018 225c df8d 7e60 91a8 4601 8621  j.`."\..~`..F..!
-00006240: c2f5 dcf2 0716 896a 1460 1822 5ce7 0d51  .......j.`."\..Q
-00006250: 60b9 a608 4026 22ba ebdb 0c03 0ee2 1290  `...@&".........
-00006260: a670 2c51 60b9 a608 4026 22ba ebdc 0e05  .p,Q`...@&".....
-00006270: 16aa 899c 65f9 9189 8848 319d d99b 9c4b  ....e....H1....K
-00006280: 991b 990b dbdb 1b5c 195e 1add 0c4c 8e4b  .......\.^...L.K
-00006290: 9d9b 5c0b dbd8 dc5c 98a9 1714 febd fb88  ..\....\........
-000062a0: b90a 1cbe ee23 76ad db78 01e4 d7b8 8ff8  .....#v..x......
-000062b0: 9464 efb9 4f3c c862 a303 4f83 4c44 74db  .d..O<.b..O.LDt.
-000062c0: b7df 08cc e3df e63f b048 54a3 00c3 10e1  .......?.HT.....
-000062d0: 7b7d 01dc 46fb 4433 2085 4f34 0352 f844  {}..F.D3 .O4.R.D
-000062e0: 3320 854f 3403 52f8 88fd 0f2c 12d5 28c0  3 .O4.R....,..(.
-000062f0: 3044 f86e db20 c122 518d 020c 4384 efb8  0D.n. ."Q...C...
-00006300: 1112 2c12 d528 c030 44f8 9e5b 20c1 2251  ..,..(.0D..[ ."Q
-00006310: 8d02 0c43 84ef b719 122c 12d5 28c0 3044  ...C.....,..(.0D
-00006320: f8ae 1b22 c122 518d 020c 4384 efbb 2512  ..."."Q...C...%.
-00006330: 2c12 d528 c030 44f8 ce1b ffc0 2251 8d02  ,..(.0D....."Q..
-00006340: 0c43 84ef b485 173c 7ecf f73e 25d9 fbed  .C.....<~..>%...
-00006350: 130f b2d8 22c1 2251 8d02 0c43 84ef bdf1  ...."."Q...C....
-00006360: 1228 7edf d33e 25d9 3b7e 2a48 e144 7ee0  .(~..>%.;~*H.D~.
-00006370: 0c98 f90e 1881 4335 036d e201 d296 e33e  ......C5.m.....>
-00006380: d10c 48e1 4f44 c408 4e33 d8ef 8011 3854  ..H.OD..N3....8T
-00006390: 33d4 87c2 30c8 302c 841f 2c8e a018 7140  3...0.0,..,...q@
-000063a0: e1f3 b48f 987e c0e2 44be e034 838f d4b6  .....~..D..4....
-000063b0: 850e 287e 4dd7 bd4f 49fe 6d8d 048b 4435  ..(~M..OI.m...D5
-000063c0: 0a30 0c11 ced3 e648 b048 54a3 00c3 10e1  .0.....H.HT.....
-000063d0: 7c6d 9004 8b44 350a 300c 11ce db26 49b0  |m...D5.0....&I.
-000063e0: 4854 a300 c310 e1fc 6d93 048b 4435 0a30  HT......m...D5.0
-000063f0: 0c11 cee3 e64b b048 54a3 00c3 10e1 7c7e  .....K.HT.....|~
-00006400: 224f 4508 9313 f90c c108 0721 2806 4cb0  "OE........!(.L.
-00006410: 4854 a300 c310 e1bc 6ec7 048b 4435 0a30  HT......n...D5.0
-00006420: 0c11 ceef 964c b048 54a3 00c3 10e1 3c6f  .....L.HT.....<o
-00006430: ca04 8b44 350a 300c 11ce f7e6 5e60 f8f8  ...D5.0.....^`..
-00006440: 6efb 8841 1730 7ebf f73e 25f9 c483 2c86  n..A.0~..>%...,.
-00006450: 2f70 f8fd defb 9464 9b02 0a65 2c98 413c  /p.....d...e,.A<
-00006460: 374d 5bb3 40e3 d7b8 8ff8 94e4 5392 5fdb  7M[.@.......S._.
-00006470: b740 e3d7 b88f f894 e453 926f df44 5538  .@.......S.o.DU8
-00006480: 911f 3803 e653 92ff 44c4 4100 0311 d9ba  ..8..S..D.A.....
-00006490: 40e3 d7b8 8ff8 94e4 5392 7f5b 33c1 2251  @.......S..[3."Q
-000064a0: 8d02 0c43 84f7 b439 132c 12d5 28c0 3044  ...C...9.,..(.0D
-000064b0: 785f 1b34 c122 518d 020c 4384 f7b6 5113  x_.4."Q...C...Q.
-000064c0: 2c12 d528 c030 4478 7f1f 42b2 ddb8 4f34  ,..(.0Dx..B...O4
-000064d0: 0352 d835 c122 518d 020c 4384 f7f9 7554  .R.5."Q...C...uT
-000064e0: 8513 f981 3360 fe13 1107 010c 4474 d7b4  ....3`......Dt..
-000064f0: 7913 2c12 d528 c030 4478 af1b 38c1 2251  y.,..(.0Dx..8."Q
-00006500: 8d02 0c43 84f7 bbc5 0720 fe5d e73e d254  ...C..... .].>.T
-00006510: e62b a0f8 fdde fb94 e453 9271 0718 3e8e  .+.......S.q..>.
-00006520: ef3e 62e9 028c dff3 bd4f 493e 25f9 b72d  .>b......OI>%..-
-00006530: 0b30 7ecf f73e 25f9 94e4 d766 4db0 4854  .0~..>%....fM.HT
-00006540: a300 c310 e13d 6eec 048b 4435 0a30 0c11  .....=n...D5.0..
-00006550: def7 164e b048 54a3 00c3 10e1 3d6f d105  ...N.HT.....=o..
-00006560: 8cdf f3b4 4f49 3ef1 20cb 5560 8513 f981  ....OI>. .U`....
-00006570: 3360 3e25 f994 e43f 1171 10c0 4044 a415  3`>%...?.q..@D..
-00006580: cdec 4dce a5cc 8dcc 85ed ed0d ae0c 2f8d  ..M.........../.
-00006590: cea5 ce4d ae85 6d6c 6e2e ec30 96c2 89fc  ...M..mln..0....
-000065a0: c019 309f 928c 5980 f1fb 9ef6 29c9 a724  ..0...Y.....)..$
-000065b0: bf36 6f01 c6ef 7bda a724 9f92 7cdb d405  .6o...{..$..|...
-000065c0: 18bf ef69 9f92 7c4a f26f c324 4890 6620  ...i..|J.o.$H.f 
-000065d0: 2e9f 6a22 a317 781a 6422 a2db e6fd 4660  ..j"..x.d"....F`
-000065e0: 1eff be08 a970 223f 7006 cc7f 22e2 2080  .....p"?p...". .
-000065f0: 8188 ae01 db76 da27 9a01 297c a219 90c2  .....v.'..)|....
-00006600: 279a 0129 7ca4 30f6 802b 22a6 678a fc88  '..)|.0..+".g...
-00006610: 7800 41b1 e9de 8f88 0710 144b 2720 fc9e  x.A........K' ..
-00006620: a7ef c1db 76da 279a 0129 7ca2 1990 c227  ....v.'..)|....'
-00006630: 9a01 297c a219 90c2 478a 0ba9 0a27 f203  ..)|....G....'..
-00006640: 67c0 fc27 220e 0218 88e8 be73 eb0e 307c  g..'"......s..0|
-00006650: 1ce7 7dc4 9003 0a9f b77d e428 b0c2 89fc  ..}......}.(....
-00006660: c019 309f 92fc 2722 0e02 1888 e8be 6d53  ..0...'"......mS
-00006670: 2720 fcbe a78d b7e0 f1fb 9ef6 29c9 a724  ' ..........)..$
-00006680: 9f78 90c5 8405 16bf c67d c4a7 249f 920c  .x.......}..$...
-00006690: 78c0 291c aa19 7cc1 698a 0511 2613 1c48  x.)...|.i...&..H
-000066a0: fc9e a77d 4af2 6b9b 0e30 7cbb cf7d c49c  ...}J.k..0|..}..
-000066b0: 030c bfee 771f b1cc 81c4 ef79 daa7 24ff  ....w......y..$.
-000066c0: b6c7 81c4 ef79 daa7 24df 3e10 ab70 223f  .....y..$.>..p"?
-000066d0: 7006 cc7f 2267 f117 c779 880b 99ec 3ae0  p..."g...y....:.
-000066e0: 911e 42f0 2562 2184 e9b6 7dc4 9e03 0cdf  ..B.%b!...}.....
-000066f0: a66f 1fb1 fc00 c4b7 e9da 47ea daaa 0b9c  .o........G.....
-00006700: 458a 7ca4 f21b e29a 709a 37d5 0169 719c  E.|.....p.7..iq.
-00006710: c747 9a81 b8ea 7ef7 9fc8 5948 3623 f1a5  .G....~...YH6#..
-00006720: e554 e356 d726 1626 e306 67c3 96e6 16c6  .T.V.&.&..g.....
-00006730: 7616 43f3 7556 46f7 e5f6 26d7 f695 d606  v.C.uVF...&.....
-00006740: c716 2343 3233 c6f6 3616 c636 4732 5316  ..#C23..6..6G2S.
-00006750: 43f3 e656 46f4 95d6 06c7 4622 4323 7353  C..VF.....F"C#sS
-00006760: 5413 2427 1796 9744 c694 1653 1433 74d3  T.$'...D...S.3t.
-00006770: 5647 1726 c656 7613 c696 76e6 5646 5624  VG.&.Vv...v.VFV$
-00006780: 73f3 d696 4647 5746 4622 8343 5666 1656  s...FGWFF".CVf.V
-00006790: c746 4732 43e6 f4e6 5646 2293 e352 8697  .FG2C...VF"..R..
-000067a0: 4667 c501 85cf df3e 62b3 03cd 1339 8b8f  Fg.....>b....9..
-000067b0: 4c44 e44b 5460 d605 ce22 453e 52f9 0d71  LD.KT`..."E>R..q
-000067c0: 4d78 5d9f c556 3891 1f38 03e6 5392 4f49  Mx]..V8..8..S.OI
-000067d0: fe13 1107 010c 4474 dfb4 c90b 388b 14f9  ......Dt....8...
-000067e0: 48e5 37c4 35e1 f56d f302 ce22 453e 52f9  H.7.5..m..."E>R.
-000067f0: 0d71 4d78 9d1b 7580 e1db bdee 23b7 b115  .qMx..u.....#...
-00006800: 4ee4 07ce 80f9 9464 ebb9 ff44 c441 0003  N......d...D.A..
-00006810: 11dd 377e 174e e144 7ee0 0c98 4f49 3e25  ..7~.N.D~...OI>%
-00006820: d97b 40c1 1091 411c 4953 11c2 e444 fe73  .{@...A.IS...D.s
-00006830: f80d 61d9 7941 433c c8e2 2313 11f9 02f3  ..a.yAC<..#.....
-00006840: d8b0 0022 518d 020c 4374 1c55 e144 7ee0  ..."Q...Ct.U.D~.
-00006850: 0c98 ff44 c441 0003 11d9 fd6d bf05 ce22  ...D.A.....m..."
-00006860: 453e 52f9 0d71 4db8 ad9b a280 4335 91b3  E>R..qM.....C5..
-00006870: 2c3f 3211 d15d ef16 1eb0 2c52 e423 95df  ,?2..]....,R.#..
-00006880: 10d7 7410 61b0 edb4 4f34 0352 f844 3320  ..t.a...O4.R.D3 
-00006890: 854f 3403 52f8 4433 2085 4f34 0352 1870  .O4.R.D3 .O4.R.p
-000068a0: 81b3 4891 8f54 7e43 5c13 6ef7 961c 50f8  ..H..T~C\.n...P.
-000068b0: 3cee 23a4 1a95 f8d2 72aa 71ab 6b13 0b93  <.#.....r.q.k...
-000068c0: 7183 b361 4b73 0b63 3b8b a1f9 3a2b a3fb  q..aKs.c;...:+..
-000068d0: 727b 936b fb4a 6b83 638b 9121 9919 637b  r{.k.Jk.c..!..c{
-000068e0: 1b0b 639b 2399 298b a179 732b 23fa 4a6b  ..c.#.)..ys+#.Jk
-000068f0: 8363 2391 a191 b929 aa09 9293 0bcb 4b22  .c#....)......K"
-00006900: 634a 8b29 8a19 ba69 aba3 0b13 632b bb09  cJ.)...i....c+..
-00006910: 634b 3b73 2b23 2b92 b979 6b4b a3a3 2b23  cK;s+#+..ykK..+#
-00006920: 2391 c121 2b33 0bab 63a3 2399 2173 7a73  #..!+3..c.#.!szs
-00006930: 2b23 91c9 7129 c34b a373 a143 932b 0b23  +#..q).K.s.C.+.#
-00006940: 3b03 62ab 6bda da03 b488 989e 29f2 23e2  ;.b.k.......).#.
-00006950: 0104 c5a6 7b3f 221e 4050 ecba 0600 0001  ....{?".@P......
-00006960: 3100 003f 0000 005b 0643 1083 2d43 2314  1..?...[.C..-C#.
-00006970: 5b06 0819 832d c384 8cc1 96e1 128a 2d03  [....-........-.
-00006980: 1808 64b0 6508 0381 0cb6 0c66 808c c196  ..d.e......f....
-00006990: e10c 0432 d832 a482 676c 1956 c233 b60c  ...2.2..gl.V.3..
-000069a0: 2c21 145b 0697 f08c 2d83 9c48 d596 4155  ,!.[....-..H..AU
-000069b0: 0e33 d832 bcca 7106 5b06 5e39 cc60 cb10  .3.2..q.[.^9.`..
-000069c0: 2ec7 196c 29ea e540 0324 0db6 14fb 72a0  ...l)..@.$....r.
-000069d0: 0192 065b 8a90 39d0 0049 832d c5c9 1c68  ...[..9..I.-...h
-000069e0: 80a4 c196 a265 0e34 40d2 604b 3133 071a  .....e.4@.`K13..
-000069f0: 2069 b0a5 c899 030d 9034 d852 fccc 8106   i.......4.R....
-00006a00: 481a 6c19 c646 d2b6 0c69 7398 c196 c16d  H.l..F...is....m
-00006a10: 8e33 d852 f4cd 8106 481a 6c29 40e7 4003  .3.R....H.l)@.@.
-00006a20: 240d b614 a373 a001 9206 5b0a d339 d000  $....s....[..9..
-00006a30: 4983 2d83 2a49 db96 e19c 246e cb00 5252  I.-.*I....$n..RR
-00006a40: b765 a029 c9db 32ec 14b2 065b 069e 42d6  .e.)..2....[..B.
-00006a50: 60cb d053 c81a 6c19 c40a 5983 2d83 5c21  `..S..l...Y.-.\!
-00006a60: 6b00 0000 0000 0061 2000 002f 0200 0013  k......a ../....
-00006a70: 0454 2c10 0000 0018 0000 0004 1801 a041  .T,............A
-00006a80: 1514 411d d400 8946 000a 32a0 200a 6a06  ..A....F..2. .j.
-00006a90: a060 8aa0 800a ace0 0a30 8056 2300 1418  .`.......0.V#...
-00006aa0: ea80 a245 0c5a 420c 5a62 0660 a883 690e  ...E.ZB.Zb.`..i.
-00006ab0: 3168 0931 6889 a10e e749 c4a0 25c4 a025  1h.1h....I..%..%
-00006ac0: 863a a4a9 1183 9610 8396 18ea a02a 480c  .:...........*H.
-00006ad0: 5a42 0c5a 820a 2300 0000 0033 11c1 500b  ZB.Z..#....3..P.
-00006ae0: a430 1311 0cb5 400a 2306 ca03 8260 3007  .0....@.#....`0.
-00006af0: f3c0 1dcf 2304 c30d 012e 80c1 4c84 190c  ....#.......L...
-00006b00: b540 0a33 1166 30d4 0229 a410 d811 0304  .@.3.f0..)......
-00006b10: 0241 3098 0571 08be ec99 8930 83a1 1648  .A0..q.....0...H
-00006b20: 2187 c08e 1820 1008 82c1 2c90 4310 065b  !.... ....,.C..[
-00006b30: 3413 510c b540 0a39 0476 c400 8140 100c  4.Q..@.9.v...@..
-00006b40: 66c1 1c82 31e8 a661 0342 6008 6026 c20c  f...1..a.B`.`&..
-00006b50: 865a 2085 0c02 3b62 8040 2008 06b3 800e  .Z ...;b.@ .....
-00006b60: 4119 7cd5 2c43 2028 5b0b d416 0132 dc10  A.|.,C ([....2..
-00006b70: d802 18cc 320c 4430 6260 4420 0806 76f0  ....2.D0b`D ..v.
-00006b80: 0f67 31ed 2dd0 1320 c904 369b c08e 1820  .g1.-.. ..6.... 
-00006b90: 1008 82c1 2cb4 43a0 0664 a08d 1818 0d08  ....,.C..d......
-00006ba0: 8201 1e84 c420 e413 d80e 1002 31c8 80bb  ..... ......1...
-00006bb0: 1488 c870 4380 0661 30dc 60b4 4318 5c20  ...pC..a0.`.C.\ 
-00006bc0: ec2c 4361 0423 0646 0482 6060 072a 0117  .,Ca.#.F..``.*..
-00006bd0: 6130 4b10 a425 580a 0224 b1c0 7680 10a4  a0K..%X..$..v...
-00006be0: 4106 dba5 8044 920b 6c07 0841 1c64 c05d  A....D..l..A.d.]
-00006bf0: 0a44 24c1 20b0 1d20 0470 9001 7729 1091  .D$. .. .p..w)..
-00006c00: 2483 c076 8010 cc41 06dc a540 4412 0d02  $..v...A...@D...
-00006c10: db01 4260 0719 7097 0211 a137 0890 6483  ..B`..p....7..d.
-00006c20: c066 1b04 76c4 0081 4010 0c66 c125 8255  .f..v...@..f.%.U
-00006c30: 2885 3d18 3130 1a10 0403 3c10 8b41 c837  (.=.10....<..A.7
-00006c40: 086c 0708 c128 64c0 5d0a 4464 b821 4885  .l...(d.].Dd.!H.
-00006c50: 3018 6e30 5c22 0c2e 1076 96e1 4082 1103  0.n0\"...v..@...
-00006c60: 2302 4130 b083 b588 0d51 1831 2800 1004  #.A0.....Q.1(...
-00006c70: 033d d809 3098 2508 920e 049b 7720 580a  .=..0.%.....w X.
-00006c80: 0224 f320 b01d 2004 ab90 c176 2920 91ec  .$. .. ....v) ..
-00006c90: 83c0 7680 10cc 4206 dca5 4044 3214 02db  ..v...B...@D2...
-00006ca0: 0142 200b 1970 9702 11c9 5208 6c07 0841  .B ..p....R.l..A
-00006cb0: 2d64 c05d 0a44 2453 21b0 1d20 04b8 9001  -d.].D$S!.. ....
-00006cc0: 7729 1091 5c85 c08e 1820 1008 82c1 2cb8  w)..\.... ....,.
-00006cd0: 45b0 0ee5 b00b 2306 9804 8260 9006 a8c1  E.....#....`....
-00006ce0: 0aaa 8007 b920 0ee2 4007 70c0 0668 4006  ..... ..@.p..h@.
-00006cf0: 562e 8883 3848 8e62 08b4 0a05 425a 80e4  V...8H.b....BZ..
-00006d00: 2b04 b603 8400 1d32 082f 0560 92b3 10d8  +......2./.`....
-00006d10: 0e10 8275 c820 bc14 80c9 8841 0180 2018  ...u. .....A.. .
-00006d20: e881 5f8c c288 4101 8020 18e8 815f 84c1  .._...A.. ..._..
-00006d30: 30c7 b024 29a1 acc2 32dc b0cc 8519 cc32  0..$)...2......2
-00006d40: 3c50 3062 5044 2008 067a d01a f3b1 f3d1  <P0bPD ..z......
-00006d50: 0082 2cb4 4306 82a5 2040 861b 02b5 0083  ..,.C... @......
-00006d60: 5986 8609 460c 8c08 04c1 800f 6043 b087  Y...F.......`C..
-00006d70: 5902 67c4 c088 4010 0cec 8036 f8e3 1c66  Y.g...@....6...f
-00006d80: 099c 818a 4060 70a5 495d 10ec b001 1144  ....@`p.I].....D
-00006d90: 0490 bb10 d80e 1002 7cc8 20bc c306 4400  ........|. ...D.
-00006da0: 1140 fa42 603b 4008 f421 83f0 0e1b 10c1  .@.B`;@..!......
-00006db0: 4300 190e 811d 3140 2210 0403 3fc8 8d60  C.....1@"...?..`
-00006dc0: 24f0 2219 3128 0010 0403 3d70 8d6c 8311  $.".1(....=p.l..
-00006dd0: 0302 0041 3000 85dc 208d 4046 1302 6034  ...A0... .@F..`4
-00006de0: 4108 4613 0661 c4e0 0040 100c 4481 3706  A.F..a...@..D.7.
-00006df0: 2118 6e08 f602 0c66 1982 2818 e618 c260  !.n....f..(....`
-00006e00: 5a09 8925 8211 8322 0241 30d0 83de 1066  Z..%...".A0....f
-00006e10: 0982 1183 2202 4130 d003 de30 9159 8260  ....".A0...0.Y.`
-00006e20: c4c0 8840 100c ec80 3c4a c41e 6609 8270  ...@....<J..f..p
-00006e30: 2000 0034 0100 00f6 1be0 f8f7 ee17 02e0   ..4............
-00006e40: e3fe e200 839d 0728 12d5 28c0 3044 b67d  .......(..(.0D.}
-00006e50: 061d d14c 11e6 13cd 8014 3ed1 0c48 e113  ...L......>..H..
-00006e60: cd80 143e d10c 4861 ef01 8a44 350a 300c  ...>..Ha...D5.0.
-00006e70: 918d 5b7a 00e4 ebb6 5f08 809f fbb5 bf38  ..[z...._......8
-00006e80: c060 fb01 8a44 350a 300c 91ad 9fc0 4234  .`...D5.0.....B4
-00006e90: 5384 f944 3320 85ad 0728 12d5 28c0 3044  S..D3 ...(..(.0D
-00006ea0: f66d f501 8edf df7e 2100 3eed 2f0e 30d8  .m.....~!.>./.0.
-00006eb0: 7d80 2251 8d02 0c43 64e7 1628 40f8 b5cd  }."Q...Cd..(@...
-00006ec0: db7f 8022 518d 020c 4364 ef76 28a0 4854  ..."Q...Cd.v(.HT
-00006ed0: a300 c310 d9fc 25bc 01d1 4c11 e613 cd80  ......%...L.....
-00006ee0: 143e d10c 48e1 13cd 8014 3ed1 0c48 e113  .>..H.....>..H..
-00006ef0: cd80 143e d10c 48e1 13cd 8014 1780 10cd  ...>..H.........
-00006f00: 1461 3e52 d8a4 00e1 d77a 6d8a 028a 4435  .a>R.....zm...D5
-00006f10: 0a30 0c91 dd5f c31d 10cd 1461 3ed1 0c48  .0..._.....a>..H
-00006f20: e113 cd80 143e d10c 48e1 13cd 8014 3ed1  .....>..H.....>.
-00006f30: 0c48 e113 cd80 143e 52f8 4433 2085 4f2c  .H.....>R.D3 .O,
-00006f40: 1261 9202 845f ebb4 4107 0c3e ae5b 69c0  .a..._..A..>.[i.
-00006f50: e0e3 bb75 0738 be6e fb85 00f8 b4bf 38c0  ...u.8.n......8.
-00006f60: 60f4 0183 cfe3 361f 30f8 fc6d e101 8eaf  `.....6.0..m....
-00006f70: db7e 2100 3eee 2f0e 30d8 7200 e4df bb5f  .~!.>./.0.r...._
-00006f80: 0880 affb b4bf 38c0 700b 7240 3453 84f9  ......8.p.r@4S..
-00006f90: 4433 2085 4f34 0352 f844 3320 854f 3403  D3 .O4.R.D3 .O4.
-00006fa0: 52f8 4433 2085 4f34 0352 f848 e113 cd80  R.D3 .O4.R.H....
-00006fb0: 1417 5107 4433 4598 4f34 0352 f844 3320  ..Q.D3E.O4.R.D3 
-00006fc0: 854f 3403 52f8 4433 2085 4f34 0352 f844  .O4.R.D3 .O4.R.D
-00006fd0: 3320 854f 3403 52f8 48e1 2385 8106 087e  3 .O4.R.H.#....~
-00006fe0: 6ea1 0182 af9b 6880 e0ef 361a 20f8 bc09  n.....h...6. ...
-00006ff0: 0a10 7e7d db46 2860 f8b5 ddfb b40d 0a10  ..~}.F(`........
-00007000: 7e7d e387 9006 4433 4598 4f34 0352 f844  ~}....D3E.O4.R.D
-00007010: 3320 854f 3403 52f8 4433 2085 4f34 0352  3 .O4.R.D3 .O4.R
-00007020: f844 3320 c539 e001 d14c 11e6 13cd 8014  .D3 .9...L......
-00007030: 3ed1 0c48 e113 cd80 143e d10c 48e1 13cd  >..H.....>..H...
-00007040: 8014 3ed1 0c48 e123 854f 3403 52f8 4433  ..>..H.#.O4.R.D3
-00007050: 2085 b506 0c7e 6d1f 4041 3453 84dd 8119   ....~m.@A4S....
-00007060: 10cd 1461 3ed1 0c48 e113 cd80 143e d10c  ...a>..H.....>..
-00007070: 48e1 13cd 8014 3ed1 0c48 e123 c515 7844  H.....>..H.#..xD
-00007080: 3345 984f 3403 52f8 4433 2085 4f34 0352  3E.O4.R.D3 .O4.R
-00007090: f8d3 1111 c060 d301 839f d7e6 1a30 f8f5  .....`.......0..
-000070a0: 6ed7 0183 9fe7 861d 30f8 b96e d901 839f  n.......0..n....
-000070b0: efa6 1d30 f839 7f13 6740 3453 84f9 4433  ...0.9..g@4S..D3
-000070c0: 2085 4f34 0352 f844 3320 854f f8be 4f34   .O4.R.D3 .O..O4
-000070d0: 0352 f844 3320 8545 070c 7e4e 5b7b 00e4  .R.D3 .E..~N[{..
-000070e0: ebb6 5f08 80af fbb4 bf38 c060 c301 907f  .._......8.`....
-000070f0: ef7e 2100 7eee d3fe e200 833d 0740 febd  .~!.~......=.@..
-00007100: fb85 00f8 ba5f fb8b 030c e61f 30f8 7d6d  ....._......0.}m
-00007110: ab01 845f e3f4 29bc 01d1 4c11 e613 cd80  ..._..)...L.....
-00007120: 143e d10c 48e1 13cd 8014 3ed1 0c48 e113  .>..H.....>..H..
-00007130: cd80 143e d10c 48e1 2385 8f14 5618 a03c  ...>..H.#...V..<
-00007140: d82f 2c8e 4445 8431 0a10 7e8d dfd6 2840  ./,.DE.1..~...(@
-00007150: f835 8e5b 6ac0 415c 02d2 148e bd06 0cbe  .5.[j.A\........
-00007160: 5d1b 69c0 e0db f641 d401 d14c 11e6 13cd  ].i....A...L....
-00007170: 8014 3ed1 0c48 e113 cd80 143e d10c 48e1  ..>..H.....>..H.
-00007180: 13cd 8014 3ed1 0c48 e113 cd80 143e d10c  ....>..H.....>..
-00007190: 4861 8601 c783 fd40 6448 061b 30f8 766e  Ha.....@dH..0.vn
-000071a0: b201 836f ebc7 5007 4433 4598 4f34 0352  ...o..P.D3E.O4.R
-000071b0: f844 3320 854f 3403 52f8 4433 2085 4f34  .D3 .O4.R.D3 .O4
-000071c0: 0352 f844 3320 858f 143e d10c 48e1 23c5  .R.D3 ...>..H.#.
-000071d0: 1144 4433 4598 4f34 0352 f844 3320 c53d  .DD3E.O4.R.D3 .=
-000071e0: c801 d14c 11e6 13cd 8014 3ed1 0c48 e113  ...L......>..H..
-000071f0: cd80 143e d10c 48e1 13cd 8014 3ed1 0c48  ...>..H.....>..H
-00007200: e113 cd80 143e 5218 6d00 2251 8d02 0c43  .....>R.m."Q...C
-00007210: 6487 01c6 83fd 8a25 5979 00e4 ebb6 5f08  d......%Yy...._.
-00007220: 809f fbb4 bf38 c060 f101 90af db7e 2100  .....8.`.....~!.
-00007230: beee d7fe e200 831d 0740 febd fb85 00f8  .........@......
-00007240: b95f fb8b 030c d61b a048 54a3 00c3 10d5  ._.......HT.....
-00007250: b805 0728 12d5 28c0 3044 757e 030e d14c  ...(..(.0Du~...L
-00007260: 11e6 13cd 8014 3e52 5872 8022 518d 020c  ......>RXr."Q...
-00007270: 4354 efd6 1ca0 4854 a300 c310 d5bc 5507  CT....HT......U.
-00007280: 2812 d528 c030 4475 6f8e 0284 5fe7 b815  (..(.0Duo..._...
-00007290: 0728 12d5 28c0 3044 b56e 8f02 845f e7b9  .(..(.0D.n..._..
-000072a0: 410a 107e 9def 1629 40f8 75de 9f84 4734  A..~...)@.u...G4
-000072b0: 5384 f944 3320 854f 3403 52f8 4433 2085  S..D3 .O4.R.D3 .
-000072c0: 4ff8 be8f 1466 1b30 f837 6db7 0183 7fd7  O....f.0.7m.....
-000072d0: 861b 30f8 b76d b901 837f df76 1a30 f87b  ..0..m.....v.0.{
-000072e0: 6dbb 018e 7fef 7e21 003e ed2f 0e30 d877  m.....~!.>./.0.w
-000072f0: 8022 518d 020c 4364 d336 1ea0 4854 a300  ."Q...Cd.6..HT..
-00007300: c310 d935 0000 0001 3100 0006 0000 005b  ...5....1......[
-00007310: 0649 28b6 0c96 506c 19ca 4028 b60c aa20  .I(...Pl..@(... 
-00007320: 145b 069c 100a 0000 0000 0061 2000 0037  .[.........a ..7
-00007330: 0100 0013 0449 2c10 0000 0010 0000 0004  .....I,.........
-00007340: 1801 a041 2914 4311 9441 2154 411d d400  ...A).C..A!TA...
-00007350: 8946 0066 004a a020 0368 3502 4081 1980  .F.f.J. .h5.@...
-00007360: a10e eb8a c400 26c4 0026 863a a84a 1203  ......&..&.:.J..
-00007370: 9810 0398 a0c2 0800 9566 00c8 3403 0033  .........f..4..3
-00007380: 1166 30d4 0229 6420 d86e 1a84 0615 ba69  .f0..)d .n.....i
-00007390: 181c aa9b 06e2 a1ba 6928 20aa 9b08 23ca  ........i( ...#.
-000073a0: a26e 220e 4983 ba89 4026 6dea 2622 a136  .n".I...@&m.&".6
-000073b0: 6926 a218 6a81 1472 09ec 8801 0281 2018  i&..j..r...... .
-000073c0: cc82 3804 6040 4dc3 0684 f010 c068 8218  ..8.`@M......h..
-000073d0: 00a3 0963 408c 2690 4131 9a10 00a3 0942  ...c@.&.A1.....B
-000073e0: 309a 7006 c668 4200 8c26 08c1 6842 1a00  0.p..hB..&..hB..
-000073f0: a309 6a40 8c26 ac41 319a 1000 a309 4230  ..j@.&.A1.....B0
-00007400: 9ae0 06c6 6842 008c 2608 c188 0126 8120  ....hB..&....&. 
-00007410: 18a4 014b 7012 2406 6660 064f c328 0922  ...Kp.$.f`.O.(."
-00007420: 0666 6006 4741 0801 4d05 425d 80cc 3680  .f`.GA..M.B]..6.
-00007430: 4100 9017 20b3 0d42 10d0 2722 b30d 4220  A... ..B..'"..B 
-00007440: 1018 88c8 6c83 100c 1406 2432 db20 0404  ....l.....$2. ..
-00007450: 8981 8890 1888 0889 8188 9018 88c8 6c83  ..............l.
-00007460: 1b10 c06c 4340 04b3 0d70 4000 b30d 0111  ...lC@...p@.....
-00007470: cc36 2443 31db 1008 c64c c430 d4c2 280c  .6$C1....L.0..(.
-00007480: 1b10 c148 0cc0 30c7 7005 2d21 ac82 30dc  ...H..0.p.-!..0.
-00007490: 708d 8419 8c18 1411 0882 c129 d484 30cb  p..........)..0.
-000074a0: 4014 c10e 2306 0500 8260 900a 3491 0723  @...#....`..4..#
-000074b0: 0605 0082 60a0 0734 118c 1814 0008 8281  ....`..4........
-000074c0: 1ecc 4430 6250 4420 0806 a720 13c3 2c81  ..D0bPD ... ..,.
-000074d0: 3062 4000 2008 06a0 b013 8411 c868 4200  0b@. ........hB.
-000074e0: 8c26 08c1 68c2 208c 181c 0008 8281 28f8  .&..h. .......(.
-000074f0: c420 04c3 0d41 3f80 c12c c360 04c3 1cc3  . ...A?..,.`....
-00007500: 87b8 c4f1 12c3 8841 1181 2018 e8c1 4f08  .......A.. ...O.
-00007510: b304 c388 4111 8120 18e8 814f a0c6 2cc1  ....A.. ...O..,.
-00007520: 3062 6044 2008 0676 6016 a7f1 07b3 0443  0b`D ..v`......C
-00007530: 3810 00b1 0000 0016 1ac0 f885 00f8 b94f  8..............O
-00007540: fb06 f198 6800 e317 02e0 e77e ed1b c463  ....h......~...c
-00007550: a901 0f71 4d11 204c c4e0 4b07 f010 27b0  ...qM. L..K...'.
-00007560: 10cd 1461 3ed1 0c48 61b4 0113 714d 1120  ...a>..Ha...qM. 
-00007570: 4cc4 e04b 5384 0c84 e4d7 1780 10cd 1461  L..KS..........a
-00007580: 3e52 1870 00e4 dbba 5f08 807f fb48 2311  >R.p...._....H#.
-00007590: d164 cd01 838f df37 30f8 b86e b901 8e6f  .d.....70..n...o
-000075a0: eb7e 2100 3eed 2f0e 3018 74c0 e0e3 bd9d  .~!.>./.0.t.....
-000075b0: 0644 c435 4580 3011 83cf 100c d214 8e05  .D.5E.0.........
-000075c0: 0738 bead fb85 00f8 b8bf 38c0 6085 0182  .8........8.`...
-000075d0: 5f9b 6180 e0db d619 a0f8 8500 f8b5 6f10  _.a...........o.
-000075e0: 8f6d 0608 3e6e 9e01 8a5f 0880 6ffb 06f1  .m..>n..._..o...
-000075f0: d867 80e2 1702 e0df be41 3c06 1aa0 f885  .g.......A<.....
-00007600: 00f8 b86f 108f a906 083e 6fab 0182 df5f  ...o.....>o...._
-00007610: 8143 3453 84f9 48e1 13cd 8014 c61c 0021  .C4S..H........!
-00007620: 8d44 4413 31f8 d214 2103 2159 6bc0 e0d7  .DD.1...!.!Yk...
-00007630: b4b9 060c 7e5d 9b6f 00e4 dbba 5f08 806f  ....~].o...._..o
-00007640: fb48 2311 d174 0005 d14c 1166 b301 835f  .H#..t...L.f..._
-00007650: df26 1b30 f8b5 6db6 0183 5fe7 561b 30f8  .&.0..m..._.V.0.
-00007660: 356e b801 835f ef76 1b30 f8b5 6ed1 0183  5n..._.v.0..n...
-00007670: 9fd3 361d 30f8 396e bb01 8e6f eb7e 2100  ..6.0.9n...o.~!.
-00007680: 7eed 2f0e 3058 75c0 e0e7 ba2d 0738 4823  ~./.0Xu....-.8H#
-00007690: 11d1 440c be74 000f 61c5 0190 6feb 7e21  ..D..t..a...o.~!
-000076a0: 00be eed3 fee2 0083 4907 0c7e 6e1b 75c0  ........I..~n.u.
-000076b0: e0e7 b98d 0630 7e21 00be eed3 be41 3c46  .....0~!.....A<F
-000076c0: 1ac0 f885 00f8 ba5f fb06 f11c 8246 3453  ......._.....F4S
-000076d0: 84f9 48e1 13cd 8014 3ed1 0c48 e113 cd80  ..H.....>..H....
-000076e0: 1456 1a70 1097 8034 8563 a801 0e71 4d11  .V.p...4.c...qM.
-000076f0: 204c c4e0 0fc0 041c c142 3453 84f9 48e1   L.......B4S..H.
-00007700: 2385 f106 40be adfb 8500 f8b5 8f34 1211  #...@........4..
-00007710: 4dc6 19b0 f885 00f8 b46f 104f 6dce 0183  M........o.Om...
-00007720: 6fe3 d61b e0f8 b6ee 1702 e0db fee2 0083  o...............
-00007730: 0d07 40be adfb 8500 f8b9 4ffb 8b03 0c66  ..@.......O....f
-00007740: 1c00 f9b6 ee17 02e0 eb7e ed2f 0e30 dc41  .........~./.0.A
-00007750: 4434 5384 f948 e113 cd80 143e 5258 6c40  D4S..H.....>RXl@
-00007760: 445c 5304 0813 31f8 d201 3c84 5fdb 73c0  D\S...1...<._.s.
-00007770: e0eb fc19 3844 3345 988f 143e 52f8 4861  ....8D3E...>R.Ha
-00007780: b001 1071 4d11 204c c4e0 0fc0 04f8 b5e9  ...qM. L........
-00007790: 0640 bead fb85 00f8 b48f 3412 114d c61a  .@........4..M..
-000077a0: 1011 d714 01c2 440c be34 45c8 4048 261c  ......D..4E.@H&.
-000077b0: 00f9 b6ee 1702 e0e3 3ed2 4844 3419 72c0  ........>.HD4.r.
-000077c0: e0df b629 070c fe7d db6b c044 5c53 0408  ...)...}.k.D\S..
-000077d0: 1331 f80c c120 4de1 f8b5 fd06 38be adfb  .1... M.....8...
-000077e0: 8500 f8b7 bf38 c060 c401 906f eb7e 2100  .....8.`...o.~!.
-000077f0: 7eee d7fe e200 0300 0000 0001 3100 0002  ~...........1...
-00007800: 0000 005b 8653 100a 0000 0000 0000 0061  ...[.S.........a
-00007810: 2000 0025 0100 0013 0449 2c10 0000 0009   ..%.....I,.....
-00007820: 0000 0004 1801 28e4 001a 9441 0115 0189  ......(....A....
-00007830: 4600 4aa0 608a a020 0aaa 402c 0b22 b41a  F.J.`.. ..@,."..
-00007840: 01a0 80ed 6e08 00f1 3000 0049 0000 0022  ....n...0..I..."
-00007850: 47c8 9051 0e08 8a00 0000 00af 900b b800  G..Q............
-00007860: 0000 005f 5a4e 356e 756d 6261 326e 7036  ..._ZN5numba2np6
-00007870: 6c69 6e61 6c67 3235 5f64 756d 6d79 5f6c  linalg25_dummy_l
-00007880: 6976 656e 6573 735f 6675 6e63 2432 3432  iveness_func$242
-00007890: 3945 3330 6c69 7374 2432 3869 6e74 3634  9E30list$28int64
-000078a0: 2432 3924 3363 6976 2433 644e 6f6e 6524  $29$3civ$3dNone$
-000078b0: 3365 5f5a 4e35 6e75 6d62 6132 6e70 366c  3e_ZN5numba2np6l
-000078c0: 696e 616c 6732 355f 6475 6d6d 795f 6c69  inalg25_dummy_li
-000078d0: 7665 6e65 7373 5f66 756e 6324 3234 3239  veness_func$2429
-000078e0: 4533 306c 6973 7424 3238 696e 7436 3424  E30list$28int64$
-000078f0: 3239 2433 6369 7624 3364 4e6f 6e65 2433  29$3civ$3dNone$3
-00007900: 653a 2025 6578 6369 6e66 6f5f 5a4e 356e  e: %excinfo_ZN5n
-00007910: 756d 6261 326e 7036 6c69 6e61 6c67 3235  umba2np6linalg25
-00007920: 5f64 756d 6d79 5f6c 6976 656e 6573 735f  _dummy_liveness_
-00007930: 6675 6e63 2432 3432 3945 3330 6c69 7374  func$2429E30list
-00007940: 2432 3869 6e74 3634 2432 3924 3363 6976  $28int64$29$3civ
-00007950: 2433 644e 6f6e 6524 3365 3a20 2572 6574  $3dNone$3e: %ret
-00007960: 7074 722b 8405 5931 304b b262 6816 6583  ptr+..Y10K.bh.e.
-00007970: d030 0023 0606 1082 60f0 06f0 6030 0d20  .0.#....`...`0. 
-00007980: 0449 06db a580 4486 1b2e 070c 6619 8421  .I....D.....f..!
-00007990: 1831 2880 1004 033d 1087 62c4 8000 4210  .1(....=..b...B.
-000079a0: 0c5a 211c 860d 888e 2408 605d 61d8 80e8  .Z!.....$.`]a...
-000079b0: 4682 00d6 1532 1b59 5e23 bb40 a00c 4434  F....2.Y^#.@..D4
-000079c0: 6290 0021 0806 af50 0ed8 c605 c770 43d0  b..!...P.....pC.
-000079d0: 0b68 30cb 1010 c188 8101 8420 18c4 4239  .h0........ ..B9
-000079e0: 44cd 7043 200b 6030 cb50 18c1 b001 5106  D.pC .`0.P....Q.
-000079f0: 2a41 006b 0b0d 2008 5606 e4a5 604c ba78  *A.k.. .V...`L.x
-00007a00: 08b6 5c18 3620 828c 0092 282f 055c 326c  ..\.6 ....(/.\2l
-00007a10: 4004 1e01 5031 265d 3c04 1f18 0c1b 1041  @...P1&]<......A
-00007a20: 1904 001d 63d2 c543 1006 6490 4160 470c  ....c..C..d.A`G.
-00007a30: 9029 04c1 6016 e221 4083 6ea3 834b 860d  .)..`..!@.n..K..
-00007a40: 8820 0c08 8096 31e9 e221 2803 3418 3620  . ....1..!(.4.6 
-00007a50: 8232 2000 6ac6 a48b 87e0 0cd4 a089 84e0  .2 .j...........
-00007a60: 0c86 0d88 600e 0880 1a2e a140 4486 1b02  ....`......@D...
-00007a70: 3540 8359 8603 0932 0fb8 3b6c 4004 6640  5@.Y...2..;l@.f@
-00007a80: 00bb 0e23 0645 1482 60a0 0720 7125 1870  ...#.E..`.. q%.p
-00007a90: 9702 1119 3128 8010 0403 3d10 8932 c83e  ....1(....=..2.>
-00007aa0: e0ee b001 1108 04b0 f810 0e04 0000 0070  ...............p
-00007ab0: 0000 0087 b06d bcee 13cd 8014 3ed1 0c48  .....m......>..H
-00007ac0: e113 cd80 143e d10c 4871 03da 46fb 4433  .....>..Hq..F.D3
-00007ad0: 2085 4f34 0352 f844 3320 854f 3403 5258   .O4.R.D3 .O4.RX
-00007ae0: 6900 e1db b46e 8c01 0910 193e e0e7 3e7d  i....n.....>..>}
-00007af0: 02d7 46fb 4433 2085 4f34 0352 f844 3320  ..F.D3 .O4.R.D3 
-00007b00: 858f 1417 306c bb6d a201 847f ebb7 e106  ....0l.m........
-00007b10: 107e 6ef3 e61b 50f8 b7ee 2386 1a40 f8b7  .~n...P...#..@..
-00007b20: bd5b 6bc0 e1eb 3e62 dfb6 d106 103e cef3  .[k...>b.....>..
-00007b30: 161c 60f8 ba6d dff5 1130 1baf fb44 3320  ..`..m...0...D3 
-00007b40: 858f 1476 1b80 f8ba 8fd4 b5bd 9b69 00e1  ...v.........i..
-00007b50: db75 6ea9 0184 8fe7 b4a9 0610 3e9e d716  .un.........>...
-00007b60: 1b80 f8ba 8fd8 f78d db6a 40e1 e73e 529f  .........j@..>R.
-00007b70: 41b5 f1ba 4f34 0352 f844 3320 854f 3403  A...O4.R.D3 .O4.
-00007b80: 52d8 6900 e1db fd7e 0005 d14c 1166 b501  R.i....~...L.f..
-00007b90: 848f f7bd 7906 107e ee23 961b 70f8 ba8f  ....y..~.#..p...
-00007ba0: ec76 6f9d 0184 5fd3 bce9 0610 7e8e dbb6  .vo..._.....~...
-00007bb0: 1b40 f839 7e5b 6340 0244 860f f8ba 4f9b  .@.9~[c@.D....O.
-00007bc0: 61c0 415c 02d2 148e f506 14fe 9dfb 88cd  a.A\............
-00007bd0: 0620 beee 2375 7feb 7780 6dbc ee13 cd80  . ..#u..w.m.....
-00007be0: 143e d10c 48e1 13cd 8014 3e52 986b 00e1  .>..H.....>R.k..
-00007bf0: e3fa 6db6 0189 affb 489d dbb9 6d85 0146  ..m.....H...m..F
-00007c00: 444c cf14 1968 80e1 eb3e 62e3 061b 80f8  DL...h...>b.....
-00007c10: ba8f e0f7 5ddb 61c0 0144 860f f8b4 2106  ....].a..D....!.
-00007c20: 1c40 64f8 805f 5b62 c001 4486 0ff8 b629  .@d.._[b..D....)
-00007c30: 061c 4064 f880 7fdb 62c0 0144 860f f8b8  ..@d....b..D....
-00007c40: c906 103e bee7 461a 40f8 75bf db68 00e1  ...>..F.@.u..h..
-00007c50: d73d 6fa1 0184 5ff7 bdf1 0624 beee 23b8  .=o..._....$..#.
-00007c60: ee23 f715 481b affb 4433 2085 4f34 0352  .#..H...D3 .O4.R
-00007c70: f848 0101 3100 000b 0000 005b 8642 28b6  .H..1......[.B(.
-00007c80: 0c89 676c 1916 cfd8 3254 42b1 65b8 3c63  ..gl....2TB.e.<c
-00007c90: cb00 0748 b365 8803 a4d9 32cc 8150 6c19  ...H.e....2..Pl.
-00007ca0: ecc0 3300 0000 0000 0000 0061 2000 0026  ..3........a ..&
-00007cb0: 0000 0013 0444 2c10 0000 0001 0000 0024  .....D,........$
-00007cc0: 2a01 00c3 0dc2 1b80 c12c 4320 043a 6420  *........,C .:d 
-00007cd0: 1041 0edc 1d33 3082 4100 8460 b821 20c0  .A...30.A..`.! .
-00007ce0: 6096 6108 8221 0361 0846 0c8a 2804 c140  `.a..!.a.F..(..@
-00007cf0: 0f4a c1d0 7020 000e 0000 00a6 1830 f835  .J..p .......0.5
-00007d00: 7d00 827f db61 80e0 e337 b0f8 b74f 3403  }....a...7...O4.
-00007d10: 52f8 4871 0288 7ffb 4433 2085 2106 083e  R.Hq....D3 .!..>
-00007d20: 6f89 0184 8ffb c805 14fe ed23 8515 0608  o..........#....
-00007d30: 7e0d 0001 3100 0003 0000 005b 8640 28b6  ~...1......[.@(.
-00007d40: 0c87 5000 0000 0000 0000 0061 2000 0007  ..P........a ...
-00007d50: 0000 0013 0481 8603 0100 0003 0000 0007  ................
-00007d60: 20f8 b715 0608 7e0d 0000 0000 0000 0061   .....~........a
-00007d70: 2000 001a 0000 0013 0443 2c10 0000 0001   ........C,.....
-00007d80: 0000 0024 2a01 00c3 0dc2 1b80 c12c 4320  ...$*........,C 
-00007d90: 049a 0377 c70c 8c60 0800 21d0 7020 000a  ...w...`..!.p ..
-00007da0: 0000 0007 20f8 b71d 0608 3e7e 0288 7ffb  .... .....>~....
-00007db0: 4433 2085 2106 08fe 6e89 0184 8ffb c805  D3 .!...n.......
-00007dc0: 14fe ed23 8515 0608 7e0d 0001 3100 0002  ...#....~...1...
-00007dd0: 0000 005b 8640 2800 0000 0000 0000 0071  ...[.@(........q
-00007de0: 2000 0008 0000 0032 0e10 2284 2b93 09e8   ......2..".+...
-00007df0: b2bf 8139 ac20 f853 2e82 408c 2538 445b  ...9. .S..@.%8D[
-00007e00: 8247 bd25 0000 0000 0000 0065 0c00 0005  .G.%.......e....
-00007e10: 0200 0012 0394 2828 0000 0002 0000 0062  ......((.......b
-00007e20: 0c00 0006 0000 004c 0000 0001 0000 0058  .......L.......X
-00007e30: 0000 0000 0000 0058 0000 004b 0000 0060  .......X...K...`
-00007e40: 0700 0007 0000 0068 0c00 0019 0000 0081  .......h........
-00007e50: 0c00 0008 0000 0097 0000 0000 0000 0008  ................
-00007e60: 0800 0000 0000 0000 0000 004b 0000 0000  ...........K....
-00007e70: 0000 0089 0c00 008e 0000 0052 0800 008d  ...........R....
-00007e80: 0000 00ff ffff ff10 2600 0017 0d00 001c  ........&.......
-00007e90: 0000 00df 0800 001b 0000 00ff ffff ff08  ................
-00007ea0: 2c00 0033 0d00 001f 0000 00fa 0800 001e  ,..3............
-00007eb0: 0000 00ff ffff ff08 2400 0052 0d00 0096  ........$..R....
-00007ec0: 0000 0018 0900 0095 0000 00ff ffff ff10  ................
-00007ed0: 2600 00e8 0d00 0012 0000 00ad 0900 0011  &...............
-00007ee0: 0000 00ff ffff ff08 2400 00fa 0d00 0010  ........$.......
-00007ef0: 0000 00be 0900 000f 0000 00ff ffff ff08  ................
-00007f00: 2400 000a 0e00 001e 0000 00cd 0900 001d  $...............
-00007f10: 0000 00ff ffff ff08 2400 0028 0e00 000a  ........$..(....
-00007f20: 0000 00ea 0900 0009 0000 00ff ffff ff08  ................
-00007f30: 2400 0032 0e00 000f 0000 00f3 0900 000e  $..2............
-00007f40: 0000 00ff ffff ff08 2400 0041 0e00 0023  ........$..A...#
-00007f50: 0000 0001 0a00 0022 0000 00ff ffff ff08  ......."........
-00007f60: 2400 0064 0e00 000c 0000 0023 0a00 000b  $..d.......#....
-00007f70: 0000 00ff ffff ff08 2400 0070 0e00 000f  ........$..p....
-00007f80: 0000 002e 0a00 000e 0000 00ff ffff ff08  ................
-00007f90: 2400 007f 0e00 000f 0000 003c 0a00 000e  $..........<....
-00007fa0: 0000 00ff ffff ff08 2400 008e 0e00 000e  ........$.......
-00007fb0: 0000 004a 0a00 000d 0000 00ff ffff ff08  ...J............
-00007fc0: 2400 009c 0e00 0094 0000 0057 0a00 0093  $..........W....
-00007fd0: 0000 00ff ffff ff10 2600 0030 0f00 0011  ........&..0....
-00007fe0: 0000 00ea 0a00 0010 0000 00ff ffff ff08  ................
-00007ff0: 2400 0041 0f00 0015 0000 00fa 0a00 0014  $..A............
-00008000: 0000 00ff ffff ff08 2400 0056 0f00 0016  ........$..V....
-00008010: 0000 000e 0b00 0015 0000 00ff ffff ff08  ................
-00008020: 2400 006c 0f00 000a 0000 0023 0b00 0009  $..l.......#....
-00008030: 0000 00ff ffff ff08 2400 0076 0f00 0012  ........$..v....
-00008040: 0000 002c 0b00 0011 0000 00ff ffff ff08  ...,............
-00008050: 2400 0088 0f00 005f 0000 003d 0b00 005e  $......_...=...^
-00008060: 0000 00ff ffff ff10 2600 00e7 0f00 000b  ........&.......
-00008070: 0000 009b 0b00 000a 0000 00ff ffff ff10  ................
-00008080: 2600 00f2 0f00 0012 0000 00a5 0b00 0011  &...............
-00008090: 0000 00ff ffff ff08 2400 0004 1000 000d  ........$.......
-000080a0: 0000 00b6 0b00 000c 0000 00ff ffff ff08  ................
-000080b0: 2400 0011 1000 0011 0000 00c2 0b00 0010  $...............
-000080c0: 0000 00ff ffff ff10 2400 0022 1000 001d  ........$.."....
-000080d0: 0000 00d2 0b00 001c 0000 00ff ffff ff08  ................
-000080e0: 2400 003f 1000 0015 0000 00ee 0b00 0014  $..?............
-000080f0: 0000 00ff ffff ff08 2c00 0054 1000 0016  ........,..T....
-00008100: 0000 0002 0c00 0015 0000 00ff ffff ff08  ................
-00008110: 2400 006a 1000 000b 0000 0017 0c00 000a  $..j............
-00008120: 0000 00ff ffff ff10 2600 0075 1000 0019  ........&..u....
-00008130: 0000 0021 0c00 0018 0000 00ff ffff ff08  ...!............
-00008140: 2c00 008e 1000 0017 0000 0039 0c00 0016  ,..........9....
-00008150: 0000 00ff ffff ff08 2c00 00a5 1000 0014  ........,.......
-00008160: 0000 004f 0c00 0013 0000 00ff ffff ff08  ...O............
-00008170: 2c00 00b9 1000 0098 0000 0000 0000 0097  ,...............
-00008180: 0000 00ff ffff ff24 0400 0051 1100 0021  .......$...Q...!
-00008190: 0000 0097 0000 0020 0000 00ff ffff ff00  ....... ........
-000081a0: 0000 0072 1100 0021 0000 00b7 0000 0020  ...r...!....... 
-000081b0: 0000 00ff ffff ff00 0000 0093 1100 0022  ..............."
-000081c0: 0000 00d7 0000 0021 0000 00ff ffff ff00  .......!........
-000081d0: 0000 00b5 1100 0027 0000 00f8 0000 0026  .......'.......&
-000081e0: 0000 00ff ffff ff00 0000 00dc 1100 0022  ..............."
-000081f0: 0000 001e 0100 0021 0000 00ff ffff ff00  .......!........
-00008200: 0000 00fe 1100 0027 0000 003f 0100 0026  .......'...?...&
-00008210: 0000 00ff ffff ff00 0000 0025 1200 0024  ...........%...$
-00008220: 0000 0065 0100 0023 0000 00ff ffff ff00  ...e...#........
-00008230: 0000 0049 1200 0013 0000 0088 0100 0012  ...I............
-00008240: 0000 00ff ffff ff08 0400 005c 1200 00b4  ...........\....
-00008250: 0000 009a 0100 00b3 0000 00ff ffff ff00  ................
-00008260: 0000 0010 1300 0010 0000 004d 0200 000f  ...........M....
-00008270: 0000 00ff ffff ff08 0400 0020 1300 0060  ........... ...`
-00008280: 0000 005c 0200 005f 0000 00ff ffff ff00  ...\..._........
-00008290: 0000 0080 1300 000f 0000 00bb 0200 000e  ................
-000082a0: 0000 00ff ffff ff08 0400 008f 1300 002c  ...............,
-000082b0: 0000 00c9 0200 002b 0000 00ff ffff ff00  .......+........
-000082c0: 0000 00bb 1300 0014 0000 00f4 0200 0013  ................
-000082d0: 0000 00ff ffff ff08 0400 00cf 1300 0012  ................
-000082e0: 0000 0007 0300 0011 0000 00ff ffff ff08  ................
-000082f0: 0400 00e1 1300 0032 0000 0018 0300 0031  .......2.......1
-00008300: 0000 00ff ffff ff00 0000 0013 1400 003c  ...............<
-00008310: 0000 0049 0300 003b 0000 00ff ffff ff00  ...I...;........
-00008320: 0000 004f 1400 0034 0000 0084 0300 0033  ...O...4.......3
-00008330: 0000 00ff ffff ff00 0000 0083 1400 0059  ...............Y
-00008340: 0000 00b7 0300 0058 0000 00ff ffff ff24  .......X.......$
-00008350: 0400 00dc 1400 0021 0000 000f 0400 0020  .......!....... 
-00008360: 0000 00ff ffff ff00 0000 00fd 1400 0021  ...............!
-00008370: 0000 002f 0400 0020 0000 00ff ffff ff00  .../... ........
-00008380: 0000 001e 1500 0022 0000 004f 0400 0021  ......."...O...!
-00008390: 0000 00ff ffff ff00 0000 0040 1500 0027  ...........@...'
-000083a0: 0000 0070 0400 0026 0000 00ff ffff ff00  ...p...&........
-000083b0: 0000 0067 1500 0022 0000 0096 0400 0021  ...g...".......!
-000083c0: 0000 00ff ffff ff00 0000 0089 1500 0027  ...............'
-000083d0: 0000 00b7 0400 0026 0000 00ff ffff ff00  .......&........
-000083e0: 0000 00b0 1500 0048 0000 00dd 0400 0047  .......H.......G
-000083f0: 0000 00ff ffff ff24 0400 00f8 1500 004a  .......$.......J
-00008400: 0000 0024 0500 0049 0000 00ff ffff ff24  ...$...I.......$
-00008410: 0400 0042 1600 0089 0000 006d 0500 0088  ...B.......m....
-00008420: 0000 00ff ffff ff24 0400 00cb 1600 0069  .......$.......i
-00008430: 0000 00f5 0500 0068 0000 00ff ffff ff24  .......h.......$
-00008440: 0400 0034 1700 005a 0000 005d 0600 0059  ...4...Z...]...Y
-00008450: 0000 00ff ffff ff24 0400 008e 1700 0021  .......$.......!
-00008460: 0000 00b6 0600 0020 0000 00ff ffff ff00  ....... ........
-00008470: 0000 00af 1700 0021 0000 00d6 0600 0020  .......!....... 
-00008480: 0000 00ff ffff ff00 0000 00d0 1700 0021  ...............!
-00008490: 0000 00f6 0600 0020 0000 00ff ffff ff00  ....... ........
-000084a0: 0000 00f1 1700 0021 0000 0016 0700 0020  .......!....... 
-000084b0: 0000 00ff ffff ff00 0000 0012 1800 0022  ..............."
-000084c0: 0000 0036 0700 0021 0000 00ff ffff ff00  ...6...!........
-000084d0: 0000 0034 1800 0027 0000 0057 0700 0026  ...4...'...W...&
-000084e0: 0000 00ff ffff ff00 0000 005b 1800 0022  ...........[..."
-000084f0: 0000 007d 0700 0021 0000 00ff ffff ff00  ...}...!........
-00008500: 0000 007d 1800 0027 0000 009e 0700 0026  ...}...'.......&
-00008510: 0000 00ff ffff ff00 0000 00a4 1800 0022  ..............."
-00008520: 0000 00c4 0700 0021 0000 00ff ffff ff00  .......!........
-00008530: 0000 00c6 1800 0027 0000 00e5 0700 0026  .......'.......&
-00008540: 0000 00ff ffff ff00 0000 00ed 1800 0022  ..............."
-00008550: 0000 000b 0800 0021 0000 00ff ffff ff00  .......!........
-00008560: 0000 000f 1900 0027 0000 002c 0800 0026  .......'...,...&
-00008570: 0000 00ff ffff ff00 0000 0008 0000 0000  ................
-00008580: 0000 0097 0000 0000 0000 0097 0000 0000  ................
-00008590: 0000 0008 0000 0000 0000 0097 0000 0000  ................
-000085a0: 0000 0097 0000 0000 0000 0008 0000 0000  ................
-000085b0: 0000 0097 0000 0000 0000 0097 0000 0000  ................
-000085c0: 0000 0008 0000 0000 0000 0097 0000 0000  ................
-000085d0: 0000 0097 0000 0000 0000 0008 0000 0000  ................
-000085e0: 0000 0097 0000 0000 0000 0097 0000 0000  ................
-000085f0: 0000 0008 0000 0000 0000 0097 0000 0000  ................
-00008600: 0000 0097 0000 0000 0000 0008 0000 0000  ................
-00008610: 0000 0097 0000 0000 0000 0097 0000 0000  ................
-00008620: 0000 0000 0000 005d 0c00 0051 0600 0012  .......]...Q....
-00008630: 0394 766a 0000 005f 5a4e 3038 4e75 6d62  ..vj..._ZN08Numb
-00008640: 6145 6e76 3573 696d 6261 366d 6978 696e  aEnv5simba6mixin
-00008650: 7332 3466 6561 7475 7265 5f65 7874 7261  s24feature_extra
-00008660: 6374 696f 6e5f 6d69 7869 6e32 3246 6561  ction_mixin22Fea
-00008670: 7475 7265 4578 7472 6163 7469 6f6e 4d69  tureExtractionMi
-00008680: 7869 6e31 3063 6469 7374 2432 3435 3545  xin10cdist$2455E
-00008690: 3541 7272 6179 4964 4c69 3245 3141 376d  5ArrayIdLi2E1A7m
-000086a0: 7574 6162 6c65 3761 6c69 676e 6564 4535  utable7alignedE5
-000086b0: 4172 7261 7949 644c 6932 4531 4137 6d75  ArrayIdLi2E1A7mu
-000086c0: 7461 626c 6537 616c 6967 6e65 6445 2e63  table7alignedE.c
-000086d0: 6f6e 7374 2e70 6963 6b6c 6562 7566 2e31  onst.picklebuf.1
-000086e0: 3430 3531 3339 3739 3236 3334 3438 2e63  40513979263448.c
-000086f0: 6f6e 7374 2e70 6963 6b6c 6562 7566 2e31  onst.picklebuf.1
-00008700: 3430 3531 3339 3638 3332 3739 3932 2e63  40513968327992.c
-00008710: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
-00008720: 3134 3035 3133 3936 3833 3237 3939 322e  140513968327992.
-00008730: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
-00008740: 2e31 3430 3531 3339 3638 3332 3739 3932  .140513968327992
-00008750: 2e73 6861 312e 636f 6e73 742e 7069 636b  .sha1.const.pick
-00008760: 6c65 6461 7461 2e31 3430 3531 3339 3739  ledata.140513979
-00008770: 3236 3334 3438 2e63 6f6e 7374 2e70 6963  263448.const.pic
-00008780: 6b6c 6564 6174 612e 3134 3035 3133 3937  kledata.14051397
-00008790: 3932 3633 3434 382e 7368 6131 2e63 6f6e  9263448.sha1.con
-000087a0: 7374 2e46 6561 7475 7265 4578 7472 6163  st.FeatureExtrac
-000087b0: 7469 6f6e 4d69 7869 6e2e 6364 6973 7450  tionMixin.cdistP
-000087c0: 7945 7863 5f52 756e 7469 6d65 4572 726f  yExc_RuntimeErro
-000087d0: 722e 636f 6e73 742e 6d69 7373 696e 6720  r.const.missing 
-000087e0: 456e 7669 726f 6e6d 656e 743a 205f 5a4e  Environment: _ZN
-000087f0: 3038 4e75 6d62 6145 6e76 3573 696d 6261  08NumbaEnv5simba
-00008800: 366d 6978 696e 7332 3466 6561 7475 7265  6mixins24feature
-00008810: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
-00008820: 6e32 3246 6561 7475 7265 4578 7472 6163  n22FeatureExtrac
-00008830: 7469 6f6e 4d69 7869 6e31 3063 6469 7374  tionMixin10cdist
-00008840: 2432 3435 3545 3541 7272 6179 4964 4c69  $2455E5ArrayIdLi
-00008850: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
-00008860: 676e 6564 4535 4172 7261 7949 644c 6932  gnedE5ArrayIdLi2
-00008870: 4531 4137 6d75 7461 626c 6537 616c 6967  E1A7mutable7alig
-00008880: 6e65 6445 5079 4578 635f 5479 7065 4572  nedEPyExc_TypeEr
-00008890: 726f 722e 636f 6e73 742e 6361 6e27 7420  ror.const.can't 
-000088a0: 756e 626f 7820 6172 7261 7920 6672 6f6d  unbox array from
-000088b0: 2050 794f 626a 6563 7420 696e 746f 206e   PyObject into n
-000088c0: 6174 6976 6520 7661 6c75 652e 2020 5468  ative value.  Th
-000088d0: 6520 6f62 6a65 6374 206d 6179 6265 206f  e object maybe o
-000088e0: 6620 6120 6469 6666 6572 656e 7420 7479  f a different ty
-000088f0: 7065 5f50 795f 4e6f 6e65 5374 7275 6374  pe_Py_NoneStruct
-00008900: 2e63 6f6e 7374 2e60 656e 762e 636f 6e73  .const.`env.cons
-00008910: 7473 6020 6973 204e 554c 4c20 696e 2060  ts` is NULL in `
-00008920: 7265 6164 5f63 6f6e 7374 6050 7945 7863  read_const`PyExc
-00008930: 5f53 746f 7049 7465 7261 7469 6f6e 5079  _StopIterationPy
-00008940: 4578 635f 5379 7374 656d 4572 726f 722e  Exc_SystemError.
-00008950: 636f 6e73 742e 756e 6b6e 6f77 6e20 6572  const.unknown er
-00008960: 726f 7220 7768 656e 2063 616c 6c69 6e67  ror when calling
-00008970: 206e 6174 6976 6520 6675 6e63 7469 6f6e   native function
-00008980: 2e63 6f6e 7374 2e3c 6e75 6d62 612e 636f  .const.<numba.co
-00008990: 7265 2e63 7075 2e43 5055 436f 6e74 6578  re.cpu.CPUContex
-000089a0: 7420 6f62 6a65 6374 2061 7420 3078 3766  t object at 0x7f
-000089b0: 6362 6635 3561 6432 3038 3e2e 636f 6e73  cbf55ad208>.cons
-000089c0: 742e 756e 6b6e 6f77 6e20 6572 726f 7220  t.unknown error 
-000089d0: 7768 656e 2063 616c 6c69 6e67 206e 6174  when calling nat
-000089e0: 6976 6520 6675 6e63 7469 6f6e 2e31 5f5a  ive function.1_Z
-000089f0: 4e30 384e 756d 6261 456e 7635 6e75 6d62  N08NumbaEnv5numb
-00008a00: 6132 6e70 3861 7272 6179 6f62 6a31 336e  a2np8arrayobj13n
-00008a10: 756d 7079 5f66 756c 6c5f 6e64 3132 2433  umpy_full_nd12$3
-00008a20: 636c 6f63 616c 7324 3365 3966 756c 6c24  clocals$3e9full$
-00008a30: 3234 3536 4538 556e 6954 7570 6c65 4978  2456E8UniTupleIx
-00008a40: 4c69 3245 4564 2e63 6f6e 7374 2e70 6963  Li2EEd.const.pic
-00008a50: 6b6c 6562 7566 2e31 3430 3531 3339 3633  klebuf.140513963
-00008a60: 3036 3631 3336 2e63 6f6e 7374 2e70 6963  066136.const.pic
-00008a70: 6b6c 6562 7566 2e31 3430 3531 3339 3739  klebuf.140513979
-00008a80: 3830 3235 3336 2e63 6f6e 7374 2e70 6963  802536.const.pic
-00008a90: 6b6c 6564 6174 612e 3134 3035 3133 3937  kledata.14051397
-00008aa0: 3938 3032 3533 362e 636f 6e73 742e 7069  9802536.const.pi
-00008ab0: 636b 6c65 6461 7461 2e31 3430 3531 3339  ckledata.1405139
-00008ac0: 3739 3830 3235 3336 2e73 6861 312e 636f  79802536.sha1.co
-00008ad0: 6e73 742e 7069 636b 6c65 6461 7461 2e31  nst.pickledata.1
-00008ae0: 3430 3531 3339 3633 3036 3631 3336 2e63  40513963066136.c
-00008af0: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
-00008b00: 3134 3035 3133 3936 3330 3636 3133 362e  140513963066136.
-00008b10: 7368 6131 5f5a 4e30 384e 756d 6261 456e  sha1_ZN08NumbaEn
-00008b20: 7631 3324 3363 6479 6e61 6d69 6324 3365  v13$3cdynamic$3e
-00008b30: 3338 5f5f 6e75 6d62 615f 6172 7261 795f  38__numba_array_
-00008b40: 6578 7072 5f30 7837 6663 6266 3535 6232  expr_0x7fcbf55b2
-00008b50: 6534 3824 3234 3537 4564 645f 5a4e 3038  e48$2457Edd_ZN08
-00008b60: 4e75 6d62 6145 6e76 356e 756d 6261 326e  NumbaEnv5numba2n
-00008b70: 7037 6e70 7969 6d70 6c32 305f 6272 6f61  p7npyimpl20_broa
-00008b80: 6463 6173 745f 6f6e 746f 2432 3431 3045  dcast_onto$2410E
-00008b90: 7838 696e 7436 3424 3261 7838 696e 7436  x8int64$2ax8int6
-00008ba0: 3424 3261 5f5a 4e30 384e 756d 6261 456e  4$2a_ZN08NumbaEn
-00008bb0: 7635 6e75 6d62 6132 6e70 366c 696e 616c  v5numba2np6linal
-00008bc0: 6731 345f 6765 745f 6e6f 726d 5f69 6d70  g14_get_norm_imp
-00008bd0: 6c31 3224 3363 6c6f 6361 6c73 2433 6531  l12$3clocals$3e1
-00008be0: 346f 6e65 445f 696d 706c 2432 3432 3745  4oneD_impl$2427E
-00008bf0: 3541 7272 6179 4964 4c69 3145 3143 376d  5ArrayIdLi1E1C7m
-00008c00: 7574 6162 6c65 3761 6c69 676e 6564 4532  utable7alignedE2
-00008c10: 376f 6d69 7474 6564 2432 3864 6566 6175  7omitted$28defau
-00008c20: 6c74 2433 644e 6f6e 6524 3239 5f5a 4e30  lt$3dNone$29_ZN0
-00008c30: 384e 756d 6261 456e 7635 6e75 6d62 6132  8NumbaEnv5numba2
-00008c40: 6e70 366c 696e 616c 6731 375f 6f6e 6544  np6linalg17_oneD
-00008c50: 5f6e 6f72 6d5f 325f 696d 706c 3132 2433  _norm_2_impl12$3
-00008c60: 636c 6f63 616c 7324 3365 3969 6d70 6c24  clocals$3e9impl$
-00008c70: 3234 3238 4535 4172 7261 7949 644c 6931  2428E5ArrayIdLi1
-00008c80: 4531 4337 6d75 7461 626c 6537 616c 6967  E1C7mutable7alig
-00008c90: 6e65 6445 5f5a 4e30 384e 756d 6261 456e  nedE_ZN08NumbaEn
-00008ca0: 7635 6e75 6d62 6132 6e70 366c 696e 616c  v5numba2np6linal
-00008cb0: 6732 355f 6475 6d6d 795f 6c69 7665 6e65  g25_dummy_livene
-00008cc0: 7373 5f66 756e 6324 3234 3239 4533 306c  ss_func$2429E30l
-00008cd0: 6973 7424 3238 696e 7436 3424 3239 2433  ist$28int64$29$3
-00008ce0: 6369 7624 3364 4e6f 6e65 2433 652e 636f  civ$3dNone$3e.co
-00008cf0: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
-00008d00: 3035 3133 3937 3338 3130 3031 362e 636f  0513973810016.co
-00008d10: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
-00008d20: 3035 3133 3936 3431 3530 3134 342e 636f  0513964150144.co
-00008d30: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
-00008d40: 3035 3133 3936 3838 3932 3038 382e 636f  0513968892088.co
-00008d50: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
-00008d60: 3035 3133 3937 3237 3535 3430 382e 636f  0513972755408.co
-00008d70: 6e73 742e 7069 636b 6c65 6461 7461 2e31  nst.pickledata.1
-00008d80: 3430 3531 3339 3732 3735 3534 3038 2e63  40513972755408.c
-00008d90: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
-00008da0: 3134 3035 3133 3937 3237 3535 3430 382e  140513972755408.
-00008db0: 7368 6131 2e63 6f6e 7374 2e70 6963 6b6c  sha1.const.pickl
-00008dc0: 6564 6174 612e 3134 3035 3133 3936 3838  edata.1405139688
-00008dd0: 3932 3038 382e 636f 6e73 742e 7069 636b  92088.const.pick
-00008de0: 6c65 6461 7461 2e31 3430 3531 3339 3638  ledata.140513968
-00008df0: 3839 3230 3838 2e73 6861 312e 636f 6e73  892088.sha1.cons
-00008e00: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
-00008e10: 3531 3339 3634 3135 3031 3434 2e63 6f6e  513964150144.con
-00008e20: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-00008e30: 3035 3133 3936 3431 3530 3134 342e 7368  0513964150144.sh
-00008e40: 6131 2e63 6f6e 7374 2e70 6963 6b6c 6564  a1.const.pickled
-00008e50: 6174 612e 3134 3035 3133 3937 3338 3130  ata.140513973810
-00008e60: 3031 362e 636f 6e73 742e 7069 636b 6c65  016.const.pickle
-00008e70: 6461 7461 2e31 3430 3531 3339 3733 3831  data.14051397381
-00008e80: 3030 3136 2e73 6861 315f 5a4e 3573 696d  0016.sha1_ZN5sim
-00008e90: 6261 366d 6978 696e 7332 3466 6561 7475  ba6mixins24featu
-00008ea0: 7265 5f65 7874 7261 6374 696f 6e5f 6d69  re_extraction_mi
-00008eb0: 7869 6e32 3246 6561 7475 7265 4578 7472  xin22FeatureExtr
-00008ec0: 6163 7469 6f6e 4d69 7869 6e31 3063 6469  actionMixin10cdi
-00008ed0: 7374 2432 3435 3545 3541 7272 6179 4964  st$2455E5ArrayId
-00008ee0: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
-00008ef0: 6c69 676e 6564 4535 4172 7261 7949 644c  lignedE5ArrayIdL
-00008f00: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
-00008f10: 6967 6e65 6445 6c6c 766d 2e73 6d75 6c2e  ignedEllvm.smul.
-00008f20: 7769 7468 2e6f 7665 7266 6c6f 772e 6936  with.overflow.i6
-00008f30: 344e 5254 5f4d 656d 496e 666f 5f61 6c6c  4NRT_MemInfo_all
-00008f40: 6f63 5f73 6166 655f 616c 6967 6e65 645f  oc_safe_aligned_
-00008f50: 5a4e 3763 7079 7468 6f6e 3573 696d 6261  ZN7cpython5simba
-00008f60: 366d 6978 696e 7332 3466 6561 7475 7265  6mixins24feature
-00008f70: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
-00008f80: 6e32 3246 6561 7475 7265 4578 7472 6163  n22FeatureExtrac
-00008f90: 7469 6f6e 4d69 7869 6e31 3063 6469 7374  tionMixin10cdist
-00008fa0: 2432 3435 3545 3541 7272 6179 4964 4c69  $2455E5ArrayIdLi
-00008fb0: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
-00008fc0: 676e 6564 4535 4172 7261 7949 644c 6932  gnedE5ArrayIdLi2
-00008fd0: 4531 4137 6d75 7461 626c 6537 616c 6967  E1A7mutable7alig
-00008fe0: 6e65 6445 5079 4172 675f 556e 7061 636b  nedEPyArg_Unpack
-00008ff0: 5475 706c 6550 7945 7272 5f53 6574 5374  TuplePyErr_SetSt
-00009000: 7269 6e67 4e52 545f 6164 6170 745f 6e64  ringNRT_adapt_nd
-00009010: 6172 7261 795f 6672 6f6d 5f70 7974 686f  array_from_pytho
-00009020: 6e50 795f 496e 6352 6566 5079 4c69 7374  nPy_IncRefPyList
-00009030: 5f47 6574 4974 656d 4e52 545f 6164 6170  _GetItemNRT_adap
-00009040: 745f 6e64 6172 7261 795f 746f 5f70 7974  t_ndarray_to_pyt
-00009050: 686f 6e5f 6163 7172 6566 5079 4572 725f  hon_acqrefPyErr_
-00009060: 436c 6561 726e 756d 6261 5f75 6e70 6963  Clearnumba_unpic
-00009070: 6b6c 656e 756d 6261 5f64 6f5f 7261 6973  klenumba_do_rais
-00009080: 6550 7945 7272 5f53 6574 4e6f 6e65 6366  ePyErr_SetNonecf
-00009090: 756e 632e 5f5a 4e35 7369 6d62 6136 6d69  unc._ZN5simba6mi
-000090a0: 7869 6e73 3234 6665 6174 7572 655f 6578  xins24feature_ex
-000090b0: 7472 6163 7469 6f6e 5f6d 6978 696e 3232  traction_mixin22
-000090c0: 4665 6174 7572 6545 7874 7261 6374 696f  FeatureExtractio
-000090d0: 6e4d 6978 696e 3130 6364 6973 7424 3234  nMixin10cdist$24
-000090e0: 3535 4535 4172 7261 7949 644c 6932 4531  55E5ArrayIdLi2E1
-000090f0: 4137 6d75 7461 626c 6537 616c 6967 6e65  A7mutable7aligne
-00009100: 6445 3541 7272 6179 4964 4c69 3245 3141  dE5ArrayIdLi2E1A
-00009110: 376d 7574 6162 6c65 3761 6c69 676e 6564  7mutable7aligned
-00009120: 456e 756d 6261 5f67 696c 5f65 6e73 7572  Enumba_gil_ensur
-00009130: 6550 7955 6e69 636f 6465 5f46 726f 6d53  ePyUnicode_FromS
-00009140: 7472 696e 6750 7945 7272 5f57 7269 7465  tringPyErr_Write
-00009150: 556e 7261 6973 6162 6c65 5079 5f44 6563  UnraisablePy_Dec
-00009160: 5265 666e 756d 6261 5f67 696c 5f72 656c  Refnumba_gil_rel
-00009170: 6561 7365 5f5a 4e35 6e75 6d62 6132 6e70  ease_ZN5numba2np
-00009180: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
-00009190: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
-000091a0: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
-000091b0: 3238 4535 4172 7261 7949 644c 6931 4531  28E5ArrayIdLi1E1
-000091c0: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
-000091d0: 6445 4e52 545f 6465 6372 6566 6e75 6d62  dENRT_decrefnumb
-000091e0: 615f 6661 7461 6c5f 6572 726f 726e 756d  a_fatal_errornum
-000091f0: 6261 5f78 786e 726d 322e 6474 6f72 2e6c  ba_xxnrm2.dtor.l
-00009200: 6973 742e 696e 7436 344e 5254 5f4d 656d  ist.int64NRT_Mem
-00009210: 496e 666f 5f6e 6577 5f76 6172 7369 7a65  Info_new_varsize
-00009220: 5f64 746f 726c 6c76 6d2e 6d65 6d73 6574  _dtorllvm.memset
-00009230: 2e70 3069 382e 6936 344e 5254 5f4d 656d  .p0i8.i64NRT_Mem
-00009240: 496e 666f 5f63 616c 6c5f 6474 6f72 4e52  Info_call_dtorNR
-00009250: 545f 696e 6372 6566 6c6c 766d 2e6c 6966  T_increfllvm.lif
-00009260: 6574 696d 652e 7374 6172 742e 7030 6938  etime.start.p0i8
-00009270: 6c6c 766d 2e6c 6966 6574 696d 652e 656e  llvm.lifetime.en
-00009280: 642e 7030 6938 6c6c 766d 2e73 7461 636b  d.p0i8llvm.stack
-00009290: 7072 6f74 6563 746f 7231 302e 302e 3178  protector10.0.1x
-000092a0: 3836 5f36 342d 6170 706c 652d 6461 7277  86_64-apple-darw
-000092b0: 696e 3139 2e36 2e30 3c73 7472 696e 673e  in19.6.0<string>
-000092c0: 5f5f 5a4e 3573 696d 6261 366d 6978 696e  __ZN5simba6mixin
-000092d0: 7332 3466 6561 7475 7265 5f65 7874 7261  s24feature_extra
-000092e0: 6374 696f 6e5f 6d69 7869 6e32 3246 6561  ction_mixin22Fea
-000092f0: 7475 7265 4578 7472 6163 7469 6f6e 4d69  tureExtractionMi
-00009300: 7869 6e31 3063 6469 7374 2432 3435 3545  xin10cdist$2455E
-00009310: 3541 7272 6179 4964 4c69 3245 3141 376d  5ArrayIdLi2E1A7m
-00009320: 7574 6162 6c65 3761 6c69 676e 6564 4535  utable7alignedE5
-00009330: 4172 7261 7949 644c 6932 4531 4137 6d75  ArrayIdLi2E1A7mu
-00009340: 7461 626c 6537 616c 6967 6e65 6445 5f6c  table7alignedE_l
-00009350: 6c76 6d2e 736d 756c 2e77 6974 682e 6f76  lvm.smul.with.ov
-00009360: 6572 666c 6f77 2e69 3634 5f4e 5254 5f4d  erflow.i64_NRT_M
-00009370: 656d 496e 666f 5f61 6c6c 6f63 5f73 6166  emInfo_alloc_saf
-00009380: 655f 616c 6967 6e65 645f 5f5a 4e37 6370  e_aligned__ZN7cp
-00009390: 7974 686f 6e35 7369 6d62 6136 6d69 7869  ython5simba6mixi
-000093a0: 6e73 3234 6665 6174 7572 655f 6578 7472  ns24feature_extr
-000093b0: 6163 7469 6f6e 5f6d 6978 696e 3232 4665  action_mixin22Fe
-000093c0: 6174 7572 6545 7874 7261 6374 696f 6e4d  atureExtractionM
-000093d0: 6978 696e 3130 6364 6973 7424 3234 3535  ixin10cdist$2455
-000093e0: 4535 4172 7261 7949 644c 6932 4531 4137  E5ArrayIdLi2E1A7
-000093f0: 6d75 7461 626c 6537 616c 6967 6e65 6445  mutable7alignedE
-00009400: 3541 7272 6179 4964 4c69 3245 3141 376d  5ArrayIdLi2E1A7m
-00009410: 7574 6162 6c65 3761 6c69 676e 6564 455f  utable7alignedE_
-00009420: 5079 4172 675f 556e 7061 636b 5475 706c  PyArg_UnpackTupl
-00009430: 655f 5079 4572 725f 5365 7453 7472 696e  e_PyErr_SetStrin
-00009440: 675f 4e52 545f 6164 6170 745f 6e64 6172  g_NRT_adapt_ndar
-00009450: 7261 795f 6672 6f6d 5f70 7974 686f 6e5f  ray_from_python_
-00009460: 5079 5f49 6e63 5265 665f 5079 4c69 7374  Py_IncRef_PyList
-00009470: 5f47 6574 4974 656d 5f4e 5254 5f61 6461  _GetItem_NRT_ada
-00009480: 7074 5f6e 6461 7272 6179 5f74 6f5f 7079  pt_ndarray_to_py
-00009490: 7468 6f6e 5f61 6371 7265 665f 5079 4572  thon_acqref_PyEr
-000094a0: 725f 436c 6561 725f 6e75 6d62 615f 756e  r_Clear_numba_un
-000094b0: 7069 636b 6c65 5f6e 756d 6261 5f64 6f5f  pickle_numba_do_
-000094c0: 7261 6973 655f 5079 4572 725f 5365 744e  raise_PyErr_SetN
-000094d0: 6f6e 655f 6366 756e 632e 5f5a 4e35 7369  one_cfunc._ZN5si
-000094e0: 6d62 6136 6d69 7869 6e73 3234 6665 6174  mba6mixins24feat
-000094f0: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
-00009500: 6978 696e 3232 4665 6174 7572 6545 7874  ixin22FeatureExt
-00009510: 7261 6374 696f 6e4d 6978 696e 3130 6364  ractionMixin10cd
-00009520: 6973 7424 3234 3535 4535 4172 7261 7949  ist$2455E5ArrayI
-00009530: 644c 6932 4531 4137 6d75 7461 626c 6537  dLi2E1A7mutable7
-00009540: 616c 6967 6e65 6445 3541 7272 6179 4964  alignedE5ArrayId
-00009550: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
-00009560: 6c69 676e 6564 455f 6e75 6d62 615f 6769  lignedE_numba_gi
-00009570: 6c5f 656e 7375 7265 5f50 7955 6e69 636f  l_ensure_PyUnico
-00009580: 6465 5f46 726f 6d53 7472 696e 675f 5079  de_FromString_Py
-00009590: 4572 725f 5772 6974 6555 6e72 6169 7361  Err_WriteUnraisa
-000095a0: 626c 655f 5079 5f44 6563 5265 665f 6e75  ble_Py_DecRef_nu
-000095b0: 6d62 615f 6769 6c5f 7265 6c65 6173 655f  mba_gil_release_
-000095c0: 5f5a 4e35 6e75 6d62 6132 6e70 366c 696e  _ZN5numba2np6lin
-000095d0: 616c 6731 375f 6f6e 6544 5f6e 6f72 6d5f  alg17_oneD_norm_
-000095e0: 325f 696d 706c 3132 2433 636c 6f63 616c  2_impl12$3clocal
-000095f0: 7324 3365 3969 6d70 6c24 3234 3238 4535  s$3e9impl$2428E5
-00009600: 4172 7261 7949 644c 6931 4531 4337 6d75  ArrayIdLi1E1C7mu
-00009610: 7461 626c 6537 616c 6967 6e65 6445 5f4e  table7alignedE_N
-00009620: 5254 5f64 6563 7265 665f 6e75 6d62 615f  RT_decref_numba_
-00009630: 6661 7461 6c5f 6572 726f 725f 6e75 6d62  fatal_error_numb
-00009640: 615f 7878 6e72 6d32 5f2e 6474 6f72 2e6c  a_xxnrm2_.dtor.l
-00009650: 6973 742e 696e 7436 345f 4e52 545f 4d65  ist.int64_NRT_Me
-00009660: 6d49 6e66 6f5f 6e65 775f 7661 7273 697a  mInfo_new_varsiz
-00009670: 655f 6474 6f72 5f6c 6c76 6d2e 6d65 6d73  e_dtor_llvm.mems
-00009680: 6574 2e70 3069 382e 6936 345f 4e52 545f  et.p0i8.i64_NRT_
-00009690: 4d65 6d49 6e66 6f5f 6361 6c6c 5f64 746f  MemInfo_call_dto
-000096a0: 725f 4e52 545f 696e 6372 6566 5f6c 6c76  r_NRT_incref_llv
-000096b0: 6d2e 6c69 6665 7469 6d65 2e73 7461 7274  m.lifetime.start
-000096c0: 2e70 3069 385f 6c6c 766d 2e6c 6966 6574  .p0i8_llvm.lifet
-000096d0: 696d 652e 656e 642e 7030 6938 5f6c 6c76  ime.end.p0i8_llv
-000096e0: 6d2e 7374 6163 6b70 726f 7465 6374 6f72  m.stackprotector
-000096f0: 5f5f 5a4e 3038 4e75 6d62 6145 6e76 3573  __ZN08NumbaEnv5s
-00009700: 696d 6261 366d 6978 696e 7332 3466 6561  imba6mixins24fea
-00009710: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
-00009720: 6d69 7869 6e32 3246 6561 7475 7265 4578  mixin22FeatureEx
-00009730: 7472 6163 7469 6f6e 4d69 7869 6e31 3063  tractionMixin10c
-00009740: 6469 7374 2432 3435 3545 3541 7272 6179  dist$2455E5Array
-00009750: 4964 4c69 3245 3141 376d 7574 6162 6c65  IdLi2E1A7mutable
-00009760: 3761 6c69 676e 6564 4535 4172 7261 7949  7alignedE5ArrayI
-00009770: 644c 6932 4531 4137 6d75 7461 626c 6537  dLi2E1A7mutable7
-00009780: 616c 6967 6e65 6445 5f2e 636f 6e73 742e  alignedE_.const.
-00009790: 7069 636b 6c65 6275 662e 3134 3035 3133  picklebuf.140513
-000097a0: 3937 3932 3633 3434 385f 2e63 6f6e 7374  979263448_.const
-000097b0: 2e70 6963 6b6c 6562 7566 2e31 3430 3531  .picklebuf.14051
-000097c0: 3339 3638 3332 3739 3932 5f2e 636f 6e73  3968327992_.cons
-000097d0: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
-000097e0: 3531 3339 3638 3332 3739 3932 5f2e 636f  513968327992_.co
-000097f0: 6e73 742e 7069 636b 6c65 6461 7461 2e31  nst.pickledata.1
-00009800: 3430 3531 3339 3638 3332 3739 3932 2e73  40513968327992.s
-00009810: 6861 315f 2e63 6f6e 7374 2e70 6963 6b6c  ha1_.const.pickl
-00009820: 6564 6174 612e 3134 3035 3133 3937 3932  edata.1405139792
-00009830: 3633 3434 385f 2e63 6f6e 7374 2e70 6963  63448_.const.pic
-00009840: 6b6c 6564 6174 612e 3134 3035 3133 3937  kledata.14051397
-00009850: 3932 3633 3434 382e 7368 6131 5f2e 636f  9263448.sha1_.co
-00009860: 6e73 742e 4665 6174 7572 6545 7874 7261  nst.FeatureExtra
-00009870: 6374 696f 6e4d 6978 696e 2e63 6469 7374  ctionMixin.cdist
-00009880: 5f50 7945 7863 5f52 756e 7469 6d65 4572  _PyExc_RuntimeEr
-00009890: 726f 725f 2e63 6f6e 7374 2e6d 6973 7369  ror_.const.missi
-000098a0: 6e67 2045 6e76 6972 6f6e 6d65 6e74 3a20  ng Environment: 
-000098b0: 5f5a 4e30 384e 756d 6261 456e 7635 7369  _ZN08NumbaEnv5si
-000098c0: 6d62 6136 6d69 7869 6e73 3234 6665 6174  mba6mixins24feat
-000098d0: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
-000098e0: 6978 696e 3232 4665 6174 7572 6545 7874  ixin22FeatureExt
-000098f0: 7261 6374 696f 6e4d 6978 696e 3130 6364  ractionMixin10cd
-00009900: 6973 7424 3234 3535 4535 4172 7261 7949  ist$2455E5ArrayI
-00009910: 644c 6932 4531 4137 6d75 7461 626c 6537  dLi2E1A7mutable7
-00009920: 616c 6967 6e65 6445 3541 7272 6179 4964  alignedE5ArrayId
-00009930: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
-00009940: 6c69 676e 6564 455f 5079 4578 635f 5479  lignedE_PyExc_Ty
-00009950: 7065 4572 726f 725f 2e63 6f6e 7374 2e63  peError_.const.c
-00009960: 616e 2774 2075 6e62 6f78 2061 7272 6179  an't unbox array
-00009970: 2066 726f 6d20 5079 4f62 6a65 6374 2069   from PyObject i
-00009980: 6e74 6f20 6e61 7469 7665 2076 616c 7565  nto native value
-00009990: 2e20 2054 6865 206f 626a 6563 7420 6d61  .  The object ma
-000099a0: 7962 6520 6f66 2061 2064 6966 6665 7265  ybe of a differe
-000099b0: 6e74 2074 7970 655f 5f50 795f 4e6f 6e65  nt type__Py_None
-000099c0: 5374 7275 6374 5f2e 636f 6e73 742e 6065  Struct_.const.`e
-000099d0: 6e76 2e63 6f6e 7374 7360 2069 7320 4e55  nv.consts` is NU
-000099e0: 4c4c 2069 6e20 6072 6561 645f 636f 6e73  LL in `read_cons
-000099f0: 7460 5f50 7945 7863 5f53 746f 7049 7465  t`_PyExc_StopIte
-00009a00: 7261 7469 6f6e 5f50 7945 7863 5f53 7973  ration_PyExc_Sys
-00009a10: 7465 6d45 7272 6f72 5f2e 636f 6e73 742e  temError_.const.
-00009a20: 756e 6b6e 6f77 6e20 6572 726f 7220 7768  unknown error wh
-00009a30: 656e 2063 616c 6c69 6e67 206e 6174 6976  en calling nativ
-00009a40: 6520 6675 6e63 7469 6f6e 5f2e 636f 6e73  e function_.cons
-00009a50: 742e 3c6e 756d 6261 2e63 6f72 652e 6370  t.<numba.core.cp
-00009a60: 752e 4350 5543 6f6e 7465 7874 206f 626a  u.CPUContext obj
-00009a70: 6563 7420 6174 2030 7837 6663 6266 3535  ect at 0x7fcbf55
-00009a80: 6164 3230 383e 5f2e 636f 6e73 742e 756e  ad208>_.const.un
-00009a90: 6b6e 6f77 6e20 6572 726f 7220 7768 656e  known error when
-00009aa0: 2063 616c 6c69 6e67 206e 6174 6976 6520   calling native 
-00009ab0: 6675 6e63 7469 6f6e 2e31 5f5f 5a4e 3038  function.1__ZN08
-00009ac0: 4e75 6d62 6145 6e76 356e 756d 6261 326e  NumbaEnv5numba2n
-00009ad0: 7038 6172 7261 796f 626a 3133 6e75 6d70  p8arrayobj13nump
-00009ae0: 795f 6675 6c6c 5f6e 6431 3224 3363 6c6f  y_full_nd12$3clo
-00009af0: 6361 6c73 2433 6539 6675 6c6c 2432 3435  cals$3e9full$245
-00009b00: 3645 3855 6e69 5475 706c 6549 784c 6932  6E8UniTupleIxLi2
-00009b10: 4545 645f 2e63 6f6e 7374 2e70 6963 6b6c  EEd_.const.pickl
-00009b20: 6562 7566 2e31 3430 3531 3339 3633 3036  ebuf.14051396306
-00009b30: 3631 3336 5f2e 636f 6e73 742e 7069 636b  6136_.const.pick
-00009b40: 6c65 6275 662e 3134 3035 3133 3937 3938  lebuf.1405139798
-00009b50: 3032 3533 365f 2e63 6f6e 7374 2e70 6963  02536_.const.pic
-00009b60: 6b6c 6564 6174 612e 3134 3035 3133 3937  kledata.14051397
-00009b70: 3938 3032 3533 365f 2e63 6f6e 7374 2e70  9802536_.const.p
-00009b80: 6963 6b6c 6564 6174 612e 3134 3035 3133  ickledata.140513
-00009b90: 3937 3938 3032 3533 362e 7368 6131 5f2e  979802536.sha1_.
-00009ba0: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
-00009bb0: 2e31 3430 3531 3339 3633 3036 3631 3336  .140513963066136
-00009bc0: 5f2e 636f 6e73 742e 7069 636b 6c65 6461  _.const.pickleda
-00009bd0: 7461 2e31 3430 3531 3339 3633 3036 3631  ta.1405139630661
-00009be0: 3336 2e73 6861 315f 5f5a 4e30 384e 756d  36.sha1__ZN08Num
-00009bf0: 6261 456e 7631 3324 3363 6479 6e61 6d69  baEnv13$3cdynami
-00009c00: 6324 3365 3338 5f5f 6e75 6d62 615f 6172  c$3e38__numba_ar
-00009c10: 7261 795f 6578 7072 5f30 7837 6663 6266  ray_expr_0x7fcbf
-00009c20: 3535 6232 6534 3824 3234 3537 4564 645f  55b2e48$2457Edd_
-00009c30: 5f5a 4e30 384e 756d 6261 456e 7635 6e75  _ZN08NumbaEnv5nu
-00009c40: 6d62 6132 6e70 376e 7079 696d 706c 3230  mba2np7npyimpl20
-00009c50: 5f62 726f 6164 6361 7374 5f6f 6e74 6f24  _broadcast_onto$
-00009c60: 3234 3130 4578 3869 6e74 3634 2432 6178  2410Ex8int64$2ax
-00009c70: 3869 6e74 3634 2432 615f 5f5a 4e30 384e  8int64$2a__ZN08N
-00009c80: 756d 6261 456e 7635 6e75 6d62 6132 6e70  umbaEnv5numba2np
-00009c90: 366c 696e 616c 6731 345f 6765 745f 6e6f  6linalg14_get_no
-00009ca0: 726d 5f69 6d70 6c31 3224 3363 6c6f 6361  rm_impl12$3cloca
-00009cb0: 6c73 2433 6531 346f 6e65 445f 696d 706c  ls$3e14oneD_impl
-00009cc0: 2432 3432 3745 3541 7272 6179 4964 4c69  $2427E5ArrayIdLi
-00009cd0: 3145 3143 376d 7574 6162 6c65 3761 6c69  1E1C7mutable7ali
-00009ce0: 676e 6564 4532 376f 6d69 7474 6564 2432  gnedE27omitted$2
-00009cf0: 3864 6566 6175 6c74 2433 644e 6f6e 6524  8default$3dNone$
-00009d00: 3239 5f5f 5a4e 3038 4e75 6d62 6145 6e76  29__ZN08NumbaEnv
-00009d10: 356e 756d 6261 326e 7036 6c69 6e61 6c67  5numba2np6linalg
-00009d20: 3137 5f6f 6e65 445f 6e6f 726d 5f32 5f69  17_oneD_norm_2_i
-00009d30: 6d70 6c31 3224 3363 6c6f 6361 6c73 2433  mpl12$3clocals$3
-00009d40: 6539 696d 706c 2432 3432 3845 3541 7272  e9impl$2428E5Arr
-00009d50: 6179 4964 4c69 3145 3143 376d 7574 6162  ayIdLi1E1C7mutab
-00009d60: 6c65 3761 6c69 676e 6564 455f 5f5a 4e30  le7alignedE__ZN0
-00009d70: 384e 756d 6261 456e 7635 6e75 6d62 6132  8NumbaEnv5numba2
-00009d80: 6e70 366c 696e 616c 6732 355f 6475 6d6d  np6linalg25_dumm
-00009d90: 795f 6c69 7665 6e65 7373 5f66 756e 6324  y_liveness_func$
-00009da0: 3234 3239 4533 306c 6973 7424 3238 696e  2429E30list$28in
-00009db0: 7436 3424 3239 2433 6369 7624 3364 4e6f  t64$29$3civ$3dNo
-00009dc0: 6e65 2433 655f 2e63 6f6e 7374 2e70 6963  ne$3e_.const.pic
-00009dd0: 6b6c 6562 7566 2e31 3430 3531 3339 3733  klebuf.140513973
-00009de0: 3831 3030 3136 5f2e 636f 6e73 742e 7069  810016_.const.pi
-00009df0: 636b 6c65 6275 662e 3134 3035 3133 3936  cklebuf.14051396
-00009e00: 3431 3530 3134 345f 2e63 6f6e 7374 2e70  4150144_.const.p
-00009e10: 6963 6b6c 6562 7566 2e31 3430 3531 3339  icklebuf.1405139
-00009e20: 3638 3839 3230 3838 5f2e 636f 6e73 742e  68892088_.const.
-00009e30: 7069 636b 6c65 6275 662e 3134 3035 3133  picklebuf.140513
-00009e40: 3937 3237 3535 3430 385f 2e63 6f6e 7374  972755408_.const
-00009e50: 2e70 6963 6b6c 6564 6174 612e 3134 3035  .pickledata.1405
-00009e60: 3133 3937 3237 3535 3430 385f 2e63 6f6e  13972755408_.con
-00009e70: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-00009e80: 3035 3133 3937 3237 3535 3430 382e 7368  0513972755408.sh
-00009e90: 6131 5f2e 636f 6e73 742e 7069 636b 6c65  a1_.const.pickle
-00009ea0: 6461 7461 2e31 3430 3531 3339 3638 3839  data.14051396889
-00009eb0: 3230 3838 5f2e 636f 6e73 742e 7069 636b  2088_.const.pick
-00009ec0: 6c65 6461 7461 2e31 3430 3531 3339 3638  ledata.140513968
-00009ed0: 3839 3230 3838 2e73 6861 315f 2e63 6f6e  892088.sha1_.con
-00009ee0: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
-00009ef0: 3035 3133 3936 3431 3530 3134 345f 2e63  0513964150144_.c
-00009f00: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
-00009f10: 3134 3035 3133 3936 3431 3530 3134 342e  140513964150144.
-00009f20: 7368 6131 5f2e 636f 6e73 742e 7069 636b  sha1_.const.pick
-00009f30: 6c65 6461 7461 2e31 3430 3531 3339 3733  ledata.140513973
-00009f40: 3831 3030 3136 5f2e 636f 6e73 742e 7069  810016_.const.pi
-00009f50: 636b 6c65 6461 7461 2e31 3430 3531 3339  ckledata.1405139
-00009f60: 3733 3831 3030 3136 2e73 6861 3100 0000  73810016.sha1...
-00009f70: 0000 0000 0000 0094 8694 8794 8c13 6e75  ..............nu
-00009f80: 6d62 612e 636f 7265 2e66 756e 6364 6573  mba.core.funcdes
-00009f90: 6394 8c18 5079 7468 6f6e 4675 6e63 7469  c...PythonFuncti
-00009fa0: 6f6e 4465 7363 7269 7074 6f72 9493 9429  onDescriptor...)
-00009fb0: 8194 4e7d 9428 8c06 6e61 7469 7665 9488  ..N}.(..native..
-00009fc0: 8c07 6d6f 646e 616d 6594 8c25 7369 6d62  ..modname..%simb
-00009fd0: 612e 6d69 7869 6e73 2e66 6561 7475 7265  a.mixins.feature
-00009fe0: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
-00009ff0: 6e94 8c08 7175 616c 6e61 6d65 9468 008c  n...qualname.h..
-0000a000: 0364 6f63 948c 0094 8c07 7479 7065 6d61  .doc......typema
-0000a010: 7094 4e8c 0963 616c 6c74 7970 6573 944e  p.N..calltypes.N
-0000a020: 8c04 6172 6773 948c 0761 7272 6179 5f31  ..args...array_1
-0000a030: 948c 0761 7272 6179 5f32 9486 948c 036b  ...array_2.....k
-0000a040: 7773 9429 8c07 7265 7374 7970 6594 8c19  ws.)..restype...
-0000a050: 6e75 6d62 612e 636f 7265 2e74 7970 6573  numba.core.types
-0000a060: 2e61 6273 7472 6163 7494 8c13 5f74 7970  .abstract..._typ
-0000a070: 655f 7265 636f 6e73 7472 7563 746f 7294  e_reconstructor.
-0000a080: 9394 8c07 636f 7079 7265 6794 8c0e 5f72  ....copyreg..._r
-0000a090: 6563 6f6e 7374 7275 6374 6f72 9493 948c  econstructor....
-0000a0a0: 196e 756d 6261 2e63 6f72 652e 7479 7065  .numba.core.type
-0000a0b0: 732e 6e70 7974 7970 6573 948c 0541 7272  s.npytypes...Arr
-0000a0c0: 6179 9493 948c 0862 7569 6c74 696e 7394  ay.....builtins.
-0000a0d0: 8c06 6f62 6a65 6374 9493 944e 8794 7d94  ..object...N..}.
-0000a0e0: 288c 0564 7479 7065 9468 1b68 1e8c 186e  (..dtype.h.h...n
-0000a0f0: 756d 6261 2e63 6f72 652e 7479 7065 732e  umba.core.types.
-0000a100: 7363 616c 6172 7394 8c05 466c 6f61 7494  scalars...Float.
-0000a110: 9394 6824 4e87 947d 9428 8c04 6e61 6d65  ..h$N..}.(..name
-0000a120: 948c 0766 6c6f 6174 3634 948c 0862 6974  ...float64...bit
-0000a130: 7769 6474 6894 4b40 8c05 5f63 6f64 6594  width.K@.._code.
-0000a140: 4b17 7587 9452 948c 046e 6469 6d94 4b02  K.u..R...ndim.K.
-0000a150: 8c06 6c61 796f 7574 948c 0143 9468 2d8c  ..layout...C.h-.
-0000a160: 1561 7272 6179 2866 6c6f 6174 3634 2c20  .array(float64, 
-0000a170: 3264 2c20 4329 9468 304d bc05 7587 9452  2d, C).h0M..u..R
-0000a180: 948c 0861 7267 7479 7065 7394 681b 681e  ...argtypes.h.h.
-0000a190: 6821 6824 4e87 947d 9428 6827 6832 6833  h!h$N..}.(h'h2h3
-0000a1a0: 4b02 6834 8c01 4194 682d 8c15 6172 7261  K.h4..A.h-..arra
-0000a1b0: 7928 666c 6f61 7436 342c 2032 642c 2041  y(float64, 2d, A
-0000a1c0: 2994 6830 4df7 0375 8794 5294 683f 8694  ).h0M..u..R.h?..
-0000a1d0: 8c0c 6d61 6e67 6c65 645f 6e61 6d65 948c  ..mangled_name..
-0000a1e0: 8d5f 5a4e 3573 696d 6261 366d 6978 696e  ._ZN5simba6mixin
-0000a1f0: 7332 3466 6561 7475 7265 5f65 7874 7261  s24feature_extra
-0000a200: 6374 696f 6e5f 6d69 7869 6e32 3246 6561  ction_mixin22Fea
-0000a210: 7475 7265 4578 7472 6163 7469 6f6e 4d69  tureExtractionMi
-0000a220: 7869 6e31 3063 6469 7374 2432 3435 3545  xin10cdist$2455E
-0000a230: 3541 7272 6179 4964 4c69 3245 3141 376d  5ArrayIdLi2E1A7m
-0000a240: 7574 6162 6c65 3761 6c69 676e 6564 4535  utable7alignedE5
-0000a250: 4172 7261 7949 644c 6932 4531 4137 6d75  ArrayIdLi2E1A7mu
-0000a260: 7461 626c 6537 616c 6967 6e65 6445 948c  table7alignedE..
-0000a270: 0b75 6e69 7175 655f 6e61 6d65 948c 1f46  .unique_name...F
-0000a280: 6561 7475 7265 4578 7472 6163 7469 6f6e  eatureExtraction
-0000a290: 4d69 7869 6e2e 6364 6973 7424 3535 948c  Mixin.cdist$55..
-0000a2a0: 0865 6e76 5f6e 616d 6594 8c97 5f5a 4e30  .env_name..._ZN0
-0000a2b0: 384e 756d 6261 456e 7635 7369 6d62 6136  8NumbaEnv5simba6
-0000a2c0: 6d69 7869 6e73 3234 6665 6174 7572 655f  mixins24feature_
-0000a2d0: 6578 7472 6163 7469 6f6e 5f6d 6978 696e  extraction_mixin
-0000a2e0: 3232 4665 6174 7572 6545 7874 7261 6374  22FeatureExtract
-0000a2f0: 696f 6e4d 6978 696e 3130 6364 6973 7424  ionMixin10cdist$
-0000a300: 3234 3535 4535 4172 7261 7949 644c 6932  2455E5ArrayIdLi2
-0000a310: 4531 4137 6d75 7461 626c 6537 616c 6967  E1A7mutable7alig
-0000a320: 6e65 6445 3541 7272 6179 4964 4c69 3245  nedE5ArrayIdLi2E
-0000a330: 3141 376d 7574 6162 6c65 3761 6c69 676e  1A7mutable7align
-0000a340: 6564 4594 8c0b 676c 6f62 616c 5f64 6963  edE...global_dic
-0000a350: 7494 4e8c 0669 6e6c 696e 6594 898c 076e  t.N..inline....n
-0000a360: 6f61 6c69 6173 9489 7586 9462 8c16 6e75  oalias..u..b..nu
-0000a370: 6d62 612e 636f 7265 2e65 6e76 6972 6f6e  mba.core.environ
-0000a380: 6d65 6e74 948c 0c5f 7265 6275 696c 645f  ment..._rebuild_
-0000a390: 656e 7694 9394 680d 5d94 8c05 6e75 6d70  env...h.]...nump
-0000a3a0: 7994 8c05 6474 7970 6594 9394 8c02 6638  y...dtype.....f8
-0000a3b0: 9489 8887 9452 9428 4b03 8c01 3c94 4e4e  .....R.(K...<.NN
-0000a3c0: 4e4a ffff ffff 4aff ffff ff4b 0074 9462  NJ....J....K.t.b
-0000a3d0: 6168 4687 9452 948c 1b6e 756d 6261 2e63  ahF..R...numba.c
-0000a3e0: 6f72 652e 7479 7069 6e67 2e74 656d 706c  ore.typing.templ
-0000a3f0: 6174 6573 948c 0953 6967 6e61 7475 7265  ates...Signature
-0000a400: 9493 9429 8194 2868 3868 3f68 3f86 944e  ...)..(h8h?h?..N
-0000a410: 4e74 9462 8929 5862 1c00 0023 2046 696c  Nt.b.)Xb...# Fil
-0000a420: 653a 202f 5573 6572 732f 7369 6d6f 6e2f  e: /Users/simon/
-0000a430: 4465 736b 746f 702f 656e 7673 2f73 696d  Desktop/envs/sim
-0000a440: 6261 5f64 6576 2f73 696d 6261 2f6d 6978  ba_dev/simba/mix
-0000a450: 696e 732f 6665 6174 7572 655f 6578 7472  ins/feature_extr
-0000a460: 6163 7469 6f6e 5f6d 6978 696e 2e70 790a  action_mixin.py.
-0000a470: 2320 2d2d 2d20 4c49 4e45 2031 3833 202d  # --- LINE 183 -
-0000a480: 2d2d 200a 0a40 7374 6174 6963 6d65 7468  -- ..@staticmeth
-0000a490: 6f64 0a0a 2320 2d2d 2d20 4c49 4e45 2031  od..# --- LINE 1
-0000a4a0: 3834 202d 2d2d 200a 0a40 6a69 7428 6e6f  84 --- ..@jit(no
-0000a4b0: 7079 7468 6f6e 3d54 7275 652c 2063 6163  python=True, cac
-0000a4c0: 6865 3d54 7275 6529 0a0a 2320 2d2d 2d20  he=True)..# --- 
-0000a4d0: 4c49 4e45 2031 3835 202d 2d2d 200a 0a64  LINE 185 --- ..d
-0000a4e0: 6566 2063 6469 7374 2861 7272 6179 5f31  ef cdist(array_1
-0000a4f0: 3a20 6e70 2e61 7272 6179 2c20 6172 7261  : np.array, arra
-0000a500: 795f 323a 206e 702e 6172 7261 7929 3a0a  y_2: np.array):.
-0000a510: 0a20 2020 2023 202d 2d2d 204c 494e 4520  .    # --- LINE 
-0000a520: 3138 3620 2d2d 2d20 0a20 2020 2023 206c  186 --- .    # l
-0000a530: 6162 656c 2030 0a20 2020 2023 2020 2061  abel 0.    #   a
-0000a540: 7272 6179 5f31 203d 2061 7267 2830 2c20  rray_1 = arg(0, 
-0000a550: 6e61 6d65 3d61 7272 6179 5f31 2920 203a  name=array_1)  :
-0000a560: 3a20 6172 7261 7928 666c 6f61 7436 342c  : array(float64,
-0000a570: 2032 642c 2041 290a 2020 2020 2320 2020   2d, A).    #   
-0000a580: 6172 7261 795f 3220 3d20 6172 6728 312c  array_2 = arg(1,
-0000a590: 206e 616d 653d 6172 7261 795f 3229 2020   name=array_2)  
-0000a5a0: 3a3a 2061 7272 6179 2866 6c6f 6174 3634  :: array(float64
-0000a5b0: 2c20 3264 2c20 4129 0a20 2020 2023 2020  , 2d, A).    #  
-0000a5c0: 2024 302e 3120 3d20 676c 6f62 616c 286e   $0.1 = global(n
-0000a5d0: 703a 203c 6d6f 6475 6c65 2027 6e75 6d70  p: <module 'nump
-0000a5e0: 7927 2066 726f 6d20 272f 5573 6572 732f  y' from '/Users/
-0000a5f0: 7369 6d6f 6e2f 2e63 6f6e 6461 2f65 6e76  simon/.conda/env
-0000a600: 732f 7369 6d62 615f 6465 762f 6c69 622f  s/simba_dev/lib/
-0000a610: 7079 7468 6f6e 332e 362f 7369 7465 2d70  python3.6/site-p
-0000a620: 6163 6b61 6765 732f 6e75 6d70 792f 5f5f  ackages/numpy/__
-0000a630: 696e 6974 5f5f 2e70 7927 3e29 2020 3a3a  init__.py'>)  ::
-0000a640: 204d 6f64 756c 6528 3c6d 6f64 756c 6520   Module(<module 
-0000a650: 276e 756d 7079 2720 6672 6f6d 2027 2f55  'numpy' from '/U
-0000a660: 7365 7273 2f73 696d 6f6e 2f2e 636f 6e64  sers/simon/.cond
-0000a670: 612f 656e 7673 2f73 696d 6261 5f64 6576  a/envs/simba_dev
-0000a680: 2f6c 6962 2f70 7974 686f 6e33 2e36 2f73  /lib/python3.6/s
-0000a690: 6974 652d 7061 636b 6167 6573 2f6e 756d  ite-packages/num
-0000a6a0: 7079 2f5f 5f69 6e69 745f 5f2e 7079 273e  py/__init__.py'>
-0000a6b0: 290a 2020 2020 2320 2020 2430 2e32 203d  ).    #   $0.2 =
-0000a6c0: 2067 6574 6174 7472 2876 616c 7565 3d24   getattr(value=$
-0000a6d0: 302e 312c 2061 7474 723d 6675 6c6c 2920  0.1, attr=full) 
-0000a6e0: 203a 3a20 4675 6e63 7469 6f6e 283c 6675   :: Function(<fu
-0000a6f0: 6e63 7469 6f6e 2066 756c 6c20 6174 2030  nction full at 0
-0000a700: 7837 6663 6265 6638 3961 3266 303e 290a  x7fcbef89a2f0>).
-0000a710: 2020 2020 2320 2020 6465 6c20 2430 2e31      #   del $0.1
-0000a720: 0a20 2020 2023 2020 2024 302e 3420 3d20  .    #   $0.4 = 
-0000a730: 6765 7461 7474 7228 7661 6c75 653d 6172  getattr(value=ar
-0000a740: 7261 795f 312c 2061 7474 723d 7368 6170  ray_1, attr=shap
-0000a750: 6529 2020 3a3a 2055 6e69 5475 706c 6528  e)  :: UniTuple(
-0000a760: 696e 7436 3420 7820 3229 0a20 2020 2023  int64 x 2).    #
-0000a770: 2020 2024 636f 6e73 7430 2e35 203d 2063     $const0.5 = c
-0000a780: 6f6e 7374 2869 6e74 2c20 3029 2020 3a3a  onst(int, 0)  ::
-0000a790: 204c 6974 6572 616c 5b69 6e74 5d28 3029   Literal[int](0)
-0000a7a0: 0a20 2020 2023 2020 2024 302e 3620 3d20  .    #   $0.6 = 
-0000a7b0: 7374 6174 6963 5f67 6574 6974 656d 2876  static_getitem(v
-0000a7c0: 616c 7565 3d24 302e 342c 2069 6e64 6578  alue=$0.4, index
-0000a7d0: 3d30 2c20 696e 6465 785f 7661 723d 2463  =0, index_var=$c
-0000a7e0: 6f6e 7374 302e 352c 2066 6e3d 3c62 7569  onst0.5, fn=<bui
-0000a7f0: 6c74 2d69 6e20 6675 6e63 7469 6f6e 2067  lt-in function g
-0000a800: 6574 6974 656d 3e29 2020 3a3a 2069 6e74  etitem>)  :: int
-0000a810: 3634 0a20 2020 2023 2020 2064 656c 2024  64.    #   del $
-0000a820: 636f 6e73 7430 2e35 0a20 2020 2023 2020  const0.5.    #  
-0000a830: 2064 656c 2024 302e 340a 2020 2020 2320   del $0.4.    # 
-0000a840: 2020 2430 2e38 203d 2067 6574 6174 7472    $0.8 = getattr
-0000a850: 2876 616c 7565 3d61 7272 6179 5f32 2c20  (value=array_2, 
-0000a860: 6174 7472 3d73 6861 7065 2920 203a 3a20  attr=shape)  :: 
-0000a870: 556e 6954 7570 6c65 2869 6e74 3634 2078  UniTuple(int64 x
-0000a880: 2032 290a 2020 2020 2320 2020 2463 6f6e   2).    #   $con
-0000a890: 7374 302e 3920 3d20 636f 6e73 7428 696e  st0.9 = const(in
-0000a8a0: 742c 2030 2920 203a 3a20 4c69 7465 7261  t, 0)  :: Litera
-0000a8b0: 6c5b 696e 745d 2830 290a 2020 2020 2320  l[int](0).    # 
-0000a8c0: 2020 2430 2e31 3020 3d20 7374 6174 6963    $0.10 = static
-0000a8d0: 5f67 6574 6974 656d 2876 616c 7565 3d24  _getitem(value=$
-0000a8e0: 302e 382c 2069 6e64 6578 3d30 2c20 696e  0.8, index=0, in
-0000a8f0: 6465 785f 7661 723d 2463 6f6e 7374 302e  dex_var=$const0.
-0000a900: 392c 2066 6e3d 3c62 7569 6c74 2d69 6e20  9, fn=<built-in 
-0000a910: 6675 6e63 7469 6f6e 2067 6574 6974 656d  function getitem
-0000a920: 3e29 2020 3a3a 2069 6e74 3634 0a20 2020  >)  :: int64.   
-0000a930: 2023 2020 2064 656c 2024 636f 6e73 7430   #   del $const0
-0000a940: 2e39 0a20 2020 2023 2020 2064 656c 2024  .9.    #   del $
-0000a950: 302e 380a 2020 2020 2320 2020 2430 2e31  0.8.    #   $0.1
-0000a960: 3120 3d20 6275 696c 645f 7475 706c 6528  1 = build_tuple(
-0000a970: 6974 656d 733d 5b56 6172 2824 302e 362c  items=[Var($0.6,
-0000a980: 2066 6561 7475 7265 5f65 7874 7261 6374   feature_extract
-0000a990: 696f 6e5f 6d69 7869 6e2e 7079 3a31 3836  ion_mixin.py:186
-0000a9a0: 292c 2056 6172 2824 302e 3130 2c20 6665  ), Var($0.10, fe
-0000a9b0: 6174 7572 655f 6578 7472 6163 7469 6f6e  ature_extraction
-0000a9c0: 5f6d 6978 696e 2e70 793a 3138 3629 5d29  _mixin.py:186)])
-0000a9d0: 2020 3a3a 2055 6e69 5475 706c 6528 696e    :: UniTuple(in
-0000a9e0: 7436 3420 7820 3229 0a20 2020 2023 2020  t64 x 2).    #  
-0000a9f0: 2064 656c 2024 302e 360a 2020 2020 2320   del $0.6.    # 
-0000aa00: 2020 6465 6c20 2430 2e31 300a 2020 2020    del $0.10.    
-0000aa10: 2320 2020 2430 2e31 3220 3d20 676c 6f62  #   $0.12 = glob
-0000aa20: 616c 286e 703a 203c 6d6f 6475 6c65 2027  al(np: <module '
-0000aa30: 6e75 6d70 7927 2066 726f 6d20 272f 5573  numpy' from '/Us
-0000aa40: 6572 732f 7369 6d6f 6e2f 2e63 6f6e 6461  ers/simon/.conda
-0000aa50: 2f65 6e76 732f 7369 6d62 615f 6465 762f  /envs/simba_dev/
-0000aa60: 6c69 622f 7079 7468 6f6e 332e 362f 7369  lib/python3.6/si
-0000aa70: 7465 2d70 6163 6b61 6765 732f 6e75 6d70  te-packages/nump
-0000aa80: 792f 5f5f 696e 6974 5f5f 2e70 7927 3e29  y/__init__.py'>)
-0000aa90: 2020 3a3a 204d 6f64 756c 6528 3c6d 6f64    :: Module(<mod
-0000aaa0: 756c 6520 276e 756d 7079 2720 6672 6f6d  ule 'numpy' from
-0000aab0: 2027 2f55 7365 7273 2f73 696d 6f6e 2f2e   '/Users/simon/.
-0000aac0: 636f 6e64 612f 656e 7673 2f73 696d 6261  conda/envs/simba
-0000aad0: 5f64 6576 2f6c 6962 2f70 7974 686f 6e33  _dev/lib/python3
-0000aae0: 2e36 2f73 6974 652d 7061 636b 6167 6573  .6/site-packages
-0000aaf0: 2f6e 756d 7079 2f5f 5f69 6e69 745f 5f2e  /numpy/__init__.
-0000ab00: 7079 273e 290a 2020 2020 2320 2020 2430  py'>).    #   $0
-0000ab10: 2e31 3320 3d20 6765 7461 7474 7228 7661  .13 = getattr(va
-0000ab20: 6c75 653d 2430 2e31 322c 2061 7474 723d  lue=$0.12, attr=
-0000ab30: 6e61 6e29 2020 3a3a 2066 6c6f 6174 3634  nan)  :: float64
-0000ab40: 0a20 2020 2023 2020 2064 656c 2024 302e  .    #   del $0.
-0000ab50: 3132 0a20 2020 2023 2020 2024 302e 3134  12.    #   $0.14
-0000ab60: 203d 2063 616c 6c20 2430 2e32 2824 302e   = call $0.2($0.
-0000ab70: 3131 2c20 2430 2e31 332c 2066 756e 633d  11, $0.13, func=
-0000ab80: 2430 2e32 2c20 6172 6773 3d5b 5661 7228  $0.2, args=[Var(
-0000ab90: 2430 2e31 312c 2066 6561 7475 7265 5f65  $0.11, feature_e
-0000aba0: 7874 7261 6374 696f 6e5f 6d69 7869 6e2e  xtraction_mixin.
-0000abb0: 7079 3a31 3836 292c 2056 6172 2824 302e  py:186), Var($0.
-0000abc0: 3133 2c20 6665 6174 7572 655f 6578 7472  13, feature_extr
-0000abd0: 6163 7469 6f6e 5f6d 6978 696e 2e70 793a  action_mixin.py:
-0000abe0: 3138 3629 5d2c 206b 7773 3d28 292c 2076  186)], kws=(), v
-0000abf0: 6172 6172 673d 4e6f 6e65 2920 203a 3a20  ararg=None)  :: 
-0000ac00: 2855 6e69 5475 706c 6528 696e 7436 3420  (UniTuple(int64 
-0000ac10: 7820 3229 2c20 666c 6f61 7436 3429 202d  x 2), float64) -
-0000ac20: 3e20 6172 7261 7928 666c 6f61 7436 342c  > array(float64,
-0000ac30: 2032 642c 2043 290a 2020 2020 2320 2020   2d, C).    #   
-0000ac40: 6465 6c20 2430 2e32 0a20 2020 2023 2020  del $0.2.    #  
-0000ac50: 2064 656c 2024 302e 3133 0a20 2020 2023   del $0.13.    #
-0000ac60: 2020 2064 656c 2024 302e 3131 0a20 2020     del $0.11.   
-0000ac70: 2023 2020 2072 6573 756c 7473 203d 2024   #   results = $
-0000ac80: 302e 3134 2020 3a3a 2061 7272 6179 2866  0.14  :: array(f
-0000ac90: 6c6f 6174 3634 2c20 3264 2c20 4329 0a20  loat64, 2d, C). 
-0000aca0: 2020 2023 2020 2064 656c 2024 302e 3134     #   del $0.14
-0000acb0: 0a0a 2020 2020 7265 7375 6c74 7320 3d20  ..    results = 
-0000acc0: 6e70 2e66 756c 6c28 2861 7272 6179 5f31  np.full((array_1
-0000acd0: 2e73 6861 7065 5b30 5d2c 2061 7272 6179  .shape[0], array
-0000ace0: 5f32 2e73 6861 7065 5b30 5d29 2c20 6e70  _2.shape[0]), np
-0000acf0: 2e6e 616e 290a 0a20 2020 2023 202d 2d2d  .nan)..    # ---
-0000ad00: 204c 494e 4520 3138 3720 2d2d 2d20 0a20   LINE 187 --- . 
-0000ad10: 2020 2023 2020 206a 756d 7020 3332 0a20     #   jump 32. 
-0000ad20: 2020 2023 206c 6162 656c 2033 320a 2020     # label 32.  
-0000ad30: 2020 2320 2020 6a75 6d70 2033 340a 2020    #   jump 34.  
-0000ad40: 2020 2320 6c61 6265 6c20 3334 0a20 2020    # label 34.   
-0000ad50: 2023 2020 2024 3334 2e31 203d 2067 6c6f   #   $34.1 = glo
-0000ad60: 6261 6c28 7072 616e 6765 3a20 3c63 6c61  bal(prange: <cla
-0000ad70: 7373 2027 6e75 6d62 612e 6d69 7363 2e73  ss 'numba.misc.s
-0000ad80: 7065 6369 616c 2e70 7261 6e67 6527 3e29  pecial.prange'>)
-0000ad90: 2020 3a3a 2046 756e 6374 696f 6e28 3c63    :: Function(<c
-0000ada0: 6c61 7373 2027 6e75 6d62 612e 6d69 7363  lass 'numba.misc
-0000adb0: 2e73 7065 6369 616c 2e70 7261 6e67 6527  .special.prange'
-0000adc0: 3e29 0a20 2020 2023 2020 2024 3334 2e33  >).    #   $34.3
-0000add0: 203d 2067 6574 6174 7472 2876 616c 7565   = getattr(value
-0000ade0: 3d61 7272 6179 5f31 2c20 6174 7472 3d73  =array_1, attr=s
-0000adf0: 6861 7065 2920 203a 3a20 556e 6954 7570  hape)  :: UniTup
-0000ae00: 6c65 2869 6e74 3634 2078 2032 290a 2020  le(int64 x 2).  
-0000ae10: 2020 2320 2020 2463 6f6e 7374 3334 2e34    #   $const34.4
-0000ae20: 203d 2063 6f6e 7374 2869 6e74 2c20 3029   = const(int, 0)
-0000ae30: 2020 3a3a 204c 6974 6572 616c 5b69 6e74    :: Literal[int
-0000ae40: 5d28 3029 0a20 2020 2023 2020 2024 3334  ](0).    #   $34
-0000ae50: 2e35 203d 2073 7461 7469 635f 6765 7469  .5 = static_geti
-0000ae60: 7465 6d28 7661 6c75 653d 2433 342e 332c  tem(value=$34.3,
-0000ae70: 2069 6e64 6578 3d30 2c20 696e 6465 785f   index=0, index_
-0000ae80: 7661 723d 2463 6f6e 7374 3334 2e34 2c20  var=$const34.4, 
-0000ae90: 666e 3d3c 6275 696c 742d 696e 2066 756e  fn=<built-in fun
-0000aea0: 6374 696f 6e20 6765 7469 7465 6d3e 2920  ction getitem>) 
-0000aeb0: 203a 3a20 696e 7436 340a 2020 2020 2320   :: int64.    # 
-0000aec0: 2020 6465 6c20 2463 6f6e 7374 3334 2e34    del $const34.4
-0000aed0: 0a20 2020 2023 2020 2064 656c 2024 3334  .    #   del $34
-0000aee0: 2e33 0a20 2020 2023 2020 2024 3334 2e36  .3.    #   $34.6
-0000aef0: 203d 2063 616c 6c20 2433 342e 3128 2433   = call $34.1($3
-0000af00: 342e 352c 2066 756e 633d 2433 342e 312c  4.5, func=$34.1,
-0000af10: 2061 7267 733d 5b56 6172 2824 3334 2e35   args=[Var($34.5
-0000af20: 2c20 6665 6174 7572 655f 6578 7472 6163  , feature_extrac
-0000af30: 7469 6f6e 5f6d 6978 696e 2e70 793a 3138  tion_mixin.py:18
-0000af40: 3729 5d2c 206b 7773 3d28 292c 2076 6172  7)], kws=(), var
-0000af50: 6172 673d 4e6f 6e65 2920 203a 3a20 2869  arg=None)  :: (i
-0000af60: 6e74 3634 2c29 202d 3e20 7261 6e67 655f  nt64,) -> range_
-0000af70: 7374 6174 655f 696e 7436 340a 2020 2020  state_int64.    
-0000af80: 2320 2020 6465 6c20 2433 342e 350a 2020  #   del $34.5.  
-0000af90: 2020 2320 2020 6465 6c20 2433 342e 310a    #   del $34.1.
-0000afa0: 2020 2020 2320 2020 2433 342e 3720 3d20      #   $34.7 = 
-0000afb0: 6765 7469 7465 7228 7661 6c75 653d 2433  getiter(value=$3
-0000afc0: 342e 3629 2020 3a3a 2072 616e 6765 5f69  4.6)  :: range_i
-0000afd0: 7465 725f 696e 7436 340a 2020 2020 2320  ter_int64.    # 
-0000afe0: 2020 6465 6c20 2433 342e 360a 2020 2020    del $34.6.    
-0000aff0: 2320 2020 2470 6869 3438 2e31 203d 2024  #   $phi48.1 = $
-0000b000: 3334 2e37 2020 3a3a 2072 616e 6765 5f69  34.7  :: range_i
-0000b010: 7465 725f 696e 7436 340a 2020 2020 2320  ter_int64.    # 
-0000b020: 2020 6465 6c20 2433 342e 370a 2020 2020    del $34.7.    
-0000b030: 2320 2020 6a75 6d70 2034 380a 2020 2020  #   jump 48.    
-0000b040: 2320 6c61 6265 6c20 3438 0a20 2020 2023  # label 48.    #
-0000b050: 2020 2024 3438 2e32 203d 2069 7465 726e     $48.2 = itern
-0000b060: 6578 7428 7661 6c75 653d 2470 6869 3438  ext(value=$phi48
-0000b070: 2e31 2920 203a 3a20 7061 6972 3c69 6e74  .1)  :: pair<int
-0000b080: 3634 2c20 626f 6f6c 3e0a 2020 2020 2320  64, bool>.    # 
-0000b090: 2020 2434 382e 3320 3d20 7061 6972 5f66    $48.3 = pair_f
-0000b0a0: 6972 7374 2876 616c 7565 3d24 3438 2e32  irst(value=$48.2
-0000b0b0: 2920 203a 3a20 696e 7436 340a 2020 2020  )  :: int64.    
-0000b0c0: 2320 2020 2434 382e 3420 3d20 7061 6972  #   $48.4 = pair
-0000b0d0: 5f73 6563 6f6e 6428 7661 6c75 653d 2434  _second(value=$4
-0000b0e0: 382e 3229 2020 3a3a 2062 6f6f 6c0a 2020  8.2)  :: bool.  
-0000b0f0: 2020 2320 2020 6465 6c20 2434 382e 320a    #   del $48.2.
-0000b100: 2020 2020 2320 2020 2470 6869 3530 2e31      #   $phi50.1
-0000b110: 203d 2024 3438 2e33 2020 3a3a 2069 6e74   = $48.3  :: int
-0000b120: 3634 0a20 2020 2023 2020 2024 7068 6931  64.    #   $phi1
-0000b130: 3130 2e31 203d 2024 3438 2e33 2020 3a3a  10.1 = $48.3  ::
-0000b140: 2069 6e74 3634 0a20 2020 2023 2020 2064   int64.    #   d
-0000b150: 656c 2024 7068 6931 3130 2e31 0a20 2020  el $phi110.1.   
-0000b160: 2023 2020 2064 656c 2024 3438 2e33 0a20   #   del $48.3. 
-0000b170: 2020 2023 2020 2024 7068 6931 3130 2e32     #   $phi110.2
-0000b180: 203d 2024 7068 6934 382e 3120 203a 3a20   = $phi48.1  :: 
-0000b190: 7261 6e67 655f 6974 6572 5f69 6e74 3634  range_iter_int64
-0000b1a0: 0a20 2020 2023 2020 2064 656c 2024 7068  .    #   del $ph
-0000b1b0: 6931 3130 2e32 0a20 2020 2023 2020 2062  i110.2.    #   b
-0000b1c0: 7261 6e63 6820 2434 382e 342c 2035 302c  ranch $48.4, 50,
-0000b1d0: 2031 3130 0a20 2020 2023 206c 6162 656c   110.    # label
-0000b1e0: 2035 300a 2020 2020 2320 2020 6465 6c20   50.    #   del 
-0000b1f0: 2434 382e 340a 2020 2020 2320 2020 6920  $48.4.    #   i 
-0000b200: 3d20 2470 6869 3530 2e31 2020 3a3a 2069  = $phi50.1  :: i
-0000b210: 6e74 3634 0a20 2020 2023 2020 2064 656c  nt64.    #   del
-0000b220: 2024 7068 6935 302e 310a 0a20 2020 2066   $phi50.1..    f
-0000b230: 6f72 2069 2069 6e20 7072 616e 6765 2861  or i in prange(a
-0000b240: 7272 6179 5f31 2e73 6861 7065 5b30 5d29  rray_1.shape[0])
-0000b250: 3a0a 0a20 2020 2020 2020 2023 202d 2d2d  :..        # ---
-0000b260: 204c 494e 4520 3138 3820 2d2d 2d20 0a20   LINE 188 --- . 
-0000b270: 2020 2020 2020 2023 2020 206a 756d 7020         #   jump 
-0000b280: 3532 0a20 2020 2020 2020 2023 206c 6162  52.        # lab
-0000b290: 656c 2035 320a 2020 2020 2020 2020 2320  el 52.        # 
-0000b2a0: 2020 6a75 6d70 2035 340a 2020 2020 2020    jump 54.      
-0000b2b0: 2020 2320 6c61 6265 6c20 3534 0a20 2020    # label 54.   
-0000b2c0: 2020 2020 2023 2020 2024 3534 2e31 203d       #   $54.1 =
-0000b2d0: 2067 6c6f 6261 6c28 7072 616e 6765 3a20   global(prange: 
-0000b2e0: 3c63 6c61 7373 2027 6e75 6d62 612e 6d69  <class 'numba.mi
-0000b2f0: 7363 2e73 7065 6369 616c 2e70 7261 6e67  sc.special.prang
-0000b300: 6527 3e29 2020 3a3a 2046 756e 6374 696f  e'>)  :: Functio
-0000b310: 6e28 3c63 6c61 7373 2027 6e75 6d62 612e  n(<class 'numba.
-0000b320: 6d69 7363 2e73 7065 6369 616c 2e70 7261  misc.special.pra
-0000b330: 6e67 6527 3e29 0a20 2020 2020 2020 2023  nge'>).        #
-0000b340: 2020 2024 3534 2e33 203d 2067 6574 6174     $54.3 = getat
-0000b350: 7472 2876 616c 7565 3d61 7272 6179 5f32  tr(value=array_2
-0000b360: 2c20 6174 7472 3d73 6861 7065 2920 203a  , attr=shape)  :
-0000b370: 3a20 556e 6954 7570 6c65 2869 6e74 3634  : UniTuple(int64
-0000b380: 2078 2032 290a 2020 2020 2020 2020 2320   x 2).        # 
-0000b390: 2020 2463 6f6e 7374 3534 2e34 203d 2063    $const54.4 = c
-0000b3a0: 6f6e 7374 2869 6e74 2c20 3029 2020 3a3a  onst(int, 0)  ::
-0000b3b0: 204c 6974 6572 616c 5b69 6e74 5d28 3029   Literal[int](0)
-0000b3c0: 0a20 2020 2020 2020 2023 2020 2024 3534  .        #   $54
-0000b3d0: 2e35 203d 2073 7461 7469 635f 6765 7469  .5 = static_geti
-0000b3e0: 7465 6d28 7661 6c75 653d 2435 342e 332c  tem(value=$54.3,
-0000b3f0: 2069 6e64 6578 3d30 2c20 696e 6465 785f   index=0, index_
-0000b400: 7661 723d 2463 6f6e 7374 3534 2e34 2c20  var=$const54.4, 
-0000b410: 666e 3d3c 6275 696c 742d 696e 2066 756e  fn=<built-in fun
-0000b420: 6374 696f 6e20 6765 7469 7465 6d3e 2920  ction getitem>) 
-0000b430: 203a 3a20 696e 7436 340a 2020 2020 2020   :: int64.      
-0000b440: 2020 2320 2020 6465 6c20 2463 6f6e 7374    #   del $const
-0000b450: 3534 2e34 0a20 2020 2020 2020 2023 2020  54.4.        #  
-0000b460: 2064 656c 2024 3534 2e33 0a20 2020 2020   del $54.3.     
-0000b470: 2020 2023 2020 2024 3534 2e36 203d 2063     #   $54.6 = c
-0000b480: 616c 6c20 2435 342e 3128 2435 342e 352c  all $54.1($54.5,
-0000b490: 2066 756e 633d 2435 342e 312c 2061 7267   func=$54.1, arg
-0000b4a0: 733d 5b56 6172 2824 3534 2e35 2c20 6665  s=[Var($54.5, fe
-0000b4b0: 6174 7572 655f 6578 7472 6163 7469 6f6e  ature_extraction
-0000b4c0: 5f6d 6978 696e 2e70 793a 3138 3829 5d2c  _mixin.py:188)],
-0000b4d0: 206b 7773 3d28 292c 2076 6172 6172 673d   kws=(), vararg=
-0000b4e0: 4e6f 6e65 2920 203a 3a20 2869 6e74 3634  None)  :: (int64
-0000b4f0: 2c29 202d 3e20 7261 6e67 655f 7374 6174  ,) -> range_stat
-0000b500: 655f 696e 7436 340a 2020 2020 2020 2020  e_int64.        
-0000b510: 2320 2020 6465 6c20 2435 342e 350a 2020  #   del $54.5.  
-0000b520: 2020 2020 2020 2320 2020 6465 6c20 2435        #   del $5
-0000b530: 342e 310a 2020 2020 2020 2020 2320 2020  4.1.        #   
-0000b540: 2435 342e 3720 3d20 6765 7469 7465 7228  $54.7 = getiter(
-0000b550: 7661 6c75 653d 2435 342e 3629 2020 3a3a  value=$54.6)  ::
-0000b560: 2072 616e 6765 5f69 7465 725f 696e 7436   range_iter_int6
-0000b570: 340a 2020 2020 2020 2020 2320 2020 6465  4.        #   de
-0000b580: 6c20 2435 342e 360a 2020 2020 2020 2020  l $54.6.        
-0000b590: 2320 2020 2470 6869 3638 2e31 203d 2024  #   $phi68.1 = $
-0000b5a0: 3534 2e37 2020 3a3a 2072 616e 6765 5f69  54.7  :: range_i
-0000b5b0: 7465 725f 696e 7436 340a 2020 2020 2020  ter_int64.      
-0000b5c0: 2020 2320 2020 6465 6c20 2435 342e 370a    #   del $54.7.
-0000b5d0: 2020 2020 2020 2020 2320 2020 6a75 6d70          #   jump
-0000b5e0: 2036 380a 2020 2020 2020 2020 2320 6c61   68.        # la
-0000b5f0: 6265 6c20 3638 0a20 2020 2020 2020 2023  bel 68.        #
-0000b600: 2020 2024 3638 2e32 203d 2069 7465 726e     $68.2 = itern
-0000b610: 6578 7428 7661 6c75 653d 2470 6869 3638  ext(value=$phi68
-0000b620: 2e31 2920 203a 3a20 7061 6972 3c69 6e74  .1)  :: pair<int
-0000b630: 3634 2c20 626f 6f6c 3e0a 2020 2020 2020  64, bool>.      
-0000b640: 2020 2320 2020 2436 382e 3320 3d20 7061    #   $68.3 = pa
-0000b650: 6972 5f66 6972 7374 2876 616c 7565 3d24  ir_first(value=$
-0000b660: 3638 2e32 2920 203a 3a20 696e 7436 340a  68.2)  :: int64.
-0000b670: 2020 2020 2020 2020 2320 2020 2436 382e          #   $68.
-0000b680: 3420 3d20 7061 6972 5f73 6563 6f6e 6428  4 = pair_second(
-0000b690: 7661 6c75 653d 2436 382e 3229 2020 3a3a  value=$68.2)  ::
-0000b6a0: 2062 6f6f 6c0a 2020 2020 2020 2020 2320   bool.        # 
-0000b6b0: 2020 6465 6c20 2436 382e 320a 2020 2020    del $68.2.    
-0000b6c0: 2020 2020 2320 2020 2470 6869 3730 2e31      #   $phi70.1
-0000b6d0: 203d 2024 3638 2e33 2020 3a3a 2069 6e74   = $68.3  :: int
-0000b6e0: 3634 0a20 2020 2020 2020 2023 2020 2024  64.        #   $
-0000b6f0: 7068 6931 3036 2e31 203d 2024 3638 2e33  phi106.1 = $68.3
-0000b700: 2020 3a3a 2069 6e74 3634 0a20 2020 2020    :: int64.     
-0000b710: 2020 2023 2020 2064 656c 2024 7068 6931     #   del $phi1
-0000b720: 3036 2e31 0a20 2020 2020 2020 2023 2020  06.1.        #  
-0000b730: 2064 656c 2024 3638 2e33 0a20 2020 2020   del $68.3.     
-0000b740: 2020 2023 2020 2024 7068 6931 3036 2e32     #   $phi106.2
-0000b750: 203d 2024 7068 6936 382e 3120 203a 3a20   = $phi68.1  :: 
-0000b760: 7261 6e67 655f 6974 6572 5f69 6e74 3634  range_iter_int64
-0000b770: 0a20 2020 2020 2020 2023 2020 2064 656c  .        #   del
-0000b780: 2024 7068 6931 3036 2e32 0a20 2020 2020   $phi106.2.     
-0000b790: 2020 2023 2020 2062 7261 6e63 6820 2436     #   branch $6
-0000b7a0: 382e 342c 2037 302c 2031 3036 0a20 2020  8.4, 70, 106.   
-0000b7b0: 2020 2020 2023 206c 6162 656c 2037 300a       # label 70.
-0000b7c0: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
-0000b7d0: 2436 382e 340a 2020 2020 2020 2020 2320  $68.4.        # 
-0000b7e0: 2020 6a20 3d20 2470 6869 3730 2e31 2020    j = $phi70.1  
-0000b7f0: 3a3a 2069 6e74 3634 0a20 2020 2020 2020  :: int64.       
-0000b800: 2023 2020 2064 656c 2024 7068 6937 302e   #   del $phi70.
-0000b810: 310a 0a20 2020 2020 2020 2066 6f72 206a  1..        for j
-0000b820: 2069 6e20 7072 616e 6765 2861 7272 6179   in prange(array
-0000b830: 5f32 2e73 6861 7065 5b30 5d29 3a0a 0a20  _2.shape[0]):.. 
-0000b840: 2020 2020 2020 2020 2020 2023 202d 2d2d             # ---
-0000b850: 204c 494e 4520 3138 3920 2d2d 2d20 0a20   LINE 189 --- . 
-0000b860: 2020 2020 2020 2020 2020 2023 2020 2024             #   $
-0000b870: 3730 2e32 203d 2067 6c6f 6261 6c28 6e70  70.2 = global(np
-0000b880: 3a20 3c6d 6f64 756c 6520 276e 756d 7079  : <module 'numpy
-0000b890: 2720 6672 6f6d 2027 2f55 7365 7273 2f73  ' from '/Users/s
-0000b8a0: 696d 6f6e 2f2e 636f 6e64 612f 656e 7673  imon/.conda/envs
-0000b8b0: 2f73 696d 6261 5f64 6576 2f6c 6962 2f70  /simba_dev/lib/p
-0000b8c0: 7974 686f 6e33 2e36 2f73 6974 652d 7061  ython3.6/site-pa
-0000b8d0: 636b 6167 6573 2f6e 756d 7079 2f5f 5f69  ckages/numpy/__i
-0000b8e0: 6e69 745f 5f2e 7079 273e 2920 203a 3a20  nit__.py'>)  :: 
-0000b8f0: 4d6f 6475 6c65 283c 6d6f 6475 6c65 2027  Module(<module '
-0000b900: 6e75 6d70 7927 2066 726f 6d20 272f 5573  numpy' from '/Us
-0000b910: 6572 732f 7369 6d6f 6e2f 2e63 6f6e 6461  ers/simon/.conda
-0000b920: 2f65 6e76 732f 7369 6d62 615f 6465 762f  /envs/simba_dev/
-0000b930: 6c69 622f 7079 7468 6f6e 332e 362f 7369  lib/python3.6/si
-0000b940: 7465 2d70 6163 6b61 6765 732f 6e75 6d70  te-packages/nump
-0000b950: 792f 5f5f 696e 6974 5f5f 2e70 7927 3e29  y/__init__.py'>)
-0000b960: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000b970: 2024 3730 2e33 203d 2067 6574 6174 7472   $70.3 = getattr
-0000b980: 2876 616c 7565 3d24 3730 2e32 2c20 6174  (value=$70.2, at
-0000b990: 7472 3d6c 696e 616c 6729 2020 3a3a 204d  tr=linalg)  :: M
-0000b9a0: 6f64 756c 6528 3c6d 6f64 756c 6520 276e  odule(<module 'n
-0000b9b0: 756d 7079 2e6c 696e 616c 6727 2066 726f  umpy.linalg' fro
-0000b9c0: 6d20 272f 5573 6572 732f 7369 6d6f 6e2f  m '/Users/simon/
-0000b9d0: 2e63 6f6e 6461 2f65 6e76 732f 7369 6d62  .conda/envs/simb
-0000b9e0: 615f 6465 762f 6c69 622f 7079 7468 6f6e  a_dev/lib/python
-0000b9f0: 332e 362f 7369 7465 2d70 6163 6b61 6765  3.6/site-package
-0000ba00: 732f 6e75 6d70 792f 6c69 6e61 6c67 2f5f  s/numpy/linalg/_
-0000ba10: 5f69 6e69 745f 5f2e 7079 273e 290a 2020  _init__.py'>).  
-0000ba20: 2020 2020 2020 2020 2020 2320 2020 6465            #   de
-0000ba30: 6c20 2437 302e 320a 2020 2020 2020 2020  l $70.2.        
-0000ba40: 2020 2020 2320 2020 2437 302e 3420 3d20      #   $70.4 = 
-0000ba50: 6765 7461 7474 7228 7661 6c75 653d 2437  getattr(value=$7
-0000ba60: 302e 332c 2061 7474 723d 6e6f 726d 2920  0.3, attr=norm) 
-0000ba70: 203a 3a20 4675 6e63 7469 6f6e 283c 6675   :: Function(<fu
-0000ba80: 6e63 7469 6f6e 206e 6f72 6d20 6174 2030  nction norm at 0
-0000ba90: 7837 6663 6265 6639 6461 3438 383e 290a  x7fcbef9da488>).
-0000baa0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000bab0: 6465 6c20 2437 302e 330a 2020 2020 2020  del $70.3.      
-0000bac0: 2020 2020 2020 2320 2020 2437 302e 3720        #   $70.7 
-0000bad0: 3d20 6765 7469 7465 6d28 7661 6c75 653d  = getitem(value=
-0000bae0: 6172 7261 795f 312c 2069 6e64 6578 3d69  array_1, index=i
-0000baf0: 2c20 666e 3d3c 6275 696c 742d 696e 2066  , fn=<built-in f
-0000bb00: 756e 6374 696f 6e20 6765 7469 7465 6d3e  unction getitem>
-0000bb10: 2920 203a 3a20 6172 7261 7928 666c 6f61  )  :: array(floa
-0000bb20: 7436 342c 2031 642c 2041 290a 2020 2020  t64, 1d, A).    
-0000bb30: 2020 2020 2020 2020 2320 2020 2437 302e          #   $70.
-0000bb40: 3130 203d 2067 6574 6974 656d 2876 616c  10 = getitem(val
-0000bb50: 7565 3d61 7272 6179 5f32 2c20 696e 6465  ue=array_2, inde
-0000bb60: 783d 6a2c 2066 6e3d 3c62 7569 6c74 2d69  x=j, fn=<built-i
-0000bb70: 6e20 6675 6e63 7469 6f6e 2067 6574 6974  n function getit
-0000bb80: 656d 3e29 2020 3a3a 2061 7272 6179 2866  em>)  :: array(f
-0000bb90: 6c6f 6174 3634 2c20 3164 2c20 4129 0a20  loat64, 1d, A). 
-0000bba0: 2020 2020 2020 2020 2020 2023 2020 2024             #   $
-0000bbb0: 3730 2e31 3120 3d20 2437 302e 3720 2d20  70.11 = $70.7 - 
-0000bbc0: 2437 302e 3130 2020 3a3a 2061 7272 6179  $70.10  :: array
-0000bbd0: 2866 6c6f 6174 3634 2c20 3164 2c20 4329  (float64, 1d, C)
-0000bbe0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000bbf0: 2064 656c 2024 3730 2e37 0a20 2020 2020   del $70.7.     
-0000bc00: 2020 2020 2020 2023 2020 2064 656c 2024         #   del $
-0000bc10: 3730 2e31 300a 2020 2020 2020 2020 2020  70.10.          
-0000bc20: 2020 2320 2020 2437 302e 3132 203d 2063    #   $70.12 = c
-0000bc30: 616c 6c20 2437 302e 3428 2437 302e 3131  all $70.4($70.11
-0000bc40: 2c20 6675 6e63 3d24 3730 2e34 2c20 6172  , func=$70.4, ar
-0000bc50: 6773 3d5b 5661 7228 2437 302e 3131 2c20  gs=[Var($70.11, 
-0000bc60: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
-0000bc70: 6f6e 5f6d 6978 696e 2e70 793a 3138 3929  on_mixin.py:189)
-0000bc80: 5d2c 206b 7773 3d28 292c 2076 6172 6172  ], kws=(), varar
-0000bc90: 673d 4e6f 6e65 2920 203a 3a20 2861 7272  g=None)  :: (arr
-0000bca0: 6179 2866 6c6f 6174 3634 2c20 3164 2c20  ay(float64, 1d, 
-0000bcb0: 4329 2c20 6f6d 6974 7465 6428 6465 6661  C), omitted(defa
-0000bcc0: 756c 743d 4e6f 6e65 2929 202d 3e20 666c  ult=None)) -> fl
-0000bcd0: 6f61 7436 340a 2020 2020 2020 2020 2020  oat64.          
-0000bce0: 2020 2320 2020 6465 6c20 2437 302e 340a    #   del $70.4.
-0000bcf0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000bd00: 6465 6c20 2437 302e 3131 0a20 2020 2020  del $70.11.     
-0000bd10: 2020 2020 2020 2023 2020 2024 3730 2e31         #   $70.1
-0000bd20: 3520 3d20 6765 7469 7465 6d28 7661 6c75  5 = getitem(valu
-0000bd30: 653d 7265 7375 6c74 732c 2069 6e64 6578  e=results, index
-0000bd40: 3d69 2c20 666e 3d3c 6275 696c 742d 696e  =i, fn=<built-in
-0000bd50: 2066 756e 6374 696f 6e20 6765 7469 7465   function getite
-0000bd60: 6d3e 2920 203a 3a20 6172 7261 7928 666c  m>)  :: array(fl
-0000bd70: 6f61 7436 342c 2031 642c 2043 290a 2020  oat64, 1d, C).  
-0000bd80: 2020 2020 2020 2020 2020 2320 2020 2437            #   $7
-0000bd90: 302e 3135 5b6a 5d20 3d20 2437 302e 3132  0.15[j] = $70.12
-0000bda0: 2020 3a3a 2028 6172 7261 7928 666c 6f61    :: (array(floa
-0000bdb0: 7436 342c 2031 642c 2043 292c 2069 6e74  t64, 1d, C), int
-0000bdc0: 3634 2c20 666c 6f61 7436 3429 202d 3e20  64, float64) -> 
-0000bdd0: 6e6f 6e65 0a20 2020 2020 2020 2020 2020  none.           
-0000bde0: 2023 2020 2064 656c 206a 0a20 2020 2020   #   del j.     
-0000bdf0: 2020 2020 2020 2023 2020 2064 656c 2024         #   del $
-0000be00: 3730 2e31 350a 2020 2020 2020 2020 2020  70.15.          
-0000be10: 2020 2320 2020 6465 6c20 2437 302e 3132    #   del $70.12
-0000be20: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000be30: 206a 756d 7020 3638 0a20 2020 2020 2020   jump 68.       
-0000be40: 2020 2020 2023 206c 6162 656c 2031 3036       # label 106
-0000be50: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000be60: 2064 656c 2069 0a20 2020 2020 2020 2020   del i.         
-0000be70: 2020 2023 2020 2064 656c 2024 7068 6937     #   del $phi7
-0000be80: 302e 310a 2020 2020 2020 2020 2020 2020  0.1.            
-0000be90: 2320 2020 6465 6c20 2470 6869 3638 2e31  #   del $phi68.1
-0000bea0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000beb0: 2064 656c 2024 3638 2e34 0a20 2020 2020   del $68.4.     
-0000bec0: 2020 2020 2020 2023 2020 206a 756d 7020         #   jump 
-0000bed0: 3130 380a 2020 2020 2020 2020 2020 2020  108.            
-0000bee0: 2320 6c61 6265 6c20 3130 380a 2020 2020  # label 108.    
-0000bef0: 2020 2020 2020 2020 2320 2020 6a75 6d70          #   jump
-0000bf00: 2034 380a 2020 2020 2020 2020 2020 2020   48.            
-0000bf10: 2320 6c61 6265 6c20 3131 300a 0a20 2020  # label 110..   
-0000bf20: 2020 2020 2020 2020 2072 6573 756c 7473           results
-0000bf30: 5b69 5d5b 6a5d 203d 206e 702e 6c69 6e61  [i][j] = np.lina
-0000bf40: 6c67 2e6e 6f72 6d28 6172 7261 795f 315b  lg.norm(array_1[
-0000bf50: 695d 202d 2061 7272 6179 5f32 5b6a 5d29  i] - array_2[j])
-0000bf60: 0a0a 2020 2020 2320 2d2d 2d20 4c49 4e45  ..    # --- LINE
-0000bf70: 2031 3930 202d 2d2d 200a 2020 2020 2320   190 --- .    # 
-0000bf80: 2020 6465 6c20 6172 7261 795f 320a 2020    del array_2.  
-0000bf90: 2020 2320 2020 6465 6c20 6172 7261 795f    #   del array_
-0000bfa0: 310a 2020 2020 2320 2020 6465 6c20 2470  1.    #   del $p
-0000bfb0: 6869 3530 2e31 0a20 2020 2023 2020 2064  hi50.1.    #   d
-0000bfc0: 656c 2024 7068 6934 382e 310a 2020 2020  el $phi48.1.    
-0000bfd0: 2320 2020 6465 6c20 2434 382e 340a 2020  #   del $48.4.  
-0000bfe0: 2020 2320 2020 6a75 6d70 2031 3132 0a20    #   jump 112. 
-0000bff0: 2020 2023 206c 6162 656c 2031 3132 0a20     # label 112. 
-0000c000: 2020 2023 2020 2024 3131 322e 3220 3d20     #   $112.2 = 
-0000c010: 6361 7374 2876 616c 7565 3d72 6573 756c  cast(value=resul
-0000c020: 7473 2920 203a 3a20 6172 7261 7928 666c  ts)  :: array(fl
-0000c030: 6f61 7436 342c 2032 642c 2043 290a 2020  oat64, 2d, C).  
-0000c040: 2020 2320 2020 6465 6c20 7265 7375 6c74    #   del result
-0000c050: 730a 2020 2020 2320 2020 7265 7475 726e  s.    #   return
-0000c060: 2024 3131 322e 320a 0a20 2020 2072 6574   $112.2..    ret
-0000c070: 7572 6e20 7265 7375 6c74 730a 0a94 5d94  urn results...].
-0000c080: 2868 5868 4d8c 116e 756d 6261 2e6e 702e  (hXhM..numba.np.
-0000c090: 6172 7261 796f 626a 945d 948c 585f 5a4e  arrayobj.]..X_ZN
-0000c0a0: 3038 4e75 6d62 6145 6e76 356e 756d 6261  08NumbaEnv5numba
-0000c0b0: 326e 7038 6172 7261 796f 626a 3133 6e75  2np8arrayobj13nu
-0000c0c0: 6d70 795f 6675 6c6c 5f6e 6431 3224 3363  mpy_full_nd12$3c
-0000c0d0: 6c6f 6361 6c73 2433 6539 6675 6c6c 2432  locals$3e9full$2
-0000c0e0: 3435 3645 3855 6e69 5475 706c 6549 784c  456E8UniTupleIxL
-0000c0f0: 6932 4545 6494 8794 5294 684d 8c10 6e75  i2EEd...R.hM..nu
-0000c100: 6d62 612e 6e70 2e6e 7079 696d 706c 945d  mba.np.npyimpl.]
-0000c110: 948c 495f 5a4e 3038 4e75 6d62 6145 6e76  ..I_ZN08NumbaEnv
-0000c120: 356e 756d 6261 326e 7037 6e70 7969 6d70  5numba2np7npyimp
-0000c130: 6c32 305f 6272 6f61 6463 6173 745f 6f6e  l20_broadcast_on
-0000c140: 746f 2432 3431 3045 7838 696e 7436 3424  to$2410Ex8int64$
-0000c150: 3261 7838 696e 7436 3424 3261 9487 9452  2ax8int64$2a...R
-0000c160: 9468 4d8c 0f6e 756d 6261 2e6e 702e 6c69  .hM..numba.np.li
-0000c170: 6e61 6c67 945d 948c 885f 5a4e 3038 4e75  nalg.]..._ZN08Nu
-0000c180: 6d62 6145 6e76 356e 756d 6261 326e 7036  mbaEnv5numba2np6
-0000c190: 6c69 6e61 6c67 3134 5f67 6574 5f6e 6f72  linalg14_get_nor
-0000c1a0: 6d5f 696d 706c 3132 2433 636c 6f63 616c  m_impl12$3clocal
-0000c1b0: 7324 3365 3134 6f6e 6544 5f69 6d70 6c24  s$3e14oneD_impl$
-0000c1c0: 3234 3237 4535 4172 7261 7949 644c 6931  2427E5ArrayIdLi1
-0000c1d0: 4531 4337 6d75 7461 626c 6537 616c 6967  E1C7mutable7alig
-0000c1e0: 6e65 6445 3237 6f6d 6974 7465 6424 3238  nedE27omitted$28
-0000c1f0: 6465 6661 756c 7424 3364 4e6f 6e65 2432  default$3dNone$2
-0000c200: 3994 8794 5294 684d 686b 5d94 8c68 5f5a  9...R.hMhk]..h_Z
-0000c210: 4e30 384e 756d 6261 456e 7635 6e75 6d62  N08NumbaEnv5numb
-0000c220: 6132 6e70 366c 696e 616c 6731 375f 6f6e  a2np6linalg17_on
-0000c230: 6544 5f6e 6f72 6d5f 325f 696d 706c 3132  eD_norm_2_impl12
-0000c240: 2433 636c 6f63 616c 7324 3365 3969 6d70  $3clocals$3e9imp
-0000c250: 6c24 3234 3238 4535 4172 7261 7949 644c  l$2428E5ArrayIdL
-0000c260: 6931 4531 4337 6d75 7461 626c 6537 616c  i1E1C7mutable7al
-0000c270: 6967 6e65 6445 9487 9452 9468 4d68 6b5d  ignedE...R.hMhk]
-0000c280: 948c 595f 5a4e 3038 4e75 6d62 6145 6e76  ..Y_ZN08NumbaEnv
-0000c290: 356e 756d 6261 326e 7036 6c69 6e61 6c67  5numba2np6linalg
-0000c2a0: 3235 5f64 756d 6d79 5f6c 6976 656e 6573  25_dummy_livenes
-0000c2b0: 735f 6675 6e63 2432 3432 3945 3330 6c69  s_func$2429E30li
-0000c2c0: 7374 2432 3869 6e74 3634 2432 3924 3363  st$28int64$29$3c
-0000c2d0: 6976 2433 644e 6f6e 6524 3365 9487 9452  iv$3dNone$3e...R
-0000c2e0: 9474 9474 942e                           .t.t..
+00000590: a424 d800 0000 eb58 90c5 fa10 4424 2cc5  .$.....X....D$,.
+000005a0: fa5a c048 8b84 24e0 0000 0048 8b4c 2470  .Z.H..$....H.L$p
+000005b0: c5fb 1104 c848 89df 48b8 0000 0000 0000  .....H..H.......
+000005c0: 0000 ffd0 31c0 488b 9424 1001 0000 4885  ....1.H..$....H.
+000005d0: d20f 9fc0 4889 d148 29c1 488b ac24 0001  ....H..H).H..$..
+000005e0: 0000 48ff c5b3 0148 85d2 0f8e 09ff ffff  ..H....H........
+000005f0: 4889 8c24 1001 0000 488b 7c24 4849 be00  H..$....H.|$HI..
+00000600: 0000 0000 0000 0041 ffd6 488b bc24 7801  .......A..H..$x.
+00000610: 0000 41ff d6f6 c301 0f84 3c06 0000 807c  ..A.......<....|
+00000620: 241f 000f 854d 0600 0048 89e8 48c1 f83f  $....M...H..H..?
+00000630: 4c21 f848 89ac 2400 0100 0048 01e8 4889  L!.H..$....H..H.
+00000640: 4424 7048 8bbc 24f8 0000 00be 2000 0000  D$pH..$..... ...
+00000650: 48b8 0000 0000 0000 0000 ffd0 4889 8424  H...........H..$
+00000660: 0801 0000 488b 6818 4883 7c24 2000 4c8b  ....H.h.H.|$ .L.
+00000670: 9c24 b801 0000 4c8b 8c24 f000 0000 4c8b  .$....L..$....L.
+00000680: b424 7001 0000 488b 9c24 e800 0000 0f8e  .$p...H..$......
+00000690: b503 0000 4c8b 4424 704c 0faf 8424 b001  ....L.D$pL...$..
+000006a0: 0000 488b 8424 9801 0000 4c01 c048 83bc  ..H..$....L..H..
+000006b0: 24a8 0100 0002 7231 4883 bc24 6001 0000  $.....r1H..$`...
+000006c0: 0176 4448 837c 2430 034c 8b54 2440 0f83  .vDH.|$0.L.T$@..
+000006d0: 3901 0000 31c0 e9af 0100 0066 2e0f 1f84  9...1......f....
+000006e0: 0000 0000 000f 1f40 0048 83bc 2460 0100  .......@.H..$`..
+000006f0: 0002 722b 4883 7c24 3003 0f83 e901 0000  ..r+H.|$0.......
+00000700: 31c9 e94b 0200 0048 837c 2430 0348 8b4c  1..K...H.|$0.H.L
+00000710: 2440 0f83 7e02 0000 31d2 e9db 0200 0048  $@..~...1......H
+00000720: 837c 2420 1f0f 87a5 0300 0031 c948 8b54  .|$ .......1.H.T
+00000730: 2430 4829 ca48 8bb4 24c8 0000 0048 85f6  $0H).H..$....H..
+00000740: 741f 0f1f 8000 0000 00c4 c17a 1045 00c5  t..........z.E..
+00000750: fa5c 00c5 fa11 448d 0048 ffc1 48ff ce75  .\....D..H..H..u
+00000760: e848 83fa 070f 82de 0200 0066 2e0f 1f84  .H.........f....
+00000770: 0000 0000 000f 1f40 00c4 c17a 1045 00c5  .......@...z.E..
+00000780: fa5c 00c5 fa11 448d 00c4 c17a 1045 00c5  .\....D....z.E..
+00000790: fa5c 00c5 fa11 448d 04c4 c17a 1045 00c5  .\....D....z.E..
+000007a0: fa5c 00c5 fa11 448d 08c4 c17a 1045 00c5  .\....D....z.E..
+000007b0: fa5c 00c5 fa11 448d 0cc4 c17a 1045 00c5  .\....D....z.E..
+000007c0: fa5c 00c5 fa11 448d 10c4 c17a 1045 00c5  .\....D....z.E..
+000007d0: fa5c 00c5 fa11 448d 14c4 c17a 1045 00c5  .\....D....z.E..
+000007e0: fa5c 00c5 fa11 448d 18c4 c17a 1045 00c5  .\....D....z.E..
+000007f0: fa5c 00c5 fa11 448d 1c48 83c1 0848 394c  .\....D..H...H9L
+00000800: 2420 0f85 71ff ffff e93c 0200 0048 8b84  $ ..q....<...H..
+00000810: 2498 0100 0049 8d14 004c 89ee 31c0 488b  $....I...L..1.H.
+00000820: 4c24 6048 8b7c 2458 4c8b 6424 5066 2e0f  L$`H.|$XL.d$Pf..
+00000830: 1f84 0000 0000 0066 90c5 fa10 06c5 fa5c  .......f.......\
+00000840: 02c5 fa11 4485 00c4 c17a 1004 36c4 c17a  ....D....z..6..z
+00000850: 5c04 13c5 fa11 4485 04c4 a17a 1004 76c4  \.....D....z..v.
+00000860: a17a 5c04 5ac5 fa11 4485 08c5 fa10 0431  .z\.Z...D......1
+00000870: c5fa 5c04 13c5 fa11 4485 0c48 83c0 044c  ..\.....D..H...L
+00000880: 01e2 4801 fe49 39c2 75af f644 2420 034c  ..H..I9.u..D$ .L
+00000890: 8ba4 24d8 0000 000f 84ac 0100 0048 8d14  ..$..........H..
+000008a0: 8500 0000 0048 01ea 4c89 f648 0faf f04c  .....H..L..H...L
+000008b0: 01ee 490f afc3 4803 8424 9801 0000 4c01  ..I...H..$....L.
+000008c0: c031 c966 0f1f 4400 00c5 fa10 06c5 fa5c  .1.f..D........\
+000008d0: 00c5 fa11 048a 48ff c14c 01f6 4c01 d849  ......H..L..L..I
+000008e0: 39c9 75e5 e960 0100 004c 89ea 31c9 488b  9.u..`...L..1.H.
+000008f0: 7424 4048 8b7c 2460 488b 5c24 5866 2e0f  t$@H.|$`H.\$Xf..
+00000900: 1f84 0000 0000 0066 90c5 fa10 02c5 fa5c  .......f.......\
+00000910: 00c5 fa11 448d 00c4 c17a 1004 16c5 fa5c  ....D....z.....\
+00000920: 00c5 fa11 448d 04c4 a17a 1004 72c5 fa5c  ....D....z..r..\
+00000930: 00c5 fa11 448d 08c5 fa10 0417 c5fa 5c00  ....D.........\.
+00000940: c5fa 1144 8d0c 4883 c104 4801 da48 39ce  ...D..H...H..H9.
+00000950: 75b7 4d85 c90f 84ee 0000 0048 8d14 8d00  u.M........H....
+00000960: 0000 0048 01ea 490f afce 4c01 e931 f666  ...H..I...L..1.f
+00000970: 2e0f 1f84 0000 0000 00c5 fa10 01c5 fa5c  ...............\
+00000980: 00c5 fa11 04b2 48ff c64c 01f1 4939 f175  ......H..L..I9.u
+00000990: e8e9 b300 0000 31d2 488b 7424 5066 2e0f  ......1.H.t$Pf..
+000009a0: 1f84 0000 0000 0066 90c4 c17a 1045 00c5  .......f...z.E..
+000009b0: fa5c 00c5 fa11 4495 00c4 c17a 1045 00c4  .\....D....z.E..
+000009c0: c17a 5c04 03c5 fa11 4495 04c4 c17a 1045  .z\.....D....z.E
+000009d0: 00c4 a17a 5c04 58c5 fa11 4495 08c4 c17a  ...z\.X...D....z
+000009e0: 1045 00c5 fa5c 0403 c5fa 1144 950c 4883  .E...\.....D..H.
+000009f0: c204 4801 f048 39d1 75af f644 2420 0374  ..H..H9.u..D$ .t
+00000a00: 4848 8d04 9500 0000 0048 01e8 490f afd3  HH.......H..I...
+00000a10: 4803 9424 9801 0000 4c01 c231 c966 2e0f  H..$....L..1.f..
+00000a20: 1f84 0000 0000 0066 90c4 c17a 1045 00c5  .......f...z.E..
+00000a30: fa5c 02c5 fa11 0488 48ff c14c 01da 4939  .\......H..L..I9
+00000a40: c975 e666 0f1f 4400 0048 8b7c 2448 49be  .u.f..D..H.|$HI.
+00000a50: 0000 0000 0000 0000 c5f8 7741 ffd6 488b  ..........wA..H.
+00000a60: bc24 7801 0000 41ff d64c 8b44 2420 48c7  .$x...A..L.D$ H.
+00000a70: 4424 7800 0000 00c7 4424 2c00 0000 004c  D$x.....D$,....L
+00000a80: 8944 2408 4889 2c24 48c7 4424 1004 0000  .D$.H.,$H.D$....
+00000a90: 0041 b904 0000 0048 8d7c 242c 488d 7424  .A.....H.|$,H.t$
+00000aa0: 7848 8b9c 2408 0100 0048 89da 31c9 48b8  xH..$....H..1.H.
+00000ab0: 0000 0000 0000 0000 ffd0 85c0 0f84 d7fa  ................
+00000ac0: ffff 83f8 fe0f 84ce faff ffe9 9601 0000  ................
+00000ad0: 488b 4c24 2048 8d0c 8d00 0000 0048 01e9  H.L$ H.......H..
+00000ae0: 488d 5001 4839 ea40 0f97 c748 39c8 410f  H.P.H9.@...H9.A.
+00000af0: 92c0 4839 ac24 c000 0000 0f97 c249 39cd  ..H9.$.......I9.
+00000b00: 400f 92c6 4484 c70f 851e fcff ffb9 0000  @...D...........
+00000b10: 0000 4020 f20f 8512 fcff ff48 83bc 2498  ..@ .......H..$.
+00000b20: 0000 0000 0f84 b200 0000 c4c1 7a10 4500  ............z.E.
+00000b30: c5fa 5c00 c4e2 7d18 c031 c948 8b94 2480  ..\...}..1.H..$.
+00000b40: 0000 0066 0f1f 4400 00c5 fc11 448d 00c5  ...f..D.....D...
+00000b50: fc11 448d 20c5 fc11 448d 40c5 fc11 448d  ..D. ...D.@...D.
+00000b60: 60c5 fc11 848d 8000 0000 c5fc 1184 8da0  `...............
+00000b70: 0000 00c5 fc11 848d c000 0000 c5fc 1184  ................
+00000b80: 8de0 0000 0048 83c1 4048 83c2 fe75 ba48  .....H..@H...u.H
+00000b90: 83bc 2488 0000 0000 7427 c4c1 7a10 4500  ..$.....t'..z.E.
+00000ba0: c5fa 5c00 c4e2 7d18 c0c5 fc11 448d 00c5  ..\...}.....D...
+00000bb0: fc11 448d 20c5 fc11 448d 40c5 fc11 448d  ..D. ...D.@...D.
+00000bc0: 6048 8b94 2490 0000 0048 89d1 4839 5424  `H..$....H..H9T$
+00000bd0: 200f 8556 fbff ffe9 6dfe ffff 31c9 4883   ..V....m...1.H.
+00000be0: bc24 8800 0000 0075 b1eb d648 8b84 24b0  .$.....u...H..$.
+00000bf0: 0000 0048 8b8c 24a0 0000 0048 8908 48c7  ...H..$....H..H.
+00000c00: 4008 0000 0000 488b 8c24 a800 0000 4889  @.....H..$....H.
+00000c10: 4810 48c7 4018 0800 0000 488b 4c24 6848  H.H.@.....H.L$hH
+00000c20: 8948 204c 8940 284c 8978 3049 c1e7 034c  .H L.@(L.x0I...L
+00000c30: 8978 3848 c740 4008 0000 0048 8bbc 2478  .x8H.@@....H..$x
+00000c40: 0100 0048 bb00 0000 0000 0000 00ff d348  ...H...........H
+00000c50: 8b7c 2448 ffd3 31c0 eb33 48b8 0000 0000  .|$H..1..3H.....
+00000c60: 0000 0000 eb1a 488b 4c24 784c 8b6c 2438  ......H.L$xL.l$8
+00000c70: 4989 4d00 eb17 48b8 0000 0000 0000 0000  I.M...H.........
+00000c80: 488b 4c24 3848 8901 b801 0000 0048 81c4  H.L$8H.......H..
+00000c90: 1801 0000 5b41 5c41 5d41 5e41 5f5d c348  ....[A\A]A^A_].H
+00000ca0: b900 0000 0000 0000 0049 894d 00eb de66  .........I.M...f
+00000cb0: 2e0f 1f84 0000 0000 0055 4889 e541 5741  .........UH..AWA
+00000cc0: 5641 5541 5453 4883 e4e0 4881 ec80 0200  VAUATSH...H.....
+00000cd0: 0048 89f7 48be 0000 0000 0000 0000 48bb  .H..H.........H.
+00000ce0: 0000 0000 0000 0000 4c8d 8424 9800 0000  ........L..$....
+00000cf0: 4c8d 8c24 9000 0000 ba02 0000 00b9 0200  L..$............
+00000d00: 0000 31c0 ffd3 c5f8 57c0 c5fc 2984 24a0  ..1.....W...).$.
+00000d10: 0000 00c5 fc29 8424 c000 0000 48c7 8424  .....).$....H..$
+00000d20: e000 0000 0000 0000 c5fc 2984 2400 0100  ..........).$...
+00000d30: 00c5 fc29 8424 2001 0000 48c7 8424 4001  ...).$ ...H..$@.
+00000d40: 0000 0000 0000 c5fc 2984 2460 0100 00c5  ........).$`....
+00000d50: fc29 8424 8001 0000 48c7 8424 a001 0000  .).$....H..$....
+00000d60: 0000 0000 48c7 8424 8000 0000 0000 0000  ....H..$........
+00000d70: c5fc 2984 24e0 0100 00c5 fc29 8424 0002  ..).$......).$..
+00000d80: 0000 48c7 8424 2002 0000 0000 0000 85c0  ..H..$ .........
+00000d90: 0f84 7403 0000 48b8 0000 0000 0000 0000  ..t...H.........
+00000da0: 488b 1848 85db 0f84 2503 0000 488b bc24  H..H....%...H..$
+00000db0: 9800 0000 c5f8 57c0 c5fc 2984 24a0 0000  ......W...).$...
+00000dc0: 00c5 fc29 8424 c000 0000 48c7 8424 e000  ...).$....H..$..
+00000dd0: 0000 0000 0000 49bc 0000 0000 0000 0000  ......I.........
+00000de0: 488d b424 a000 0000 c5f8 7741 ffd4 85c0  H..$......wA....
+00000df0: 0f85 f102 0000 4883 bc24 b800 0000 040f  ......H..$......
+00000e00: 85e2 0200 0048 899c 2488 0000 004c 8bbc  .....H..$....L..
+00000e10: 24a0 0000 0048 8b84 24c0 0000 0048 8944  $....H..$....H.D
+00000e20: 2478 488b 8424 c800 0000 4889 8424 c001  $xH..$....H..$..
+00000e30: 0000 4c8b ac24 d000 0000 4c8b b424 d800  ..L..$....L..$..
+00000e40: 0000 488b 9c24 e000 0000 488b bc24 9000  ..H..$....H..$..
+00000e50: 0000 c5f8 57c0 c5fc 2984 2400 0100 00c5  ....W...).$.....
+00000e60: fc29 8424 2001 0000 48c7 8424 4001 0000  .).$ ...H..$@...
+00000e70: 0000 0000 488d b424 0001 0000 c5f8 7741  ....H..$......wA
+00000e80: ffd4 85c0 0f85 9402 0000 4883 bc24 1801  ..........H..$..
+00000e90: 0000 040f 8585 0200 004c 8ba4 2400 0100  .........L..$...
+00000ea0: 00c5 fc28 8424 2001 0000 488b 8424 4001  ...(.$ ...H..$@.
+00000eb0: 0000 c5f0 57c9 c5fc 298c 2460 0100 00c5  ....W...).$`....
+00000ec0: fc29 8c24 8001 0000 48c7 8424 a001 0000  .).$....H..$....
+00000ed0: 0000 0000 4889 4424 68c5 fc11 4424 484c  ....H.D$h...D$HL
+00000ee0: 8964 2428 4889 5c24 204c 8974 2418 4c89  .d$(H.\$ L.t$.L.
+00000ef0: 6c24 1048 8b84 24c0 0100 0048 8944 2408  l$.H..$....H.D$.
+00000f00: 488b 4424 7848 8904 2448 b800 0000 0000  H.D$xH..$H......
+00000f10: 0000 0048 8dbc 2460 0100 0048 8db4 2480  ...H..$`...H..$.
+00000f20: 0000 004c 89fa c5f8 77ff d089 c34c 8bac  ...L....w....L..
+00000f30: 2480 0000 0048 8b84 2460 0100 0048 8944  $....H..$`...H.D
+00000f40: 2478 c5fc 1084 2468 0100 00c5 fc29 8424  $x....$h.....).$
+00000f50: c001 0000 c5fc 1084 2488 0100 00c5 fc29  ........$......)
+00000f60: 8424 4002 0000 49be 0000 0000 0000 0000  .$@...I.........
+00000f70: 4c89 ffc5 f877 41ff d64c 89e7 41ff d683  L....wA..L..A...
+00000f80: fbfe 742b 85db 7548 488b 8424 8800 0000  ..t+..uHH..$....
+00000f90: 488b 7818 4885 ff74 7e48 b800 0000 0000  H.x.H..t~H......
+00000fa0: 0000 0031 f6ff d048 89c1 e98a 0000 0048  ...1...H.......H
+00000fb0: bb00 0000 0000 0000 0048 b800 0000 0000  .........H......
+00000fc0: 0000 0048 89df ffd0 4889 d8e9 3c01 0000  ...H....H...<...
+00000fd0: 0f8e c300 0000 48b8 0000 0000 0000 0000  ......H.........
+00000fe0: ffd0 498b 5510 418b 7508 498b 7d00 48b8  ..I.U.A.u.I.}.H.
+00000ff0: 0000 0000 0000 0000 ffd0 4885 c00f 8407  ..........H.....
+00001000: 0100 0048 b900 0000 0000 0000 0048 89c7  ...H.........H..
+00001010: ffd1 e9f3 0000 0048 bf00 0000 0000 0000  .......H........
+00001020: 0048 be00 0000 0000 0000 0048 b800 0000  .H.........H....
+00001030: 0000 0000 00ff d031 c948 8b5c 2478 4889  .......1.H.\$xH.
+00001040: 9c24 e001 0000 c5fc 2884 24c0 0100 00c5  .$......(.$.....
+00001050: fc11 8424 e801 0000 c5fc 2884 2440 0200  ...$......(.$@..
+00001060: 00c5 fc11 8424 0802 0000 48b8 0000 0000  .....$....H.....
+00001070: 0000 0000 488d bc24 e001 0000 be02 0000  ....H..$........
+00001080: 00ba 0100 0000 c5f8 77ff d049 89c7 4889  ........w..I..H.
+00001090: df41 ffd6 4c89 f8eb 7383 fbfd 741b 83fb  .A..L...s...t...
+000010a0: ff74 6748 bf00 0000 0000 0000 0048 be00  .tgH.........H..
+000010b0: 0000 0000 0000 00eb 4248 bf00 0000 0000  ........BH......
+000010c0: 0000 0048 b800 0000 0000 0000 00ff d0eb  ...H............
+000010d0: 3948 bf00 0000 0000 0000 0048 be00 0000  9H.........H....
+000010e0: 0000 0000 00eb 1448 bf00 0000 0000 0000  .......H........
+000010f0: 0048 be00 0000 0000 0000 0048 b800 0000  .H.........H....
+00001100: 0000 0000 00c5 f877 ffd0 31c0 488d 65d8  .......w..1.H.e.
+00001110: 5b41 5c41 5d41 5e41 5f5d c5f8 77c3 48bf  [A\A]A^A_]..w.H.
+00001120: 0000 0000 0000 0000 48be 0000 0000 0000  ........H.......
+00001130: 0000 48b8 0000 0000 0000 0000 ffd0 48b8  ..H...........H.
+00001140: 0000 0000 0000 0000 4c89 ffff d0eb bb66  ........L......f
+00001150: 2e0f 1f84 0000 0000 0055 4889 e541 5741  .........UH..AWA
+00001160: 5641 5541 5453 4883 e4e0 4881 ec20 0100  VAUATSH...H.. ..
+00001170: 00c5 fc10 4510 4889 f248 89fb 488b 4530  ....E.H..H..H.E0
+00001180: c5fc 104d 5048 8b4d 70c5 e857 d2c5 fc29  ...MPH.Mp..W...)
+00001190: 9424 e000 0000 c5fc 2994 24c0 0000 0048  .$......).$....H
+000011a0: c784 2400 0100 0000 0000 0048 c784 2480  ..$........H..$.
+000011b0: 0000 0000 0000 0048 894c 2468 c5fc 114c  .......H.L$h...L
+000011c0: 2448 4889 4424 28c5 fc11 4424 084c 890c  $HH.D$(...D$.L..
+000011d0: 2448 b800 0000 0000 0000 0048 8dbc 24c0  $H.........H..$.
+000011e0: 0000 0048 8db4 2480 0000 00c5 f877 ffd0  ...H..$......w..
+000011f0: 4189 c64c 8bbc 2480 0000 004c 8b84 24c0  A..L..$....L..$.
+00001200: 0000 004c 8ba4 24c8 0000 004c 8bac 24d0  ...L..$....L..$.
+00001210: 0000 0048 8b8c 24d8 0000 0048 8b94 24e0  ...H..$....H..$.
+00001220: 0000 0048 8bb4 24e8 0000 0048 8bbc 24f0  ...H..$....H..$.
+00001230: 0000 0048 8b84 24f8 0000 004c 8b8c 2400  ...H..$....L..$.
+00001240: 0100 00c7 4424 7c00 0000 0041 83fe fe0f  ....D$|....A....
+00001250: 8412 0100 0045 85f6 0f84 0901 0000 4c89  .....E........L.
+00001260: 8c24 8800 0000 4889 8424 9000 0000 4889  .$....H..$....H.
+00001270: bc24 9800 0000 4889 b424 a000 0000 4889  .$....H..$....H.
+00001280: 9424 a800 0000 4889 8c24 b000 0000 4c89  .$....H..$....L.
+00001290: 8424 b800 0000 48b8 0000 0000 0000 0000  .$....H.........
+000012a0: 488d 7c24 7cff d045 85f6 0f8e ec00 0000  H.|$|..E........
+000012b0: 48b8 0000 0000 0000 0000 ffd0 498b 5710  H...........I.W.
+000012c0: 418b 7708 498b 3f48 b800 0000 0000 0000  A.w.I.?H........
+000012d0: 00ff d048 85c0 740f 48b9 0000 0000 0000  ...H..t.H.......
+000012e0: 0000 4889 c7ff d148 bf00 0000 0000 0000  ..H....H........
+000012f0: 0048 b800 0000 0000 0000 00ff d049 89c6  .H...........I..
+00001300: 48b8 0000 0000 0000 0000 4c89 f7ff d048  H.........L....H
+00001310: b800 0000 0000 0000 004c 89f7 ffd0 48b8  .........L....H.
+00001320: 0000 0000 0000 0000 488d 7c24 7cff d04c  ........H.|$|..L
+00001330: 8b84 24b8 0000 0048 8b8c 24b0 0000 0048  ..$....H..$....H
+00001340: 8b94 24a8 0000 0048 8bb4 24a0 0000 0048  ..$....H..$....H
+00001350: 8bbc 2498 0000 0048 8b84 2490 0000 004c  ..$....H..$....L
+00001360: 8b8c 2488 0000 004c 8903 4c89 6308 4c89  ..$....L..L.c.L.
+00001370: 6b10 4889 4b18 4889 5320 4889 7328 4889  k.H.K.H.S H.s(H.
+00001380: 7b30 4889 4338 4c89 4b40 4889 d848 8d65  {0H.C8L.K@H..H.e
+00001390: d85b 415c 415d 415e 415f 5dc3 4183 fefd  .[A\A]A^A_].A...
+000013a0: 742f 4183 feff 0f84 3bff ffff 48bf 0000  t/A.....;...H...
+000013b0: 0000 0000 0000 48be 0000 0000 0000 0000  ......H.........
+000013c0: 48b8 0000 0000 0000 0000 ffd0 e916 ffff  H...............
+000013d0: ff48 bf00 0000 0000 0000 0048 b800 0000  .H.........H....
+000013e0: 0000 0000 00ff d0e9 fbfe ffff 662e 0f1f  ............f...
+000013f0: 8400 0000 0000 0f1f 0041 5741 5641 5541  .........AWAVAUA
+00001400: 5453 4c89 cb4d 89c4 4989 f649 89ff 48b8  TSL..M..I..I..H.
+00001410: 0000 0000 0000 0000 bf04 0000 00be 2000  .............. .
+00001420: 0000 ffd0 4885 db0f 8411 0100 0049 89c5  ....H........I..
+00001430: 488b 7424 3848 8b54 2430 c4e1 fb2a c348  H.t$8H.T$0...*.H
+00001440: 8b58 18c4 e1f3 2a4c 2440 c5f3 5ec0 c4e1  .X....*L$@..^...
+00001450: fb2c c848 b800 0000 0000 0000 00bf 7300  .,.H..........s.
+00001460: 0000 4989 d8ff d085 c00f 8898 0000 0048  ..I............H
+00001470: be00 0000 0000 0000 0048 b800 0000 0000  .........H......
+00001480: 0000 00bf 2800 0000 ffd0 4885 c00f 84b7  ....(.....H.....
+00001490: 0000 0048 8b48 1848 c741 0802 0000 0048  ...H.H.H.A.....H
+000014a0: 8b48 1848 c701 0000 0000 488b 4818 c641  .H.H......H.H..A
+000014b0: 1000 488b 4818 c5f9 57c0 c5f9 1141 1848  ..H.H...W....A.H
+000014c0: 8b48 1848 c701 0200 0000 488b 4818 48c7  .H.H......H.H.H.
+000014d0: 4118 0100 0000 488b 4818 4c89 6120 488b  A.....H.H.L.a H.
+000014e0: 4818 4883 3900 7e6e 49be 0000 0000 0000  H.H.9.~nI.......
+000014f0: 0000 4889 c741 ffd6 8b1b 4c89 ef41 ffd6  ..H..A....L..A..
+00001500: 4189 1f31 c0eb 2d48 b800 0000 0000 0000  A..1..-H........
+00001510: 004c 89ef ffd0 48b8 0000 0000 0000 0000  .L....H.........
+00001520: ffd0 48b8 0000 0000 0000 0000 4989 06b8  ..H.........I...
+00001530: 0100 0000 5b41 5c41 5d41 5e41 5fc3 48b8  ....[A\A]A^A_.H.
+00001540: 0000 0000 0000 0000 ebe2 48b8 0000 0000  ..........H.....
+00001550: 0000 0000 ebd6 48b8 0000 0000 0000 0000  ......H.........
+00001560: ebca 0f1f 8000 0000 0048 85ff 7406 f048  .........H..t..H
+00001570: ff0f 7401 c348 b800 0000 0000 0000 00ff  ..t..H..........
+00001580: e00f 1f84 0000 0000 00c3 662e 0f1f 8400  ..........f.....
+00001590: 0000 0000 0f1f 4400 0048 85ff 7405 f048  ......D..H..t..H
+000015a0: ff07 c3c3 0000 0000 0000 0000 0000 0000  ................
+000015b0: 00b6 0000 0000 0000 0000 0000 0000 0000  ................
+000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015d0: 0083 0000 0000 0000 0000 0000 0000 0000  ................
+000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015f0: 0047 0000 0000 0000 0000 0000 0000 0000  .G..............
+00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001610: 0083 0000 0000 0000 0000 0000 0000 0000  ................
+00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001630: 008b 0000 0000 0000 0000 0000 0000 0000  ................
+00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001650: 003f 0000 0000 0000 0000 0000 0000 0000  .?..............
+00001660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001670: 003d 0000 0000 0000 0000 0000 0000 0000  .=..............
+00001680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001690: 003c 0000 0000 0000 0000 0000 0000 0000  .<..............
+000016a0: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+000016b0: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
+000016c0: 7100 585b 0000 0061 7272 6179 2069 7320  q.X[...array is 
+000016d0: 746f 6f20 6269 673b 2060 6172 722e 7369  too big; `arr.si
+000016e0: 7a65 202a 2061 7272 2e64 7479 7065 2e69  ze * arr.dtype.i
+000016f0: 7465 6d73 697a 6560 2069 7320 6c61 7267  temsize` is larg
+00001700: 6572 2074 6861 6e20 7468 6520 6d61 7869  er than the maxi
+00001710: 6d75 6d20 706f 7373 6962 6c65 2073 697a  mum possible siz
+00001720: 652e 7101 8571 024e 8771 032e 0000 0000  e.q..q.N.q......
+00001730: 0000 0000 0000 0000 0036 3738 f0a8 d2e2  .........678....
+00001740: 6071 fb50 e9d2 1b4b 80a9 532f 0600 0000  `q.P...K..S/....
+00001750: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001760: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
+00001770: 7100 588e 0000 0075 6e61 626c 6520 746f  q.X....unable to
+00001780: 2062 726f 6164 6361 7374 2061 7267 756d   broadcast argum
+00001790: 656e 7420 3120 746f 206f 7574 7075 7420  ent 1 to output 
+000017a0: 6172 7261 790a 4669 6c65 2022 2f55 7365  array.File "/Use
+000017b0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+000017c0: 2f65 6e76 732f 7369 6d62 615f 6465 762f  /envs/simba_dev/
+000017d0: 7369 6d62 612f 6d69 7869 6e73 2f66 6561  simba/mixins/fea
+000017e0: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
+000017f0: 6d69 7869 6e2e 7079 222c 206c 696e 6520  mixin.py", line 
+00001800: 3335 352c 2071 0185 7102 4e87 7103 2e00  355, q..q.N.q...
+00001810: 0000 0000 0000 0000 0050 4af1 a8e9 28fa  .........PJ...(.
+00001820: 621a bb2d bd2e e95a 0642 3af7 b400 0000  b..-...Z.B:.....
+00001830: 0000 0000 0000 0000 0046 6561 7475 7265  .........Feature
+00001840: 4578 7472 6163 7469 6f6e 4d69 7869 6e2e  ExtractionMixin.
+00001850: 6364 6973 7400 0000 006d 6973 7369 6e67  cdist....missing
+00001860: 2045 6e76 6972 6f6e 6d65 6e74 3a20 5f5a   Environment: _Z
+00001870: 4e30 384e 756d 6261 456e 7635 7369 6d62  N08NumbaEnv5simb
+00001880: 6136 6d69 7869 6e73 3234 6665 6174 7572  a6mixins24featur
+00001890: 655f 6578 7472 6163 7469 6f6e 5f6d 6978  e_extraction_mix
+000018a0: 696e 3232 4665 6174 7572 6545 7874 7261  in22FeatureExtra
+000018b0: 6374 696f 6e4d 6978 696e 3130 6364 6973  ctionMixin10cdis
+000018c0: 7424 3234 3630 4535 4172 7261 7949 664c  t$2460E5ArrayIfL
+000018d0: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
+000018e0: 6967 6e65 6445 3541 7272 6179 4966 4c69  ignedE5ArrayIfLi
+000018f0: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
+00001900: 676e 6564 4500 0000 0063 616e 2774 2075  gnedE....can't u
+00001910: 6e62 6f78 2061 7272 6179 2066 726f 6d20  nbox array from 
+00001920: 5079 4f62 6a65 6374 2069 6e74 6f20 6e61  PyObject into na
+00001930: 7469 7665 2076 616c 7565 2e20 2054 6865  tive value.  The
+00001940: 206f 626a 6563 7420 6d61 7962 6520 6f66   object maybe of
+00001950: 2061 2064 6966 6665 7265 6e74 2074 7970   a different typ
+00001960: 6500 0000 0000 0000 0060 656e 762e 636f  e........`env.co
+00001970: 6e73 7473 6020 6973 204e 554c 4c20 696e  nsts` is NULL in
+00001980: 2060 7265 6164 5f63 6f6e 7374 6000 0000   `read_const`...
+00001990: 0000 0000 0000 0000 0075 6e6b 6e6f 776e  .........unknown
+000019a0: 2065 7272 6f72 2077 6865 6e20 6361 6c6c   error when call
+000019b0: 696e 6720 6e61 7469 7665 2066 756e 6374  ing native funct
+000019c0: 696f 6e00 0000 0000 003c 6e75 6d62 612e  ion......<numba.
+000019d0: 636f 7265 2e63 7075 2e43 5055 436f 6e74  core.cpu.CPUCont
+000019e0: 6578 7420 6f62 6a65 6374 2061 7420 3078  ext object at 0x
+000019f0: 3766 3935 3535 3530 3639 3430 3e00 0000  7f9555506940>...
+00001a00: 0000 0000 0000 0000 0075 6e6b 6e6f 776e  .........unknown
+00001a10: 2065 7272 6f72 2077 6865 6e20 6361 6c6c   error when call
+00001a20: 696e 6720 6e61 7469 7665 2066 756e 6374  ing native funct
+00001a30: 696f 6e00 0000 0000 0080 0363 6275 696c  ion........cbuil
+00001a40: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
+00001a50: 7100 585b 0000 0061 7272 6179 2069 7320  q.X[...array is 
+00001a60: 746f 6f20 6269 673b 2060 6172 722e 7369  too big; `arr.si
+00001a70: 7a65 202a 2061 7272 2e64 7479 7065 2e69  ze * arr.dtype.i
+00001a80: 7465 6d73 697a 6560 2069 7320 6c61 7267  temsize` is larg
+00001a90: 6572 2074 6861 6e20 7468 6520 6d61 7869  er than the maxi
+00001aa0: 6d75 6d20 706f 7373 6962 6c65 2073 697a  mum possible siz
+00001ab0: 652e 7101 8571 024e 8771 032e 0000 0000  e.q..q.N.q......
+00001ac0: 0000 0000 0000 0000 0036 3738 f0a8 d2e2  .........678....
+00001ad0: 6071 fb50 e9d2 1b4b 80a9 532f 0600 0000  `q.P...K..S/....
+00001ae0: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001af0: 7469 6e73 0a56 616c 7565 4572 726f 720a  tins.ValueError.
+00001b00: 7100 581f 0000 006e 6567 6174 6976 6520  q.X....negative 
+00001b10: 6469 6d65 6e73 696f 6e73 206e 6f74 2061  dimensions not a
+00001b20: 6c6c 6f77 6564 7101 8571 024e 8771 032e  llowedq..q.N.q..
+00001b30: 0000 0000 0000 0000 00ae da98 e06c 49b7  .............lI.
+00001b40: ad8d 31d8 f7bf e26d 725c eeb4 fd00 0000  ..1....mr\......
+00001b50: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001b60: 7469 6e73 0a49 6e64 6578 4572 726f 720a  tins.IndexError.
+00001b70: 7100 5814 0000 0067 6574 6974 656d 206f  q.X....getitem o
+00001b80: 7574 206f 6620 7261 6e67 6571 0185 7102  ut of rangeq..q.
+00001b90: 4e87 7103 2e00 0000 0020 07e5 5362 341d  N.q...... ..Sb4.
+00001ba0: 8cb1 31a7 6c9a ffe8 647a bda8 6d00 0000  ..1.l...dz..m...
+00001bb0: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001bc0: 7469 6e73 0a4d 656d 6f72 7945 7272 6f72  tins.MemoryError
+00001bd0: 0a71 0058 1400 0000 6361 6e6e 6f74 2061  .q.X....cannot a
+00001be0: 6c6c 6f63 6174 6520 6c69 7374 7101 8571  llocate listq..q
+00001bf0: 024e 8771 032e 0000 00ee a280 57b5 a3e7  .N.q........W...
+00001c00: aa1c aed9 439a e21e e2dc 0c7a 9b00 0000  ....C......z....
+00001c10: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001c20: 7469 6e73 0a5a 6572 6f44 6976 6973 696f  tins.ZeroDivisio
+00001c30: 6e45 7272 6f72 0a71 0058 1000 0000 6469  nError.q.X....di
+00001c40: 7669 7369 6f6e 2062 7920 7a65 726f 7101  vision by zeroq.
+00001c50: 8571 024e 8771 032e 007e 37a9 709c 0a80  .q.N.q...~7.p...
+00001c60: 79dd 9427 5983 7d90 f293 2bae 3600 0000  y..'Y.}...+.6...
+00001c70: 0000 0000 0000 0000 0080 0363 6275 696c  ...........cbuil
+00001c80: 7469 6e73 0a41 7373 6572 7469 6f6e 4572  tins.AssertionEr
+00001c90: 726f 720a 7100 2958 0400 0000 696d 706c  ror.q.)X....impl
+00001ca0: 7101 5851 0000 002f 5573 6572 732f 7369  q.XQ.../Users/si
+00001cb0: 6d6f 6e2f 2e63 6f6e 6461 2f65 6e76 732f  mon/.conda/envs/
+00001cc0: 7369 6d62 615f 6465 762f 6c69 622f 7079  simba_dev/lib/py
+00001cd0: 7468 6f6e 332e 362f 7369 7465 2d70 6163  thon3.6/site-pac
+00001ce0: 6b61 6765 732f 6e75 6d62 612f 6e70 2f6c  kages/numba/np/l
+00001cf0: 696e 616c 672e 7079 7102 4d5e 0887 7103  inalg.pyq.M^..q.
+00001d00: 8771 042e 0000 0000 0049 1f9a 1741 ace0  .q.......I...A..
+00001d10: 7701 f821 d0e5 1919 89e8 abf9 9d00 0000  w..!............
+00001d20: 0000 0000 0000 0000 0006 0a00 0000 182a  ...............*
+00001d30: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0010 0a00 0000 0000 0096 0400 00d1 5805  ..............X.
+00001d50: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 00b0 0e00 0000 0000 0093 0200 00d1 5805  ..............X.
+00001d70: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0050 1100 0000 0000 0069 0100 0000 1406  .P.......i......
+00001d90: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0014 0000 0000 0000 0001 7a52 0001 7810  ..........zR..x.
+00001db0: 0110 0c07 0890 0100 003c 0000 001c 0000  .........<......
+00001dc0: 00e8 e4ff ffff ffff ff06 0a00 0000 0000  ................
+00001dd0: 0000 410e 1042 0e18 420e 2042 0e28 420e  ..A..B..B. B.(B.
+00001de0: 3041 0e38 470e d002 8307 8c06 8d05 8e04  0A.8G...........
+00001df0: 8f03 8602 0000 0000 002c 0000 005c 0000  .........,...\..
+00001e00: 00b8 eeff ffff ffff ff96 0400 0000 0000  ................
+00001e10: 0000 410e 1086 0243 0d06 5483 078c 068d  ..A....C..T.....
+00001e20: 058e 048f 0300 0000 002c 0000 008c 0000  .........,......
+00001e30: 0028 f3ff ffff ffff ff93 0200 0000 0000  .(..............
+00001e40: 0000 410e 1086 0243 0d06 5483 078c 068d  ..A....C..T.....
+00001e50: 058e 048f 0300 0000 0034 0000 00bc 0000  .........4......
+00001e60: 0098 f5ff ffff ffff ff69 0100 0000 0000  .........i......
+00001e70: 0000 420e 1042 0e18 420e 2042 0e28 410e  ..B..B..B. B.(A.
+00001e80: 3083 068c 058d 048e 038f 0200 0000 0000  0...............
+00001e90: 001c 0000 00f4 0000 00d0 f6ff ffff ffff  ................
+00001ea0: ff18 0000 0000 0000 0000 0000 0000 0000  ................
+00001eb0: 001c 0000 0014 0100 00d0 f6ff ffff ffff  ................
+00001ec0: ff01 0000 0000 0000 0000 0000 0000 0000  ................
+00001ed0: 00ce 1200 0027 0000 0eaf 1200 000e 0000  .....'..........
+00001ee0: 0ea3 1200 000d 0000 0e97 1200 000c 0000  ................
+00001ef0: 0e7b 1200 000b 0000 0e6f 1200 0041 0000  .{.......o...A..
+00001f00: 0e60 1200 0020 0000 0e41 1200 0020 0000  .`... ...A... ..
+00001f10: 0ed2 1100 0028 0000 0ec8 1100 001f 0000  .....(..........
+00001f20: 0eac 1100 0045 0000 0e67 1100 0026 0000  .....E...g...&..
+00001f30: 0e34 1100 002d 0000 0e2a 1100 0031 0000  .4...-...*...1..
+00001f40: 0e19 1100 002e 0000 0e0f 1100 000a 0000  ................
+00001f50: 0e05 1100 0032 0000 0e77 1000 0043 0000  .....2...w...C..
+00001f60: 0e68 1000 0036 0000 0e59 1000 002f 0000  .h...6...Y.../..
+00001f70: 0e4a 1000 0035 0000 0e40 1000 0009 0000  .J...5...@......
+00001f80: 0e31 1000 0040 0000 0e20 1000 0044 0000  .1...@... ...D..
+00001f90: 0e09 1000 002c 0000 0eef 0f00 0042 0000  .....,.......B..
+00001fa0: 0e2a 0f00 0023 0000 0e97 0e00 0020 0000  .*...#....... ..
+00001fb0: 0e8b 0e00 002e 0000 0e81 0e00 0008 0000  ................
+00001fc0: 0e77 0e00 0033 0000 0e54 0e00 002e 0000  .w...3...T......
+00001fd0: 0e4a 0e00 0008 0000 0e40 0e00 0033 0000  .J.......@...3..
+00001fe0: 0e34 0e00 0007 0000 0e2a 0e00 0030 0000  .4.......*...0..
+00001ff0: 0e1c 0e00 002d 0000 0e12 0e00 0031 0000  .....-.......1..
+00002000: 0e06 0e00 0006 0000 0efc 0d00 0032 0000  .............2..
+00002010: 0ec3 0d00 002a 0000 0e84 0d00 002e 0000  .....*..........
+00002020: 0e7a 0d00 0005 0000 0e70 0d00 0030 0000  .z.......p...0..
+00002030: 0e5c 0d00 0040 0000 0e47 0d00 0044 0000  .\...@...G...D..
+00002040: 0e2f 0d00 002c 0000 0e12 0d00 0037 0000  ./...,.......7..
+00002050: 0e08 0d00 0038 0000 0ef2 0c00 0034 0000  .....8.......4..
+00002060: 0ebf 0c00 0020 0000 0e62 0c00 0023 0000  ..... ...b...#..
+00002070: 0e2f 0b00 0029 0000 0eef 0a00 003f 0000  ./...).......?..
+00002080: 0e37 0a00 002b 0000 0e2d 0a00 0004 0000  .7...+...-......
+00002090: 0ef8 0900 0003 0000 0ecf 0900 0002 0000  ................
+000020a0: 0eb3 0900 0001 0000 0e9c 0900 0020 0000  ............. ..
+000020b0: 0e07 0800 0022 0000 0ea7 0700 0020 0000  ....."....... ..
+000020c0: 0ea9 0300 0026 0000 0e56 0300 0021 0000  .....&...V...!..
+000020d0: 0e11 0300 0020 0000 0e9d 0000 0026 0000  ..... .......&..
+000020e0: 0e70 0000 0000 0000 0e31 0000 0021 0000  .p.......1...!..
+000020f0: 0ef0 0000 001e 0000 0ee0 0000 001d 0000  ................
+00002100: 0ed0 0000 001c 0000 0ec0 0000 001b 0000  ................
+00002110: 0eb0 0000 001a 0000 0ea0 0000 0019 0000  ................
+00002120: 0e90 0000 0018 0000 0e80 0000 0017 0000  ................
+00002130: 0e70 0000 0016 0000 0e60 0000 0015 0000  .p.......`......
+00002140: 0e50 0000 0014 0000 0e40 0000 0013 0000  .P.......@......
+00002150: 0e30 0000 0012 0000 0e20 0000 0011 0000  .0....... ......
+00002160: 0e10 0000 0010 0000 0e00 0000 000f 0000  ................
+00002170: 0e60 0000 0001 0000 0640 0000 0001 0000  .`.......@......
+00002180: 0620 0000 0001 0000 0600 0000 0001 0000  . ..............
+00002190: 0607 0900 000e 0200 0060 1300 0000 0000  .........`......
+000021a0: 004c 0900 000e 0200 0000 1300 0000 0000  .L..............
+000021b0: 003a 0c00 000e 0200 0020 1300 0000 0000  .:....... ......
+000021c0: 00a3 0900 000e 0200 0040 1300 0000 0000  .........@......
+000021d0: 0001 0000 000e 0300 0090 1500 0000 0000  ................
+000021e0: 00fb 0300 000e 0300 00c0 1600 0000 0000  ................
+000021f0: 00c3 0000 000e 0300 00f0 1600 0000 0000  ................
+00002200: 008b 0500 000e 0300 00b0 1500 0000 0000  ................
+00002210: 0031 0200 000e 0300 0060 1600 0000 0000  .1.......`......
+00002220: 00fb 0700 000e 0300 0020 1700 0000 0000  ......... ......
+00002230: 00c0 0b00 000e 0300 0060 1700 0000 0000  .........`......
+00002240: 00f6 0900 000e 0200 0080 1300 0000 0000  ................
+00002250: 003b 0a00 000e 0200 00a0 1300 0000 0000  .;..............
+00002260: 00f5 0b00 000e 0200 00c0 1300 0000 0000  ................
+00002270: 00c2 0800 000e 0200 00e0 1300 0000 0000  ................
+00002280: 006e 0900 000e 0300 00b0 1400 0000 0000  .n..............
+00002290: 00d0 0a00 000e 0300 0070 1500 0000 0000  .........p......
+000022a0: 005c 0c00 000e 0300 0000 1400 0000 0000  .\..............
+000022b0: 0098 0b00 000e 0300 0090 1400 0000 0000  ................
+000022c0: 00c5 0900 000e 0300 0040 1800 0000 0000  .........@......
+000022d0: 00f8 0a00 000e 0300 0090 1800 0000 0000  ................
+000022e0: 0029 0900 000e 0300 0090 1700 0000 0000  .)..............
+000022f0: 00a8 0a00 000e 0300 0020 1800 0000 0000  ......... ......
+00002300: 0018 0a00 000e 0300 00d0 1900 0000 0000  ................
+00002310: 0020 0b00 000e 0300 0060 1a00 0000 0000  . .......`......
+00002320: 005d 0a00 000e 0300 0070 1900 0000 0000  .].......p......
+00002330: 0048 0b00 000e 0300 00b0 1900 0000 0000  .H..............
+00002340: 0017 0c00 000e 0300 0010 1900 0000 0000  ................
+00002350: 0070 0b00 000e 0300 0050 1900 0000 0000  .p.......P......
+00002360: 00e4 0800 000e 0300 00b0 1800 0000 0000  ................
+00002370: 0080 0a00 000e 0300 00f0 1800 0000 0000  ................
+00002380: 0091 0900 000f 0180 00e0 1200 0000 0000  ................
+00002390: 00da 0100 000f 01c0 00c0 1200 0000 0000  ................
+000023a0: 00ce 0100 000f 01c0 00f0 1200 0000 0000  ................
+000023b0: 0092 0400 000f 01c0 0050 1100 0000 0000  .........P......
+000023c0: 00d7 0600 000f 0100 0000 0000 0000 0000  ................
+000023d0: 0040 0600 000f 0100 0010 0a00 0000 0000  .@..............
+000023e0: 0066 0700 000f 0100 00b0 0e00 0000 0000  .f..............
+000023f0: 0036 0300 0001 0000 0000 0000 0000 0000  .6..............
+00002400: 0036 0000 0001 0000 0000 0000 0000 0000  .6..............
+00002410: 004d 0000 0001 0000 0000 0000 0000 0000  .M..............
+00002420: 000b 0100 0001 0000 0000 0000 0000 0000  ................
+00002430: 00aa 0100 0001 0000 0000 0000 0000 0000  ................
+00002440: 00a1 0200 0001 0000 0000 0000 0000 0000  ................
+00002450: 00b6 0000 0001 0000 0000 0000 0000 0000  ................
+00002460: 0092 0200 0001 0000 0000 0000 0000 0000  ................
+00002470: 003a 0100 0001 0000 0000 0000 0000 0000  .:..............
+00002480: 00c4 0200 0001 0000 0000 0000 0000 0000  ................
+00002490: 00a2 0000 0001 0000 0000 0000 0000 0000  ................
+000024a0: 00f6 0000 0001 0000 0000 0000 0000 0000  ................
+000024b0: 007e 0000 0001 0000 0000 0000 0000 0000  .~..............
+000024c0: 0091 0000 0001 0000 0000 0000 0000 0000  ................
+000024d0: 002a 0100 0001 0000 0000 0000 0000 0000  .*..............
+000024e0: 004b 0100 0001 0000 0000 0000 0000 0000  .K..............
+000024f0: 00f1 0100 0001 0000 0000 0000 0000 0000  ................
+00002500: 00e6 0100 0001 0000 0000 0000 0000 0000  ................
+00002510: 0026 0000 0001 0000 0000 0000 0000 0000  .&..............
+00002520: 0061 0100 0001 0000 0308 0000 0000 0000  .a..............
+00002530: 0038 0800 0001 0000 0308 0000 0000 0000  .8..............
+00002540: 0028 0400 0001 0000 0308 0000 0000 0000  .(..............
+00002550: 00db 0200 0001 0000 0308 0000 0000 0000  ................
+00002560: 00b0 0300 0001 0000 0308 0000 0000 0000  ................
+00002570: 0056 0300 0001 0000 0308 0000 0000 0000  .V..............
+00002580: 00f2 0400 0001 0000 0308 0000 0000 0000  ................
+00002590: 00fc 0100 0001 0000 0000 0000 0000 0000  ................
+000025a0: 006b 0000 0001 0000 0000 0000 0000 0000  .k..............
+000025b0: 001f 0200 0001 0000 0000 0000 0000 0000  ................
+000025c0: 000c 0200 0001 0000 0000 0000 0000 0000  ................
+000025d0: 00b4 0200 0001 0000 0000 0000 0000 0000  ................
+000025e0: 00e8 0900 0001 0000 0000 0000 0000 0000  ................
+000025f0: 0000 5f2e 636f 6e73 742e 4665 6174 7572  .._.const.Featur
+00002600: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
+00002610: 2e63 6469 7374 005f 5f50 795f 4e6f 6e65  .cdist.__Py_None
+00002620: 5374 7275 6374 005f 4e52 545f 4d65 6d49  Struct._NRT_MemI
+00002630: 6e66 6f5f 6361 6c6c 5f64 746f 7200 5f4e  nfo_call_dtor._N
+00002640: 5254 5f4d 656d 496e 666f 5f6e 6577 5f76  RT_MemInfo_new_v
+00002650: 6172 7369 7a65 5f64 746f 7200 5f6e 756d  arsize_dtor._num
+00002660: 6261 5f66 6174 616c 5f65 7272 6f72 005f  ba_fatal_error._
+00002670: 5079 4578 635f 5379 7374 656d 4572 726f  PyExc_SystemErro
+00002680: 7200 5f50 7945 7863 5f54 7970 6545 7272  r._PyExc_TypeErr
+00002690: 6f72 005f 5079 4578 635f 5275 6e74 696d  or._PyExc_Runtim
+000026a0: 6545 7272 6f72 005f 5079 4572 725f 436c  eError._PyErr_Cl
+000026b0: 6561 7200 5f2e 636f 6e73 742e 756e 6b6e  ear._.const.unkn
+000026c0: 6f77 6e20 6572 726f 7220 7768 656e 2063  own error when c
+000026d0: 616c 6c69 6e67 206e 6174 6976 6520 6675  alling native fu
+000026e0: 6e63 7469 6f6e 005f 5079 4578 635f 5374  nction._PyExc_St
+000026f0: 6f70 4974 6572 6174 696f 6e00 5f4e 5254  opIteration._NRT
+00002700: 5f61 6461 7074 5f6e 6461 7272 6179 5f66  _adapt_ndarray_f
+00002710: 726f 6d5f 7079 7468 6f6e 005f 5079 4c69  rom_python._PyLi
+00002720: 7374 5f47 6574 4974 656d 005f 5079 4572  st_GetItem._PyEr
+00002730: 725f 5365 7453 7472 696e 6700 5f50 7955  r_SetString._PyU
+00002740: 6e69 636f 6465 5f46 726f 6d53 7472 696e  nicode_FromStrin
+00002750: 6700 5f5f 5a4e 3038 4e75 6d62 6145 6e76  g.__ZN08NumbaEnv
+00002760: 3133 2433 6364 796e 616d 6963 2433 6533  13$3cdynamic$3e3
+00002770: 385f 5f6e 756d 6261 5f61 7272 6179 5f65  8__numba_array_e
+00002780: 7870 725f 3078 3766 3935 3535 3530 3965  xpr_0x7f9555509e
+00002790: 3130 2432 3436 3445 6666 005f 4e52 545f  10$2464Eff._NRT_
+000027a0: 6164 6170 745f 6e64 6172 7261 795f 746f  adapt_ndarray_to
+000027b0: 5f70 7974 686f 6e5f 6163 7172 6566 005f  _python_acqref._
+000027c0: 4e52 545f 696e 6372 6566 005f 4e52 545f  NRT_incref._NRT_
+000027d0: 6465 6372 6566 005f 5079 5f49 6e63 5265  decref._Py_IncRe
+000027e0: 6600 5f50 795f 4465 6352 6566 005f 6e75  f._Py_DecRef._nu
+000027f0: 6d62 615f 646f 5f72 6169 7365 005f 6e75  mba_do_raise._nu
+00002800: 6d62 615f 6769 6c5f 7265 6c65 6173 6500  mba_gil_release.
+00002810: 5f6e 756d 6261 5f67 696c 5f65 6e73 7572  _numba_gil_ensur
+00002820: 6500 5f2e 636f 6e73 742e 6361 6e27 7420  e._.const.can't 
+00002830: 756e 626f 7820 6172 7261 7920 6672 6f6d  unbox array from
+00002840: 2050 794f 626a 6563 7420 696e 746f 206e   PyObject into n
+00002850: 6174 6976 6520 7661 6c75 652e 2020 5468  ative value.  Th
+00002860: 6520 6f62 6a65 6374 206d 6179 6265 206f  e object maybe o
+00002870: 6620 6120 6469 6666 6572 656e 7420 7479  f a different ty
+00002880: 7065 005f 5079 4572 725f 5365 744e 6f6e  pe._PyErr_SetNon
+00002890: 6500 5f50 7941 7267 5f55 6e70 6163 6b54  e._PyArg_UnpackT
+000028a0: 7570 6c65 005f 6e75 6d62 615f 756e 7069  uple._numba_unpi
+000028b0: 636b 6c65 005f 5079 4572 725f 5772 6974  ckle._PyErr_Writ
+000028c0: 6555 6e72 6169 7361 626c 6500 5f5f 5a4e  eUnraisable.__ZN
+000028d0: 3038 4e75 6d62 6145 6e76 356e 756d 6261  08NumbaEnv5numba
+000028e0: 326e 7036 6c69 6e61 6c67 3235 5f64 756d  2np6linalg25_dum
+000028f0: 6d79 5f6c 6976 656e 6573 735f 6675 6e63  my_liveness_func
+00002900: 2432 3432 3945 3330 6c69 7374 2432 3869  $2429E30list$28i
+00002910: 6e74 3634 2432 3924 3363 6976 2433 644e  nt64$29$3civ$3dN
+00002920: 6f6e 6524 3365 005f 4e52 545f 4d65 6d49  one$3e._NRT_MemI
+00002930: 6e66 6f5f 616c 6c6f 635f 7361 6665 5f61  nfo_alloc_safe_a
+00002940: 6c69 676e 6564 005f 5f5a 4e30 384e 756d  ligned.__ZN08Num
+00002950: 6261 456e 7635 6e75 6d62 6132 6e70 3861  baEnv5numba2np8a
+00002960: 7272 6179 6f62 6a31 336e 756d 7079 5f66  rrayobj13numpy_f
+00002970: 756c 6c5f 6e64 3132 2433 636c 6f63 616c  ull_nd12$3clocal
+00002980: 7324 3365 3966 756c 6c24 3234 3633 4538  s$3e9full$2463E8
+00002990: 556e 6954 7570 6c65 4978 4c69 3245 4564  UniTupleIxLi2EEd
+000029a0: 005f 5f5a 4e30 384e 756d 6261 456e 7635  .__ZN08NumbaEnv5
+000029b0: 6e75 6d62 6132 6e70 376e 7079 696d 706c  numba2np7npyimpl
+000029c0: 3230 5f62 726f 6164 6361 7374 5f6f 6e74  20_broadcast_ont
+000029d0: 6f24 3234 3130 4578 3869 6e74 3634 2432  o$2410Ex8int64$2
+000029e0: 6178 3869 6e74 3634 2432 6100 5f2e 636f  ax8int64$2a._.co
+000029f0: 6e73 742e 6065 6e76 2e63 6f6e 7374 7360  nst.`env.consts`
+00002a00: 2069 7320 4e55 4c4c 2069 6e20 6072 6561   is NULL in `rea
+00002a10: 645f 636f 6e73 7460 005f 5f5a 4e30 384e  d_const`.__ZN08N
+00002a20: 756d 6261 456e 7635 6e75 6d62 6132 6e70  umbaEnv5numba2np
+00002a30: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
+00002a40: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
+00002a50: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
+00002a60: 3632 4535 4172 7261 7949 664c 6931 4531  62E5ArrayIfLi1E1
+00002a70: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
+00002a80: 6445 005f 5f5a 4e35 6e75 6d62 6132 6e70  dE.__ZN5numba2np
+00002a90: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
+00002aa0: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
+00002ab0: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
+00002ac0: 3632 4535 4172 7261 7949 664c 6931 4531  62E5ArrayIfLi1E1
+00002ad0: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
+00002ae0: 6445 005f 5f5a 4e30 384e 756d 6261 456e  dE.__ZN08NumbaEn
+00002af0: 7635 7369 6d62 6136 6d69 7869 6e73 3234  v5simba6mixins24
+00002b00: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
+00002b10: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
+00002b20: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
+00002b30: 3130 6364 6973 7424 3234 3630 4535 4172  10cdist$2460E5Ar
+00002b40: 7261 7949 664c 6932 4531 4137 6d75 7461  rayIfLi2E1A7muta
+00002b50: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
+00002b60: 6179 4966 4c69 3245 3141 376d 7574 6162  ayIfLi2E1A7mutab
+00002b70: 6c65 3761 6c69 676e 6564 4500 5f2e 636f  le7alignedE._.co
+00002b80: 6e73 742e 6d69 7373 696e 6720 456e 7669  nst.missing Envi
+00002b90: 726f 6e6d 656e 743a 205f 5a4e 3038 4e75  ronment: _ZN08Nu
+00002ba0: 6d62 6145 6e76 3573 696d 6261 366d 6978  mbaEnv5simba6mix
+00002bb0: 696e 7332 3466 6561 7475 7265 5f65 7874  ins24feature_ext
+00002bc0: 7261 6374 696f 6e5f 6d69 7869 6e32 3246  raction_mixin22F
+00002bd0: 6561 7475 7265 4578 7472 6163 7469 6f6e  eatureExtraction
+00002be0: 4d69 7869 6e31 3063 6469 7374 2432 3436  Mixin10cdist$246
+00002bf0: 3045 3541 7272 6179 4966 4c69 3245 3141  0E5ArrayIfLi2E1A
+00002c00: 376d 7574 6162 6c65 3761 6c69 676e 6564  7mutable7aligned
+00002c10: 4535 4172 7261 7949 664c 6932 4531 4137  E5ArrayIfLi2E1A7
+00002c20: 6d75 7461 626c 6537 616c 6967 6e65 6445  mutable7alignedE
+00002c30: 005f 5f5a 4e37 6370 7974 686f 6e35 7369  .__ZN7cpython5si
+00002c40: 6d62 6136 6d69 7869 6e73 3234 6665 6174  mba6mixins24feat
+00002c50: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
+00002c60: 6978 696e 3232 4665 6174 7572 6545 7874  ixin22FeatureExt
+00002c70: 7261 6374 696f 6e4d 6978 696e 3130 6364  ractionMixin10cd
+00002c80: 6973 7424 3234 3630 4535 4172 7261 7949  ist$2460E5ArrayI
+00002c90: 664c 6932 4531 4137 6d75 7461 626c 6537  fLi2E1A7mutable7
+00002ca0: 616c 6967 6e65 6445 3541 7272 6179 4966  alignedE5ArrayIf
+00002cb0: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
+00002cc0: 6c69 676e 6564 4500 5f5f 5a4e 3573 696d  lignedE.__ZN5sim
+00002cd0: 6261 366d 6978 696e 7332 3466 6561 7475  ba6mixins24featu
+00002ce0: 7265 5f65 7874 7261 6374 696f 6e5f 6d69  re_extraction_mi
+00002cf0: 7869 6e32 3246 6561 7475 7265 4578 7472  xin22FeatureExtr
+00002d00: 6163 7469 6f6e 4d69 7869 6e31 3063 6469  actionMixin10cdi
+00002d10: 7374 2432 3436 3045 3541 7272 6179 4966  st$2460E5ArrayIf
+00002d20: 4c69 3245 3141 376d 7574 6162 6c65 3761  Li2E1A7mutable7a
+00002d30: 6c69 676e 6564 4535 4172 7261 7949 664c  lignedE5ArrayIfL
+00002d40: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
+00002d50: 6967 6e65 6445 005f 6366 756e 632e 5f5a  ignedE._cfunc._Z
+00002d60: 4e35 7369 6d62 6136 6d69 7869 6e73 3234  N5simba6mixins24
+00002d70: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
+00002d80: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
+00002d90: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
+00002da0: 3130 6364 6973 7424 3234 3630 4535 4172  10cdist$2460E5Ar
+00002db0: 7261 7949 664c 6932 4531 4137 6d75 7461  rayIfLi2E1A7muta
+00002dc0: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
+00002dd0: 6179 4966 4c69 3245 3141 376d 7574 6162  ayIfLi2E1A7mutab
+00002de0: 6c65 3761 6c69 676e 6564 4500 5f2e 636f  le7alignedE._.co
+00002df0: 6e73 742e 3c6e 756d 6261 2e63 6f72 652e  nst.<numba.core.
+00002e00: 6370 752e 4350 5543 6f6e 7465 7874 206f  cpu.CPUContext o
+00002e10: 626a 6563 7420 6174 2030 7837 6639 3535  bject at 0x7f955
+00002e20: 3535 3036 3934 303e 005f 5f5a 4e30 384e  5506940>.__ZN08N
+00002e30: 756d 6261 456e 7635 6e75 6d62 6132 6e70  umbaEnv5numba2np
+00002e40: 366c 696e 616c 6731 345f 6765 745f 6e6f  6linalg14_get_no
+00002e50: 726d 5f69 6d70 6c31 3224 3363 6c6f 6361  rm_impl12$3cloca
+00002e60: 6c73 2433 6531 346f 6e65 445f 696d 706c  ls$3e14oneD_impl
+00002e70: 2432 3436 3145 3541 7272 6179 4966 4c69  $2461E5ArrayIfLi
+00002e80: 3145 3143 376d 7574 6162 6c65 3761 6c69  1E1C7mutable7ali
+00002e90: 676e 6564 4532 376f 6d69 7474 6564 2432  gnedE27omitted$2
+00002ea0: 3864 6566 6175 6c74 2433 644e 6f6e 6524  8default$3dNone$
+00002eb0: 3239 005f 2e63 6f6e 7374 2e70 6963 6b6c  29._.const.pickl
+00002ec0: 6562 7566 2e31 3430 3237 3938 3930 3130  ebuf.14027989010
+00002ed0: 3834 3838 005f 2e63 6f6e 7374 2e70 6963  8488._.const.pic
+00002ee0: 6b6c 6564 6174 612e 3134 3032 3739 3839  kledata.14027989
+00002ef0: 3031 3038 3438 3800 5f2e 636f 6e73 742e  0108488._.const.
+00002f00: 7069 636b 6c65 6275 662e 3134 3032 3739  picklebuf.140279
+00002f10: 3836 3938 3838 3639 3600 5f2e 636f 6e73  869888696._.cons
+00002f20: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
+00002f30: 3237 3938 3639 3838 3836 3936 005f 2e63  279869888696._.c
+00002f40: 6f6e 7374 2e70 6963 6b6c 6562 7566 2e31  onst.picklebuf.1
+00002f50: 3430 3237 3938 3738 3330 3532 3536 005f  40279878305256._
+00002f60: 2e63 6f6e 7374 2e70 6963 6b6c 6564 6174  .const.pickledat
+00002f70: 612e 3134 3032 3739 3837 3833 3035 3235  a.14027987830525
+00002f80: 3600 5f2e 6474 6f72 2e6c 6973 742e 696e  6._.dtor.list.in
+00002f90: 7436 3400 5f2e 636f 6e73 742e 7069 636b  t64._.const.pick
+00002fa0: 6c65 6275 662e 3134 3032 3739 3837 3638  lebuf.1402798768
+00002fb0: 3533 3930 3400 5f2e 636f 6e73 742e 7069  53904._.const.pi
+00002fc0: 636b 6c65 6461 7461 2e31 3430 3237 3938  ckledata.1402798
+00002fd0: 3736 3835 3339 3034 005f 6e75 6d62 615f  76853904._numba_
+00002fe0: 7878 6e72 6d32 005f 2e63 6f6e 7374 2e70  xxnrm2._.const.p
+00002ff0: 6963 6b6c 6562 7566 2e31 3430 3237 3938  icklebuf.1402798
+00003000: 3733 3237 3031 3932 005f 2e63 6f6e 7374  73270192._.const
+00003010: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00003020: 3739 3837 3332 3730 3139 3200 5f2e 636f  79873270192._.co
+00003030: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
+00003040: 3032 3739 3837 3638 3534 3931 3200 5f2e  0279876854912._.
+00003050: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
+00003060: 2e31 3430 3237 3938 3736 3835 3439 3132  .140279876854912
+00003070: 005f 2e63 6f6e 7374 2e70 6963 6b6c 6564  ._.const.pickled
+00003080: 6174 612e 3134 3032 3739 3839 3031 3038  ata.140279890108
+00003090: 3438 382e 7368 6131 005f 2e63 6f6e 7374  488.sha1._.const
+000030a0: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+000030b0: 3739 3836 3938 3838 3639 362e 7368 6131  79869888696.sha1
+000030c0: 005f 2e63 6f6e 7374 2e70 6963 6b6c 6564  ._.const.pickled
+000030d0: 6174 612e 3134 3032 3739 3837 3833 3035  ata.140279878305
+000030e0: 3235 362e 7368 6131 005f 2e63 6f6e 7374  256.sha1._.const
+000030f0: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00003100: 3739 3837 3638 3533 3930 342e 7368 6131  79876853904.sha1
+00003110: 005f 2e63 6f6e 7374 2e70 6963 6b6c 6564  ._.const.pickled
+00003120: 6174 612e 3134 3032 3739 3837 3332 3730  ata.140279873270
+00003130: 3139 322e 7368 6131 005f 2e63 6f6e 7374  192.sha1._.const
+00003140: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00003150: 3739 3837 3638 3534 3931 322e 7368 6131  79876854912.sha1
+00003160: 005f 2e63 6f6e 7374 2e70 6963 6b6c 6564  ._.const.pickled
+00003170: 6174 612e 3134 3032 3739 3837 3638 3534  ata.140279876854
+00003180: 3834 302e 7368 6131 005f 2e63 6f6e 7374  840.sha1._.const
+00003190: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+000031a0: 3739 3837 3833 3034 3332 302e 7368 6131  79878304320.sha1
+000031b0: 005f 2e63 6f6e 7374 2e75 6e6b 6e6f 776e  ._.const.unknown
+000031c0: 2065 7272 6f72 2077 6865 6e20 6361 6c6c   error when call
+000031d0: 696e 6720 6e61 7469 7665 2066 756e 6374  ing native funct
+000031e0: 696f 6e2e 3100 5f2e 636f 6e73 742e 7069  ion.1._.const.pi
+000031f0: 636b 6c65 6275 662e 3134 3032 3739 3837  cklebuf.14027987
+00003200: 3638 3534 3834 3000 5f2e 636f 6e73 742e  6854840._.const.
+00003210: 7069 636b 6c65 6461 7461 2e31 3430 3237  pickledata.14027
+00003220: 3938 3736 3835 3438 3430 005f 2e63 6f6e  9876854840._.con
+00003230: 7374 2e70 6963 6b6c 6562 7566 2e31 3430  st.picklebuf.140
+00003240: 3237 3938 3738 3330 3433 3230 005f 2e63  279878304320._.c
+00003250: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
+00003260: 3134 3032 3739 3837 3833 3034 3332 3000  140279878304320.
+00003270: 0094 4220 6d00 00de c017 0b00 0000 0014  ..B m...........
+00003280: 0000 000c 6d00 0007 0000 0142 43c0 de35  ....m......BC..5
+00003290: 1400 0005 0000 0062 0c30 244a 59be 664d  .......b.0$JY.fM
+000032a0: fbb4 5f0b 5180 4c01 0000 0021 0c00 00df  .._.Q.L....!....
+000032b0: 1200 000b 0221 0002 0000 0016 0000 0007  .....!..........
+000032c0: 8123 9141 c804 4906 1032 3992 0184 0c25  .#.A..I..29....%
+000032d0: 0508 191e 048b 6280 1c45 0242 920b 42e4  ......b..E.B..B.
+000032e0: 1032 1438 0818 4b0a 3272 8848 70c4 2123  .2.8..K.2r.Hp.!#
+000032f0: 4412 878c 1041 9202 64c8 08b1 1420 4346  D....A..d.... CF
+00003300: 8820 c901 3272 8418 2a28 2a90 317c b05c  . ..2r..*(*.1|.\
+00003310: 9120 c7c8 0000 0089 2000 0050 0000 0032  . ...... ..P...2
+00003320: 22c8 0920 6485 0493 23a4 8404 9323 e384  ".. d...#....#..
+00003330: a190 1412 4c8e 8c0b 84e4 4c10 acc3 1c01  ....L.....L.....
+00003340: 4200 0acc 1180 8119 0283 0011 7230 0040  B...........r0.@
+00003350: 86a4 0010 226d 0300 a4c8 0e00 31b2 3500  ...."m......1.5.
+00003360: 408e cc02 1024 4b00 24c9 1500 51b2 0640  @....$K.$...Q..@
+00003370: 963c 0210 2679 00a4 c91e 0071 f207 409e  .<..&y.....q..@.
+00003380: 5c0c 0010 688e 0014 8600 6894 0222 7304  \...h.....h.."s.
+00003390: 0222 11a9 5422 1315 6600 2855 aac1 0915  ."..T"..f.(U....
+000033a0: 0888 442a 9148 240a 0444 2295 4824 12d1  ..D*.H$..D".H$..
+000033b0: 6a8e 2030 82a8 5506 9748 44af 3204 4403  j. 0..U..HD.2.D.
+000033c0: 8a15 2210 0804 6856 8b41 2020 1251 6d04  .."...hV.A  .Qm.
+000033d0: a00c b740 8070 6518 0402 a42b c22d 40bc  ...@.pe....+.-@.
+000033e0: 3204 0222 f295 2210 180c 0204 2cc1 8d84  2.."..".....,...
+000033f0: 8508 0406 0122 9a23 1010 8954 a552 194c  .....".#...T.R.L
+00003400: 4623 1d69 5084 5b92 9445 0804 8859 9481  F#.iP.[..E...Y..
+00003410: 0a15 0888 442a 9188 9c25 1810 b418 0380  ....D*...%......
+00003420: 4825 5291 b40c 0151 80a8 a5b8 0500 a216  H%R....Q........
+00003430: 59cb 7013 0508 5b86 5b40 40da 8180 2900  Y.p...[.[@@...).
+00003440: 2291 8854 c308 481a 0c23 2003 85c9 388c  "..T..H..# ...8.
+00003450: 4088 0195 0d21 1201 4474 2634 7d01 0051  @....!..Dt&4}..Q
+00003460: 1800 002d 0000 001b 8c20 0012 60d9 6008  ...-..... ..`.`.
+00003470: 0290 00cb 0663 2080 05a0 3618 4403 2c00  .....c ...6.D.,.
+00003480: b541 29fe ffff ff7f 0024 8002 ea00 e883  .A)......$......
+00003490: 0d84 0100 c906 e308 8005 a036 18c8 002c  ...........6...,
+000034a0: 00b5 8148 0260 d940 2802 b06c 2096 ffff  ...H.`.@(..l ...
+000034b0: ffff 1f00 6703 c2fc ffff ffff 00b4 0120  ....g.......... 
+000034c0: 017d b0c1 6802 6001 e860 03e1 1000 1f6c  .}..h.`..`.....l
+000034d0: 509e ffff ffff 1f00 3f00 1c00 0e00 6903  P.......?.....i.
+000034e0: 0105 001f 6c20 a2ff ffff ff1f 0069 0321  ....l .......i.!
+000034f0: 09c0 196c 20a6 0038 830d 0455 0067 b081  ...l ..8...U.g..
+00003500: a80c e00c 3628 5600 9c41 1020 411a a0c2  ....6(V..A. A...
+00003510: 06e5 0a80 3308 8220 4803 0849 1800 0010  ....3.. H..I....
+00003520: 0000 0013 8840 1888 0941 3121 3026 0807  .....@...A1!0&..
+00003530: 3241 4894 0941 3281 0804 6498 102c 1306  2AH..A2...d..,..
+00003540: a671 2604 cf84 8181 9409 4134 2190 2608  .q&.......A4!.&.
+00003550: 9334 41a0 aa09 8135 2198 260c cb24 4d08  .4A....5!.&..$M.
+00003560: 2e00 0013 327c c003 3bf8 053b a083 3608  ....2|..;..;..6.
+00003570: 0778 8007 7628 8736 2087 7090 877b 4807  .x..v(.6 .p..{H.
+00003580: 7788 833c 7003 3b70 0338 d860 0ae5 d006  w..<p.;p.8.`....
+00003590: eda0 07ef d006 f020 0777 0007 7a30 0772  ....... .w..z0.r
+000035a0: a007 7320 076d 000f 7270 0771 a007 7320  ..s .m..rp.q..s 
+000035b0: 077a 3007 72d0 06f0 2007 7720 077a 6007  .z0.r... .w .z`.
+000035c0: 74a0 0776 4007 6d90 0e76 4007 7a60 0774  t..v@.m..v@.z`.t
+000035d0: d006 e680 0770 a007 7120 0778 d006 ee80  .....p..q .x....
+000035e0: 077a 1007 76a0 0773 2007 7a60 0774 d006  .z..v..s .z`.t..
+000035f0: b310 0772 8007 4a0f 0811 1243 868c 9400  ...r..J....C....
+00003600: 0134 4298 9c22 bc39 5d9e 769f 7d3b 24e0  .4B..".9].v.};$.
+00003610: 2602 2117 1000 0000 0100 0000 b809 6087  &.!...........`.
+00003620: 7413 6040 0cea 3000 0000 0000 0000 c14d  t.`@..0........M
+00003630: 003b a4bb 0003 6258 8701 0000 0000 0000  .;....bX........
+00003640: 086e 02d8 21dd 4618 1883 3c0c 0000 0000  .n..!.F...<.....
+00003650: 0000 4070 13c0 0e09 3fcc 0019 e661 0000  ..@p....?....a..
+00003660: 0000 0000 0082 9b00 7648 3e12 06ca a00f  ........vH>.....
+00003670: 0300 0000 0000 0010 dc04 b043 fa13 3340  ...........C..3@
+00003680: 067a 1800 0000 0000 0080 e026 801d 52b9  .z.........&..R.
+00003690: 8c01 33ec c300 0000 0000 0000 0437 0110  ..3..........7..
+000036a0: 7140 0210 00b0 43d2 99b9 7006 7e18 0000  q@....C...p.~...
+000036b0: 0000 0000 80e0 2600 3613 3c00 0200 7648  ......&.6.<...vH
+000036c0: bcf4 0bd0 d00f 0300 0000 0000 0010 dc04  ................
+000036d0: c0dd 0207 4000 c00e 29b5 d640 1afc 6100  ....@...)..@..a.
+000036e0: 0000 0000 0000 829b 0048 5f30 0108 00e0  .........H_0....
+000036f0: a141 0420 0060 8784 6371 400d ff30 0000  .A. .`..cq@..0..
+00003700: 0000 0000 00c1 4d00 3ba4 54db 036b 0089  ......M.;.T..k..
+00003710: 0100 0000 0000 0008 6e02 d821 91dc 1c50  ........n..!...P
+00003720: c33f 0c00 0000 0000 0040 7013 c00e e9ee  .?.......@p.....
+00003730: 7021 1072 0101 0000 1000 0000 809b 0076  p!.r...........v
+00003740: 482f 1880 0131 b0c3 0000 0000 0000 0004  H/...1..........
+00003750: 3701 ec90 de30 0003 6268 8701 0000 0000  7....0..bh......
+00003760: 0000 086e 02d8 21bd 6210 06c6 200f 0300  ...n..!.b... ...
+00003770: 0000 0000 0010 dc04 b043 82c7 c00c 9061  .........C.....a
+00003780: 1e06 0000 0000 0000 20b8 0960 8764 9341  ........ ..`.d.A
+00003790: 1860 4348 0c00 0000 0000 0040 7013 c00e  .`CH.......@p...
+000037a0: e92e 0333 4086 7a18 0000 0000 0000 80e0  ...3@.z.........
+000037b0: 2680 1d52 6f06 a710 08b9 8000 0000 0800  &..Ro...........
+000037c0: 0000 c04d 003b 2432 0d52 2110 7201 0100  ...M.;$2.R!.r...
+000037d0: 0010 0000 0080 9b00 7648 ed1a a044 20e4  ........vH...D .
+000037e0: 0202 0000 2000 0000 0037 01ec 90ea 3740  .... ....7....7@
+000037f0: 8740 c805 0400 0040 0000 0000 6e02 d821  .@.....@....n..!
+00003800: f572 900b 8190 0b08 0000 8000 0000 00dc  .r..............
+00003810: 04b0 43b2 eb00 0c88 c11d 0600 0000 0000  ..C.............
+00003820: 0020 b809 6087 64db 0118 10c3 3b0c 0000  . ..`.d.....;...
+00003830: 0000 0000 4070 13c0 0ec9 be03 3020 0678  ....@p......0 .x
+00003840: 1800 0000 0000 0080 e026 801d 928d 0760  .........&.....`
+00003850: 400c f130 0000 0000 0000 00c1 4d00 3b24  @..0........M.;$
+00003860: 3b0f c240 1b44 6200 0000 0000 0000 829b  ;..@.Db.........
+00003870: 0076 48b7 1e98 0132 d8c3 0000 0000 0000  .vH....2........
+00003880: 0004 3701 ec90 fa3d 0803 6e18 8901 0000  ..7....=..n.....
+00003890: 0000 0000 086e 02d8 21f9 7c60 06c8 700f  .....n..!.|`..p.
+000038a0: 0300 0000 0000 0010 dc04 b043 22fd 200c  ...........C". .
+000038b0: bc81 2406 0000 0000 0000 20b8 0960 8754  ..$....... ..`.T
+000038c0: fe81 1920 033e 0c00 0000 0000 0040 7013  ... .>.......@p.
+000038d0: c00e 6905 8530 0083 a124 0600 0000 0000  ..i..0...$......
+000038e0: 0020 b809 6087 c486 8219 2043 3e0c 0000  . ..`..... C>...
+000038f0: 0000 0000 4070 13c0 904a 1685 9658 0300  ....@p...J...X..
+00003900: 9802 0000 0001 0000 0000 809b 0086 54bf  ..............T.
+00003910: 296c 6f00 0480 0000 0000 0000 0000 0070  )lo............p
+00003920: 13c0 904a 3f05 2f0e 8000 1800 0000 0400  ...J?./.........
+00003930: 0000 0000 6e02 1852 e1a8 5013 7300 0013  ....n..R..P.s...
+00003940: 0100 0020 0000 0000 0070 13c0 90aa 6d85  ... .....p....m.
+00003950: a80e 8000 0000 0000 0400 0000 0000 6e02  ..............n.
+00003960: 1852 f9ad f0e0 0110 0000 0000 8000 0000  .R..............
+00003970: 0000 c04d 0043 aad6 153a 3d00 02a0 0000  ...M.C...:=.....
+00003980: 0010 0000 0000 00b8 0960 48a5 be42 c207  .........`H..B..
+00003990: 4000 0000 0000 0200 0000 0000 3701 0ca9  @...........7...
+000039a0: e657 70fc 0008 0000 0000 4000 0000 0000  .Wp.......@.....
+000039b0: e026 8021 5508 0b62 000a 4000 1800 0000  .&.!U..b..@.....
+000039c0: 0200 0000 0000 3701 0ca9 c658 5844 0108  ......7....XXD..
+000039d0: 0000 0000 4000 0000 0000 e026 8021 951b  ....@......&.!..
+000039e0: 0b0e 2900 0100 0000 0008 0000 0000 00dc  ..).............
+000039f0: 0430 a4e2 63c1 e103 2000 0000 0000 0100  .0..c... .......
+00003a00: 0000 0080 9b00 8654 aa2c 347c 0004 0000  .......T.,4|....
+00003a10: 0000 2000 0000 0000 7013 c090 ea96 8599  .. .....p.......
+00003a20: 3805 0098 0000 0000 0100 0000 0080 9b00  8...............
+00003a30: 8654 ea2d 40aa 0004 0000 0000 2000 0000  .T.-@....... ...
+00003a40: 0000 7013 c090 4abf 058a 1580 0000 0000  ..p...J.........
+00003a50: 0004 0000 0000 006e 0218 52b9 b850 f101  .......n..R..P..
+00003a60: 1000 0000 0080 0000 0000 00c0 4d00 43aa  ............M.C.
+00003a70: 3117 123e 0002 0000 0000 1000 0000 0000  1..>............
+00003a80: b809 6048 c5e6 42a4 0a40 0000 0000 0002  ..`H..B..@......
+00003a90: 0000 0000 0037 010c a9fa 5cf0 0557 0080  .....7....\..W..
+00003aa0: e900 0000 1000 0000 0000 b809 6048 b5f3  ............`H..
+00003ab0: 82c2 0700 3021 0000 0002 0000 0000 0037  ....0!.........7
+00003ac0: 010c a9ca 5e88 6001 0800 0000 0040 0000  ....^.`......@..
+00003ad0: 0000 00e0 2680 2195 dd0b 8c2c 0001 0000  ....&.!....,....
+00003ae0: 0000 0800 0000 0000 dc04 30a4 127d 01e2  ..........0..}..
+00003af0: 0300 9800 0000 0000 0000 0000 809b 0086  ................
+00003b00: 54b2 2f70 b400 0400 0000 0020 0000 0000  T./p....... ....
+00003b10: 0070 13c0 90ca fd05 ca16 8000 4800 0000  .p..........H...
+00003b20: 0000 0000 0000 6e02 1852 89e0 50f1 0110  ......n..R..P...
+00003b30: 0000 0000 8000 0000 0000 c04d 0043 aa1b  ...........M.C..
+00003b40: 1c14 3e00 8049 0100 0010 0000 0000 00b8  ..>..I..........
+00003b50: 0960 4815 8603 860b 4000 2c00 0000 0000  .`H.....@.,.....
+00003b60: 0000 0000 3701 0ca9 f270 b070 0108 8005  ....7....p.p....
+00003b70: 0000 0000 0000 0000 e026 8021 d52b 0e93  .........&.!.+..
+00003b80: 2e00 01c0 0000 0000 0000 0000 00dc 0420  ............... 
+00003b90: b141 a0b0 b704 0040 1608 0076 0100 0032  .A.....@...v...2
+00003ba0: 1e98 2019 114c 908c 0926 47c6 0443 1a8c  .. ..L...&G..C..
+00003bb0: 0094 a140 b10b 9463 4059 0a94 5fe9 155e  ...@...c@Y.._..^
+00003bc0: 390e 9464 6640 0994 7100 b56a 8002 2300  9..df@..q..j..#.
+00003bd0: 431d ca52 0cab 30ac c250 0792 18c3 2a0c  C..R..0..P....*.
+00003be0: ab30 d461 1cc3 b00a c32a 0c75 2009 31ac  .0.a.....*.u .1.
+00003bf0: c2b0 0a43 1d58 860d ab30 acc2 5007 9264  ...C.X...0..P..d
+00003c00: c32a 0cab 30d4 611c d6b0 0ac3 2a0c 7520  .*..0.a.....*.u 
+00003c10: c935 acc2 b00a 431d 6010 0669 30ac c2b0  .5....C.`..i0...
+00003c20: 0a43 1d48 a206 c32a 0cab 30d4 e17d 6730  .C.H...*..0..}g0
+00003c30: acc2 b00a 431d 4882 06c3 2a0c ab30 d4c1  ....C.H...*..0..
+00003c40: 7565 30ac c2b0 0a43 1d48 6206 c32a 0cab  ue0....C.Hb..*..
+00003c50: 30d4 a16d 6330 acc2 b00a 431d 4842 06c3  0..mc0....C.HB..
+00003c60: 2a0c ab40 041c b29a b470 d862 e2c2 a1cb  *..@.....p.b....
+00003c70: c90b 872f 2630 1cc2 9ec4 7018 8322 c3a1  .../&0....p.."..
+00003c80: 2cca 0c87 3329 3432 e448 000e 8c89 d5a5  ,...3)42.H......
+00003c90: b1d1 a5b9 cd29 5885 b1d5 9515 c9c9 bdc9  .....)X.........
+00003ca0: 29c4 0160 6d01 0000 84c9 c985 e581 a4cd  )..`m...........
+00003cb0: 81d0 bdbd 8188 a59d ed80 8085 c9c9 b9cc  ................
+00003cc0: a5e9 9581 a880 84c9 c9b9 90d1 e5c1 95b9  ................
+00003cd0: a4d1 95b5 cda5 e995 8181 a4cd 81b0 85c9  ................
+00003ce0: 9d95 c981 d0a1 85b9 81d0 a195 81b4 85e1  ................
+00003cf0: a5b5 d5b5 81c0 bdcd cda5 89b1 9581 cca5  ................
+00003d00: e995 b9c4 0514 c609 381d c60d b810 2229  ........8.....")
+00003d10: 9b1b 1c78 5469 71b0 b87d a874 e98d 25c0  ...xTiq..}.t..%.
+00003d20: d4a9 1783 a4a0 94e2 51d3 51f4 c534 765b  ........Q.Q..4v[
+00003d30: 7a5d d2b5 0c84 74ee 6993 72d5 c604 674b  z]....t.i.r...gK
+00003d40: ba6d 6d8c c1be ff15 6f93 e372 a7ed 4f0a  .mm.....o..r..O.
+00003d50: e4a0 7c4a 8ca6 8331 36e6 944d f31f 9d4c  ..|J...16..M...L
+00003d60: af17 b52d 2977 51c0 abda d173 550e d7ec  ...-)wQ....sU...
+00003d70: 214d 710f 716e 06bd cda4 fc6e 52e1 3815  !Mq.qn.....nR.8.
+00003d80: 00f3 ba29 4fb2 06fb 20e5 2757 5c6d 924a  ...)O... .'W\m.J
+00003d90: fad0 bc08 6205 bf0b c00f 812e cfc8 4844  ....b.........HD
+00003da0: 5fcd ef24 45da 05e0 c098 585d 1a1b 5d9a  _..$E.....X]..].
+00003db0: db9c 8255 185b 5d59 919c dc9b 9c42 1c00  ...U.[]Y.....B..
+00003dc0: 9623 0000 409d 5b98 185b 1908 dd1b 8898  .#..@.[..[......
+00003dd0: dc5b 18d9 58d8 1c1d 4898 dc59 5d5b 991b  .[..X...H..Y][..
+00003de0: 1d48 0c08 dd1b c85b 1d1d 5c1d 1d48 989c  .H.....[..\..H..
+00003df0: 5c58 9e82 511a 5b19 88c8 4bd5 5c99 dcdc  \X..Q.[...K.\...
+00003e00: cb5c 5adb 9bdb 0b51 d9dc 1add 1bdc 4b99  .\Z....Q......K.
+00003e10: 9bdd dccb 5c5a 9b58 d817 5999 ddcb 5c5a  ....\Z.X..Y...\Z
+00003e20: 9b58 d84b 5b1a 5e9a dbdc 8b59 5918 5d9d  .X.K[.^....YY.].
+00003e30: 5cd9 5719 1e9d 5cd8 185d da9b db57 5b1a  \.W...\..]...W[.
+00003e40: 5e9a 9b0b 5c9e 080b 085b 9a5b 19c8 4c4d  ^...\....[.[..LM
+00003e50: 0d0b 485c 4061 9c80 d361 dc80 0b31 96fb  ..H\@a...a...1..
+00003e60: 0860 a222 c2bb a608 1026 c469 4ce4 421a  .`.".....&.iL.B.
+00003e70: 5f18 1069 2287 b245 3b3d 9fa7 dd67 50d1  _..i"..E;=...gP.
+00003e80: 6d4f cbdf ee76 d94d d781 be5a 270c e7ac  mO...v.M...Z'...
+00003e90: b7c5 e1a2 db5e 9ba7 dbe2 b0ad 9dc6 a7dd  .....^..........
+00003ea0: 7319 cd5c 0ed3 ebf2 f2b7 8ca7 cbc3 637a  s..\..........cz
+00003eb0: faed feb6 d3f8 b45b 2633 96c3 f4ba bc5c  .......[&3.....\
+00003ec0: c4d3 e5e1 313d fd76 37d3 f8b4 3b06 1b93  ....1=.v7...;...
+00003ed0: d373 3a49 46b3 c18a b5a0 5c1e ce27 cdcc  .s:IF.....\..'..
+00003ee0: b4ac 180b deda 757a 58cc 2edf c2ec f4d9  ......uzX.......
+00003ef0: 5d26 176b 41b9 3c9c 4f9a 9969 5931 16bc  ]&.kA.<.O..iY1..
+00003f00: b5eb f4b0 985d be85 d9e9 b3bb 4c2e 1244  .....]......L..D
+00003f10: 7161 1c76 9fe8 a0ba 5bfc c683 c272 7938  qa.v....[....ry8
+00003f20: 0f32 cbdf 6d10 34ff 14ab cb63 3a28 eda6  .2..m.4....c:(..
+00003f30: bf41 ee30 3d6d 2f83 ec61 76bd ec02 81a8  .A.0=m/..av.....
+00003f40: e832 e82d 5697 c774 503b 9c17 9741 6f33  .2.-V..tP;...Ao3
+00003f50: 280c 22a7 cde6 b2bc eca6 83e8 7978 9924  (.".........yx.$
+00003f60: 4a06 e0b2 dbee 1abf dd73 fa1c 0c4a cf41  J........s...J.A
+00003f70: ce2a 9309 4abb 4160 7939 4cfe 8edf ee39  .*..J.A`y9L....9
+00003f80: 1d4c 1455 83ba 7bed 7edf dda0 b25c fe96  .L.U..{.~....\..
+00003f90: 83ee e8b2 1b34 0eb3 d969 f719 e40e d3d3  .....4...i......
+00003fa0: f632 c85c 778f e9e9 b79b 2c4a 073c 77bd  .2.\w.....,J.<w.
+00003fb0: 2d0e bbc6 6f79 d935 86d7 5d43 6875 f876  -...oy.5..]Chu.v
+00003fc0: d3cb 783a e82d 5697 c774 5098 0e82 e16f  ..x:.-V..tP....o
+00003fd0: e65c ad56 abc1 6c39 1acc 4798 3c05 c081  .\.V..l9..G.<...
+00003fe0: 31b1 ba34 36ba 34b7 3905 ab30 b6ba b222  1..46.4.9..0..."
+00003ff0: 39b9 3739 8538 00ac 0f00 0000 b7b2 b330  9.79.8.........0
+00004000: ba34 bb32 10b2 b4b6 32b7 b9b4 37b7 3910  .4.2....2...7.9.
+00004010: b737 3a90 3036 b6b7 bb32 b2b8 80c2 3801  .7:.06...2....8.
+00004020: a7c3 b801 17d2 241f 000e 8c89 d5a5 b1d1  ......$.........
+00004030: a5b9 cd29 24b9 9195 e115 c9c9 bdc9 29c4  ...)$.........).
+00004040: 0160 5100 0000 9c95 d1a5 d195 b581 bcd5  .`Q.............
+00004050: d181 bc99 81c8 85b9 9d95 c505 14c6 0938  ...............8
+00004060: 1dc6 0db8 1027 fb00 7060 4cac 2e8d 8d2e  .....'..p`L.....
+00004070: cd6d 4ea1 a9ac ed4d 2eaf 484e ee4d 4e21  .mN....M..HN.MN!
+00004080: 0e00 8b02 0000 602c cccd ed8d 0e24 8c8d  ......`,.....$..
+00004090: ed6d 2c8c ae0c 842d 6d8e 2e2e a030 4ec0  .m,....-m....0N.
+000040a0: e930 6ec0 853c f907 8003 6362 7569 6c74  .0n..<....cbuilt
+000040b0: 696e 730a 5a65 726f 4469 7669 7369 6f6e  ins.ZeroDivision
+000040c0: 4572 726f 720a 7100 5810 0000 0064 6976  Error.q.X....div
+000040d0: 6973 696f 6e20 6279 207a 6572 6f71 0185  ision by zeroq..
+000040e0: 7102 4e87 7103 2e04 ca95 001c 1813 ab4b  q.N.q..........K
+000040f0: 63a3 4b73 9b53 089a 9b2b 93a3 4b7b 732b  c.Ks.S...+..K{s+
+00004100: 9293 7b93 5388 0348 c122 0000 0048 6b83  ..{.S..H."...Hk.
+00004110: 638b 0bc0 8a02 0000 78a9 9a2b 939b 7b99  c.......x..+..{.
+00004120: 4b6b 7b73 7b71 197b 7323 0b7b 2973 b39b  Kk{s{q.{s#.{)s..
+00004130: 7b99 4b6b 130b fb22 2bb3 7b61 4b13 7b81  {.Kk..."+.{aK.{.
+00004140: cba3 437b 739b 71b1 7999 4ba3 2b6b 810b  ..C{s.q.y.K.+k..
+00004150: 1b5b 0b3b 2b9b 7b71 ab6b 130b 7b71 837b  .[.;+.{q.k..{q.{
+00004160: 614b 730b 633b 7381 cb8b 1368 f242 388c  aKs.c;s....h.B8.
+00004170: 1b38 8c23 7001 00b1 1800 009e 0000 0033  .8.#p..........3
+00004180: 0880 1cc4 e11c 6614 013d 8843 3884 c38c  ......f..=.C8...
+00004190: 4280 0779 7807 7398 710c e600 0fed 100e  B..yx.s.q.......
+000041a0: f480 0e33 0c42 1ec2 c11d cea1 1c66 3005  ...3.B.......f0.
+000041b0: 3d88 4338 8483 1bcc 033d c843 3d8c 033d  =.C8.....=.C=..=
+000041c0: cc78 8c74 7007 7b08 0779 4887 7070 077a  .x.tp.{..yH.pp.z
+000041d0: 7003 7678 8770 2087 19cc 110e ec90 0ee1  p.vx.p .........
+000041e0: 300f 6e30 0fe3 f00e f050 0e33 10c4 1dde  0.n0.....P.3....
+000041f0: 211c d821 1dc2 611e 6630 893b bc83 3bd0  !..!..a.f0.;..;.
+00004200: 4339 b403 3cbc 833c 8403 3bcc f014 7660  C9..<..<..;...v`
+00004210: 077b 6807 3768 8772 6807 3780 8770 9087  .{h.7h.rh.7..p..
+00004220: 7060 0776 2807 76f8 0576 7887 7780 875f  p`.v(.v..vx.w.._
+00004230: 0887 7118 8772 9887 7998 812c eef0 0eee  ..q..r..y..,....
+00004240: e00e f5c0 0eec 3003 62c8 a11c e4a1 1ccc  ......0.b.......
+00004250: a11c e4a1 1cdc 611c ca21 1cc4 811d ca61  ......a..!.....a
+00004260: 06d6 9043 39c8 4339 9843 39c8 4339 b8c3  ...C9.C9.C9.C9..
+00004270: 3894 4338 8803 3b94 c32f bc83 3cfc 823b  8.C8..;../..<..;
+00004280: d403 3bb0 c30c c769 8770 5887 7270 8374  ..;....i.pX.rp.t
+00004290: 6807 7860 8774 1887 74a0 8719 ce53 0fee  h.x`.t..t....S..
+000042a0: 000f f250 0ee4 900e e340 0fe1 200e ec50  ...P.....@.. ..P
+000042b0: 0e33 2028 1ddc c11e c241 1ed2 211c dc81  .3 (.....A..!...
+000042c0: 1edc e01c e4e1 1dea 011e 6618 5138 b043  ..........f.Q8.C
+000042d0: 3a9c 833b cc50 2476 6007 7b68 0737 6087  :..;.P$v`.{h.7`.
+000042e0: 7778 0778 9851 4cf4 900f f050 0e33 1e6a  wx.x.QL....P.3.j
+000042f0: 1eca 611c e821 1dde c11d 7e01 1ee4 a11c  ..a..!....~.....
+00004300: cc21 1df0 6106 5485 8338 ccc3 3bb0 433d  .!..a.T..8..;.C=
+00004310: d043 39fc c23c e443 3b88 c33b b0c3 8cc5  .C9..<.C;..;....
+00004320: 0a87 7998 8777 1887 7408 077a 2807 7298  ..y..w..t..z(.r.
+00004330: 815c e310 0eec c00e e550 0ef3 3023 c1d2  .\.......P..0#..
+00004340: 411e e4e1 17d8 e11d de01 1e66 4819 3bb0  A..........fH.;.
+00004350: 833d b483 1b84 c338 8c43 39cc c33c b8c1  .=.....8.C9..<..
+00004360: 39c8 c33b d403 3ccc 48b4 7108 0776 6007  9..;..<.H.q..v`.
+00004370: 7108 8771 5887 19db c60e ec60 0fed e006  q..qX......`....
+00004380: f020 0fe5 300f e520 0ff6 500e 6e10 0ee3  . ..0.. ..P.n...
+00004390: 300e e530 0ff3 e006 e9e0 0ee4 500e f830  0..0........P..0
+000043a0: 43e1 da21 1de6 a11c f001 1eca 611c e861  C..!........a..a
+000043b0: 46d4 d9c3 3884 033b b0c3 2fd8 433a cc43  F...8..;../.C:.C
+000043c0: 3a88 433a b043 3ad0 433e cc68 3c79 2807  :.C:.C:.C>.h<y(.
+000043d0: 7af8 8574 9887 5f90 8770 4887 7928 8719  z..t.._..pH.y(..
+000043e0: ce87 0ee5 100e f010 0eec c00e ef30 0ef3  .............0..
+000043f0: 900e f450 0e00 0079 2000 001e 0000 0072  ...P...y ......r
+00004400: 1e48 2043 880c 1909 7232 4820 2381 8c91  .H C....r2H #...
+00004410: 91d1 44a0 1028 643c 3132 428e 9021 a318  ..D..(d<12B..!..
+00004420: 1012 000e 0000 0062 7261 6e63 685f 7765  .......branch_we
+00004430: 6967 6874 7300 0023 0843 2d8c 200c b630  ights..#.C-. ..0
+00004440: 82d0 06b7 3045 00cc 3004 c230 4340 c848  ....0E..0..0C@.H
+00004450: 6082 d273 ab6b 130b fb0a 933b 9bfb 6a0b  `..s.k.....;..j.
+00004460: cbfb 0a63 bb0b cb9b fb72 2b2b 23fb 7293  ...c.....r++#.r.
+00004470: a31b 4520 0800 00a9 1800 0011 0000 000b  ..E ............
+00004480: 0a72 2887 7780 077a 5870 9843 3db8 c338  .r(.w..zXp.C=..8
+00004490: b043 39d0 c382 e61c c6a1 0de8 411e c2c1  .C9.........A...
+000044a0: 1de6 211d e821 1dde c11d 1634 e360 0ee7  ..!..!.....4.`..
+000044b0: 500f e120 0fe4 400f e120 0fe7 500e f400  P.. ..@.. ..P...
+000044c0: 0000 00d1 1000 0006 0000 0007 cc3c a483  .............<..
+000044d0: 3b9c 033b 9403 3da0 833c 9443 3890 c301  ;..;..=..<.C8...
+000044e0: 0000 0061 2000 0068 0900 0013 0477 100b  ...a ..h.....w..
+000044f0: 0400 0016 0000 0034 28a0 5228 8622 2883  .......4(.R(."(.
+00004500: 42a8 0212 8d00 1442 0914 4419 1441 c114  B......B..D..A..
+00004510: 460d 5450 3914 5001 0614 8865 a1c2 b240  F.TP9.P....e...@
+00004520: 510a 051c 5080 0205 2c50 8003 053c 5005  Q...P...,P...<P.
+00004530: 8552 3824 1e01 a0c2 0800 8dc6 0840 1004  .R8$.........@..
+00004540: 4110 0441 d0ff 0f4a 8d00 5078 0600 00f1  A..A...J..Px....
+00004550: 3000 00d2 0000 0022 47c8 9051 268c 6b01  0......"G..Q&.k.
+00004560: 0000 00ae 800b b780 2996 3fa0 c449 005f  ........).?..I._
+00004570: 5a4e 356e 756d 6261 326e 7038 6172 7261  ZN5numba2np8arra
+00004580: 796f 626a 3133 6e75 6d70 795f 6675 6c6c  yobj13numpy_full
+00004590: 5f6e 6431 3224 3363 6c6f 6361 6c73 2433  _nd12$3clocals$3
+000045a0: 6539 6675 6c6c 2432 3436 3345 3855 6e69  e9full$2463E8Uni
+000045b0: 5475 706c 6549 784c 6932 4545 645f 5a4e  TupleIxLi2EEd_ZN
+000045c0: 356e 756d 6261 326e 7038 6172 7261 796f  5numba2np8arrayo
+000045d0: 626a 3133 6e75 6d70 795f 6675 6c6c 5f6e  bj13numpy_full_n
+000045e0: 6431 3224 3363 6c6f 6361 6c73 2433 6539  d12$3clocals$3e9
+000045f0: 6675 6c6c 2432 3436 3345 3855 6e69 5475  full$2463E8UniTu
+00004600: 706c 6549 784c 6932 4545 643a 2025 6578  pleIxLi2EEd: %ex
+00004610: 6369 6e66 6f5f 5a4e 356e 756d 6261 326e  cinfo_ZN5numba2n
+00004620: 7038 6172 7261 796f 626a 3133 6e75 6d70  p8arrayobj13nump
+00004630: 795f 6675 6c6c 5f6e 6431 3224 3363 6c6f  y_full_nd12$3clo
+00004640: 6361 6c73 2433 6539 6675 6c6c 2432 3436  cals$3e9full$246
+00004650: 3345 3855 6e69 5475 706c 6549 784c 6932  3E8UniTupleIxLi2
+00004660: 4545 643a 2025 7265 7470 7472 6c6c 766d  EEd: %retptrllvm
+00004670: 2e6c 6f6f 702e 756e 726f 6c6c 2e64 6973  .loop.unroll.dis
+00004680: 6162 6c65 4c56 6572 446f 6d61 696e 6c6c  ableLVerDomainll
+00004690: 766d 2e6c 6f6f 702e 6973 7665 6374 6f72  vm.loop.isvector
+000046a0: 697a 6564 5f5a 4e35 6e75 6d62 6132 6e70  ized_ZN5numba2np
+000046b0: 366c 696e 616c 6731 345f 6765 745f 6e6f  6linalg14_get_no
+000046c0: 726d 5f69 6d70 6c31 3224 3363 6c6f 6361  rm_impl12$3cloca
+000046d0: 6c73 2433 6531 346f 6e65 445f 696d 706c  ls$3e14oneD_impl
+000046e0: 2432 3436 3145 3541 7272 6179 4966 4c69  $2461E5ArrayIfLi
+000046f0: 3145 3143 376d 7574 6162 6c65 3761 6c69  1E1C7mutable7ali
+00004700: 676e 6564 4532 376f 6d69 7474 6564 2432  gnedE27omitted$2
+00004710: 3864 6566 6175 6c74 2433 644e 6f6e 6524  8default$3dNone$
+00004720: 3239 5f5a 4e35 6e75 6d62 6132 6e70 366c  29_ZN5numba2np6l
+00004730: 696e 616c 6731 345f 6765 745f 6e6f 726d  inalg14_get_norm
+00004740: 5f69 6d70 6c31 3224 3363 6c6f 6361 6c73  _impl12$3clocals
+00004750: 2433 6531 346f 6e65 445f 696d 706c 2432  $3e14oneD_impl$2
+00004760: 3436 3145 3541 7272 6179 4966 4c69 3145  461E5ArrayIfLi1E
+00004770: 3143 376d 7574 6162 6c65 3761 6c69 676e  1C7mutable7align
+00004780: 6564 4532 376f 6d69 7474 6564 2432 3864  edE27omitted$28d
+00004790: 6566 6175 6c74 2433 644e 6f6e 6524 3239  efault$3dNone$29
+000047a0: 3a20 2565 7863 696e 666f 5f5a 4e35 6e75  : %excinfo_ZN5nu
+000047b0: 6d62 6132 6e70 366c 696e 616c 6731 345f  mba2np6linalg14_
+000047c0: 6765 745f 6e6f 726d 5f69 6d70 6c31 3224  get_norm_impl12$
+000047d0: 3363 6c6f 6361 6c73 2433 6531 346f 6e65  3clocals$3e14one
+000047e0: 445f 696d 706c 2432 3436 3145 3541 7272  D_impl$2461E5Arr
+000047f0: 6179 4966 4c69 3145 3143 376d 7574 6162  ayIfLi1E1C7mutab
+00004800: 6c65 3761 6c69 676e 6564 4532 376f 6d69  le7alignedE27omi
+00004810: 7474 6564 2432 3864 6566 6175 6c74 2433  tted$28default$3
+00004820: 644e 6f6e 6524 3239 3a20 2572 6574 7074  dNone$29: %retpt
+00004830: 7200 0013 8461 1626 0803 2dac 1026 64c5  r....a.&..-..&d.
+00004840: 404d c98a a19a 9415 8265 062b 848b 5921  @M.......e.+..Y!
+00004850: 60d7 0a21 bb56 08da b542 d8d6 6085 c0ad  `..!.V...B..`...
+00004860: c10a a133 8315 8267 062b 84cf 0c56 0860  ...3...g.+...V.`
+00004870: e0ac 18c2 000c 9e15 8318 8001 b461 0822  .............a."
+00004880: 6983 5051 1b86 6010 3604 cb86 00db 1064  i.PQ..`.6......d
+00004890: 1b02 6d83 8065 1b84 46d8 2088 4118 0033  ..m..e..F. .A..3
+000048a0: 1169 30d4 c228 cc44 1443 2d90 c288 4101  .i0..(.D.C-...A.
+000048b0: 8420 18f0 413e e4c1 8841 0184 2018 f041  . ..A>...A.. ..A
+000048c0: 3ec0 c1ad 011d ec70 4310 0668 30cb 7004  >......pC..h0.p.
+000048d0: c188 8101 8420 18bc 814d d841 1b8c 2604  ..... ...M.A..&.
+000048e0: c068 8210 8c18 1840 0882 c11b e484 2006  .h.....@...... .
+000048f0: a309 4170 43b0 b30c 8710 dc1c 90c1 8d26  ..ApC..........&
+00004900: 10c0 8881 0184 2018 c441 4f04 71d0 0042  ...... ..AO.q..B
+00004910: 5006 1978 9702 1219 6e10 0537 0083 e106  P..x....n..7....
+00004920: 3d78 0330 3821 d859 0664 0866 0988 810a  =x.08!.Y.d.f....
+00004930: 3188 0871 1806 2ac4 a021 c861 c020 0e60  1..q..*..!.a. .`
+00004940: 60b8 21f8 0334 4062 0e40 60b8 2150 0534  `.!..4@b.@`.!P.4
+00004950: 986e 10ee 2098 6e28 f080 986e 4084 e208  .n.. .n(...n@...
+00004960: 634f 3105 b940 8136 12a0 60d8 8008 c680  cO1..@.6..`.....
+00004970: 0066 1908 8418 8e70 fdff ffff 410c fcc0  .f.....p....A...
+00004980: 0c32 10c9 0805 ecff ffff 0f62 1000 c208  .2.........b....
+00004990: 85ec ffff ff0f 62f0 0740 301c 21fb ffff  ......b..@0.!...
+000049a0: ff83 1888 8219 cc32 2846 9099 28f3 17be  .......2(F..(...
+000049b0: 3b6c 4004 0201 74d3 000e a500 1319 7c77  ;l@...t.......|w
+000049c0: d880 084e 8100 ba69 1087 5358 8561 0322  ...N...i..SX.a."
+000049d0: 2803 02e8 a661 1c50 6115 860d 88c0 1408  (....a.Pa.......
+000049e0: a09b 0672 4885 5518 3620 828e 00ba 8928  ...rH.U.6 .....(
+000049f0: 0755 8005 5518 3620 825f 2080 6e22 cc61  .U..U.6 ._ .n".a
+00004a00: 1562 2115 860d 88e0 1608 a09b 8873 6085  .b!..........s`.
+00004a10: 5860 8561 0322 2803 02e8 2602 1d5a 4116  X`.a."(...&..ZA.
+00004a20: 5661 d880 0856 8100 460c 0a20 04c1 800f  Va...V..F.. ....
+00004a30: dcc2 1746 0c0a 2004 c180 0fdc e21c 762c  ...F.. .......v,
+00004a40: 063a c4a0 0603 3b00 89c0 1f80 818e e1fe  .:....;.........
+00004a50: ec80 4e02 3a01 521d be3b 6c40 0403 01ac  ..N.:.R..;l@....
+00004a60: 30dc 500e b160 06b3 0c89 11a0 39a8 0208  0.P..`......9...
+00004a70: 0c37 f8c2 2c98 c174 c32f d042 9082 4850  .7..,..t./.B..HP
+00004a80: 0840 60b8 211c 6a01 0c86 1bc4 611d c060  .@`.!.j.....a..`
+00004a90: b881 1d6e 010c 2e10 76ba a11c dc41 b842  ...n....v....A.B
+00004aa0: d8e9 06e1 1c8c 1103 0308 4130 7803 d908  ..........A0x...
+00004ab0: 7a61 3421 0846 1304 e008 5c80 0b64 0131  za4!.F....\..d.1
+00004ac0: 0807 18b8 8317 e010 5ed0 1bc8 4191 0862  ........^...A..b
+00004ad0: e016 5fd0 63ca 41af 09e2 f8e1 1ce4 fae1  .._.c.A.........
+00004ae0: 1cee ea21 1de4 ec21 1d6e 9640 19a8 1003  ...!...!.n.@....
+00004af0: df48 78a1 18a8 1003 3e48 c0a1 186e e087  .Hx.....>H...n..
+00004b00: 7830 8359 86a5 08f2 2444 39dc 40cc 031a  x0.Y....$D9.@...
+00004b10: 4c37 a004 3d04 1718 7001 4ac8 0505 dc30  L7..=...p.J....0
+00004b20: 12d2 4602 2b04 3904 b401 8420 1f0e 69e0  ..F.+.9.... ..i.
+00004b30: 5e22 9063 02b8 4680 7306 9825 6006 2ac4  ^".c..F.s..%`.*.
+00004b40: 4044 96b2 ab83 818a 3660 85c5 66ea 60a0  @D......6`..f.`.
+00004b50: 420c 7461 f9b9 3a48 9810 e588 4101 8420  B.ta..:H....A.. 
+00004b60: 18f0 816f f8c4 7003 5112 6830 dd10 1326  ...o..p.Q.h0...&
+00004b70: 115c 60c0 0531 2117 1430 6250 0021 0806  .\`..1!..0bP.!..
+00004b80: 7c30 1e3a 31cb e034 c8b0 0141 1669 4200  |0.:1..4...A.iB.
+00004b90: 5b1b b30c 0fb4 06c3 0604 59a0 0901 6c6d  [.........Y...lm
+00004ba0: 0c37 b481 4a98 c188 8101 8420 18c4 817f  .7..J...... ....
+00004bb0: ac81 4c34 8010 9844 06e0 a540 4566 1922  ..L4...D...@Ef."
+00004bc0: 3a28 861b 72a2 25c4 6096 41ca 82e1 86b1  :(..r.%.`.A.....
+00004bd0: 7009 3198 65a8 a660 b8a1 0d5a 820c 6619  p.1.e..`...Z..f.
+00004be0: dc80 0ad2 2744 798d 04d7 1381 dc10 c02c  ....'Dy........,
+00004bf0: 0136 dc20 0732 4106 b30c 6b60 0539 16a2  .6. .2A...k`.9..
+00004c00: 3ce9 8213 8b40 6e08 6096 e01a a810 033c  <....@n.`......<
+00004c10: b0e2 e11a a810 03c2 6a87 6ba0 420c d2e1  ........j.k.B...
+00004c20: d213 2b05 9552 901a 59a8 9482 d4b8 6088  ..+..R..Y.....`.
+00004c30: 33c4 42d2 0a6c 0308 8190 816a 870d 88a0  3.B..l.....j....
+00004c40: 1880 7b8b 0532 5029 05a9 717b f140 062a  ..{..2P)..q{.@.*
+00004c50: a520 352e 20e2 a2b6 900c 83c0 3680 1008  . 5. .......6...
+00004c60: 0d20 0470 9181 6a87 0d88 c018 80bc 547a  . .p..j.......Tz
+00004c70: 7cf1 1692 4260 1b40 0884 0c54 4b41 6aa4  |...B`.@...TKAj.
+00004c80: a7d2 5b8d ba90 1402 db00 4220 64a0 5a0a  ..[.......B d.Z.
+00004c90: 52e3 8223 6e0c fe42 720e 02db 0042 2034  R..#n..Br....B 4
+00004ca0: 8010 8046 06aa 1d36 2002 6300 0e17 d200  ...F...6 .c.....
+00004cb0: 3250 2905 a971 bdd0 0690 814a 2948 8d0b  2P)..q.....J)H..
+00004cc0: 88b8 3758 0dc9 3f08 6c03 0881 d000 4280  ..7X..?.l.....B.
+00004cd0: 1a19 a876 d880 088c 0140 3a80 0d18 383b  ...v.....@:...8;
+00004ce0: 2007 383c 3807 186e 5087 010c 6619 d6e0   .8<8..nP...f...
+00004cf0: 0a06 2ac4 0024 a85d c006 2ac4 e016 30b6  ..*..$.]..*...0.
+00004d00: a112 1c54 9a83 4a29 480d 1a52 e302 21ce  ...T..J)H..R..!.
+00004d10: d80d c957 086c 0308 8190 816a 870d 88a0  ...W.l.....j....
+00004d20: 1880 438f 0532 5029 05a9 414c 6a5c 20c4  ..C..2P)..ALj\ .
+00004d30: 3de4 2189 0b81 6d00 2110 1a40 08ce 2303  =.!...m.!..@..#.
+00004d40: d50e 1b10 8131 0059 a9f4 e6c3 3c24 85c0  .....1.Y....<$..
+00004d50: 3680 1008 19a8 9682 d4a0 2c35 2e10 e2b8  6.........,5....
+00004d60: f890 2c87 c036 8010 080d 2004 f291 816a  ..,..6.... ....j
+00004d70: 870d 88c0 1880 5309 3180 0c54 4a41 6ad0  ......S.1..TJAj.
+00004d80: 18a4 c605 429c 19ec 87e4 3b04 b601 8440  ....B.....;....@
+00004d90: 6800 21c0 8f0c 543b 6c40 04c6 00e0 1a80  h.!...T;l@......
+00004da0: 080c 5c1b d004 0c37 e484 0006 b30c 6e80  ..\....7......n.
+00004db0: 05c3 0d37 2222 6230 cba0 71c1 7043 5884  ...7""b0..q.pCX.
+00004dc0: 0819 cc32 c4c1 16cc 12a4 c170 435a ec07  ...2.......pCZ..
+00004dd0: 19cc 3274 6210 0c74 8881 0b89 810b 71a4  ..2tb..t......q.
+00004de0: 8206 c30d 6081 2260 7065 21c4 2c03 1878  ....`."`pe!.,..x
+00004df0: c22c c137 5021 06d1 6778 0315 6210 7da6  .,.7P!..gx..b.}.
+00004e00: e2e5 48a8 346d 42a5 24a4 0609 a971 8110  ..H.4mB.$....q..
+00004e10: 2d25 8cc4 316c 4004 c200 2002 2330 70c8  -%..1l@... .#0p.
+00004e20: 8ac0 7043 4023 6030 cb00 065f 3050 2106  ..pC@#`0..._0P!.
+00004e30: 5c67 7cc3 0d0d 8b90 c12c 031d 8441 304b  \g|......,...A0K
+00004e40: a006 e912 014d 9508 6c8a 4540 5b4a 6089  .....M..l.E@[J`.
+00004e50: bec8 20b0 0d20 143a 9234 11d0 e106 c110  .. .. .:.4......
+00004e60: 83e1 0681 2083 1302 1d6e 308b 440c 861b  .... ....n0.D...
+00004e70: 9283 0c4e 08f4 8860 6719 ba31 0886 1b46  ...N...`g..1...F
+00004e80: a34c c060 96c1 0cc8 20c8 9e50 69c2 854a  .L.`.... ..Pi..J
+00004e90: 4948 8d39 0616 09fc 658e a145 847f 9963  IH.9....e..E...c
+00004ea0: 7091 0164 e618 5e84 0819 3252 638e 2146  p..d..^...2Rc.!F
+00004eb0: 8291 9963 9011 8164 e618 6664 2899 3906  ...c...d..fd(.9.
+00004ec0: 1a21 4ce6 8824 0619 021b d191 2b94 1864  .!L..$......+..d
+00004ed0: 0870 8447 ce58 6290 21d0 111f b983 8941  .p.G.Xb.!......A
+00004ee0: 8680 47c0 84a8 d498 63f0 9100 66e6 187e  ..G.....c...f..~
+00004ef0: 4488 9939 0630 1964 668e 214c 8899 212c  D..9.0.df.!L..!,
+00004f00: 35e6 18c6 24a8 9939 0632 116c 668e a14c  5...$..9.2.lf..L
+00004f10: 869b 9963 3013 0267 8e48 6290 2140 1336  ...c0..g.Hb.!@.6
+00004f20: b942 8941 8640 4ddc e48c 2506 1902 3681  .B.A.@M...%...6.
+00004f30: 933b 9818 6408 dc44 4e66 09ca 60a0 420c  .;..d..DNf..`.B.
+00004f40: 708a 0c66 a10c 062a c480 75c8 6016 cae0  p..f...*..u.`...
+00004f50: 8456 910c 8dc0 3680 1008 198c 77d8 8008  .V....6.....w...
+00004f60: be01 3823 5624 4b23 b00d 2004 4203 0881  ..8#V$K#.. .B...
+00004f70: aa64 30de 6103 2210 8301 b8c5 5624 5523  .d0.a.".....V$U#
+00004f80: b00d 2004 4203 0881 ab64 30de 6103 2228  .. .B....d0.a."(
+00004f90: 8301 3868 5724 5f23 b00d 2004 4203 0881  ..8hW$_#.. .B...
+00004fa0: ab64 30de 6103 2240 8301 b80a 5c24 6923  .d0.a."@....\$i#
+00004fb0: b00d 2004 4203 0881 ac64 30de 6103 2208  .. .B....d0.a.".
+00004fc0: 8301 38ad 5c24 7323 b00d 2004 4203 0881  ..8.\$s#.. .B...
+00004fd0: ad64 30de 6103 2220 8301 b84f 5d24 7d23  .d0.a." ...O]$}#
+00004fe0: b00d 2004 4203 0881 ae64 30de 6103 2238  .. .B....d0.a."8
+00004ff0: 8301 3832 7817 c9f1 086c 0308 81d0 0042  ..82x....l.....B
+00005000: e02b 198c 77d8 8008 d460 002e 0dd2 052e  .+..w....`......
+00005010: 0dc0 0586 1b82 7b01 8359 0633 2883 60a0  ......{..Y.3(.`.
+00005020: 420c e06b 0c8c 3218 6e98 917c 0183 5906  B..k..2.n..|..Y.
+00005030: 3438 8320 e343 a549 222a 2521 35e6 18c0  48. .C.I"*%!5...
+00005040: 2590 9d39 8670 1166 678e 415c 06da 9963  %..9.p.fg.A\...c
+00005050: 1817 a276 c848 8d39 8672 096e 678e c15c  ...v.H.9.r.ng..\
+00005060: 04dc 9963 3897 2177 e618 d085 d09d 2392  ...c8.!w......#.
+00005070: 1864 08d4 c55d ae50 6290 2160 1778 3963  .d...].Pb.!`.x9c
+00005080: 8941 86c0 5de4 e50e 2606 1902 78a1 9796  .A..]...&...x...
+00005090: 1240 c4ca 60bc c306 4490 0c40 4b09 42cb  .@..`...D..@K.B.
+000050a0: 6430 de61 0322 4806 a0a5 04a2 6432 18ef  d0.a."H.....d2..
+000050b0: b001 1124 03d0 5282 e132 198c 77d8 8008  ...$..R..2..w...
+000050c0: 9201 9825 4083 e186 3c89 1330 9865 a083  ...%@...<..0.e..
+000050d0: 2e18 a810 0339 da76 210d 062a c4e0 16d2  .....9.v!..*....
+000050e0: 00ce b684 1195 5290 1a49 a894 82d4 b860  ......R..I.....`
+000050f0: 8833 7a46 3246 02db 0042 2064 a0da 6103  .3zF2F...B d..a.
+00005100: 2228 0680 92d4 38ba 6120 0395 5290 1a17  "(....8.a ..R...
+00005110: 1071 8fd9 48ea 4860 1b40 0884 0610 82b4  .q..H.H`.@......
+00005120: c940 b5c3 0644 600c 004d a991 964a ef6f  .@...D`..M...J.o
+00005130: d246 5208 6c03 0881 9081 6a29 488d 0b8e  .FR.l.....j)H...
+00005140: 386e 6e24 cf24 b00d 2004 4203 0801 dd64  8nn$.$.. .B....d
+00005150: a0da 6103 2230 0680 c020 35ee 55c6 0032  ..a."0... 5.U..2
+00005160: 5029 05a9 7101 1167 067d 2319 2781 6d00  P)..q..g.}#.'.m.
+00005170: 2110 1a40 08f4 2603 d50e 1b10 8131 00b8  !..@..&......1..
+00005180: 06a2 0303 d706 b802 c30d bb22 80c1 2c43  ..........."..,C
+00005190: 1ca4 4130 5021 0625 a106 e212 06e9 272a  ..A0P!.%......'*
+000051a0: cd58 5129 09a9 4142 6a5c 20c4 19ab 23f9  .XQ)..ABj\ ...#.
+000051b0: 2781 6d00 2110 3250 edb0 0111 1403 4049  '.m.!.2P......@I
+000051c0: 6a50 921a 1708 718d ec48 9a4a 601b 4008  jP....q..H.J`.@.
+000051d0: 8406 1082 dac9 40b5 c306 4460 0c00 45a9  ......@...D`..E.
+000051e0: 4151 6a5c 20c4 55ba 23e9 2a81 6d00 2110  AQj\ .U.#.*.m.!.
+000051f0: 1a40 0876 2703 d50e 1b10 8131 0094 a506  .@.v'......1....
+00005200: 65a9 7181 10d7 898f a4ad 04b6 0184 4068  e.q...........@h
+00005210: 0021 f89d 0c54 3b6c 4004 c600 5018 a406  .!...T;l@...P...
+00005220: 8541 6a5c 20c4 9581 fa48 fa4a 601b 4008  .Aj\ ....H.J`.@.
+00005230: 8406 1082 f0c9 40b5 c306 4460 0c00 a541  ......@...D`...A
+00005240: 6a50 1aa4 c605 425c 1bc8 8fa4 b904 b601  jP....B\........
+00005250: 8440 6800 21f8 9d0c 543b 6c40 04c6 0050  .@h.!...T;l@...P
+00005260: 1ca4 06c5 416a 5c20 c4d5 81fe 48ba 4b60  ....Aj\ ....H.K`
+00005270: 1b40 0884 0610 02fc c940 b5c3 0644 600c  .@.......@...D`.
+00005280: 00e5 416a 501e a4c6 0542 5c1f 8890 a4bd  ..AjP....B\.....
+00005290: 04b6 0184 4068 0021 709f 0c54 3b6c 4004  ....@h.!p..T;l@.
+000052a0: c600 a028 9410 0c0c 37b0 4d00 06b3 0c74  ...(....7.M....t
+000052b0: a006 c140 8518 d060 50c9 d375 6e73 423a  ...@...`P..unsB:
+000052c0: dc10 b010 18cc 32d0 011b 0499 43a2 6c29  ......2.....C.l)
+000052d0: 0164 8803 a342 0e66 02b8 1c3a e48a 00ae  .d...B.f...:....
+000052e0: 6564 06ae 8702 b921 8059 8236 18a8 1003  ed.....!.Y.6....
+000052f0: 810d ae36 18a8 1003 870d a636 18a8 1003  ...6.......6....
+00005300: 380c d8e0 6983 1c54 4a41 6a24 a152 0a52  8...i..TJAj$.R.R
+00005310: e382 215a 4a80 8c61 0322 1006 008f 1e82  ..!ZJ..a."......
+00005320: 814b e208 6e49 2318 6ec8 9b01 0c66 19e8  .K..nI#.n....f..
+00005330: a00d 8281 0a31 30c5 6022 25ec 4e07 8c74  .....10.`"%.N..t
+00005340: b821 2823 3098 65a0 8337 0852 8e44 d952  .!(#0.e..7.R.D.R
+00005350: 42ce 1007 4785 dc10 c091 4dda c0d1 5120  B...G.....M...Q 
+00005360: 3704 304b 0007 0315 6220 bcc1 0407 0315  7.0K....b ......
+00005370: 62c0 8bc1 1b3c 7090 78a3 d21c 544a 416a  b....<p.x...TJAj
+00005380: d090 1a17 08d1 5242 630c 1b10 8130 0078  ......RBc....0.x
+00005390: cc11 0c5c e247 30dc e03a 0218 cc32 d001  ...\.G0..:...2..
+000053a0: 1c04 0315 6200 8f81 a61e 6930 dc00 3b79  ....b.....i0..;y
+000053b0: 0406 b30c 7420 0741 4b09 6c23 1c2b 0d72  ....t .AK.l#.+.r
+000053c0: 7d13 c02c c11c 0c54 8881 2007 d31c 0c54  }..,...T.. ....T
+000053d0: 8801 3f06 72f0 cc41 da8d 4a29 488d 2454  ..?.r..A..J)H.$T
+000053e0: 4a41 6a5c 3044 4b09 8a31 6c40 04c2 00e0  JAj\0DK..1l@....
+000053f0: 314a 3070 c92d c170 83ef 0860 30cb 4007  1J0p.-.p...`0.@.
+00005400: 7310 641a 0536 d728 b023 0605 1082 60c0  s.d..6.(.#....`.
+00005410: 076a 354e 2306 0510 8260 c007 6aa5 4b23  .j5N#....`..j.K#
+00005420: 0646 0382 6080 0b62 954a c188 81d1 8020  .F..`..b.J..... 
+00005430: 18e0 8258 9d92 306c 40ac 111c 11c0 b001  ...X..0l@.......
+00005440: c146 6e34 0023 068d 0382 60e0 0a6b c546  .Fn4.#....`..k.F
+00005450: 6bf4 3732 d53e a9c4 37ed 934a c31c 4360  k.72.>..7..J..C`
+00005460: 073f 5107 ab50 07c9 4681 4d37 0a2c bd51  .?Q..P..F.M7.,.Q
+00005470: 6a8c 1818 0d08 8201 2e94 552b 0923 0646  j.........U+.#.F
+00005480: 0382 6080 0b65 b54a 431b 09b5 733a 298c  ..`..e.JC...s:).
+00005490: 70d8 8010 0202 1831 2880 1004 033e 80ab  p......1(....>..
+000054a0: d219 6e68 1d58 3283 0c44 82af 1380 00ca  ..nh.X2..D......
+000054b0: 4e2c 41c0 7043 ecd0 9219 cc32 3045 9076  N,A.pC.....20E.v
+000054c0: 14d8 c4a3 c026 1e7d 9702 1119 3130 1a10  .....&.}....10..
+000054d0: 0403 5c80 2b5c 1a46 0c8c 0604 c100 17e0  ..\.+\.F........
+000054e0: ca96 8859 8223 1c08 0000 0025 0500 0016  ...Y.#.....%....
+000054f0: 5ce0 2c52 e423 95df 10d7 84df b501 0b28  \.,R.#.........(
+00005500: 7ecf f73e 25f9 9464 b503 d1e2 388f 8f34  ~..>%..d....8..4
+00005510: 0371 d5fd ee53 4d64 ca01 85df df3e 62da  .q...SMd.....>b.
+00005520: 0153 0344 9163 ddb8 3f10 8c13 1940 e323  .S.D.c..?....@.#
+00005530: 27b1 154e e407 ce80 f94f 441c 0430 1091  '..N.....OD..0..
+00005540: 2f3d 0b32 f994 64d3 058d 5fe3 3ee2 5392  /=.2..d..._.>.S.
+00005550: 4f3c c862 d501 867f d3b7 8f18 7880 e1df  O<.b........x...
+00005560: 34ee d796 2f70 f83d 4ffb 9454 a202 8f58  4.../p.=O..T...X
+00005570: de2e cbcf 6517 5c5e 6ec1 d1e9 f3b8 0a27  ....e.\^n......'
+00005580: f203 67c0 fc27 7216 ff89 8883 0006 2232  ..g..'r......."2
+00005590: dd81 4312 88ca 209e 93e9 0a27 f203 67c0  ..C... ....'..g.
+000055a0: 7c4a b2f5 dc27 1e64 f19f 8838 0860 2022  |J...'.d...8.` "
+000055b0: 330e 287c 3ef7 1173 0fd0 884b 409a c2f1  3.(|>..s...K@...
+000055c0: 6b5f 8a1c c0a7 7dda 7f0e 5f42 1ac5 0c05  k_....}..._B....
+000055d0: 906b 8a00 6422 223b 0c68 80c8 f081 2802  .k..d"";.h....(.
+000055e0: b0bf f669 430c 6880 c8f0 8128 02b0 bff6  ...iC.h....(....
+000055f0: 6b4b 0c68 80c8 f081 2802 b0bf f66d 530c  kK.h....(....mS.
+00005600: 6880 c8f0 8128 02b0 bff6 6f5b 0c68 80c8  h....(....o[.h..
+00005610: f081 2802 b0bf f671 2b14 281a bf22 04eb  ..(....q+.(.."..
+00005620: 2558 fc1a f711 9f92 ec3d 37e9 02c6 ef7b  %X.......=7....{
+00005630: daa7 249f 7890 c5f6 0510 bfc6 7dc4 a724  ..$.x.......}..$
+00005640: 1b1c 48fc bea7 7d4a f26b 831c 48fc bea7  ..H...}J.k..H...
+00005650: 7d4a f26d d31c 48fc bea7 7d4a f2ef 3b40  }J.m..H...}J..;@
+00005660: 36da 470a 1f29 8c9c c059 a4c8 472a bf21  6.G..)...Y..G*.!
+00005670: aee9 de7b cb0e 98fc baa7 6b5f 8a1c c0a7  ...{......k_....
+00005680: fdda 7f0e 1f39 876d db69 9f68 06a4 f089  .....9.m.i.h....
+00005690: 6640 0a9f 6806 a4f0 8966 400a b30e 30fc  f@..h....f@...0.
+000056a0: 9bc6 7dc4 0207 12bf df7b 9f92 fcda 3007  ..}......{....0.
+000056b0: 12bf df7b 9f92 fcdb 8e03 0a9f d77d c420  ...{.........}. 
+000056c0: 031a 2032 7c20 8a00 ecb7 7dda 2203 1a20  .. 2| ....}.".. 
+000056d0: 327c 208a 00ec b7fd da24 031a 2032 7c20  2| ......$.. 2| 
+000056e0: 8a00 ecb7 7ddb 2603 1a20 327c 208a 00ec  ....}.&.. 2| ...
+000056f0: b7fd db28 031a 2032 7c20 8a00 ecb7 7dfc  ...(.. 2| ....}.
+00005700: 4692 8a10 2627 f29f e352 9cc2 89fc c019  F...&'...R......
+00005710: 309f 926c 3db7 f202 6791 221f a9fc 86b8  0..l=...g.".....
+00005720: a6bb a7cd bcc0 59a4 c847 2abf 21ae e9ee  ......Y..G*.!...
+00005730: 6f9b 2f70 1629 f291 ca6f 886b bafb dc44  o./p.)...o.k...D
+00005740: 079c 458a 7ca4 f21b e29a ee7e bf92 a522  ..E.|......~..."
+00005750: 84c9 89fc c019 301b 2768 fc9a ae7b 9f92  ......0.'h...{..
+00005760: ec7d f7ef 7bd1 0a27 f203 67c0 7c4a f289  .}..{..'..g.|J..
+00005770: 0759 fc27 220e 0218 88c8 8403 0a7f e77d  .Y.'"..........}
+00005780: e434 b0c2 89fc c019 309f 926c 3df7 9f88  .4......0..l=...
+00005790: 3808 6020 2213 2f78 fcbe a77d 4ab2 77dc  8.` "./x...}J.w.
+000057a0: 271e 6431 4d81 c3ef f9de ee7b d317 38fc  '.d1M......{..8.
+000057b0: bea7 7d4a b2d3 0168 719c c747 9a81 b8ea  ..}J...hq..G....
+000057c0: 7ef7 9fc3 8e0b 1449 202a 8378 705a 37ea  ~......I *.xpZ7.
+000057d0: 0245 1288 ca20 1e9c eead 3ee0 f0f3 9db7  .E... ....>.....
+000057e0: 73db 3005 0abf ae6b db32 050a bfae 6bdc  s.0....k.2....k.
+000057f0: f603 16e9 2104 5f22 1642 986c 9740 f17b  ....!._".B.l.@.{
+00005800: bef7 29c9 de6f 231e 6004 a729 1644 98fc  ..)..o#.`..).D..
+00005810: 68b8 6c38 a0f0 f7de 470c 7640 f16b dc47  h.l8....G.v@.k.G
+00005820: fc27 7216 630c 7880 c8f0 8128 02b0 bff6  .'r.c.x....(....
+00005830: 739f b6c6 8007 880c 1f88 2200 fb6b 3ff7  s........."..k?.
+00005840: 6bcb 2d78 fc7e ef7d 4af2 29c9 271e 6431  k.-x.~.}J.).'.d1
+00005850: de81 8332 16cc 201e 432d 38fc 9aae 7b7f  ...2.. .C-8...{.
+00005860: 3f85 64cb 719f 6806 a430 d702 4512 88ca  ?.d.q.h..0..E...
+00005870: 201e dcc6 cdb7 4091 04a2 3288 07b7 7713   .....@...2...w.
+00005880: 2e80 8807 597c 6422 a2db ce7d 8179 8c3f  ....Y|d"...}.y.?
+00005890: 80f0 9f88 b0df 8085 b804 a429 1cbf f611  ...........)....
+000058a0: eb1d 1002 c12c 0998 0699 88c8 6f24 2af0  .....,......o$*.
+000058b0: eb6b 990a 27f2 0367 c07c 4af2 29c9 271e  .k..'..g.|J.).'.
+000058c0: 64b1 de02 c8af 711f f129 c9a7 249f 7890  d.....q..)..$.x.
+000058d0: c51c 031e 2032 7c20 8a00 ecaf 7ddd a7ed  .... 2| ....}...
+000058e0: 31e0 0122 c307 a208 c0fe dad7 fdfa 188c  1.."............
+000058f0: edd6 7da4 b7d8 0145 1288 ca20 9e5b afad  ..}....E... .[..
+00005900: 5760 5a1c e7f1 9166 20ae badf 7d4a f229  W`Z....f ...}J.)
+00005910: c9e0 090c bfe7 69bf 367c 02c3 ef79 dab7  ......i.6|...y..
+00005920: af80 d970 de5f 1ce7 212e 64ba 8467 cb71  ...p._..!.d..g.q
+00005930: 9f68 06a4 f097 c87f 8e03 2888 668a 3003  .h........(.f.0.
+00005940: 2c30 fc9e a7fd db10 0b0c bfe7 691f 37d0  ,0..........i.7.
+00005950: 02c3 ef79 dadf 0db3 c0f0 7b9e f675 832c  ...y......{..u.,
+00005960: 30fc 9ea7 fddc 5805 083f f711 fb15 50fc  0.....X..?....P.
+00005970: 9ea7 7d4a f229 c982 0792 c0a1 9a81 be69  ..}J.).........i
+00005980: dbf0 0310 bfde 731f a969 8b17 68fc 9aae  ......s..i..h...
+00005990: 7b9f 927c 4af2 6ff3 0d28 fcbb f611 5b27  {..|J.o..(....['
+000059a0: 28fc 1af7 11db 1d50 2481 a80c e2b1 fbdd  (......P$.......
+000059b0: 8607 a2c2 a19a c117 9ca6 5810 61ba 69dc  ..........X.a.i.
+000059c0: ec05 a0c5 711e 1f69 06e2 aafb dda7 24ab  ....q..i......$.
+000059d0: 0c78 80c8 f081 2802 b0df f673 9f36 cb80  .x....(....s.6..
+000059e0: 0788 0c1f 8822 00fb 6d3f f76b 931d 50fc  ....."..m?.k..P.
+000059f0: 9aae 7bff 899c c588 0918 bfe7 7b9f 92ec  ..{.........{...
+00005a00: fdf6 6bdb 2660 fc9e ef7d 4ab2 f7db bf4d  ..k.&`...}J....M
+00005a10: b5e0 5a1c e7f1 9166 20ae badf 7d4a f229  ..Z....f ...}J.)
+00005a20: c9a7 9ac8 b40b 1449 202a 8378 6e9e b7f5  .......I *.xn...
+00005a30: 002d 22a6 678a fc88 7800 41b1 e9dd 8f88  .-".g...x.A.....
+00005a40: 0710 14bb be8d 7da0 409a 81b8 4c3e 20f1  ......}.@...L> .
+00005a50: 6f1a f76b 5ba7 ed92 8069 9089 88fc 4660  o..k[....i....F`
+00005a60: 1ebf b6fb 00c3 b777 da47 0c52 20f1 6f1a  .......w.G.R .o.
+00005a70: f76b 5bb7 0dbc e0f1 7b9e f629 c9d6 7b9f  .k[.....{..)..{.
+00005a80: 7890 c5d4 03ae 8898 9e29 f223 e201 04c5  x........).#....
+00005a90: a677 3f22 1e40 504c 9880 f17b 9ef6 29c9  .w?".@PL...{..).
+00005aa0: d67b bf36 6602 c6ef 79da a724 5bef 7ddb  .{.6f...y..$[.}.
+00005ab0: b209 18bf e769 9f92 6cbd f76f 232f 5024  .....i..l..o#/P$
+00005ac0: 81a8 0ce2 b9fb dabc 0308 ffd6 7392 89d5  ............s...
+00005ad0: 9646 46c6 56e6 22c6 f636 b6e6 52e7 26d7  .FF.V."..6..R.&.
+00005ae0: c236 3637 1766 f104 86df f7b4 5f1b 7400  .667.f......_.t.
+00005af0: d200 51e4 583e 6281 0586 dff7 b47f 5b62  ..Q.X>b.......[b
+00005b00: 81e1 f73d ede3 964f 60f8 7d4f fbb6 4516  ...=...O`.}O..E.
+00005b10: 187e dfd3 7e6e a105 86df f7b4 bf5b 6681  .~..~n.......[f.
+00005b20: e1f7 3ded eb24 97ce ec4d cea5 cc8d cc85  ..=..$...M......
+00005b30: eded 0dae 0c2f 8d6e 0606 c7a5 ce4d ae85  ...../.n.....M..
+00005b40: 6d6c 6e2e cc2e 031e 2032 7c20 8a00 ecb7  mln..... 2| ....
+00005b50: 7ddd a70d 33e0 0122 c307 a208 c07e dbd7  }...3..".....~..
+00005b60: fdda b003 26bf eee9 da97 2207 f075 bff6  ....&....."..u..
+00005b70: 9fc3 47cc bda0 f0eb 9ab7 edbd a0f0 eb9a  ..G.............
+00005b80: bf4d 7820 091c aa19 ea9b be2d b540 212e  .Mx .......-.@!.
+00005b90: 6412 9c66 f077 b30f 48fc 9ce6 fdda ce6f  d..f.w..H......o
+00005ba0: 1b15 48fc 9ce6 fdda ce75 732e 4816 29f2  ..H......us.H.).
+00005bb0: 910a a777 fb0e 20fc 7bc7 adb9 2059 a4c8  ...w.. .{... Y..
+00005bc0: 472a bca6 8d57 2059 a4c8 472a bcb6 8d3e  G*...W Y..G*...>
+00005bd0: c091 1e42 f025 6221 84c9 c679 8b0e 90fc  ...B.%b!...y....
+00005be0: baa7 6b5f 8a1c c0a7 7dfa d67d c4ce 03a0  ..k_....}..}....
+00005bf0: 8898 9e29 f223 e201 04c5 a66b 430f 8022  ...).#.....kC.."
+00005c00: 627a a6c8 8f88 0710 149b be2d 3d00 8a88  bz.........-=...
+00005c10: e999 223f 221e 4050 6c3a b75d 8164 9122  .."?".@Pl:.].d."
+00005c20: 1fa9 f01a 3773 8266 719c c747 9a81 b8ea  ....7s.fq..G....
+00005c30: 7eb7 6202 c6ef 7bda a724 7bc7 fdda a409  ~.b...{..${.....
+00005c40: 18bf ef69 9f92 ec1d f76d e326 60fc bea7  ...i.....m.&`...
+00005c50: 7d4a b277 dcbf ef04 aa08 6172 223f 7006  }J.w......ar"?p.
+00005c60: cc27 1e64 399a a370 229f 6886 1ba8 b6db  .'.d9..p".h.....
+00005c70: f689 6640 0a1f f19f 8838 0860 2022 c325  ..f@.....8.` ".%
+00005c80: 9816 c779 7ca4 1988 abee 779f 926c 5d37  ...y|.....w..l]7
+00005c90: dc82 6491 221f a970 3bb7 db82 6491 221f  ..d."..p;...d.".
+00005ca0: a970 9b37 6382 c6af 711f f129 c9de 73bf  .p.7c...q..)..s.
+00005cb0: b669 82c6 af71 1ff1 29c9 de73 dfb6 6e82  .i...q..)..s..n.
+00005cc0: c6af 711f f129 c9de 73ff b6fe 8047 7a08  ..q..)..s....Gz.
+00005cd0: c197 8885 1026 9fa1 2ed3 2550 fc9e a77d  .....&....%P...}
+00005ce0: 4ab2 f5de e409 0ebf c67d c4af 4d9f e0f0  J........}..M...
+00005cf0: 6bdc 477c db04 0b0e bfc6 7dc4 bf4d b1e0  k.G|......}..M..
+00005d00: f06b dc47 7cdc 240b 0ebf c67d c4cf 4db3  .k.G|.$....}..M.
+00005d10: e0f0 6bdc 477c dd44 0b0e bfc6 7dc4 df49  ..k.G|.D....}..I
+00005d20: 3623 f1a5 e554 e356 d726 1626 e306 67c3  6#...T.V.&.&..g.
+00005d30: 96e6 16c6 7616 43f3 7556 46f7 e5f6 26d7  ....v.C.uVF...&.
+00005d40: f695 d606 c716 2343 3233 c6f6 3616 c636  ......#C23..6..6
+00005d50: 4732 5316 43f3 e656 46f4 95d6 06c7 4622  G2S.C..VF.....F"
+00005d60: 4363 1353 5413 2427 1796 9764 c694 1653  Cc.ST.$'...d...S
+00005d70: 1433 74d3 5647 1726 c656 7613 c696 76e6  .3t.VG.&.Vv...v.
+00005d80: 5646 5624 73f3 d696 4647 5746 4622 8343  VFV$s...FGWFF".C
+00005d90: 5666 1656 c746 4732 43e6 f4e6 5646 2293  Vf.V.FG2C...VF".
+00005da0: e352 8697 4667 ba05 8fdf f3b4 4f49 3e25  .R..Fg......OI>%
+00005db0: f9c4 832c 665b 902c 52e4 2315 7ed3 e63a  ...,f[.,R.#.~..:
+00005dc0: 90f8 3d4f fb4f e42c 261d 20f9 754f d7be  ..=O.O.,&. .uO..
+00005dd0: 1439 80af fbf4 9dfb 8821 0b30 7ebf f73e  .9.......!.0~..>
+00005de0: 25f9 94e4 d766 2ec0 f8fd defb 94e4 5392  %....f........S.
+00005df0: 7fdf 4753 3891 1f38 03e6 3f91 b3dc cc54  ..GS8..8..?....T
+00005e00: 3891 1f38 03e6 5392 ade7 3ef1 208b 2d07  8..8..S...>. .-.
+00005e10: 187e ee23 3e62 f005 849f ebbd 6117 5c8b  .~.#>b......a.\.
+00005e20: e33c 3ed2 0cc4 55f7 bb4f 49b6 aefb 5413  .<>...U..OI...T.
+00005e30: 59b2 00e3 f73c ed53 924f 497e 6dd8 028c  Y....<.S.OI~m...
+00005e40: dff3 b44f 493e 25f9 b605 0b28 7edf d33e  ...OI>%....(~..>
+00005e50: 25f9 9464 e702 8cdf f3b4 4f49 3e25 f9b7  %..d......OI>%..
+00005e60: ad0e 244f e42c 3e32 1191 b50f 140d 3211  ..$O.,>2......2.
+00005e70: 91c9 1718 7e4e f37e 7d02 62b0 d13e d10c  ....~N.~}.b..>..
+00005e80: 48e1 13cd 8014 3ed1 0c48 e113 cd80 143e  H.....>..H.....>
+00005e90: d10c 48e1 23e6 4eb0 4854 a300 c310 e534  ..H.#.N.HT.....4
+00005ea0: 6df3 048b 4435 0a30 0c51 4ed7 564f b048  m...D5.0.QN.VO.H
+00005eb0: 54a3 00c3 10e5 b46d f604 8b44 350a 300c  T......m...D5.0.
+00005ec0: 514e dfb6 4fb0 4854 a300 c310 e534 6efd  QN..O.HT.....4n.
+00005ed0: 048b 4435 0a30 0c51 4ee7 e64f b048 54a3  ..D5.0.QN..O.HT.
+00005ee0: 00c3 10e5 b46e 8305 8b44 350a 300c 514e  .....n...D5.0.QN
+00005ef0: ef56 58b0 4854 a300 c310 e534 6f86 058b  .VX.HT.....4o...
+00005f00: 4435 0a30 0c51 4ef7 564e f034 c844 4477  D5.0.QN.VN.4.DDw
+00005f10: cdfb 8dc0 3cfe 4daa 5189 2f2d a71a b7ba  ....<.M.Q./-....
+00005f20: 36b1 3019 3738 1bb6 34b7 30b6 b318 9aaf  6.0.78..4.0.....
+00005f30: b332 ba2f b737 b9b6 afb4 3638 b618 1992  .2./.7....68....
+00005f40: 9931 b6b7 b130 b639 9299 b218 9a37 b732  .1...0.9.....7.2
+00005f50: a2af b436 3836 1219 1a9b 98a2 9a20 39b9  ...686....... 9.
+00005f60: b0bc 2433 a6b4 98a2 98a1 9bb6 3aba 3031  ..$3........:.01
+00005f70: b6b2 9b30 b6b4 33b7 32b2 2299 9bb7 b634  ...0..3.2."....4
+00005f80: 3aba 3232 1219 1cb2 32b3 b03a 363a 9219  :.22....2..:6:..
+00005f90: 32a7 37b7 3212 991c 9732 bc34 3a17 3a34  2.7.2....2.4:.:4
+00005fa0: b9b2 3032 bb25 4816 29f2 91ea de79 8b2f  ..02.%H.)....y./
+00005fb0: 20fc 7ce7 ad92 8041 9a81 b8fc 86b8 26bf   .|....A......&.
+00005fc0: b6c5 8245 a21a 0518 8628 af69 6b2c 5824  ...E.....(.ik,X$
+00005fd0: aa51 8061 88f2 ba36 c782 45a2 1a05 1886  .Q.a...6..E.....
+00005fe0: 28af 6d2b 1658 24aa 5180 6188 f0db 3667  (.m+.X$.Q.a...6g
+00005ff0: 8145 a21a 0518 8608 bf6f 8316 5824 aa51  .E.......o..X$.Q
+00006000: 8061 88f0 1bb7 6881 45a2 1a05 1886 08bf  .a....h.E.......
+00006010: 739b 1658 24aa 5180 6188 f05b 376a 8145  s..X$.Q.a..[7j.E
+00006020: a21a 0518 8608 bf77 b316 5824 aa51 8061  .......w..X$.Q.a
+00006030: 88f0 9bb7 6c81 45a2 1a05 1886 08bf 7bb3  ....l.E.......{.
+00006040: 2c58 24aa 5180 6188 f23a b7cd 8245 a21a  ,X$.Q.a..:...E..
+00006050: 0518 8628 af75 231c 50fc 1af7 119f 92fc  ...(.u#.P.......
+00006060: da22 0714 bfc6 7dc4 a724 dfb6 c200 2322  ."....}..$....#"
+00006070: a667 8a6c 3bc0 f071 1cf7 11eb 2c58 24aa  .g.l;..q....,X$.
+00006080: 5180 6188 f27a b7cd 01c5 af71 1ff1 29c9  Q.a..z.....q..).
+00006090: bfad b260 91a8 4601 8621 ca6b dc76 0b1e  ...`..F..!.k.v..
+000060a0: bfe7 7b9f 927c 4af2 8907 598e a52b 9cc8  ..{..|J...Y..+..
+000060b0: 0f9c 01f3 29c9 a724 9f78 90c5 7f22 e220  ....)..$.x...". 
+000060c0: 8081 88cc b360 91a8 4601 8621 ca6b de26  .....`..F..!.k.&
+000060d0: 0b16 896a 1460 18a2 bcbe cdbb 2059 a4c8  ...j.`...... Y..
+000060e0: 47aa 9bef 6f81 d96e dd47 7a7f 89fc e7b0  G...o..n.Gz.....
+000060f0: 5201 c2df f3db 4c05 087f cf71 9b14 207c  R.....L....q.. |
+00006100: 7dcf 8d52 80f0 f55d b74a 01c2 d7f7 dd4a  }..R...].J.....J
+00006110: 0b16 896a 1460 18a2 dca6 4d5b 6091 a846  ...j.`....M[`..F
+00006120: 0186 21c2 71da 4e05 087f cf73 e316 5824  ..!.q.N....s..X$
+00006130: aa51 8061 8870 bc36 7181 45a2 1a05 1886  .Q.a.p.6q.E.....
+00006140: 08c7 6f1b 1758 24aa 5180 6188 701c 3776  ..o..X$.Q.a.p.7v
+00006150: 8145 a21a 0518 8608 c773 7317 5824 aa51  .E.......ss.X$.Q
+00006160: 8061 8870 5cb7 7781 45a2 1a05 1886 08c7  .a.p\.w.E.......
+00006170: 77e3 1758 24aa 5180 6188 709c 377f 8145  w..X$.Q.a.p.7..E
+00006180: a21a 0518 8608 c77b 0b15 4816 29f2 91ea  .......{..H.)...
+00006190: ee71 1b2d 5824 aa51 8061 88f2 ba37 7081  .q.-X$.Q.a...7p.
+000061a0: 45a2 1a05 1886 08c7 6dab 1748 1629 f291  E.......m..H.)..
+000061b0: eaee 75eb 2e48 1629 f291 eaee 6d33 2d58  ..u..H.)....m3-X
+000061c0: 24aa 5180 6188 72bb b6eb 0288 7890 c547  $.Q.a.r.....x..G
+000061d0: 2622 ba6d da17 98c7 fc03 08bf b769 0314  &".m.........i..
+000061e0: 20fc deae ed3f 80f0 7bdb b6c2 8145 a21a   ....?..{....E..
+000061f0: 0518 8608 cf69 3b1c 5824 aa51 8061 88f0  .....i;.X$.Q.a..
+00006200: bc36 c481 45a2 1a05 1886 08cf 6d53 1c58  .6..E.......mS.X
+00006210: 24aa 5180 6188 f0fc b6c5 8145 a21a 0518  $.Q.a......E....
+00006220: 8608 cf71 6b1c 5824 aa51 8061 88f0 3c37  ...qk.X$.Q.a..<7
+00006230: c981 45a2 1a05 1886 08cf 75a3 1c58 24aa  ..E.......u..X$.
+00006240: 5180 6188 f07c b7ca 8145 a21a 0518 8608  Q.a..|...E......
+00006250: cf79 e31c 5824 aa51 8061 88f0 bcb7 e102  .y..X$.Q.a......
+00006260: 6a71 9cc7 479a 81b8 ea7e f729 c9a7 9ac8  jq..G....~.)....
+00006270: f00b 0cff e66b 1fb1 e680 c3d7 7dc4 f611  .....k......}...
+00006280: a32f 78b6 5bf7 91de 9f88 8811 9c66 b0f2  ./x.[........f..
+00006290: 0028 22a6 678a fc88 7800 41a9 fbde e603  .(".g...x.A.....
+000062a0: 103f af7b 1f69 2a5b 1520 fcfe a60d 5580  .?.{.i*[. ....U.
+000062b0: f0f7 bd36 da81 e689 9cc5 4726 22f2 05e6  ...6......G&"...
+000062c0: b154 01c2 dff7 db2c 0508 5fef ef83 810a  .T.....,.._.....
+000062d0: 27f2 0367 c07c 4af2 8907 598e 60d9 6edb  '..g.|J...Y.`.n.
+000062e0: 279a 0129 7cc4 2e05 085f ef73 f31c 5824  '..)|...._.s..X$
+000062f0: aa51 8061 8870 9db6 cf81 45a2 1a05 1886  .Q.a.p....E.....
+00006300: 08d7 6b73 1f58 24aa 5180 6188 70dd 36f8  ..ks.X$.Q.a.p.6.
+00006310: 8145 a21a 0518 8608 d76f 931f 5824 aa51  .E.......o..X$.Q
+00006320: 8061 8870 1dbf 0cac 7022 3f70 06cc 7f22  .a.p....p"?p..."
+00006330: e220 8081 887c e959 90c9 5e07 12bf ef69  . ...|.Y..^....i
+00006340: ff89 9cc5 ea07 1689 6a14 6018 225c d7ed  ........j.`."\..
+00006350: 51c0 58a4 c847 2ad3 1f58 24aa 5180 6188  Q.X..G*..X$.Q.a.
+00006360: 70bd b7fb 8145 a21a 0518 8608 d777 a31f  p....E.......w..
+00006370: 5824 aa51 8061 8870 3db7 fc81 45a2 1a05  X$.Q.a.p=...E...
+00006380: 1886 08d7 7943 1458 ae29 0290 8988 eefa  ....yC.X.)......
+00006390: 36c3 8083 b804 a429 1c4b 1458 ae29 0290  6......).K.X.)..
+000063a0: 8988 ee3a b743 8185 6a22 6759 7e64 2222  ...:.C..j"gY~d""
+000063b0: 524c 67f6 26e7 52e6 46e6 c2f6 f606 5786  RLg.&.R.F.....W.
+000063c0: 9746 3703 93e3 52e7 26d7 c236 3637 1766  .F7...R.&..667.f
+000063d0: ea05 857f ef3e 62ae 0287 affb 885d eb36  .....>b......].6
+000063e0: 5e00 f935 ee23 3e25 d97b ee13 0fb2 d8e8  ^..5.#>%.{......
+000063f0: c0d3 2013 11dd f6ed 3702 f3f8 b7f9 0f2c  .. .....7......,
+00006400: 12d5 28c0 3044 f85e 5f00 b7d1 3ed1 0c48  ..(.0D.^_...>..H
+00006410: e113 cd80 143e d10c 48e1 13cd 8014 3e62  .....>..H.....>b
+00006420: ff03 8b44 350a 300c 11be db36 48b0 4854  ...D5.0....6H.HT
+00006430: a300 c310 e13b 6e84 048b 4435 0a30 0c11  .....;n...D5.0..
+00006440: bee7 1648 b048 54a3 00c3 10e1 fb6d 8604  ...H.HT......m..
+00006450: 8b44 350a 300c 11be eb86 48b0 4854 a300  .D5.0.....H.HT..
+00006460: c310 e1fb 6e89 048b 4435 0a30 0c11 bef3  ....n...D5.0....
+00006470: c63f b048 54a3 00c3 10e1 3b6d e105 8fdf  .?.HT.....;m....
+00006480: f3bd 4f49 f67e fbc4 832c b648 b048 54a3  ..OI.~...,.H.HT.
+00006490: 00c3 10e1 7b6f bc04 8adf f7b4 4f49 f68e  ....{o......OI..
+000064a0: 9f0a 5238 911f 3803 66be 0346 e050 cd40  ..R8..8.f..F.P.@
+000064b0: 9b78 80b4 e5b8 4f34 0352 f813 1131 82d3  .x....O4.R...1..
+000064c0: 0cf6 3b60 040e d50c f5a1 300c 320c 0be1  ..;`......0.2...
+000064d0: 078b 2328 461c 50f8 3ced 23a6 1fb0 3891  ..#(F.P.<.#...8.
+000064e0: 2f38 cde0 23b5 6da1 038a 5fd3 75ef 5392  /8..#.m..._.u.S.
+000064f0: 7f5b 23c1 2251 8d02 0c43 84f3 b439 122c  .[#."Q...C...9.,
+00006500: 12d5 28c0 3044 385f 1b24 c122 518d 020c  ..(.0D8_.$."Q...
+00006510: 4384 f3b6 4912 2c12 d528 c030 4438 7fdb  C...I.,..(.0D8..
+00006520: 24c1 2251 8d02 0c43 84f3 b8f9 122c 12d5  $."Q...C.....,..
+00006530: 28c0 3044 389f 9fc8 5311 c2e4 443e 4330  (.0D8...S...D>C0
+00006540: c241 088a 0113 2c12 d528 c030 4438 afdb  .A....,..(.0D8..
+00006550: 31c1 2251 8d02 0c43 84f3 bb25 132c 12d5  1."Q...C...%.,..
+00006560: 28c0 3044 38cf 9b32 c122 518d 020c 4384  (.0D8..2."Q...C.
+00006570: f3bd 4117 307e bff7 3e25 f9c4 832c 862f  ..A.0~..>%...,./
+00006580: 70f8 fdde fb94 649b 020a 652c 9841 3c37  p.....d...e,.A<7
+00006590: 4d5b b340 e3d7 b88f f894 e453 925f dbb7  M[.@.......S._..
+000065a0: 40e3 d7b8 8ff8 94e4 5392 6fdf 4455 3891  @.......S.o.DU8.
+000065b0: 1f38 03e6 5392 ff44 c441 0003 11d9 ba40  .8..S..D.A.....@
+000065c0: e3d7 b88f f894 e453 927f 5b33 c122 518d  .......S..[3."Q.
+000065d0: 020c 4384 f7b4 3913 2c12 d528 c030 4478  ..C...9.,..(.0Dx
+000065e0: 5f1b 34c1 2251 8d02 0c43 84f7 b651 132c  _.4."Q...C...Q.,
+000065f0: 12d5 28c0 3044 787f 1f42 b2dd b84f 3403  ..(.0Dx..B...O4.
+00006600: 52d8 35c1 2251 8d02 0c43 84f7 f975 5485  R.5."Q...C...uT.
+00006610: 13f9 8133 60fe 1311 0701 0c44 74d7 b479  ...3`......Dt..y
+00006620: 132c 12d5 28c0 3044 78af 1b38 c122 518d  .,..(.0Dx..8."Q.
+00006630: 020c 4384 f7bb c507 20fe 5de7 3ed2 54e6  ..C..... .].>.T.
+00006640: 2ba0 f8fd defb 94e4 5392 7107 183e 8eef  +.......S.q..>..
+00006650: 3e62 e902 8cdf f3bd 4f49 3e25 f9b7 2d0b  >b......OI>%..-.
+00006660: 307e cff7 3e25 f994 e4d7 664d b048 54a3  0~..>%....fM.HT.
+00006670: 00c3 10e1 3d6e ec04 8b44 350a 300c 11de  ....=n...D5.0...
+00006680: f716 4eb0 4854 a300 c310 e13d 6fd1 058c  ..N.HT.....=o...
+00006690: dff3 b44f 493e f120 cb55 6085 13f9 8133  ...OI>. .U`....3
+000066a0: 603e 25f9 94e4 3f11 7110 c040 44a4 15cd  `>%...?.q..@D...
+000066b0: ec4d cea5 cc8d cc85 eded 0dae 0c2f 8dce  .M.........../..
+000066c0: a5ce 4dae 856d 6c6e 2eec 3096 c289 fcc0  ..M..mln..0.....
+000066d0: 1930 9f92 8c59 80f1 fb9e f629 c9a7 24bf  .0...Y.....)..$.
+000066e0: 366f 01c6 ef7b daa7 249f 927c dbd4 0518  6o...{..$..|....
+000066f0: bfef 699f 927c 4af2 6fc3 2448 9066 202e  ..i..|J.o.$H.f .
+00006700: 9f6a 22a3 1778 1a64 22a2 dbe6 fd46 601e  .j"..x.d"....F`.
+00006710: ffbe 08a9 7022 3f70 06cc 7f22 e220 8081  ....p"?p...". ..
+00006720: 88ae 01db 76da 279a 0129 7ca2 1990 c227  ....v.'..)|....'
+00006730: 9a01 297c a430 f680 2b22 a667 8afc 8878  ..)|.0..+".g...x
+00006740: 0041 b1e9 de8f 8807 1014 4b27 20fc 9ea7  .A........K' ...
+00006750: efc1 db76 da27 9a01 297c a219 90c2 279a  ...v.'..)|....'.
+00006760: 0129 7ca2 1990 c247 8a0b a90a 27f2 0367  .)|....G....'..g
+00006770: c0fc 2722 0e02 1888 e8be 736b 2f48 7c7c  ..'"......sk/H||
+00006780: b77d c4c6 7beb 0e30 7c1c e77d c490 030a  .}..{..0|..}....
+00006790: 9fb7 7de4 28b0 c289 fcc0 1930 9f92 fc27  ..}.(......0...'
+000067a0: 220e 0218 88e8 be6d 5327 20fc bea7 8db7  "......mS' .....
+000067b0: e0f1 fb9e f629 c9a7 249f 7890 c584 0516  .....)..$.x.....
+000067c0: bfc6 7dc4 a724 9f92 0c78 c029 1caa 197c  ..}..$...x.)...|
+000067d0: c169 8a05 1126 131c 48fc 9ea7 7d4a f26b  .i...&..H...}J.k
+000067e0: 9b0e 307c bbcf 7dc4 9c03 0cbf ee77 1fb1  ..0|..}......w..
+000067f0: cc81 c4ef 79da a724 ffb6 c781 c4ef 79da  ....y..$......y.
+00006800: a724 df3e 10ab 7022 3f70 06cc 7f22 67f1  .$.>..p"?p..."g.
+00006810: 17c7 7988 0b99 ec3a e091 1e42 f025 6221  ..y....:...B.%b!
+00006820: 84e9 b67d c49e 030c dfa6 6f1f b1fc 00c4  ...}......o.....
+00006830: b7e9 da47 eada aa0b 9c45 8a7c a4f2 1be2  ...G.....E.|....
+00006840: 9a70 9a37 d501 6971 9cc7 479a 81b8 ea7e  .p.7..iq..G....~
+00006850: f79f c859 ac38 a0f0 f9db 476c 76a0 7922  ...Y.8....Glv.y"
+00006860: 67f1 9189 887c 890a ccba c059 a4c8 472a  g....|.....Y..G*
+00006870: bf21 ae09 afeb b3d8 0a27 f203 67c0 7c4a  .!.......'..g.|J
+00006880: f229 c97f 22e2 2080 8188 ee9b 3679 0167  .)..". .....6y.g
+00006890: 9122 1fa9 fc86 b826 bcbe 6d5e c059 a4c8  .".....&..m^.Y..
+000068a0: 472a bf21 ae09 af73 a30e 307c bbd7 7de4  G*.!...s..0|..}.
+000068b0: 36b6 c289 fcc0 1930 9f92 6c3d f79f 8838  6......0..l=...8
+000068c0: 0860 20a2 fbc6 efc2 299c c80f 9c01 f329  .` .....)......)
+000068d0: c9a7 247b 0f28 1822 3288 2369 2a42 989c  ..${.(."2.#i*B..
+000068e0: c87f 0ebf 212c 3b2f 6888 0759 7c64 2222  ....!,;/h..Y|d""
+000068f0: 5f60 1e1b 1640 24aa 5180 6188 8ea3 2a9c  _`...@$.Q.a...*.
+00006900: c80f 9c01 f39f 8838 0860 2022 bbbf edb7  .......8.` "....
+00006910: c059 a4c8 472a bf21 ae09 b775 5314 70a8  .Y..G*.!...uS.p.
+00006920: 2672 96e5 4726 22ba ebdd c203 9645 8a7c  &r..G&"......E.|
+00006930: a4f2 1be2 9a0e 220c b69d f689 6640 0a9f  ......".....f@..
+00006940: 6806 a4f0 8966 400a 9f68 06a4 f089 6640  h....f@..h....f@
+00006950: 0a03 2e70 1629 f291 ca6f 886b c2ed de92  ...p.)...o.k....
+00006960: 030a 9fc7 7de4 0c88 adae 696b 0fd0 2262  ....}.....ik.."b
+00006970: 7aa6 c88f 8807 1014 9bee fd88 7800 41b1  z...........x.A.
+00006980: eb1a 0001 3100 003f 0000 005b 0643 1083  ....1..?...[.C..
+00006990: 2d43 2314 5b06 0819 832d c384 8cc1 96e1  -C#.[....-......
+000069a0: 128a 2d03 1808 64b0 6508 0381 0cb6 0c66  ..-...d.e......f
+000069b0: 808c c196 e10c 0432 d832 a482 676c 1956  .......2.2..gl.V
+000069c0: c233 b60c 2c21 145b 0697 f08c 2d83 9c48  .3..,!.[....-..H
+000069d0: d596 4155 0e33 d832 bcca 7106 5b06 5e39  ..AU.3.2..q.[.^9
+000069e0: cc60 cb10 2ec7 196c 29ea e540 0324 0db6  .`.....l)..@.$..
+000069f0: 14fb 72a0 0192 065b 8a90 39d0 0049 832d  ..r....[..9..I.-
+00006a00: c5c9 1c68 80a4 c196 a265 0e34 40d2 604b  ...h.....e.4@.`K
+00006a10: 3133 071a 2069 b0a5 c899 030d 9034 d852  13.. i.......4.R
+00006a20: fccc 8106 481a 6c19 c646 d2b6 0c69 7398  ....H.l..F...is.
+00006a30: c196 c16d 8e33 d852 f4cd 8106 481a 6c29  ...m.3.R....H.l)
+00006a40: 40e7 4003 240d b614 a373 a001 9206 5b0a  @.@.$....s....[.
+00006a50: d339 d000 4983 2d83 2a49 db96 e19c 246e  .9..I.-.*I....$n
+00006a60: cb00 5252 b765 a029 c9db 32ec 14b2 065b  ..RR.e.)..2....[
+00006a70: 069e 42d6 60cb d053 c81a 6c19 c20a 5983  ..B.`..S..l...Y.
+00006a80: 2d43 5c21 6b00 0000 0000 0061 2000 002f  -C\!k......a ../
+00006a90: 0200 0013 0454 2c10 0000 0018 0000 0004  .....T,.........
+00006aa0: 1801 a041 1514 411d d400 8946 000a 32a0  ...A..A....F..2.
+00006ab0: a066 000a a608 0aa1 800a ace0 0a30 a020  .f...........0. 
+00006ac0: a835 0240 81a1 0e28 5ac4 a025 c4a0 2566  .5.@...(Z..%..%f
+00006ad0: 0086 3a98 e610 8396 1083 9618 ea70 9e44  ..:..........p.D
+00006ae0: 0c5a 420c 5a62 a843 9a1a 3168 0931 6889  .ZB.Zb.C..1h.1h.
+00006af0: a10e aa82 c4a0 25c4 a025 a830 0200 0033  ......%..%.0...3
+00006b00: 11c1 500b a430 1311 0cb5 400a 2306 ca03  ..P..0....@.#...
+00006b10: 8260 5007 f4d0 1d51 2404 c30d 412e 80c1  .`P....Q$...A...
+00006b20: 4c84 290c b540 0a33 11a6 30d4 0229 a410  L.)..@.3..0..)..
+00006b30: d811 0304 0241 30b0 8571 08c0 407b 6622  .....A0..q..@{f"
+00006b40: cc60 a805 52c8 21b0 2306 0804 8260 600b  .`..R.!.#....``.
+00006b50: e510 8801 17cd 4414 432d 9042 0e81 1d31  ......D.C-.B...1
+00006b60: 4020 1004 035b 3887 800c bc69 d880 1018  @ ...[8....i....
+00006b70: 0298 8930 83a1 1648 2183 c08e 1820 1008  ...0...H!.... ..
+00006b80: 8281 2da4 4360 0660 50cd 3204 82b2 b640  ..-.C`.`P.2....@
+00006b90: 6e11 20c3 0dc1 2d80 c12c c340 0423 0646  n. ...-..,.@.#.F
+00006ba0: 0482 6080 0720 8116 d3e2 023d 0192 4c60  ..`.. .....=..L`
+00006bb0: b309 ec88 0102 8120 18d8 823b 046b 5006  ....... ...;.kP.
+00006bc0: da88 81d1 8020 18e8 8148 0c42 3e81 ed00  ..... ...H.B>...
+00006bd0: 2120 830c be4b 8188 0c37 0465 1006 c30d  ! ...K...7.e....
+00006be0: 863b 84c1 05c2 ce32 1446 3062 6044 2008  .;.....2.F0b`D .
+00006bf0: 0678 b012 7111 06b3 0441 5a82 a520 4012  .x..q....AZ.. @.
+00006c00: 0b6c 0708 811a 6400 5e0a 5424 b9c0 7680  .l....d.^.T$..v.
+00006c10: 10cc 4106 dfa5 4044 120c 02db 0142 1007  ..A...@D.....B..
+00006c20: 197c 9702 1149 3208 6c07 0801 1d64 f05d  .|...I2.l....d.]
+00006c30: 0a44 24d1 20b0 1d20 0477 90c1 7729 1011  .D$. .. .w..w)..
+00006c40: 7a83 0049 3608 6cb6 4160 470c 1008 04c1  z..I6.l.A`G.....
+00006c50: c016 5e22 6005 53d8 8311 03a3 0141 30d0  ..^"`.S......A0.
+00006c60: 83b1 1884 7c83 c076 8010 9442 06df a540  ....|..v...B...@
+00006c70: 4486 1b02 5308 83e1 06e3 25c2 e002 6167  D...S.....%...ag
+00006c80: 190e 2418 3130 2210 0403 3c60 0bd9 1085  ..$.10"...<`....
+00006c90: 1183 0200 4130 e003 9e00 8359 8220 e940  ....A0.....Y. .@
+00006ca0: b079 0782 a520 4032 0f02 db01 42c0 0a19  .y... @2....B...
+00006cb0: 8097 0215 c93e 086c 0708 412d 64f0 5d0a  .....>.l..A-d.].
+00006cc0: 4424 4321 b01d 2004 b390 c177 2910 912c  D$C!.. ....w)..,
+00006cd0: 85c0 7680 10d8 4206 dfa5 4044 3215 02db  ..v...B...@D2...
+00006ce0: 0142 900b 197c 9702 11c9 5508 ec88 0102  .B...|....U.....
+00006cf0: 8120 18d8 c25b 04ec 600e bb30 6280 4920  . ...[..`..0b.I 
+00006d00: 0806 6b90 1aac a00a 7890 0be4 400e 7400  ..k.....x...@.t.
+00006d10: 076c 8006 6460 e502 3990 83e4 2886 40ab  .l..d`..9...(.@.
+00006d20: 5020 a405 48be 4260 3b40 08c0 2103 f352  P ..H.B`;@..!..R
+00006d30: 5026 390b 81ed 0021 6887 0ccc 4b41 998c  P&9....!h...KA..
+00006d40: 1814 0008 8201 1ffc c528 8c18 1400 0882  .........(......
+00006d50: 011f fc45 180c 730c 4b92 12ca 2a2c c30d  ...E..s.K...*,..
+00006d60: 0b5d 98c1 2cc3 0305 2306 4504 8260 c007  .]..,...#.E..`..
+00006d70: ae41 1f4b 1f0d 20c8 c23b 6420 580a 0264  .A.K.. ..;d X..d
+00006d80: b821 580b 3098 6568 9860 c4c0 8840 100c  .!X.0.eh.`...@..
+00006d90: fc20 3684 7b98 2570 460c 8c08 04c1 000f  . 6.{.%pF.......
+00006da0: 6aa3 3fce 6196 c019 a808 0446 579a d405  j.?.a......FW...
+00006db0: c10e 1b10 4144 00b9 0b81 ed00 2180 870c  ....AD......!...
+00006dc0: cc3b 6c40 0410 01a4 2f04 b603 8480 1f32  .;l@..../......2
+00006dd0: 30ef b001 113c 0490 e110 d811 0324 0241  0....<.......$.A
+00006de0: 3000 05dd 0848 222f 9211 8302 0041 30e0  0....H"/.....A0.
+00006df0: 83d7 c836 1831 2000 1004 0351 d00d d208  ...6.1 ....Q....
+00006e00: 6434 2100 4613 8460 3461 1046 0c0e 0004  d4!.F..`4a.F....
+00006e10: c180 147a 6310 82e1 8680 2fc0 6096 2188  ...zc...../.`.!.
+00006e20: 8261 8e21 0ca6 9590 5822 1831 2822 1004  .a.!....X".1("..
+00006e30: 033e f00d 6196 2018 3128 2210 0403 3ee8  .>..a. .1("...>.
+00006e40: 8d13 9925 0846 0c8c 0804 c100 0fca c344  ...%.F.........D
+00006e50: ec61 9620 0807 0234 0100 0006 1ce0 f8f7  .a. ...4........
+00006e60: ee17 02e0 e3fe e200 83a1 0728 12d5 28c0  ...........(..(.
+00006e70: 3044 b67d 061d d14c 11e6 13cd 8014 3ed1  0D.}...L......>.
+00006e80: 0c48 e113 cd80 143e d10c 4861 f001 8a44  .H.....>..Ha...D
+00006e90: 350a 300c 918d 9b7a 00e4 ebb6 5f08 809f  5.0....z...._...
+00006ea0: fbb5 bf38 c060 fc01 8a44 350a 300c 91ad  ...8.`...D5.0...
+00006eb0: 9fc0 4234 5384 f944 3320 85b1 0728 12d5  ..B4S..D3 ...(..
+00006ec0: 28c0 3044 f66d f601 8edf df7e 2100 3eed  (.0D.m.....~!.>.
+00006ed0: 2f0e 3018 7e80 2251 8d02 0c43 64e7 2628  /.0.~."Q...Cd.&(
+00006ee0: 40f8 b5cd 1ba0 8022 518d 020c 4364 ef86  @......"Q...Cd..
+00006ef0: 28a0 4854 a300 c310 d9fc 25bc 01d1 4c11  (.HT......%...L.
+00006f00: e613 cd80 143e d10c 48e1 13cd 8014 3ed1  .....>..H.....>.
+00006f10: 0c48 e113 cd80 143e d10c 48e1 13cd 8014  .H.....>..H.....
+00006f20: 1780 10cd 1461 3e52 18a5 00e1 d77a 6d8b  .....a>R.....zm.
+00006f30: 028a 4435 0a30 0c91 dd5f c31d 10cd 1461  ..D5.0..._.....a
+00006f40: 3ed1 0c48 e113 cd80 143e d10c 48e1 13cd  >..H.....>..H...
+00006f50: 8014 3ed1 0c48 e113 cd80 143e 52f8 4433  ..>..H.....>R.D3
+00006f60: 2085 4f2c 1261 9302 845f ebb4 4507 0c3e   .O,.a..._..E..>
+00006f70: ae9b 69c0 e0e3 bb79 0738 be6e fb85 00f8  ..i....y.8.n....
+00006f80: b4bf 38c0 60f5 0183 cfe3 461f 30f8 fc6d  ..8.`.....F.0..m
+00006f90: e201 8eaf db7e 2100 3eee 2f0e 3018 7300  .....~!.>./.0.s.
+00006fa0: e4df bb5f 0880 affb b4bf 38c0 700b 7240  ..._......8.p.r@
+00006fb0: 3453 84f9 4433 2085 4f34 0352 f844 3320  4S..D3 .O4.R.D3 
+00006fc0: 854f 3403 52f8 4433 2085 4f34 0352 f848  .O4.R.D3 .O4.R.H
+00006fd0: e113 cd80 1417 5107 4433 4598 4f34 0352  ......Q.D3E.O4.R
+00006fe0: f844 3320 854f 3403 52f8 4433 2085 4f34  .D3 .O4.R.D3 .O4
+00006ff0: 0352 f844 3320 854f 3403 52f8 48e1 2385  .R.D3 .O4.R.H.#.
+00007000: 8506 087e 6ea2 0182 afdb 6880 e0ef 461a  ...~n.....h...F.
+00007010: 20f8 bc0d 0a10 7e7d db56 2860 f8b5 ddfb   .....~}.V(`....
+00007020: b411 0a10 7e7d e387 9006 4433 4598 4f34  ....~}....D3E.O4
+00007030: 0352 f844 3320 854f 3403 52f8 4433 2085  .R.D3 .O4.R.D3 .
+00007040: 4f34 0352 f844 3320 c539 e001 d14c 11e6  O4.R.D3 .9...L..
+00007050: 13cd 8014 3ed1 0c48 e113 cd80 143e d10c  ....>..H.....>..
+00007060: 48e1 13cd 8014 3ed1 0c48 e123 854f 3403  H.....>..H.#.O4.
+00007070: 52f8 4433 2085 b906 0c7e 6d1f 4041 3453  R.D3 ....~m.@A4S
+00007080: 84dd 8119 10cd 1461 3ed1 0c48 e113 cd80  .......a>..H....
+00007090: 143e d10c 48e1 13cd 8014 3ed1 0c48 e123  .>..H.....>..H.#
+000070a0: c515 7844 3345 984f 3403 52f8 4433 2085  ..xD3E.O4.R.D3 .
+000070b0: 4f34 0352 f8d3 1111 c060 d401 839f d7f6  O4.R.....`......
+000070c0: 1a30 f8f5 6ed8 0183 9fe7 961d 30f8 b96e  .0..n.......0..n
+000070d0: da01 839f efb6 1d30 f839 7f13 6740 3453  .......0.9..g@4S
+000070e0: 84f9 4433 2085 4f34 0352 f844 3320 854f  ..D3 .O4.R.D3 .O
+000070f0: f8be 4f34 0352 f844 3320 8549 070c 7e4e  ..O4.R.D3 .I..~N
+00007100: 9b7b 00e4 ebb6 5f08 80af fbb4 bf38 c060  .{...._......8.`
+00007110: c401 907f ef7e 2100 7eee d3fe e200 8341  .....~!.~......A
+00007120: 0740 febd fb85 00f8 ba5f fb8b 030c f61f  .@......._......
+00007130: 30f8 7d6d ac01 845f e3f4 29bc 01d1 4c11  0.}m..._..)...L.
+00007140: e613 cd80 143e d10c 48e1 13cd 8014 3ed1  .....>..H.....>.
+00007150: 0c48 e113 cd80 143e d10c 48e1 2385 8f14  .H.....>..H.#...
+00007160: 5618 a03c d82f 2c8e 4445 8435 0a10 7e8d  V..<./,.DE.5..~.
+00007170: dfe6 2840 f835 8e9b 6ac0 415c 02d2 148e  ..(@.5..j.A\....
+00007180: c106 0cbe 5d5b 69c0 e0db f641 d401 d14c  ....][i....A...L
+00007190: 11e6 13cd 8014 3ed1 0c48 e113 cd80 143e  ......>..H.....>
+000071a0: d10c 48e1 13cd 8014 3ed1 0c48 e113 cd80  ..H.....>..H....
+000071b0: 143e d10c 4861 8601 c783 fd40 6448 161b  .>..Ha.....@dH..
+000071c0: 30f8 766e b301 836f ebc7 5007 4433 4598  0.vn...o..P.D3E.
+000071d0: 4f34 0352 f844 3320 854f 3403 52f8 4433  O4.R.D3 .O4.R.D3
+000071e0: 2085 4f34 0352 f844 3320 858f 143e d10c   .O4.R.D3 ...>..
+000071f0: 48e1 23c5 1144 4433 4598 4f34 0352 f844  H.#..DD3E.O4.R.D
+00007200: 3320 c53d c801 d14c 11e6 13cd 8014 3ed1  3 .=...L......>.
+00007210: 0c48 e113 cd80 143e d10c 48e1 13cd 8014  .H.....>..H.....
+00007220: 3ed1 0c48 e113 cd80 143e 5258 6d00 2251  >..H.....>RXm."Q
+00007230: 8d02 0c43 6487 01c6 83fd 8a25 9979 00e4  ...Cd......%.y..
+00007240: ebb6 5f08 809f fbb4 bf38 c060 f201 90af  .._......8.`....
+00007250: db7e 2100 beee d7fe e200 8321 0740 febd  .~!........!.@..
+00007260: fb85 00f8 b95f fb8b 030c e61b a048 54a3  ....._.......HT.
+00007270: 00c3 10d5 b809 0728 12d5 28c0 3044 757e  .......(..(.0Du~
+00007280: 030e d14c 11e6 13cd 8014 3e52 9872 8022  ...L......>R.r."
+00007290: 518d 020c 4354 efe6 1ca0 4854 a300 c310  Q...CT....HT....
+000072a0: d5bc 5907 2812 d528 c030 4475 6f8f 0284  ..Y.(..(.0Duo...
+000072b0: 5fe7 b819 0728 12d5 28c0 3044 b56e 9002  _....(..(.0D.n..
+000072c0: 845f e7b9 450a 107e 9def 2629 40f8 75de  ._..E..~..&)@.u.
+000072d0: 9f84 4734 5384 f944 3320 854f 3403 52f8  ..G4S..D3 .O4.R.
+000072e0: 4433 2085 4ff8 be8f 1476 1b30 f837 6db8  D3 .O....v.0.7m.
+000072f0: 0183 7fd7 961b 30f8 b76d ba01 837f df86  ......0..m......
+00007300: 1a30 f87b 6dbc 018e 7fef 7e21 003e ed2f  .0.{m.....~!.>./
+00007310: 0e30 1878 8022 518d 020c 4364 d346 1ea0  .0.x."Q...Cd.F..
+00007320: 4854 a300 c310 d935 0000 0001 3100 0006  HT.....5....1...
+00007330: 0000 005b 0649 28b6 0c96 506c 19ca 4028  ...[.I(...Pl..@(
+00007340: b60c aa20 145b 069c 100a 0000 0000 0061  ... .[.........a
+00007350: 2000 0037 0100 0013 0449 2c10 0000 0010   ..7.....I,.....
+00007360: 0000 0004 1801 a041 2914 4311 9441 2154  .......A).C..A!T
+00007370: 411d d400 8946 0066 004a a020 03a8 3502  A....F.f.J. ..5.
+00007380: 4081 1980 a10e eb8a c400 26c4 0026 863a  @.........&..&.:
+00007390: a84a 1203 9810 0398 a0c2 0800 9566 00c8  .J...........f..
+000073a0: 3403 0033 1166 30d4 0229 6420 d86e 1a84  4..3.f0..)d .n..
+000073b0: 0615 ba69 181c aa9b 06e2 a1ba 6928 20aa  ...i........i( .
+000073c0: 9b08 23ca a26e 220e 4983 ba89 4026 6dea  ..#..n".I...@&m.
+000073d0: 2622 a136 6926 a218 6a81 1472 09ec 8801  &".6i&..j..r....
+000073e0: 0281 2018 d882 3804 6040 4dc3 0684 f010  .. ...8.`@M.....
+000073f0: c068 8218 00a3 0963 408c 2690 4131 9a10  .h.....c@.&.A1..
+00007400: 00a3 0942 309a 7006 c668 4200 8c26 08c1  ...B0.p..hB..&..
+00007410: 6842 1a00 a309 6a40 8c26 ac41 319a 1000  hB....j@.&.A1...
+00007420: a309 4230 9ae0 06c6 6842 008c 2608 c188  ..B0....hB..&...
+00007430: 0126 8120 18ac 014b 7012 2406 6660 064f  .&. ...Kp.$.f`.O
+00007440: c328 0922 0666 6006 4741 0801 4d05 425d  .(.".f`.GA..M.B]
+00007450: 80cc 3680 4100 9017 20b3 0d42 10d0 2722  ..6.A... ..B..'"
+00007460: b30d 4220 1018 88c8 6c83 100c 1406 2432  ..B ....l.....$2
+00007470: db20 0404 8981 8890 1888 0889 8188 9018  . ..............
+00007480: 88c8 6c83 1b10 c06c 4340 04b3 0d70 4000  ..l....lC@...p@.
+00007490: b30d 0111 cc36 2443 31db 1008 c64c c430  .....6$C1....L.0
+000074a0: d4c2 280c 1b10 c148 0cc0 30c7 7005 2d21  ..(....H..0.p.-!
+000074b0: ac82 30dc 708d 8419 8c18 1411 0882 812a  ..0.p..........*
+000074c0: d484 30cb 4014 c10e 2306 0500 8260 c00a  ..0.@...#....`..
+000074d0: 3491 0723 0605 0082 60c0 0734 118c 1814  4..#....`..4....
+000074e0: 0008 8201 1fcc 4430 6250 4420 0806 aa20  ......D0bPD ... 
+000074f0: 13c3 2c81 3062 4000 2008 06a2 b013 8411  ..,.0b@. .......
+00007500: c868 4200 8c26 08c1 68c2 208c 181c 0008  .hB..&..h. .....
+00007510: 8201 29f8 c420 04c3 0d41 3f80 c12c c360  ..).. ...A?..,.`
+00007520: 04c3 1cc3 87b8 c4f1 12c3 8841 1181 2018  ...........A.. .
+00007530: f0c1 4f08 b304 c388 4111 8120 18f0 814f  ..O.....A.. ...O
+00007540: a0c6 2cc1 3062 6044 2008 0678 6016 a7f1  ..,.0b`D ..x`...
+00007550: 07b3 0443 3810 00b1 0000 0016 1ac0 f885  ...C8...........
+00007560: 00f8 b94f fb06 f198 6800 e317 02e0 e77e  ...O....h......~
+00007570: ed1b c463 a901 0f71 4d11 204c c4e0 4b07  ...c...qM. L..K.
+00007580: f010 27b0 10cd 1461 3ed1 0c48 61b4 0113  ..'....a>..Ha...
+00007590: 714d 1120 4cc4 e04b 5384 0c84 e4d7 1780  qM. L..KS.......
+000075a0: 10cd 1461 3e52 1870 00e4 dbba 5f08 807f  ...a>R.p...._...
+000075b0: fb48 2311 d164 cd01 838f df37 30f8 b86e  .H#..d.....70..n
+000075c0: b901 8e6f eb7e 2100 3eed 2f0e 3018 74c0  ...o.~!.>./.0.t.
+000075d0: e0e3 bd9d 0644 c435 4580 3011 83cf 100c  .....D.5E.0.....
+000075e0: d214 8e05 0738 bead fb85 00f8 b8bf 38c0  .....8........8.
+000075f0: 6085 0182 5f9b 6180 e0db d619 a0f8 8500  `..._.a.........
+00007600: f8b5 6f10 8f6d 0608 3e6e 9e01 8a5f 0880  ..o..m..>n..._..
+00007610: 6ffb 06f1 d867 80e2 1702 e0df be41 3c06  o....g.......A<.
+00007620: 1aa0 f885 00f8 b86f 108f a906 083e 6fab  .......o.....>o.
+00007630: 0182 df5f 8143 3453 84f9 48e1 13cd 8014  ..._.C4S..H.....
+00007640: c61c 0021 8d44 4413 31f8 d214 2103 2159  ...!.DD.1...!.!Y
+00007650: 6bc0 e0d7 b4b9 060c 7e5d 9b6f 00e4 dbba  k.......~].o....
+00007660: 5f08 806f fb48 2311 d174 0005 d14c 1166  _..o.H#..t...L.f
+00007670: b301 835f df26 1b30 f8b5 6db6 0183 5fe7  ..._.&.0..m..._.
+00007680: 561b 30f8 356e b801 835f ef76 1b30 f8b5  V.0.5n..._.v.0..
+00007690: 6ed1 0183 9fd3 361d 30f8 396e bb01 8e6f  n.....6.0.9n...o
+000076a0: eb7e 2100 7eed 2f0e 3058 75c0 e0e7 ba2d  .~!.~./.0Xu....-
+000076b0: 0738 4823 11d1 440c be74 000f 61c5 0190  .8H#..D..t..a...
+000076c0: 6feb 7e21 00be eed3 fee2 0083 4907 0c7e  o.~!........I..~
+000076d0: 6e1b 75c0 e0e7 b98d 0630 7e21 00be eed3  n.u......0~!....
+000076e0: be41 3c46 1ac0 f885 00f8 ba5f fb06 f11c  .A<F......._....
+000076f0: 8246 3453 84f9 48e1 13cd 8014 3ed1 0c48  .F4S..H.....>..H
+00007700: e113 cd80 1456 1a70 1097 8034 8563 a801  .....V.p...4.c..
+00007710: 0e71 4d11 204c c4e0 0fc0 041c c142 3453  .qM. L.......B4S
+00007720: 84f9 48e1 2385 f106 40be adfb 8500 f8b5  ..H.#...@.......
+00007730: 8f34 1211 4dc6 19b0 f885 00f8 b46f 104f  .4..M........o.O
+00007740: 6dce 0183 6fe3 d61b e0f8 b6ee 1702 e0db  m...o...........
+00007750: fee2 0083 0d07 40be adfb 8500 f8b9 4ffb  ......@.......O.
+00007760: 8b03 0c66 1c00 f9b6 ee17 02e0 eb7e ed2f  ...f.........~./
+00007770: 0e30 dc41 4434 5384 f948 e113 cd80 143e  .0.AD4S..H.....>
+00007780: 5258 6c40 445c 5304 0813 31f8 d201 3c84  RXl@D\S...1...<.
+00007790: 5fdb 73c0 e0eb fc19 3844 3345 988f 143e  _.s.....8D3E...>
+000077a0: 52f8 4861 b001 1071 4d11 204c c4e0 0fc0  R.Ha...qM. L....
+000077b0: 04f8 b5e9 0640 bead fb85 00f8 b48f 3412  .....@........4.
+000077c0: 114d c61a 1011 d714 01c2 440c be34 45c8  .M........D..4E.
+000077d0: 4048 261c 00f9 b6ee 1702 e0e3 3ed2 4844  @H&.........>.HD
+000077e0: 3419 72c0 e0df b629 070c fe7d db6b c044  4.r....)...}.k.D
+000077f0: 5c53 0408 1331 f80c c120 4de1 f8b5 fd06  \S...1... M.....
+00007800: 38be adfb 8500 f8b7 bf38 c060 c401 906f  8........8.`...o
+00007810: eb7e 2100 7eee d7fe e200 0300 0000 0001  .~!.~...........
+00007820: 3100 0002 0000 005b 8653 100a 0000 0000  1......[.S......
+00007830: 0000 0061 2000 0025 0100 0013 0449 2c10  ...a ..%.....I,.
+00007840: 0000 0009 0000 0004 1801 28f3 001a 9441  ..........(....A
+00007850: 0115 0189 4600 4aa0 608a a010 0aaa 402c  ....F.J.`.....@,
+00007860: 0b22 d41a 01a0 806d 6f08 00f1 3000 0049  .".....mo...0..I
+00007870: 0000 0022 47c8 9051 0e08 8a00 0000 00af  ..."G..Q........
+00007880: 900b b800 0000 005f 5a4e 356e 756d 6261  ......._ZN5numba
+00007890: 326e 7036 6c69 6e61 6c67 3235 5f64 756d  2np6linalg25_dum
+000078a0: 6d79 5f6c 6976 656e 6573 735f 6675 6e63  my_liveness_func
+000078b0: 2432 3432 3945 3330 6c69 7374 2432 3869  $2429E30list$28i
+000078c0: 6e74 3634 2432 3924 3363 6976 2433 644e  nt64$29$3civ$3dN
+000078d0: 6f6e 6524 3365 5f5a 4e35 6e75 6d62 6132  one$3e_ZN5numba2
+000078e0: 6e70 366c 696e 616c 6732 355f 6475 6d6d  np6linalg25_dumm
+000078f0: 795f 6c69 7665 6e65 7373 5f66 756e 6324  y_liveness_func$
+00007900: 3234 3239 4533 306c 6973 7424 3238 696e  2429E30list$28in
+00007910: 7436 3424 3239 2433 6369 7624 3364 4e6f  t64$29$3civ$3dNo
+00007920: 6e65 2433 653a 2025 6578 6369 6e66 6f5f  ne$3e: %excinfo_
+00007930: 5a4e 356e 756d 6261 326e 7036 6c69 6e61  ZN5numba2np6lina
+00007940: 6c67 3235 5f64 756d 6d79 5f6c 6976 656e  lg25_dummy_liven
+00007950: 6573 735f 6675 6e63 2432 3432 3945 3330  ess_func$2429E30
+00007960: 6c69 7374 2432 3869 6e74 3634 2432 3924  list$28int64$29$
+00007970: 3363 6976 2433 644e 6f6e 6524 3365 3a20  3civ$3dNone$3e: 
+00007980: 2572 6574 7074 722b 8405 5931 304b b262  %retptr+..Y10K.b
+00007990: 6816 6583 d030 0023 0606 1082 6010 07f0  h.e..0.#....`...
+000079a0: 6030 0d20 0449 06e0 a540 4586 1b2e 070c  `0. .I...@E.....
+000079b0: 6619 8421 1831 2880 1004 033e 1087 62c4  f..!.1(....>..b.
+000079c0: 8000 4210 0c60 211c 860d 888e 2408 605d  ..B..`!.....$.`]
+000079d0: 61d8 80e8 4682 00d6 1532 1b59 5e23 bb40  a...F....2.Y^#.@
+000079e0: a00c 4434 6290 0021 0806 b250 0ed8 c605  ..D4b..!...P....
+000079f0: c770 43d0 0b68 30cb 1010 c188 8101 8420  .pC..h0........ 
+00007a00: 18d0 4239 44cd 7043 200b 6030 cb50 18c1  ..B9D.pC .`0.P..
+00007a10: b001 5106 2a41 006b 0b0d 2008 5606 e9a5  ..Q.*A.k.. .V...
+00007a20: 004d fa79 08b6 5c18 3620 828c 0092 502f  .M.y..\.6 ....P/
+00007a30: 055f 326c 4004 1e01 5081 26fd 3c04 1f18  ._2l@...P.&.<...
+00007a40: 0c1b 1041 1904 001d 68d2 cf43 1006 6490  ...A....h..C..d.
+00007a50: 4160 470c 9029 04c1 c016 e221 4083 6ea3  A`G..).....!@.n.
+00007a60: e34b 860d 8820 0c08 8016 34e9 e721 2803  .K... ....4..!(.
+00007a70: 3418 3620 8232 2000 6ad0 a49f 87e0 0cd4  4.6 .2 .j.......
+00007a80: a089 84e0 0c86 0d88 600e 0880 9a2f a140  ........`..../.@
+00007a90: 4486 1b02 3540 8359 8603 0932 0fbe 3b6c  D...5@.Y...2..;l
+00007aa0: 4004 6640 00bb 0e23 0645 1482 60c0 0720  @.f@...#.E..`.. 
+00007ab0: 7125 1824 9782 c118 3128 8010 0403 3e10  q%.$....1(....>.
+00007ac0: 8932 c83e 48ee b001 1108 03b0 f810 0e04  .2.>H...........
+00007ad0: 0000 0070 0000 0087 b06d bcee 13cd 8014  ...p.....m......
+00007ae0: 3ed1 0c48 e113 cd80 143e d10c 4871 03da  >..H.....>..Hq..
+00007af0: 46fb 4433 2085 4f34 0352 f844 3320 854f  F.D3 .O4.R.D3 .O
+00007b00: 3403 5258 6900 e1db b46e 8c01 0910 193e  4.RXi....n.....>
+00007b10: e0e7 3e7d 02d7 46fb 4433 2085 4f34 0352  ..>}..F.D3 .O4.R
+00007b20: f844 3320 858f 1417 306c bb6d a201 847f  .D3 ....0l.m....
+00007b30: ebb7 e106 107e 6ef3 e61b 50f8 b7ee 2386  .....~n...P...#.
+00007b40: 1a40 f8b7 bd5b 6bc0 e1eb 3e62 dfb6 d106  .@...[k...>b....
+00007b50: 103e cef3 161c 60f8 ba6d dff5 1130 1baf  .>....`..m...0..
+00007b60: fb44 3320 858f 1476 1b80 f8ba 8fd4 b5bd  .D3 ...v........
+00007b70: 9b69 00e1 db75 6ea9 0184 8fe7 b4a9 0610  .i...un.........
+00007b80: 3e9e d716 1b80 f8ba 8fd8 f78d db6a 40e1  >............j@.
+00007b90: e73e 529f 41b5 f1ba 4f34 0352 f844 3320  .>R.A...O4.R.D3 
+00007ba0: 854f 3403 52d8 6900 e1db fd7e 0005 d14c  .O4.R.i....~...L
+00007bb0: 1166 b501 848f f7bd 7906 107e ee23 961b  .f......y..~.#..
+00007bc0: 70f8 ba8f ec76 6f9d 0184 5fd3 bce9 0610  p....vo..._.....
+00007bd0: 7e8e dbb6 1b40 f839 7e5b 6340 0244 860f  ~....@.9~[c@.D..
+00007be0: f8ba 4f9b 61c0 415c 02d2 148e f506 14fe  ..O.a.A\........
+00007bf0: 9dfb 88cd 0620 beee 2375 7feb 7780 6dbc  ..... ..#u..w.m.
+00007c00: ee13 cd80 143e d10c 48e1 13cd 8014 3e52  .....>..H.....>R
+00007c10: 986b 00e1 e3fa 6db6 0189 affb 489d dbb9  .k....m.....H...
+00007c20: 6d85 0146 444c cf14 1968 80e1 eb3e 62e3  m..FDL...h...>b.
+00007c30: 061b 80f8 ba8f e0f7 5ddb 61c0 0144 860f  ........].a..D..
+00007c40: f8b4 2106 1c40 64f8 805f 5b62 c001 4486  ..!..@d.._[b..D.
+00007c50: 0ff8 b629 061c 4064 f880 7fdb 62c0 0144  ...)..@d....b..D
+00007c60: 860f f8b8 c906 103e bee7 461a 40f8 75bf  .......>..F.@.u.
+00007c70: db68 00e1 d73d 6fa1 0184 5ff7 bdf1 0624  .h...=o..._....$
+00007c80: beee 23b8 ee23 f715 481b affb 4433 2085  ..#..#..H...D3 .
+00007c90: 4f34 0352 f848 0101 3100 000b 0000 005b  O4.R.H..1......[
+00007ca0: 8642 28b6 0c89 676c 1916 cfd8 3254 42b1  .B(...gl....2TB.
+00007cb0: 65b8 3c63 cb00 0748 b365 8803 a4d9 32cc  e.<c...H.e....2.
+00007cc0: 8150 6c19 ecc0 3300 0000 0000 0000 0061  .Pl...3........a
+00007cd0: 2000 0026 0000 0013 0444 2c10 0000 0001   ..&.....D,.....
+00007ce0: 0000 0024 2a01 00c3 0dc2 1b80 c12c 4320  ...$*........,C 
+00007cf0: 043a 6420 1041 0edf 1d33 3082 4100 8460  .:d .A...30.A..`
+00007d00: b821 20c0 6096 6108 8221 0361 0846 0c8a  .! .`.a..!.a.F..
+00007d10: 2804 c180 0f4a c1d0 7020 000e 0000 00a6  (....J..p ......
+00007d20: 1830 f835 7d00 827f db61 80e0 e337 b0f8  .0.5}....a...7..
+00007d30: b74f 3403 52f8 4871 0288 7ffb 4433 2085  .O4.R.Hq....D3 .
+00007d40: 2106 083e 6f89 0184 8ffb c805 14fe ed23  !..>o..........#
+00007d50: 8515 0608 7e0d 0001 3100 0003 0000 005b  ....~...1......[
+00007d60: 8640 28b6 0c87 5000 0000 0000 0000 0061  .@(...P........a
+00007d70: 2000 0007 0000 0013 0481 8603 0100 0003   ...............
+00007d80: 0000 0007 20f8 b715 0608 7e0d 0000 0000  .... .....~.....
+00007d90: 0000 0061 2000 001a 0000 0013 0443 2c10  ...a ........C,.
+00007da0: 0000 0001 0000 0024 2a01 00c3 0dc2 1b80  .......$*.......
+00007db0: c12c 4320 049a c377 c70c 8c60 0800 21d0  .,C ...w...`..!.
+00007dc0: 7020 000a 0000 0007 20f8 b71d 0608 3e7e  p ...... .....>~
+00007dd0: 0288 7ffb 4433 2085 2106 08fe 6e89 0184  ....D3 .!...n...
+00007de0: 8ffb c805 14fe ed23 8515 0608 7e0d 0001  .......#....~...
+00007df0: 3100 0002 0000 005b 8640 2800 0000 0000  1......[.@(.....
+00007e00: 0000 0071 2000 0008 0000 0032 0e10 2284  ...q ......2..".
+00007e10: 2b96 09e8 02c8 8139 b120 f8a3 2e82 4091  +......9. ....@.
+00007e20: 2538 945b 8247 c225 0000 0000 0000 0065  %8.[.G.%.......e
+00007e30: 0c00 0005 0200 0012 0394 2828 0000 0002  ..........((....
+00007e40: 0000 0062 0c00 0006 0000 004c 0000 0001  ...b.......L....
+00007e50: 0000 0058 0000 0000 0000 0058 0000 004b  ...X.......X...K
+00007e60: 0000 0060 0700 0007 0000 0068 0c00 0019  ...`.......h....
+00007e70: 0000 0081 0c00 0008 0000 0097 0000 0000  ................
+00007e80: 0000 0008 0800 0000 0000 0000 0000 004b  ...............K
+00007e90: 0000 0000 0000 0089 0c00 008e 0000 0052  ...............R
+00007ea0: 0800 008d 0000 00ff ffff ff10 2600 0017  ............&...
+00007eb0: 0d00 001c 0000 00df 0800 001b 0000 00ff  ................
+00007ec0: ffff ff08 2c00 0033 0d00 001f 0000 00fa  ....,..3........
+00007ed0: 0800 001e 0000 00ff ffff ff08 2400 0052  ............$..R
+00007ee0: 0d00 0096 0000 0018 0900 0095 0000 00ff  ................
+00007ef0: ffff ff10 2600 00e8 0d00 0012 0000 00ad  ....&...........
+00007f00: 0900 0011 0000 00ff ffff ff08 2400 00fa  ............$...
+00007f10: 0d00 0010 0000 00be 0900 000f 0000 00ff  ................
+00007f20: ffff ff08 2400 000a 0e00 001e 0000 00cd  ....$...........
+00007f30: 0900 001d 0000 00ff ffff ff08 2400 0028  ............$..(
+00007f40: 0e00 000a 0000 00ea 0900 0009 0000 00ff  ................
+00007f50: ffff ff08 2400 0032 0e00 000f 0000 00f3  ....$..2........
+00007f60: 0900 000e 0000 00ff ffff ff08 2400 0041  ............$..A
+00007f70: 0e00 0023 0000 0001 0a00 0022 0000 00ff  ...#......."....
+00007f80: ffff ff08 2400 0064 0e00 000c 0000 0023  ....$..d.......#
+00007f90: 0a00 000b 0000 00ff ffff ff08 2400 0070  ............$..p
+00007fa0: 0e00 000f 0000 002e 0a00 000e 0000 00ff  ................
+00007fb0: ffff ff08 2400 007f 0e00 000f 0000 003c  ....$..........<
+00007fc0: 0a00 000e 0000 00ff ffff ff08 2400 008e  ............$...
+00007fd0: 0e00 000e 0000 004a 0a00 000d 0000 00ff  .......J........
+00007fe0: ffff ff08 2400 009c 0e00 0094 0000 0057  ....$..........W
+00007ff0: 0a00 0093 0000 00ff ffff ff10 2600 0030  ............&..0
+00008000: 0f00 0011 0000 00ea 0a00 0010 0000 00ff  ................
+00008010: ffff ff08 2400 0041 0f00 0015 0000 00fa  ....$..A........
+00008020: 0a00 0014 0000 00ff ffff ff08 2400 0056  ............$..V
+00008030: 0f00 0016 0000 000e 0b00 0015 0000 00ff  ................
+00008040: ffff ff08 2400 006c 0f00 000a 0000 0023  ....$..l.......#
+00008050: 0b00 0009 0000 00ff ffff ff08 2400 0076  ............$..v
+00008060: 0f00 0012 0000 002c 0b00 0011 0000 00ff  .......,........
+00008070: ffff ff08 2400 0088 0f00 005f 0000 003d  ....$......_...=
+00008080: 0b00 005e 0000 00ff ffff ff10 2600 00e7  ...^........&...
+00008090: 0f00 000b 0000 009b 0b00 000a 0000 00ff  ................
+000080a0: ffff ff10 2600 00f2 0f00 0012 0000 00a5  ....&...........
+000080b0: 0b00 0011 0000 00ff ffff ff08 2400 0004  ............$...
+000080c0: 1000 000d 0000 00b6 0b00 000c 0000 00ff  ................
+000080d0: ffff ff08 2400 0011 1000 0011 0000 00c2  ....$...........
+000080e0: 0b00 0010 0000 00ff ffff ff10 2400 0022  ............$.."
+000080f0: 1000 001d 0000 00d2 0b00 001c 0000 00ff  ................
+00008100: ffff ff08 2400 003f 1000 0015 0000 00ee  ....$..?........
+00008110: 0b00 0014 0000 00ff ffff ff08 2c00 0054  ............,..T
+00008120: 1000 0016 0000 0002 0c00 0015 0000 00ff  ................
+00008130: ffff ff08 2400 006a 1000 000b 0000 0017  ....$..j........
+00008140: 0c00 000a 0000 00ff ffff ff10 2600 0075  ............&..u
+00008150: 1000 0019 0000 0021 0c00 0018 0000 00ff  .......!........
+00008160: ffff ff08 2c00 008e 1000 0017 0000 0039  ....,..........9
+00008170: 0c00 0016 0000 00ff ffff ff08 2c00 00a5  ............,...
+00008180: 1000 0014 0000 004f 0c00 0013 0000 00ff  .......O........
+00008190: ffff ff08 2c00 00b9 1000 0098 0000 0000  ....,...........
+000081a0: 0000 0097 0000 00ff ffff ff24 0400 0051  ...........$...Q
+000081b0: 1100 0021 0000 0097 0000 0020 0000 00ff  ...!....... ....
+000081c0: ffff ff00 0000 0072 1100 0021 0000 00b7  .......r...!....
+000081d0: 0000 0020 0000 00ff ffff ff00 0000 0093  ... ............
+000081e0: 1100 0022 0000 00d7 0000 0021 0000 00ff  ...".......!....
+000081f0: ffff ff00 0000 00b5 1100 0027 0000 00f8  ...........'....
+00008200: 0000 0026 0000 00ff ffff ff00 0000 00dc  ...&............
+00008210: 1100 0022 0000 001e 0100 0021 0000 00ff  ...".......!....
+00008220: ffff ff00 0000 00fe 1100 0027 0000 003f  ...........'...?
+00008230: 0100 0026 0000 00ff ffff ff00 0000 0025  ...&...........%
+00008240: 1200 0024 0000 0065 0100 0023 0000 00ff  ...$...e...#....
+00008250: ffff ff00 0000 0049 1200 0013 0000 0088  .......I........
+00008260: 0100 0012 0000 00ff ffff ff08 0400 005c  ...............\
+00008270: 1200 00b4 0000 009a 0100 00b3 0000 00ff  ................
+00008280: ffff ff00 0000 0010 1300 0010 0000 004d  ...............M
+00008290: 0200 000f 0000 00ff ffff ff08 0400 0020  ............... 
+000082a0: 1300 0060 0000 005c 0200 005f 0000 00ff  ...`...\..._....
+000082b0: ffff ff00 0000 0080 1300 000f 0000 00bb  ................
+000082c0: 0200 000e 0000 00ff ffff ff08 0400 008f  ................
+000082d0: 1300 002c 0000 00c9 0200 002b 0000 00ff  ...,.......+....
+000082e0: ffff ff00 0000 00bb 1300 0014 0000 00f4  ................
+000082f0: 0200 0013 0000 00ff ffff ff08 0400 00cf  ................
+00008300: 1300 0012 0000 0007 0300 0011 0000 00ff  ................
+00008310: ffff ff08 0400 00e1 1300 0032 0000 0018  ...........2....
+00008320: 0300 0031 0000 00ff ffff ff00 0000 0013  ...1............
+00008330: 1400 003c 0000 0049 0300 003b 0000 00ff  ...<...I...;....
+00008340: ffff ff00 0000 004f 1400 0034 0000 0084  .......O...4....
+00008350: 0300 0033 0000 00ff ffff ff00 0000 0083  ...3............
+00008360: 1400 0059 0000 00b7 0300 0058 0000 00ff  ...Y.......X....
+00008370: ffff ff24 0400 00dc 1400 0021 0000 000f  ...$.......!....
+00008380: 0400 0020 0000 00ff ffff ff00 0000 00fd  ... ............
+00008390: 1400 0021 0000 002f 0400 0020 0000 00ff  ...!.../... ....
+000083a0: ffff ff00 0000 001e 1500 0022 0000 004f  ..........."...O
+000083b0: 0400 0021 0000 00ff ffff ff00 0000 0040  ...!...........@
+000083c0: 1500 0027 0000 0070 0400 0026 0000 00ff  ...'...p...&....
+000083d0: ffff ff00 0000 0067 1500 0022 0000 0096  .......g..."....
+000083e0: 0400 0021 0000 00ff ffff ff00 0000 0089  ...!............
+000083f0: 1500 0027 0000 00b7 0400 0026 0000 00ff  ...'.......&....
+00008400: ffff ff00 0000 00b0 1500 0048 0000 00dd  ...........H....
+00008410: 0400 0047 0000 00ff ffff ff24 0400 00f8  ...G.......$....
+00008420: 1500 004a 0000 0024 0500 0049 0000 00ff  ...J...$...I....
+00008430: ffff ff24 0400 0042 1600 0089 0000 006d  ...$...B.......m
+00008440: 0500 0088 0000 00ff ffff ff24 0400 00cb  ...........$....
+00008450: 1600 0069 0000 00f5 0500 0068 0000 00ff  ...i.......h....
+00008460: ffff ff24 0400 0034 1700 005a 0000 005d  ...$...4...Z...]
+00008470: 0600 0059 0000 00ff ffff ff24 0400 008e  ...Y.......$....
+00008480: 1700 0021 0000 00b6 0600 0020 0000 00ff  ...!....... ....
+00008490: ffff ff00 0000 00af 1700 0021 0000 00d6  ...........!....
+000084a0: 0600 0020 0000 00ff ffff ff00 0000 00d0  ... ............
+000084b0: 1700 0021 0000 00f6 0600 0020 0000 00ff  ...!....... ....
+000084c0: ffff ff00 0000 00f1 1700 0021 0000 0016  ...........!....
+000084d0: 0700 0020 0000 00ff ffff ff00 0000 0012  ... ............
+000084e0: 1800 0022 0000 0036 0700 0021 0000 00ff  ..."...6...!....
+000084f0: ffff ff00 0000 0034 1800 0027 0000 0057  .......4...'...W
+00008500: 0700 0026 0000 00ff ffff ff00 0000 005b  ...&...........[
+00008510: 1800 0022 0000 007d 0700 0021 0000 00ff  ..."...}...!....
+00008520: ffff ff00 0000 007d 1800 0027 0000 009e  .......}...'....
+00008530: 0700 0026 0000 00ff ffff ff00 0000 00a4  ...&............
+00008540: 1800 0022 0000 00c4 0700 0021 0000 00ff  ...".......!....
+00008550: ffff ff00 0000 00c6 1800 0027 0000 00e5  ...........'....
+00008560: 0700 0026 0000 00ff ffff ff00 0000 00ed  ...&............
+00008570: 1800 0022 0000 000b 0800 0021 0000 00ff  ...".......!....
+00008580: ffff ff00 0000 000f 1900 0027 0000 002c  ...........'...,
+00008590: 0800 0026 0000 00ff ffff ff00 0000 0008  ...&............
+000085a0: 0000 0000 0000 0097 0000 0000 0000 0097  ................
+000085b0: 0000 0000 0000 0008 0000 0000 0000 0097  ................
+000085c0: 0000 0000 0000 0097 0000 0000 0000 0008  ................
+000085d0: 0000 0000 0000 0097 0000 0000 0000 0097  ................
+000085e0: 0000 0000 0000 0008 0000 0000 0000 0097  ................
+000085f0: 0000 0000 0000 0097 0000 0000 0000 0008  ................
+00008600: 0000 0000 0000 0097 0000 0000 0000 0097  ................
+00008610: 0000 0000 0000 0008 0000 0000 0000 0097  ................
+00008620: 0000 0000 0000 0097 0000 0000 0000 0008  ................
+00008630: 0000 0000 0000 0097 0000 0000 0000 0097  ................
+00008640: 0000 0000 0000 0000 0000 005d 0c00 0051  ...........]...Q
+00008650: 0600 0012 0394 766a 0000 005f 5a4e 3038  ......vj..._ZN08
+00008660: 4e75 6d62 6145 6e76 3573 696d 6261 366d  NumbaEnv5simba6m
+00008670: 6978 696e 7332 3466 6561 7475 7265 5f65  ixins24feature_e
+00008680: 7874 7261 6374 696f 6e5f 6d69 7869 6e32  xtraction_mixin2
+00008690: 3246 6561 7475 7265 4578 7472 6163 7469  2FeatureExtracti
+000086a0: 6f6e 4d69 7869 6e31 3063 6469 7374 2432  onMixin10cdist$2
+000086b0: 3436 3045 3541 7272 6179 4966 4c69 3245  460E5ArrayIfLi2E
+000086c0: 3141 376d 7574 6162 6c65 3761 6c69 676e  1A7mutable7align
+000086d0: 6564 4535 4172 7261 7949 664c 6932 4531  edE5ArrayIfLi2E1
+000086e0: 4137 6d75 7461 626c 6537 616c 6967 6e65  A7mutable7aligne
+000086f0: 6445 2e63 6f6e 7374 2e70 6963 6b6c 6562  dE.const.pickleb
+00008700: 7566 2e31 3430 3237 3938 3738 3330 3532  uf.1402798783052
+00008710: 3536 2e63 6f6e 7374 2e70 6963 6b6c 6562  56.const.pickleb
+00008720: 7566 2e31 3430 3237 3938 3738 3330 3433  uf.1402798783043
+00008730: 3230 2e63 6f6e 7374 2e70 6963 6b6c 6564  20.const.pickled
+00008740: 6174 612e 3134 3032 3739 3837 3833 3034  ata.140279878304
+00008750: 3332 302e 636f 6e73 742e 7069 636b 6c65  320.const.pickle
+00008760: 6461 7461 2e31 3430 3237 3938 3738 3330  data.14027987830
+00008770: 3433 3230 2e73 6861 312e 636f 6e73 742e  4320.sha1.const.
+00008780: 7069 636b 6c65 6461 7461 2e31 3430 3237  pickledata.14027
+00008790: 3938 3738 3330 3532 3536 2e63 6f6e 7374  9878305256.const
+000087a0: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+000087b0: 3739 3837 3833 3035 3235 362e 7368 6131  79878305256.sha1
+000087c0: 2e63 6f6e 7374 2e46 6561 7475 7265 4578  .const.FeatureEx
+000087d0: 7472 6163 7469 6f6e 4d69 7869 6e2e 6364  tractionMixin.cd
+000087e0: 6973 7450 7945 7863 5f52 756e 7469 6d65  istPyExc_Runtime
+000087f0: 4572 726f 722e 636f 6e73 742e 6d69 7373  Error.const.miss
+00008800: 696e 6720 456e 7669 726f 6e6d 656e 743a  ing Environment:
+00008810: 205f 5a4e 3038 4e75 6d62 6145 6e76 3573   _ZN08NumbaEnv5s
+00008820: 696d 6261 366d 6978 696e 7332 3466 6561  imba6mixins24fea
+00008830: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
+00008840: 6d69 7869 6e32 3246 6561 7475 7265 4578  mixin22FeatureEx
+00008850: 7472 6163 7469 6f6e 4d69 7869 6e31 3063  tractionMixin10c
+00008860: 6469 7374 2432 3436 3045 3541 7272 6179  dist$2460E5Array
+00008870: 4966 4c69 3245 3141 376d 7574 6162 6c65  IfLi2E1A7mutable
+00008880: 3761 6c69 676e 6564 4535 4172 7261 7949  7alignedE5ArrayI
+00008890: 664c 6932 4531 4137 6d75 7461 626c 6537  fLi2E1A7mutable7
+000088a0: 616c 6967 6e65 6445 5079 4578 635f 5479  alignedEPyExc_Ty
+000088b0: 7065 4572 726f 722e 636f 6e73 742e 6361  peError.const.ca
+000088c0: 6e27 7420 756e 626f 7820 6172 7261 7920  n't unbox array 
+000088d0: 6672 6f6d 2050 794f 626a 6563 7420 696e  from PyObject in
+000088e0: 746f 206e 6174 6976 6520 7661 6c75 652e  to native value.
+000088f0: 2020 5468 6520 6f62 6a65 6374 206d 6179    The object may
+00008900: 6265 206f 6620 6120 6469 6666 6572 656e  be of a differen
+00008910: 7420 7479 7065 5f50 795f 4e6f 6e65 5374  t type_Py_NoneSt
+00008920: 7275 6374 2e63 6f6e 7374 2e60 656e 762e  ruct.const.`env.
+00008930: 636f 6e73 7473 6020 6973 204e 554c 4c20  consts` is NULL 
+00008940: 696e 2060 7265 6164 5f63 6f6e 7374 6050  in `read_const`P
+00008950: 7945 7863 5f53 746f 7049 7465 7261 7469  yExc_StopIterati
+00008960: 6f6e 5079 4578 635f 5379 7374 656d 4572  onPyExc_SystemEr
+00008970: 726f 722e 636f 6e73 742e 756e 6b6e 6f77  ror.const.unknow
+00008980: 6e20 6572 726f 7220 7768 656e 2063 616c  n error when cal
+00008990: 6c69 6e67 206e 6174 6976 6520 6675 6e63  ling native func
+000089a0: 7469 6f6e 2e63 6f6e 7374 2e3c 6e75 6d62  tion.const.<numb
+000089b0: 612e 636f 7265 2e63 7075 2e43 5055 436f  a.core.cpu.CPUCo
+000089c0: 6e74 6578 7420 6f62 6a65 6374 2061 7420  ntext object at 
+000089d0: 3078 3766 3935 3535 3530 3639 3430 3e2e  0x7f9555506940>.
+000089e0: 636f 6e73 742e 756e 6b6e 6f77 6e20 6572  const.unknown er
+000089f0: 726f 7220 7768 656e 2063 616c 6c69 6e67  ror when calling
+00008a00: 206e 6174 6976 6520 6675 6e63 7469 6f6e   native function
+00008a10: 2e31 5f5a 4e30 384e 756d 6261 456e 7635  .1_ZN08NumbaEnv5
+00008a20: 6e75 6d62 6132 6e70 3861 7272 6179 6f62  numba2np8arrayob
+00008a30: 6a31 336e 756d 7079 5f66 756c 6c5f 6e64  j13numpy_full_nd
+00008a40: 3132 2433 636c 6f63 616c 7324 3365 3966  12$3clocals$3e9f
+00008a50: 756c 6c24 3234 3633 4538 556e 6954 7570  ull$2463E8UniTup
+00008a60: 6c65 4978 4c69 3245 4564 2e63 6f6e 7374  leIxLi2EEd.const
+00008a70: 2e70 6963 6b6c 6562 7566 2e31 3430 3237  .picklebuf.14027
+00008a80: 3938 3736 3835 3339 3034 2e63 6f6e 7374  9876853904.const
+00008a90: 2e70 6963 6b6c 6562 7566 2e31 3430 3237  .picklebuf.14027
+00008aa0: 3938 3639 3838 3836 3936 2e63 6f6e 7374  9869888696.const
+00008ab0: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00008ac0: 3739 3836 3938 3838 3639 362e 636f 6e73  79869888696.cons
+00008ad0: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
+00008ae0: 3237 3938 3639 3838 3836 3936 2e73 6861  279869888696.sha
+00008af0: 312e 636f 6e73 742e 7069 636b 6c65 6461  1.const.pickleda
+00008b00: 7461 2e31 3430 3237 3938 3736 3835 3339  ta.1402798768539
+00008b10: 3034 2e63 6f6e 7374 2e70 6963 6b6c 6564  04.const.pickled
+00008b20: 6174 612e 3134 3032 3739 3837 3638 3533  ata.140279876853
+00008b30: 3930 342e 7368 6131 5f5a 4e30 384e 756d  904.sha1_ZN08Num
+00008b40: 6261 456e 7631 3324 3363 6479 6e61 6d69  baEnv13$3cdynami
+00008b50: 6324 3365 3338 5f5f 6e75 6d62 615f 6172  c$3e38__numba_ar
+00008b60: 7261 795f 6578 7072 5f30 7837 6639 3535  ray_expr_0x7f955
+00008b70: 3535 3039 6531 3024 3234 3634 4566 665f  5509e10$2464Eff_
+00008b80: 5a4e 3038 4e75 6d62 6145 6e76 356e 756d  ZN08NumbaEnv5num
+00008b90: 6261 326e 7037 6e70 7969 6d70 6c32 305f  ba2np7npyimpl20_
+00008ba0: 6272 6f61 6463 6173 745f 6f6e 746f 2432  broadcast_onto$2
+00008bb0: 3431 3045 7838 696e 7436 3424 3261 7838  410Ex8int64$2ax8
+00008bc0: 696e 7436 3424 3261 5f5a 4e30 384e 756d  int64$2a_ZN08Num
+00008bd0: 6261 456e 7635 6e75 6d62 6132 6e70 366c  baEnv5numba2np6l
+00008be0: 696e 616c 6731 345f 6765 745f 6e6f 726d  inalg14_get_norm
+00008bf0: 5f69 6d70 6c31 3224 3363 6c6f 6361 6c73  _impl12$3clocals
+00008c00: 2433 6531 346f 6e65 445f 696d 706c 2432  $3e14oneD_impl$2
+00008c10: 3436 3145 3541 7272 6179 4966 4c69 3145  461E5ArrayIfLi1E
+00008c20: 3143 376d 7574 6162 6c65 3761 6c69 676e  1C7mutable7align
+00008c30: 6564 4532 376f 6d69 7474 6564 2432 3864  edE27omitted$28d
+00008c40: 6566 6175 6c74 2433 644e 6f6e 6524 3239  efault$3dNone$29
+00008c50: 5f5a 4e30 384e 756d 6261 456e 7635 6e75  _ZN08NumbaEnv5nu
+00008c60: 6d62 6132 6e70 366c 696e 616c 6731 375f  mba2np6linalg17_
+00008c70: 6f6e 6544 5f6e 6f72 6d5f 325f 696d 706c  oneD_norm_2_impl
+00008c80: 3132 2433 636c 6f63 616c 7324 3365 3969  12$3clocals$3e9i
+00008c90: 6d70 6c24 3234 3632 4535 4172 7261 7949  mpl$2462E5ArrayI
+00008ca0: 664c 6931 4531 4337 6d75 7461 626c 6537  fLi1E1C7mutable7
+00008cb0: 616c 6967 6e65 6445 5f5a 4e30 384e 756d  alignedE_ZN08Num
+00008cc0: 6261 456e 7635 6e75 6d62 6132 6e70 366c  baEnv5numba2np6l
+00008cd0: 696e 616c 6732 355f 6475 6d6d 795f 6c69  inalg25_dummy_li
+00008ce0: 7665 6e65 7373 5f66 756e 6324 3234 3239  veness_func$2429
+00008cf0: 4533 306c 6973 7424 3238 696e 7436 3424  E30list$28int64$
+00008d00: 3239 2433 6369 7624 3364 4e6f 6e65 2433  29$3civ$3dNone$3
+00008d10: 652e 636f 6e73 742e 7069 636b 6c65 6275  e.const.picklebu
+00008d20: 662e 3134 3032 3739 3837 3332 3730 3139  f.14027987327019
+00008d30: 322e 636f 6e73 742e 7069 636b 6c65 6275  2.const.picklebu
+00008d40: 662e 3134 3032 3739 3837 3638 3534 3931  f.14027987685491
+00008d50: 322e 636f 6e73 742e 7069 636b 6c65 6275  2.const.picklebu
+00008d60: 662e 3134 3032 3739 3837 3638 3534 3834  f.14027987685484
+00008d70: 302e 636f 6e73 742e 7069 636b 6c65 6275  0.const.picklebu
+00008d80: 662e 3134 3032 3739 3839 3031 3038 3438  f.14027989010848
+00008d90: 382e 636f 6e73 742e 7069 636b 6c65 6461  8.const.pickleda
+00008da0: 7461 2e31 3430 3237 3938 3930 3130 3834  ta.1402798901084
+00008db0: 3838 2e63 6f6e 7374 2e70 6963 6b6c 6564  88.const.pickled
+00008dc0: 6174 612e 3134 3032 3739 3839 3031 3038  ata.140279890108
+00008dd0: 3438 382e 7368 6131 2e63 6f6e 7374 2e70  488.sha1.const.p
+00008de0: 6963 6b6c 6564 6174 612e 3134 3032 3739  ickledata.140279
+00008df0: 3837 3638 3534 3834 302e 636f 6e73 742e  876854840.const.
+00008e00: 7069 636b 6c65 6461 7461 2e31 3430 3237  pickledata.14027
+00008e10: 3938 3736 3835 3438 3430 2e73 6861 312e  9876854840.sha1.
+00008e20: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
+00008e30: 2e31 3430 3237 3938 3736 3835 3439 3132  .140279876854912
+00008e40: 2e63 6f6e 7374 2e70 6963 6b6c 6564 6174  .const.pickledat
+00008e50: 612e 3134 3032 3739 3837 3638 3534 3931  a.14027987685491
+00008e60: 322e 7368 6131 2e63 6f6e 7374 2e70 6963  2.sha1.const.pic
+00008e70: 6b6c 6564 6174 612e 3134 3032 3739 3837  kledata.14027987
+00008e80: 3332 3730 3139 322e 636f 6e73 742e 7069  3270192.const.pi
+00008e90: 636b 6c65 6461 7461 2e31 3430 3237 3938  ckledata.1402798
+00008ea0: 3733 3237 3031 3932 2e73 6861 315f 5a4e  73270192.sha1_ZN
+00008eb0: 3573 696d 6261 366d 6978 696e 7332 3466  5simba6mixins24f
+00008ec0: 6561 7475 7265 5f65 7874 7261 6374 696f  eature_extractio
+00008ed0: 6e5f 6d69 7869 6e32 3246 6561 7475 7265  n_mixin22Feature
+00008ee0: 4578 7472 6163 7469 6f6e 4d69 7869 6e31  ExtractionMixin1
+00008ef0: 3063 6469 7374 2432 3436 3045 3541 7272  0cdist$2460E5Arr
+00008f00: 6179 4966 4c69 3245 3141 376d 7574 6162  ayIfLi2E1A7mutab
+00008f10: 6c65 3761 6c69 676e 6564 4535 4172 7261  le7alignedE5Arra
+00008f20: 7949 664c 6932 4531 4137 6d75 7461 626c  yIfLi2E1A7mutabl
+00008f30: 6537 616c 6967 6e65 6445 6c6c 766d 2e73  e7alignedEllvm.s
+00008f40: 6d75 6c2e 7769 7468 2e6f 7665 7266 6c6f  mul.with.overflo
+00008f50: 772e 6936 344e 5254 5f4d 656d 496e 666f  w.i64NRT_MemInfo
+00008f60: 5f61 6c6c 6f63 5f73 6166 655f 616c 6967  _alloc_safe_alig
+00008f70: 6e65 645f 5a4e 3763 7079 7468 6f6e 3573  ned_ZN7cpython5s
+00008f80: 696d 6261 366d 6978 696e 7332 3466 6561  imba6mixins24fea
+00008f90: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
+00008fa0: 6d69 7869 6e32 3246 6561 7475 7265 4578  mixin22FeatureEx
+00008fb0: 7472 6163 7469 6f6e 4d69 7869 6e31 3063  tractionMixin10c
+00008fc0: 6469 7374 2432 3436 3045 3541 7272 6179  dist$2460E5Array
+00008fd0: 4966 4c69 3245 3141 376d 7574 6162 6c65  IfLi2E1A7mutable
+00008fe0: 3761 6c69 676e 6564 4535 4172 7261 7949  7alignedE5ArrayI
+00008ff0: 664c 6932 4531 4137 6d75 7461 626c 6537  fLi2E1A7mutable7
+00009000: 616c 6967 6e65 6445 5079 4172 675f 556e  alignedEPyArg_Un
+00009010: 7061 636b 5475 706c 6550 7945 7272 5f53  packTuplePyErr_S
+00009020: 6574 5374 7269 6e67 4e52 545f 6164 6170  etStringNRT_adap
+00009030: 745f 6e64 6172 7261 795f 6672 6f6d 5f70  t_ndarray_from_p
+00009040: 7974 686f 6e50 795f 496e 6352 6566 5079  ythonPy_IncRefPy
+00009050: 4c69 7374 5f47 6574 4974 656d 4e52 545f  List_GetItemNRT_
+00009060: 6164 6170 745f 6e64 6172 7261 795f 746f  adapt_ndarray_to
+00009070: 5f70 7974 686f 6e5f 6163 7172 6566 5079  _python_acqrefPy
+00009080: 4572 725f 436c 6561 726e 756d 6261 5f75  Err_Clearnumba_u
+00009090: 6e70 6963 6b6c 656e 756d 6261 5f64 6f5f  npicklenumba_do_
+000090a0: 7261 6973 6550 7945 7272 5f53 6574 4e6f  raisePyErr_SetNo
+000090b0: 6e65 6366 756e 632e 5f5a 4e35 7369 6d62  necfunc._ZN5simb
+000090c0: 6136 6d69 7869 6e73 3234 6665 6174 7572  a6mixins24featur
+000090d0: 655f 6578 7472 6163 7469 6f6e 5f6d 6978  e_extraction_mix
+000090e0: 696e 3232 4665 6174 7572 6545 7874 7261  in22FeatureExtra
+000090f0: 6374 696f 6e4d 6978 696e 3130 6364 6973  ctionMixin10cdis
+00009100: 7424 3234 3630 4535 4172 7261 7949 664c  t$2460E5ArrayIfL
+00009110: 6932 4531 4137 6d75 7461 626c 6537 616c  i2E1A7mutable7al
+00009120: 6967 6e65 6445 3541 7272 6179 4966 4c69  ignedE5ArrayIfLi
+00009130: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
+00009140: 676e 6564 456e 756d 6261 5f67 696c 5f65  gnedEnumba_gil_e
+00009150: 6e73 7572 6550 7955 6e69 636f 6465 5f46  nsurePyUnicode_F
+00009160: 726f 6d53 7472 696e 6750 7945 7272 5f57  romStringPyErr_W
+00009170: 7269 7465 556e 7261 6973 6162 6c65 5079  riteUnraisablePy
+00009180: 5f44 6563 5265 666e 756d 6261 5f67 696c  _DecRefnumba_gil
+00009190: 5f72 656c 6561 7365 5f5a 4e35 6e75 6d62  _release_ZN5numb
+000091a0: 6132 6e70 366c 696e 616c 6731 375f 6f6e  a2np6linalg17_on
+000091b0: 6544 5f6e 6f72 6d5f 325f 696d 706c 3132  eD_norm_2_impl12
+000091c0: 2433 636c 6f63 616c 7324 3365 3969 6d70  $3clocals$3e9imp
+000091d0: 6c24 3234 3632 4535 4172 7261 7949 664c  l$2462E5ArrayIfL
+000091e0: 6931 4531 4337 6d75 7461 626c 6537 616c  i1E1C7mutable7al
+000091f0: 6967 6e65 6445 4e52 545f 6465 6372 6566  ignedENRT_decref
+00009200: 6e75 6d62 615f 6661 7461 6c5f 6572 726f  numba_fatal_erro
+00009210: 726e 756d 6261 5f78 786e 726d 322e 6474  rnumba_xxnrm2.dt
+00009220: 6f72 2e6c 6973 742e 696e 7436 344e 5254  or.list.int64NRT
+00009230: 5f4d 656d 496e 666f 5f6e 6577 5f76 6172  _MemInfo_new_var
+00009240: 7369 7a65 5f64 746f 726c 6c76 6d2e 6d65  size_dtorllvm.me
+00009250: 6d73 6574 2e70 3069 382e 6936 344e 5254  mset.p0i8.i64NRT
+00009260: 5f4d 656d 496e 666f 5f63 616c 6c5f 6474  _MemInfo_call_dt
+00009270: 6f72 4e52 545f 696e 6372 6566 6c6c 766d  orNRT_increfllvm
+00009280: 2e6c 6966 6574 696d 652e 7374 6172 742e  .lifetime.start.
+00009290: 7030 6938 6c6c 766d 2e6c 6966 6574 696d  p0i8llvm.lifetim
+000092a0: 652e 656e 642e 7030 6938 6c6c 766d 2e73  e.end.p0i8llvm.s
+000092b0: 7461 636b 7072 6f74 6563 746f 7231 302e  tackprotector10.
+000092c0: 302e 3178 3836 5f36 342d 6170 706c 652d  0.1x86_64-apple-
+000092d0: 6461 7277 696e 3139 2e36 2e30 3c73 7472  darwin19.6.0<str
+000092e0: 696e 673e 5f5f 5a4e 3573 696d 6261 366d  ing>__ZN5simba6m
+000092f0: 6978 696e 7332 3466 6561 7475 7265 5f65  ixins24feature_e
+00009300: 7874 7261 6374 696f 6e5f 6d69 7869 6e32  xtraction_mixin2
+00009310: 3246 6561 7475 7265 4578 7472 6163 7469  2FeatureExtracti
+00009320: 6f6e 4d69 7869 6e31 3063 6469 7374 2432  onMixin10cdist$2
+00009330: 3436 3045 3541 7272 6179 4966 4c69 3245  460E5ArrayIfLi2E
+00009340: 3141 376d 7574 6162 6c65 3761 6c69 676e  1A7mutable7align
+00009350: 6564 4535 4172 7261 7949 664c 6932 4531  edE5ArrayIfLi2E1
+00009360: 4137 6d75 7461 626c 6537 616c 6967 6e65  A7mutable7aligne
+00009370: 6445 5f6c 6c76 6d2e 736d 756c 2e77 6974  dE_llvm.smul.wit
+00009380: 682e 6f76 6572 666c 6f77 2e69 3634 5f4e  h.overflow.i64_N
+00009390: 5254 5f4d 656d 496e 666f 5f61 6c6c 6f63  RT_MemInfo_alloc
+000093a0: 5f73 6166 655f 616c 6967 6e65 645f 5f5a  _safe_aligned__Z
+000093b0: 4e37 6370 7974 686f 6e35 7369 6d62 6136  N7cpython5simba6
+000093c0: 6d69 7869 6e73 3234 6665 6174 7572 655f  mixins24feature_
+000093d0: 6578 7472 6163 7469 6f6e 5f6d 6978 696e  extraction_mixin
+000093e0: 3232 4665 6174 7572 6545 7874 7261 6374  22FeatureExtract
+000093f0: 696f 6e4d 6978 696e 3130 6364 6973 7424  ionMixin10cdist$
+00009400: 3234 3630 4535 4172 7261 7949 664c 6932  2460E5ArrayIfLi2
+00009410: 4531 4137 6d75 7461 626c 6537 616c 6967  E1A7mutable7alig
+00009420: 6e65 6445 3541 7272 6179 4966 4c69 3245  nedE5ArrayIfLi2E
+00009430: 3141 376d 7574 6162 6c65 3761 6c69 676e  1A7mutable7align
+00009440: 6564 455f 5079 4172 675f 556e 7061 636b  edE_PyArg_Unpack
+00009450: 5475 706c 655f 5079 4572 725f 5365 7453  Tuple_PyErr_SetS
+00009460: 7472 696e 675f 4e52 545f 6164 6170 745f  tring_NRT_adapt_
+00009470: 6e64 6172 7261 795f 6672 6f6d 5f70 7974  ndarray_from_pyt
+00009480: 686f 6e5f 5079 5f49 6e63 5265 665f 5079  hon_Py_IncRef_Py
+00009490: 4c69 7374 5f47 6574 4974 656d 5f4e 5254  List_GetItem_NRT
+000094a0: 5f61 6461 7074 5f6e 6461 7272 6179 5f74  _adapt_ndarray_t
+000094b0: 6f5f 7079 7468 6f6e 5f61 6371 7265 665f  o_python_acqref_
+000094c0: 5079 4572 725f 436c 6561 725f 6e75 6d62  PyErr_Clear_numb
+000094d0: 615f 756e 7069 636b 6c65 5f6e 756d 6261  a_unpickle_numba
+000094e0: 5f64 6f5f 7261 6973 655f 5079 4572 725f  _do_raise_PyErr_
+000094f0: 5365 744e 6f6e 655f 6366 756e 632e 5f5a  SetNone_cfunc._Z
+00009500: 4e35 7369 6d62 6136 6d69 7869 6e73 3234  N5simba6mixins24
+00009510: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
+00009520: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
+00009530: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
+00009540: 3130 6364 6973 7424 3234 3630 4535 4172  10cdist$2460E5Ar
+00009550: 7261 7949 664c 6932 4531 4137 6d75 7461  rayIfLi2E1A7muta
+00009560: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
+00009570: 6179 4966 4c69 3245 3141 376d 7574 6162  ayIfLi2E1A7mutab
+00009580: 6c65 3761 6c69 676e 6564 455f 6e75 6d62  le7alignedE_numb
+00009590: 615f 6769 6c5f 656e 7375 7265 5f50 7955  a_gil_ensure_PyU
+000095a0: 6e69 636f 6465 5f46 726f 6d53 7472 696e  nicode_FromStrin
+000095b0: 675f 5079 4572 725f 5772 6974 6555 6e72  g_PyErr_WriteUnr
+000095c0: 6169 7361 626c 655f 5079 5f44 6563 5265  aisable_Py_DecRe
+000095d0: 665f 6e75 6d62 615f 6769 6c5f 7265 6c65  f_numba_gil_rele
+000095e0: 6173 655f 5f5a 4e35 6e75 6d62 6132 6e70  ase__ZN5numba2np
+000095f0: 366c 696e 616c 6731 375f 6f6e 6544 5f6e  6linalg17_oneD_n
+00009600: 6f72 6d5f 325f 696d 706c 3132 2433 636c  orm_2_impl12$3cl
+00009610: 6f63 616c 7324 3365 3969 6d70 6c24 3234  ocals$3e9impl$24
+00009620: 3632 4535 4172 7261 7949 664c 6931 4531  62E5ArrayIfLi1E1
+00009630: 4337 6d75 7461 626c 6537 616c 6967 6e65  C7mutable7aligne
+00009640: 6445 5f4e 5254 5f64 6563 7265 665f 6e75  dE_NRT_decref_nu
+00009650: 6d62 615f 6661 7461 6c5f 6572 726f 725f  mba_fatal_error_
+00009660: 6e75 6d62 615f 7878 6e72 6d32 5f2e 6474  numba_xxnrm2_.dt
+00009670: 6f72 2e6c 6973 742e 696e 7436 345f 4e52  or.list.int64_NR
+00009680: 545f 4d65 6d49 6e66 6f5f 6e65 775f 7661  T_MemInfo_new_va
+00009690: 7273 697a 655f 6474 6f72 5f6c 6c76 6d2e  rsize_dtor_llvm.
+000096a0: 6d65 6d73 6574 2e70 3069 382e 6936 345f  memset.p0i8.i64_
+000096b0: 4e52 545f 4d65 6d49 6e66 6f5f 6361 6c6c  NRT_MemInfo_call
+000096c0: 5f64 746f 725f 4e52 545f 696e 6372 6566  _dtor_NRT_incref
+000096d0: 5f6c 6c76 6d2e 6c69 6665 7469 6d65 2e73  _llvm.lifetime.s
+000096e0: 7461 7274 2e70 3069 385f 6c6c 766d 2e6c  tart.p0i8_llvm.l
+000096f0: 6966 6574 696d 652e 656e 642e 7030 6938  ifetime.end.p0i8
+00009700: 5f6c 6c76 6d2e 7374 6163 6b70 726f 7465  _llvm.stackprote
+00009710: 6374 6f72 5f5f 5a4e 3038 4e75 6d62 6145  ctor__ZN08NumbaE
+00009720: 6e76 3573 696d 6261 366d 6978 696e 7332  nv5simba6mixins2
+00009730: 3466 6561 7475 7265 5f65 7874 7261 6374  4feature_extract
+00009740: 696f 6e5f 6d69 7869 6e32 3246 6561 7475  ion_mixin22Featu
+00009750: 7265 4578 7472 6163 7469 6f6e 4d69 7869  reExtractionMixi
+00009760: 6e31 3063 6469 7374 2432 3436 3045 3541  n10cdist$2460E5A
+00009770: 7272 6179 4966 4c69 3245 3141 376d 7574  rrayIfLi2E1A7mut
+00009780: 6162 6c65 3761 6c69 676e 6564 4535 4172  able7alignedE5Ar
+00009790: 7261 7949 664c 6932 4531 4137 6d75 7461  rayIfLi2E1A7muta
+000097a0: 626c 6537 616c 6967 6e65 6445 5f2e 636f  ble7alignedE_.co
+000097b0: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
+000097c0: 3032 3739 3837 3833 3035 3235 365f 2e63  0279878305256_.c
+000097d0: 6f6e 7374 2e70 6963 6b6c 6562 7566 2e31  onst.picklebuf.1
+000097e0: 3430 3237 3938 3738 3330 3433 3230 5f2e  40279878304320_.
+000097f0: 636f 6e73 742e 7069 636b 6c65 6461 7461  const.pickledata
+00009800: 2e31 3430 3237 3938 3738 3330 3433 3230  .140279878304320
+00009810: 5f2e 636f 6e73 742e 7069 636b 6c65 6461  _.const.pickleda
+00009820: 7461 2e31 3430 3237 3938 3738 3330 3433  ta.1402798783043
+00009830: 3230 2e73 6861 315f 2e63 6f6e 7374 2e70  20.sha1_.const.p
+00009840: 6963 6b6c 6564 6174 612e 3134 3032 3739  ickledata.140279
+00009850: 3837 3833 3035 3235 365f 2e63 6f6e 7374  878305256_.const
+00009860: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00009870: 3739 3837 3833 3035 3235 362e 7368 6131  79878305256.sha1
+00009880: 5f2e 636f 6e73 742e 4665 6174 7572 6545  _.const.FeatureE
+00009890: 7874 7261 6374 696f 6e4d 6978 696e 2e63  xtractionMixin.c
+000098a0: 6469 7374 5f50 7945 7863 5f52 756e 7469  dist_PyExc_Runti
+000098b0: 6d65 4572 726f 725f 2e63 6f6e 7374 2e6d  meError_.const.m
+000098c0: 6973 7369 6e67 2045 6e76 6972 6f6e 6d65  issing Environme
+000098d0: 6e74 3a20 5f5a 4e30 384e 756d 6261 456e  nt: _ZN08NumbaEn
+000098e0: 7635 7369 6d62 6136 6d69 7869 6e73 3234  v5simba6mixins24
+000098f0: 6665 6174 7572 655f 6578 7472 6163 7469  feature_extracti
+00009900: 6f6e 5f6d 6978 696e 3232 4665 6174 7572  on_mixin22Featur
+00009910: 6545 7874 7261 6374 696f 6e4d 6978 696e  eExtractionMixin
+00009920: 3130 6364 6973 7424 3234 3630 4535 4172  10cdist$2460E5Ar
+00009930: 7261 7949 664c 6932 4531 4137 6d75 7461  rayIfLi2E1A7muta
+00009940: 626c 6537 616c 6967 6e65 6445 3541 7272  ble7alignedE5Arr
+00009950: 6179 4966 4c69 3245 3141 376d 7574 6162  ayIfLi2E1A7mutab
+00009960: 6c65 3761 6c69 676e 6564 455f 5079 4578  le7alignedE_PyEx
+00009970: 635f 5479 7065 4572 726f 725f 2e63 6f6e  c_TypeError_.con
+00009980: 7374 2e63 616e 2774 2075 6e62 6f78 2061  st.can't unbox a
+00009990: 7272 6179 2066 726f 6d20 5079 4f62 6a65  rray from PyObje
+000099a0: 6374 2069 6e74 6f20 6e61 7469 7665 2076  ct into native v
+000099b0: 616c 7565 2e20 2054 6865 206f 626a 6563  alue.  The objec
+000099c0: 7420 6d61 7962 6520 6f66 2061 2064 6966  t maybe of a dif
+000099d0: 6665 7265 6e74 2074 7970 655f 5f50 795f  ferent type__Py_
+000099e0: 4e6f 6e65 5374 7275 6374 5f2e 636f 6e73  NoneStruct_.cons
+000099f0: 742e 6065 6e76 2e63 6f6e 7374 7360 2069  t.`env.consts` i
+00009a00: 7320 4e55 4c4c 2069 6e20 6072 6561 645f  s NULL in `read_
+00009a10: 636f 6e73 7460 5f50 7945 7863 5f53 746f  const`_PyExc_Sto
+00009a20: 7049 7465 7261 7469 6f6e 5f50 7945 7863  pIteration_PyExc
+00009a30: 5f53 7973 7465 6d45 7272 6f72 5f2e 636f  _SystemError_.co
+00009a40: 6e73 742e 756e 6b6e 6f77 6e20 6572 726f  nst.unknown erro
+00009a50: 7220 7768 656e 2063 616c 6c69 6e67 206e  r when calling n
+00009a60: 6174 6976 6520 6675 6e63 7469 6f6e 5f2e  ative function_.
+00009a70: 636f 6e73 742e 3c6e 756d 6261 2e63 6f72  const.<numba.cor
+00009a80: 652e 6370 752e 4350 5543 6f6e 7465 7874  e.cpu.CPUContext
+00009a90: 206f 626a 6563 7420 6174 2030 7837 6639   object at 0x7f9
+00009aa0: 3535 3535 3036 3934 303e 5f2e 636f 6e73  555506940>_.cons
+00009ab0: 742e 756e 6b6e 6f77 6e20 6572 726f 7220  t.unknown error 
+00009ac0: 7768 656e 2063 616c 6c69 6e67 206e 6174  when calling nat
+00009ad0: 6976 6520 6675 6e63 7469 6f6e 2e31 5f5f  ive function.1__
+00009ae0: 5a4e 3038 4e75 6d62 6145 6e76 356e 756d  ZN08NumbaEnv5num
+00009af0: 6261 326e 7038 6172 7261 796f 626a 3133  ba2np8arrayobj13
+00009b00: 6e75 6d70 795f 6675 6c6c 5f6e 6431 3224  numpy_full_nd12$
+00009b10: 3363 6c6f 6361 6c73 2433 6539 6675 6c6c  3clocals$3e9full
+00009b20: 2432 3436 3345 3855 6e69 5475 706c 6549  $2463E8UniTupleI
+00009b30: 784c 6932 4545 645f 2e63 6f6e 7374 2e70  xLi2EEd_.const.p
+00009b40: 6963 6b6c 6562 7566 2e31 3430 3237 3938  icklebuf.1402798
+00009b50: 3736 3835 3339 3034 5f2e 636f 6e73 742e  76853904_.const.
+00009b60: 7069 636b 6c65 6275 662e 3134 3032 3739  picklebuf.140279
+00009b70: 3836 3938 3838 3639 365f 2e63 6f6e 7374  869888696_.const
+00009b80: 2e70 6963 6b6c 6564 6174 612e 3134 3032  .pickledata.1402
+00009b90: 3739 3836 3938 3838 3639 365f 2e63 6f6e  79869888696_.con
+00009ba0: 7374 2e70 6963 6b6c 6564 6174 612e 3134  st.pickledata.14
+00009bb0: 3032 3739 3836 3938 3838 3639 362e 7368  0279869888696.sh
+00009bc0: 6131 5f2e 636f 6e73 742e 7069 636b 6c65  a1_.const.pickle
+00009bd0: 6461 7461 2e31 3430 3237 3938 3736 3835  data.14027987685
+00009be0: 3339 3034 5f2e 636f 6e73 742e 7069 636b  3904_.const.pick
+00009bf0: 6c65 6461 7461 2e31 3430 3237 3938 3736  ledata.140279876
+00009c00: 3835 3339 3034 2e73 6861 315f 5f5a 4e30  853904.sha1__ZN0
+00009c10: 384e 756d 6261 456e 7631 3324 3363 6479  8NumbaEnv13$3cdy
+00009c20: 6e61 6d69 6324 3365 3338 5f5f 6e75 6d62  namic$3e38__numb
+00009c30: 615f 6172 7261 795f 6578 7072 5f30 7837  a_array_expr_0x7
+00009c40: 6639 3535 3535 3039 6531 3024 3234 3634  f9555509e10$2464
+00009c50: 4566 665f 5f5a 4e30 384e 756d 6261 456e  Eff__ZN08NumbaEn
+00009c60: 7635 6e75 6d62 6132 6e70 376e 7079 696d  v5numba2np7npyim
+00009c70: 706c 3230 5f62 726f 6164 6361 7374 5f6f  pl20_broadcast_o
+00009c80: 6e74 6f24 3234 3130 4578 3869 6e74 3634  nto$2410Ex8int64
+00009c90: 2432 6178 3869 6e74 3634 2432 615f 5f5a  $2ax8int64$2a__Z
+00009ca0: 4e30 384e 756d 6261 456e 7635 6e75 6d62  N08NumbaEnv5numb
+00009cb0: 6132 6e70 366c 696e 616c 6731 345f 6765  a2np6linalg14_ge
+00009cc0: 745f 6e6f 726d 5f69 6d70 6c31 3224 3363  t_norm_impl12$3c
+00009cd0: 6c6f 6361 6c73 2433 6531 346f 6e65 445f  locals$3e14oneD_
+00009ce0: 696d 706c 2432 3436 3145 3541 7272 6179  impl$2461E5Array
+00009cf0: 4966 4c69 3145 3143 376d 7574 6162 6c65  IfLi1E1C7mutable
+00009d00: 3761 6c69 676e 6564 4532 376f 6d69 7474  7alignedE27omitt
+00009d10: 6564 2432 3864 6566 6175 6c74 2433 644e  ed$28default$3dN
+00009d20: 6f6e 6524 3239 5f5f 5a4e 3038 4e75 6d62  one$29__ZN08Numb
+00009d30: 6145 6e76 356e 756d 6261 326e 7036 6c69  aEnv5numba2np6li
+00009d40: 6e61 6c67 3137 5f6f 6e65 445f 6e6f 726d  nalg17_oneD_norm
+00009d50: 5f32 5f69 6d70 6c31 3224 3363 6c6f 6361  _2_impl12$3cloca
+00009d60: 6c73 2433 6539 696d 706c 2432 3436 3245  ls$3e9impl$2462E
+00009d70: 3541 7272 6179 4966 4c69 3145 3143 376d  5ArrayIfLi1E1C7m
+00009d80: 7574 6162 6c65 3761 6c69 676e 6564 455f  utable7alignedE_
+00009d90: 5f5a 4e30 384e 756d 6261 456e 7635 6e75  _ZN08NumbaEnv5nu
+00009da0: 6d62 6132 6e70 366c 696e 616c 6732 355f  mba2np6linalg25_
+00009db0: 6475 6d6d 795f 6c69 7665 6e65 7373 5f66  dummy_liveness_f
+00009dc0: 756e 6324 3234 3239 4533 306c 6973 7424  unc$2429E30list$
+00009dd0: 3238 696e 7436 3424 3239 2433 6369 7624  28int64$29$3civ$
+00009de0: 3364 4e6f 6e65 2433 655f 2e63 6f6e 7374  3dNone$3e_.const
+00009df0: 2e70 6963 6b6c 6562 7566 2e31 3430 3237  .picklebuf.14027
+00009e00: 3938 3733 3237 3031 3932 5f2e 636f 6e73  9873270192_.cons
+00009e10: 742e 7069 636b 6c65 6275 662e 3134 3032  t.picklebuf.1402
+00009e20: 3739 3837 3638 3534 3931 325f 2e63 6f6e  79876854912_.con
+00009e30: 7374 2e70 6963 6b6c 6562 7566 2e31 3430  st.picklebuf.140
+00009e40: 3237 3938 3736 3835 3438 3430 5f2e 636f  279876854840_.co
+00009e50: 6e73 742e 7069 636b 6c65 6275 662e 3134  nst.picklebuf.14
+00009e60: 3032 3739 3839 3031 3038 3438 385f 2e63  0279890108488_.c
+00009e70: 6f6e 7374 2e70 6963 6b6c 6564 6174 612e  onst.pickledata.
+00009e80: 3134 3032 3739 3839 3031 3038 3438 385f  140279890108488_
+00009e90: 2e63 6f6e 7374 2e70 6963 6b6c 6564 6174  .const.pickledat
+00009ea0: 612e 3134 3032 3739 3839 3031 3038 3438  a.14027989010848
+00009eb0: 382e 7368 6131 5f2e 636f 6e73 742e 7069  8.sha1_.const.pi
+00009ec0: 636b 6c65 6461 7461 2e31 3430 3237 3938  ckledata.1402798
+00009ed0: 3736 3835 3438 3430 5f2e 636f 6e73 742e  76854840_.const.
+00009ee0: 7069 636b 6c65 6461 7461 2e31 3430 3237  pickledata.14027
+00009ef0: 3938 3736 3835 3438 3430 2e73 6861 315f  9876854840.sha1_
+00009f00: 2e63 6f6e 7374 2e70 6963 6b6c 6564 6174  .const.pickledat
+00009f10: 612e 3134 3032 3739 3837 3638 3534 3931  a.14027987685491
+00009f20: 325f 2e63 6f6e 7374 2e70 6963 6b6c 6564  2_.const.pickled
+00009f30: 6174 612e 3134 3032 3739 3837 3638 3534  ata.140279876854
+00009f40: 3931 322e 7368 6131 5f2e 636f 6e73 742e  912.sha1_.const.
+00009f50: 7069 636b 6c65 6461 7461 2e31 3430 3237  pickledata.14027
+00009f60: 3938 3733 3237 3031 3932 5f2e 636f 6e73  9873270192_.cons
+00009f70: 742e 7069 636b 6c65 6461 7461 2e31 3430  t.pickledata.140
+00009f80: 3237 3938 3733 3237 3031 3932 2e73 6861  279873270192.sha
+00009f90: 3100 0000 0000 0094 8694 8794 8c13 6e75  1.............nu
+00009fa0: 6d62 612e 636f 7265 2e66 756e 6364 6573  mba.core.funcdes
+00009fb0: 6394 8c18 5079 7468 6f6e 4675 6e63 7469  c...PythonFuncti
+00009fc0: 6f6e 4465 7363 7269 7074 6f72 9493 9429  onDescriptor...)
+00009fd0: 8194 4e7d 9428 8c06 6e61 7469 7665 9488  ..N}.(..native..
+00009fe0: 8c07 6d6f 646e 616d 6594 8c25 7369 6d62  ..modname..%simb
+00009ff0: 612e 6d69 7869 6e73 2e66 6561 7475 7265  a.mixins.feature
+0000a000: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
+0000a010: 6e94 8c08 7175 616c 6e61 6d65 9468 008c  n...qualname.h..
+0000a020: 0364 6f63 9458 ce02 0000 0a20 2020 2020  .doc.X.....     
+0000a030: 2020 204a 6974 7465 6420 616e 616c 6f67     Jitted analog
+0000a040: 7565 206f 6620 6d65 7468 3a60 7363 6970  ue of meth:`scip
+0000a050: 792e 6364 6973 7460 2e0a 0a20 2020 2020  y.cdist`...     
+0000a060: 2020 203a 7061 7261 6d65 7465 7220 6e70     :parameter np
+0000a070: 2e6e 6461 7272 6179 2061 7272 6179 5f31  .ndarray array_1
+0000a080: 3a20 3244 2061 7272 6179 206f 6620 626f  : 2D array of bo
+0000a090: 6479 2d70 6172 7420 636f 6f72 6469 6e61  dy-part coordina
+0000a0a0: 7465 730a 2020 2020 2020 2020 3a70 6172  tes.        :par
+0000a0b0: 616d 6574 6572 206e 702e 6e64 6172 7261  ameter np.ndarra
+0000a0c0: 7920 6172 7261 795f 323a 2032 4420 6172  y array_2: 2D ar
+0000a0d0: 7261 7920 6f66 2062 6f64 792d 7061 7274  ray of body-part
+0000a0e0: 2063 6f6f 7264 696e 6174 6573 0a20 2020   coordinates.   
+0000a0f0: 2020 2020 203a 7265 7475 726e 206e 702e       :return np.
+0000a100: 6e64 6172 7261 793a 2032 4420 6172 7261  ndarray: 2D arra
+0000a110: 7920 6f66 2065 7563 6c69 6465 616e 2064  y of euclidean d
+0000a120: 6973 7461 6e63 6573 2062 6574 7765 656e  istances between
+0000a130: 2062 6f64 792d 7061 7274 7320 696e 2060   body-parts in `
+0000a140: 6061 7272 6179 5f31 6060 2061 6e64 2060  `array_1`` and `
+0000a150: 6061 7272 6179 5f32 6060 0a0a 2020 2020  `array_2``..    
+0000a160: 2020 2020 3a65 7861 6d70 6c65 3a0a 2020      :example:.  
+0000a170: 2020 2020 2020 3e3e 3e20 6172 7261 795f        >>> array_
+0000a180: 3120 3d20 6e70 2e72 616e 646f 6d2e 7261  1 = np.random.ra
+0000a190: 6e64 696e 7428 312c 2031 302c 2073 697a  ndint(1, 10, siz
+0000a1a0: 653d 2833 2c20 3229 292e 6173 7479 7065  e=(3, 2)).astype
+0000a1b0: 286e 702e 666c 6f61 7433 3229 0a20 2020  (np.float32).   
+0000a1c0: 2020 2020 203e 3e3e 2061 7272 6179 5f32       >>> array_2
+0000a1d0: 203d 206e 702e 7261 6e64 6f6d 2e72 616e   = np.random.ran
+0000a1e0: 6469 6e74 2831 2c20 3130 2c20 7369 7a65  dint(1, 10, size
+0000a1f0: 3d28 332c 2032 2929 2e61 7374 7970 6528  =(3, 2)).astype(
+0000a200: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
+0000a210: 2020 2020 3e3e 3e20 4665 6174 7572 6545      >>> FeatureE
+0000a220: 7874 7261 6374 696f 6e4d 6978 696e 2e63  xtractionMixin.c
+0000a230: 6469 7374 2861 7272 6179 5f31 3d61 7272  dist(array_1=arr
+0000a240: 6179 5f31 2c20 6172 7261 795f 323d 6172  ay_1, array_2=ar
+0000a250: 7261 795f 3229 0a20 2020 2020 2020 203e  ray_2).        >
+0000a260: 3e3e 205b 5b37 2e30 3731 3036 3738 312c  >> [[7.07106781,
+0000a270: 2031 2e20 2020 2020 2020 202c 2033 2e36   1.        , 3.6
+0000a280: 3035 3535 3132 345d 2c0a 2020 2020 2020  0555124],.      
+0000a290: 2020 3e3e 3e20 5b33 2e36 3035 3535 3132    >>> [3.6055512
+0000a2a0: 342c 2036 2e33 3234 3535 3534 202c 2032  4, 6.3245554 , 2
+0000a2b0: 2e20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+0000a2c0: 2020 2020 3e3e 3e20 205b 332e 3136 3232      >>>  [3.1622
+0000a2d0: 3737 3720 2c20 352e 3338 3531 3634 3734  777 , 5.38516474
+0000a2e0: 2c20 342e 3132 3331 3035 3533 5d5d 290a  , 4.12310553]]).
+0000a2f0: 2020 2020 2020 2020 948c 0774 7970 656d          ...typem
+0000a300: 6170 944e 8c09 6361 6c6c 7479 7065 7394  ap.N..calltypes.
+0000a310: 4e8c 0461 7267 7394 8c07 6172 7261 795f  N..args...array_
+0000a320: 3194 8c07 6172 7261 795f 3294 8694 8c03  1...array_2.....
+0000a330: 6b77 7394 298c 0772 6573 7479 7065 948c  kws.)..restype..
+0000a340: 196e 756d 6261 2e63 6f72 652e 7479 7065  .numba.core.type
+0000a350: 732e 6162 7374 7261 6374 948c 135f 7479  s.abstract..._ty
+0000a360: 7065 5f72 6563 6f6e 7374 7275 6374 6f72  pe_reconstructor
+0000a370: 9493 948c 0763 6f70 7972 6567 948c 0e5f  .....copyreg..._
+0000a380: 7265 636f 6e73 7472 7563 746f 7294 9394  reconstructor...
+0000a390: 8c19 6e75 6d62 612e 636f 7265 2e74 7970  ..numba.core.typ
+0000a3a0: 6573 2e6e 7079 7479 7065 7394 8c05 4172  es.npytypes...Ar
+0000a3b0: 7261 7994 9394 8c08 6275 696c 7469 6e73  ray.....builtins
+0000a3c0: 948c 066f 626a 6563 7494 9394 4e87 947d  ...object...N..}
+0000a3d0: 9428 8c05 6474 7970 6594 681b 681e 8c18  .(..dtype.h.h...
+0000a3e0: 6e75 6d62 612e 636f 7265 2e74 7970 6573  numba.core.types
+0000a3f0: 2e73 6361 6c61 7273 948c 0546 6c6f 6174  .scalars...Float
+0000a400: 9493 9468 244e 8794 7d94 288c 046e 616d  ...h$N..}.(..nam
+0000a410: 6594 8c07 666c 6f61 7436 3494 8c08 6269  e...float64...bi
+0000a420: 7477 6964 7468 944b 408c 055f 636f 6465  twidth.K@.._code
+0000a430: 944b 1775 8794 5294 8c04 6e64 696d 944b  .K.u..R...ndim.K
+0000a440: 028c 066c 6179 6f75 7494 8c01 4394 682d  ...layout...C.h-
+0000a450: 8c15 6172 7261 7928 666c 6f61 7436 342c  ..array(float64,
+0000a460: 2032 642c 2043 2994 6830 4db7 0675 8794   2d, C).h0M..u..
+0000a470: 5294 8c08 6172 6774 7970 6573 9468 1b68  R...argtypes.h.h
+0000a480: 1e68 2168 244e 8794 7d94 2868 2768 1b68  .h!h$N..}.(h'h.h
+0000a490: 1e68 2a68 244e 8794 7d94 2868 2d8c 0766  .h*h$N..}.(h-..f
+0000a4a0: 6c6f 6174 3332 9468 2f4b 2068 304b 1675  loat32.h/K h0K.u
+0000a4b0: 8794 5294 6833 4b02 6834 8c01 4194 682d  ..R.h3K.h4..A.h-
+0000a4c0: 8c15 6172 7261 7928 666c 6f61 7433 322c  ..array(float32,
+0000a4d0: 2032 642c 2041 2994 6830 4df7 0375 8794   2d, A).h0M..u..
+0000a4e0: 5294 6844 8694 8c0c 6d61 6e67 6c65 645f  R.hD....mangled_
+0000a4f0: 6e61 6d65 948c 8d5f 5a4e 3573 696d 6261  name..._ZN5simba
+0000a500: 366d 6978 696e 7332 3466 6561 7475 7265  6mixins24feature
+0000a510: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
+0000a520: 6e32 3246 6561 7475 7265 4578 7472 6163  n22FeatureExtrac
+0000a530: 7469 6f6e 4d69 7869 6e31 3063 6469 7374  tionMixin10cdist
+0000a540: 2432 3436 3045 3541 7272 6179 4966 4c69  $2460E5ArrayIfLi
+0000a550: 3245 3141 376d 7574 6162 6c65 3761 6c69  2E1A7mutable7ali
+0000a560: 676e 6564 4535 4172 7261 7949 664c 6932  gnedE5ArrayIfLi2
+0000a570: 4531 4137 6d75 7461 626c 6537 616c 6967  E1A7mutable7alig
+0000a580: 6e65 6445 948c 0b75 6e69 7175 655f 6e61  nedE...unique_na
+0000a590: 6d65 948c 1f46 6561 7475 7265 4578 7472  me...FeatureExtr
+0000a5a0: 6163 7469 6f6e 4d69 7869 6e2e 6364 6973  actionMixin.cdis
+0000a5b0: 7424 3630 948c 0865 6e76 5f6e 616d 6594  t$60...env_name.
+0000a5c0: 8c97 5f5a 4e30 384e 756d 6261 456e 7635  .._ZN08NumbaEnv5
+0000a5d0: 7369 6d62 6136 6d69 7869 6e73 3234 6665  simba6mixins24fe
+0000a5e0: 6174 7572 655f 6578 7472 6163 7469 6f6e  ature_extraction
+0000a5f0: 5f6d 6978 696e 3232 4665 6174 7572 6545  _mixin22FeatureE
+0000a600: 7874 7261 6374 696f 6e4d 6978 696e 3130  xtractionMixin10
+0000a610: 6364 6973 7424 3234 3630 4535 4172 7261  cdist$2460E5Arra
+0000a620: 7949 664c 6932 4531 4137 6d75 7461 626c  yIfLi2E1A7mutabl
+0000a630: 6537 616c 6967 6e65 6445 3541 7272 6179  e7alignedE5Array
+0000a640: 4966 4c69 3245 3141 376d 7574 6162 6c65  IfLi2E1A7mutable
+0000a650: 3761 6c69 676e 6564 4594 8c0b 676c 6f62  7alignedE...glob
+0000a660: 616c 5f64 6963 7494 4e8c 0669 6e6c 696e  al_dict.N..inlin
+0000a670: 6594 898c 076e 6f61 6c69 6173 9489 7586  e....noalias..u.
+0000a680: 9462 8c16 6e75 6d62 612e 636f 7265 2e65  .b..numba.core.e
+0000a690: 6e76 6972 6f6e 6d65 6e74 948c 0c5f 7265  nvironment..._re
+0000a6a0: 6275 696c 645f 656e 7694 9394 680d 5d94  build_env...h.].
+0000a6b0: 8c05 6e75 6d70 7994 8c05 6474 7970 6594  ..numpy...dtype.
+0000a6c0: 9394 8c02 6638 944b 004b 0187 9452 9428  ....f8.K.K...R.(
+0000a6d0: 4b03 8c01 3c94 4e4e 4e4a ffff ffff 4aff  K...<.NNNJ....J.
+0000a6e0: ffff ff4b 0074 9462 6168 4b87 9452 948c  ...K.t.bahK..R..
+0000a6f0: 1b6e 756d 6261 2e63 6f72 652e 7479 7069  .numba.core.typi
+0000a700: 6e67 2e74 656d 706c 6174 6573 948c 0953  ng.templates...S
+0000a710: 6967 6e61 7475 7265 9493 9429 8194 2868  ignature...)..(h
+0000a720: 3868 4468 4486 944e 4e74 9462 8929 58c5  8hDhD..NNt.b.)X.
+0000a730: 2000 0023 2046 696c 653a 202f 5573 6572   ..# File: /User
+0000a740: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+0000a750: 656e 7673 2f73 696d 6261 5f64 6576 2f73  envs/simba_dev/s
+0000a760: 696d 6261 2f6d 6978 696e 732f 6665 6174  imba/mixins/feat
+0000a770: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
+0000a780: 6978 696e 2e70 790a 2320 2d2d 2d20 4c49  ixin.py.# --- LI
+0000a790: 4e45 2033 3333 202d 2d2d 200a 0a40 7374  NE 333 --- ..@st
+0000a7a0: 6174 6963 6d65 7468 6f64 0a0a 2320 2d2d  aticmethod..# --
+0000a7b0: 2d20 4c49 4e45 2033 3334 202d 2d2d 200a  - LINE 334 --- .
+0000a7c0: 0a40 6a69 7428 6e6f 7079 7468 6f6e 3d54  .@jit(nopython=T
+0000a7d0: 7275 652c 2063 6163 6865 3d54 7275 6529  rue, cache=True)
+0000a7e0: 0a0a 2320 2d2d 2d20 4c49 4e45 2033 3335  ..# --- LINE 335
+0000a7f0: 202d 2d2d 200a 0a64 6566 2063 6469 7374   --- ..def cdist
+0000a800: 2861 7272 6179 5f31 3a20 6e70 2e6e 6461  (array_1: np.nda
+0000a810: 7272 6179 2c0a 0a20 2020 2020 2020 2020  rray,..         
+0000a820: 2023 202d 2d2d 204c 494e 4520 3333 3620   # --- LINE 336 
+0000a830: 2d2d 2d20 0a0a 2020 2020 2020 2020 2020  --- ..          
+0000a840: 6172 7261 795f 323a 206e 702e 6e64 6172  array_2: np.ndar
+0000a850: 7261 7929 202d 3e20 6e70 2e6e 6461 7272  ray) -> np.ndarr
+0000a860: 6179 3a0a 0a20 2020 2023 202d 2d2d 204c  ay:..    # --- L
+0000a870: 494e 4520 3333 3720 2d2d 2d20 0a0a 2020  INE 337 --- ..  
+0000a880: 2020 2222 220a 0a20 2020 2023 202d 2d2d    """..    # ---
+0000a890: 204c 494e 4520 3333 3820 2d2d 2d20 0a0a   LINE 338 --- ..
+0000a8a0: 2020 2020 4a69 7474 6564 2061 6e61 6c6f      Jitted analo
+0000a8b0: 6775 6520 6f66 206d 6574 683a 6073 6369  gue of meth:`sci
+0000a8c0: 7079 2e63 6469 7374 602e 0a0a 2320 2d2d  py.cdist`...# --
+0000a8d0: 2d20 4c49 4e45 2033 3339 202d 2d2d 200a  - LINE 339 --- .
+0000a8e0: 0a0a 0a20 2020 2023 202d 2d2d 204c 494e  ...    # --- LIN
+0000a8f0: 4520 3334 3020 2d2d 2d20 0a0a 2020 2020  E 340 --- ..    
+0000a900: 3a70 6172 616d 6574 6572 206e 702e 6e64  :parameter np.nd
+0000a910: 6172 7261 7920 6172 7261 795f 313a 2032  array array_1: 2
+0000a920: 4420 6172 7261 7920 6f66 2062 6f64 792d  D array of body-
+0000a930: 7061 7274 2063 6f6f 7264 696e 6174 6573  part coordinates
+0000a940: 0a0a 2020 2020 2320 2d2d 2d20 4c49 4e45  ..    # --- LINE
+0000a950: 2033 3431 202d 2d2d 200a 0a20 2020 203a   341 --- ..    :
+0000a960: 7061 7261 6d65 7465 7220 6e70 2e6e 6461  parameter np.nda
+0000a970: 7272 6179 2061 7272 6179 5f32 3a20 3244  rray array_2: 2D
+0000a980: 2061 7272 6179 206f 6620 626f 6479 2d70   array of body-p
+0000a990: 6172 7420 636f 6f72 6469 6e61 7465 730a  art coordinates.
+0000a9a0: 0a20 2020 2023 202d 2d2d 204c 494e 4520  .    # --- LINE 
+0000a9b0: 3334 3220 2d2d 2d20 0a0a 2020 2020 3a72  342 --- ..    :r
+0000a9c0: 6574 7572 6e20 6e70 2e6e 6461 7272 6179  eturn np.ndarray
+0000a9d0: 3a20 3244 2061 7272 6179 206f 6620 6575  : 2D array of eu
+0000a9e0: 636c 6964 6561 6e20 6469 7374 616e 6365  clidean distance
+0000a9f0: 7320 6265 7477 6565 6e20 626f 6479 2d70  s between body-p
+0000aa00: 6172 7473 2069 6e20 6060 6172 7261 795f  arts in ``array_
+0000aa10: 3160 6020 616e 6420 6060 6172 7261 795f  1`` and ``array_
+0000aa20: 3260 600a 0a23 202d 2d2d 204c 494e 4520  2``..# --- LINE 
+0000aa30: 3334 3320 2d2d 2d20 0a0a 0a0a 2020 2020  343 --- ....    
+0000aa40: 2320 2d2d 2d20 4c49 4e45 2033 3434 202d  # --- LINE 344 -
+0000aa50: 2d2d 200a 0a20 2020 203a 6578 616d 706c  -- ..    :exampl
+0000aa60: 653a 0a0a 2020 2020 2320 2d2d 2d20 4c49  e:..    # --- LI
+0000aa70: 4e45 2033 3435 202d 2d2d 200a 0a20 2020  NE 345 --- ..   
+0000aa80: 203e 3e3e 2061 7272 6179 5f31 203d 206e   >>> array_1 = n
+0000aa90: 702e 7261 6e64 6f6d 2e72 616e 6469 6e74  p.random.randint
+0000aaa0: 2831 2c20 3130 2c20 7369 7a65 3d28 332c  (1, 10, size=(3,
+0000aab0: 2032 2929 2e61 7374 7970 6528 6e70 2e66   2)).astype(np.f
+0000aac0: 6c6f 6174 3332 290a 0a20 2020 2023 202d  loat32)..    # -
+0000aad0: 2d2d 204c 494e 4520 3334 3620 2d2d 2d20  -- LINE 346 --- 
+0000aae0: 0a0a 2020 2020 3e3e 3e20 6172 7261 795f  ..    >>> array_
+0000aaf0: 3220 3d20 6e70 2e72 616e 646f 6d2e 7261  2 = np.random.ra
+0000ab00: 6e64 696e 7428 312c 2031 302c 2073 697a  ndint(1, 10, siz
+0000ab10: 653d 2833 2c20 3229 292e 6173 7479 7065  e=(3, 2)).astype
+0000ab20: 286e 702e 666c 6f61 7433 3229 0a0a 2020  (np.float32)..  
+0000ab30: 2020 2320 2d2d 2d20 4c49 4e45 2033 3437    # --- LINE 347
+0000ab40: 202d 2d2d 200a 0a20 2020 203e 3e3e 2046   --- ..    >>> F
+0000ab50: 6561 7475 7265 4578 7472 6163 7469 6f6e  eatureExtraction
+0000ab60: 4d69 7869 6e2e 6364 6973 7428 6172 7261  Mixin.cdist(arra
+0000ab70: 795f 313d 6172 7261 795f 312c 2061 7272  y_1=array_1, arr
+0000ab80: 6179 5f32 3d61 7272 6179 5f32 290a 0a20  ay_2=array_2).. 
+0000ab90: 2020 2023 202d 2d2d 204c 494e 4520 3334     # --- LINE 34
+0000aba0: 3820 2d2d 2d20 0a0a 2020 2020 3e3e 3e20  8 --- ..    >>> 
+0000abb0: 5b5b 372e 3037 3130 3637 3831 2c20 312e  [[7.07106781, 1.
+0000abc0: 2020 2020 2020 2020 2c20 332e 3630 3535          , 3.6055
+0000abd0: 3531 3234 5d2c 0a0a 2020 2020 2320 2d2d  5124],..    # --
+0000abe0: 2d20 4c49 4e45 2033 3439 202d 2d2d 200a  - LINE 349 --- .
+0000abf0: 0a20 2020 203e 3e3e 205b 332e 3630 3535  .    >>> [3.6055
+0000ac00: 3531 3234 2c20 362e 3332 3435 3535 3420  5124, 6.3245554 
+0000ac10: 2c20 322e 2020 2020 2020 2020 5d2c 0a0a  , 2.        ],..
+0000ac20: 2020 2020 2320 2d2d 2d20 4c49 4e45 2033      # --- LINE 3
+0000ac30: 3530 202d 2d2d 200a 0a20 2020 203e 3e3e  50 --- ..    >>>
+0000ac40: 2020 5b33 2e31 3632 3237 3737 202c 2035    [3.1622777 , 5
+0000ac50: 2e33 3835 3136 3437 342c 2034 2e31 3233  .38516474, 4.123
+0000ac60: 3130 3535 335d 5d29 0a0a 2020 2020 2320  10553]])..    # 
+0000ac70: 2d2d 2d20 4c49 4e45 2033 3531 202d 2d2d  --- LINE 351 ---
+0000ac80: 200a 0a20 2020 2022 2222 0a0a 2020 2020   ..    """..    
+0000ac90: 2320 2d2d 2d20 4c49 4e45 2033 3532 202d  # --- LINE 352 -
+0000aca0: 2d2d 200a 2020 2020 2320 6c61 6265 6c20  -- .    # label 
+0000acb0: 300a 2020 2020 2320 2020 6172 7261 795f  0.    #   array_
+0000acc0: 3120 3d20 6172 6728 302c 206e 616d 653d  1 = arg(0, name=
+0000acd0: 6172 7261 795f 3129 2020 3a3a 2061 7272  array_1)  :: arr
+0000ace0: 6179 2866 6c6f 6174 3332 2c20 3264 2c20  ay(float32, 2d, 
+0000acf0: 4129 0a20 2020 2023 2020 2061 7272 6179  A).    #   array
+0000ad00: 5f32 203d 2061 7267 2831 2c20 6e61 6d65  _2 = arg(1, name
+0000ad10: 3d61 7272 6179 5f32 2920 203a 3a20 6172  =array_2)  :: ar
+0000ad20: 7261 7928 666c 6f61 7433 322c 2032 642c  ray(float32, 2d,
+0000ad30: 2041 290a 2020 2020 2320 2020 2430 2e31   A).    #   $0.1
+0000ad40: 203d 2067 6c6f 6261 6c28 6e70 3a20 3c6d   = global(np: <m
+0000ad50: 6f64 756c 6520 276e 756d 7079 2720 6672  odule 'numpy' fr
+0000ad60: 6f6d 2027 2f55 7365 7273 2f73 696d 6f6e  om '/Users/simon
+0000ad70: 2f2e 636f 6e64 612f 656e 7673 2f73 696d  /.conda/envs/sim
+0000ad80: 6261 5f64 6576 2f6c 6962 2f70 7974 686f  ba_dev/lib/pytho
+0000ad90: 6e33 2e36 2f73 6974 652d 7061 636b 6167  n3.6/site-packag
+0000ada0: 6573 2f6e 756d 7079 2f5f 5f69 6e69 745f  es/numpy/__init_
+0000adb0: 5f2e 7079 273e 2920 203a 3a20 4d6f 6475  _.py'>)  :: Modu
+0000adc0: 6c65 283c 6d6f 6475 6c65 2027 6e75 6d70  le(<module 'nump
+0000add0: 7927 2066 726f 6d20 272f 5573 6572 732f  y' from '/Users/
+0000ade0: 7369 6d6f 6e2f 2e63 6f6e 6461 2f65 6e76  simon/.conda/env
+0000adf0: 732f 7369 6d62 615f 6465 762f 6c69 622f  s/simba_dev/lib/
+0000ae00: 7079 7468 6f6e 332e 362f 7369 7465 2d70  python3.6/site-p
+0000ae10: 6163 6b61 6765 732f 6e75 6d70 792f 5f5f  ackages/numpy/__
+0000ae20: 696e 6974 5f5f 2e70 7927 3e29 0a20 2020  init__.py'>).   
+0000ae30: 2023 2020 2024 302e 3220 3d20 6765 7461   #   $0.2 = geta
+0000ae40: 7474 7228 7661 6c75 653d 2430 2e31 2c20  ttr(value=$0.1, 
+0000ae50: 6174 7472 3d66 756c 6c29 2020 3a3a 2046  attr=full)  :: F
+0000ae60: 756e 6374 696f 6e28 3c66 756e 6374 696f  unction(<functio
+0000ae70: 6e20 6675 6c6c 2061 7420 3078 3766 3935  n full at 0x7f95
+0000ae80: 3665 6438 3235 3130 3e29 0a20 2020 2023  6ed82510>).    #
+0000ae90: 2020 2064 656c 2024 302e 310a 2020 2020     del $0.1.    
+0000aea0: 2320 2020 2430 2e34 203d 2067 6574 6174  #   $0.4 = getat
+0000aeb0: 7472 2876 616c 7565 3d61 7272 6179 5f31  tr(value=array_1
+0000aec0: 2c20 6174 7472 3d73 6861 7065 2920 203a  , attr=shape)  :
+0000aed0: 3a20 556e 6954 7570 6c65 2869 6e74 3634  : UniTuple(int64
+0000aee0: 2078 2032 290a 2020 2020 2320 2020 2463   x 2).    #   $c
+0000aef0: 6f6e 7374 302e 3520 3d20 636f 6e73 7428  onst0.5 = const(
+0000af00: 696e 742c 2030 2920 203a 3a20 4c69 7465  int, 0)  :: Lite
+0000af10: 7261 6c5b 696e 745d 2830 290a 2020 2020  ral[int](0).    
+0000af20: 2320 2020 2430 2e36 203d 2073 7461 7469  #   $0.6 = stati
+0000af30: 635f 6765 7469 7465 6d28 7661 6c75 653d  c_getitem(value=
+0000af40: 2430 2e34 2c20 696e 6465 783d 302c 2069  $0.4, index=0, i
+0000af50: 6e64 6578 5f76 6172 3d24 636f 6e73 7430  ndex_var=$const0
+0000af60: 2e35 2c20 666e 3d3c 6275 696c 742d 696e  .5, fn=<built-in
+0000af70: 2066 756e 6374 696f 6e20 6765 7469 7465   function getite
+0000af80: 6d3e 2920 203a 3a20 696e 7436 340a 2020  m>)  :: int64.  
+0000af90: 2020 2320 2020 6465 6c20 2463 6f6e 7374    #   del $const
+0000afa0: 302e 350a 2020 2020 2320 2020 6465 6c20  0.5.    #   del 
+0000afb0: 2430 2e34 0a20 2020 2023 2020 2024 302e  $0.4.    #   $0.
+0000afc0: 3820 3d20 6765 7461 7474 7228 7661 6c75  8 = getattr(valu
+0000afd0: 653d 6172 7261 795f 322c 2061 7474 723d  e=array_2, attr=
+0000afe0: 7368 6170 6529 2020 3a3a 2055 6e69 5475  shape)  :: UniTu
+0000aff0: 706c 6528 696e 7436 3420 7820 3229 0a20  ple(int64 x 2). 
+0000b000: 2020 2023 2020 2024 636f 6e73 7430 2e39     #   $const0.9
+0000b010: 203d 2063 6f6e 7374 2869 6e74 2c20 3029   = const(int, 0)
+0000b020: 2020 3a3a 204c 6974 6572 616c 5b69 6e74    :: Literal[int
+0000b030: 5d28 3029 0a20 2020 2023 2020 2024 302e  ](0).    #   $0.
+0000b040: 3130 203d 2073 7461 7469 635f 6765 7469  10 = static_geti
+0000b050: 7465 6d28 7661 6c75 653d 2430 2e38 2c20  tem(value=$0.8, 
+0000b060: 696e 6465 783d 302c 2069 6e64 6578 5f76  index=0, index_v
+0000b070: 6172 3d24 636f 6e73 7430 2e39 2c20 666e  ar=$const0.9, fn
+0000b080: 3d3c 6275 696c 742d 696e 2066 756e 6374  =<built-in funct
+0000b090: 696f 6e20 6765 7469 7465 6d3e 2920 203a  ion getitem>)  :
+0000b0a0: 3a20 696e 7436 340a 2020 2020 2320 2020  : int64.    #   
+0000b0b0: 6465 6c20 2463 6f6e 7374 302e 390a 2020  del $const0.9.  
+0000b0c0: 2020 2320 2020 6465 6c20 2430 2e38 0a20    #   del $0.8. 
+0000b0d0: 2020 2023 2020 2024 302e 3131 203d 2062     #   $0.11 = b
+0000b0e0: 7569 6c64 5f74 7570 6c65 2869 7465 6d73  uild_tuple(items
+0000b0f0: 3d5b 5661 7228 2430 2e36 2c20 6665 6174  =[Var($0.6, feat
+0000b100: 7572 655f 6578 7472 6163 7469 6f6e 5f6d  ure_extraction_m
+0000b110: 6978 696e 2e70 793a 3335 3229 2c20 5661  ixin.py:352), Va
+0000b120: 7228 2430 2e31 302c 2066 6561 7475 7265  r($0.10, feature
+0000b130: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
+0000b140: 6e2e 7079 3a33 3532 295d 2920 203a 3a20  n.py:352)])  :: 
+0000b150: 556e 6954 7570 6c65 2869 6e74 3634 2078  UniTuple(int64 x
+0000b160: 2032 290a 2020 2020 2320 2020 6465 6c20   2).    #   del 
+0000b170: 2430 2e36 0a20 2020 2023 2020 2064 656c  $0.6.    #   del
+0000b180: 2024 302e 3130 0a20 2020 2023 2020 2024   $0.10.    #   $
+0000b190: 302e 3132 203d 2067 6c6f 6261 6c28 6e70  0.12 = global(np
+0000b1a0: 3a20 3c6d 6f64 756c 6520 276e 756d 7079  : <module 'numpy
+0000b1b0: 2720 6672 6f6d 2027 2f55 7365 7273 2f73  ' from '/Users/s
+0000b1c0: 696d 6f6e 2f2e 636f 6e64 612f 656e 7673  imon/.conda/envs
+0000b1d0: 2f73 696d 6261 5f64 6576 2f6c 6962 2f70  /simba_dev/lib/p
+0000b1e0: 7974 686f 6e33 2e36 2f73 6974 652d 7061  ython3.6/site-pa
+0000b1f0: 636b 6167 6573 2f6e 756d 7079 2f5f 5f69  ckages/numpy/__i
+0000b200: 6e69 745f 5f2e 7079 273e 2920 203a 3a20  nit__.py'>)  :: 
+0000b210: 4d6f 6475 6c65 283c 6d6f 6475 6c65 2027  Module(<module '
+0000b220: 6e75 6d70 7927 2066 726f 6d20 272f 5573  numpy' from '/Us
+0000b230: 6572 732f 7369 6d6f 6e2f 2e63 6f6e 6461  ers/simon/.conda
+0000b240: 2f65 6e76 732f 7369 6d62 615f 6465 762f  /envs/simba_dev/
+0000b250: 6c69 622f 7079 7468 6f6e 332e 362f 7369  lib/python3.6/si
+0000b260: 7465 2d70 6163 6b61 6765 732f 6e75 6d70  te-packages/nump
+0000b270: 792f 5f5f 696e 6974 5f5f 2e70 7927 3e29  y/__init__.py'>)
+0000b280: 0a20 2020 2023 2020 2024 302e 3133 203d  .    #   $0.13 =
+0000b290: 2067 6574 6174 7472 2876 616c 7565 3d24   getattr(value=$
+0000b2a0: 302e 3132 2c20 6174 7472 3d6e 616e 2920  0.12, attr=nan) 
+0000b2b0: 203a 3a20 666c 6f61 7436 340a 2020 2020   :: float64.    
+0000b2c0: 2320 2020 6465 6c20 2430 2e31 320a 2020  #   del $0.12.  
+0000b2d0: 2020 2320 2020 2430 2e31 3420 3d20 6361    #   $0.14 = ca
+0000b2e0: 6c6c 2024 302e 3228 2430 2e31 312c 2024  ll $0.2($0.11, $
+0000b2f0: 302e 3133 2c20 6675 6e63 3d24 302e 322c  0.13, func=$0.2,
+0000b300: 2061 7267 733d 5b56 6172 2824 302e 3131   args=[Var($0.11
+0000b310: 2c20 6665 6174 7572 655f 6578 7472 6163  , feature_extrac
+0000b320: 7469 6f6e 5f6d 6978 696e 2e70 793a 3335  tion_mixin.py:35
+0000b330: 3229 2c20 5661 7228 2430 2e31 332c 2066  2), Var($0.13, f
+0000b340: 6561 7475 7265 5f65 7874 7261 6374 696f  eature_extractio
+0000b350: 6e5f 6d69 7869 6e2e 7079 3a33 3532 295d  n_mixin.py:352)]
+0000b360: 2c20 6b77 733d 2829 2c20 7661 7261 7267  , kws=(), vararg
+0000b370: 3d4e 6f6e 6529 2020 3a3a 2028 556e 6954  =None)  :: (UniT
+0000b380: 7570 6c65 2869 6e74 3634 2078 2032 292c  uple(int64 x 2),
+0000b390: 2066 6c6f 6174 3634 2920 2d3e 2061 7272   float64) -> arr
+0000b3a0: 6179 2866 6c6f 6174 3634 2c20 3264 2c20  ay(float64, 2d, 
+0000b3b0: 4329 0a20 2020 2023 2020 2064 656c 2024  C).    #   del $
+0000b3c0: 302e 320a 2020 2020 2320 2020 6465 6c20  0.2.    #   del 
+0000b3d0: 2430 2e31 330a 2020 2020 2320 2020 6465  $0.13.    #   de
+0000b3e0: 6c20 2430 2e31 310a 2020 2020 2320 2020  l $0.11.    #   
+0000b3f0: 7265 7375 6c74 7320 3d20 2430 2e31 3420  results = $0.14 
+0000b400: 203a 3a20 6172 7261 7928 666c 6f61 7436   :: array(float6
+0000b410: 342c 2032 642c 2043 290a 2020 2020 2320  4, 2d, C).    # 
+0000b420: 2020 6465 6c20 2430 2e31 340a 0a20 2020    del $0.14..   
+0000b430: 2072 6573 756c 7473 203d 206e 702e 6675   results = np.fu
+0000b440: 6c6c 2828 6172 7261 795f 312e 7368 6170  ll((array_1.shap
+0000b450: 655b 305d 2c20 6172 7261 795f 322e 7368  e[0], array_2.sh
+0000b460: 6170 655b 305d 292c 206e 702e 6e61 6e29  ape[0]), np.nan)
+0000b470: 0a0a 2020 2020 2320 2d2d 2d20 4c49 4e45  ..    # --- LINE
+0000b480: 2033 3533 202d 2d2d 200a 2020 2020 2320   353 --- .    # 
+0000b490: 2020 6a75 6d70 2033 320a 2020 2020 2320    jump 32.    # 
+0000b4a0: 6c61 6265 6c20 3332 0a20 2020 2023 2020  label 32.    #  
+0000b4b0: 206a 756d 7020 3334 0a20 2020 2023 206c   jump 34.    # l
+0000b4c0: 6162 656c 2033 340a 2020 2020 2320 2020  abel 34.    #   
+0000b4d0: 2433 342e 3120 3d20 676c 6f62 616c 2870  $34.1 = global(p
+0000b4e0: 7261 6e67 653a 203c 636c 6173 7320 276e  range: <class 'n
+0000b4f0: 756d 6261 2e6d 6973 632e 7370 6563 6961  umba.misc.specia
+0000b500: 6c2e 7072 616e 6765 273e 2920 203a 3a20  l.prange'>)  :: 
+0000b510: 4675 6e63 7469 6f6e 283c 636c 6173 7320  Function(<class 
+0000b520: 276e 756d 6261 2e6d 6973 632e 7370 6563  'numba.misc.spec
+0000b530: 6961 6c2e 7072 616e 6765 273e 290a 2020  ial.prange'>).  
+0000b540: 2020 2320 2020 2433 342e 3320 3d20 6765    #   $34.3 = ge
+0000b550: 7461 7474 7228 7661 6c75 653d 6172 7261  tattr(value=arra
+0000b560: 795f 312c 2061 7474 723d 7368 6170 6529  y_1, attr=shape)
+0000b570: 2020 3a3a 2055 6e69 5475 706c 6528 696e    :: UniTuple(in
+0000b580: 7436 3420 7820 3229 0a20 2020 2023 2020  t64 x 2).    #  
+0000b590: 2024 636f 6e73 7433 342e 3420 3d20 636f   $const34.4 = co
+0000b5a0: 6e73 7428 696e 742c 2030 2920 203a 3a20  nst(int, 0)  :: 
+0000b5b0: 4c69 7465 7261 6c5b 696e 745d 2830 290a  Literal[int](0).
+0000b5c0: 2020 2020 2320 2020 2433 342e 3520 3d20      #   $34.5 = 
+0000b5d0: 7374 6174 6963 5f67 6574 6974 656d 2876  static_getitem(v
+0000b5e0: 616c 7565 3d24 3334 2e33 2c20 696e 6465  alue=$34.3, inde
+0000b5f0: 783d 302c 2069 6e64 6578 5f76 6172 3d24  x=0, index_var=$
+0000b600: 636f 6e73 7433 342e 342c 2066 6e3d 3c62  const34.4, fn=<b
+0000b610: 7569 6c74 2d69 6e20 6675 6e63 7469 6f6e  uilt-in function
+0000b620: 2067 6574 6974 656d 3e29 2020 3a3a 2069   getitem>)  :: i
+0000b630: 6e74 3634 0a20 2020 2023 2020 2064 656c  nt64.    #   del
+0000b640: 2024 636f 6e73 7433 342e 340a 2020 2020   $const34.4.    
+0000b650: 2320 2020 6465 6c20 2433 342e 330a 2020  #   del $34.3.  
+0000b660: 2020 2320 2020 2433 342e 3620 3d20 6361    #   $34.6 = ca
+0000b670: 6c6c 2024 3334 2e31 2824 3334 2e35 2c20  ll $34.1($34.5, 
+0000b680: 6675 6e63 3d24 3334 2e31 2c20 6172 6773  func=$34.1, args
+0000b690: 3d5b 5661 7228 2433 342e 352c 2066 6561  =[Var($34.5, fea
+0000b6a0: 7475 7265 5f65 7874 7261 6374 696f 6e5f  ture_extraction_
+0000b6b0: 6d69 7869 6e2e 7079 3a33 3533 295d 2c20  mixin.py:353)], 
+0000b6c0: 6b77 733d 2829 2c20 7661 7261 7267 3d4e  kws=(), vararg=N
+0000b6d0: 6f6e 6529 2020 3a3a 2028 696e 7436 342c  one)  :: (int64,
+0000b6e0: 2920 2d3e 2072 616e 6765 5f73 7461 7465  ) -> range_state
+0000b6f0: 5f69 6e74 3634 0a20 2020 2023 2020 2064  _int64.    #   d
+0000b700: 656c 2024 3334 2e35 0a20 2020 2023 2020  el $34.5.    #  
+0000b710: 2064 656c 2024 3334 2e31 0a20 2020 2023   del $34.1.    #
+0000b720: 2020 2024 3334 2e37 203d 2067 6574 6974     $34.7 = getit
+0000b730: 6572 2876 616c 7565 3d24 3334 2e36 2920  er(value=$34.6) 
+0000b740: 203a 3a20 7261 6e67 655f 6974 6572 5f69   :: range_iter_i
+0000b750: 6e74 3634 0a20 2020 2023 2020 2064 656c  nt64.    #   del
+0000b760: 2024 3334 2e36 0a20 2020 2023 2020 2024   $34.6.    #   $
+0000b770: 7068 6934 382e 3120 3d20 2433 342e 3720  phi48.1 = $34.7 
+0000b780: 203a 3a20 7261 6e67 655f 6974 6572 5f69   :: range_iter_i
+0000b790: 6e74 3634 0a20 2020 2023 2020 2064 656c  nt64.    #   del
+0000b7a0: 2024 3334 2e37 0a20 2020 2023 2020 206a   $34.7.    #   j
+0000b7b0: 756d 7020 3438 0a20 2020 2023 206c 6162  ump 48.    # lab
+0000b7c0: 656c 2034 380a 2020 2020 2320 2020 2434  el 48.    #   $4
+0000b7d0: 382e 3220 3d20 6974 6572 6e65 7874 2876  8.2 = iternext(v
+0000b7e0: 616c 7565 3d24 7068 6934 382e 3129 2020  alue=$phi48.1)  
+0000b7f0: 3a3a 2070 6169 723c 696e 7436 342c 2062  :: pair<int64, b
+0000b800: 6f6f 6c3e 0a20 2020 2023 2020 2024 3438  ool>.    #   $48
+0000b810: 2e33 203d 2070 6169 725f 6669 7273 7428  .3 = pair_first(
+0000b820: 7661 6c75 653d 2434 382e 3229 2020 3a3a  value=$48.2)  ::
+0000b830: 2069 6e74 3634 0a20 2020 2023 2020 2024   int64.    #   $
+0000b840: 3438 2e34 203d 2070 6169 725f 7365 636f  48.4 = pair_seco
+0000b850: 6e64 2876 616c 7565 3d24 3438 2e32 2920  nd(value=$48.2) 
+0000b860: 203a 3a20 626f 6f6c 0a20 2020 2023 2020   :: bool.    #  
+0000b870: 2064 656c 2024 3438 2e32 0a20 2020 2023   del $48.2.    #
+0000b880: 2020 2024 7068 6935 302e 3120 3d20 2434     $phi50.1 = $4
+0000b890: 382e 3320 203a 3a20 696e 7436 340a 2020  8.3  :: int64.  
+0000b8a0: 2020 2320 2020 2470 6869 3131 302e 3120    #   $phi110.1 
+0000b8b0: 3d20 2434 382e 3320 203a 3a20 696e 7436  = $48.3  :: int6
+0000b8c0: 340a 2020 2020 2320 2020 6465 6c20 2470  4.    #   del $p
+0000b8d0: 6869 3131 302e 310a 2020 2020 2320 2020  hi110.1.    #   
+0000b8e0: 6465 6c20 2434 382e 330a 2020 2020 2320  del $48.3.    # 
+0000b8f0: 2020 2470 6869 3131 302e 3220 3d20 2470    $phi110.2 = $p
+0000b900: 6869 3438 2e31 2020 3a3a 2072 616e 6765  hi48.1  :: range
+0000b910: 5f69 7465 725f 696e 7436 340a 2020 2020  _iter_int64.    
+0000b920: 2320 2020 6465 6c20 2470 6869 3131 302e  #   del $phi110.
+0000b930: 320a 2020 2020 2320 2020 6272 616e 6368  2.    #   branch
+0000b940: 2024 3438 2e34 2c20 3530 2c20 3131 300a   $48.4, 50, 110.
+0000b950: 2020 2020 2320 6c61 6265 6c20 3530 0a20      # label 50. 
+0000b960: 2020 2023 2020 2064 656c 2024 3438 2e34     #   del $48.4
+0000b970: 0a20 2020 2023 2020 2069 203d 2024 7068  .    #   i = $ph
+0000b980: 6935 302e 3120 203a 3a20 696e 7436 340a  i50.1  :: int64.
+0000b990: 2020 2020 2320 2020 6465 6c20 2470 6869      #   del $phi
+0000b9a0: 3530 2e31 0a0a 2020 2020 666f 7220 6920  50.1..    for i 
+0000b9b0: 696e 2070 7261 6e67 6528 6172 7261 795f  in prange(array_
+0000b9c0: 312e 7368 6170 655b 305d 293a 0a0a 2020  1.shape[0]):..  
+0000b9d0: 2020 2020 2020 2320 2d2d 2d20 4c49 4e45        # --- LINE
+0000b9e0: 2033 3534 202d 2d2d 200a 2020 2020 2020   354 --- .      
+0000b9f0: 2020 2320 2020 6a75 6d70 2035 320a 2020    #   jump 52.  
+0000ba00: 2020 2020 2020 2320 6c61 6265 6c20 3532        # label 52
+0000ba10: 0a20 2020 2020 2020 2023 2020 206a 756d  .        #   jum
+0000ba20: 7020 3534 0a20 2020 2020 2020 2023 206c  p 54.        # l
+0000ba30: 6162 656c 2035 340a 2020 2020 2020 2020  abel 54.        
+0000ba40: 2320 2020 2435 342e 3120 3d20 676c 6f62  #   $54.1 = glob
+0000ba50: 616c 2870 7261 6e67 653a 203c 636c 6173  al(prange: <clas
+0000ba60: 7320 276e 756d 6261 2e6d 6973 632e 7370  s 'numba.misc.sp
+0000ba70: 6563 6961 6c2e 7072 616e 6765 273e 2920  ecial.prange'>) 
+0000ba80: 203a 3a20 4675 6e63 7469 6f6e 283c 636c   :: Function(<cl
+0000ba90: 6173 7320 276e 756d 6261 2e6d 6973 632e  ass 'numba.misc.
+0000baa0: 7370 6563 6961 6c2e 7072 616e 6765 273e  special.prange'>
+0000bab0: 290a 2020 2020 2020 2020 2320 2020 2435  ).        #   $5
+0000bac0: 342e 3320 3d20 6765 7461 7474 7228 7661  4.3 = getattr(va
+0000bad0: 6c75 653d 6172 7261 795f 322c 2061 7474  lue=array_2, att
+0000bae0: 723d 7368 6170 6529 2020 3a3a 2055 6e69  r=shape)  :: Uni
+0000baf0: 5475 706c 6528 696e 7436 3420 7820 3229  Tuple(int64 x 2)
+0000bb00: 0a20 2020 2020 2020 2023 2020 2024 636f  .        #   $co
+0000bb10: 6e73 7435 342e 3420 3d20 636f 6e73 7428  nst54.4 = const(
+0000bb20: 696e 742c 2030 2920 203a 3a20 4c69 7465  int, 0)  :: Lite
+0000bb30: 7261 6c5b 696e 745d 2830 290a 2020 2020  ral[int](0).    
+0000bb40: 2020 2020 2320 2020 2435 342e 3520 3d20      #   $54.5 = 
+0000bb50: 7374 6174 6963 5f67 6574 6974 656d 2876  static_getitem(v
+0000bb60: 616c 7565 3d24 3534 2e33 2c20 696e 6465  alue=$54.3, inde
+0000bb70: 783d 302c 2069 6e64 6578 5f76 6172 3d24  x=0, index_var=$
+0000bb80: 636f 6e73 7435 342e 342c 2066 6e3d 3c62  const54.4, fn=<b
+0000bb90: 7569 6c74 2d69 6e20 6675 6e63 7469 6f6e  uilt-in function
+0000bba0: 2067 6574 6974 656d 3e29 2020 3a3a 2069   getitem>)  :: i
+0000bbb0: 6e74 3634 0a20 2020 2020 2020 2023 2020  nt64.        #  
+0000bbc0: 2064 656c 2024 636f 6e73 7435 342e 340a   del $const54.4.
+0000bbd0: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
+0000bbe0: 2435 342e 330a 2020 2020 2020 2020 2320  $54.3.        # 
+0000bbf0: 2020 2435 342e 3620 3d20 6361 6c6c 2024    $54.6 = call $
+0000bc00: 3534 2e31 2824 3534 2e35 2c20 6675 6e63  54.1($54.5, func
+0000bc10: 3d24 3534 2e31 2c20 6172 6773 3d5b 5661  =$54.1, args=[Va
+0000bc20: 7228 2435 342e 352c 2066 6561 7475 7265  r($54.5, feature
+0000bc30: 5f65 7874 7261 6374 696f 6e5f 6d69 7869  _extraction_mixi
+0000bc40: 6e2e 7079 3a33 3534 295d 2c20 6b77 733d  n.py:354)], kws=
+0000bc50: 2829 2c20 7661 7261 7267 3d4e 6f6e 6529  (), vararg=None)
+0000bc60: 2020 3a3a 2028 696e 7436 342c 2920 2d3e    :: (int64,) ->
+0000bc70: 2072 616e 6765 5f73 7461 7465 5f69 6e74   range_state_int
+0000bc80: 3634 0a20 2020 2020 2020 2023 2020 2064  64.        #   d
+0000bc90: 656c 2024 3534 2e35 0a20 2020 2020 2020  el $54.5.       
+0000bca0: 2023 2020 2064 656c 2024 3534 2e31 0a20   #   del $54.1. 
+0000bcb0: 2020 2020 2020 2023 2020 2024 3534 2e37         #   $54.7
+0000bcc0: 203d 2067 6574 6974 6572 2876 616c 7565   = getiter(value
+0000bcd0: 3d24 3534 2e36 2920 203a 3a20 7261 6e67  =$54.6)  :: rang
+0000bce0: 655f 6974 6572 5f69 6e74 3634 0a20 2020  e_iter_int64.   
+0000bcf0: 2020 2020 2023 2020 2064 656c 2024 3534       #   del $54
+0000bd00: 2e36 0a20 2020 2020 2020 2023 2020 2024  .6.        #   $
+0000bd10: 7068 6936 382e 3120 3d20 2435 342e 3720  phi68.1 = $54.7 
+0000bd20: 203a 3a20 7261 6e67 655f 6974 6572 5f69   :: range_iter_i
+0000bd30: 6e74 3634 0a20 2020 2020 2020 2023 2020  nt64.        #  
+0000bd40: 2064 656c 2024 3534 2e37 0a20 2020 2020   del $54.7.     
+0000bd50: 2020 2023 2020 206a 756d 7020 3638 0a20     #   jump 68. 
+0000bd60: 2020 2020 2020 2023 206c 6162 656c 2036         # label 6
+0000bd70: 380a 2020 2020 2020 2020 2320 2020 2436  8.        #   $6
+0000bd80: 382e 3220 3d20 6974 6572 6e65 7874 2876  8.2 = iternext(v
+0000bd90: 616c 7565 3d24 7068 6936 382e 3129 2020  alue=$phi68.1)  
+0000bda0: 3a3a 2070 6169 723c 696e 7436 342c 2062  :: pair<int64, b
+0000bdb0: 6f6f 6c3e 0a20 2020 2020 2020 2023 2020  ool>.        #  
+0000bdc0: 2024 3638 2e33 203d 2070 6169 725f 6669   $68.3 = pair_fi
+0000bdd0: 7273 7428 7661 6c75 653d 2436 382e 3229  rst(value=$68.2)
+0000bde0: 2020 3a3a 2069 6e74 3634 0a20 2020 2020    :: int64.     
+0000bdf0: 2020 2023 2020 2024 3638 2e34 203d 2070     #   $68.4 = p
+0000be00: 6169 725f 7365 636f 6e64 2876 616c 7565  air_second(value
+0000be10: 3d24 3638 2e32 2920 203a 3a20 626f 6f6c  =$68.2)  :: bool
+0000be20: 0a20 2020 2020 2020 2023 2020 2064 656c  .        #   del
+0000be30: 2024 3638 2e32 0a20 2020 2020 2020 2023   $68.2.        #
+0000be40: 2020 2024 7068 6937 302e 3120 3d20 2436     $phi70.1 = $6
+0000be50: 382e 3320 203a 3a20 696e 7436 340a 2020  8.3  :: int64.  
+0000be60: 2020 2020 2020 2320 2020 2470 6869 3130        #   $phi10
+0000be70: 362e 3120 3d20 2436 382e 3320 203a 3a20  6.1 = $68.3  :: 
+0000be80: 696e 7436 340a 2020 2020 2020 2020 2320  int64.        # 
+0000be90: 2020 6465 6c20 2470 6869 3130 362e 310a    del $phi106.1.
+0000bea0: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
+0000beb0: 2436 382e 330a 2020 2020 2020 2020 2320  $68.3.        # 
+0000bec0: 2020 2470 6869 3130 362e 3220 3d20 2470    $phi106.2 = $p
+0000bed0: 6869 3638 2e31 2020 3a3a 2072 616e 6765  hi68.1  :: range
+0000bee0: 5f69 7465 725f 696e 7436 340a 2020 2020  _iter_int64.    
+0000bef0: 2020 2020 2320 2020 6465 6c20 2470 6869      #   del $phi
+0000bf00: 3130 362e 320a 2020 2020 2020 2020 2320  106.2.        # 
+0000bf10: 2020 6272 616e 6368 2024 3638 2e34 2c20    branch $68.4, 
+0000bf20: 3730 2c20 3130 360a 2020 2020 2020 2020  70, 106.        
+0000bf30: 2320 6c61 6265 6c20 3730 0a20 2020 2020  # label 70.     
+0000bf40: 2020 2023 2020 2064 656c 2024 3638 2e34     #   del $68.4
+0000bf50: 0a20 2020 2020 2020 2023 2020 206a 203d  .        #   j =
+0000bf60: 2024 7068 6937 302e 3120 203a 3a20 696e   $phi70.1  :: in
+0000bf70: 7436 340a 2020 2020 2020 2020 2320 2020  t64.        #   
+0000bf80: 6465 6c20 2470 6869 3730 2e31 0a0a 2020  del $phi70.1..  
+0000bf90: 2020 2020 2020 666f 7220 6a20 696e 2070        for j in p
+0000bfa0: 7261 6e67 6528 6172 7261 795f 322e 7368  range(array_2.sh
+0000bfb0: 6170 655b 305d 293a 0a0a 2020 2020 2020  ape[0]):..      
+0000bfc0: 2020 2020 2020 2320 2d2d 2d20 4c49 4e45        # --- LINE
+0000bfd0: 2033 3535 202d 2d2d 200a 2020 2020 2020   355 --- .      
+0000bfe0: 2020 2020 2020 2320 2020 2437 302e 3220        #   $70.2 
+0000bff0: 3d20 676c 6f62 616c 286e 703a 203c 6d6f  = global(np: <mo
+0000c000: 6475 6c65 2027 6e75 6d70 7927 2066 726f  dule 'numpy' fro
+0000c010: 6d20 272f 5573 6572 732f 7369 6d6f 6e2f  m '/Users/simon/
+0000c020: 2e63 6f6e 6461 2f65 6e76 732f 7369 6d62  .conda/envs/simb
+0000c030: 615f 6465 762f 6c69 622f 7079 7468 6f6e  a_dev/lib/python
+0000c040: 332e 362f 7369 7465 2d70 6163 6b61 6765  3.6/site-package
+0000c050: 732f 6e75 6d70 792f 5f5f 696e 6974 5f5f  s/numpy/__init__
+0000c060: 2e70 7927 3e29 2020 3a3a 204d 6f64 756c  .py'>)  :: Modul
+0000c070: 6528 3c6d 6f64 756c 6520 276e 756d 7079  e(<module 'numpy
+0000c080: 2720 6672 6f6d 2027 2f55 7365 7273 2f73  ' from '/Users/s
+0000c090: 696d 6f6e 2f2e 636f 6e64 612f 656e 7673  imon/.conda/envs
+0000c0a0: 2f73 696d 6261 5f64 6576 2f6c 6962 2f70  /simba_dev/lib/p
+0000c0b0: 7974 686f 6e33 2e36 2f73 6974 652d 7061  ython3.6/site-pa
+0000c0c0: 636b 6167 6573 2f6e 756d 7079 2f5f 5f69  ckages/numpy/__i
+0000c0d0: 6e69 745f 5f2e 7079 273e 290a 2020 2020  nit__.py'>).    
+0000c0e0: 2020 2020 2020 2020 2320 2020 2437 302e          #   $70.
+0000c0f0: 3320 3d20 6765 7461 7474 7228 7661 6c75  3 = getattr(valu
+0000c100: 653d 2437 302e 322c 2061 7474 723d 6c69  e=$70.2, attr=li
+0000c110: 6e61 6c67 2920 203a 3a20 4d6f 6475 6c65  nalg)  :: Module
+0000c120: 283c 6d6f 6475 6c65 2027 6e75 6d70 792e  (<module 'numpy.
+0000c130: 6c69 6e61 6c67 2720 6672 6f6d 2027 2f55  linalg' from '/U
+0000c140: 7365 7273 2f73 696d 6f6e 2f2e 636f 6e64  sers/simon/.cond
+0000c150: 612f 656e 7673 2f73 696d 6261 5f64 6576  a/envs/simba_dev
+0000c160: 2f6c 6962 2f70 7974 686f 6e33 2e36 2f73  /lib/python3.6/s
+0000c170: 6974 652d 7061 636b 6167 6573 2f6e 756d  ite-packages/num
+0000c180: 7079 2f6c 696e 616c 672f 5f5f 696e 6974  py/linalg/__init
+0000c190: 5f5f 2e70 7927 3e29 0a20 2020 2020 2020  __.py'>).       
+0000c1a0: 2020 2020 2023 2020 2064 656c 2024 3730       #   del $70
+0000c1b0: 2e32 0a20 2020 2020 2020 2020 2020 2023  .2.            #
+0000c1c0: 2020 2024 3730 2e34 203d 2067 6574 6174     $70.4 = getat
+0000c1d0: 7472 2876 616c 7565 3d24 3730 2e33 2c20  tr(value=$70.3, 
+0000c1e0: 6174 7472 3d6e 6f72 6d29 2020 3a3a 2046  attr=norm)  :: F
+0000c1f0: 756e 6374 696f 6e28 3c66 756e 6374 696f  unction(<functio
+0000c200: 6e20 6e6f 726d 2061 7420 3078 3766 3935  n norm at 0x7f95
+0000c210: 3665 6536 6366 3238 3e29 0a20 2020 2020  6ee6cf28>).     
+0000c220: 2020 2020 2020 2023 2020 2064 656c 2024         #   del $
+0000c230: 3730 2e33 0a20 2020 2020 2020 2020 2020  70.3.           
+0000c240: 2023 2020 2024 3730 2e37 203d 2067 6574   #   $70.7 = get
+0000c250: 6974 656d 2876 616c 7565 3d61 7272 6179  item(value=array
+0000c260: 5f31 2c20 696e 6465 783d 692c 2066 6e3d  _1, index=i, fn=
+0000c270: 3c62 7569 6c74 2d69 6e20 6675 6e63 7469  <built-in functi
+0000c280: 6f6e 2067 6574 6974 656d 3e29 2020 3a3a  on getitem>)  ::
+0000c290: 2061 7272 6179 2866 6c6f 6174 3332 2c20   array(float32, 
+0000c2a0: 3164 2c20 4129 0a20 2020 2020 2020 2020  1d, A).         
+0000c2b0: 2020 2023 2020 2024 3730 2e31 3020 3d20     #   $70.10 = 
+0000c2c0: 6765 7469 7465 6d28 7661 6c75 653d 6172  getitem(value=ar
+0000c2d0: 7261 795f 322c 2069 6e64 6578 3d6a 2c20  ray_2, index=j, 
+0000c2e0: 666e 3d3c 6275 696c 742d 696e 2066 756e  fn=<built-in fun
+0000c2f0: 6374 696f 6e20 6765 7469 7465 6d3e 2920  ction getitem>) 
+0000c300: 203a 3a20 6172 7261 7928 666c 6f61 7433   :: array(float3
+0000c310: 322c 2031 642c 2041 290a 2020 2020 2020  2, 1d, A).      
+0000c320: 2020 2020 2020 2320 2020 2437 302e 3131        #   $70.11
+0000c330: 203d 2024 3730 2e37 202d 2024 3730 2e31   = $70.7 - $70.1
+0000c340: 3020 203a 3a20 6172 7261 7928 666c 6f61  0  :: array(floa
+0000c350: 7433 322c 2031 642c 2043 290a 2020 2020  t32, 1d, C).    
+0000c360: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
+0000c370: 2437 302e 370a 2020 2020 2020 2020 2020  $70.7.          
+0000c380: 2020 2320 2020 6465 6c20 2437 302e 3130    #   del $70.10
+0000c390: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0000c3a0: 2024 3730 2e31 3220 3d20 6361 6c6c 2024   $70.12 = call $
+0000c3b0: 3730 2e34 2824 3730 2e31 312c 2066 756e  70.4($70.11, fun
+0000c3c0: 633d 2437 302e 342c 2061 7267 733d 5b56  c=$70.4, args=[V
+0000c3d0: 6172 2824 3730 2e31 312c 2066 6561 7475  ar($70.11, featu
+0000c3e0: 7265 5f65 7874 7261 6374 696f 6e5f 6d69  re_extraction_mi
+0000c3f0: 7869 6e2e 7079 3a33 3535 295d 2c20 6b77  xin.py:355)], kw
+0000c400: 733d 2829 2c20 7661 7261 7267 3d4e 6f6e  s=(), vararg=Non
+0000c410: 6529 2020 3a3a 2028 6172 7261 7928 666c  e)  :: (array(fl
+0000c420: 6f61 7433 322c 2031 642c 2043 292c 206f  oat32, 1d, C), o
+0000c430: 6d69 7474 6564 2864 6566 6175 6c74 3d4e  mitted(default=N
+0000c440: 6f6e 6529 2920 2d3e 2066 6c6f 6174 3332  one)) -> float32
+0000c450: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0000c460: 2064 656c 2024 3730 2e34 0a20 2020 2020   del $70.4.     
+0000c470: 2020 2020 2020 2023 2020 2064 656c 2024         #   del $
+0000c480: 3730 2e31 310a 2020 2020 2020 2020 2020  70.11.          
+0000c490: 2020 2320 2020 2437 302e 3135 203d 2067    #   $70.15 = g
+0000c4a0: 6574 6974 656d 2876 616c 7565 3d72 6573  etitem(value=res
+0000c4b0: 756c 7473 2c20 696e 6465 783d 692c 2066  ults, index=i, f
+0000c4c0: 6e3d 3c62 7569 6c74 2d69 6e20 6675 6e63  n=<built-in func
+0000c4d0: 7469 6f6e 2067 6574 6974 656d 3e29 2020  tion getitem>)  
+0000c4e0: 3a3a 2061 7272 6179 2866 6c6f 6174 3634  :: array(float64
+0000c4f0: 2c20 3164 2c20 4329 0a20 2020 2020 2020  , 1d, C).       
+0000c500: 2020 2020 2023 2020 2024 3730 2e31 355b       #   $70.15[
+0000c510: 6a5d 203d 2024 3730 2e31 3220 203a 3a20  j] = $70.12  :: 
+0000c520: 2861 7272 6179 2866 6c6f 6174 3634 2c20  (array(float64, 
+0000c530: 3164 2c20 4329 2c20 696e 7436 342c 2066  1d, C), int64, f
+0000c540: 6c6f 6174 3332 2920 2d3e 206e 6f6e 650a  loat32) -> none.
+0000c550: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000c560: 6465 6c20 6a0a 2020 2020 2020 2020 2020  del j.          
+0000c570: 2020 2320 2020 6465 6c20 2437 302e 3135    #   del $70.15
+0000c580: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0000c590: 2064 656c 2024 3730 2e31 320a 2020 2020   del $70.12.    
+0000c5a0: 2020 2020 2020 2020 2320 2020 6a75 6d70          #   jump
+0000c5b0: 2036 380a 2020 2020 2020 2020 2020 2020   68.            
+0000c5c0: 2320 6c61 6265 6c20 3130 360a 2020 2020  # label 106.    
+0000c5d0: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
+0000c5e0: 690a 2020 2020 2020 2020 2020 2020 2320  i.            # 
+0000c5f0: 2020 6465 6c20 2470 6869 3730 2e31 0a20    del $phi70.1. 
+0000c600: 2020 2020 2020 2020 2020 2023 2020 2064             #   d
+0000c610: 656c 2024 7068 6936 382e 310a 2020 2020  el $phi68.1.    
+0000c620: 2020 2020 2020 2020 2320 2020 6465 6c20          #   del 
+0000c630: 2436 382e 340a 2020 2020 2020 2020 2020  $68.4.          
+0000c640: 2020 2320 2020 6a75 6d70 2031 3038 0a20    #   jump 108. 
+0000c650: 2020 2020 2020 2020 2020 2023 206c 6162             # lab
+0000c660: 656c 2031 3038 0a20 2020 2020 2020 2020  el 108.         
+0000c670: 2020 2023 2020 206a 756d 7020 3438 0a20     #   jump 48. 
+0000c680: 2020 2020 2020 2020 2020 2023 206c 6162             # lab
+0000c690: 656c 2031 3130 0a0a 2020 2020 2020 2020  el 110..        
+0000c6a0: 2020 2020 7265 7375 6c74 735b 695d 5b6a      results[i][j
+0000c6b0: 5d20 3d20 6e70 2e6c 696e 616c 672e 6e6f  ] = np.linalg.no
+0000c6c0: 726d 2861 7272 6179 5f31 5b69 5d20 2d20  rm(array_1[i] - 
+0000c6d0: 6172 7261 795f 325b 6a5d 290a 0a20 2020  array_2[j])..   
+0000c6e0: 2023 202d 2d2d 204c 494e 4520 3335 3620   # --- LINE 356 
+0000c6f0: 2d2d 2d20 0a20 2020 2023 2020 2064 656c  --- .    #   del
+0000c700: 2061 7272 6179 5f32 0a20 2020 2023 2020   array_2.    #  
+0000c710: 2064 656c 2061 7272 6179 5f31 0a20 2020   del array_1.   
+0000c720: 2023 2020 2064 656c 2024 7068 6935 302e   #   del $phi50.
+0000c730: 310a 2020 2020 2320 2020 6465 6c20 2470  1.    #   del $p
+0000c740: 6869 3438 2e31 0a20 2020 2023 2020 2064  hi48.1.    #   d
+0000c750: 656c 2024 3438 2e34 0a20 2020 2023 2020  el $48.4.    #  
+0000c760: 206a 756d 7020 3131 320a 2020 2020 2320   jump 112.    # 
+0000c770: 6c61 6265 6c20 3131 320a 2020 2020 2320  label 112.    # 
+0000c780: 2020 2431 3132 2e32 203d 2063 6173 7428    $112.2 = cast(
+0000c790: 7661 6c75 653d 7265 7375 6c74 7329 2020  value=results)  
+0000c7a0: 3a3a 2061 7272 6179 2866 6c6f 6174 3634  :: array(float64
+0000c7b0: 2c20 3264 2c20 4329 0a20 2020 2023 2020  , 2d, C).    #  
+0000c7c0: 2064 656c 2072 6573 756c 7473 0a20 2020   del results.   
+0000c7d0: 2023 2020 2072 6574 7572 6e20 2431 3132   #   return $112
+0000c7e0: 2e32 0a0a 2020 2020 7265 7475 726e 2072  .2..    return r
+0000c7f0: 6573 756c 7473 0a0a 945d 9428 685d 6852  esults...].(h]hR
+0000c800: 8c11 6e75 6d62 612e 6e70 2e61 7272 6179  ..numba.np.array
+0000c810: 6f62 6a94 5d94 8c58 5f5a 4e30 384e 756d  obj.]..X_ZN08Num
+0000c820: 6261 456e 7635 6e75 6d62 6132 6e70 3861  baEnv5numba2np8a
+0000c830: 7272 6179 6f62 6a31 336e 756d 7079 5f66  rrayobj13numpy_f
+0000c840: 756c 6c5f 6e64 3132 2433 636c 6f63 616c  ull_nd12$3clocal
+0000c850: 7324 3365 3966 756c 6c24 3234 3633 4538  s$3e9full$2463E8
+0000c860: 556e 6954 7570 6c65 4978 4c69 3245 4564  UniTupleIxLi2EEd
+0000c870: 9487 9452 9468 528c 106e 756d 6261 2e6e  ...R.hR..numba.n
+0000c880: 702e 6e70 7969 6d70 6c94 5d94 8c49 5f5a  p.npyimpl.]..I_Z
+0000c890: 4e30 384e 756d 6261 456e 7635 6e75 6d62  N08NumbaEnv5numb
+0000c8a0: 6132 6e70 376e 7079 696d 706c 3230 5f62  a2np7npyimpl20_b
+0000c8b0: 726f 6164 6361 7374 5f6f 6e74 6f24 3234  roadcast_onto$24
+0000c8c0: 3130 4578 3869 6e74 3634 2432 6178 3869  10Ex8int64$2ax8i
+0000c8d0: 6e74 3634 2432 6194 8794 5294 6852 8c0f  nt64$2a...R.hR..
+0000c8e0: 6e75 6d62 612e 6e70 2e6c 696e 616c 6794  numba.np.linalg.
+0000c8f0: 5d94 8c88 5f5a 4e30 384e 756d 6261 456e  ]..._ZN08NumbaEn
+0000c900: 7635 6e75 6d62 6132 6e70 366c 696e 616c  v5numba2np6linal
+0000c910: 6731 345f 6765 745f 6e6f 726d 5f69 6d70  g14_get_norm_imp
+0000c920: 6c31 3224 3363 6c6f 6361 6c73 2433 6531  l12$3clocals$3e1
+0000c930: 346f 6e65 445f 696d 706c 2432 3436 3145  4oneD_impl$2461E
+0000c940: 3541 7272 6179 4966 4c69 3145 3143 376d  5ArrayIfLi1E1C7m
+0000c950: 7574 6162 6c65 3761 6c69 676e 6564 4532  utable7alignedE2
+0000c960: 376f 6d69 7474 6564 2432 3864 6566 6175  7omitted$28defau
+0000c970: 6c74 2433 644e 6f6e 6524 3239 9487 9452  lt$3dNone$29...R
+0000c980: 9468 5268 705d 948c 685f 5a4e 3038 4e75  .hRhp]..h_ZN08Nu
+0000c990: 6d62 6145 6e76 356e 756d 6261 326e 7036  mbaEnv5numba2np6
+0000c9a0: 6c69 6e61 6c67 3137 5f6f 6e65 445f 6e6f  linalg17_oneD_no
+0000c9b0: 726d 5f32 5f69 6d70 6c31 3224 3363 6c6f  rm_2_impl12$3clo
+0000c9c0: 6361 6c73 2433 6539 696d 706c 2432 3436  cals$3e9impl$246
+0000c9d0: 3245 3541 7272 6179 4966 4c69 3145 3143  2E5ArrayIfLi1E1C
+0000c9e0: 376d 7574 6162 6c65 3761 6c69 676e 6564  7mutable7aligned
+0000c9f0: 4594 8794 5294 6852 6870 5d94 8c59 5f5a  E...R.hRhp]..Y_Z
+0000ca00: 4e30 384e 756d 6261 456e 7635 6e75 6d62  N08NumbaEnv5numb
+0000ca10: 6132 6e70 366c 696e 616c 6732 355f 6475  a2np6linalg25_du
+0000ca20: 6d6d 795f 6c69 7665 6e65 7373 5f66 756e  mmy_liveness_fun
+0000ca30: 6324 3234 3239 4533 306c 6973 7424 3238  c$2429E30list$28
+0000ca40: 696e 7436 3424 3239 2433 6369 7624 3364  int64$29$3civ$3d
+0000ca50: 4e6f 6e65 2433 6594 8794 5294 7494 7494  None$3e...R.t.t.
+0000ca60: 2e                                       .
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.60.3/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 
 class DeepEthogramImporter(ConfigReader):
 
     """
     Append DeepEthogram optical flow annotations onto featurized pose-estimation data.
 
     :param str config_path: path to SimBA project config file in Configparser format
-    :param str deep_ethogram_dir: path to folder holding DeepEthogram data files is CSV format
+    :param str data_dir: path to folder holding DeepEthogram data files is CSV format
 
     .. note::
        `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
        `Example expected input <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv>`__.
 
     Examples
     ----------
-    >>> deepethogram_importer = DeepEthogramImporter(config_path=r'MySimBAConfigPath', deep_ethogram_dir=r'MyDeepEthogramDir')
+    >>> deepethogram_importer = DeepEthogramImporter(config_path=r'MySimBAConfigPath', data_dir=r'MyDeepEthogramDir')
     >>> deepethogram_importer.run()
 
     References
     ----------
 
     .. [1] `DeepEthogram repo <https://github.com/jbohnslav/deepethogram>`__.
     .. [2] `Example DeepEthogram input file <https://github.com/sgoldenlab/simba/blob/master/misc/deep_ethogram_labels.csv>`__.
     """
 
     def __init__(self,
-                 deep_ethogram_dir: str,
+                 data_dir: str,
                  config_path: str):
 
         super().__init__(config_path=config_path)
-        self.data_dir = deep_ethogram_dir
+        self.data_dir = data_dir
         check_if_dir_exists(in_dir=self.data_dir)
         self.deepethogram_files_found = glob.glob(self.data_dir + '/*.csv')
         check_if_filepath_list_is_empty(filepaths=self.deepethogram_files_found,
                                         error_msg=f'SIMBA ERROR: ZERO DeepEthogram CSV files found in {self.data_dir} directory')
         check_if_filepath_list_is_empty(filepaths=self.feature_file_paths,
                                         error_msg='SIMBA ERROR: ZERO files found in the project_folder/csv/features_extracted directory')
         feature_file_names, self.matches_dict = [], {}
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from copy import deepcopy
 import os, glob
 from simba.mixins.config_reader import ConfigReader
+from simba.third_party_label_appenders.tools import is_new_boris_version
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 from simba.utils.checks import check_if_dir_exists, check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success
 from simba.utils.errors import (ThirdPartyAnnotationOverlapError,
                                 ThirdPartyAnnotationEventCountError)
 from simba.utils.warnings import (ThirdPartyAnnotationsOutsidePoseEstimationDataWarning,
                                   ThirdPartyAnnotationsInvalidFileFormatWarning)
 
+
 class BorisAppender(ConfigReader):
 
     """
     Append BORIS human annotations onto featurized pose-estimation data.
 
     :param str config_path: path to SimBA project config file in Configparser format
-    :param str boris_folder: path to folder holding BORIS data files is CSV format
+    :param str data_dir: path to folder holding BORIS data files is CSV format
 
     .. note::
        `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
        `Example BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv>`_.
 
     Examples
     ----------
-    >>> boris_appender = BorisAppender(config_path='MyProjectConfigPath', boris_folder=r'BorisDataFolder')
+    >>> boris_appender = BorisAppender(config_path='MyProjectConfigPath', data_dir=r'BorisDataFolder')
     >>> boris_appender.create_boris_master_file()
     >>> boris_appender.run()
 
     References
     ----------
 
     .. [1] `Behavioral Observation Research Interactive Software (BORIS) user guide <https://boris.readthedocs.io/en/latest/#>`__.
     """
 
     def __init__(self,
                  config_path: str,
-                 boris_folder: str):
+                 data_dir: str):
 
         super().__init__(config_path=config_path)
-        self.boris_dir = boris_folder
+        self.boris_dir = data_dir
         self.boris_files_found = glob.glob(self.boris_dir + '/*.csv')
-        check_if_dir_exists(boris_folder)
+        check_if_dir_exists(data_dir)
         check_if_filepath_list_is_empty(filepaths=self.boris_files_found,
-                                        error_msg=f'SIMBA ERROR: 0 BORIS CSV files found in {boris_folder} directory')
+                                        error_msg=f'SIMBA ERROR: 0 BORIS CSV files found in {data_dir} directory')
         print(f'Processing BORIS for {str(len(self.feature_file_paths))} file(s)...')
 
     def create_boris_master_file(self):
         """
         Method to create concatenated dataframe of BORIS annotations.
 
         Returns
@@ -58,18 +60,28 @@
             master_boris_df
         """
         self.master_boris_df_list = []
         for file_cnt, file_path in enumerate(self.boris_files_found):
             try:
                 _, video_name, _ = get_fn_ext(file_path)
                 boris_df = pd.read_csv(file_path)
-                index = (boris_df[boris_df['Observation id'] == "Time"].index.values)
-                boris_df = pd.read_csv(file_path, skiprows=range(0, int(index + 1)))
-                boris_df = boris_df.loc[:, ~boris_df.columns.str.contains('^Unnamed')]
-                boris_df.drop(['Behavioral category', 'Comment', 'Subject'], axis=1, inplace=True)
+                if not is_new_boris_version(boris_df):
+                    index = (boris_df[boris_df['Observation id'] == "Time"].index.values)
+                    boris_df = pd.read_csv(file_path, skiprows=range(0, int(index + 1)))
+                    boris_df = boris_df.loc[:, ~boris_df.columns.str.contains('^Unnamed')]
+                    boris_df.drop(['Behavioral category', 'Comment', 'Subject'], axis=1, inplace=True)
+                else:
+                    target_cols = ['Time', 'Media file path', 'Total length', 'FPS', 'Behavior', 'Status']
+                    boris_df.rename(columns={
+                        'Media file name': 'Media file path',
+                        'Media duration (s)': 'Total length',
+                        'Behavior type': 'Status'},
+                        inplace=True
+                    )
+                    boris_df = boris_df.reindex(columns=target_cols)
                 _, video_base_name, _ = get_fn_ext(boris_df.loc[0, 'Media file path'])
                 boris_df['Media file path'] = video_base_name
                 self.master_boris_df_list.append(boris_df)
             except Exception as e:
                 print(e.args)
                 ThirdPartyAnnotationsInvalidFileFormatWarning(annotation_app='BORIS', file_path=file_path)
         self.master_boris_df = pd.concat(self.master_boris_df_list, axis=0).reset_index(drop=True)
@@ -136,16 +148,16 @@
                 self.out_df[clf] = 0
                 self.out_df.loc[annotations_idx, clf] = 1
             self.__save_boris_annotations()
         self.timer.stop_timer()
         stdout_success(msg='BORIS annotations appended to dataset and saved in project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __save_boris_annotations(self):
-        save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
-        write_df(self.out_df, self.file_type, save_path)
+        self.save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
+        write_df(self.out_df, self.file_type, self.save_path)
         print('Saved BORIS annotations for video {}...'.format(self.video_name))
 
 # test = BorisAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                      boris_folder='/Users/simon/Downloads/FIXED')
 # test.create_boris_master_file()
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import numpy as np
 from typing import List, Dict
-
 from simba.utils.data import detect_bouts
 from simba.utils.read_write import get_fn_ext, read_video_info
 from simba.utils.enums import Methods
 from simba.utils.warnings import ThirdPartyAnnotationsInvalidFileFormatWarning
 from simba.utils.errors import (InvalidFileTypeError, ColumnNotFoundError)
 
 def observer_timestamp_corrector(timestamps: List[str]) -> List[str]:
@@ -15,34 +14,52 @@
         missing_fractions = 9 - len(s)
         if missing_fractions == 0:
             corrected_ts.append(timestamp)
         else:
             corrected_ts.append(f'{h}:{m}:{s}.{"0" * missing_fractions}')
     return corrected_ts
 
+def is_new_boris_version(pd_df: pd.DataFrame):
+    """
+    Check the format of a boris annotation file.
+
+    In the new version, additional column names are present, while
+    others have slightly different name. Here, we check for the presence
+    of a column name present only in the newer version.
+
+    :return: True if newer version
+    """
+    return 'Media file name' in list(pd_df.columns)
 
 def read_boris_annotation_files(data_paths: List[str],
                                 error_setting: str,
                                 video_info_df: pd.DataFrame,
                                 log_setting: bool=False) -> Dict[str, pd.DataFrame]:
 
     MEDIA_FILE_PATH = 'Media file path'
     OBSERVATION_ID = 'Observation id'
     TIME = 'Time'
     BEHAVIOR = 'Behavior'
     STATUS = 'Status'
-    EXPECTED_HEADERS = [TIME, MEDIA_FILE_PATH, BEHAVIOR, STATUS]
 
     dfs = {}
     for file_cnt, file_path in enumerate(data_paths):
         _, video_name, _ = get_fn_ext(file_path)
         boris_df = pd.read_csv(file_path)
         try:
-            start_idx = (boris_df[boris_df[OBSERVATION_ID] == TIME].index.values)
-            df = pd.read_csv(file_path, skiprows=range(0, int(start_idx + 1)))[EXPECTED_HEADERS]
+            if not is_new_boris_version(boris_df):
+                expected_headers = [TIME, MEDIA_FILE_PATH, BEHAVIOR, STATUS]
+                start_idx = (boris_df[boris_df[OBSERVATION_ID] == TIME].index.values)
+                df = pd.read_csv(file_path, skiprows=range(0, int(start_idx + 1)))[expected_headers]
+            else:
+                # Adjust column names to newer BORIS annotation format
+                MEDIA_FILE_PATH = 'Media file name'
+                STATUS = 'Behavior type'
+                expected_headers = [TIME, MEDIA_FILE_PATH, BEHAVIOR, STATUS]
+                df = pd.read_csv(file_path)[expected_headers]
             _, video_base_name, _ = get_fn_ext(df.loc[0, MEDIA_FILE_PATH])
             df.drop(MEDIA_FILE_PATH, axis=1, inplace=True)
             df.columns = ['TIME', 'BEHAVIOR', 'EVENT']
             df['TIME'] = df['TIME'].astype(float)
             dfs[video_base_name] = df.sort_values(by='TIME')
         except Exception as e:
             print(e)
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/ethovision_import.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,38 @@
 class ImportEthovision(ConfigReader):
     """
     Append ETHOVISION human annotations onto featurized pose-estimation data.
     Results are saved within the project_folder/csv/targets_inserted directory of
     the SimBA project (as parquets' or CSVs).
 
     :param str config_path: path to SimBA project config file in Configparser format
-    :param str folder_path: path to folder holding ETHOVISION data files is XLSX or XLS format
+    :param str data_dir: path to folder holding ETHOVISION data files is XLSX or XLS format
 
     .. note::
        `Third-party import GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
        `Example of expected ETHOVISION file <https://github.com/sgoldenlab/simba/blob/master/misc/ethovision_example.xlsx>`__.
 
     Examples
     -----
-    >>> _ = ImportEthovision(config_path="MyConfigPath", folder_path="MyEthovisionFolderPath")
+    >>> ethovision_importer = ImportEthovision(config_path="MyConfigPath", data_dir="MyEthovisionFolderPath")
+    >>> ethovision_importer.run()
     """
 
     def __init__(self,
                  config_path: str,
-                 folder_path: str):
+                 data_dir: str):
 
         super().__init__(config_path=config_path)
 
         print('Appending ETHOVISION annotations...')
         self.config = read_config_file(config_path)
-        self.files_found = glob.glob(folder_path + '/*.xlsx') + glob.glob(folder_path + '/*.xls')
+        self.files_found = glob.glob(data_dir + '/*.xlsx') + glob.glob(data_dir + '/*.xls')
         self.files_found = [x for x in self.files_found if '~$' not in x]
         check_if_filepath_list_is_empty(filepaths=self.files_found,
-                                        error_msg='SIMBA ERROR: No ETHOVISION xlsx or xls files found in {}'.format(str(folder_path)))
-        self.processed_videos = []
-        self.__read_files()
-        self.timer.stop_timer()
-        stdout_success(msg='All Ethovision annotations added. Files with annotation are located in the project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
+                                        error_msg='SIMBA ERROR: No ETHOVISION xlsx or xls files found in {}'.format(str(data_dir)))
 
     def __read_files(self):
         for file_path in self.files_found:
             ethovision_df = pd.read_excel(file_path, sheet_name=None)
             manual_scoring_sheet_name = list(ethovision_df.keys())[-1]
             ethovision_df = pd.read_excel(file_path, sheet_name=manual_scoring_sheet_name, index_col=0, header=None)
             try:
@@ -109,9 +106,17 @@
         self.__save_data()
 
     def __save_data(self):
         save_file_name = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
         write_df(self.features_df, self.file_type, save_file_name)
         print('Added Ethovision annotations for video {} ... '.format(self.video_name))
 
-#test = ImportEthovision(config_path= r"/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/project_folder/project_config.ini", folder_path=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/ethovision_data')
-# test = ImportEthovision(config_path= r"/Users/simon/Desktop/simbapypi_dev/tests/test_data/multi_animal_dlc_two_c57/project_folder/project_config.ini", folder_path=r'/Users/simon/Desktop/simbapypi_dev/tests/test_data/multi_animal_dlc_two_c57/ethovision_import')
+    def run(self):
+        self.processed_videos = []
+        self.__read_files()
+        self.timer.stop_timer()
+        stdout_success(msg='All Ethovision annotations added. Files with annotation are located in the project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
+
+
+# test = ImportEthovision(config_path= r"/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/project_folder/project_config.ini", data_dir=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/ethovision_data')
+# test = ImportEthovision(config_path= r"/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/project_folder/project_config.ini", data_dir='/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/ethovision_annotations')
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 
 
 class BentoAppender(ConfigReader):
     """
     Append BENTO annotation to SimBA featurized datasets.
 
     :param str config_path: path to SimBA project config file in Configparser format
-    :param str bento_dir: Path to folder containing BENTO data.
+    :param str data_dir: Path to folder containing BENTO data.
 
     .. note::
        `Example BENTO input file <https://github.com/sgoldenlab/simba/blob/master/misc/bento_example.annot>`_.
 
        'GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`_.
 
     Examples
     ----------
     >>> bento_dir = 'tests/test_data/bento_example'
     >>> config_path = 'tests/test_data/import_tests/project_folder/project_config.ini'
-    >>> bento_appender = BentoAppender(config_path=config_path, bento_dir=bento_dir)
+    >>> bento_appender = BentoAppender(config_path=config_path, data_dir=bento_dir)
     >>> bento_appender.run()
 
     References
     ----------
 
     .. [1] Segalin et al., eLife, https://doi.org/10.7554/eLife.63720
     """
 
     def __init__(self,
                  config_path: str,
-                 bento_dir: str):
+                 data_dir: str):
 
         ConfigReader.__init__(self, config_path=config_path)
-        self.bento_dir = bento_dir
+        self.bento_dir = data_dir
         self.feature_files = glob.glob(self.features_dir + '/*.' + self.file_type)
         self.bento_files = glob.glob(self.bento_dir + '/*.' + 'annot')
         check_if_filepath_list_is_empty(filepaths=self.feature_files, error_msg='SIMBA ERROR: No feature files found in project_folder/csv/features_extracted. Extract Features BEFORE appending BENTO annotations')
         check_if_filepath_list_is_empty(filepaths=self.bento_files, error_msg=f'SIMBA ERROR: No BENTO files with .annot extension found in {self.bento_dir}.')
         self.saved_files = []
 
     def run(self):
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/third_party_label_appenders/solomon_importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 from copy import deepcopy
 
+import pandas as pd
+
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_that_column_exist, check_if_filepath_list_is_empty
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.mixins.config_reader import ConfigReader
 
 class SolomonImporter(ConfigReader):
     """
     Append SOLOMON human annotations onto featurized pose-estimation data.
 
     :param str config_path: path to SimBA project config file in Configparser format
-    :param str solomon_dir: path to folder holding SOLOMON data files is CSV format
+    :param str data_dir: path to folder holding SOLOMON data files is CSV format
 
     .. note::
        `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
        `Example of expected SOLOMON file format <https://github.com/sgoldenlab/simba/blob/master/misc/solomon_example.csv>`__.
 
     Examples
     ----------
-    >>> solomon_imported = SolomonImporter(config_path=r'MySimBAConfigPath', solomon_dir=r'MySolomonDir')
-    >>> solomon_imported.import_solomon()
+    >>> solomon_imported = SolomonImporter(config_path=r'MySimBAConfigPath', data_dir=r'MySolomonDir')
+    >>> solomon_imported.run()
 
     References
     ----------
 
     .. [1] `SOLOMON CODER USER-GUIDE (PDF) <https://solomon.andraspeter.com/Solomon%20Intro.pdf>`__.
     """
 
     def __init__(self,
                  config_path: str,
-                 solomon_dir: str):
+                 data_dir: str):
+
         super().__init__(config_path=config_path)
-        self.solomon_paths = glob.glob(solomon_dir + '/*.csv')
+        self.solomon_paths = glob.glob(data_dir + '/*.csv')
         check_if_filepath_list_is_empty(filepaths=self.solomon_paths,
-                                        error_msg=f'SIMBA ERROR: No CSV files detected in SOLOMON directory {solomon_dir}')
+                                        error_msg=f'SIMBA ERROR: No CSV files detected in SOLOMON directory {data_dir}')
         check_if_filepath_list_is_empty(filepaths=self.feature_file_paths,
                                         error_msg=f'SIMBA ERROR: No CSV files detected in feature directory {self.features_dir}')
         if not os.path.exists(self.targets_folder): os.mkdir(self.targets_folder)
 
-    def import_solomon(self):
+    def run(self):
         for file_cnt, file_path in enumerate(self.solomon_paths):
             _, file_name, _ = get_fn_ext(file_path)
             feature_file_path = os.path.join(self.features_dir, file_name + '.' + self.file_type)
             _, _, fps = self.read_video_info(video_name=file_name)
             if not os.path.isfile(feature_file_path):
                 print('SIMBA WARNING: Data for video {} does not exist in the features directory. SimBA will SKIP appending annotations for video {}'.format(file_name, file_name))
                 continue
             save_path = os.path.join(self.targets_folder, file_name + '.' + self.file_type)
-            solomon_df = read_df(file_path, self.file_type).reset_index()
+            solomon_df = pd.read_csv(file_path)
             check_that_column_exist(df=solomon_df, column_name='Behaviour', file_name=file_path)
             features_df = read_df(feature_file_path, self.file_type)
             out_df = deepcopy(features_df)
             features_frames = list(features_df.index)
             solomon_df['frame_cnt'] = solomon_df.index
             for clf_name in self.clf_names:
                 target_col = list(solomon_df.columns[solomon_df.isin([clf_name]).any()])
@@ -75,13 +78,13 @@
                 out_df[clf_name] = 0
                 out_df.loc[target_frm_list, clf_name] = 1
 
             write_df(out_df, self.file_type, save_path)
             print('Solomon annotations appended for video {}...'.format(file_name))
         stdout_success(msg='All SOLOMON annotations imported. Data saved in the project_folder/csv/targets_inserted directory of the SimBA project')
 
-# test = SolomonImporter(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/project_folder/project_config.ini',
-#                        solomon_dir='/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/solomon_data')
+# test = SolomonImporter(config_path='/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/project_folder/project_config.ini',
+#                        data_dir='/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/solomon_annotations')
 #
-# test.import_solomon()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.60.3/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/enums.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/utils/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
-00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
+00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
+00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000e  ................
-00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
-00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
+00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
+00000050: 0000 0001 0000 1000 7370 626c 6f62 0000  ........spblob..
+00000060: 00ca 6270 0000 0000 0000 0000 0000 0000  ..bp............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,144 +250,144 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
-00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0001 c47b 0000 000b 005f 005f 0070  .....{....._._.p
-00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 27d0 9c79  moDDblob....'..y
-00001060: 4c04 c541 0000 000b 005f 005f 0070 0079  L..A....._._.p.y
-00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 a48d 7b10 0d04  dDblob......{...
-00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0002 0000 0000 0003  comp............
-000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
-000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001130: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00001140: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00001150: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
-00001160: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-00001170: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-00001180: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00001190: 0000 0000 0000 0000 0000 009b 0000 0003  ................
-000011a0: 0063 006c 0069 6c67 3153 636f 6d70 0000  .c.l.ilg1Scomp..
-000011b0: 0000 0000 10fa 0000 0003 0063 006c 0069  ...........c.l.i
-000011c0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
-000011d0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-000011e0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
-000011f0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001200: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001210: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00001220: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001230: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00001240: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00001250: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00001260: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
-00001270: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-00001280: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-00001290: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-000012a0: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
-000012b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-000012c0: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
-000012d0: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
-000012e0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-000012f0: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
-00001300: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
-00001310: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
-00001320: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
-00001330: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
-00001340: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
-00001350: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
-00001360: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
-00001370: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-00001380: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
-00001390: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-000013a0: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
-000013b0: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
-000013c0: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
-000013d0: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
-000013e0: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
-000013f0: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
-00001400: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
-00001410: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
-00001420: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
-00001430: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
-00001440: da01 db00 0000 0000 0002 0100 0000 0000  ................
-00001450: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00001460: 0001 dd00 0000 0300 6300 6c00 696c 7376  ........c.l.ilsv
-00001470: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-00001480: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
-00001490: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
-000014a0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-000014b0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-000014c0: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-000014d0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-000014e0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000014f0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001500: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-00001510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00001520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00001530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00001540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00001550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00001560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-00001570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-00001580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00001590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-000015a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-000015b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-000015c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-000015d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-000015e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-000015f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00001600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00001610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00001620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00001630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00001640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00001650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00001660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00001670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00001680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00001690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-000016a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-000016b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-000016c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-000016d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-000016e0: 696d 6f44 4462 6c6f 6200 0000 0835 ca16  imoDDblob....5..
-000016f0: bc91 04c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00001700: 6f64 4462 6c6f 6200 0000 0835 ca16 bc91  odDblob....5....
-00001710: 04c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00001720: 5363 6f6d 7000 0000 0000 0020 0000 0000  Scomp...... ....
-00001730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00001740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-00001750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-00001760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-00001770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-00001780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-00001790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-000017a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-000017b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-000017c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-000017d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-000017e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-000017f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00001800: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
-00001810: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
+00001000: 0000 0000 0000 0000 0000 000a 0000 0003  ................
+00001010: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
+00001020: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00001030: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00001040: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00001050: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00001060: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001070: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001080: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00001090: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+000010a0: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
+000010b0: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
+000010c0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+000010d0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+000010e0: 0000 0000 0000 0000 0000 009b 0000 0003  ................
+000010f0: 0063 006c 0069 6c67 3153 636f 6d70 0000  .c.l.ilg1Scomp..
+00001100: 0000 0000 0c9b 0000 0003 0063 006c 0069  ...........c.l.i
+00001110: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
+00001120: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00001130: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
+00001140: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001150: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001160: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00001170: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00001180: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001190: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+000011a0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000011b0: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
+000011c0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+000011d0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+000011e0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+000011f0: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
+00001200: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00001210: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
+00001220: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
+00001230: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00001240: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
+00001250: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
+00001260: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
+00001270: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
+00001280: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
+00001290: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
+000012a0: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
+000012b0: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
+000012c0: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+000012d0: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
+000012e0: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+000012f0: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
+00001300: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
+00001310: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
+00001320: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
+00001330: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
+00001340: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
+00001350: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
+00001360: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
+00001370: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
+00001380: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
+00001390: da01 db00 0000 0000 0002 0100 0000 0000  ................
+000013a0: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
+000013b0: 0001 dd00 0000 0300 6300 6c00 696c 7376  ........c.l.ilsv
+000013c0: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+000013d0: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
+000013e0: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
+000013f0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00001400: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00001410: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00001420: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00001430: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00001440: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001450: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
+00001460: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
+00001470: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
+00001480: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
+00001490: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+000014a0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+000014b0: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
+000014c0: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
+000014d0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+000014e0: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
+000014f0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
+00001500: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
+00001510: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
+00001520: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
+00001530: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
+00001540: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
+00001550: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
+00001560: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
+00001570: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
+00001580: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
+00001590: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
+000015a0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
+000015b0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
+000015c0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
+000015d0: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
+000015e0: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
+000015f0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
+00001600: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
+00001610: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+00001620: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
+00001630: 696d 6f44 4462 6c6f 6200 0000 0855 3191  imoDDblob....U1.
+00001640: f9a1 0cc5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
+00001650: 6f64 4462 6c6f 6200 0000 0855 3191 f9a1  odDblob....U1...
+00001660: 0cc5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
+00001670: 5363 6f6d 7000 0000 0000 0010 0000 0000  Scomp...........
+00001680: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
+00001690: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
+000016a0: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
+000016b0: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
+000016c0: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
+000016d0: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
+000016e0: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
+000016f0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
+00001700: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
+00001710: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
+00001720: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
+00001730: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
+00001740: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
+00001750: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
+00001760: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
+00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
+00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -442,200 +442,72 @@
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00001c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00001c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
+00001c60: 0100 0008 0000 0000 0000 0000 0100 0020  ............... 
+00001c70: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
+00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
+00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
+00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
+00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
+00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
+00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
+00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
+00001cf0: 0000 0000 0140 0000 0000 0000 00d4 1617  .....@..........
+00001d00: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
+00001d10: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
+00001d20: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
+00001d30: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
+00001d40: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
+00001d50: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
+00001d60: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
+00001d70: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
+00001d80: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
+00001d90: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
+00001da0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
+00001db0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
+00001dc0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
+00001dd0: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
+00001de0: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
+00001df0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
+00001e00: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
+00001e10: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+00001e20: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
+00001e30: 696d 6f44 4462 6c6f 6200 0000 0855 3191  imoDDblob....U1.
+00001e40: f9a1 0cc5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
+00001e50: 6f64 4462 6c6f 6200 0000 0855 3191 f9a1  odDblob....U1...
+00001e60: 0cc5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
+00001e70: 5363 6f6d 7000 0000 0000 0010 0000 0000  Scomp...........
+00001e80: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
+00001e90: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
+00001ea0: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
+00001eb0: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
+00001ec0: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
+00001ed0: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
+00001ee0: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
+00001ef0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
+00001f00: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
+00001f10: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
+00001f20: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
+00001f30: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
+00001f40: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
+00001f50: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
+00001f60: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0003 0000 0000 0000 200b  .............. .
-00002010: 0000 0045 0000 100c 0000 0000 0000 0000  ...E............
-00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00002410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
-00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00002440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00002450: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00002460: 0200 0008 0000 0028 0000 0000 0100 0030  .......(.......0
-00002470: 0000 0000 0000 0000 0100 0040 0000 0000  ...........@....
-00002480: 0100 0080 0000 0000 0100 0100 0000 0000  ................
-00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
-000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
-000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
-000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
-000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
-000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
-000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0073 696f 6e23 4030 0000 0000 0000 09d9  .sion#@0........
-00002510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00002520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00002530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00002540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00002550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00002560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-00002570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-00002580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00002590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-000025a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-000025b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-000025c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-000025d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-000025e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-000025f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00002600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00002610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00002620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00002630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00002640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00002650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00002660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00002670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00002680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00002690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-000026a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-000026b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-000026c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-000026d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-000026e0: 696d 6f44 4462 6c6f 6200 0000 0835 ca16  imoDDblob....5..
-000026f0: bc91 04c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00002700: 6f64 4462 6c6f 6200 0000 0835 ca16 bc91  odDblob....5....
-00002710: 04c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00002720: 5363 6f6d 7000 0000 0000 0020 0000 0000  Scomp...... ....
-00002730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00002740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-00002750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-00002760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-00002770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-00002780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-00002790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-000027a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-000027b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-000027c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-000027d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-000027e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-000027f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00002800: 0b00 7700                                ..w.
+00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/checks.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/read_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,26 +39,28 @@
                                 check_if_filepath_list_is_empty)
 
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
 def read_df(file_path: Union[str, os.PathLike],
             file_type: Union[str, os.PathLike],
+            has_index: Optional[bool] = True,
             remove_columns: Optional[List[str]] = None,
             usecols: Optional[List[str]] = None,
             check_multiindex: bool = False) -> pd.DataFrame:
 
     """
     Read single tabular data file.
 
     .. note::
        For improved runtime, defaults to :external:py:meth:`pyarrow.csv.write_cs` if file type is ``csv``.
 
     :parameter str file_path: Path to data file
     :parameter str file_type: Path to data file. OPTIONS: 'parquet', 'csv', 'pickle'.
+    :parameter Optional[bool]: If the input file has an initial index column. Default: True.
     :parameter Optional[List[str]] remove_columns: If not None, then remove columns in lits.
     :parameter Optional[List[str]] usecols: If not None, then keep columns in list.
     :parameter bool check_multiindex: check file is multi-index headers. Default: False.
     :return pd.DataFrame
 
     :example:
     >>> read_df(file_path='project_folder/csv/input_csv/Video_1.csv', file_type='csv', check_multiindex=True)
@@ -70,15 +72,19 @@
             duplicate_headers = list(set([x for x in df.column_names if df.column_names.count(x) > 1]))
             if len(duplicate_headers) > 0:
                 new_headers = [duplicate_headers[0] + f'_{x}' for x in range(len(df.column_names))]
                 df = df.rename_columns(new_headers)
             df = df.to_pandas().iloc[:, 1:]
             if check_multiindex:
                 header_col_cnt = get_number_of_header_columns_in_df(df=df)
-                df = df.drop(df.index[list(range(0, header_col_cnt))]).apply(pd.to_numeric).reset_index(drop=True)
+                df = df.drop(df.index[list(range(0, header_col_cnt))]).apply(pd.to_numeric)
+            if not has_index:
+                df = df.reset_index()
+            else:
+                df = df.reset_index(drop=True)
             df = df.astype(np.float32)
         except Exception as e:
             print(e, e.args)
             raise InvalidFileTypeError(msg=f'{file_path} is not a valid CSV file')
         if remove_columns:
             df = df[df.columns[~df.columns.isin(remove_columns)]]
         if usecols:
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/errors.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/data.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/utils/printing.py` & `Simba-UW-tf-dev-1.60.3/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.60.3/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.60.3/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.60.3/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.60.3/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.60.3/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.60.3/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.60.3/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.60.3/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.60.3/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.60.3/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.60.3/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.60.3/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.3/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/SimBA.py` & `Simba-UW-tf-dev-1.60.3/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,42 +578,43 @@
 
     def train_multiple_models_from_meta(self, config_path=None):
         model_trainer = GridSearchRandomForestClassifier(config_path=config_path)
         model_trainer.run()
 
     def importBoris(self):
         ann_folder = askdirectory()
-        boris_appender = BorisAppender(config_path=self.config_path, boris_folder=ann_folder)
+        boris_appender = BorisAppender(config_path=self.config_path, data_dir=ann_folder)
         boris_appender.create_boris_master_file()
         boris_appender.run()
 
     def importSolomon(self):
         ann_folder = askdirectory()
         solomon_importer = SolomonImporter(config_path=self.config_path,
-                                           solomon_dir=ann_folder)
-        solomon_importer.import_solomon()
+                                           data_dir=ann_folder)
+        solomon_importer.run()
 
     def import_ethovision(self):
         ann_folder = askdirectory()
-        ImportEthovision(config_path=self.config_path, folder_path=ann_folder)
+        ethovision_importer = ImportEthovision(config_path=self.config_path, data_dir=ann_folder)
+        ethovision_importer.run()
 
     def import_deepethogram(self):
         ann_folder = askdirectory()
-        deepethogram_importer = DeepEthogramImporter(config_path=self.config_path, deep_ethogram_dir=ann_folder)
+        deepethogram_importer = DeepEthogramImporter(config_path=self.config_path, data_dir=ann_folder)
         deepethogram_importer.run()
 
     def import_noldus_observer(self):
         directory = askdirectory()
         noldus_observer_importer = NoldusObserverImporter(config_path=self.config_path, data_dir=directory)
         noldus_observer_importer.run()
 
     def importMARS(self):
         bento_dir = askdirectory()
         bento_appender = BentoAppender(config_path=self.config_path,
-                                       bento_dir=bento_dir)
+                                       data_dir=bento_dir)
         bento_appender.run()
 
     def choose_animal_bps(self):
         if hasattr(self, 'path_plot_animal_bp_frm'):
             self.path_plot_animal_bp_frm.destroy()
         self.path_plot_animal_bp_frm = LabelFrame(self.path_plot_frm, text='CHOOSE ANIMAL BODY-PARTS',font=('Helvetica',10,'bold'), pady=5, padx=5)
         self.path_plot_bp_dict = {}
```

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.60.3/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.3/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.60.3/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.60.3/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.60.3/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.60.3/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.60.3/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.60.3/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.3/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.60.3/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.60.3/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.60.3/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.2
+Version: 1.60.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 Simba_UW_tf_dev.egg-info/PKG-INFO
 Simba_UW_tf_dev.egg-info/SOURCES.txt
 Simba_UW_tf_dev.egg-info/dependency_links.txt
 Simba_UW_tf_dev.egg-info/entry_points.txt
 Simba_UW_tf_dev.egg-info/requires.txt
 Simba_UW_tf_dev.egg-info/top_level.txt
@@ -158,21 +159,14 @@
 simba/feature_extractors/.idea/encodings.xml
 simba/feature_extractors/.idea/features_scripts.iml
 simba/feature_extractors/.idea/misc.xml
 simba/feature_extractors/.idea/modules.xml
 simba/feature_extractors/.idea/workspace.xml
 simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
 simba/feature_extractors/.idea/libraries/R_User_Library.xml
-simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
-simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
-simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
-simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
-simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
-simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
-simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
 simba/feature_extractors/misc/.DS_Store
 simba/feature_extractors/misc/add_probability_cnt_features.py
 simba/feature_extractors/misc/convex_hull_3_scratch_3.py
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/doctests.py
@@ -204,30 +198,19 @@
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/plotting_mixin.py
 simba/mixins/pop_up_mixin.py
 simba/mixins/pose_importer_mixin.py
 simba/mixins/train_model_mixin.py
 simba/mixins/unsupervised_mixin.py
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
-simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+simba/model/.DS_Store
 simba/model/grid_search_rf.py
 simba/model/inference_batch.py
 simba/model/inference_validation.py
 simba/model/train_rf.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
@@ -440,8 +423,18 @@
 simba/video_processors/batch_process_create_ffmpeg_commands.py
 simba/video_processors/batch_process_menus.py
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
-simba/video_processors/video_processing.py
+simba/video_processors/video_processing.py
+test/__init__.py
+test/test_featurizers.py
+test/test_thirdparty_appenders.py
+test/data/__init__.py
+test/data/test_projects/__init__.py
+test/data/test_projects/mouse_open_field/__init__.py
+test/data/test_projects/two_c57/__init__.py
+test/data/test_projects/zebrafish/__init__.py
+test/data/test_projects/zebrafish/feature_file/__init__.py
+test/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
```

### Comparing `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.60.3/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/LICENSE.md` & `Simba-UW-tf-dev-1.60.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/README.md` & `Simba-UW-tf-dev-1.60.3/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.2/setup.py` & `Simba-UW-tf-dev-1.60.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.60.2",
+    version="1.60.3",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

